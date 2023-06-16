# Comparing `tmp/summa_embed-0.17.1.tar.gz` & `tmp/summa_embed-0.17.2.tar.gz`

## Comparing `summa_embed-0.17.1.tar` & `summa_embed-0.17.2.tar`

### file list

```diff
@@ -1,113 +1,127 @@
--rw-r--r--   0        0        0     2167 1970-01-01 00:00:00.000000 summa_embed-0.17.1/local_dependencies/summa-core/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/LICENSE
--rw-r--r--   0      501       20   370551 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/dictionaries/drugs.csv
--rw-r--r--   0      501       20       92 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/collectors/mod.rs
--rw-r--r--   0      501       20     7233 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
--rw-r--r--   0      501       20     2107 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/custom_serializer.rs
--rw-r--r--   0      501       20     5297 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/default_tokenizers.rs
--rw-r--r--   0      501       20     1021 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/driver.rs
--rw-r--r--   0      501       20    13794 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/fruit_extractors.rs
--rw-r--r--   0      501       20    24321 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/index_holder.rs
--rw-r--r--   0      501       20    13903 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/index_registry.rs
--rw-r--r--   0      501       20    14323 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/index_writer_holder.rs
--rw-r--r--   0      501       20     1694 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
--rw-r--r--   0      501       20      144 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/merge_policies/mod.rs
--rw-r--r--   0      501       20     2045 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
--rw-r--r--   0      501       20     5057 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/mod.rs
--rw-r--r--   0      501       20     4711 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/queries/exists_query.rs
--rw-r--r--   0      501       20       54 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/queries/mod.rs
--rw-r--r--   0      501       20      239 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/query_parser/mod.rs
--rw-r--r--   0      501       20      615 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs
--rw-r--r--   0      501       20     1376 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/query_parser/morphology/english_nn.rs
--rw-r--r--   0      501       20      847 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs
--rw-r--r--   0      501       20     2131 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs
--rw-r--r--   0      501       20    15903 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
--rw-r--r--   0      501       20     1695 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
--rw-r--r--   0      501       20    64149 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
--rw-r--r--   0      501       20     6095 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs
--rw-r--r--   0      501       20     1039 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/query_parser/utils.rs
--rw-r--r--   0      501       20     2216 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/segment_attributes.rs
--rw-r--r--   0      501       20     1901 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/snippet_generator.rs
--rw-r--r--   0      501       20    11274 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/summa_document.rs
--rw-r--r--   0      501       20     7462 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/components/summa_tokenizer.rs
--rw-r--r--   0      501       20     2162 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/configs/config_proxy.rs
--rw-r--r--   0      501       20     4680 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/configs/core.rs
--rw-r--r--   0      501       20     3512 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/configs/file_proxy.rs
--rw-r--r--   0      501       20      383 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/configs/mod.rs
--rw-r--r--   0      501       20     3335 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/configs/partial_proxy.rs
--rw-r--r--   0      501       20     8009 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/directories/byte_range_cache.rs
--rw-r--r--   0      501       20     8014 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/directories/caching_directory.rs
--rw-r--r--   0      501       20     7015 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
--rw-r--r--   0      501       20     5258 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/directories/external_requests.rs
--rw-r--r--   0      501       20    17667 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
--rw-r--r--   0      501       20     2255 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/directories/mod.rs
--rw-r--r--   0      501       20     6756 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/directories/network_directory.rs
--rw-r--r--   0      501       20     5192 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/errors.rs
--rw-r--r--   0      501       20     2421 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/hyper_external_request.rs
--rw-r--r--   0      501       20      742 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/lib.rs
--rw-r--r--   0      501       20     1471 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/metrics/cache_metrics.rs
--rw-r--r--   0      501       20      960 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/metrics/label.rs
--rw-r--r--   0      501       20       92 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/metrics/mod.rs
--rw-r--r--   0      501       20      583 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/page_rank.rs
--rw-r--r--   0      501       20     5474 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/proto_traits/aggregation.rs
--rw-r--r--   0      501       20     2294 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/proto_traits/compression.rs
--rw-r--r--   0      501       20     1068 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
--rw-r--r--   0      501       20      323 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      662 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/proto_traits/order.rs
--rw-r--r--   0      501       20      582 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/proto_traits/snippet.rs
--rw-r--r--   0      501       20      411 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
--rw-r--r--   0      501       20     2048 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/scorers/eval_scorer.rs
--rw-r--r--   0      501       20     1538 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
--rw-r--r--   0      501       20      826 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
--rw-r--r--   0      501       20      218 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/scorers/mod.rs
--rw-r--r--   0      501       20      480 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
--rw-r--r--   0      501       20     7908 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
--rw-r--r--   0      501       20      415 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/utils/mod.rs
--rw-r--r--   0      501       20      309 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/utils/random.rs
--rw-r--r--   0      501       20     3165 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/utils/sync.rs
--rw-r--r--   0      501       20      450 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-core/src/validators.rs
--rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.17.1/local_dependencies/summa-proto/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-proto/LICENSE
--rw-r--r--   0      501       20     2381 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-proto/build.rs
--rwxr-xr-x   0      501       20      244 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-proto/gen-docs.sh
--rw-r--r--   0      501       20     2561 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-proto/markdown.tmpl
--rw-r--r--   0      501       20        0 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-proto/proto/__init__.py
--rw-r--r--   0      501       20     1556 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-proto/proto/consumer_service.proto
--rw-r--r--   0      501       20      393 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-proto/proto/dag_pb.proto
--rw-r--r--   0      501       20    10274 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-proto/proto/index_service.proto
--rw-r--r--   0      501       20     7871 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-proto/proto/query.proto
--rw-r--r--   0      501       20      499 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-proto/proto/reflection_service.proto
--rw-r--r--   0      501       20      867 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-proto/proto/search_service.proto
--rw-r--r--   0      501       20      407 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-proto/proto/unixfs.proto
--rw-r--r--   0      501       20       96 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-proto/proto/utils.proto
--rw-r--r--   0      501       20     2523 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-proto/src/lib.rs
--rw-r--r--   0      501       20     2683 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-proto/src/proto_traits/collector.rs
--rw-r--r--   0      501       20      212 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-proto/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      394 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-proto/src/proto_traits/query.rs
--rw-r--r--   0      501       20      613 2023-06-14 13:27:57.000000 summa_embed-0.17.1/local_dependencies/summa-proto/src/proto_traits/score.rs
--rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 summa_embed-0.17.1/Cargo.toml
--rw-r--r--   0      501       20      685 2023-06-14 13:27:57.000000 summa_embed-0.17.1/.gitignore
--rwxr-xr-x   0      501       20      347 2023-06-14 13:27:57.000000 summa_embed-0.17.1/build.sh
--rw-r--r--   0      501       20      515 2023-06-14 13:27:57.000000 summa_embed-0.17.1/pyproject.toml
--rw-r--r--   0      501       20       29 2023-06-14 13:27:57.000000 summa_embed-0.17.1/requirements.txt
--rw-r--r--   0      501       20     4646 2023-06-14 13:27:57.000000 summa_embed-0.17.1/src/lib.rs
--rw-r--r--   0      501       20     3340 2023-06-14 13:27:57.000000 summa_embed-0.17.1/summa_embed/__init__.py
--rw-r--r--   0      501       20        0 2023-06-14 13:27:57.000000 summa_embed-0.17.1/summa_embed/proto/__init__.py
--rw-r--r--   0      501       20     3124 2023-06-14 13:27:57.000000 summa_embed-0.17.1/summa_embed/proto/consumer_service_pb2.py
--rw-r--r--   0      501       20     3153 2023-06-14 13:27:57.000000 summa_embed-0.17.1/summa_embed/proto/consumer_service_pb2.pyi
--rw-r--r--   0      501       20     1336 2023-06-14 13:27:57.000000 summa_embed-0.17.1/summa_embed/proto/dag_pb_pb2.py
--rw-r--r--   0      501       20     1115 2023-06-14 13:27:57.000000 summa_embed-0.17.1/summa_embed/proto/dag_pb_pb2.pyi
--rw-r--r--   0      501       20    16738 2023-06-14 13:27:57.000000 summa_embed-0.17.1/summa_embed/proto/index_service_pb2.py
--rw-r--r--   0      501       20    20160 2023-06-14 13:27:57.000000 summa_embed-0.17.1/summa_embed/proto/index_service_pb2.pyi
--rw-r--r--   0      501       20    24455 2023-06-14 13:27:57.000000 summa_embed-0.17.1/summa_embed/proto/query_pb2.py
--rw-r--r--   0      501       20    33178 2023-06-14 13:27:57.000000 summa_embed-0.17.1/summa_embed/proto/query_pb2.pyi
--rw-r--r--   0      501       20     2214 2023-06-14 13:27:57.000000 summa_embed-0.17.1/summa_embed/proto/reflection_service_pb2.py
--rw-r--r--   0      501       20     1996 2023-06-14 13:27:57.000000 summa_embed-0.17.1/summa_embed/proto/reflection_service_pb2.pyi
--rw-r--r--   0      501       20     2012 2023-06-14 13:27:57.000000 summa_embed-0.17.1/summa_embed/proto/search_service_pb2.py
--rw-r--r--   0      501       20     1903 2023-06-14 13:27:57.000000 summa_embed-0.17.1/summa_embed/proto/search_service_pb2.pyi
--rw-r--r--   0      501       20     1742 2023-06-14 13:27:57.000000 summa_embed-0.17.1/summa_embed/proto/unixfs_pb2.py
--rw-r--r--   0      501       20     1653 2023-06-14 13:27:57.000000 summa_embed-0.17.1/summa_embed/proto/unixfs_pb2.pyi
--rw-r--r--   0      501       20     1041 2023-06-14 13:27:57.000000 summa_embed-0.17.1/summa_embed/proto/utils_pb2.py
--rw-r--r--   0      501       20      455 2023-06-14 13:27:57.000000 summa_embed-0.17.1/summa_embed/proto/utils_pb2.pyi
--rw-r--r--   0      501       20   115919 2023-06-14 13:28:23.000000 summa_embed-0.17.1/Cargo.lock
--rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.17.1/PKG-INFO
+-rw-r--r--   0        0        0     2167 1970-01-01 00:00:00.000000 summa_embed-0.17.2/local_dependencies/summa-core/Cargo.toml
+-rw-rw-r--   0     1000     1000     1050 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/LICENSE
+-rw-rw-r--   0     1000     1000   370551 2023-06-10 14:42:19.000000 summa_embed-0.17.2/local_dependencies/summa-core/dictionaries/drugs.csv
+-rw-rw-r--   0     1000     1000       92 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/collectors/mod.rs
+-rw-rw-r--   0     1000     1000     7233 2023-06-10 14:42:19.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
+-rw-rw-r--   0     1000     1000     2107 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/custom_serializer.rs
+-rw-rw-r--   0     1000     1000     5297 2023-06-11 15:20:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/default_tokenizers.rs
+-rw-rw-r--   0     1000     1000     1021 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/driver.rs
+-rw-rw-r--   0     1000     1000    13794 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/fruit_extractors.rs
+-rw-rw-r--   0     1000     1000    24321 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/index_holder.rs
+-rw-rw-r--   0     1000     1000    13903 2023-06-14 08:03:09.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/index_registry.rs
+-rw-rw-r--   0     1000     1000    14323 2023-06-08 17:10:59.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/index_writer_holder.rs
+-rw-rw-r--   0     1000     1000     1694 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
+-rw-rw-r--   0     1000     1000      144 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/merge_policies/mod.rs
+-rw-rw-r--   0     1000     1000     2045 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
+-rw-rw-r--   0     1000     1000     5057 2023-06-10 14:42:19.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/mod.rs
+-rw-rw-r--   0     1000     1000     4711 2023-06-01 07:26:24.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/queries/exists_query.rs
+-rw-rw-r--   0     1000     1000       54 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/queries/mod.rs
+-rw-rw-r--   0     1000     1000      239 2023-06-10 14:42:19.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/mod.rs
+-rw-rw-r--   0     1000     1000      615 2023-06-10 14:42:19.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs
+-rw-rw-r--   0     1000     1000     1376 2023-06-11 17:57:08.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/morphology/english_nn.rs
+-rw-rw-r--   0     1000     1000      847 2023-06-11 17:57:08.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs
+-rw-rw-r--   0     1000     1000     2131 2023-06-11 14:16:30.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs
+-rw-rw-r--   0     1000     1000    15903 2023-06-11 14:05:01.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
+-rw-rw-r--   0     1000     1000     1695 2023-06-10 14:42:19.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
+-rw-rw-r--   0     1000     1000    64254 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
+-rw-rw-r--   0     1000     1000     6095 2023-06-13 12:10:55.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs
+-rw-rw-r--   0     1000     1000     1039 2023-06-10 14:42:19.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/utils.rs
+-rw-rw-r--   0     1000     1000     2216 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/segment_attributes.rs
+-rw-rw-r--   0     1000     1000     1901 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/snippet_generator.rs
+-rw-rw-r--   0     1000     1000    11274 2023-06-01 07:26:30.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/summa_document.rs
+-rw-rw-r--   0     1000     1000     7462 2023-06-11 14:08:38.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/components/summa_tokenizer.rs
+-rw-rw-r--   0     1000     1000     2162 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/configs/config_proxy.rs
+-rw-rw-r--   0     1000     1000     4680 2023-06-13 08:40:32.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/configs/core.rs
+-rw-rw-r--   0     1000     1000     3512 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/configs/file_proxy.rs
+-rw-rw-r--   0     1000     1000      383 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/configs/mod.rs
+-rw-rw-r--   0     1000     1000     3335 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/configs/partial_proxy.rs
+-rw-rw-r--   0     1000     1000     8009 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/directories/byte_range_cache.rs
+-rw-rw-r--   0     1000     1000     8014 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/directories/caching_directory.rs
+-rw-rw-r--   0     1000     1000     7015 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
+-rw-rw-r--   0     1000     1000     5258 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/directories/external_requests.rs
+-rw-rw-r--   0     1000     1000    17667 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
+-rw-rw-r--   0     1000     1000     2255 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/directories/mod.rs
+-rw-rw-r--   0     1000     1000     6756 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/directories/network_directory.rs
+-rw-rw-r--   0     1000     1000     5192 2023-06-08 17:10:59.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/errors.rs
+-rw-rw-r--   0     1000     1000     2421 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/hyper_external_request.rs
+-rw-rw-r--   0     1000     1000      742 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/lib.rs
+-rw-rw-r--   0     1000     1000     1471 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/metrics/cache_metrics.rs
+-rw-rw-r--   0     1000     1000      960 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/metrics/label.rs
+-rw-rw-r--   0     1000     1000       92 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/metrics/mod.rs
+-rw-rw-r--   0     1000     1000      583 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/page_rank.rs
+-rw-rw-r--   0     1000     1000     5474 2023-06-08 17:10:59.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/proto_traits/aggregation.rs
+-rw-rw-r--   0     1000     1000     2294 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/proto_traits/compression.rs
+-rw-rw-r--   0     1000     1000     1068 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
+-rw-rw-r--   0     1000     1000      323 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/proto_traits/mod.rs
+-rw-rw-r--   0     1000     1000      662 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/proto_traits/order.rs
+-rw-rw-r--   0     1000     1000      582 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/proto_traits/snippet.rs
+-rw-rw-r--   0     1000     1000      411 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
+-rw-rw-r--   0     1000     1000     2048 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/scorers/eval_scorer.rs
+-rw-rw-r--   0     1000     1000     1538 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
+-rw-rw-r--   0     1000     1000      826 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
+-rw-rw-r--   0     1000     1000      218 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/scorers/mod.rs
+-rw-rw-r--   0     1000     1000      480 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
+-rw-rw-r--   0     1000     1000     7908 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
+-rw-rw-r--   0     1000     1000      415 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/utils/mod.rs
+-rw-rw-r--   0     1000     1000      309 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/utils/random.rs
+-rw-rw-r--   0     1000     1000     3165 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/utils/sync.rs
+-rw-rw-r--   0     1000     1000      450 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-core/src/validators.rs
+-rw-r--r--   0        0        0     2767 1970-01-01 00:00:00.000000 summa_embed-0.17.2/local_dependencies/summa-server/Cargo.toml
+-rw-rw-r--   0     1000     1000       43 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/.cargo/config.toml
+-rw-rw-r--   0     1000     1000     1050 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/LICENSE
+-rw-rw-r--   0     1000     1000     2832 2023-05-29 14:03:22.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/apis/consumer.rs
+-rw-rw-r--   0     1000     1000    13111 2023-06-08 17:10:59.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/apis/index.rs
+-rw-rw-r--   0     1000     1000      105 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/apis/mod.rs
+-rw-rw-r--   0     1000     1000     2909 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/apis/reflection.rs
+-rw-rw-r--   0     1000     1000     1278 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/apis/search.rs
+-rw-rw-r--   0     1000     1000      783 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/bin/main.rs
+-rw-rw-r--   0     1000     1000     5186 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/components/consumer_manager.rs
+-rw-rw-r--   0     1000     1000      813 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs
+-rw-rw-r--   0     1000     1000     1082 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/components/consumers/dummy.rs
+-rw-rw-r--   0     1000     1000    12123 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs
+-rw-rw-r--   0     1000     1000       84 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/components/consumers/kafka/mod.rs
+-rw-rw-r--   0     1000     1000      532 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/components/consumers/kafka/status.rs
+-rw-rw-r--   0     1000     1000      155 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/components/consumers/mod.rs
+-rw-rw-r--   0     1000     1000     3811 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/components/index_meter.rs
+-rw-rw-r--   0     1000     1000      258 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/components/mod.rs
+-rw-rw-r--   0     1000     1000      943 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/configs/api.rs
+-rw-rw-r--   0     1000     1000      919 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/configs/consumer.rs
+-rw-rw-r--   0     1000     1000      434 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/configs/metrics.rs
+-rw-rw-r--   0     1000     1000      116 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/configs/mod.rs
+-rw-rw-r--   0     1000     1000     3994 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/configs/server.rs
+-rw-rw-r--   0     1000     1000      991 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/configs/store.rs
+-rw-rw-r--   0     1000     1000     3459 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/errors.rs
+-rw-rw-r--   0     1000     1000     1427 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/lib.rs
+-rw-rw-r--   0     1000     1000     3681 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/logging.rs
+-rw-rw-r--   0     1000     1000    15747 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/server.rs
+-rw-rw-r--   0     1000     1000     7716 2023-06-01 07:26:30.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/services/api.rs
+-rw-rw-r--   0     1000     1000    40405 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/services/index.rs
+-rw-rw-r--   0     1000     1000     5174 2023-05-29 14:03:22.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/services/metrics.rs
+-rw-rw-r--   0     1000     1000      287 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/services/mod.rs
+-rw-rw-r--   0     1000     1000     2108 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/utils/mod.rs
+-rw-rw-r--   0     1000     1000      923 2023-06-16 10:18:53.000000 summa_embed-0.17.2/local_dependencies/summa-server/src/utils/thread_handler.rs
+-rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.17.2/local_dependencies/summa-proto/Cargo.toml
+-rw-rw-r--   0     1000     1000     1050 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/LICENSE
+-rw-rw-r--   0     1000     1000     2381 2023-06-10 14:42:19.000000 summa_embed-0.17.2/local_dependencies/summa-proto/build.rs
+-rwxrwxr-x   0     1000     1000      244 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/gen-docs.sh
+-rw-rw-r--   0     1000     1000     2561 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/markdown.tmpl
+-rw-rw-r--   0     1000     1000        0 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/proto/__init__.py
+-rw-rw-r--   0     1000     1000     1556 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/proto/consumer_service.proto
+-rw-rw-r--   0     1000     1000      393 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/proto/dag_pb.proto
+-rw-rw-r--   0     1000     1000    10274 2023-06-13 08:40:32.000000 summa_embed-0.17.2/local_dependencies/summa-proto/proto/index_service.proto
+-rw-rw-r--   0     1000     1000     7871 2023-06-13 08:40:32.000000 summa_embed-0.17.2/local_dependencies/summa-proto/proto/query.proto
+-rw-rw-r--   0     1000     1000      499 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/proto/reflection_service.proto
+-rw-rw-r--   0     1000     1000      867 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/proto/search_service.proto
+-rw-rw-r--   0     1000     1000      407 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/proto/unixfs.proto
+-rw-rw-r--   0     1000     1000       96 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/proto/utils.proto
+-rw-rw-r--   0     1000     1000     2523 2023-06-08 17:10:59.000000 summa_embed-0.17.2/local_dependencies/summa-proto/src/lib.rs
+-rw-rw-r--   0     1000     1000     2683 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/src/proto_traits/collector.rs
+-rw-rw-r--   0     1000     1000      212 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/src/proto_traits/mod.rs
+-rw-rw-r--   0     1000     1000      394 2023-06-08 17:10:59.000000 summa_embed-0.17.2/local_dependencies/summa-proto/src/proto_traits/query.rs
+-rw-rw-r--   0     1000     1000      613 2023-05-29 09:11:14.000000 summa_embed-0.17.2/local_dependencies/summa-proto/src/proto_traits/score.rs
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 summa_embed-0.17.2/Cargo.toml
+-rw-rw-r--   0     1000     1000      685 2023-05-29 09:11:14.000000 summa_embed-0.17.2/.gitignore
+-rw-rw-r--   0     1000     1000      400 2023-06-16 10:18:53.000000 summa_embed-0.17.2/pyproject.toml
+-rw-rw-r--   0     1000     1000     2220 2023-06-16 10:18:53.000000 summa_embed-0.17.2/src/lib.rs
+-rw-rw-r--   0     1000     1000   116194 2023-06-16 10:19:02.000000 summa_embed-0.17.2/Cargo.lock
+-rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.17.2/PKG-INFO
```

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/Cargo.toml` & `summa_embed-0.17.2/local_dependencies/summa-core/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-core"
-version = "0.17.0"
+version = "0.17.2"
 authors = ["Pasha Podolsky <ppodolsky@me.com>"]
 edition = "2021"
 license-file = "LICENSE"
 description = "Summa Core library"
 
 [lib]
 name = "summa_core"
```

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/LICENSE` & `summa_embed-0.17.2/local_dependencies/summa-core/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/dictionaries/drugs.csv` & `summa_embed-0.17.2/local_dependencies/summa-core/dictionaries/drugs.csv`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/components/custom_serializer.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/components/custom_serializer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/components/default_tokenizers.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/components/default_tokenizers.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/components/driver.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/components/driver.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/components/fruit_extractors.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/components/fruit_extractors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/components/index_holder.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/components/index_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/components/index_registry.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/components/index_registry.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/components/index_writer_holder.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/components/index_writer_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/components/mod.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/components/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/components/queries/exists_query.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/components/queries/exists_query.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/components/query_parser/morphology/english_nn.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/morphology/english_nn.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest` & `summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1120,15 +1120,15 @@
             proto::MorphologyConfig {
                 derive_tenses_coefficient: Some(0.3),
             },
         );
         query_parser.query_parser_config.0.morphology_configs = morphology_configs;
         query_parser.query_parser_config.0.query_language = Some("en".to_string());
         let query = query_parser.parse_query("search engine");
-        assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"search\"))), (Should, DisjunctionMaxQuery { disjuncts: [TermQuery(Term(field=0, type=Str, \"engine\")), TermQuery(Term(field=0, type=Str, \"engines\"))], tie_breaker: 0.3 })] })");
+        assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, DisjunctionMaxQuery { disjuncts: [TermQuery(Term(field=0, type=Str, \"search\")), TermQuery(Term(field=0, type=Str, \"searches\"))], tie_breaker: 0.3 }), (Should, DisjunctionMaxQuery { disjuncts: [TermQuery(Term(field=0, type=Str, \"engine\")), TermQuery(Term(field=0, type=Str, \"engines\"))], tie_breaker: 0.3 })] })");
     }
 
     #[test]
     pub fn test_ner() {
         let mut query_parser = create_query_parser();
         let mut morphology_configs = HashMap::new();
         morphology_configs.insert(
```

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/components/query_parser/utils.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/components/query_parser/utils.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/components/segment_attributes.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/components/segment_attributes.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/components/snippet_generator.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/components/snippet_generator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/components/summa_document.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/components/summa_document.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/components/summa_tokenizer.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/components/summa_tokenizer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/configs/config_proxy.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/configs/config_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/configs/core.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/configs/core.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/configs/file_proxy.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/configs/file_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/configs/partial_proxy.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/configs/partial_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/directories/byte_range_cache.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/directories/byte_range_cache.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/directories/caching_directory.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/directories/caching_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/directories/external_requests.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/directories/external_requests.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/directories/hot_cache_directory.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/directories/hot_cache_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/directories/mod.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/directories/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/directories/network_directory.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/directories/network_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/errors.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/errors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/hyper_external_request.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/hyper_external_request.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/lib.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/metrics/cache_metrics.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/metrics/cache_metrics.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/metrics/label.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/metrics/label.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/page_rank.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/page_rank.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/proto_traits/aggregation.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/proto_traits/aggregation.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/proto_traits/compression.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/proto_traits/compression.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/proto_traits/merge_policy.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/proto_traits/merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/proto_traits/order.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/proto_traits/order.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/proto_traits/snippet.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/proto_traits/snippet.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/scorers/eval_scorer.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/scorers/eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-core/src/utils/sync.rs` & `summa_embed-0.17.2/local_dependencies/summa-core/src/utils/sync.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-proto/Cargo.toml` & `summa_embed-0.17.2/local_dependencies/summa-proto/Cargo.toml`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-proto/LICENSE` & `summa_embed-0.17.2/local_dependencies/summa-server/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-proto/build.rs` & `summa_embed-0.17.2/local_dependencies/summa-proto/build.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-proto/markdown.tmpl` & `summa_embed-0.17.2/local_dependencies/summa-proto/markdown.tmpl`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-proto/proto/consumer_service.proto` & `summa_embed-0.17.2/local_dependencies/summa-proto/proto/consumer_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-proto/proto/index_service.proto` & `summa_embed-0.17.2/local_dependencies/summa-proto/proto/index_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-proto/proto/query.proto` & `summa_embed-0.17.2/local_dependencies/summa-proto/proto/query.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-proto/proto/search_service.proto` & `summa_embed-0.17.2/local_dependencies/summa-proto/proto/search_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-proto/src/lib.rs` & `summa_embed-0.17.2/local_dependencies/summa-proto/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-proto/src/proto_traits/collector.rs` & `summa_embed-0.17.2/local_dependencies/summa-proto/src/proto_traits/collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/local_dependencies/summa-proto/src/proto_traits/score.rs` & `summa_embed-0.17.2/local_dependencies/summa-proto/src/proto_traits/score.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/Cargo.toml` & `summa_embed-0.17.2/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [package]
 name = "summa-embed-py"
-version = "0.17.1"
+version = "0.17.2"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "summa_embed"
 crate-type = ["cdylib"]
 
 [dependencies]
+async-broadcast = "0.5"
 futures = "0.3"
 prost = "0.11"
 pyo3 = { version = "0.18", features = ["serde"] }
 pyo3-asyncio = { version =  "0.18", features = ["attributes", "tokio-runtime"] }
 pyo3-log = "0.8"
+pythonize = "0.18"
 serde_json = "1.0"
-summa-core = { version = "0.17.0", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
+summa-core = { version = "0.17.2", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
+summa-server = { version = "0.17.2", path = "local_dependencies/summa-server", default_features = false }
 summa-proto = { path = "local_dependencies/summa-proto" }
 tantivy = { git = "https://github.com/izihawa/tantivy", branch = "feature/summa", default_features = false, features = ["quickwit", "zstd-compression"] }
 tokio = { version = "1.25", default_features = false }
```

### Comparing `summa_embed-0.17.1/.gitignore` & `summa_embed-0.17.2/.gitignore`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.1/Cargo.lock` & `summa_embed-0.17.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -437,26 +437,26 @@
 dependencies = [
  "crypto-common",
  "inout",
 ]
 
 [[package]]
 name = "clap"
-version = "4.3.3"
+version = "4.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca8f255e4b8027970e78db75e78831229c9815fdbfa67eb1a1b777a62e24b4a0"
+checksum = "80672091db20273a15cf9fdd4e47ed43b5091ec9841bf4c6145c9dfbbcae09ed"
 dependencies = [
  "clap_builder",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.3.3"
+version = "4.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "acd4f3c17c83b0ba34ffbc4f8bbd74f079413f747f84a6f89292f138057e36ab"
+checksum = "c1458a1df40e1e2afebb7ab60ce55c1fa8f431146205aa5f4887e0b111c27636"
 dependencies = [
  "anstream",
  "anstyle",
  "bitflags",
  "clap_lex",
  "once_cell",
  "strsim",
@@ -2184,15 +2184,15 @@
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
 [[package]]
 name = "ownedbytes"
 version = "0.5.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#b715babfb250ae8618c9608737c8bf969a2c51e1"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#a558ead92515015b8a4b5b2aabe87cc5b9f5f515"
 dependencies = [
  "stable_deref_trait",
 ]
 
 [[package]]
 name = "parking_lot"
 version = "0.11.2"
@@ -2675,14 +2675,24 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "pythonize"
+version = "0.18.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9a0e1bbcd2a3856284bf4f4ef09ccb1157e9467847792754556f153ea3fe6b42"
+dependencies = [
+ "pyo3",
+ "serde",
+]
+
+[[package]]
 name = "quick-protobuf"
 version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d6da84cc204722a989e01ba2f6e1e276e190f22263d0cb6ce8526fcdb0d2e1f"
 dependencies = [
  "byteorder",
 ]
@@ -3330,15 +3340,15 @@
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
 
 [[package]]
 name = "summa-core"
-version = "0.17.0"
+version = "0.17.2"
 dependencies = [
  "anyhow",
  "async-trait",
  "base64 0.21.2",
  "bytes",
  "config",
  "derive_builder",
@@ -3378,24 +3388,27 @@
  "time",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "summa-embed-py"
-version = "0.17.1"
+version = "0.17.2"
 dependencies = [
+ "async-broadcast",
  "futures",
  "prost",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-log",
+ "pythonize",
  "serde_json",
  "summa-core",
  "summa-proto 0.28.0",
+ "summa-server",
  "tantivy",
  "tokio",
 ]
 
 [[package]]
 name = "summa-proto"
 version = "0.26.0"
@@ -3425,15 +3438,15 @@
  "tonic 0.9.2",
  "tonic-build 0.9.2",
  "tonic-reflection 0.9.2",
 ]
 
 [[package]]
 name = "summa-server"
-version = "0.17.0"
+version = "0.17.2"
 dependencies = [
  "anyhow",
  "async-broadcast",
  "async-trait",
  "clap",
  "config",
  "derive_builder",
@@ -3552,15 +3565,15 @@
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f764005d11ee5f36500a149ace24e00e3da98b0158b3e2d53a7495660d3f4d60"
 
 [[package]]
 name = "tantivy"
 version = "0.20.2"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#b715babfb250ae8618c9608737c8bf969a2c51e1"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#a558ead92515015b8a4b5b2aabe87cc5b9f5f515"
 dependencies = [
  "aho-corasick",
  "arc-swap",
  "async-trait",
  "base64 0.21.2",
  "bitpacking",
  "byteorder",
@@ -3609,38 +3622,38 @@
  "winapi",
  "zstd 0.12.3+zstd.1.5.2",
 ]
 
 [[package]]
 name = "tantivy-bitpacker"
 version = "0.4.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#b715babfb250ae8618c9608737c8bf969a2c51e1"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#a558ead92515015b8a4b5b2aabe87cc5b9f5f515"
 dependencies = [
  "bitpacking",
 ]
 
 [[package]]
 name = "tantivy-columnar"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#b715babfb250ae8618c9608737c8bf969a2c51e1"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#a558ead92515015b8a4b5b2aabe87cc5b9f5f515"
 dependencies = [
  "fastdivide",
  "fnv",
  "itertools",
  "serde",
  "tantivy-bitpacker",
  "tantivy-common",
  "tantivy-sstable",
  "tantivy-stacker",
 ]
 
 [[package]]
 name = "tantivy-common"
 version = "0.5.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#b715babfb250ae8618c9608737c8bf969a2c51e1"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#a558ead92515015b8a4b5b2aabe87cc5b9f5f515"
 dependencies = [
  "async-trait",
  "byteorder",
  "ownedbytes",
  "serde",
  "time",
 ]
@@ -3655,44 +3668,44 @@
  "regex-syntax 0.6.29",
  "utf8-ranges",
 ]
 
 [[package]]
 name = "tantivy-query-grammar"
 version = "0.20.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#b715babfb250ae8618c9608737c8bf969a2c51e1"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#a558ead92515015b8a4b5b2aabe87cc5b9f5f515"
 dependencies = [
  "combine",
  "once_cell",
  "regex",
 ]
 
 [[package]]
 name = "tantivy-sstable"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#b715babfb250ae8618c9608737c8bf969a2c51e1"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#a558ead92515015b8a4b5b2aabe87cc5b9f5f515"
 dependencies = [
  "izihawa-fst",
  "tantivy-common",
  "zstd 0.12.3+zstd.1.5.2",
 ]
 
 [[package]]
 name = "tantivy-stacker"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#b715babfb250ae8618c9608737c8bf969a2c51e1"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#a558ead92515015b8a4b5b2aabe87cc5b9f5f515"
 dependencies = [
  "murmurhash32",
  "tantivy-common",
 ]
 
 [[package]]
 name = "tantivy-tokenizer-api"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#b715babfb250ae8618c9608737c8bf969a2c51e1"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#a558ead92515015b8a4b5b2aabe87cc5b9f5f515"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "tap"
 version = "1.0.1"
@@ -4379,19 +4392,18 @@
  "regex",
  "stfu8",
  "unicode-segmentation",
 ]
 
 [[package]]
 name = "want"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ce8a968cb1cd110d136ff8b819a556d6fb6d919363c61534f6860c7eb172ba0"
+checksum = "bfa7760aed19e106de2c7c0b581b509f2f25d3dacaf737cb82ac61bc6d760b0e"
 dependencies = [
- "log",
  "try-lock",
 ]
 
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
```

