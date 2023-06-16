# Comparing `tmp/oarepo-model-builder-multilingual-3.0.1.tar.gz` & `tmp/oarepo-model-builder-multilingual-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-multilingual-3.0.1.tar", last modified: Fri Jun 16 11:05:34 2023, max compression
+gzip compressed data, was "oarepo-model-builder-multilingual-3.0.2.tar", last modified: Fri Jun 16 12:16:14 2023, max compression
```

## Comparing `oarepo-model-builder-multilingual-3.0.1.tar` & `oarepo-model-builder-multilingual-3.0.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.396382 oarepo-model-builder-multilingual-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-16 11:05:34.396382 oarepo-model-builder-multilingual-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.380382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.384382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/builders/mult_setup_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.384382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/builtin_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/builtin_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/builtin_models/i18n.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.384382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.384382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.384382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/facets/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/facets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/facets/i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.388382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/mapping/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/mapping/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/mapping/multi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.388382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/marshmallow/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/marshmallow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/marshmallow/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/marshmallow/ui_i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.388382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/model/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/model/multilingual_dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.388382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/multilingual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/multilingual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/multilingual/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/multilings.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/faker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.388382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/invenio_record_multilingual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.392382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/templates/invenio_record_dumper_multilingual.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/templates/invenio_record_multilingual.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.392382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/utils/supported_langs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.392382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.380382 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-16 11:05:34.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-16 11:05:34.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:05:34.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-16 11:05:34.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-16 11:05:34.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-16 11:05:34.000000 oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-16 11:05:34.396382 oarepo-model-builder-multilingual-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:05:34.396382 oarepo-model-builder-multilingual-3.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/tests/mock_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/tests/model.json5
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/tests/multilingual_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/tests/test_build_from_entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/tests/test_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/tests/test_i18nStr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/tests/test_marshmallow_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/tests/test_multi_facets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-16 11:04:56.000000 oarepo-model-builder-multilingual-3.0.1/tests/test_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:16:14.615229 oarepo-model-builder-multilingual-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-16 12:16:14.615229 oarepo-model-builder-multilingual-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:16:14.611229 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:16:14.611229 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/builders/mult_setup_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:16:14.611229 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/builtin_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/builtin_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/builtin_models/i18n.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:16:14.611229 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:16:14.611229 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:16:14.611229 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/facets/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/facets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/facets/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:16:14.611229 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/mapping/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/mapping/multi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:16:14.611229 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/marshmallow/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/marshmallow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/marshmallow/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/marshmallow/ui_i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:16:14.615229 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/model/multilingual_dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:16:14.615229 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/multilingual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/multilingual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/multilingual/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/multilings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/faker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:16:14.615229 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/invenio/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/invenio/invenio_record_multilingual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:16:14.615229 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/invenio/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/invenio/templates/invenio_record_dumper_multilingual.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/invenio/templates/invenio_record_multilingual.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:16:14.615229 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/utils/supported_langs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:16:14.615229 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:16:14.611229 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-16 12:16:14.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-16 12:16:14.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:16:14.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-16 12:16:14.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-16 12:16:14.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-16 12:16:14.000000 oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-16 12:16:14.615229 oarepo-model-builder-multilingual-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:16:14.615229 oarepo-model-builder-multilingual-3.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/tests/mock_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/tests/model.json5
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/tests/multilingual_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/tests/test_build_from_entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/tests/test_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/tests/test_i18nStr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/tests/test_marshmallow_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/tests/test_multi_facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-16 12:15:45.000000 oarepo-model-builder-multilingual-3.0.2/tests/test_ui.py
```

### Comparing `oarepo-model-builder-multilingual-3.0.1/LICENSE` & `oarepo-model-builder-multilingual-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.1/PKG-INFO` & `oarepo-model-builder-multilingual-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-multilingual
-Version: 3.0.1
+Version: 3.0.2
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo Model Builder Multilingual
 
 plugin for the [oarepo-model-builder module](https://github.com/oarepo/oarepo-model-builder) that adds support for
```

### Comparing `oarepo-model-builder-multilingual-3.0.1/README.md` & `oarepo-model-builder-multilingual-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/__init__.py` & `oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/facets/i18n.py` & `oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/facets/i18n.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/mapping/multi.py` & `oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/mapping/multi.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from oarepo_model_builder.datatypes import (
     ArrayDataType,
     DataTypeComponent,
     ModelDataType,
-    NestedDataType,
+    NestedDataType, datatypes,
 )
 from oarepo_model_builder.utils.deepmerge import deepmerge
 
 from oarepo_model_builder_multilingual.datatypes import (
     I18nDataType,
     MultilingualDataType,
 )
@@ -14,15 +14,27 @@
 
 from .field import RegularMultilingualMappingComponent
 
 
 class FieldMultilingualMappingComponent(RegularMultilingualMappingComponent):
     eligible_datatypes = [MultilingualDataType, I18nDataType]
 
-    def after_model_prepare(self, datatype, *, context, **kwargs):
+    def create_alternative_mapping(self, datatype, *, context, **kwargs):
+
+        if hasattr(datatype.parent, 'mapping_type') and datatype.parent.mapping_type == 'multilingual':
+            return #alternative mapping already added by parent
+
+        if not datatype.key:
+            key = datatype.parent.key
+            node = datatype.parent.parent
+        else:
+            key = datatype.key
+            node = datatype.parent
+
         alternative = alternative_gen(
-            datatype.schema.settings["supported_langs"], datatype.key
+            datatype.schema.settings["supported_langs"], key
         )
+
         if "properties" in datatype.parent.section_mapping.config:
-            deepmerge(datatype.parent.section_mapping.config["properties"], alternative)
+            deepmerge(node.section_mapping.config["properties"], alternative)
         else:
-            datatype.parent.section_mapping.config["properties"] = alternative
+            node.section_mapping.config["properties"] = alternative
```

### Comparing `oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/marshmallow/i18n.py` & `oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/marshmallow/i18n.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/marshmallow/ui_i18n.py` & `oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/marshmallow/ui_i18n.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/model/multilingual_dumper.py` & `oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/model/multilingual_dumper.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/components/multilingual/field.py` & `oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/components/multilingual/field.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/datatypes/multilings.py` & `oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/datatypes/multilings.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/faker.py` & `oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/faker.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py` & `oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py` & `oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2` & `oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/utils/supported_langs.py` & `oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/utils/supported_langs.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual/validation/__init__.py` & `oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual.egg-info/PKG-INFO` & `oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-multilingual
-Version: 3.0.1
+Version: 3.0.2
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo Model Builder Multilingual
 
 plugin for the [oarepo-model-builder module](https://github.com/oarepo/oarepo-model-builder) that adds support for
```

### Comparing `oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual.egg-info/SOURCES.txt` & `oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.1/oarepo_model_builder_multilingual.egg-info/entry_points.txt` & `oarepo-model-builder-multilingual-3.0.2/oarepo_model_builder_multilingual.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.1/setup.cfg` & `oarepo-model-builder-multilingual-3.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-multilingual
-version = 3.0.1
+version = 3.0.2
 description = 
 authors = ["Alzbeta Pokorna <alzbeta.pokorna@cesnet.cz>"]
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

### Comparing `oarepo-model-builder-multilingual-3.0.1/tests/mock_filesystem.py` & `oarepo-model-builder-multilingual-3.0.2/tests/mock_filesystem.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.1/tests/multilingual_schema.py` & `oarepo-model-builder-multilingual-3.0.2/tests/multilingual_schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.1/tests/test_build_from_entrypoints.py` & `oarepo-model-builder-multilingual-3.0.2/tests/test_build_from_entrypoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,16 +116,15 @@
         model_content={
             "settings": {
                 "supported-langs": {"cs": {}, "en": {}},
             },
             "record": {
                 "module": {"qualified": "test"},
                 "properties": {
-                    "a": {"type": "i18nStr"},
-                    "b": {"properties": {"c": "multilingual"}},
+                    "b[]": {"properties": {"c": "multilingual"}},
                 },
             },
         },
         isort=False,
         black=False,
         autoflake=False,
     )
@@ -135,14 +134,19 @@
 
     builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "records", "mappings", "os-v2", "test", "test-1.0.0.json")
     ).read()
     print(data)
+    # data = builder.filesystem.open(
+    #     os.path.join("test", "services", "records", "facets.py")
+    # ).read()
+    #
+    # print(data)
 
 
 def test_dumper():
     schema = basic_schema()
 
     filesystem = MockFilesystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
```

### Comparing `oarepo-model-builder-multilingual-3.0.1/tests/test_cfg.py` & `oarepo-model-builder-multilingual-3.0.2/tests/test_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.1/tests/test_helper.py` & `oarepo-model-builder-multilingual-3.0.2/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.1/tests/test_i18nStr.py` & `oarepo-model-builder-multilingual-3.0.2/tests/test_i18nStr.py`

 * *Files 13% similar despite different names*

```diff
@@ -207,19 +207,39 @@
     )
 
 
 def test_mapping():
     schema = load_model(
         "test.yaml",
         model_content={
-            "settings": {"supported-langs": {"cs": {}, "en": {}}},
+            "settings": {
+                "supported-langs": {"cs": {}, "en": {}},
+            },
             "record": {
                 "module": {"qualified": "test"},
                 "properties": {
-                    "a": {"type": "fulltext", "multilingual": {"i18n": True}}
+                    # "h": "keyword",
+                    # "a": {"type": "i18nStr"},
+                    # "b": {"type": "multilingual"},
+                    # "jej": {
+                    #     "type": "array",
+                    #     "items": {
+                    #         "type": "object",
+                    #         "properties": {"kch": {"type": "multilingual"}},
+                    #     },
+                    # },
+                    "c": {
+                        "type": "object",
+                        "properties": {
+                            "f": {"type": "array", "items": {"type": "i18nStr"}},
+                            "d": {"type": "array", "items": {"type": "multilingual"}},
+
+                        },
+
+                    },
                 },
             },
         },
         isort=False,
         black=False,
         autoflake=False,
     )
```

### Comparing `oarepo-model-builder-multilingual-3.0.1/tests/test_marshmallow_ui.py` & `oarepo-model-builder-multilingual-3.0.2/tests/test_marshmallow_ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.1/tests/test_multi_facets.py` & `oarepo-model-builder-multilingual-3.0.2/tests/test_multi_facets.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.1/tests/test_schema.py` & `oarepo-model-builder-multilingual-3.0.2/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.1/tests/test_ui.py` & `oarepo-model-builder-multilingual-3.0.2/tests/test_ui.py`

 * *Files identical despite different names*

