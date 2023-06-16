# Comparing `tmp/oarepo-model-builder-multilingual-2.0.8.tar.gz` & `tmp/oarepo-model-builder-multilingual-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-multilingual-2.0.8.tar", last modified: Wed Apr 26 11:16:58 2023, max compression
+gzip compressed data, was "oarepo-model-builder-multilingual-3.0.1.tar", last modified: Fri Jun 16 11:05:34 2023, max compression
```

## Comparing `oarepo-model-builder-multilingual-2.0.8.tar` & `oarepo-model-builder-multilingual-3.0.1.tar`

### file list

```diff
@@ -1,66 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.979758 oarepo-model-builder-multilingual-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-04-26 11:16:58.979758 oarepo-model-builder-multilingual-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.971758 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.975758 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/builders/mult_setup_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.975758 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/builtin_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/builtin_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/builtin_models/i18n.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.975758 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/datatypes/multilings.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/faker.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/i18n.json5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.975758 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/invenio_search_multilingual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.975758 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/templates/invenio_record_dumper_multilingual.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/templates/invenio_record_multilingual.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.979758 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/model_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/model_preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/model_preprocessors/multilingual.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/multilingual_jsonschema.json5
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/multilingual_settings.json5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.979758 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/property_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/property_preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/property_preprocessors/i18nStr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/property_preprocessors/multilingual.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/ui_jsonschema.json5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.979758 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/utils/supported_langs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.979758 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.975758 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-04-26 11:16:58.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-26 11:16:58.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:16:58.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-26 11:16:58.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-26 11:16:58.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-26 11:16:58.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-26 11:16:58.983758 oarepo-model-builder-multilingual-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.979758 oarepo-model-builder-multilingual-2.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/mock_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/model.json5
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/multilingual_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/test_build_from_entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/test_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/test_i18nStr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/test_marshmallow_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/test_multi_facets.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/test_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.396382 oarepo-model-builder-multilingual-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-16 11:05:34.396382 oarepo-model-builder-multilingual-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.380382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.384382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/builders/mult_setup_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.384382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/builtin_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/builtin_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/builtin_models/i18n.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.384382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.384382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.384382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/facets/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/facets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/facets/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.388382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/mapping/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/mapping/multi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.388382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/marshmallow/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/marshmallow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/marshmallow/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/marshmallow/ui_i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.388382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/model/multilingual_dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.388382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/multilingual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/multilingual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/multilingual/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/multilings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/faker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.388382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/invenio_record_multilingual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.392382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/templates/invenio_record_dumper_multilingual.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/templates/invenio_record_multilingual.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.392382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/utils/supported_langs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.392382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.380382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-16 11:05:34.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-16 11:05:34.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:05:34.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-16 11:05:34.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-16 11:05:34.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-16 11:05:34.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-16 11:05:34.396382 oarepo-model-builder-multilingual-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.396382 oarepo-model-builder-multilingual-3.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/tests/mock_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/tests/model.json5
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/tests/multilingual_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/tests/test_build_from_entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/tests/test_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/tests/test_i18nStr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/tests/test_marshmallow_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/tests/test_multi_facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/tests/test_ui.py
```

### Comparing `oarepo-model-builder-multilingual-2.0.8/LICENSE` & `oarepo-model-builder-multilingual-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.8/PKG-INFO` & `oarepo-model-builder-multilingual-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-multilingual
-Version: 2.0.8
+Version: 3.0.1
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo Model Builder Multilingual
 
 plugin for the [oarepo-model-builder module](https://github.com/oarepo/oarepo-model-builder) that adds support for
```

### Comparing `oarepo-model-builder-multilingual-2.0.8/README.md` & `oarepo-model-builder-multilingual-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py` & `oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2` & `oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual.egg-info/PKG-INFO` & `oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-multilingual
-Version: 2.0.8
+Version: 3.0.1
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo Model Builder Multilingual
 
 plugin for the [oarepo-model-builder module](https://github.com/oarepo/oarepo-model-builder) that adds support for
```

### Comparing `oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual.egg-info/SOURCES.txt` & `oarepo-model-builder-multilingual-3.0.1/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,57 @@
-LICENSE
-README.md
-pyproject.toml
-setup.cfg
-setup.py
-oarepo_model_builder_multilingual/__init__.py
-oarepo_model_builder_multilingual/faker.py
-oarepo_model_builder_multilingual/i18n.json5
-oarepo_model_builder_multilingual/multilingual_jsonschema.json5
-oarepo_model_builder_multilingual/multilingual_settings.json5
-oarepo_model_builder_multilingual/ui_jsonschema.json5
-oarepo_model_builder_multilingual.egg-info/PKG-INFO
-oarepo_model_builder_multilingual.egg-info/SOURCES.txt
-oarepo_model_builder_multilingual.egg-info/dependency_links.txt
-oarepo_model_builder_multilingual.egg-info/entry_points.txt
-oarepo_model_builder_multilingual.egg-info/requires.txt
-oarepo_model_builder_multilingual.egg-info/top_level.txt
-oarepo_model_builder_multilingual/builders/__init__.py
-oarepo_model_builder_multilingual/builders/mult_setup_cfg.py
-oarepo_model_builder_multilingual/builtin_models/__init__.py
-oarepo_model_builder_multilingual/builtin_models/i18n.json
-oarepo_model_builder_multilingual/datatypes/__init__.py
-oarepo_model_builder_multilingual/datatypes/multilings.py
-oarepo_model_builder_multilingual/invenio/__init__.py
-oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py
-oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py
-oarepo_model_builder_multilingual/invenio/invenio_search_multilingual.py
-oarepo_model_builder_multilingual/invenio/templates/__init__.py
-oarepo_model_builder_multilingual/invenio/templates/invenio_record_dumper_multilingual.py.jinja2
-oarepo_model_builder_multilingual/invenio/templates/invenio_record_multilingual.py.jinja2
-oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2
-oarepo_model_builder_multilingual/model_preprocessors/__init__.py
-oarepo_model_builder_multilingual/model_preprocessors/multilingual.py
-oarepo_model_builder_multilingual/property_preprocessors/__init__.py
-oarepo_model_builder_multilingual/property_preprocessors/i18nStr.py
-oarepo_model_builder_multilingual/property_preprocessors/multilingual.py
-oarepo_model_builder_multilingual/utils/__init__.py
-oarepo_model_builder_multilingual/utils/supported_langs.py
-oarepo_model_builder_multilingual/validation/__init__.py
-tests/__init__.py
-tests/mock_filesystem.py
-tests/model.json5
-tests/multilingual_schema.py
-tests/test_build_from_entrypoints.py
-tests/test_cfg.py
-tests/test_helper.py
-tests/test_i18nStr.py
-tests/test_marshmallow_ui.py
-tests/test_multi_facets.py
-tests/test_runtime.py
-tests/test_schema.py
-tests/test_ui.py
+[metadata]
+name = oarepo-model-builder-multilingual
+version = 3.0.1
+description = 
+authors = ["Alzbeta Pokorna <alzbeta.pokorna@cesnet.cz>"]
+readme = README.md
+long_description = file:README.md
+long_description_content_type = text/markdown
+
+[options]
+python = >=3.9
+install_requires = 
+	oarepo-model-builder-tests>=2.0.0
+	langcodes>=3.3.0
+packages = find:
+
+[options.package_data]
+* = *.json, *.rst, *.md, *.json5, *.jinja2
+
+[options.packages.find]
+exclude = example_model
+
+[options.entry_points]
+oarepo.models = 
+	i18n = oarepo_model_builder_multilingual.builtin_models:i18n.json
+oarepo_model_builder.builders.record = 
+	300-multilingual_record = oarepo_model_builder_multilingual.invenio.invenio_record_multilingual:InvenioRecordMultilingualBuilder
+	380-invenio_record_dumper = oarepo_model_builder_multilingual.invenio.invenio_record_dumper_multilingual:InvenioRecordMultilingualDumperBuilder
+	0100-mult-setup-cfg = oarepo_model_builder_multilingual.builders.mult_setup_cfg:MultSetupCfgBuilder
+oarepo_model_builder.validation.settings = 
+	languages-settings = oarepo_model_builder_multilingual.validation:LanguagesSettingsSchema
+oarepo_model_builder.templates = 
+	100-multilingual_templates = oarepo_model_builder_multilingual.invenio
+oarepo.model_schemas = 
+	es-strings = oarepo_model_builder_multilingual:multilingual_jsonschema.json5
+	mult-settings = oarepo_model_builder_multilingual:multilingual_settings.json5
+	i18n = oarepo_model_builder_multilingual:i18n.json5
+	ui = oarepo_model_builder_multilingual:ui_jsonschema.json5
+oarepo_model_builder.sample_data_providers = 
+	multilingual = oarepo_model_builder_multilingual.faker:multilingual_sample_provider
+oarepo_model_builder.datatypes = 
+	0200-multilingual-datatypes = oarepo_model_builder_multilingual.datatypes:MULTILINGUAL_TYPES
+oarepo_model_builder.datatypes.components = 
+	0100-default-multilingual-datatypes = oarepo_model_builder_multilingual.datatypes.components:DEFAULT_COMPONENTS
+
+[options.extras_require]
+tests = 
+	pytest
+
+[tool:pytest]
+testpaths = 
+	tests
+
+[egg_info]
+tag_build = 
+tag_date = 0
+
```

### Comparing `oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual.egg-info/entry_points.txt` & `oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual.egg-info/entry_points.txt`

 * *Files 18% similar despite different names*

```diff
@@ -3,30 +3,26 @@
 i18n = oarepo_model_builder_multilingual:i18n.json5
 mult-settings = oarepo_model_builder_multilingual:multilingual_settings.json5
 ui = oarepo_model_builder_multilingual:ui_jsonschema.json5
 
 [oarepo.models]
 i18n = oarepo_model_builder_multilingual.builtin_models:i18n.json
 
-[oarepo_model_builder.builders.model]
+[oarepo_model_builder.builders.record]
 0100-mult-setup-cfg = oarepo_model_builder_multilingual.builders.mult_setup_cfg:MultSetupCfgBuilder
-0301-invenio_record_search_options_multilang = oarepo_model_builder_multilingual.invenio.invenio_search_multilingual:InvenioRecordSearchOptionsBuilderMultilingual
+300-multilingual_record = oarepo_model_builder_multilingual.invenio.invenio_record_multilingual:InvenioRecordMultilingualBuilder
 380-invenio_record_dumper = oarepo_model_builder_multilingual.invenio.invenio_record_dumper_multilingual:InvenioRecordMultilingualDumperBuilder
 
 [oarepo_model_builder.datatypes]
 0200-multilingual-datatypes = oarepo_model_builder_multilingual.datatypes:MULTILINGUAL_TYPES
 
-[oarepo_model_builder.model_preprocessors.model]
-30-multilingual = oarepo_model_builder_multilingual.model_preprocessors.multilingual:MultilingualModelPreprocessor
-
-[oarepo_model_builder.property_preprocessors.model]
-1001-i18n = oarepo_model_builder_multilingual.property_preprocessors.i18nStr:I18nStrPreprocessor
-700-multilingual = oarepo_model_builder_multilingual.property_preprocessors.multilingual:MultilangPreprocessor
+[oarepo_model_builder.datatypes.components]
+0100-default-multilingual-datatypes = oarepo_model_builder_multilingual.datatypes.components:DEFAULT_COMPONENTS
 
 [oarepo_model_builder.sample_data_providers]
 multilingual = oarepo_model_builder_multilingual.faker:multilingual_sample_provider
 
 [oarepo_model_builder.templates]
 100-multilingual_templates = oarepo_model_builder_multilingual.invenio
 
-[oarepo_model_builder.validation]
-multilingual-validation = oarepo_model_builder_multilingual.validation:validators
+[oarepo_model_builder.validation.settings]
+languages-settings = oarepo_model_builder_multilingual.validation:LanguagesSettingsSchema
```

### Comparing `oarepo-model-builder-multilingual-2.0.8/setup.cfg` & `oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,55 @@
-[metadata]
-name = oarepo-model-builder-multilingual
-version = 2.0.8
-description = 
-authors = ["Alzbeta Pokorna <alzbeta.pokorna@cesnet.cz>"]
-readme = README.md
-long_description = file:README.md
-long_description_content_type = text/markdown
-
-[options]
-python = >=3.9
-install_requires = 
-	oarepo-model-builder-tests>=2.0.0
-	langcodes>=3.3.0
-packages = find:
-
-[options.package_data]
-* = *.json, *.rst, *.md, *.json5, *.jinja2
-
-[options.packages.find]
-exclude = example_model
-
-[options.entry_points]
-oarepo_model_builder.property_preprocessors.model = 
-	700-multilingual = oarepo_model_builder_multilingual.property_preprocessors.multilingual:MultilangPreprocessor
-	1001-i18n = oarepo_model_builder_multilingual.property_preprocessors.i18nStr:I18nStrPreprocessor
-oarepo.models = 
-	i18n = oarepo_model_builder_multilingual.builtin_models:i18n.json
-oarepo_model_builder.builders.model = 
-	0301-invenio_record_search_options_multilang = oarepo_model_builder_multilingual.invenio.invenio_search_multilingual:InvenioRecordSearchOptionsBuilderMultilingual
-	380-invenio_record_dumper = oarepo_model_builder_multilingual.invenio.invenio_record_dumper_multilingual:InvenioRecordMultilingualDumperBuilder
-	0100-mult-setup-cfg = oarepo_model_builder_multilingual.builders.mult_setup_cfg:MultSetupCfgBuilder
-oarepo_model_builder.validation = 
-	multilingual-validation = oarepo_model_builder_multilingual.validation:validators
-oarepo_model_builder.model_preprocessors.model = 
-	30-multilingual = oarepo_model_builder_multilingual.model_preprocessors.multilingual:MultilingualModelPreprocessor
-oarepo_model_builder.templates = 
-	100-multilingual_templates = oarepo_model_builder_multilingual.invenio
-oarepo.model_schemas = 
-	es-strings = oarepo_model_builder_multilingual:multilingual_jsonschema.json5
-	mult-settings = oarepo_model_builder_multilingual:multilingual_settings.json5
-	i18n = oarepo_model_builder_multilingual:i18n.json5
-	ui = oarepo_model_builder_multilingual:ui_jsonschema.json5
-oarepo_model_builder.sample_data_providers = 
-	multilingual = oarepo_model_builder_multilingual.faker:multilingual_sample_provider
-oarepo_model_builder.datatypes = 
-	0200-multilingual-datatypes = oarepo_model_builder_multilingual.datatypes:MULTILINGUAL_TYPES
-
-[options.extras_require]
-tests = 
-	pytest
-
-[tool:pytest]
-testpaths = 
-	tests
-
-[egg_info]
-tag_build = 
-tag_date = 0
-
+LICENSE
+README.md
+pyproject.toml
+setup.cfg
+setup.py
+oarepo_model_builder_multilingual/__init__.py
+oarepo_model_builder_multilingual/faker.py
+oarepo_model_builder_multilingual.egg-info/PKG-INFO
+oarepo_model_builder_multilingual.egg-info/SOURCES.txt
+oarepo_model_builder_multilingual.egg-info/dependency_links.txt
+oarepo_model_builder_multilingual.egg-info/entry_points.txt
+oarepo_model_builder_multilingual.egg-info/requires.txt
+oarepo_model_builder_multilingual.egg-info/top_level.txt
+oarepo_model_builder_multilingual/builders/__init__.py
+oarepo_model_builder_multilingual/builders/mult_setup_cfg.py
+oarepo_model_builder_multilingual/builtin_models/__init__.py
+oarepo_model_builder_multilingual/builtin_models/i18n.json
+oarepo_model_builder_multilingual/datatypes/__init__.py
+oarepo_model_builder_multilingual/datatypes/multilings.py
+oarepo_model_builder_multilingual/datatypes/components/__init__.py
+oarepo_model_builder_multilingual/datatypes/components/facets/__init__.py
+oarepo_model_builder_multilingual/datatypes/components/facets/i18n.py
+oarepo_model_builder_multilingual/datatypes/components/mapping/__init__.py
+oarepo_model_builder_multilingual/datatypes/components/mapping/field.py
+oarepo_model_builder_multilingual/datatypes/components/mapping/multi.py
+oarepo_model_builder_multilingual/datatypes/components/marshmallow/__init__.py
+oarepo_model_builder_multilingual/datatypes/components/marshmallow/i18n.py
+oarepo_model_builder_multilingual/datatypes/components/marshmallow/ui_i18n.py
+oarepo_model_builder_multilingual/datatypes/components/model/__init__.py
+oarepo_model_builder_multilingual/datatypes/components/model/multilingual_dumper.py
+oarepo_model_builder_multilingual/datatypes/components/multilingual/__init__.py
+oarepo_model_builder_multilingual/datatypes/components/multilingual/field.py
+oarepo_model_builder_multilingual/invenio/__init__.py
+oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py
+oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py
+oarepo_model_builder_multilingual/invenio/invenio_record_multilingual.py
+oarepo_model_builder_multilingual/invenio/templates/__init__.py
+oarepo_model_builder_multilingual/invenio/templates/invenio_record_dumper_multilingual.py.jinja2
+oarepo_model_builder_multilingual/invenio/templates/invenio_record_multilingual.py.jinja2
+oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2
+oarepo_model_builder_multilingual/utils/__init__.py
+oarepo_model_builder_multilingual/utils/supported_langs.py
+oarepo_model_builder_multilingual/validation/__init__.py
+tests/__init__.py
+tests/mock_filesystem.py
+tests/model.json5
+tests/multilingual_schema.py
+tests/test_build_from_entrypoints.py
+tests/test_cfg.py
+tests/test_helper.py
+tests/test_i18nStr.py
+tests/test_marshmallow_ui.py
+tests/test_multi_facets.py
+tests/test_schema.py
+tests/test_ui.py
```

### Comparing `oarepo-model-builder-multilingual-2.0.8/tests/mock_filesystem.py` & `oarepo-model-builder-multilingual-3.0.1/tests/mock_filesystem.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.8/tests/multilingual_schema.py` & `oarepo-model-builder-multilingual-3.0.1/tests/multilingual_schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.8/tests/test_build_from_entrypoints.py` & `oarepo-model-builder-multilingual-3.0.1/tests/test_build_from_entrypoints.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,23 +7,21 @@
 
 from tests.mock_filesystem import MockFilesystem
 from tests.test_helper import basic_schema
 
 DUMMY_YAML = "test.yaml"
 
 
-
-
 def test_json():
     schema = basic_schema()
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "records", "jsonschemas", "test-1.0.0.json")
     ).read()
     print(data)
     data = json.loads(data)
     assert data == {
@@ -49,223 +47,248 @@
 
 def test_mapping():
     schema = basic_schema()
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "records", "mappings", "os-v2", "test", "test-1.0.0.json")
     ).read()
     print(data)
     data = json.loads(data)
     assert data == {
-    "mappings": {
-        "properties": {
-            "a": {
-                "type": "nested",
-                "properties": {
-                    "lang": {
-                        "type": "keyword"
+        "mappings": {
+            "properties": {
+                "a": {
+                    "type": "nested",
+                    "properties": {
+                        "lang": {"type": "keyword"},
+                        "value": {
+                            "type": "text",
+                            "fields": {"keyword": {"type": "keyword"}},
+                        },
                     },
-                    "value": {
-                        "type": "text",
-                        "fields": {
-                            "keyword": {
-                                "type": "keyword"
-                            }
-                        }
-                    }
-                }
-            },
-            "a_cs": {
-                "type": "text",
-                "analyzer": "czech",
-                "fields": {
-                    "sort": {
-                        "type": "icu_collation_keyword",
-                        "index": False,
-                        "language": "cs"
-                    },
-                    "keyword": {
-                        "type": "keyword"
-                    }
-                }
-            },
-            "a_en": {
-                "type": "text",
-                "analyzer": "en",
-                "fields": {
-                    "sort": {
-                        "type": "icu_collation_keyword",
-                        "index": False,
-                        "language": "en"
-                    },
-                    "keyword": {
-                        "type": "keyword"
-                    }
-                }
-            },
-            "id": {
-                "type": "keyword"
-            },
-            "created": {
-                "type": "date"
-            },
-            "updated": {
-                "type": "date"
-            },
-            "$schema": {
-                "type": "keyword"
+                },
+                "a_cs": {
+                    "type": "text",
+                    "analyzer": "czech",
+                    "fields": {
+                        "sort": {
+                            "type": "icu_collation_keyword",
+                            "index": False,
+                            "language": "cs",
+                        },
+                        "keyword": {"type": "keyword"},
+                    },
+                },
+                "a_en": {
+                    "type": "text",
+                    "analyzer": "en",
+                    "fields": {
+                        "sort": {
+                            "type": "icu_collation_keyword",
+                            "index": False,
+                            "language": "en",
+                        },
+                        "keyword": {"type": "keyword"},
+                    },
+                },
+                "id": {"type": "keyword"},
+                "created": {
+                    "format": "strict_date_time||strict_date_time_no_millis||basic_date_time||basic_date_time_no_millis||basic_date||strict_date",
+                    "type": "date",
+                },
+                "updated": {
+                    "format": "strict_date_time||strict_date_time_no_millis||basic_date_time||basic_date_time_no_millis||basic_date||strict_date",
+                    "type": "date",
+                },
+                "$schema": {"type": "keyword"},
             }
         }
     }
-}
 
 
+def test_mapping2():
+    schema = load_model(
+        "test.yaml",
+        model_content={
+            "settings": {
+                "supported-langs": {"cs": {}, "en": {}},
+            },
+            "record": {
+                "module": {"qualified": "test"},
+                "properties": {
+                    "a": {"type": "i18nStr"},
+                    "b": {"properties": {"c": "multilingual"}},
+                },
+            },
+        },
+        isort=False,
+        black=False,
+        autoflake=False,
+    )
+
+    filesystem = InMemoryFileSystem()
+    builder = create_builder_from_entrypoints(filesystem=filesystem)
+
+    builder.build(schema, "record", ["record"], "")
+
+    data = builder.filesystem.open(
+        os.path.join("test", "records", "mappings", "os-v2", "test", "test-1.0.0.json")
+    ).read()
+    print(data)
+
 
 def test_dumper():
     schema = basic_schema()
 
     filesystem = MockFilesystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(os.path.join("test", "records", "api.py")).read()
-    assert "dumper_extensions = [MultilingualSearchDumper()]" in data
+    print(data)
+    data = str(data)
+    assert "dumper_extensions = [  MultilingualSearchDumper()]" in data
+
+
 def test_dumper_file():
     schema = load_model(
         "test.yaml",
-        "test",
         model_content={
             "settings": {
                 "supported-langs": {"cs": {}, "en": {}},
             },
-            "model": {
+            "record": {
+                "module": {"qualified": "test"},
                 "properties": {
-                    "h" : "keyword",
+                    "h": "keyword",
                     "a": {"type": "i18nStr"},
-                    "b": {
-                        "type": "multilingual"
-
+                    "b": {"type": "multilingual"},
+                    "jej": {
+                        "type": "array",
+                        "items": {
+                            "type": "object",
+                            "properties": {"kch": {"type": "multilingual"}},
+                        },
+                    },
+                    "c": {
+                        "type": "object",
+                        "properties": {
+                            "d": {"type": "array", "items": {"type": "multilingual"}},
+                            "f": {"type": "array", "items": {"type": "i18nStr"}},
+                        },
                     },
-                    "c": {"type": "object", "properties": {"d": {"type": "array", "items": {"type": "multilingual"}},
-                                                           "f": {"type": "array",
-                                                                 "items": {"type": "i18nStr"}}}}
                 },
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = MockFilesystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
-    data = builder.filesystem.open(os.path.join("test", "records", "multilingual_dumper.py")).read()
+    data = builder.filesystem.open(
+        os.path.join("test", "records", "multilingual_dumper.py")
+    ).read()
     print(data)
-    assert re.sub(r"\s", "", data) == re.sub(
-        r"\s",
-        "",
-        """
-
-from oarepo_runtime.i18n.dumper import MultilingualDumper
+    assert "/a" in re.sub(r"\s", "", data)
+    assert "/b" in re.sub(r"\s", "", data)
+    assert "/c/d" in re.sub(r"\s", "", data)
+    assert "/c/f" in re.sub(r"\s", "", data)
+    assert "/jej/kch" in re.sub(r"\s", "", data)
 
-class MultilingualSearchDumper(MultilingualDumper):
-    \"""TestRecord search dumper.\"""
-
-    paths = ['/a', '/b', '/c/d', '/c/f']
-    SUPPORTED_LANGS = ['cs', 'en']
-
-    def dump(self, record, data):
-        super().dump(record, data)
-
-    def load(self, record, data):
-        super().load(record, data)
-""",
-    )
 
 def test_generated_schema2():
     schema = load_model(
         "test.yaml",
-        "test",
         model_content={
             "settings": {
                 "supported-langs": {"cs": {}, "en": {}},
             },
-            "model": {
+            "record": {
+                "module": {"qualified": "test"},
                 "properties": {
-                    "a": {"type": "i18nStr", "marshmallow" : {"imports" : [{"import" :"test"}], "field-class": "FieldClassa", "arguments": ["test=cosi"]}},
+                    "a": {
+                        "type": "i18nStr",
+                        "marshmallow": {
+                            "imports": [{"import": "test"}],
+                            "field-class": "FieldClassa",
+                            "arguments": ["test=cosi"],
+                        },
+                    },
                     "b": {
                         "type": "i18nStr",
                         "marshmallow": {"arguments": ["test=cosi"]},
                         "multilingual": {
                             "lang-field": "language",
                             "value-field": "val",
                         },
                     },
                 },
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = MockFilesystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "services", "records", "schema.py")
     ).read()
     print(data)
 
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
 
-from invenio_records_resources.services.records.schema import BaseRecordSchema as InvenioBaseRecordSchema
 from marshmallow import ValidationError
 from marshmallow import validate as ma_validate
 import marshmallow as ma
-from marshmallow import fields as ma_fields
 from marshmallow_utils import fields as mu_fields
 from marshmallow_utils import schemas as mu_schemas
 
-
-
 from oarepo_runtime.i18n.schema import I18nStrField
+import test
 
 
 
-from test import test
 
 
+class TestSchema(ma.Schema):
 
+    class Meta:
+        unknown = ma.RAISE
 
 
-class TestSchema(ma.Schema):
-    \"""TestSchema schema.\"""
     a = FieldClassa(test=cosi)
+
     b = I18nStrField(test=cosi, lang_field=language, value_field=val)
+
     """,
     )
 
 
 def test_generated_schema():
     schema = load_model(
         DUMMY_YAML,
-        "test",
         model_content={
             "settings": {
                 "supported-langs": {
                     "cs": {
                         "text": {
                             "analyzer": "czech",
                         },
@@ -273,66 +296,63 @@
                     },
                     "en": {
                         "text": {"analyzer": "en"},
                         "sort": {"type": "icu_collation_keyword"},
                     },
                 }
             },
-            "model": {"properties": {"a": {"type": "multilingual"}}},
+            "record": {
+                "module": {"qualified": "test"},
+                "properties": {"a": {"type": "multilingual"}},
+            },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = MockFilesystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "services", "records", "schema.py")
     ).read()
     print(data)
 
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
 
-from invenio_records_resources.services.records.schema import BaseRecordSchema as InvenioBaseRecordSchema
 from marshmallow import ValidationError
 from marshmallow import validate as ma_validate
 import marshmallow as ma
-from marshmallow import fields as ma_fields
 from marshmallow_utils import fields as mu_fields
 from marshmallow_utils import schemas as mu_schemas
 
-
-
 from oarepo_runtime.i18n.schema import I18nStrField
-
-
-
 from oarepo_runtime.i18n.schema import MultilingualField
 
 
+class TestSchema(ma.Schema):
 
+    class Meta:
+        unknown = ma.RAISE
 
 
-class TestSchema(ma.Schema):
-    \"""TestSchema schema.\"""
     a = MultilingualField(I18nStrField())
     """,
     )
 
 
 def test_sample_data():
     schema = load_model(
         "test.yaml",
-        "test",
         model_content={
             "settings": {
                 "supported-langs": {
                     "cs": {
                         "text": {
                             "analyzer": "czech",
                         },
@@ -341,35 +361,37 @@
                     },
                     "en": {
                         "text": {"analyzer": "czech"},
                         "sort": {"type": "icu_collation_keyword"},
                     },
                 }
             },
-            "model": {
+            "record": {
+                "module": {"qualified": "test"},
                 "use": "invenio",
                 "sample": {"count": 1},
                 "properties": {
                     "a": {"type": "multilingual"},
                     "b": {"type": "i18nStr"},
                     "c": {
                         "type": "object",
                         "properties": {"d": "multilingual", "e": "keyword"},
                     },
                 },
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = MockFilesystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
     # file = builder.filesystem.open(os.path.join("data" ,"sample_data.yaml"))
     data_yaml = builder.filesystem.open(os.path.join("data", "sample_data.yaml")).read()
     import yaml
 
     yaml_docs = data_yaml.split("---")
     for doc in yaml_docs:
         if doc.strip():
```

### Comparing `oarepo-model-builder-multilingual-2.0.8/tests/test_cfg.py` & `oarepo-model-builder-multilingual-3.0.1/tests/test_cfg.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,12 @@
 
 def test_json():
     schema = basic_schema()
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
-
-
-    data = builder.filesystem.open(
-        os.path.join( "setup.cfg")
-    ).read()
+    builder.build(schema, "record", ["record"], "")
 
+    data = builder.filesystem.open(os.path.join("setup.cfg")).read()
 
     assert "deepmerge>=1.1.0" in data
```

### Comparing `oarepo-model-builder-multilingual-2.0.8/tests/test_i18nStr.py` & `oarepo-model-builder-multilingual-3.0.1/tests/test_i18nStr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 import json
 import os
 import re
 
-import yaml
 from oarepo_model_builder.entrypoints import create_builder_from_entrypoints, load_model
 
 from tests.mock_filesystem import MockFilesystem
 
 
 def test_generated_jsonschema():
     schema = load_model(
         "test.yaml",
-        "test",
         model_content={
             "settings": {
                 "supported-langs": {"cs": {}, "en": {}},
             },
-            "model": {
+            "record": {
+                "module": {"qualified": "test"},
                 "properties": {
                     "a": {"type": "i18nStr"},
                     "b": {
                         "type": "i18nStr",
                         "multilingual": {
                             "lang-field": "language",
                             "value-field": "val",
                         },
-                    },
+                    }
                 },
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = MockFilesystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "records", "jsonschemas", "test-1.0.0.json")
     ).read()
     print(data)
     data = json.loads(data)
     assert data == {
@@ -60,40 +60,41 @@
         },
     }
 
 
 def test_generated_mapping():
     schema = load_model(
         "test.yaml",
-        "test",
         model_content={
             "settings": {
                 "supported-langs": {"cs": {}, "en": {}},
             },
-            "model": {
+            "record": {
+                "module": {"qualified": "test"},
                 "properties": {
                     "a": {"type": "i18nStr"},
                     "b": {
                         "type": "i18nStr",
                         "multilingual": {
                             "lang-field": "language",
                             "value-field": "val",
                         },
                     },
                 },
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = MockFilesystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "records", "mappings", "os-v2", "test", "test-1.0.0.json")
     ).read()
     print(data)
     data = json.loads(data)
     assert data == {
@@ -127,105 +128,109 @@
         }
     }
 
 
 def test_generated_schema():
     schema = load_model(
         "test.yaml",
-        "test",
         model_content={
             "settings": {
                 "supported-langs": {"cs": {}, "en": {}},
             },
-            "model": {
+            "record": {
+                "module": {"qualified": "test"},
                 "properties": {
                     "a": {"type": "i18nStr"},
                     "b": {
                         "type": "i18nStr",
                         "multilingual": {
                             "lang-field": "language",
                             "value-field": "val",
                         },
                     },
+                    "c":{
+                        "properties": {
+                            "d" : "keyword"
+                        }
+                    }
                 },
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = MockFilesystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "services", "records", "schema.py")
     ).read()
     print(data)
 
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
-from invenio_records_resources.services.records.schema import BaseRecordSchema as InvenioBaseRecordSchema
 from marshmallow import ValidationError
 from marshmallow import validate as ma_validate
 import marshmallow as ma
-from marshmallow import fields as ma_fields
 from marshmallow_utils import fields as mu_fields
 from marshmallow_utils import schemas as mu_schemas
 
-
-
 from oarepo_runtime.i18n.schema import I18nStrField
 
 
+class TestSchema(ma.Schema):
 
+    class Meta:
+        unknown = ma.RAISE
 
 
-class TestSchema(ma.Schema):
-    \"""TestSchema schema.\"""
     a = I18nStrField()
+
     b = I18nStrField(lang_field=language, value_field=val)
+    
+    c = ma.fields.Nested(lambda: CSchema())
 
-    """,
-    )
+class CSchema(ma.Schema):
+
+    class Meta:
+        unknown = ma.RAISE
 
 
+    d = ma.fields.String()
+
+    """,
+    )
 
 
 def test_mapping():
     schema = load_model(
         "test.yaml",
-        "test",
         model_content={
             "settings": {"supported-langs": {"cs": {}, "en": {}}},
-            "model": {
+            "record": {
+                "module": {"qualified": "test"},
                 "properties": {
                     "a": {"type": "fulltext", "multilingual": {"i18n": True}}
-                }
+                },
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = MockFilesystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "records", "mappings", "os-v2", "test", "test-1.0.0.json")
     ).read()
     print(data)
-    data = json.loads(data)
-    assert data == {
-        "mappings": {
-            "properties": {
-                "a": {"type": "text"},
-                "a_cs": {"type": "text", "fields": {"keyword": {"type": "keyword"}}},
-                "a_en": {"type": "text", "fields": {"keyword": {"type": "keyword"}}},
-            }
-        }
-    }
+
```

### Comparing `oarepo-model-builder-multilingual-2.0.8/tests/test_marshmallow_ui.py` & `oarepo-model-builder-multilingual-3.0.1/tests/test_marshmallow_ui.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,75 +5,85 @@
 
 from tests.mock_filesystem import MockFilesystem
 
 
 def test_generated_schema_ui():
     schema = load_model(
         "test.yaml",
-        "test",
         model_content={
             "settings": {
                 "supported-langs": {"cs": {}, "en": {}},
             },
-            "model": {
+            "record": {
+                "module": {"qualified": "test"},
                 "properties": {
-                    "a": {"type": "multilingual", "ui": {
-                        "marshmallow": {"imports": [{"import": "test"}], "field-class": "FieldClassa",
-                                        "arguments": ["test=cosi"]}}},
-                    "b": {"type": "i18nStr", "ui": {
-                        "marshmallow": {"imports": [{"import": "test"}],
-                                        "arguments": ["test=cosi"]}},
-                          "multilingual": {"lang-field": "language", "value-field": "hodnota"}},
-
+                    "a": {
+                        "type": "multilingual",
+                        "ui": {
+                            "marshmallow": {
+                                "imports": [{"import": "test"}],
+                                "field-class": "FieldClassa",
+                                "arguments": ["test=cosi"],
+                            }
+                        },
+                    },
+                    "b": {
+                        "type": "i18nStr",
+                        "ui": {
+                            "marshmallow": {
+                                "imports": [{"import": "test"}],
+                                "arguments": ["test=cosi"],
+                            }
+                        },
+                        "multilingual": {
+                            "lang-field": "language",
+                            "value-field": "hodnota",
+                        },
+                    },
                 },
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = MockFilesystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "services", "records", "ui_schema.py")
     ).read()
     print(data)
 
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
 
-from invenio_records_resources.services.records.schema import BaseRecordSchema as InvenioBaseRecordSchema
 from marshmallow import ValidationError
 from marshmallow import validate as ma_validate
 import marshmallow as ma
-from marshmallow import fields as ma_fields
 from marshmallow_utils import fields as mu_fields
 from marshmallow_utils import schemas as mu_schemas
 
-
-
 from oarepo_runtime.i18n.ui_schema import I18nStrUIField
-
-
-
 from oarepo_runtime.i18n.ui_schema import MultilingualUIField
-
-
 from oarepo_runtime.ui.marshmallow import InvenioUISchema
-
-from test import test
+import test
 
 
 
 
 
-class TestUISchema(ma.Schema):
-    \"""TestUISchema schema.\"""
-    a = FieldClassa(I18nStrUIField())
+class TestUISchema(InvenioUISchema):
+    
+     class Meta:
+        unknown = ma.RAISE
+        
+        
+    a = FieldClassa(I18nStrUIField(), test=cosi)
     b = I18nStrUIField(test=cosi, lang_field=language, value_field=hodnota)
     """,
     )
```

### Comparing `oarepo-model-builder-multilingual-2.0.8/tests/test_multi_facets.py` & `oarepo-model-builder-multilingual-3.0.1/tests/test_multi_facets.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from tests.mock_filesystem import MockFilesystem
 
 
 def test_search_options():
     schema = load_model(
         "test.yaml",
-        "test",
         model_content={
             "settings": {
                 "supported-langs": {
                     "cs": {
                         "text": {
                             "analyzer": "czech",
                         },
@@ -22,27 +21,29 @@
                     },
                     "en": {
                         "text": {"analyzer": "czech"},
                         "sort": {"type": "icu_collation_keyword"},
                     },
                 }
             },
-            "model": {
+            "record": {
                 "use": "invenio",
-                "properties": {"a": {"type": "multilingual", "sortable": {}}},
+                "module": {"qualified": "test"},
+                "properties": {"a": {"type": "multilingual"}},
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = MockFilesystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "services", "records", "search.py")
     ).read()
 
     print(data)
     assert re.sub(r"\s", "", data) == re.sub(
@@ -57,75 +58,59 @@
 
 class TestSearchOptions(InvenioSearchOptions):
     \"""TestRecord search options.\"""
 
     facets = {
 
 
-    'a_lang': facets.a_lang,
+    '_schema': facets._schema,
 
 
 
-    'a_cs_keyword': facets.a_cs_keyword,
+    'a_cs': facets.a_cs,
 
 
 
-    'a_en_keyword': facets.a_en_keyword,
+    'a_en': facets.a_en,
 
 
 
-    'a_value_keyword': facets.a_value_keyword,
+    'a_lang': facets.a_lang,
 
 
 
-    '_id': facets._id,
+    'a_value': facets.a_value,
 
 
 
     'created': facets.created,
 
 
 
-    'updated': facets.updated,
+    '_id': facets._id,
 
 
 
-    '_schema': facets._schema,
+    'updated': facets.updated,
 
 
     }
     sort_options = {
         
         **InvenioSearchOptions.sort_options,
         
 
-
-    'a': {'fields': ['a']},"bestmatch": dict(
-                title=_('Best match'),
-                fields=['_score'],  # ES defaults to desc on `_score` field
-            ),
-            "newest": dict(
-                title=_('Newest'),
-                fields=['-created'],
-            ),
-            "oldest": dict(
-                title=_('Oldest'),
-                fields=['created'],
-            ),
-
-
     }
     """,
     )
 
 
 def test_facets():
     schema = load_model(
         "test.yaml",
-        "test",
         model_content={
             "settings": {
                 "supported-langs": {
                     "cs": {
                         "text": {
                             "analyzer": "czech",
                         },
@@ -134,16 +119,17 @@
                     },
                     "en": {
                         "text": {"analyzer": "czech"},
                         "sort": {"type": "icu_collation_keyword"},
                     },
                 }
             },
-            "model": {
+            "record": {
                 "use": "invenio",
+                "module": {"qualified": "test"},
                 "properties": {
                     "d": {
                         "use": "i18n",
                         "properties": {
                             "navic": {
                                 "type": "object",
                                 "properties": {"kxh": {"type": "keyword"}},
@@ -151,30 +137,31 @@
                         },
                     },
                     "b": "keyword",
                     "c": {
                         "type": "i18nStr",
                         "multilingual": {"lang-field": "language"},
                     },
-                    "a": {"type": "multilingual", "sortable": {}},
+                    "a": {"type": "multilingual"},
                     "e": {
                         "type": "object",
                         "properties": {"f": "keyword", "g": "i18nStr"},
                     },
                 },
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = MockFilesystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "services", "records", "facets.py")
     ).read()
 
     print(data)
     assert re.sub(r"\s", "", data) == re.sub(
@@ -182,116 +169,88 @@
         "",
         """
 \"""Facet definitions.\"""
 
 from invenio_search.engine import dsl
 from flask_babelex import lazy_gettext as _
 
-
-
 from invenio_records_resources.services.records.facets import TermsFacet
-
-
-
 from oarepo_runtime.facets.date import DateTimeFacet
-
-
-
 from oarepo_runtime.facets.nested_facet import NestedLabeledFacet
 
 
 
+_schema = TermsFacet(field='$schema', label =_('$schema.label'))
 
+a_cs = TermsFacet(field=a.cs.keyword, label =_('a.label'))
 
+a_en = TermsFacet(field=a.en.keyword, label =_('a.label'))
 
-d_navic_kxh = NestedLabeledFacet(path ="d", nested_facet = TermsFacet(field="d.navic.kxh", label=_("d/navic/kxh.label")))
-
-
-
-d_lang = NestedLabeledFacet(path ="d", nested_facet = TermsFacet(field="d.lang", label=_("d/lang.label")))
-
-
-
-d_cs_keyword = TermsFacet(field="d_cs.keyword")
-
-
-
-d_en_keyword = TermsFacet(field="d_en.keyword")
-
-
-
-d_value_keyword = NestedLabeledFacet(path ="d", nested_facet = TermsFacet(field="d.value.keyword", label=_("d/value/keyword.label")))
-
-
-
-b = TermsFacet(field="b", label=_("b.label"))
-
-
-
-c_language = NestedLabeledFacet(path ="c", nested_facet = TermsFacet(field="c.language", label=_("c/language.label")))
-
-
+a_lang = NestedLabeledFacet(path = 'a', nested_facet = TermsFacet(field='a.lang', label =_('a/lang.label')))
 
-c_cs_keyword = TermsFacet(field="c_cs.keyword")
+a_value = NestedLabeledFacet(path = 'a', nested_facet = TermsFacet(field='a.value.keyword', label =_('a/value.label')))
 
+b = TermsFacet(field='b', label =_('b.label'))
 
+c_cs = TermsFacet(field=c.cs.keyword, label =_('c.label'))
 
-c_en_keyword = TermsFacet(field="c_en.keyword")
+c_en = TermsFacet(field=c.en.keyword, label =_('c.label'))
 
+c_language = NestedLabeledFacet(path = 'c', nested_facet = TermsFacet(field='c.language', label =_('c/language.label')))
 
+c_value = NestedLabeledFacet(path = 'c', nested_facet = TermsFacet(field='c.value.keyword', label =_('c/value.label')))
 
-c_value_keyword = NestedLabeledFacet(path ="c", nested_facet = TermsFacet(field="c.value.keyword", label=_("c/value/keyword.label")))
+created = DateTimeFacet(field='created', label =_('created.label'))
 
+d_cs = TermsFacet(field=d.cs.keyword, label =_('d.label'))
 
+d_en = TermsFacet(field=d.en.keyword, label =_('d.label'))
 
-a_lang = NestedLabeledFacet(path ="a", nested_facet = TermsFacet(field="a.lang", label=_("a/lang.label")))
+d_lang = NestedLabeledFacet(path = 'd', nested_facet = TermsFacet(field='d.lang', label =_('d/lang.label')))
 
+d_navic_kxh = NestedLabeledFacet(path = 'd', nested_facet = TermsFacet(field='d.navic.kxh', label =_('d/navic/kxh.label')))
 
+d_value = NestedLabeledFacet(path = 'd', nested_facet = TermsFacet(field='d.value.keyword', label =_('d/value.label')))
 
-a_cs_keyword = TermsFacet(field="a_cs.keyword")
+e_f = TermsFacet(field='e.f', label =_('e/f.label'))
 
+e_g_cs = TermsFacet(field=e.g.cs.keyword, label =_('e/g.label'))
 
+e_g_en = TermsFacet(field=e.g.en.keyword, label =_('e/g.label'))
 
-a_en_keyword = TermsFacet(field="a_en.keyword")
+e_g_lang = NestedLabeledFacet(path = 'e.g', nested_facet = TermsFacet(field='e.g.lang', label =_('e/g/lang.label')))
 
+e_g_value = NestedLabeledFacet(path = 'e.g', nested_facet = TermsFacet(field='e.g.value.keyword', label =_('e/g/value.label')))
 
+_id = TermsFacet(field='id', label =_('id.label'))
 
-a_value_keyword = NestedLabeledFacet(path ="a", nested_facet = TermsFacet(field="a.value.keyword", label=_("a/value/keyword.label")))
+updated = DateTimeFacet(field='updated', label =_('updated.label'))
 
 
 
-e_f = TermsFacet(field="e.f", label=_("e/f.label"))
 
 
 
-e_g_lang = NestedLabeledFacet(path ="e.g", nested_facet = TermsFacet(field="e.g.lang", label=_("e/g/lang.label")))
 
 
 
-e_g_cs_keyword = TermsFacet(field="e.g_cs.keyword")
 
 
 
-e_g_en_keyword = TermsFacet(field="e.g_en.keyword")
 
 
 
-e_g_value_keyword = NestedLabeledFacet(path ="e.g", nested_facet = TermsFacet(field="e.g.value.keyword", label=_("e/g/value/keyword.label")))
 
 
 
-_id = TermsFacet(field="id", label=_("id.label"))
 
 
 
-created = DateTimeFacet(field="created", label=_("created.label"))
 
 
 
-updated = DateTimeFacet(field="updated", label=_("updated.label"))
 
 
 
-_schema = TermsFacet(field="$schema", label=_("$schema.label"))
 
     """,
     )
```

### Comparing `oarepo-model-builder-multilingual-2.0.8/tests/test_schema.py` & `oarepo-model-builder-multilingual-3.0.1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.8/tests/test_ui.py` & `oarepo-model-builder-multilingual-3.0.1/tests/test_ui.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 from tests.mock_filesystem import MockFilesystem
 
 
 def test_validity():
     schema = load_model(
         "test.yaml",
-        "test",
         model_content={
             "settings": {
                 "supported-langs": {
                     "en": {
                         "text": {"analyzer": "czech"},
                         "sort": {"type": "icu_collation_keyword"},
                     }
                 }
             },
-            "model": {
+            "record": {
                 "use": "invenio",
                 "properties": {"a": {"type": "multilingual", "ui": {}}},
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = MockFilesystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
```

