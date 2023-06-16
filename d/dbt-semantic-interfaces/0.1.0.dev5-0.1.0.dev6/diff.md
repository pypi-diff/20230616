# Comparing `tmp/dbt_semantic_interfaces-0.1.0.dev5.tar.gz` & `tmp/dbt_semantic_interfaces-0.1.0.dev6.tar.gz`

## Comparing `dbt_semantic_interfaces-0.1.0.dev5.tar` & `dbt_semantic_interfaces-0.1.0.dev6.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/CHANGELOG.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/Makefile
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/mypy.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/__init__.py
--rw-r--r--   0        0        0    18186 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/dataclass_serialization.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/enum_extension.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/errors.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/pretty_print.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/py.typed
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/references.py
--rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/__init__.py
--rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/base.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/metadata.py
--rw-r--r--   0        0        0     7556 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/metric.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/semantic_manifest.py
--rw-r--r--   0        0        0     6512 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/semantic_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/elements/__init__.py
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/elements/dimension.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/elements/entity.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/elements/measure.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/filters/__init__.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/filters/where_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/__init__.py
--rw-r--r--   0        0        0    14122 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/dir_to_model.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/explicit_schema.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/objects.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/schema_validator.py
--rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/schemas.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/yaml_loader.py
--rw-r--r--   0        0        0    14950 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/schemas/default_explicit_schema.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/__init__.py
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/dimension.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/entity.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/measure.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/metadata.py
--rw-r--r--   0        0        0     5436 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/metric.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/protocol_hint.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/semantic_manifest.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/semantic_model.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/where_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/__init__.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/add_input_metric_measures.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/agg_time_dimension.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/boolean_measure.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/convert_count.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/convert_median.py
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/names.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/proxy_measure.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/pydantic_rule_set.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/rule_set.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/transform_rule.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/type_enums/__init__.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/type_enums/aggregation_type.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/type_enums/dimension_type.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/type_enums/entity_type.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/type_enums/metric_type.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/type_enums/time_granularity.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/__init__.py
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/agg_time_dimension.py
--rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/common_entities.py
--rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/dimension_const.py
--rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/element_const.py
--rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/entities.py
--rw-r--r--   0        0        0    28504 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/measures.py
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/metrics.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/non_empty.py
--rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/reserved_keywords.py
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/semantic_manifest_validator.py
--rw-r--r--   0        0        0    11010 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/semantic_models.py
--rw-r--r--   0        0        0    10051 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/unique_valid_name.py
--rw-r--r--   0        0        0    15207 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/validator_helpers.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/LICENSE
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/README.md
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/pyproject.toml
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/PKG-INFO
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/CHANGELOG.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/Makefile
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/mypy.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/__init__.py
+-rw-r--r--   0        0        0    18186 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/dataclass_serialization.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/enum_extension.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/errors.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/pretty_print.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/py.typed
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/references.py
+-rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/__init__.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/base.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/metadata.py
+-rw-r--r--   0        0        0     7429 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/metric.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/semantic_manifest.py
+-rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/semantic_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/elements/__init__.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/elements/dimension.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/elements/entity.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/elements/measure.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/filters/__init__.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py
+-rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/filters/where_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/__init__.py
+-rw-r--r--   0        0        0    14122 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/dir_to_model.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/explicit_schema.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/objects.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/schema_validator.py
+-rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/schemas.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/yaml_loader.py
+-rw-r--r--   0        0        0    14950 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/schemas/default_explicit_schema.json
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/__init__.py
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/dimension.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/entity.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/measure.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/metadata.py
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/metric.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/protocol_hint.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/semantic_manifest.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/semantic_model.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/where_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/__init__.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/add_input_metric_measures.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/agg_time_dimension.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/boolean_measure.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/convert_count.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/convert_median.py
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/names.py
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/proxy_measure.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/pydantic_rule_set.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/rule_set.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/transform_rule.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/type_enums/__init__.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/type_enums/aggregation_type.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/type_enums/dimension_type.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/type_enums/entity_type.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/type_enums/metric_type.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/type_enums/time_granularity.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/__init__.py
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/agg_time_dimension.py
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/common_entities.py
+-rw-r--r--   0        0        0     7487 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/dimension_const.py
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/element_const.py
+-rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/entities.py
+-rw-r--r--   0        0        0    28360 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/measures.py
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/metrics.py
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/non_empty.py
+-rw-r--r--   0        0        0     6753 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/reserved_keywords.py
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/semantic_manifest_validator.py
+-rw-r--r--   0        0        0    10920 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/semantic_models.py
+-rw-r--r--   0        0        0     9960 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/unique_valid_name.py
+-rw-r--r--   0        0        0    15060 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/validator_helpers.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/LICENSE
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/README.md
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/pyproject.toml
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/PKG-INFO
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/Makefile` & `dbt_semantic_interfaces-0.1.0.dev6/Makefile`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/dataclass_serialization.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/dataclass_serialization.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/enum_extension.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/enum_extension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/errors.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/errors.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/pretty_print.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/pretty_print.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/references.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/references.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/test_utils.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,26 @@
     PydanticWhereFilter,
 )
 from dbt_semantic_interfaces.implementations.metadata import (
     PydanticFileSlice,
     PydanticMetadata,
 )
 from dbt_semantic_interfaces.implementations.metric import (
-    MetricType,
     PydanticMetric,
     PydanticMetricTypeParams,
 )
 from dbt_semantic_interfaces.implementations.semantic_manifest import (
     PydanticSemanticManifest,
 )
 from dbt_semantic_interfaces.implementations.semantic_model import (
     NodeRelation,
     PydanticSemanticModel,
 )
 from dbt_semantic_interfaces.parsing.objects import YamlConfigFile
+from dbt_semantic_interfaces.type_enums import MetricType
 
 logger = logging.getLogger(__name__)
 
 
 def as_datetime(date_string: str) -> datetime.datetime:
     """Helper to convert a string like '2020-01-01' into a datetime object."""
     return dateutil.parser.parse(date_string)
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/base.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/base.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/metric.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,15 @@
     PydanticParseableValueType,
 )
 from dbt_semantic_interfaces.implementations.filters.where_filter import (
     PydanticWhereFilter,
 )
 from dbt_semantic_interfaces.implementations.metadata import PydanticMetadata
 from dbt_semantic_interfaces.references import MeasureReference, MetricReference
-from dbt_semantic_interfaces.type_enums.metric_type import MetricType
-from dbt_semantic_interfaces.type_enums.time_granularity import (
-    TimeGranularity,
-    string_to_time_granularity,
-)
+from dbt_semantic_interfaces.type_enums import MetricType, TimeGranularity
 
 
 class PydanticMetricInputMeasure(PydanticCustomInputParser, HashableBaseModel):
     """Provides a pointer to a measure along with metric-specific processing directives.
 
     If an alias is set, this will be used as the string name reference for this measure after the aggregation
     phase in the SQL plan.
@@ -105,15 +101,15 @@
 
         count = parts[0]
         if not count.isdigit():
             raise ParsingException(f"Invalid count ({count}) in cumulative metric window string: ({window})")
 
         return PydanticMetricTimeWindow(
             count=int(count),
-            granularity=string_to_time_granularity(granularity),
+            granularity=TimeGranularity(granularity),
         )
 
 
 class PydanticMetricInput(HashableBaseModel):
     """Provides a pointer to a metric along with the additional properties used on that metric."""
 
     name: str
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/semantic_manifest.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/semantic_manifest.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 from importlib_metadata import version
 from pydantic import validator
 from typing_extensions import override
 
 from dbt_semantic_interfaces.implementations.base import HashableBaseModel
 from dbt_semantic_interfaces.implementations.metric import PydanticMetric
 from dbt_semantic_interfaces.implementations.semantic_model import PydanticSemanticModel
-from dbt_semantic_interfaces.protocols.protocol_hint import ProtocolHint
-from dbt_semantic_interfaces.protocols.semantic_manifest import SemanticManifest
+from dbt_semantic_interfaces.protocols import ProtocolHint, SemanticManifest
 
 
 class PydanticSemanticManifest(HashableBaseModel, ProtocolHint[SemanticManifest]):
     """Model holds all the information the SemanticLayer needs to render a query."""
 
     @override
     def _implements_protocol(self) -> SemanticManifest:  # noqa: D
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/semantic_model.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/semantic_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     HashableBaseModel,
     ModelWithMetadataParsing,
 )
 from dbt_semantic_interfaces.implementations.elements.dimension import PydanticDimension
 from dbt_semantic_interfaces.implementations.elements.entity import PydanticEntity
 from dbt_semantic_interfaces.implementations.elements.measure import PydanticMeasure
 from dbt_semantic_interfaces.implementations.metadata import PydanticMetadata
-from dbt_semantic_interfaces.protocols.protocol_hint import ProtocolHint
-from dbt_semantic_interfaces.protocols.semantic_model import (
+from dbt_semantic_interfaces.protocols import (
+    ProtocolHint,
     SemanticModel,
     SemanticModelDefaults,
 )
 from dbt_semantic_interfaces.references import (
     LinkableElementReference,
     MeasureReference,
     SemanticModelReference,
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/elements/dimension.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/elements/dimension.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,15 @@
     ModelWithMetadataParsing,
 )
 from dbt_semantic_interfaces.implementations.metadata import PydanticMetadata
 from dbt_semantic_interfaces.references import (
     DimensionReference,
     TimeDimensionReference,
 )
-from dbt_semantic_interfaces.type_enums.dimension_type import DimensionType
-from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
+from dbt_semantic_interfaces.type_enums import DimensionType, TimeGranularity
 
 ISO8601_FMT = "YYYY-MM-DD"
 
 
 class PydanticDimensionValidityParams(HashableBaseModel):
     """Parameters identifying a given dimension as an entity for validity state.
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/elements/entity.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/elements/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from dbt_semantic_interfaces.implementations.base import (
     HashableBaseModel,
     ModelWithMetadataParsing,
 )
 from dbt_semantic_interfaces.implementations.metadata import PydanticMetadata
 from dbt_semantic_interfaces.references import EntityReference
-from dbt_semantic_interfaces.type_enums.entity_type import EntityType
+from dbt_semantic_interfaces.type_enums import EntityType
 
 
 class PydanticEntity(HashableBaseModel, ModelWithMetadataParsing):
     """Describes a entity."""
 
     name: str
     description: Optional[str]
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/elements/measure.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/elements/measure.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from dbt_semantic_interfaces.implementations.base import (
     HashableBaseModel,
     ModelWithMetadataParsing,
 )
 from dbt_semantic_interfaces.implementations.metadata import PydanticMetadata
 from dbt_semantic_interfaces.references import MeasureReference, TimeDimensionReference
-from dbt_semantic_interfaces.type_enums.aggregation_type import AggregationType
+from dbt_semantic_interfaces.type_enums import AggregationType
 
 
 class PydanticNonAdditiveDimensionParameters(HashableBaseModel):
     """Describes the params for specifying non-additive dimensions in a measure.
 
     NOTE: Currently, only TimeDimensions are supported for this filter
     """
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Tuple
 
 from dbt_semantic_interfaces.references import (
     DimensionReference,
     EntityReference,
     TimeDimensionReference,
 )
-from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
+from dbt_semantic_interfaces.type_enums import TimeGranularity
 
 
 @dataclass(frozen=True)
 class DimensionCallParameterSet:
     """When 'dimension(...)' is used in the Jinja template of the where filter, the parameters to that call."""
 
     entity_path: Tuple[EntityReference, ...]
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/filters/where_filter.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/filters/where_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     TimeDimensionCallParameterSet,
 )
 from dbt_semantic_interfaces.references import (
     DimensionReference,
     EntityReference,
     TimeDimensionReference,
 )
-from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
+from dbt_semantic_interfaces.type_enums import TimeGranularity
 
 
 class PydanticWhereFilter(PydanticCustomInputParser, HashableBaseModel):
     """A filter applied to the data set containing measures, dimensions, identifiers relevant to the query.
 
     TODO: Clarify whether the filter applies to aggregated or un-aggregated data sets.
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/dir_to_model.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/dir_to_model.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/explicit_schema.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/explicit_schema.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/objects.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/objects.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/schema_validator.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/schema_validator.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/schemas.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/schemas.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/yaml_loader.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/schemas/default_explicit_schema.json` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/schemas/default_explicit_schema.json`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/dimension.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/dimension.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 from typing import Optional, Protocol
 
 from dbt_semantic_interfaces.protocols.metadata import Metadata
 from dbt_semantic_interfaces.references import (
     DimensionReference,
     TimeDimensionReference,
 )
-from dbt_semantic_interfaces.type_enums.dimension_type import DimensionType
-from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
+from dbt_semantic_interfaces.type_enums import DimensionType, TimeGranularity
 
 
 class DimensionValidityParams(Protocol):
     """Parameters identifying a given dimension as an entity for validity state.
 
     This construct is used for supporting SCD Type II tables, such as might be
     created via dbt's snapshot feature, or generated via periodic loads from external
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/entity.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from abc import abstractmethod
 from typing import Optional, Protocol
 
 from dbt_semantic_interfaces.references import EntityReference
-from dbt_semantic_interfaces.type_enums.entity_type import EntityType
+from dbt_semantic_interfaces.type_enums import EntityType
 
 
 class Entity(Protocol):
     """Describes a entity."""
 
     @property
     @abstractmethod
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/measure.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/measure.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from abc import abstractmethod
 from typing import Optional, Protocol, Sequence
 
 from dbt_semantic_interfaces.references import MeasureReference, TimeDimensionReference
-from dbt_semantic_interfaces.type_enums.aggregation_type import AggregationType
+from dbt_semantic_interfaces.type_enums import AggregationType
 
 
 class NonAdditiveDimensionParameters(Protocol):
     """Describes the params for specifying non-additive dimensions in a measure."""
 
     @property
     @abstractmethod
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/metadata.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/metric.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 from abc import abstractmethod
 from typing import Optional, Protocol, Sequence
 
 from dbt_semantic_interfaces.protocols.metadata import Metadata
 from dbt_semantic_interfaces.protocols.where_filter import WhereFilter
 from dbt_semantic_interfaces.references import MeasureReference, MetricReference
-from dbt_semantic_interfaces.type_enums.metric_type import MetricType
-from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
+from dbt_semantic_interfaces.type_enums import MetricType, TimeGranularity
 
 
 class MetricInputMeasure(Protocol):
     """Provides a pointer to a measure along with metric-specific processing directives.
 
     If an alias is set, this will be used as the string name reference for this measure after the aggregation
     phase in the SQL plan.
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/protocol_hint.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/protocol_hint.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/semantic_manifest.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/semantic_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/semantic_model.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/semantic_model.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/add_input_metric_measures.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/add_input_metric_measures.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from typing import Set
 
 from typing_extensions import override
 
 from dbt_semantic_interfaces.errors import ModelTransformError
-from dbt_semantic_interfaces.implementations.metric import (
-    MetricType,
-    PydanticMetricInputMeasure,
-)
+from dbt_semantic_interfaces.implementations.metric import PydanticMetricInputMeasure
 from dbt_semantic_interfaces.implementations.semantic_manifest import (
     PydanticSemanticManifest,
 )
-from dbt_semantic_interfaces.protocols.protocol_hint import ProtocolHint
+from dbt_semantic_interfaces.protocols import ProtocolHint
 from dbt_semantic_interfaces.transformations.transform_rule import (
     SemanticManifestTransformRule,
 )
+from dbt_semantic_interfaces.type_enums import MetricType
 
 
 class AddInputMetricMeasuresRule(ProtocolHint[SemanticManifestTransformRule[PydanticSemanticManifest]]):
     """Add all measures corresponding to the input metrics of the derived metric."""
 
     @override
     def _implements_protocol(self) -> SemanticManifestTransformRule[PydanticSemanticManifest]:  # noqa: D
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/agg_time_dimension.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/agg_time_dimension.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from typing_extensions import override
 
 from dbt_semantic_interfaces.implementations.semantic_manifest import (
     PydanticSemanticManifest,
 )
-from dbt_semantic_interfaces.protocols.protocol_hint import ProtocolHint
+from dbt_semantic_interfaces.protocols import ProtocolHint
 from dbt_semantic_interfaces.transformations.transform_rule import (
     SemanticManifestTransformRule,
 )
 
 logger = logging.getLogger(__name__)
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/boolean_measure.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/boolean_measure.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
 
 from typing_extensions import override
 
 from dbt_semantic_interfaces.implementations.semantic_manifest import (
     PydanticSemanticManifest,
 )
-from dbt_semantic_interfaces.protocols.protocol_hint import ProtocolHint
+from dbt_semantic_interfaces.protocols import ProtocolHint
 from dbt_semantic_interfaces.transformations.transform_rule import (
     SemanticManifestTransformRule,
 )
-from dbt_semantic_interfaces.type_enums.aggregation_type import AggregationType
+from dbt_semantic_interfaces.type_enums import AggregationType
 
 logger = logging.getLogger(__name__)
 
 
 class BooleanMeasureAggregationRule(ProtocolHint[SemanticManifestTransformRule[PydanticSemanticManifest]]):
     """Converts the expression used in boolean measures so that it can be aggregated."""
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/convert_count.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/convert_count.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing_extensions import override
 
 from dbt_semantic_interfaces.errors import ModelTransformError
 from dbt_semantic_interfaces.implementations.semantic_manifest import (
     PydanticSemanticManifest,
 )
-from dbt_semantic_interfaces.protocols.protocol_hint import ProtocolHint
+from dbt_semantic_interfaces.protocols import ProtocolHint
 from dbt_semantic_interfaces.transformations.transform_rule import (
     SemanticManifestTransformRule,
 )
-from dbt_semantic_interfaces.type_enums.aggregation_type import AggregationType
+from dbt_semantic_interfaces.type_enums import AggregationType
 
 ONE = "1"
 
 
 class ConvertCountToSumRule(ProtocolHint[SemanticManifestTransformRule[PydanticSemanticManifest]]):
     """Converts any COUNT measures to SUM equivalent."""
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/convert_median.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/convert_median.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from dbt_semantic_interfaces.errors import ModelTransformError
 from dbt_semantic_interfaces.implementations.elements.measure import (
     PydanticMeasureAggregationParameters,
 )
 from dbt_semantic_interfaces.implementations.semantic_manifest import (
     PydanticSemanticManifest,
 )
-from dbt_semantic_interfaces.protocols.protocol_hint import ProtocolHint
+from dbt_semantic_interfaces.protocols import ProtocolHint
 from dbt_semantic_interfaces.transformations.transform_rule import (
     SemanticManifestTransformRule,
 )
-from dbt_semantic_interfaces.type_enums.aggregation_type import AggregationType
+from dbt_semantic_interfaces.type_enums import AggregationType
 
 MEDIAN_PERCENTILE = 0.5
 
 
 class ConvertMedianToPercentileRule(ProtocolHint[SemanticManifestTransformRule[PydanticSemanticManifest]]):
     """Converts any MEDIAN measures to percentile equivalent."""
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/names.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/names.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing_extensions import override
 
 from dbt_semantic_interfaces.implementations.semantic_manifest import (
     PydanticSemanticManifest,
 )
 from dbt_semantic_interfaces.implementations.semantic_model import PydanticSemanticModel
-from dbt_semantic_interfaces.protocols.protocol_hint import ProtocolHint
+from dbt_semantic_interfaces.protocols import ProtocolHint
 from dbt_semantic_interfaces.transformations.transform_rule import (
     SemanticManifestTransformRule,
 )
 
 logger = logging.getLogger(__name__)
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/proxy_measure.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/proxy_measure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import logging
 
 from typing_extensions import override
 
 from dbt_semantic_interfaces.errors import ModelTransformError
 from dbt_semantic_interfaces.implementations.metric import (
-    MetricType,
     PydanticMetric,
     PydanticMetricInputMeasure,
     PydanticMetricTypeParams,
 )
 from dbt_semantic_interfaces.implementations.semantic_manifest import (
     PydanticSemanticManifest,
 )
-from dbt_semantic_interfaces.protocols.protocol_hint import ProtocolHint
+from dbt_semantic_interfaces.protocols import ProtocolHint
 from dbt_semantic_interfaces.transformations.transform_rule import (
     SemanticManifestTransformRule,
 )
+from dbt_semantic_interfaces.type_enums import MetricType
 
 logger = logging.getLogger(__name__)
 
 
 class CreateProxyMeasureRule(ProtocolHint[SemanticManifestTransformRule[PydanticSemanticManifest]]):
     """Adds a proxy metric for measures that have the create_metric flag set, if it does not already exist.
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/pydantic_rule_set.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/pydantic_rule_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Sequence
 
 from typing_extensions import override
 
 from dbt_semantic_interfaces.implementations.semantic_manifest import (
     PydanticSemanticManifest,
 )
-from dbt_semantic_interfaces.protocols.protocol_hint import ProtocolHint
+from dbt_semantic_interfaces.protocols import ProtocolHint
 from dbt_semantic_interfaces.transformations.add_input_metric_measures import (
     AddInputMetricMeasuresRule,
 )
 from dbt_semantic_interfaces.transformations.agg_time_dimension import (
     SetMeasureAggregationTimeDimensionRule,
 )
 from dbt_semantic_interfaces.transformations.boolean_measure import (
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/rule_set.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/rule_set.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from abc import abstractmethod
 from typing import Protocol, Sequence
 
-from dbt_semantic_interfaces.protocols.semantic_manifest import SemanticManifestT
+from dbt_semantic_interfaces.protocols import SemanticManifestT
 from dbt_semantic_interfaces.transformations.transform_rule import (
     SemanticManifestTransformRule,
 )
 
 logger = logging.getLogger(__name__)
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 from typing import Optional, Protocol, Sequence
 
 from typing_extensions import override
 
 from dbt_semantic_interfaces.implementations.semantic_manifest import (
     PydanticSemanticManifest,
 )
-from dbt_semantic_interfaces.protocols.protocol_hint import ProtocolHint
-from dbt_semantic_interfaces.protocols.semantic_manifest import SemanticManifestT
+from dbt_semantic_interfaces.protocols import ProtocolHint, SemanticManifestT
 from dbt_semantic_interfaces.transformations.pydantic_rule_set import (
     PydanticSemanticManifestTransformRuleSet,
 )
 from dbt_semantic_interfaces.transformations.transform_rule import (
     SemanticManifestTransformRule,
 )
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/transform_rule.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/transform_rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from abc import abstractmethod
 from typing import Protocol, TypeVar
 
-from dbt_semantic_interfaces.protocols.semantic_manifest import SemanticManifestT
+from dbt_semantic_interfaces.protocols import SemanticManifestT
 
 
 class SemanticManifestTransformRule(Protocol[SemanticManifestT]):
     """Encapsulates logic for transforming a model. e.g. add metrics based on measures."""
 
     @abstractmethod
     def transform_model(self, semantic_manifest: SemanticManifestT) -> SemanticManifestT:
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/type_enums/time_granularity.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/type_enums/time_granularity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/agg_time_dimension.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/agg_time_dimension.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Generic, List, Sequence
 
-from dbt_semantic_interfaces.protocols.semantic_manifest import SemanticManifestT
-from dbt_semantic_interfaces.protocols.semantic_model import SemanticModel
+from dbt_semantic_interfaces.protocols import SemanticManifestT, SemanticModel
 from dbt_semantic_interfaces.references import SemanticModelElementReference
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
     SemanticManifestValidationRule,
     SemanticModelElementContext,
     SemanticModelElementType,
     SemanticModelValidationHelpers,
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/common_entities.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/common_entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from typing import Dict, Generic, List, Sequence, Set
 
-from dbt_semantic_interfaces.protocols.entity import Entity
-from dbt_semantic_interfaces.protocols.semantic_manifest import SemanticManifestT
-from dbt_semantic_interfaces.protocols.semantic_model import SemanticModel
+from dbt_semantic_interfaces.protocols import Entity, SemanticManifestT, SemanticModel
 from dbt_semantic_interfaces.references import (
     EntityReference,
     SemanticModelElementReference,
 )
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
     SemanticManifestValidationRule,
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/dimension_const.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/dimension_const.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import Dict, Generic, List, Sequence
 
-from dbt_semantic_interfaces.protocols.dimension import Dimension
-from dbt_semantic_interfaces.protocols.semantic_manifest import SemanticManifestT
-from dbt_semantic_interfaces.protocols.semantic_model import SemanticModel
+from dbt_semantic_interfaces.protocols import (
+    Dimension,
+    SemanticManifestT,
+    SemanticModel,
+)
 from dbt_semantic_interfaces.references import (
     DimensionReference,
     SemanticModelElementReference,
 )
-from dbt_semantic_interfaces.type_enums.dimension_type import DimensionType
-from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
+from dbt_semantic_interfaces.type_enums import DimensionType, TimeGranularity
 from dbt_semantic_interfaces.validations.validator_helpers import (
     DimensionInvariants,
     FileContext,
     SemanticManifestValidationRule,
     SemanticModelElementContext,
     SemanticModelElementType,
     ValidationError,
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/element_const.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/element_const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import defaultdict
 from typing import DefaultDict, Generic, List, Sequence
 
 from dbt_semantic_interfaces.implementations.semantic_manifest import (
     PydanticSemanticManifest,
 )
-from dbt_semantic_interfaces.protocols.semantic_manifest import SemanticManifestT
+from dbt_semantic_interfaces.protocols import SemanticManifestT
 from dbt_semantic_interfaces.references import SemanticModelReference
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
     SemanticManifestValidationRule,
     SemanticModelContext,
     SemanticModelElementType,
     ValidationError,
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/entities.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/entities.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 from datetime import date
 from typing import Generic, List, MutableSet, Sequence
 
-from dbt_semantic_interfaces.protocols.semantic_manifest import SemanticManifestT
-from dbt_semantic_interfaces.protocols.semantic_model import SemanticModel
+from dbt_semantic_interfaces.protocols import SemanticManifestT, SemanticModel
 from dbt_semantic_interfaces.references import SemanticModelReference
-from dbt_semantic_interfaces.type_enums.entity_type import EntityType
+from dbt_semantic_interfaces.type_enums import EntityType
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
     SemanticManifestValidationRule,
     SemanticModelContext,
     ValidationError,
     ValidationFutureError,
     ValidationIssue,
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/measures.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/measures.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from collections import defaultdict
 from typing import DefaultDict, Dict, Generic, List, Sequence, Set
 
 from more_itertools import bucket
 
-from dbt_semantic_interfaces.protocols.metric import Metric
-from dbt_semantic_interfaces.protocols.semantic_manifest import (
+from dbt_semantic_interfaces.protocols import (
+    Metric,
     SemanticManifest,
     SemanticManifestT,
 )
 from dbt_semantic_interfaces.references import MeasureReference, MetricModelReference
-from dbt_semantic_interfaces.type_enums.aggregation_type import AggregationType
-from dbt_semantic_interfaces.type_enums.dimension_type import DimensionType
+from dbt_semantic_interfaces.type_enums import AggregationType, DimensionType
 from dbt_semantic_interfaces.validations.unique_valid_name import UniqueAndValidNameRule
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
     MetricContext,
     SemanticManifestValidationRule,
     SemanticModelElementContext,
     SemanticModelElementReference,
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/metrics.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import traceback
 from typing import Generic, List, Sequence
 
 from dbt_semantic_interfaces.errors import ParsingException
 from dbt_semantic_interfaces.implementations.metric import PydanticMetricTimeWindow
-from dbt_semantic_interfaces.protocols.metric import Metric, MetricType
-from dbt_semantic_interfaces.protocols.semantic_manifest import (
+from dbt_semantic_interfaces.protocols import (
+    Metric,
     SemanticManifest,
     SemanticManifestT,
 )
 from dbt_semantic_interfaces.references import MetricModelReference
+from dbt_semantic_interfaces.type_enums import MetricType
 from dbt_semantic_interfaces.validations.unique_valid_name import UniqueAndValidNameRule
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
     MetricContext,
     SemanticManifestValidationRule,
     ValidationError,
     ValidationIssue,
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/non_empty.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/non_empty.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Generic, List, Sequence
 
 from dbt_semantic_interfaces.implementations.semantic_manifest import (
     PydanticSemanticManifest,
 )
-from dbt_semantic_interfaces.protocols.semantic_manifest import SemanticManifestT
+from dbt_semantic_interfaces.protocols import SemanticManifestT
 from dbt_semantic_interfaces.validations.validator_helpers import (
     SemanticManifestValidationRule,
     ValidationError,
     ValidationIssue,
     validate_safely,
 )
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/reserved_keywords.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/reserved_keywords.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Generic, List
 
-from dbt_semantic_interfaces.protocols.semantic_manifest import (
+from dbt_semantic_interfaces.protocols import (
     SemanticManifest,
     SemanticManifestT,
+    SemanticModel,
 )
-from dbt_semantic_interfaces.protocols.semantic_model import SemanticModel
 from dbt_semantic_interfaces.references import SemanticModelElementReference
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
     SemanticManifestValidationRule,
     SemanticModelContext,
     SemanticModelElementContext,
     SemanticModelElementType,
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/semantic_manifest_validator.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/semantic_manifest_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import copy
 import logging
 from concurrent.futures import ProcessPoolExecutor, as_completed
 from typing import Generic, List, Sequence
 
-from dbt_semantic_interfaces.protocols.semantic_manifest import (
-    SemanticManifest,
-    SemanticManifestT,
-)
+from dbt_semantic_interfaces.protocols import SemanticManifest, SemanticManifestT
 from dbt_semantic_interfaces.validations.agg_time_dimension import (
     AggregationTimeDimensionRule,
 )
 from dbt_semantic_interfaces.validations.dimension_const import DimensionConsistencyRule
 from dbt_semantic_interfaces.validations.element_const import ElementConsistencyRule
 from dbt_semantic_interfaces.validations.entities import (
     NaturalEntityConfigurationRule,
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/semantic_models.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/semantic_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 from typing import Generic, List, Sequence
 
-from dbt_semantic_interfaces.protocols.semantic_manifest import SemanticManifestT
-from dbt_semantic_interfaces.protocols.semantic_model import SemanticModel
+from dbt_semantic_interfaces.protocols import SemanticManifestT, SemanticModel
 from dbt_semantic_interfaces.references import SemanticModelReference
-from dbt_semantic_interfaces.type_enums.entity_type import EntityType
+from dbt_semantic_interfaces.type_enums import EntityType
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
     SemanticManifestValidationRule,
     SemanticModelContext,
     SemanticModelValidationHelpers,
     ValidationError,
     ValidationIssue,
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/unique_valid_name.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/unique_valid_name.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 
 import enum
 import re
 from typing import Dict, Generic, List, Optional, Sequence, Tuple
 
 from dbt_semantic_interfaces.enum_extension import assert_values_exhausted
-from dbt_semantic_interfaces.protocols.semantic_manifest import (
+from dbt_semantic_interfaces.protocols import (
     SemanticManifest,
     SemanticManifestT,
+    SemanticModel,
 )
-from dbt_semantic_interfaces.protocols.semantic_model import SemanticModel
 from dbt_semantic_interfaces.references import (
     ElementReference,
     MetricModelReference,
     SemanticModelElementReference,
     SemanticModelReference,
 )
-from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
+from dbt_semantic_interfaces.type_enums import TimeGranularity
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
     MetricContext,
     SemanticManifestValidationRule,
     SemanticModelContext,
     SemanticModelElementContext,
     SemanticModelElementType,
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/validator_helpers.py` & `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/validator_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,23 +19,21 @@
     Union,
 )
 
 import click
 from pydantic import BaseModel, Extra
 
 from dbt_semantic_interfaces.implementations.base import FrozenBaseModel
-from dbt_semantic_interfaces.protocols.metadata import Metadata
-from dbt_semantic_interfaces.protocols.semantic_manifest import SemanticManifestT
-from dbt_semantic_interfaces.protocols.semantic_model import SemanticModel
+from dbt_semantic_interfaces.protocols import Metadata, SemanticManifestT, SemanticModel
 from dbt_semantic_interfaces.references import (
     MetricModelReference,
     SemanticModelElementReference,
     SemanticModelReference,
 )
-from dbt_semantic_interfaces.type_enums.dimension_type import DimensionType
+from dbt_semantic_interfaces.type_enums import DimensionType
 
 VALIDATE_SAFELY_ERROR_STR_TMPLT = ". Issue occurred in method `{method_name}` called with {arguments_str}"
 ValidationContextJSON = Dict[str, Union[str, int, None]]
 ValidationIssueJSON = Dict[str, Union[str, int, ValidationContextJSON]]
 
 
 class ValidationIssueLevel(Enum):
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/.gitignore` & `dbt_semantic_interfaces-0.1.0.dev6/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/LICENSE` & `dbt_semantic_interfaces-0.1.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/README.md` & `dbt_semantic_interfaces-0.1.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/pyproject.toml` & `dbt_semantic_interfaces-0.1.0.dev6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbt-semantic-interfaces"
-version = "0.1.0.dev5"
+version = "0.1.0.dev6"
 description = 'The shared semantic layer definitions that dbt-core and MetricFlow use'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "dbt Labs", email = "info@dbtlabs.com" },
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev5/PKG-INFO` & `dbt_semantic_interfaces-0.1.0.dev6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-semantic-interfaces
-Version: 0.1.0.dev5
+Version: 0.1.0.dev6
 Summary: The shared semantic layer definitions that dbt-core and MetricFlow use
 Author-email: dbt Labs <info@dbtlabs.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-semantic-interfaces Version: 0.1.0.dev5
+Metadata-Version: 2.1 Name: dbt-semantic-interfaces Version: 0.1.0.dev6
 Summary: The shared semantic layer definitions that dbt-core and MetricFlow use
 Author-email: dbt Labs
 dbtlabs.com> License-Expression: Apache-2.0 License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
```

