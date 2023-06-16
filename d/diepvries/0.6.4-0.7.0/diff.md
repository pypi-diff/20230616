# Comparing `tmp/diepvries-0.6.4.tar.gz` & `tmp/diepvries-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diepvries-0.6.4.tar", last modified: Wed Mar  1 12:08:38 2023, max compression
+gzip compressed data, was "diepvries-0.7.0.tar", last modified: Fri Jun 16 14:06:31 2023, max compression
```

## Comparing `diepvries-0.6.4.tar` & `diepvries-0.7.0.tar`

### file list

```diff
@@ -1,99 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:08:38.191596 diepvries-0.6.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:08:38.183596 diepvries-0.6.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:08:38.183596 diepvries-0.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-03-01 12:08:09.000000 diepvries-0.6.4/.github/workflows/pages-build-and-deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-01 12:08:09.000000 diepvries-0.6.4/.github/workflows/pypi-build-and-deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-01 12:08:09.000000 diepvries-0.6.4/.github/workflows/run-test-suite.yml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-01 12:08:09.000000 diepvries-0.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-01 12:08:09.000000 diepvries-0.6.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-03-01 12:08:09.000000 diepvries-0.6.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-03-01 12:08:09.000000 diepvries-0.6.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-03-01 12:08:09.000000 diepvries-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-03-01 12:08:38.191596 diepvries-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-03-01 12:08:09.000000 diepvries-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:08:38.187596 diepvries-0.6.4/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc/advanced-topics.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc/naming-conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc/philosophy.rst
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc/security.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:08:38.187596 diepvries-0.6.4/doc/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc/snippets/deserializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc/snippets/dv_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc/snippets/effsat.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc/snippets/effsat_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc/snippets/extract.sql
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc/snippets/h_customer.sql
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc/snippets/h_order.sql
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc/snippets/l_order_customer.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc/snippets/nodeserializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc/snippets/rph.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc/snippets/rph_deserializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:08:38.187596 diepvries-0.6.4/doc/static/
--rw-r--r--   0 runner    (1001) docker     (123)    32153 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc/static/diepvries-round.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc/static/diepvries-square.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21652 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc/static/diepvries.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc/tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:08:38.187596 diepvries-0.6.4/doc_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc_templates/package.rst_t
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-01 12:08:09.000000 diepvries-0.6.4/doc_templates/toc.rst_t
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-01 12:08:09.000000 diepvries-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-01 12:08:38.195596 diepvries-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-01 12:08:09.000000 diepvries-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:08:38.183596 diepvries-0.6.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:08:38.187596 diepvries-0.6.4/src/diepvries/
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-03-01 12:08:09.000000 diepvries-0.6.4/src/diepvries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-03-01 12:08:09.000000 diepvries-0.6.4/src/diepvries/data_vault_load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:08:38.191596 diepvries-0.6.4/src/diepvries/deserializers/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-01 12:08:09.000000 diepvries-0.6.4/src/diepvries/deserializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-03-01 12:08:09.000000 diepvries-0.6.4/src/diepvries/deserializers/snowflake_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-01 12:08:09.000000 diepvries-0.6.4/src/diepvries/deserializers/snowflake_model_metadata.sql
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-03-01 12:08:09.000000 diepvries-0.6.4/src/diepvries/driving_key_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-03-01 12:08:09.000000 diepvries-0.6.4/src/diepvries/effectivity_satellite.py
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-03-01 12:08:09.000000 diepvries-0.6.4/src/diepvries/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-03-01 12:08:09.000000 diepvries-0.6.4/src/diepvries/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-03-01 12:08:09.000000 diepvries-0.6.4/src/diepvries/link.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 12:08:09.000000 diepvries-0.6.4/src/diepvries/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-03-01 12:08:09.000000 diepvries-0.6.4/src/diepvries/role_playing_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-03-01 12:08:09.000000 diepvries-0.6.4/src/diepvries/satellite.py
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-03-01 12:08:09.000000 diepvries-0.6.4/src/diepvries/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:08:38.191596 diepvries-0.6.4/src/diepvries/template_sql/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-01 12:08:09.000000 diepvries-0.6.4/src/diepvries/template_sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-03-01 12:08:09.000000 diepvries-0.6.4/src/diepvries/template_sql/effectivity_satellite_dml.sql
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-01 12:08:09.000000 diepvries-0.6.4/src/diepvries/template_sql/hub_link_dml.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-03-01 12:08:09.000000 diepvries-0.6.4/src/diepvries/template_sql/satellite_dml.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-03-01 12:08:09.000000 diepvries-0.6.4/src/diepvries/template_sql/sql_formulas.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-01 12:08:09.000000 diepvries-0.6.4/src/diepvries/template_sql/staging_table_ddl.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:08:38.191596 diepvries-0.6.4/src/diepvries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-03-01 12:08:38.000000 diepvries-0.6.4/src/diepvries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-03-01 12:08:38.000000 diepvries-0.6.4/src/diepvries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 12:08:38.000000 diepvries-0.6.4/src/diepvries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-01 12:08:38.000000 diepvries-0.6.4/src/diepvries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-01 12:08:38.000000 diepvries-0.6.4/src/diepvries.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:08:38.191596 diepvries-0.6.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-01 12:08:09.000000 diepvries-0.6.4/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24383 2023-03-01 12:08:09.000000 diepvries-0.6.4/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:08:38.191596 diepvries-0.6.4/test/deserializers/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-01 12:08:09.000000 diepvries-0.6.4/test/deserializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-03-01 12:08:09.000000 diepvries-0.6.4/test/deserializers/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24045 2023-03-01 12:08:09.000000 diepvries-0.6.4/test/deserializers/model_metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-03-01 12:08:09.000000 diepvries-0.6.4/test/deserializers/test_snowflake_deserializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:08:38.191596 diepvries-0.6.4/test/sql/
--rw-r--r--   0 runner    (1001) docker     (123)    23067 2023-03-01 12:08:09.000000 diepvries-0.6.4/test/sql/expected_result_data_vault_load.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-03-01 12:08:09.000000 diepvries-0.6.4/test/sql/expected_result_effectivity_satellite.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-03-01 12:08:09.000000 diepvries-0.6.4/test/sql/expected_result_hashdiff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-01 12:08:09.000000 diepvries-0.6.4/test/sql/expected_result_hashkey.sql
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-01 12:08:09.000000 diepvries-0.6.4/test/sql/expected_result_hub.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-03-01 12:08:09.000000 diepvries-0.6.4/test/sql/expected_result_link.sql
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-01 12:08:09.000000 diepvries-0.6.4/test/sql/expected_result_role_playing_hub.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-03-01 12:08:09.000000 diepvries-0.6.4/test/sql/expected_result_satellite.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-03-01 12:08:09.000000 diepvries-0.6.4/test/sql/expected_result_staging.sql
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-01 12:08:09.000000 diepvries-0.6.4/test/test_data_vault_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    14880 2023-03-01 12:08:09.000000 diepvries-0.6.4/test/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-03-01 12:08:09.000000 diepvries-0.6.4/test/test_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-03-01 12:08:09.000000 diepvries-0.6.4/test/test_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-03-01 12:08:09.000000 diepvries-0.6.4/test/test_satellite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-03-01 12:08:09.000000 diepvries-0.6.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:31.881083 diepvries-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:31.837083 diepvries-0.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:31.845083 diepvries-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-16 14:06:04.000000 diepvries-0.7.0/.github/workflows/pages-build-and-deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-16 14:06:04.000000 diepvries-0.7.0/.github/workflows/pypi-build-and-deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-16 14:06:04.000000 diepvries-0.7.0/.github/workflows/run-test-suite.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-16 14:06:04.000000 diepvries-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-16 14:06:04.000000 diepvries-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-16 14:06:04.000000 diepvries-0.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-06-16 14:06:04.000000 diepvries-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-16 14:06:04.000000 diepvries-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-16 14:06:31.881083 diepvries-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-16 14:06:04.000000 diepvries-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:31.849083 diepvries-0.7.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc/advanced-topics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc/naming-conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc/philosophy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc/security.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:31.853083 diepvries-0.7.0/doc/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc/snippets/deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc/snippets/dv_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc/snippets/effsat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc/snippets/effsat_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc/snippets/extract.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc/snippets/h_customer.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc/snippets/h_order.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc/snippets/l_order_customer.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc/snippets/nodeserializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc/snippets/rph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc/snippets/rph_deserializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:31.857083 diepvries-0.7.0/doc/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    32153 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc/static/diepvries-round.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc/static/diepvries-square.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21652 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc/static/diepvries.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:31.857083 diepvries-0.7.0/doc_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc_templates/package.rst_t
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-16 14:06:04.000000 diepvries-0.7.0/doc_templates/toc.rst_t
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-16 14:06:04.000000 diepvries-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-16 14:06:31.881083 diepvries-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-16 14:06:04.000000 diepvries-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:31.837083 diepvries-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:31.861083 diepvries-0.7.0/src/diepvries/
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-16 14:06:04.000000 diepvries-0.7.0/src/diepvries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-06-16 14:06:04.000000 diepvries-0.7.0/src/diepvries/data_vault_load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:31.865083 diepvries-0.7.0/src/diepvries/deserializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-16 14:06:04.000000 diepvries-0.7.0/src/diepvries/deserializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-06-16 14:06:04.000000 diepvries-0.7.0/src/diepvries/deserializers/snowflake_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-16 14:06:04.000000 diepvries-0.7.0/src/diepvries/deserializers/snowflake_model_metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-16 14:06:04.000000 diepvries-0.7.0/src/diepvries/driving_key_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-06-16 14:06:04.000000 diepvries-0.7.0/src/diepvries/effectivity_satellite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-06-16 14:06:04.000000 diepvries-0.7.0/src/diepvries/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-06-16 14:06:04.000000 diepvries-0.7.0/src/diepvries/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-16 14:06:04.000000 diepvries-0.7.0/src/diepvries/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:04.000000 diepvries-0.7.0/src/diepvries/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-16 14:06:04.000000 diepvries-0.7.0/src/diepvries/role_playing_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-06-16 14:06:04.000000 diepvries-0.7.0/src/diepvries/satellite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-06-16 14:06:04.000000 diepvries-0.7.0/src/diepvries/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:31.869083 diepvries-0.7.0/src/diepvries/template_sql/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-16 14:06:04.000000 diepvries-0.7.0/src/diepvries/template_sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-06-16 14:06:04.000000 diepvries-0.7.0/src/diepvries/template_sql/effectivity_satellite_dml.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-16 14:06:04.000000 diepvries-0.7.0/src/diepvries/template_sql/hub_link_dml.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-06-16 14:06:04.000000 diepvries-0.7.0/src/diepvries/template_sql/satellite_dml.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-16 14:06:04.000000 diepvries-0.7.0/src/diepvries/template_sql/sql_formulas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-16 14:06:04.000000 diepvries-0.7.0/src/diepvries/template_sql/staging_table_ddl.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:31.865083 diepvries-0.7.0/src/diepvries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-16 14:06:31.000000 diepvries-0.7.0/src/diepvries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-16 14:06:31.000000 diepvries-0.7.0/src/diepvries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 14:06:31.000000 diepvries-0.7.0/src/diepvries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 14:06:31.000000 diepvries-0.7.0/src/diepvries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 14:06:31.000000 diepvries-0.7.0/src/diepvries.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:31.873083 diepvries-0.7.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-16 14:06:04.000000 diepvries-0.7.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24383 2023-06-16 14:06:04.000000 diepvries-0.7.0/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:31.873083 diepvries-0.7.0/test/deserializers/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-16 14:06:04.000000 diepvries-0.7.0/test/deserializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-06-16 14:06:04.000000 diepvries-0.7.0/test/deserializers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24045 2023-06-16 14:06:04.000000 diepvries-0.7.0/test/deserializers/model_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-06-16 14:06:04.000000 diepvries-0.7.0/test/deserializers/test_snowflake_deserializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:31.877083 diepvries-0.7.0/test/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)    24348 2023-06-16 14:06:04.000000 diepvries-0.7.0/test/sql/expected_result_data_vault_load.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-16 14:06:04.000000 diepvries-0.7.0/test/sql/expected_result_effectivity_satellite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-16 14:06:04.000000 diepvries-0.7.0/test/sql/expected_result_hashdiff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-16 14:06:04.000000 diepvries-0.7.0/test/sql/expected_result_hashkey.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-16 14:06:04.000000 diepvries-0.7.0/test/sql/expected_result_hub.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-16 14:06:04.000000 diepvries-0.7.0/test/sql/expected_result_link.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-16 14:06:04.000000 diepvries-0.7.0/test/sql/expected_result_role_playing_hub.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-06-16 14:06:04.000000 diepvries-0.7.0/test/sql/expected_result_satellite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-06-16 14:06:04.000000 diepvries-0.7.0/test/sql/expected_result_staging.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-16 14:06:04.000000 diepvries-0.7.0/test/test_data_vault_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-16 14:06:04.000000 diepvries-0.7.0/test/test_driving_key_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14880 2023-06-16 14:06:04.000000 diepvries-0.7.0/test/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-16 14:06:04.000000 diepvries-0.7.0/test/test_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-16 14:06:04.000000 diepvries-0.7.0/test/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-16 14:06:04.000000 diepvries-0.7.0/test/test_satellite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-06-16 14:06:04.000000 diepvries-0.7.0/tox.ini
```

### Comparing `diepvries-0.6.4/.github/workflows/pages-build-and-deploy.yml` & `diepvries-0.7.0/.github/workflows/pages-build-and-deploy.yml`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/.github/workflows/pypi-build-and-deploy.yml` & `diepvries-0.7.0/.github/workflows/pypi-build-and-deploy.yml`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/.github/workflows/run-test-suite.yml` & `diepvries-0.7.0/.github/workflows/run-test-suite.yml`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/CHANGELOG.md` & `diepvries-0.7.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.7.0] - 2023-05-26
+### Added
+- Add validation for driving keys (#41)
+
+### Changed
+- Exclude more recent records from satellites based on hashkey or driving key (#42)
+
 ## [0.6.4] - 2023-03-01
 ### Added
 - Add support for python 3.10 (#37)
 
 ### Changed
 - Update `snowflake-connector-python` to `~=3.0` (#37)
```

### Comparing `diepvries-0.6.4/CONTRIBUTING.md` & `diepvries-0.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/LICENSE` & `diepvries-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/PKG-INFO` & `diepvries-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diepvries
-Version: 0.6.4
+Version: 0.7.0
 Summary: diepvries - Picnic Data Vault framework
 Home-page: https://github.com/PicnicSupermarket/diepvries
 Author: Picnic Technologies
 License: MIT
 Project-URL: Documentation, https://diepvries.picnic.tech/
 Project-URL: Source Code, https://github.com/PicnicSupermarket/diepvries
 Project-URL: Issue Tracker, https://github.com/PicnicSupermarket/diepvries/issues
```

### Comparing `diepvries-0.6.4/README.md` & `diepvries-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/doc/advanced-topics.rst` & `diepvries-0.7.0/doc/advanced-topics.rst`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/doc/development.rst` & `diepvries-0.7.0/doc/development.rst`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/doc/glossary.rst` & `diepvries-0.7.0/doc/glossary.rst`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/doc/index.rst` & `diepvries-0.7.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/doc/installation.rst` & `diepvries-0.7.0/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/doc/naming-conventions.rst` & `diepvries-0.7.0/doc/naming-conventions.rst`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/doc/philosophy.rst` & `diepvries-0.7.0/doc/philosophy.rst`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/doc/security.rst` & `diepvries-0.7.0/doc/security.rst`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/doc/snippets/deserializer.py` & `diepvries-0.7.0/doc/snippets/deserializer.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/doc/snippets/dv_load.py` & `diepvries-0.7.0/doc/snippets/dv_load.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/doc/snippets/effsat.py` & `diepvries-0.7.0/doc/snippets/effsat.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/doc/snippets/effsat_deserializer.py` & `diepvries-0.7.0/doc/snippets/effsat_deserializer.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/doc/snippets/extract.sql` & `diepvries-0.7.0/doc/snippets/extract.sql`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/doc/snippets/h_customer.sql` & `diepvries-0.7.0/doc/snippets/h_customer.sql`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/doc/snippets/h_order.sql` & `diepvries-0.7.0/doc/snippets/h_order.sql`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/doc/snippets/l_order_customer.sql` & `diepvries-0.7.0/doc/snippets/l_order_customer.sql`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/doc/snippets/nodeserializer.py` & `diepvries-0.7.0/doc/snippets/nodeserializer.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/doc/snippets/rph.py` & `diepvries-0.7.0/doc/snippets/rph.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/doc/snippets/rph_deserializer.py` & `diepvries-0.7.0/doc/snippets/rph_deserializer.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/doc/static/diepvries-round.svg` & `diepvries-0.7.0/doc/static/diepvries-round.svg`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/doc/static/diepvries-square.svg` & `diepvries-0.7.0/doc/static/diepvries-square.svg`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/doc/static/diepvries.svg` & `diepvries-0.7.0/doc/static/diepvries.svg`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/doc/tutorial.rst` & `diepvries-0.7.0/doc/tutorial.rst`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/doc_templates/package.rst_t` & `diepvries-0.7.0/doc_templates/package.rst_t`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/setup.cfg` & `diepvries-0.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/src/diepvries/__init__.py` & `diepvries-0.7.0/src/diepvries/__init__.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/src/diepvries/data_vault_load.py` & `diepvries-0.7.0/src/diepvries/data_vault_load.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/src/diepvries/deserializers/snowflake_deserializer.py` & `diepvries-0.7.0/src/diepvries/deserializers/snowflake_deserializer.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/src/diepvries/effectivity_satellite.py` & `diepvries-0.7.0/src/diepvries/effectivity_satellite.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/src/diepvries/field.py` & `diepvries-0.7.0/src/diepvries/field.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/src/diepvries/hub.py` & `diepvries-0.7.0/src/diepvries/hub.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/src/diepvries/link.py` & `diepvries-0.7.0/src/diepvries/link.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/src/diepvries/role_playing_hub.py` & `diepvries-0.7.0/src/diepvries/role_playing_hub.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/src/diepvries/satellite.py` & `diepvries-0.7.0/src/diepvries/satellite.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/src/diepvries/table.py` & `diepvries-0.7.0/src/diepvries/table.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/src/diepvries/template_sql/effectivity_satellite_dml.sql` & `diepvries-0.7.0/src/diepvries/template_sql/effectivity_satellite_dml.sql`

 * *Files 6% similar despite different names*

```diff
@@ -1,82 +1,88 @@
 MERGE INTO {target_schema}.{target_table} AS satellite
   USING (
-    WITH
-      filtered_staging AS (
-        SELECT DISTINCT
-          {staging_driving_keys},
-          staging.{hashkey_field},
-          staging.{staging_hashdiff_field},
-          staging.{record_start_timestamp},
-          staging.{record_source}
-          {staging_descriptive_fields}
-        FROM {staging_schema}.{staging_table} AS staging
-          CROSS JOIN (
-                       SELECT
-                         MAX({record_start_timestamp}) AS max_r_timestamp
-                       FROM {target_schema}.{target_table}
-                     ) AS max_satellite_timestamp
-        WHERE staging.{record_start_timestamp} >= COALESCE(max_satellite_timestamp.max_r_timestamp, '1970-01-01 00:00:00')
-      ),
-      effectivity_satellite AS (
-        SELECT
-          {link_driving_keys},
-          satellite.*
-        FROM filtered_staging AS staging
-          INNER JOIN {target_schema}.{link_table} AS l
-                     ON ({link_driving_key_condition})
-          INNER JOIN {target_schema}.{target_table} AS satellite
-                     ON (l.{hashkey_field} = satellite.{hashkey_field}
+        WITH
+          effectivity_satellite AS (
+          SELECT
+            {link_driving_keys},
+            satellite.*
+          FROM {target_schema}.{link_table} AS l
+            INNER JOIN {target_schema}.{target_table} AS satellite
+                       ON (l.{hashkey_field} = satellite.{hashkey_field}
                          AND satellite.{record_end_timestamp_name} = {end_of_time})
-      ),
-      staging_satellite_affected_records AS (
-        /* Records that will be inserted (don't exist in target table or exist
-          in the target table but the hashdiff changed). As the r_timestamp is fetched
-          from the staging table, these records will always be included in the
-          WHEN NOT MATCHED condition of the MERGE command. */
-        SELECT
-          {staging_driving_keys},
-          staging.{hashkey_field},
-          staging.{staging_hashdiff_field},
-          staging.{record_start_timestamp},
-          staging.{record_source}
-          {staging_descriptive_fields}
-        FROM filtered_staging AS staging
-          LEFT JOIN effectivity_satellite AS satellite
-                    ON ({satellite_driving_key_condition})
-        WHERE satellite.{hashkey_field} IS NULL
-           OR satellite.{hashdiff_field} <> staging.{staging_hashdiff_field}
-        UNION ALL
-        /* Records from the target table that will have its r_timestamp_end updated
-          (hashkey already exists in target table, but hashdiff changed). As the
-          r_timestamp is fetched from the target table, these records will always be
-          included in the WHEN MATCHED condition of the MERGE command. */
+                                   ),
+          filtered_effectivity_satellite AS (
+          SELECT
+            satellite.*
+          FROM {staging_schema}.{staging_table} AS staging
+            INNER JOIN effectivity_satellite AS satellite
+                       ON ({satellite_driving_key_condition})
+                                            ),
+          filtered_staging AS (
+          SELECT DISTINCT
+            {staging_driving_keys},
+            staging.{hashkey_field},
+            staging.{staging_hashdiff_field},
+            staging.{record_start_timestamp},
+            staging.{record_source}
+            {staging_descriptive_fields}
+          FROM {staging_schema}.{staging_table} AS staging
+          WHERE NOT EXISTS (
+                           SELECT
+                             1
+                           FROM filtered_effectivity_satellite AS satellite
+                           WHERE {satellite_driving_key_condition}
+                            AND satellite.r_timestamp >= staging.r_timestamp
+                           )
+                              ),
+          --   Records that will be inserted (don't exist in target table or exist
+          --   in the target table but the hashdiff changed). As the r_timestamp is fetched
+          --   from the staging table, these records will always be included in the
+          --   WHEN NOT MATCHED condition of the MERGE command.
+          staging_satellite_affected_records AS (
+          SELECT
+            {staging_driving_keys},
+            staging.{hashkey_field},
+            staging.{staging_hashdiff_field},
+            staging.{record_start_timestamp},
+            staging.{record_source}
+            {staging_descriptive_fields}
+          FROM filtered_staging AS staging
+            LEFT JOIN filtered_effectivity_satellite AS satellite
+                      ON ({satellite_driving_key_condition})
+          WHERE satellite.{hashkey_field} IS NULL
+             OR satellite.{hashdiff_field} <> staging.{staging_hashdiff_field}
+          UNION ALL
+          --  Records from the target table that will have its r_timestamp_end updated
+          --  (hashkey already exists in target table, but hashdiff changed). As the
+          --  r_timestamp is fetched from the target table, these records will always be
+          --  included in the WHEN MATCHED condition of the MERGE command.
+          SELECT
+            {satellite_driving_keys},
+            satellite.{hashkey_field},
+            satellite.{hashdiff_field} AS {staging_hashdiff_field},
+            satellite.{record_start_timestamp},
+            satellite.{record_source}
+            {satellite_descriptive_fields}
+          FROM filtered_staging AS staging
+            INNER JOIN filtered_effectivity_satellite AS satellite
+                       ON ({satellite_driving_key_condition})
+          WHERE satellite.{hashdiff_field} <> staging.{staging_hashdiff_field}
+                                                )
         SELECT
-          {satellite_driving_keys},
-          satellite.{hashkey_field},
-          satellite.{hashdiff_field} AS {staging_hashdiff_field},
-          satellite.{record_start_timestamp},
-          satellite.{record_source}
-          {satellite_descriptive_fields}
-        FROM filtered_staging AS staging
-          INNER JOIN effectivity_satellite AS satellite
-                     ON ({satellite_driving_key_condition})
-        WHERE satellite.{hashdiff_field} <> staging.{staging_hashdiff_field}
-      )
-    SELECT
-      {hashkey_field},
-      {staging_hashdiff_field},
-      {record_start_timestamp} AS {record_start_timestamp},
-      {record_end_timestamp_expression},
-      {record_source}
-      {descriptive_fields}
-    FROM staging_satellite_affected_records
-  ) AS staging
+          {hashkey_field},
+          {staging_hashdiff_field},
+          {record_start_timestamp} AS {record_start_timestamp},
+          {record_end_timestamp_expression},
+          {record_source}
+          {descriptive_fields}
+        FROM staging_satellite_affected_records
+        ) AS staging
   ON (satellite.{hashkey_field} = staging.{hashkey_field}
-      AND satellite.{record_start_timestamp} = staging.{record_start_timestamp})
+    AND satellite.{record_start_timestamp} = staging.{record_start_timestamp})
   WHEN MATCHED THEN
     UPDATE SET satellite.{record_end_timestamp_name} = staging.{record_end_timestamp_name}
   WHEN NOT MATCHED
     THEN
     INSERT ({fields})
       VALUES (
                staging.{hashkey_field},
```

### Comparing `diepvries-0.6.4/src/diepvries/template_sql/hub_link_dml.sql` & `diepvries-0.7.0/src/diepvries/template_sql/hub_link_dml.sql`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/src/diepvries/template_sql/satellite_dml.sql` & `diepvries-0.7.0/src/diepvries/template_sql/satellite_dml.sql`

 * *Files 8% similar despite different names*

```diff
@@ -1,68 +1,69 @@
 MERGE INTO {target_schema}.{target_table} AS satellite
   USING (
-    WITH
-      filtered_staging AS (
-        SELECT DISTINCT
-          staging.{hashkey_field},
-          staging.{staging_hashdiff_field},
-          staging.{record_start_timestamp},
-          staging.{record_source}
-          {staging_descriptive_fields}
-        FROM {staging_schema}.{staging_table} AS staging
-          CROSS JOIN (
-                       SELECT
-                         MAX({record_start_timestamp}) AS max_r_timestamp
-                       FROM {target_schema}.{target_table}
-                     ) AS max_satellite_timestamp
-        WHERE staging.{record_start_timestamp} >= COALESCE(max_satellite_timestamp.max_r_timestamp, '1970-01-01 00:00:00')
-      ),
-      staging_satellite_affected_records AS (
-        /* Records that will be inserted (don't exist in target table or exist
-          in the target table but the hashdiff changed). As the r_timestamp is fetched
-          from the staging table, these records will always be included in the
-          WHEN NOT MATCHED condition of the MERGE command. */
-        SELECT
-          staging.{hashkey_field},
-          staging.{staging_hashdiff_field},
-          staging.{record_start_timestamp},
-          staging.{record_source}
-          {staging_descriptive_fields}
-        FROM filtered_staging AS staging
-          LEFT OUTER JOIN {target_schema}.{target_table} AS satellite
-                          ON (staging.{hashkey_field} = satellite.{hashkey_field}
+        WITH
+          filtered_staging AS (
+          SELECT DISTINCT
+            staging.{hashkey_field},
+            staging.{staging_hashdiff_field},
+            staging.{record_start_timestamp},
+            staging.{record_source}
+            {staging_descriptive_fields}
+          FROM {staging_schema}.{staging_table} AS staging
+          WHERE NOT EXISTS (
+                           SELECT
+                             1
+                           FROM {target_schema}.{target_table} AS satellite
+                           WHERE staging.{hashkey_field} = satellite.{hashkey_field}
+                             AND satellite.r_timestamp >= staging.r_timestamp
+                           )
+                              ),
+          --  Records that will be inserted (don't exist in target table or exist
+          --  in the target table but the hashdiff changed). As the r_timestamp is fetched
+          --  from the staging table, these records will always be included in the
+          --  WHEN NOT MATCHED condition of the MERGE command.
+          staging_satellite_affected_records AS (
+          SELECT
+            staging.{hashkey_field},
+            staging.{staging_hashdiff_field},
+            staging.{record_start_timestamp},
+            staging.{record_source}
+            {staging_descriptive_fields}
+          FROM filtered_staging AS staging
+            LEFT OUTER JOIN {target_schema}.{target_table} AS satellite
+                            ON (staging.{hashkey_field} = satellite.{hashkey_field}
                               AND satellite.{record_end_timestamp_name} = {end_of_time})
-        WHERE satellite.{hashkey_field} IS NULL
-           OR satellite.{hashdiff_field} <> staging.{staging_hashdiff_field}
-        UNION ALL
-        /* Records from the target table that will have its r_timestamp_end updated
-          (hashkey already exists in target table, but hashdiff changed). As the
-          r_timestamp is fetched from the target table, these records will always be
-          included in the WHEN MATCHED condition of the MERGE command. */
+          WHERE satellite.{hashkey_field} IS NULL
+             OR satellite.{hashdiff_field} <> staging.{staging_hashdiff_field}
+          UNION ALL
+          -- Records from the target table that will have its r_timestamp_end updated
+          -- (hashkey already exists in target table, but hashdiff changed). As the
+          -- r_timestamp is fetched from the target table, these records will always be
+          -- included in the WHEN MATCHED condition of the MERGE command.
+          SELECT
+            satellite.{hashkey_field},
+            satellite.{hashdiff_field},
+            satellite.{record_start_timestamp},
+            satellite.{record_source}
+            {satellite_descriptive_fields}
+          FROM {target_schema}.{target_table} AS satellite
+            INNER JOIN filtered_staging AS staging
+                       ON (staging.{hashkey_field} = satellite.{hashkey_field}
+                         AND satellite.{record_end_timestamp_name} = {end_of_time})
+          WHERE staging.{staging_hashdiff_field} <> satellite.{hashdiff_field}
+                                                )
         SELECT
-          satellite.{hashkey_field},
-          satellite.{hashdiff_field},
-          satellite.{record_start_timestamp},
-          satellite.{record_source}
-          {satellite_descriptive_fields}
-        FROM {target_schema}.{target_table} AS satellite
-          INNER JOIN filtered_staging AS staging
-                     ON (staging.{hashkey_field} = satellite.{hashkey_field}
-                      AND satellite.{record_end_timestamp_name} = {end_of_time})
-        WHERE staging.{staging_hashdiff_field} <> satellite.{hashdiff_field}
-      )
-    SELECT
-      {hashkey_field},
-      {staging_hashdiff_field},
-      {record_start_timestamp} AS {record_start_timestamp},
-      {record_end_timestamp_expression},
-      {record_source}
-      {descriptive_fields}
-    FROM staging_satellite_affected_records
-  ) AS staging
+          {hashkey_field},
+          {staging_hashdiff_field},
+          {record_start_timestamp} AS {record_start_timestamp},
+          {record_end_timestamp_expression},
+          {record_source}
+          {descriptive_fields}
+        FROM staging_satellite_affected_records
+        ) AS staging
   ON (satellite.{hashkey_field} = staging.{hashkey_field}
     AND satellite.{record_start_timestamp} = staging.{record_start_timestamp})
   WHEN MATCHED THEN
     UPDATE SET satellite.{record_end_timestamp_name} = staging.{record_end_timestamp_name}
   WHEN NOT MATCHED
     THEN
     INSERT ({fields})
```

### Comparing `diepvries-0.6.4/src/diepvries/template_sql/sql_formulas.py` & `diepvries-0.7.0/src/diepvries/template_sql/sql_formulas.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/src/diepvries.egg-info/PKG-INFO` & `diepvries-0.7.0/src/diepvries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diepvries
-Version: 0.6.4
+Version: 0.7.0
 Summary: diepvries - Picnic Data Vault framework
 Home-page: https://github.com/PicnicSupermarket/diepvries
 Author: Picnic Technologies
 License: MIT
 Project-URL: Documentation, https://diepvries.picnic.tech/
 Project-URL: Source Code, https://github.com/PicnicSupermarket/diepvries
 Project-URL: Issue Tracker, https://github.com/PicnicSupermarket/diepvries/issues
```

### Comparing `diepvries-0.6.4/src/diepvries.egg-info/SOURCES.txt` & `diepvries-0.7.0/src/diepvries.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 src/diepvries/template_sql/hub_link_dml.sql
 src/diepvries/template_sql/satellite_dml.sql
 src/diepvries/template_sql/sql_formulas.py
 src/diepvries/template_sql/staging_table_ddl.sql
 test/__init__.py
 test/conftest.py
 test/test_data_vault_load.py
+test/test_driving_key_field.py
 test/test_field.py
 test/test_hub.py
 test/test_link.py
 test/test_satellite.py
 test/deserializers/__init__.py
 test/deserializers/conftest.py
 test/deserializers/model_metadata.json
```

### Comparing `diepvries-0.6.4/test/conftest.py` & `diepvries-0.7.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/test/deserializers/conftest.py` & `diepvries-0.7.0/test/deserializers/conftest.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/test/deserializers/model_metadata.json` & `diepvries-0.7.0/test/deserializers/model_metadata.json`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/test/deserializers/test_snowflake_deserializer.py` & `diepvries-0.7.0/test/deserializers/test_snowflake_deserializer.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/test/sql/expected_result_data_vault_load.sql` & `diepvries-0.7.0/test/sql/expected_result_data_vault_load.sql`

 * *Files 4% similar despite different names*

```diff
@@ -76,73 +76,74 @@
         FROM dv_stg.orders_20190806_000000
         ) AS staging ON (target.l_order_customer_role_playing_hashkey = staging.l_order_customer_role_playing_hashkey)
   WHEN NOT MATCHED THEN INSERT (l_order_customer_role_playing_hashkey, h_order_hashkey, h_customer_role_playing_hashkey, order_id, customer_role_playing_id, ck_test_string, ck_test_timestamp, r_timestamp, r_source)
     VALUES (staging.l_order_customer_role_playing_hashkey, staging.h_order_hashkey, staging.h_customer_role_playing_hashkey, staging.order_id, staging.customer_role_playing_id, staging.ck_test_string, staging.ck_test_timestamp, staging.r_timestamp, staging.r_source);
 
 MERGE INTO dv.hs_customer AS satellite
   USING (
-    WITH
-      filtered_staging AS (
-        SELECT DISTINCT
-          staging.h_customer_hashkey,
-          staging.hs_customer_hashdiff,
-          staging.r_timestamp,
-          staging.r_source
-          , staging.test_string, staging.test_date, staging.test_timestamp_ntz, staging.test_integer, staging.test_decimal, staging.x_customer_id, staging.grouping_key, staging.test_geography, staging.test_array, staging.test_object, staging.test_variant, staging.test_timestamp_tz, staging.test_timestamp_ltz, staging.test_time, staging.test_boolean, staging.test_real
-        FROM dv_stg.orders_20190806_000000 AS staging
-          CROSS JOIN (
-                       SELECT
-                         MAX(r_timestamp) AS max_r_timestamp
-                       FROM dv.hs_customer
-                     ) AS max_satellite_timestamp
-        WHERE staging.r_timestamp >= COALESCE(max_satellite_timestamp.max_r_timestamp, '1970-01-01 00:00:00')
-      ),
-      staging_satellite_affected_records AS (
-        /* Records that will be inserted (don't exist in target table or exist
-          in the target table but the hashdiff changed). As the r_timestamp is fetched
-          from the staging table, these records will always be included in the
-          WHEN NOT MATCHED condition of the MERGE command. */
-        SELECT
-          staging.h_customer_hashkey,
-          staging.hs_customer_hashdiff,
-          staging.r_timestamp,
-          staging.r_source
-          , staging.test_string, staging.test_date, staging.test_timestamp_ntz, staging.test_integer, staging.test_decimal, staging.x_customer_id, staging.grouping_key, staging.test_geography, staging.test_array, staging.test_object, staging.test_variant, staging.test_timestamp_tz, staging.test_timestamp_ltz, staging.test_time, staging.test_boolean, staging.test_real
-        FROM filtered_staging AS staging
-          LEFT OUTER JOIN dv.hs_customer AS satellite
-                          ON (staging.h_customer_hashkey = satellite.h_customer_hashkey
+        WITH
+          filtered_staging AS (
+          SELECT DISTINCT
+            staging.h_customer_hashkey,
+            staging.hs_customer_hashdiff,
+            staging.r_timestamp,
+            staging.r_source
+            , staging.test_string, staging.test_date, staging.test_timestamp_ntz, staging.test_integer, staging.test_decimal, staging.x_customer_id, staging.grouping_key, staging.test_geography, staging.test_array, staging.test_object, staging.test_variant, staging.test_timestamp_tz, staging.test_timestamp_ltz, staging.test_time, staging.test_boolean, staging.test_real
+          FROM dv_stg.orders_20190806_000000 AS staging
+          WHERE NOT EXISTS (
+                           SELECT
+                             1
+                           FROM dv.hs_customer AS satellite
+                           WHERE staging.h_customer_hashkey = satellite.h_customer_hashkey
+                             AND satellite.r_timestamp >= staging.r_timestamp
+                           )
+                              ),
+          --  Records that will be inserted (don't exist in target table or exist
+          --  in the target table but the hashdiff changed). As the r_timestamp is fetched
+          --  from the staging table, these records will always be included in the
+          --  WHEN NOT MATCHED condition of the MERGE command.
+          staging_satellite_affected_records AS (
+          SELECT
+            staging.h_customer_hashkey,
+            staging.hs_customer_hashdiff,
+            staging.r_timestamp,
+            staging.r_source
+            , staging.test_string, staging.test_date, staging.test_timestamp_ntz, staging.test_integer, staging.test_decimal, staging.x_customer_id, staging.grouping_key, staging.test_geography, staging.test_array, staging.test_object, staging.test_variant, staging.test_timestamp_tz, staging.test_timestamp_ltz, staging.test_time, staging.test_boolean, staging.test_real
+          FROM filtered_staging AS staging
+            LEFT OUTER JOIN dv.hs_customer AS satellite
+                            ON (staging.h_customer_hashkey = satellite.h_customer_hashkey
                               AND satellite.r_timestamp_end = CAST('9999-12-31T00:00:00.000000Z' AS TIMESTAMP))
-        WHERE satellite.h_customer_hashkey IS NULL
-           OR satellite.s_hashdiff <> staging.hs_customer_hashdiff
-        UNION ALL
-        /* Records from the target table that will have its r_timestamp_end updated
-          (hashkey already exists in target table, but hashdiff changed). As the
-          r_timestamp is fetched from the target table, these records will always be
-          included in the WHEN MATCHED condition of the MERGE command. */
+          WHERE satellite.h_customer_hashkey IS NULL
+             OR satellite.s_hashdiff <> staging.hs_customer_hashdiff
+          UNION ALL
+          -- Records from the target table that will have its r_timestamp_end updated
+          -- (hashkey already exists in target table, but hashdiff changed). As the
+          -- r_timestamp is fetched from the target table, these records will always be
+          -- included in the WHEN MATCHED condition of the MERGE command.
+          SELECT
+            satellite.h_customer_hashkey,
+            satellite.s_hashdiff,
+            satellite.r_timestamp,
+            satellite.r_source
+            , satellite.test_string, satellite.test_date, satellite.test_timestamp_ntz, satellite.test_integer, satellite.test_decimal, satellite.x_customer_id, satellite.grouping_key, satellite.test_geography, satellite.test_array, satellite.test_object, satellite.test_variant, satellite.test_timestamp_tz, satellite.test_timestamp_ltz, satellite.test_time, satellite.test_boolean, satellite.test_real
+          FROM dv.hs_customer AS satellite
+            INNER JOIN filtered_staging AS staging
+                       ON (staging.h_customer_hashkey = satellite.h_customer_hashkey
+                         AND satellite.r_timestamp_end = CAST('9999-12-31T00:00:00.000000Z' AS TIMESTAMP))
+          WHERE staging.hs_customer_hashdiff <> satellite.s_hashdiff
+                                                )
         SELECT
-          satellite.h_customer_hashkey,
-          satellite.s_hashdiff,
-          satellite.r_timestamp,
-          satellite.r_source
-          , satellite.test_string, satellite.test_date, satellite.test_timestamp_ntz, satellite.test_integer, satellite.test_decimal, satellite.x_customer_id, satellite.grouping_key, satellite.test_geography, satellite.test_array, satellite.test_object, satellite.test_variant, satellite.test_timestamp_tz, satellite.test_timestamp_ltz, satellite.test_time, satellite.test_boolean, satellite.test_real
-        FROM dv.hs_customer AS satellite
-          INNER JOIN filtered_staging AS staging
-                     ON (staging.h_customer_hashkey = satellite.h_customer_hashkey
-                      AND satellite.r_timestamp_end = CAST('9999-12-31T00:00:00.000000Z' AS TIMESTAMP))
-        WHERE staging.hs_customer_hashdiff <> satellite.s_hashdiff
-      )
-    SELECT
-      h_customer_hashkey,
-      hs_customer_hashdiff,
-      r_timestamp AS r_timestamp,
-      LEAD(DATEADD(milliseconds, - 1, r_timestamp), 1, CAST('9999-12-31T00:00:00.000000Z' AS TIMESTAMP)) OVER (PARTITION BY h_customer_hashkey ORDER BY r_timestamp) AS r_timestamp_end,
-      r_source
-      , test_string, test_date, test_timestamp_ntz, test_integer, test_decimal, x_customer_id, grouping_key, test_geography, test_array, test_object, test_variant, test_timestamp_tz, test_timestamp_ltz, test_time, test_boolean, test_real
-    FROM staging_satellite_affected_records
-  ) AS staging
+          h_customer_hashkey,
+          hs_customer_hashdiff,
+          r_timestamp AS r_timestamp,
+          LEAD(DATEADD(milliseconds, - 1, r_timestamp), 1, CAST('9999-12-31T00:00:00.000000Z' AS TIMESTAMP)) OVER (PARTITION BY h_customer_hashkey ORDER BY r_timestamp) AS r_timestamp_end,
+          r_source
+          , test_string, test_date, test_timestamp_ntz, test_integer, test_decimal, x_customer_id, grouping_key, test_geography, test_array, test_object, test_variant, test_timestamp_tz, test_timestamp_ltz, test_time, test_boolean, test_real
+        FROM staging_satellite_affected_records
+        ) AS staging
   ON (satellite.h_customer_hashkey = staging.h_customer_hashkey
     AND satellite.r_timestamp = staging.r_timestamp)
   WHEN MATCHED THEN
     UPDATE SET satellite.r_timestamp_end = staging.r_timestamp_end
   WHEN NOT MATCHED
     THEN
     INSERT (h_customer_hashkey, s_hashdiff, r_timestamp, r_timestamp_end, r_source, test_string, test_date, test_timestamp_ntz, test_integer, test_decimal, x_customer_id, grouping_key, test_geography, test_array, test_object, test_variant, test_timestamp_tz, test_timestamp_ltz, test_time, test_boolean, test_real)
@@ -152,87 +153,93 @@
                staging.r_timestamp,
                staging.r_timestamp_end,
                staging.r_source
                , staging.test_string, staging.test_date, staging.test_timestamp_ntz, staging.test_integer, staging.test_decimal, staging.x_customer_id, staging.grouping_key, staging.test_geography, staging.test_array, staging.test_object, staging.test_variant, staging.test_timestamp_tz, staging.test_timestamp_ltz, staging.test_time, staging.test_boolean, staging.test_real);
 
 MERGE INTO dv.ls_order_customer_eff AS satellite
   USING (
-    WITH
-      filtered_staging AS (
-        SELECT DISTINCT
-          staging.h_customer_hashkey,
-          staging.l_order_customer_hashkey,
-          staging.ls_order_customer_eff_hashdiff,
-          staging.r_timestamp,
-          staging.r_source
-          , staging.dummy_descriptive_field
-        FROM dv_stg.orders_20190806_000000 AS staging
-          CROSS JOIN (
-                       SELECT
-                         MAX(r_timestamp) AS max_r_timestamp
-                       FROM dv.ls_order_customer_eff
-                     ) AS max_satellite_timestamp
-        WHERE staging.r_timestamp >= COALESCE(max_satellite_timestamp.max_r_timestamp, '1970-01-01 00:00:00')
-      ),
-      effectivity_satellite AS (
-        SELECT
-          l.h_customer_hashkey,
-          satellite.*
-        FROM filtered_staging AS staging
-          INNER JOIN dv.l_order_customer AS l
-                     ON (l.h_customer_hashkey = staging.h_customer_hashkey)
-          INNER JOIN dv.ls_order_customer_eff AS satellite
-                     ON (l.l_order_customer_hashkey = satellite.l_order_customer_hashkey
+        WITH
+          effectivity_satellite AS (
+          SELECT
+            l.h_customer_hashkey,
+            satellite.*
+          FROM dv.l_order_customer AS l
+            INNER JOIN dv.ls_order_customer_eff AS satellite
+                       ON (l.l_order_customer_hashkey = satellite.l_order_customer_hashkey
                          AND satellite.r_timestamp_end = CAST('9999-12-31T00:00:00.000000Z' AS TIMESTAMP))
-      ),
-      staging_satellite_affected_records AS (
-        /* Records that will be inserted (don't exist in target table or exist
-          in the target table but the hashdiff changed). As the r_timestamp is fetched
-          from the staging table, these records will always be included in the
-          WHEN NOT MATCHED condition of the MERGE command. */
-        SELECT
-          staging.h_customer_hashkey,
-          staging.l_order_customer_hashkey,
-          staging.ls_order_customer_eff_hashdiff,
-          staging.r_timestamp,
-          staging.r_source
-          , staging.dummy_descriptive_field
-        FROM filtered_staging AS staging
-          LEFT JOIN effectivity_satellite AS satellite
-                    ON (satellite.h_customer_hashkey = staging.h_customer_hashkey)
-        WHERE satellite.l_order_customer_hashkey IS NULL
-           OR satellite.s_hashdiff <> staging.ls_order_customer_eff_hashdiff
-        UNION ALL
-        /* Records from the target table that will have its r_timestamp_end updated
-          (hashkey already exists in target table, but hashdiff changed). As the
-          r_timestamp is fetched from the target table, these records will always be
-          included in the WHEN MATCHED condition of the MERGE command. */
+                                   ),
+          filtered_effectivity_satellite AS (
+          SELECT
+            satellite.*
+          FROM dv_stg.orders_20190806_000000 AS staging
+            INNER JOIN effectivity_satellite AS satellite
+                       ON (satellite.h_customer_hashkey = staging.h_customer_hashkey)
+                                            ),
+          filtered_staging AS (
+          SELECT DISTINCT
+            staging.h_customer_hashkey,
+            staging.l_order_customer_hashkey,
+            staging.ls_order_customer_eff_hashdiff,
+            staging.r_timestamp,
+            staging.r_source
+            , staging.dummy_descriptive_field
+          FROM dv_stg.orders_20190806_000000 AS staging
+          WHERE NOT EXISTS (
+                           SELECT
+                             1
+                           FROM filtered_effectivity_satellite AS satellite
+                           WHERE satellite.h_customer_hashkey = staging.h_customer_hashkey
+                            AND satellite.r_timestamp >= staging.r_timestamp
+                           )
+                              ),
+          --   Records that will be inserted (don't exist in target table or exist
+          --   in the target table but the hashdiff changed). As the r_timestamp is fetched
+          --   from the staging table, these records will always be included in the
+          --   WHEN NOT MATCHED condition of the MERGE command.
+          staging_satellite_affected_records AS (
+          SELECT
+            staging.h_customer_hashkey,
+            staging.l_order_customer_hashkey,
+            staging.ls_order_customer_eff_hashdiff,
+            staging.r_timestamp,
+            staging.r_source
+            , staging.dummy_descriptive_field
+          FROM filtered_staging AS staging
+            LEFT JOIN filtered_effectivity_satellite AS satellite
+                      ON (satellite.h_customer_hashkey = staging.h_customer_hashkey)
+          WHERE satellite.l_order_customer_hashkey IS NULL
+             OR satellite.s_hashdiff <> staging.ls_order_customer_eff_hashdiff
+          UNION ALL
+          --  Records from the target table that will have its r_timestamp_end updated
+          --  (hashkey already exists in target table, but hashdiff changed). As the
+          --  r_timestamp is fetched from the target table, these records will always be
+          --  included in the WHEN MATCHED condition of the MERGE command.
+          SELECT
+            satellite.h_customer_hashkey,
+            satellite.l_order_customer_hashkey,
+            satellite.s_hashdiff AS ls_order_customer_eff_hashdiff,
+            satellite.r_timestamp,
+            satellite.r_source
+            , satellite.dummy_descriptive_field
+          FROM filtered_staging AS staging
+            INNER JOIN filtered_effectivity_satellite AS satellite
+                       ON (satellite.h_customer_hashkey = staging.h_customer_hashkey)
+          WHERE satellite.s_hashdiff <> staging.ls_order_customer_eff_hashdiff
+                                                )
         SELECT
-          satellite.h_customer_hashkey,
-          satellite.l_order_customer_hashkey,
-          satellite.s_hashdiff AS ls_order_customer_eff_hashdiff,
-          satellite.r_timestamp,
-          satellite.r_source
-          , satellite.dummy_descriptive_field
-        FROM filtered_staging AS staging
-          INNER JOIN effectivity_satellite AS satellite
-                     ON (satellite.h_customer_hashkey = staging.h_customer_hashkey)
-        WHERE satellite.s_hashdiff <> staging.ls_order_customer_eff_hashdiff
-      )
-    SELECT
-      l_order_customer_hashkey,
-      ls_order_customer_eff_hashdiff,
-      r_timestamp AS r_timestamp,
-      LEAD(DATEADD(milliseconds, - 1, r_timestamp), 1, CAST('9999-12-31T00:00:00.000000Z' AS TIMESTAMP)) OVER (PARTITION BY h_customer_hashkey ORDER BY r_timestamp) AS r_timestamp_end,
-      r_source
-      , dummy_descriptive_field
-    FROM staging_satellite_affected_records
-  ) AS staging
+          l_order_customer_hashkey,
+          ls_order_customer_eff_hashdiff,
+          r_timestamp AS r_timestamp,
+          LEAD(DATEADD(milliseconds, - 1, r_timestamp), 1, CAST('9999-12-31T00:00:00.000000Z' AS TIMESTAMP)) OVER (PARTITION BY h_customer_hashkey ORDER BY r_timestamp) AS r_timestamp_end,
+          r_source
+          , dummy_descriptive_field
+        FROM staging_satellite_affected_records
+        ) AS staging
   ON (satellite.l_order_customer_hashkey = staging.l_order_customer_hashkey
-      AND satellite.r_timestamp = staging.r_timestamp)
+    AND satellite.r_timestamp = staging.r_timestamp)
   WHEN MATCHED THEN
     UPDATE SET satellite.r_timestamp_end = staging.r_timestamp_end
   WHEN NOT MATCHED
     THEN
     INSERT (l_order_customer_hashkey, s_hashdiff, r_timestamp, r_timestamp_end, r_source, dummy_descriptive_field)
       VALUES (
                staging.l_order_customer_hashkey,
@@ -240,87 +247,93 @@
                staging.r_timestamp,
                staging.r_timestamp_end,
                staging.r_source
                , staging.dummy_descriptive_field);
 
 MERGE INTO dv.ls_order_customer_role_playing_eff AS satellite
   USING (
-    WITH
-      filtered_staging AS (
-        SELECT DISTINCT
-          staging.h_customer_role_playing_hashkey,
-          staging.l_order_customer_role_playing_hashkey,
-          staging.ls_order_customer_role_playing_eff_hashdiff,
-          staging.r_timestamp,
-          staging.r_source
-          , staging.dummy_descriptive_field
-        FROM dv_stg.orders_20190806_000000 AS staging
-          CROSS JOIN (
-                       SELECT
-                         MAX(r_timestamp) AS max_r_timestamp
-                       FROM dv.ls_order_customer_role_playing_eff
-                     ) AS max_satellite_timestamp
-        WHERE staging.r_timestamp >= COALESCE(max_satellite_timestamp.max_r_timestamp, '1970-01-01 00:00:00')
-      ),
-      effectivity_satellite AS (
-        SELECT
-          l.h_customer_role_playing_hashkey,
-          satellite.*
-        FROM filtered_staging AS staging
-          INNER JOIN dv.l_order_customer_role_playing AS l
-                     ON (l.h_customer_role_playing_hashkey = staging.h_customer_role_playing_hashkey)
-          INNER JOIN dv.ls_order_customer_role_playing_eff AS satellite
-                     ON (l.l_order_customer_role_playing_hashkey = satellite.l_order_customer_role_playing_hashkey
+        WITH
+          effectivity_satellite AS (
+          SELECT
+            l.h_customer_role_playing_hashkey,
+            satellite.*
+          FROM dv.l_order_customer_role_playing AS l
+            INNER JOIN dv.ls_order_customer_role_playing_eff AS satellite
+                       ON (l.l_order_customer_role_playing_hashkey = satellite.l_order_customer_role_playing_hashkey
                          AND satellite.r_timestamp_end = CAST('9999-12-31T00:00:00.000000Z' AS TIMESTAMP))
-      ),
-      staging_satellite_affected_records AS (
-        /* Records that will be inserted (don't exist in target table or exist
-          in the target table but the hashdiff changed). As the r_timestamp is fetched
-          from the staging table, these records will always be included in the
-          WHEN NOT MATCHED condition of the MERGE command. */
+                                   ),
+          filtered_effectivity_satellite AS (
+          SELECT
+            satellite.*
+          FROM dv_stg.orders_20190806_000000 AS staging
+            INNER JOIN effectivity_satellite AS satellite
+                       ON (satellite.h_customer_role_playing_hashkey = staging.h_customer_role_playing_hashkey)
+                                            ),
+          filtered_staging AS (
+          SELECT DISTINCT
+            staging.h_customer_role_playing_hashkey,
+            staging.l_order_customer_role_playing_hashkey,
+            staging.ls_order_customer_role_playing_eff_hashdiff,
+            staging.r_timestamp,
+            staging.r_source
+            , staging.dummy_descriptive_field
+          FROM dv_stg.orders_20190806_000000 AS staging
+          WHERE NOT EXISTS (
+                           SELECT
+                             1
+                           FROM filtered_effectivity_satellite AS satellite
+                           WHERE satellite.h_customer_role_playing_hashkey = staging.h_customer_role_playing_hashkey
+                            AND satellite.r_timestamp >= staging.r_timestamp
+                           )
+                              ),
+          --   Records that will be inserted (don't exist in target table or exist
+          --   in the target table but the hashdiff changed). As the r_timestamp is fetched
+          --   from the staging table, these records will always be included in the
+          --   WHEN NOT MATCHED condition of the MERGE command.
+          staging_satellite_affected_records AS (
+          SELECT
+            staging.h_customer_role_playing_hashkey,
+            staging.l_order_customer_role_playing_hashkey,
+            staging.ls_order_customer_role_playing_eff_hashdiff,
+            staging.r_timestamp,
+            staging.r_source
+            , staging.dummy_descriptive_field
+          FROM filtered_staging AS staging
+            LEFT JOIN filtered_effectivity_satellite AS satellite
+                      ON (satellite.h_customer_role_playing_hashkey = staging.h_customer_role_playing_hashkey)
+          WHERE satellite.l_order_customer_role_playing_hashkey IS NULL
+             OR satellite.s_hashdiff <> staging.ls_order_customer_role_playing_eff_hashdiff
+          UNION ALL
+          --  Records from the target table that will have its r_timestamp_end updated
+          --  (hashkey already exists in target table, but hashdiff changed). As the
+          --  r_timestamp is fetched from the target table, these records will always be
+          --  included in the WHEN MATCHED condition of the MERGE command.
+          SELECT
+            satellite.h_customer_role_playing_hashkey,
+            satellite.l_order_customer_role_playing_hashkey,
+            satellite.s_hashdiff AS ls_order_customer_role_playing_eff_hashdiff,
+            satellite.r_timestamp,
+            satellite.r_source
+            , satellite.dummy_descriptive_field
+          FROM filtered_staging AS staging
+            INNER JOIN filtered_effectivity_satellite AS satellite
+                       ON (satellite.h_customer_role_playing_hashkey = staging.h_customer_role_playing_hashkey)
+          WHERE satellite.s_hashdiff <> staging.ls_order_customer_role_playing_eff_hashdiff
+                                                )
         SELECT
-          staging.h_customer_role_playing_hashkey,
-          staging.l_order_customer_role_playing_hashkey,
-          staging.ls_order_customer_role_playing_eff_hashdiff,
-          staging.r_timestamp,
-          staging.r_source
-          , staging.dummy_descriptive_field
-        FROM filtered_staging AS staging
-          LEFT JOIN effectivity_satellite AS satellite
-                    ON (satellite.h_customer_role_playing_hashkey = staging.h_customer_role_playing_hashkey)
-        WHERE satellite.l_order_customer_role_playing_hashkey IS NULL
-           OR satellite.s_hashdiff <> staging.ls_order_customer_role_playing_eff_hashdiff
-        UNION ALL
-        /* Records from the target table that will have its r_timestamp_end updated
-          (hashkey already exists in target table, but hashdiff changed). As the
-          r_timestamp is fetched from the target table, these records will always be
-          included in the WHEN MATCHED condition of the MERGE command. */
-        SELECT
-          satellite.h_customer_role_playing_hashkey,
-          satellite.l_order_customer_role_playing_hashkey,
-          satellite.s_hashdiff AS ls_order_customer_role_playing_eff_hashdiff,
-          satellite.r_timestamp,
-          satellite.r_source
-          , satellite.dummy_descriptive_field
-        FROM filtered_staging AS staging
-          INNER JOIN effectivity_satellite AS satellite
-                     ON (satellite.h_customer_role_playing_hashkey = staging.h_customer_role_playing_hashkey)
-        WHERE satellite.s_hashdiff <> staging.ls_order_customer_role_playing_eff_hashdiff
-      )
-    SELECT
-      l_order_customer_role_playing_hashkey,
-      ls_order_customer_role_playing_eff_hashdiff,
-      r_timestamp AS r_timestamp,
-      LEAD(DATEADD(milliseconds, - 1, r_timestamp), 1, CAST('9999-12-31T00:00:00.000000Z' AS TIMESTAMP)) OVER (PARTITION BY h_customer_role_playing_hashkey ORDER BY r_timestamp) AS r_timestamp_end,
-      r_source
-      , dummy_descriptive_field
-    FROM staging_satellite_affected_records
-  ) AS staging
+          l_order_customer_role_playing_hashkey,
+          ls_order_customer_role_playing_eff_hashdiff,
+          r_timestamp AS r_timestamp,
+          LEAD(DATEADD(milliseconds, - 1, r_timestamp), 1, CAST('9999-12-31T00:00:00.000000Z' AS TIMESTAMP)) OVER (PARTITION BY h_customer_role_playing_hashkey ORDER BY r_timestamp) AS r_timestamp_end,
+          r_source
+          , dummy_descriptive_field
+        FROM staging_satellite_affected_records
+        ) AS staging
   ON (satellite.l_order_customer_role_playing_hashkey = staging.l_order_customer_role_playing_hashkey
-      AND satellite.r_timestamp = staging.r_timestamp)
+    AND satellite.r_timestamp = staging.r_timestamp)
   WHEN MATCHED THEN
     UPDATE SET satellite.r_timestamp_end = staging.r_timestamp_end
   WHEN NOT MATCHED
     THEN
     INSERT (l_order_customer_role_playing_hashkey, s_hashdiff, r_timestamp, r_timestamp_end, r_source, dummy_descriptive_field)
       VALUES (
                staging.l_order_customer_role_playing_hashkey,
```

### Comparing `diepvries-0.6.4/test/sql/expected_result_effectivity_satellite.sql` & `diepvries-0.7.0/test/sql/expected_result_effectivity_satellite.sql`

 * *Files 11% similar despite different names*

```diff
@@ -1,82 +1,88 @@
 MERGE INTO dv.ls_order_customer_eff AS satellite
   USING (
-    WITH
-      filtered_staging AS (
-        SELECT DISTINCT
-          staging.h_customer_hashkey,
-          staging.l_order_customer_hashkey,
-          staging.ls_order_customer_eff_hashdiff,
-          staging.r_timestamp,
-          staging.r_source
-          , staging.dummy_descriptive_field
-        FROM dv_stg.orders_20190806_000000 AS staging
-          CROSS JOIN (
-                       SELECT
-                         MAX(r_timestamp) AS max_r_timestamp
-                       FROM dv.ls_order_customer_eff
-                     ) AS max_satellite_timestamp
-        WHERE staging.r_timestamp >= COALESCE(max_satellite_timestamp.max_r_timestamp, '1970-01-01 00:00:00')
-      ),
-      effectivity_satellite AS (
-        SELECT
-          l.h_customer_hashkey,
-          satellite.*
-        FROM filtered_staging AS staging
-          INNER JOIN dv.l_order_customer AS l
-                     ON (l.h_customer_hashkey = staging.h_customer_hashkey)
-          INNER JOIN dv.ls_order_customer_eff AS satellite
-                     ON (l.l_order_customer_hashkey = satellite.l_order_customer_hashkey
+        WITH
+          effectivity_satellite AS (
+          SELECT
+            l.h_customer_hashkey,
+            satellite.*
+          FROM dv.l_order_customer AS l
+            INNER JOIN dv.ls_order_customer_eff AS satellite
+                       ON (l.l_order_customer_hashkey = satellite.l_order_customer_hashkey
                          AND satellite.r_timestamp_end = CAST('9999-12-31T00:00:00.000000Z' AS TIMESTAMP))
-      ),
-      staging_satellite_affected_records AS (
-        /* Records that will be inserted (don't exist in target table or exist
-          in the target table but the hashdiff changed). As the r_timestamp is fetched
-          from the staging table, these records will always be included in the
-          WHEN NOT MATCHED condition of the MERGE command. */
-        SELECT
-          staging.h_customer_hashkey,
-          staging.l_order_customer_hashkey,
-          staging.ls_order_customer_eff_hashdiff,
-          staging.r_timestamp,
-          staging.r_source
-          , staging.dummy_descriptive_field
-        FROM filtered_staging AS staging
-          LEFT JOIN effectivity_satellite AS satellite
-                    ON (satellite.h_customer_hashkey = staging.h_customer_hashkey)
-        WHERE satellite.l_order_customer_hashkey IS NULL
-           OR satellite.s_hashdiff <> staging.ls_order_customer_eff_hashdiff
-        UNION ALL
-        /* Records from the target table that will have its r_timestamp_end updated
-          (hashkey already exists in target table, but hashdiff changed). As the
-          r_timestamp is fetched from the target table, these records will always be
-          included in the WHEN MATCHED condition of the MERGE command. */
+                                   ),
+          filtered_effectivity_satellite AS (
+          SELECT
+            satellite.*
+          FROM dv_stg.orders_20190806_000000 AS staging
+            INNER JOIN effectivity_satellite AS satellite
+                       ON (satellite.h_customer_hashkey = staging.h_customer_hashkey)
+                                            ),
+          filtered_staging AS (
+          SELECT DISTINCT
+            staging.h_customer_hashkey,
+            staging.l_order_customer_hashkey,
+            staging.ls_order_customer_eff_hashdiff,
+            staging.r_timestamp,
+            staging.r_source
+            , staging.dummy_descriptive_field
+          FROM dv_stg.orders_20190806_000000 AS staging
+          WHERE NOT EXISTS (
+                           SELECT
+                             1
+                           FROM filtered_effectivity_satellite AS satellite
+                           WHERE satellite.h_customer_hashkey = staging.h_customer_hashkey
+                            AND satellite.r_timestamp >= staging.r_timestamp
+                           )
+                              ),
+          --   Records that will be inserted (don't exist in target table or exist
+          --   in the target table but the hashdiff changed). As the r_timestamp is fetched
+          --   from the staging table, these records will always be included in the
+          --   WHEN NOT MATCHED condition of the MERGE command.
+          staging_satellite_affected_records AS (
+          SELECT
+            staging.h_customer_hashkey,
+            staging.l_order_customer_hashkey,
+            staging.ls_order_customer_eff_hashdiff,
+            staging.r_timestamp,
+            staging.r_source
+            , staging.dummy_descriptive_field
+          FROM filtered_staging AS staging
+            LEFT JOIN filtered_effectivity_satellite AS satellite
+                      ON (satellite.h_customer_hashkey = staging.h_customer_hashkey)
+          WHERE satellite.l_order_customer_hashkey IS NULL
+             OR satellite.s_hashdiff <> staging.ls_order_customer_eff_hashdiff
+          UNION ALL
+          --  Records from the target table that will have its r_timestamp_end updated
+          --  (hashkey already exists in target table, but hashdiff changed). As the
+          --  r_timestamp is fetched from the target table, these records will always be
+          --  included in the WHEN MATCHED condition of the MERGE command.
+          SELECT
+            satellite.h_customer_hashkey,
+            satellite.l_order_customer_hashkey,
+            satellite.s_hashdiff AS ls_order_customer_eff_hashdiff,
+            satellite.r_timestamp,
+            satellite.r_source
+            , satellite.dummy_descriptive_field
+          FROM filtered_staging AS staging
+            INNER JOIN filtered_effectivity_satellite AS satellite
+                       ON (satellite.h_customer_hashkey = staging.h_customer_hashkey)
+          WHERE satellite.s_hashdiff <> staging.ls_order_customer_eff_hashdiff
+                                                )
         SELECT
-          satellite.h_customer_hashkey,
-          satellite.l_order_customer_hashkey,
-          satellite.s_hashdiff AS ls_order_customer_eff_hashdiff,
-          satellite.r_timestamp,
-          satellite.r_source
-          , satellite.dummy_descriptive_field
-        FROM filtered_staging AS staging
-          INNER JOIN effectivity_satellite AS satellite
-                     ON (satellite.h_customer_hashkey = staging.h_customer_hashkey)
-        WHERE satellite.s_hashdiff <> staging.ls_order_customer_eff_hashdiff
-      )
-    SELECT
-      l_order_customer_hashkey,
-      ls_order_customer_eff_hashdiff,
-      r_timestamp AS r_timestamp,
-      LEAD(DATEADD(milliseconds, - 1, r_timestamp), 1, CAST('9999-12-31T00:00:00.000000Z' AS TIMESTAMP)) OVER (PARTITION BY h_customer_hashkey ORDER BY r_timestamp) AS r_timestamp_end,
-      r_source
-      , dummy_descriptive_field
-    FROM staging_satellite_affected_records
-  ) AS staging
+          l_order_customer_hashkey,
+          ls_order_customer_eff_hashdiff,
+          r_timestamp AS r_timestamp,
+          LEAD(DATEADD(milliseconds, - 1, r_timestamp), 1, CAST('9999-12-31T00:00:00.000000Z' AS TIMESTAMP)) OVER (PARTITION BY h_customer_hashkey ORDER BY r_timestamp) AS r_timestamp_end,
+          r_source
+          , dummy_descriptive_field
+        FROM staging_satellite_affected_records
+        ) AS staging
   ON (satellite.l_order_customer_hashkey = staging.l_order_customer_hashkey
-      AND satellite.r_timestamp = staging.r_timestamp)
+    AND satellite.r_timestamp = staging.r_timestamp)
   WHEN MATCHED THEN
     UPDATE SET satellite.r_timestamp_end = staging.r_timestamp_end
   WHEN NOT MATCHED
     THEN
     INSERT (l_order_customer_hashkey, s_hashdiff, r_timestamp, r_timestamp_end, r_source, dummy_descriptive_field)
       VALUES (
                staging.l_order_customer_hashkey,
```

### Comparing `diepvries-0.6.4/test/sql/expected_result_hashdiff.sql` & `diepvries-0.7.0/test/sql/expected_result_hashdiff.sql`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/test/sql/expected_result_hub.sql` & `diepvries-0.7.0/test/sql/expected_result_hub.sql`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/test/sql/expected_result_link.sql` & `diepvries-0.7.0/test/sql/expected_result_link.sql`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/test/sql/expected_result_role_playing_hub.sql` & `diepvries-0.7.0/test/sql/expected_result_role_playing_hub.sql`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/test/sql/expected_result_satellite.sql` & `diepvries-0.7.0/test/sql/expected_result_satellite.sql`

 * *Files 2% similar despite different names*

```diff
@@ -1,68 +1,69 @@
 MERGE INTO dv.hs_customer AS satellite
   USING (
-    WITH
-      filtered_staging AS (
-        SELECT DISTINCT
-          staging.h_customer_hashkey,
-          staging.hs_customer_hashdiff,
-          staging.r_timestamp,
-          staging.r_source
-          , staging.test_string, staging.test_date, staging.test_timestamp_ntz, staging.test_integer, staging.test_decimal, staging.x_customer_id, staging.grouping_key, staging.test_geography, staging.test_array, staging.test_object, staging.test_variant, staging.test_timestamp_tz, staging.test_timestamp_ltz, staging.test_time, staging.test_boolean, staging.test_real
-        FROM dv_stg.orders_20190806_000000 AS staging
-          CROSS JOIN (
-                       SELECT
-                         MAX(r_timestamp) AS max_r_timestamp
-                       FROM dv.hs_customer
-                     ) AS max_satellite_timestamp
-        WHERE staging.r_timestamp >= COALESCE(max_satellite_timestamp.max_r_timestamp, '1970-01-01 00:00:00')
-      ),
-      staging_satellite_affected_records AS (
-        /* Records that will be inserted (don't exist in target table or exist
-          in the target table but the hashdiff changed). As the r_timestamp is fetched
-          from the staging table, these records will always be included in the
-          WHEN NOT MATCHED condition of the MERGE command. */
-        SELECT
-          staging.h_customer_hashkey,
-          staging.hs_customer_hashdiff,
-          staging.r_timestamp,
-          staging.r_source
-          , staging.test_string, staging.test_date, staging.test_timestamp_ntz, staging.test_integer, staging.test_decimal, staging.x_customer_id, staging.grouping_key, staging.test_geography, staging.test_array, staging.test_object, staging.test_variant, staging.test_timestamp_tz, staging.test_timestamp_ltz, staging.test_time, staging.test_boolean, staging.test_real
-        FROM filtered_staging AS staging
-          LEFT OUTER JOIN dv.hs_customer AS satellite
-                          ON (staging.h_customer_hashkey = satellite.h_customer_hashkey
+        WITH
+          filtered_staging AS (
+          SELECT DISTINCT
+            staging.h_customer_hashkey,
+            staging.hs_customer_hashdiff,
+            staging.r_timestamp,
+            staging.r_source
+            , staging.test_string, staging.test_date, staging.test_timestamp_ntz, staging.test_integer, staging.test_decimal, staging.x_customer_id, staging.grouping_key, staging.test_geography, staging.test_array, staging.test_object, staging.test_variant, staging.test_timestamp_tz, staging.test_timestamp_ltz, staging.test_time, staging.test_boolean, staging.test_real
+          FROM dv_stg.orders_20190806_000000 AS staging
+          WHERE NOT EXISTS (
+                           SELECT
+                             1
+                           FROM dv.hs_customer AS satellite
+                           WHERE staging.h_customer_hashkey = satellite.h_customer_hashkey
+                             AND satellite.r_timestamp >= staging.r_timestamp
+                           )
+                              ),
+          --  Records that will be inserted (don't exist in target table or exist
+          --  in the target table but the hashdiff changed). As the r_timestamp is fetched
+          --  from the staging table, these records will always be included in the
+          --  WHEN NOT MATCHED condition of the MERGE command.
+          staging_satellite_affected_records AS (
+          SELECT
+            staging.h_customer_hashkey,
+            staging.hs_customer_hashdiff,
+            staging.r_timestamp,
+            staging.r_source
+            , staging.test_string, staging.test_date, staging.test_timestamp_ntz, staging.test_integer, staging.test_decimal, staging.x_customer_id, staging.grouping_key, staging.test_geography, staging.test_array, staging.test_object, staging.test_variant, staging.test_timestamp_tz, staging.test_timestamp_ltz, staging.test_time, staging.test_boolean, staging.test_real
+          FROM filtered_staging AS staging
+            LEFT OUTER JOIN dv.hs_customer AS satellite
+                            ON (staging.h_customer_hashkey = satellite.h_customer_hashkey
                               AND satellite.r_timestamp_end = CAST('9999-12-31T00:00:00.000000Z' AS TIMESTAMP))
-        WHERE satellite.h_customer_hashkey IS NULL
-           OR satellite.s_hashdiff <> staging.hs_customer_hashdiff
-        UNION ALL
-        /* Records from the target table that will have its r_timestamp_end updated
-          (hashkey already exists in target table, but hashdiff changed). As the
-          r_timestamp is fetched from the target table, these records will always be
-          included in the WHEN MATCHED condition of the MERGE command. */
+          WHERE satellite.h_customer_hashkey IS NULL
+             OR satellite.s_hashdiff <> staging.hs_customer_hashdiff
+          UNION ALL
+          -- Records from the target table that will have its r_timestamp_end updated
+          -- (hashkey already exists in target table, but hashdiff changed). As the
+          -- r_timestamp is fetched from the target table, these records will always be
+          -- included in the WHEN MATCHED condition of the MERGE command.
+          SELECT
+            satellite.h_customer_hashkey,
+            satellite.s_hashdiff,
+            satellite.r_timestamp,
+            satellite.r_source
+            , satellite.test_string, satellite.test_date, satellite.test_timestamp_ntz, satellite.test_integer, satellite.test_decimal, satellite.x_customer_id, satellite.grouping_key, satellite.test_geography, satellite.test_array, satellite.test_object, satellite.test_variant, satellite.test_timestamp_tz, satellite.test_timestamp_ltz, satellite.test_time, satellite.test_boolean, satellite.test_real
+          FROM dv.hs_customer AS satellite
+            INNER JOIN filtered_staging AS staging
+                       ON (staging.h_customer_hashkey = satellite.h_customer_hashkey
+                         AND satellite.r_timestamp_end = CAST('9999-12-31T00:00:00.000000Z' AS TIMESTAMP))
+          WHERE staging.hs_customer_hashdiff <> satellite.s_hashdiff
+                                                )
         SELECT
-          satellite.h_customer_hashkey,
-          satellite.s_hashdiff,
-          satellite.r_timestamp,
-          satellite.r_source
-          , satellite.test_string, satellite.test_date, satellite.test_timestamp_ntz, satellite.test_integer, satellite.test_decimal, satellite.x_customer_id, satellite.grouping_key, satellite.test_geography, satellite.test_array, satellite.test_object, satellite.test_variant, satellite.test_timestamp_tz, satellite.test_timestamp_ltz, satellite.test_time, satellite.test_boolean, satellite.test_real
-        FROM dv.hs_customer AS satellite
-          INNER JOIN filtered_staging AS staging
-                     ON (staging.h_customer_hashkey = satellite.h_customer_hashkey
-                      AND satellite.r_timestamp_end = CAST('9999-12-31T00:00:00.000000Z' AS TIMESTAMP))
-        WHERE staging.hs_customer_hashdiff <> satellite.s_hashdiff
-      )
-    SELECT
-      h_customer_hashkey,
-      hs_customer_hashdiff,
-      r_timestamp AS r_timestamp,
-      LEAD(DATEADD(milliseconds, - 1, r_timestamp), 1, CAST('9999-12-31T00:00:00.000000Z' AS TIMESTAMP)) OVER (PARTITION BY h_customer_hashkey ORDER BY r_timestamp) AS r_timestamp_end,
-      r_source
-      , test_string, test_date, test_timestamp_ntz, test_integer, test_decimal, x_customer_id, grouping_key, test_geography, test_array, test_object, test_variant, test_timestamp_tz, test_timestamp_ltz, test_time, test_boolean, test_real
-    FROM staging_satellite_affected_records
-  ) AS staging
+          h_customer_hashkey,
+          hs_customer_hashdiff,
+          r_timestamp AS r_timestamp,
+          LEAD(DATEADD(milliseconds, - 1, r_timestamp), 1, CAST('9999-12-31T00:00:00.000000Z' AS TIMESTAMP)) OVER (PARTITION BY h_customer_hashkey ORDER BY r_timestamp) AS r_timestamp_end,
+          r_source
+          , test_string, test_date, test_timestamp_ntz, test_integer, test_decimal, x_customer_id, grouping_key, test_geography, test_array, test_object, test_variant, test_timestamp_tz, test_timestamp_ltz, test_time, test_boolean, test_real
+        FROM staging_satellite_affected_records
+        ) AS staging
   ON (satellite.h_customer_hashkey = staging.h_customer_hashkey
     AND satellite.r_timestamp = staging.r_timestamp)
   WHEN MATCHED THEN
     UPDATE SET satellite.r_timestamp_end = staging.r_timestamp_end
   WHEN NOT MATCHED
     THEN
     INSERT (h_customer_hashkey, s_hashdiff, r_timestamp, r_timestamp_end, r_source, test_string, test_date, test_timestamp_ntz, test_integer, test_decimal, x_customer_id, grouping_key, test_geography, test_array, test_object, test_variant, test_timestamp_tz, test_timestamp_ltz, test_time, test_boolean, test_real)
```

### Comparing `diepvries-0.6.4/test/sql/expected_result_staging.sql` & `diepvries-0.7.0/test/sql/expected_result_staging.sql`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/test/test_data_vault_load.py` & `diepvries-0.7.0/test/test_data_vault_load.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/test/test_field.py` & `diepvries-0.7.0/test/test_field.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/test/test_hub.py` & `diepvries-0.7.0/test/test_hub.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/test/test_link.py` & `diepvries-0.7.0/test/test_link.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/test/test_satellite.py` & `diepvries-0.7.0/test/test_satellite.py`

 * *Files identical despite different names*

### Comparing `diepvries-0.6.4/tox.ini` & `diepvries-0.7.0/tox.ini`

 * *Files identical despite different names*

