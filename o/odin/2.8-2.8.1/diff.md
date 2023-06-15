# Comparing `tmp/odin-2.8.tar.gz` & `tmp/odin-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odin-2.8.tar", max compression
+gzip compressed data, was "odin-2.8.1.tar", max compression
```

## Comparing `odin-2.8.tar` & `odin-2.8.1.tar`

### file list

```diff
@@ -1,121 +1,122 @@
--rw-r--r--   0        0        0     1539 2023-05-30 23:59:27.722059 odin-2.8/LICENSE
--rw-r--r--   0        0        0     7879 2023-05-30 23:59:27.722059 odin-2.8/README.rst
--rw-r--r--   0        0        0     2489 2023-05-30 23:59:27.722059 odin-2.8/pyproject.toml
--rw-r--r--   0        0        0      718 2023-05-30 23:59:27.722059 odin-2.8/src/odin/__init__.py
--rw-r--r--   0        0        0     5356 2023-05-30 23:59:27.722059 odin-2.8/src/odin/adapters.py
--rw-r--r--   0        0        0     7306 2023-05-30 23:59:27.722059 odin-2.8/src/odin/annotated_resource/__init__.py
--rw-r--r--   0        0        0      518 2023-05-30 23:59:27.722059 odin-2.8/src/odin/annotated_resource/special_fields.py
--rw-r--r--   0        0        0      791 2023-05-30 23:59:27.722059 odin-2.8/src/odin/annotated_resource/type_aliases.py
--rw-r--r--   0        0        0     8701 2023-05-30 23:59:27.722059 odin-2.8/src/odin/annotated_resource/type_resolution.py
--rw-r--r--   0        0        0      376 2023-05-30 23:59:27.722059 odin-2.8/src/odin/bases.py
--rw-r--r--   0        0        0        0 2023-05-30 23:59:27.722059 odin-2.8/src/odin/codecs/__init__.py
--rw-r--r--   0        0        0    10541 2023-05-30 23:59:27.722059 odin-2.8/src/odin/codecs/csv_codec.py
--rw-r--r--   0        0        0     2480 2023-05-30 23:59:27.722059 odin-2.8/src/odin/codecs/dict_codec.py
--rw-r--r--   0        0        0     4547 2023-05-30 23:59:27.726059 odin-2.8/src/odin/codecs/json_codec.py
--rw-r--r--   0        0        0     4264 2023-05-30 23:59:27.726059 odin-2.8/src/odin/codecs/msgpack_codec.py
--rw-r--r--   0        0        0     5899 2023-05-30 23:59:27.726059 odin-2.8/src/odin/codecs/toml_codec.py
--rw-r--r--   0        0        0     3115 2023-05-30 23:59:27.726059 odin-2.8/src/odin/codecs/xml_codec.py
--rw-r--r--   0        0        0     3970 2023-05-30 23:59:27.726059 odin-2.8/src/odin/codecs/yaml_codec.py
--rw-r--r--   0        0        0     1249 2023-05-30 23:59:27.726059 odin-2.8/src/odin/compatibility.py
--rw-r--r--   0        0        0        0 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/__init__.py
--rw-r--r--   0        0        0      503 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/arrow/__init__.py
--rw-r--r--   0        0        0     1791 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/arrow/fields.py
--rw-r--r--   0        0        0      146 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/geo/__init__.py
--rw-r--r--   0        0        0     3765 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/geo/datatypes.py
--rw-r--r--   0        0        0     2370 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/geo/fields.py
--rw-r--r--   0        0        0      115 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/money/__init__.py
--rw-r--r--   0        0        0    18131 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/money/datatypes.py
--rw-r--r--   0        0        0     1585 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/money/fields.py
--rw-r--r--   0        0        0      222 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/pint/__init__.py
--rw-r--r--   0        0        0     2182 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/pint/fields.py
--rw-r--r--   0        0        0      245 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/pint/units.py
--rw-r--r--   0        0        0       80 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/rich/__init__.py
--rw-r--r--   0        0        0      631 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/rich/theme.py
--rw-r--r--   0        0        0     1662 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/rich/validation_tree.py
--rw-r--r--   0        0        0     6787 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/sphinx/__init__.py
--rw-r--r--   0        0        0     1309 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/swagger/__init__.py
--rw-r--r--   0        0        0     1183 2023-05-30 23:59:27.726059 odin-2.8/src/odin/datastructures.py
--rw-r--r--   0        0        0    10233 2023-05-30 23:59:27.726059 odin-2.8/src/odin/datetimeutil.py
--rw-r--r--   0        0        0     1624 2023-05-30 23:59:27.726059 odin-2.8/src/odin/decorators.py
--rw-r--r--   0        0        0     4800 2023-05-30 23:59:27.726059 odin-2.8/src/odin/exceptions.py
--rw-r--r--   0        0        0    33799 2023-05-30 23:59:27.726059 odin-2.8/src/odin/fields/__init__.py
--rw-r--r--   0        0        0     2078 2023-05-30 23:59:27.726059 odin-2.8/src/odin/fields/base.py
--rw-r--r--   0        0        0     8102 2023-05-30 23:59:27.726059 odin-2.8/src/odin/fields/composite.py
--rw-r--r--   0        0        0     4479 2023-05-30 23:59:27.726059 odin-2.8/src/odin/fields/virtual.py
--rw-r--r--   0        0        0     4426 2023-05-30 23:59:27.726059 odin-2.8/src/odin/filtering.py
--rw-r--r--   0        0        0     1849 2023-05-30 23:59:27.726059 odin-2.8/src/odin/helpers.py
--rw-r--r--   0        0        0    34236 2023-05-30 23:59:27.726059 odin-2.8/src/odin/mapping/__init__.py
--rw-r--r--   0        0        0     2359 2023-05-30 23:59:27.726059 odin-2.8/src/odin/mapping/helpers.py
--rw-r--r--   0        0        0     8940 2023-05-30 23:59:27.726059 odin-2.8/src/odin/proxy.py
--rw-r--r--   0        0        0        0 2023-05-30 23:59:27.726059 odin-2.8/src/odin/py.typed
--rw-r--r--   0        0        0     4781 2023-05-30 23:59:27.726059 odin-2.8/src/odin/registration.py
--rw-r--r--   0        0        0    27572 2023-05-30 23:59:27.726059 odin-2.8/src/odin/resources.py
--rw-r--r--   0        0        0     1562 2023-05-30 23:59:27.726059 odin-2.8/src/odin/serializers.py
--rw-r--r--   0        0        0     9572 2023-05-30 23:59:27.726059 odin-2.8/src/odin/traversal.py
--rw-r--r--   0        0        0     8910 2023-05-30 23:59:27.726059 odin-2.8/src/odin/utils/__init__.py
--rw-r--r--   0        0        0     3725 2023-05-30 23:59:27.726059 odin-2.8/src/odin/utils/ipv6.py
--rw-r--r--   0        0        0    10342 2023-05-30 23:59:27.726059 odin-2.8/src/odin/validators.py
--rw-r--r--   0        0        0        0 2023-05-30 23:59:27.726059 odin-2.8/tests/__init__.py
--rw-r--r--   0        0        0      582 2023-05-30 23:59:27.726059 odin-2.8/tests/_helpers.py
--rw-r--r--   0        0        0        0 2023-05-30 23:59:27.726059 odin-2.8/tests/annotated_resources/__init__.py
--rw-r--r--   0        0        0    12091 2023-05-30 23:59:27.726059 odin-2.8/tests/annotated_resources/test_type_resolution.py
--rw-r--r--   0        0        0      429 2023-05-30 23:59:27.726059 odin-2.8/tests/conftest.py
--rw-r--r--   0        0        0     1779 2023-05-30 23:59:27.726059 odin-2.8/tests/contrib/test_arrow_fields.py
--rw-r--r--   0        0        0     6023 2023-05-30 23:59:27.726059 odin-2.8/tests/contrib/test_geo_datatypes.py
--rw-r--r--   0        0        0     2797 2023-05-30 23:59:27.726059 odin-2.8/tests/contrib/test_geo_fields.py
--rw-r--r--   0        0        0     2293 2023-05-30 23:59:27.726059 odin-2.8/tests/contrib/test_geo_serialisation.py
--rw-r--r--   0        0        0     3323 2023-05-30 23:59:27.726059 odin-2.8/tests/contrib/test_money_datatypes.py
--rw-r--r--   0        0        0      733 2023-05-30 23:59:27.726059 odin-2.8/tests/contrib/test_money_fields.py
--rw-r--r--   0        0        0      911 2023-05-30 23:59:27.726059 odin-2.8/tests/contrib/test_money_serialisation.py
--rw-r--r--   0        0        0     1216 2023-05-30 23:59:27.726059 odin-2.8/tests/contrib/test_pint_fields.py
--rw-r--r--   0        0        0      433 2023-05-30 23:59:27.726059 odin-2.8/tests/contrib/test_sphinx.py
--rw-r--r--   0        0        0      301 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/book-incorrect.toml
--rw-r--r--   0        0        0      720 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/book-invalid.json
--rw-r--r--   0        0        0      303 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/book-invalid.toml
--rw-r--r--   0        0        0      354 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/book-invalid.yaml
--rw-r--r--   0        0        0      642 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/book-valid.json
--rw-r--r--   0        0        0      325 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/book-valid.toml
--rw-r--r--   0        0        0      453 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/book-valid.xml
--rw-r--r--   0        0        0      357 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/book-valid.yaml
--rw-r--r--   0        0        0      469 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/library-header-alt-order.csv
--rw-r--r--   0        0        0     2503 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/library-invalid-nested.json
--rw-r--r--   0        0        0      442 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/library-invalid.csv
--rw-r--r--   0        0        0      441 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/library-last-bad.csv
--rw-r--r--   0        0        0      441 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/library-lower-header.csv
--rw-r--r--   0        0        0      389 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/library-no-header.csv
--rw-r--r--   0        0        0      441 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/library-valid.csv
--rw-r--r--   0        0        0     2543 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/library.json
--rw-r--r--   0        0        0     1948 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/library.yaml
--rw-r--r--   0        0        0     6147 2023-05-30 23:59:27.726059 odin-2.8/tests/resources.py
--rw-r--r--   0        0        0     2339 2023-05-30 23:59:27.726059 odin-2.8/tests/resources_annotated.py
--rw-r--r--   0        0        0     3922 2023-05-30 23:59:27.726059 odin-2.8/tests/test_adapters.py
--rw-r--r--   0        0        0     3124 2023-05-30 23:59:27.726059 odin-2.8/tests/test_annotated_resources.py
--rw-r--r--   0        0        0     7033 2023-05-30 23:59:27.726059 odin-2.8/tests/test_codec_csv.py
--rw-r--r--   0        0        0     3018 2023-05-30 23:59:27.726059 odin-2.8/tests/test_codec_dict.py
--rw-r--r--   0        0        0     2673 2023-05-30 23:59:27.726059 odin-2.8/tests/test_codec_json.py
--rw-r--r--   0        0        0     2689 2023-05-30 23:59:27.726059 odin-2.8/tests/test_codec_msgpack.py
--rw-r--r--   0        0        0     6256 2023-05-30 23:59:27.726059 odin-2.8/tests/test_codec_toml.py
--rw-r--r--   0        0        0     2157 2023-05-30 23:59:27.726059 odin-2.8/tests/test_codec_xml.py
--rw-r--r--   0        0        0     2228 2023-05-30 23:59:27.726059 odin-2.8/tests/test_codec_yaml.py
--rw-r--r--   0        0        0     1143 2023-05-30 23:59:27.726059 odin-2.8/tests/test_compatibility.py
--rw-r--r--   0        0        0     1793 2023-05-30 23:59:27.726059 odin-2.8/tests/test_datastructures.py
--rw-r--r--   0        0        0    11627 2023-05-30 23:59:27.726059 odin-2.8/tests/test_datetimeutil.py
--rw-r--r--   0        0        0     1070 2023-05-30 23:59:27.726059 odin-2.8/tests/test_decorators.py
--rw-r--r--   0        0        0     2072 2023-05-30 23:59:27.726059 odin-2.8/tests/test_exceptions.py
--rw-r--r--   0        0        0    48478 2023-05-30 23:59:27.730059 odin-2.8/tests/test_fields.py
--rw-r--r--   0        0        0     9825 2023-05-30 23:59:27.730059 odin-2.8/tests/test_fields_composite.py
--rw-r--r--   0        0        0     1028 2023-05-30 23:59:27.730059 odin-2.8/tests/test_fields_virtual.py
--rw-r--r--   0        0        0     4564 2023-05-30 23:59:27.730059 odin-2.8/tests/test_filtering.py
--rw-r--r--   0        0        0     1735 2023-05-30 23:59:27.730059 odin-2.8/tests/test_helpers.py
--rw-r--r--   0        0        0     3176 2023-05-30 23:59:27.730059 odin-2.8/tests/test_kitchensink.py
--rw-r--r--   0        0        0    20443 2023-05-30 23:59:27.730059 odin-2.8/tests/test_mapping.py
--rw-r--r--   0        0        0      963 2023-05-30 23:59:27.730059 odin-2.8/tests/test_mapping_helpers.py
--rw-r--r--   0        0        0     1374 2023-05-30 23:59:27.730059 odin-2.8/tests/test_polymorphic.py
--rw-r--r--   0        0        0     5058 2023-05-30 23:59:27.730059 odin-2.8/tests/test_proxy.py
--rw-r--r--   0        0        0     2904 2023-05-30 23:59:27.730059 odin-2.8/tests/test_resource_base.py
--rw-r--r--   0        0        0    11513 2023-05-30 23:59:27.730059 odin-2.8/tests/test_resources.py
--rw-r--r--   0        0        0     2206 2023-05-30 23:59:27.730059 odin-2.8/tests/test_serializers.py
--rw-r--r--   0        0        0    10433 2023-05-30 23:59:27.730059 odin-2.8/tests/test_traversal.py
--rw-r--r--   0        0        0     5860 2023-05-30 23:59:27.730059 odin-2.8/tests/test_utils.py
--rw-r--r--   0        0        0     7619 2023-05-30 23:59:27.730059 odin-2.8/tests/test_validators.py
--rw-r--r--   0        0        0     9536 1970-01-01 00:00:00.000000 odin-2.8/PKG-INFO
+-rw-r--r--   0        0        0     1539 2023-06-15 23:41:28.830387 odin-2.8.1/LICENSE
+-rw-r--r--   0        0        0     7879 2023-06-15 23:41:28.830387 odin-2.8.1/README.rst
+-rw-r--r--   0        0        0     2491 2023-06-15 23:41:28.834387 odin-2.8.1/pyproject.toml
+-rw-r--r--   0        0        0      718 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/__init__.py
+-rw-r--r--   0        0        0     5356 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/adapters.py
+-rw-r--r--   0        0        0     7306 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/annotated_resource/__init__.py
+-rw-r--r--   0        0        0      518 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/annotated_resource/special_fields.py
+-rw-r--r--   0        0        0      791 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/annotated_resource/type_aliases.py
+-rw-r--r--   0        0        0     8701 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/annotated_resource/type_resolution.py
+-rw-r--r--   0        0        0      376 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/bases.py
+-rw-r--r--   0        0        0        0 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/codecs/__init__.py
+-rw-r--r--   0        0        0    10541 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/codecs/csv_codec.py
+-rw-r--r--   0        0        0     2480 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/codecs/dict_codec.py
+-rw-r--r--   0        0        0     4547 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/codecs/json_codec.py
+-rw-r--r--   0        0        0     4264 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/codecs/msgpack_codec.py
+-rw-r--r--   0        0        0     5899 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/codecs/toml_codec.py
+-rw-r--r--   0        0        0     3115 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/codecs/xml_codec.py
+-rw-r--r--   0        0        0     3970 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/codecs/yaml_codec.py
+-rw-r--r--   0        0        0     1249 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/compatibility.py
+-rw-r--r--   0        0        0        0 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/__init__.py
+-rw-r--r--   0        0        0      503 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/arrow/__init__.py
+-rw-r--r--   0        0        0     1791 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/arrow/fields.py
+-rw-r--r--   0        0        0      146 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/geo/__init__.py
+-rw-r--r--   0        0        0     3765 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/geo/datatypes.py
+-rw-r--r--   0        0        0     2370 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/geo/fields.py
+-rw-r--r--   0        0        0     6371 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/json_schema/__init__.py
+-rw-r--r--   0        0        0      115 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/money/__init__.py
+-rw-r--r--   0        0        0    18131 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/money/datatypes.py
+-rw-r--r--   0        0        0     1585 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/money/fields.py
+-rw-r--r--   0        0        0      222 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/pint/__init__.py
+-rw-r--r--   0        0        0     2182 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/pint/fields.py
+-rw-r--r--   0        0        0      245 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/pint/units.py
+-rw-r--r--   0        0        0       80 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/rich/__init__.py
+-rw-r--r--   0        0        0      631 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/rich/theme.py
+-rw-r--r--   0        0        0     1662 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/rich/validation_tree.py
+-rw-r--r--   0        0        0     6787 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/sphinx/__init__.py
+-rw-r--r--   0        0        0     1309 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/swagger/__init__.py
+-rw-r--r--   0        0        0     1183 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/datastructures.py
+-rw-r--r--   0        0        0    10233 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/datetimeutil.py
+-rw-r--r--   0        0        0     1624 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/decorators.py
+-rw-r--r--   0        0        0     4800 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/exceptions.py
+-rw-r--r--   0        0        0    33799 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/fields/__init__.py
+-rw-r--r--   0        0        0     2078 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/fields/base.py
+-rw-r--r--   0        0        0     8102 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/fields/composite.py
+-rw-r--r--   0        0        0     4479 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/fields/virtual.py
+-rw-r--r--   0        0        0     4426 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/filtering.py
+-rw-r--r--   0        0        0     1849 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/helpers.py
+-rw-r--r--   0        0        0    34236 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/mapping/__init__.py
+-rw-r--r--   0        0        0     2359 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/mapping/helpers.py
+-rw-r--r--   0        0        0     8940 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/proxy.py
+-rw-r--r--   0        0        0        0 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/py.typed
+-rw-r--r--   0        0        0     5383 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/registration.py
+-rw-r--r--   0        0        0    27572 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/resources.py
+-rw-r--r--   0        0        0     1562 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/serializers.py
+-rw-r--r--   0        0        0     9572 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/traversal.py
+-rw-r--r--   0        0        0     8910 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/utils/__init__.py
+-rw-r--r--   0        0        0     3725 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/utils/ipv6.py
+-rw-r--r--   0        0        0    10342 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/validators.py
+-rw-r--r--   0        0        0        0 2023-06-15 23:41:28.838387 odin-2.8.1/tests/__init__.py
+-rw-r--r--   0        0        0      582 2023-06-15 23:41:28.838387 odin-2.8.1/tests/_helpers.py
+-rw-r--r--   0        0        0        0 2023-06-15 23:41:28.838387 odin-2.8.1/tests/annotated_resources/__init__.py
+-rw-r--r--   0        0        0    12091 2023-06-15 23:41:28.838387 odin-2.8.1/tests/annotated_resources/test_type_resolution.py
+-rw-r--r--   0        0        0      429 2023-06-15 23:41:28.838387 odin-2.8.1/tests/conftest.py
+-rw-r--r--   0        0        0     1779 2023-06-15 23:41:28.838387 odin-2.8.1/tests/contrib/test_arrow_fields.py
+-rw-r--r--   0        0        0     6023 2023-06-15 23:41:28.838387 odin-2.8.1/tests/contrib/test_geo_datatypes.py
+-rw-r--r--   0        0        0     2797 2023-06-15 23:41:28.838387 odin-2.8.1/tests/contrib/test_geo_fields.py
+-rw-r--r--   0        0        0     2293 2023-06-15 23:41:28.838387 odin-2.8.1/tests/contrib/test_geo_serialisation.py
+-rw-r--r--   0        0        0     3323 2023-06-15 23:41:28.838387 odin-2.8.1/tests/contrib/test_money_datatypes.py
+-rw-r--r--   0        0        0      733 2023-06-15 23:41:28.838387 odin-2.8.1/tests/contrib/test_money_fields.py
+-rw-r--r--   0        0        0      911 2023-06-15 23:41:28.838387 odin-2.8.1/tests/contrib/test_money_serialisation.py
+-rw-r--r--   0        0        0     1216 2023-06-15 23:41:28.838387 odin-2.8.1/tests/contrib/test_pint_fields.py
+-rw-r--r--   0        0        0      433 2023-06-15 23:41:28.838387 odin-2.8.1/tests/contrib/test_sphinx.py
+-rw-r--r--   0        0        0      301 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/book-incorrect.toml
+-rw-r--r--   0        0        0      720 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/book-invalid.json
+-rw-r--r--   0        0        0      303 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/book-invalid.toml
+-rw-r--r--   0        0        0      354 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/book-invalid.yaml
+-rw-r--r--   0        0        0      642 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/book-valid.json
+-rw-r--r--   0        0        0      325 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/book-valid.toml
+-rw-r--r--   0        0        0      453 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/book-valid.xml
+-rw-r--r--   0        0        0      357 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/book-valid.yaml
+-rw-r--r--   0        0        0      469 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/library-header-alt-order.csv
+-rw-r--r--   0        0        0     2503 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/library-invalid-nested.json
+-rw-r--r--   0        0        0      442 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/library-invalid.csv
+-rw-r--r--   0        0        0      441 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/library-last-bad.csv
+-rw-r--r--   0        0        0      441 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/library-lower-header.csv
+-rw-r--r--   0        0        0      389 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/library-no-header.csv
+-rw-r--r--   0        0        0      441 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/library-valid.csv
+-rw-r--r--   0        0        0     2543 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/library.json
+-rw-r--r--   0        0        0     1948 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/library.yaml
+-rw-r--r--   0        0        0     6147 2023-06-15 23:41:28.838387 odin-2.8.1/tests/resources.py
+-rw-r--r--   0        0        0     2339 2023-06-15 23:41:28.838387 odin-2.8.1/tests/resources_annotated.py
+-rw-r--r--   0        0        0     3922 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_adapters.py
+-rw-r--r--   0        0        0     3124 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_annotated_resources.py
+-rw-r--r--   0        0        0     7033 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_codec_csv.py
+-rw-r--r--   0        0        0     3018 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_codec_dict.py
+-rw-r--r--   0        0        0     2673 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_codec_json.py
+-rw-r--r--   0        0        0     2689 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_codec_msgpack.py
+-rw-r--r--   0        0        0     6256 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_codec_toml.py
+-rw-r--r--   0        0        0     2157 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_codec_xml.py
+-rw-r--r--   0        0        0     2228 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_codec_yaml.py
+-rw-r--r--   0        0        0     1143 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_compatibility.py
+-rw-r--r--   0        0        0     1793 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_datastructures.py
+-rw-r--r--   0        0        0    11627 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_datetimeutil.py
+-rw-r--r--   0        0        0     1070 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_decorators.py
+-rw-r--r--   0        0        0     2072 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_exceptions.py
+-rw-r--r--   0        0        0    48478 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_fields.py
+-rw-r--r--   0        0        0     9825 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_fields_composite.py
+-rw-r--r--   0        0        0     1028 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_fields_virtual.py
+-rw-r--r--   0        0        0     4564 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_filtering.py
+-rw-r--r--   0        0        0     1735 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_helpers.py
+-rw-r--r--   0        0        0     3176 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_kitchensink.py
+-rw-r--r--   0        0        0    20443 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_mapping.py
+-rw-r--r--   0        0        0      963 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_mapping_helpers.py
+-rw-r--r--   0        0        0     1374 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_polymorphic.py
+-rw-r--r--   0        0        0     5058 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_proxy.py
+-rw-r--r--   0        0        0     2904 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_resource_base.py
+-rw-r--r--   0        0        0    11513 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_resources.py
+-rw-r--r--   0        0        0     2206 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_serializers.py
+-rw-r--r--   0        0        0    10433 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_traversal.py
+-rw-r--r--   0        0        0     5860 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_utils.py
+-rw-r--r--   0        0        0     7619 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_validators.py
+-rw-r--r--   0        0        0     9538 1970-01-01 00:00:00.000000 odin-2.8.1/PKG-INFO
```

### Comparing `odin-2.8/LICENSE` & `odin-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `odin-2.8/README.rst` & `odin-2.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `odin-2.8/pyproject.toml` & `odin-2.8.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "odin"
-version = "2.8"
+version = "2.8.1"
 description = "Data-structure definition/validation/traversal, mapping and serialisation toolkit for Python"
 authors = ["Tim Savage <tim@savage.company>"]
 license = "BSD-3-Clause"
 readme = "README.rst"
 repository = "https://github.com/python-odin/odin"
 documentation = "https://odin.readthedocs.org"
 keywords = ["data-structure", "validation", "data-mapping"]
```

### Comparing `odin-2.8/src/odin/__init__.py` & `odin-2.8.1/src/odin/__init__.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/adapters.py` & `odin-2.8.1/src/odin/adapters.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/annotated_resource/__init__.py` & `odin-2.8.1/src/odin/annotated_resource/__init__.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/annotated_resource/special_fields.py` & `odin-2.8.1/src/odin/annotated_resource/special_fields.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/annotated_resource/type_aliases.py` & `odin-2.8.1/src/odin/annotated_resource/type_aliases.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/annotated_resource/type_resolution.py` & `odin-2.8.1/src/odin/annotated_resource/type_resolution.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/codecs/csv_codec.py` & `odin-2.8.1/src/odin/codecs/csv_codec.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/codecs/dict_codec.py` & `odin-2.8.1/src/odin/codecs/dict_codec.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/codecs/json_codec.py` & `odin-2.8.1/src/odin/codecs/json_codec.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/codecs/msgpack_codec.py` & `odin-2.8.1/src/odin/codecs/msgpack_codec.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/codecs/toml_codec.py` & `odin-2.8.1/src/odin/codecs/toml_codec.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/codecs/xml_codec.py` & `odin-2.8.1/src/odin/codecs/xml_codec.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/codecs/yaml_codec.py` & `odin-2.8.1/src/odin/codecs/yaml_codec.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/compatibility.py` & `odin-2.8.1/src/odin/compatibility.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/contrib/arrow/fields.py` & `odin-2.8.1/src/odin/contrib/arrow/fields.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/contrib/geo/datatypes.py` & `odin-2.8.1/src/odin/contrib/geo/datatypes.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/contrib/geo/fields.py` & `odin-2.8.1/src/odin/contrib/geo/fields.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/contrib/money/datatypes.py` & `odin-2.8.1/src/odin/contrib/money/datatypes.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/contrib/money/fields.py` & `odin-2.8.1/src/odin/contrib/money/fields.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/contrib/pint/fields.py` & `odin-2.8.1/src/odin/contrib/pint/fields.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/contrib/rich/theme.py` & `odin-2.8.1/src/odin/contrib/rich/theme.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/contrib/rich/validation_tree.py` & `odin-2.8.1/src/odin/contrib/rich/validation_tree.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/contrib/sphinx/__init__.py` & `odin-2.8.1/src/odin/contrib/sphinx/__init__.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/contrib/swagger/__init__.py` & `odin-2.8.1/src/odin/contrib/swagger/__init__.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/datastructures.py` & `odin-2.8.1/src/odin/datastructures.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/datetimeutil.py` & `odin-2.8.1/src/odin/datetimeutil.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/decorators.py` & `odin-2.8.1/src/odin/decorators.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/exceptions.py` & `odin-2.8.1/src/odin/exceptions.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/fields/__init__.py` & `odin-2.8.1/src/odin/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/fields/base.py` & `odin-2.8.1/src/odin/fields/base.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/fields/composite.py` & `odin-2.8.1/src/odin/fields/composite.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/fields/virtual.py` & `odin-2.8.1/src/odin/fields/virtual.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/filtering.py` & `odin-2.8.1/src/odin/filtering.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/helpers.py` & `odin-2.8.1/src/odin/helpers.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/mapping/__init__.py` & `odin-2.8.1/src/odin/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/mapping/helpers.py` & `odin-2.8.1/src/odin/mapping/helpers.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/proxy.py` & `odin-2.8.1/src/odin/proxy.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/registration.py` & `odin-2.8.1/src/odin/registration.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+from typing import Sequence
+
 from odin.utils import getmeta
 
 
 def generate_mapping_cache_name(from_obj, to_obj):
     return f"{from_obj.__module__}.{from_obj.__name__} > {to_obj.__module__}.{to_obj.__name__}"
 
 
 class ResourceCache:
     # Use the Borg pattern to share state between all instances. Details at
     # http://aspn.activestate.com/ASPN/Cookbook/Python/Recipe/66531.
     __shared_state = {
         "resources": {},
+        "resource_subclasses": {},
         "mappings": {},
         "field_resolvers": set(),
         "validation_error_handlers": {},
     }
 
     def __init__(self):
         self.__dict__ = self.__shared_state
@@ -29,25 +32,38 @@
             meta = getmeta(resource)
             resource_name = meta.resource_name.lower()
             self.resources[resource_name] = resource
             class_name = meta.class_name.lower()
             if resource_name != class_name:
                 self.resources[class_name] = resource
 
-    def get_resource(self, resource_name):
+    def get_resource(self, resource_name: str):
         """
         Get a resource by name.
 
         :param resource_name: Name of the resource to find.
         :returns: The resource type that matches requested name (case insensitive); or :const:`None` if the requested
             name has not been registered.
 
         """
         return self.resources.get(resource_name.lower())
 
+    def get_child_resources(self, resource: type) -> Sequence[type]:
+        """
+        Get subclasses of a resource.
+        """
+        resource_subclasses = self.resource_subclasses.get(resource)
+        if resource_subclasses is None:
+            self.resource_subclasses[resource] = resource_subclasses = {
+                child
+                for child in self.resources.values()
+                if issubclass(child, resource)
+            }
+        return resource_subclasses
+
     def register_mapping(self, mapping):
         """
         Register a mapping
 
         :param mapping: Mapping object to register.
 
         """
@@ -128,14 +144,15 @@
         return self.validation_error_handlers[error_type.__class__]
 
 
 cache = ResourceCache()
 
 register_resources = cache.register_resources
 get_resource = cache.get_resource
+get_child_resources = cache.get_child_resources
 
 register_mapping = cache.register_mapping
 get_mapping = cache.get_mapping
 
 register_field_resolver = cache.register_field_resolver
 get_field_resolver = cache.get_field_resolver
```

### Comparing `odin-2.8/src/odin/resources.py` & `odin-2.8.1/src/odin/resources.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/serializers.py` & `odin-2.8.1/src/odin/serializers.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/traversal.py` & `odin-2.8.1/src/odin/traversal.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/utils/__init__.py` & `odin-2.8.1/src/odin/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/utils/ipv6.py` & `odin-2.8.1/src/odin/utils/ipv6.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/src/odin/validators.py` & `odin-2.8.1/src/odin/validators.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/_helpers.py` & `odin-2.8.1/tests/_helpers.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/annotated_resources/test_type_resolution.py` & `odin-2.8.1/tests/annotated_resources/test_type_resolution.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/contrib/test_arrow_fields.py` & `odin-2.8.1/tests/contrib/test_arrow_fields.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/contrib/test_geo_datatypes.py` & `odin-2.8.1/tests/contrib/test_geo_datatypes.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/contrib/test_geo_fields.py` & `odin-2.8.1/tests/contrib/test_geo_fields.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/contrib/test_geo_serialisation.py` & `odin-2.8.1/tests/contrib/test_geo_serialisation.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/contrib/test_money_datatypes.py` & `odin-2.8.1/tests/contrib/test_money_datatypes.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/contrib/test_money_fields.py` & `odin-2.8.1/tests/contrib/test_money_fields.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/contrib/test_money_serialisation.py` & `odin-2.8.1/tests/contrib/test_money_serialisation.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/contrib/test_pint_fields.py` & `odin-2.8.1/tests/contrib/test_pint_fields.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/fixtures/book-invalid.json` & `odin-2.8.1/tests/fixtures/book-invalid.json`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/fixtures/book-valid.json` & `odin-2.8.1/tests/fixtures/book-valid.json`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/fixtures/library-invalid-nested.json` & `odin-2.8.1/tests/fixtures/library-invalid-nested.json`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/fixtures/library.json` & `odin-2.8.1/tests/fixtures/library.json`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/fixtures/library.yaml` & `odin-2.8.1/tests/fixtures/library.yaml`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/resources.py` & `odin-2.8.1/tests/resources.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/resources_annotated.py` & `odin-2.8.1/tests/resources_annotated.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_adapters.py` & `odin-2.8.1/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_annotated_resources.py` & `odin-2.8.1/tests/test_annotated_resources.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_codec_csv.py` & `odin-2.8.1/tests/test_codec_csv.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_codec_dict.py` & `odin-2.8.1/tests/test_codec_dict.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_codec_json.py` & `odin-2.8.1/tests/test_codec_json.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_codec_msgpack.py` & `odin-2.8.1/tests/test_codec_msgpack.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_codec_toml.py` & `odin-2.8.1/tests/test_codec_toml.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_codec_xml.py` & `odin-2.8.1/tests/test_codec_xml.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_codec_yaml.py` & `odin-2.8.1/tests/test_codec_yaml.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_compatibility.py` & `odin-2.8.1/tests/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_datastructures.py` & `odin-2.8.1/tests/test_datastructures.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_datetimeutil.py` & `odin-2.8.1/tests/test_datetimeutil.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_decorators.py` & `odin-2.8.1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_exceptions.py` & `odin-2.8.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_fields.py` & `odin-2.8.1/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_fields_composite.py` & `odin-2.8.1/tests/test_fields_composite.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_fields_virtual.py` & `odin-2.8.1/tests/test_fields_virtual.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_filtering.py` & `odin-2.8.1/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_helpers.py` & `odin-2.8.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_kitchensink.py` & `odin-2.8.1/tests/test_kitchensink.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_mapping.py` & `odin-2.8.1/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_mapping_helpers.py` & `odin-2.8.1/tests/test_mapping_helpers.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_polymorphic.py` & `odin-2.8.1/tests/test_polymorphic.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_proxy.py` & `odin-2.8.1/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_resource_base.py` & `odin-2.8.1/tests/test_resource_base.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_resources.py` & `odin-2.8.1/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_serializers.py` & `odin-2.8.1/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_traversal.py` & `odin-2.8.1/tests/test_traversal.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_utils.py` & `odin-2.8.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/tests/test_validators.py` & `odin-2.8.1/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `odin-2.8/PKG-INFO` & `odin-2.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odin
-Version: 2.8
+Version: 2.8.1
 Summary: Data-structure definition/validation/traversal, mapping and serialisation toolkit for Python
 Home-page: https://github.com/python-odin/odin
 License: BSD-3-Clause
 Keywords: data-structure,validation,data-mapping
 Author: Tim Savage
 Author-email: tim@savage.company
 Requires-Python: >=3.8,<4.0
```

