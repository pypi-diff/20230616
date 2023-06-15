# Comparing `tmp/schematicpy-23.1.1.tar.gz` & `tmp/schematicpy-23.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schematicpy-23.1.1.tar", max compression
+gzip compressed data, was "schematicpy-23.6.1.tar", max compression
```

## Comparing `schematicpy-23.1.1.tar` & `schematicpy-23.6.1.tar`

### file list

```diff
@@ -1,52 +1,51 @@
--rw-r--r--   0        0        0     1073 2023-01-19 15:31:01.458310 schematicpy-23.1.1/LICENSE
--rw-r--r--   0        0        0    16379 2023-01-19 15:31:01.458310 schematicpy-23.1.1/README.md
--rw-r--r--   0        0        0     3007 2023-01-19 15:31:28.166390 schematicpy-23.1.1/pyproject.toml
--rw-r--r--   0        0        0     1351 2023-01-19 15:31:01.462310 schematicpy-23.1.1/schematic/__init__.py
--rw-r--r--   0        0        0     1421 2023-01-19 15:31:01.462310 schematicpy-23.1.1/schematic/__main__.py
--rw-r--r--   0        0        0     4773 2023-01-19 15:31:01.462310 schematicpy-23.1.1/schematic/configuration.py
--rw-r--r--   0        0        0      663 2023-01-19 15:31:01.462310 schematicpy-23.1.1/schematic/etc/README.md
--rw-r--r--   0        0        0    76063 2023-01-19 15:31:01.462310 schematicpy-23.1.1/schematic/etc/data_models/biothings.model.jsonld
--rw-r--r--   0        0        0  1387510 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/etc/data_models/schema_org.model.jsonld
--rw-r--r--   0        0        0     4414 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/etc/validation_schemas/class.schema.json
--rw-r--r--   0        0        0     9914 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/etc/validation_schemas/model.schema.json
--rw-r--r--   0        0        0     5021 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/etc/validation_schemas/property.schema.json
--rw-r--r--   0        0        0     2446 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/exceptions.py
--rw-r--r--   0        0        0     9202 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/help.py
--rw-r--r--   0        0        0     3172 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/loader.py
--rw-r--r--   0        0        0       59 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/manifest/__init__.py
--rw-r--r--   0        0        0     9012 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/manifest/commands.py
--rw-r--r--   0        0        0    70638 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/manifest/generator.py
--rw-r--r--   0        0        0    20805 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/models/GE_Helpers.py
--rw-r--r--   0        0        0       52 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/models/__init__.py
--rw-r--r--   0        0        0     7373 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/models/commands.py
--rw-r--r--   0        0        0    16405 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/models/metadata.py
--rw-r--r--   0        0        0    42823 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/models/validate_attribute.py
--rw-r--r--   0        0        0    10998 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/models/validate_manifest.py
--rw-r--r--   0        0        0      166 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/schemas/__init__.py
--rw-r--r--   0        0        0     2467 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/schemas/commands.py
--rw-r--r--   0        0        0     4291 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/schemas/curie.py
--rw-r--r--   0        0        0    33708 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/schemas/df_parser.py
--rw-r--r--   0        0        0    46434 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/schemas/explorer.py
--rw-r--r--   0        0        0    30347 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/schemas/generator.py
--rw-r--r--   0        0        0     7100 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/schemas/validator.py
--rw-r--r--   0        0        0       96 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/store/__init__.py
--rw-r--r--   0        0        0      218 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/store/base.py
--rw-r--r--   0        0        0    75314 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/store/synapse.py
--rw-r--r--   0        0        0      787 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/utils/__init__.py
--rw-r--r--   0        0        0     4710 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/utils/cli_utils.py
--rw-r--r--   0        0        0     2785 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/utils/curie_utils.py
--rw-r--r--   0        0        0     5922 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/utils/df_utils.py
--rw-r--r--   0        0        0      587 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/utils/general.py
--rw-r--r--   0        0        0     7869 2023-01-19 15:31:01.470310 schematicpy-23.1.1/schematic/utils/google_api_utils.py
--rw-r--r--   0        0        0     1148 2023-01-19 15:31:01.474310 schematicpy-23.1.1/schematic/utils/io_utils.py
--rw-r--r--   0        0        0     9804 2023-01-19 15:31:01.474310 schematicpy-23.1.1/schematic/utils/schema_utils.py
--rw-r--r--   0        0        0    10865 2023-01-19 15:31:01.474310 schematicpy-23.1.1/schematic/utils/validate_rules_utils.py
--rw-r--r--   0        0        0     2263 2023-01-19 15:31:01.474310 schematicpy-23.1.1/schematic/utils/validate_utils.py
--rw-r--r--   0        0        0      236 2023-01-19 15:31:01.474310 schematicpy-23.1.1/schematic/utils/viz_utils.py
--rw-r--r--   0        0        0       81 2023-01-19 15:31:01.474310 schematicpy-23.1.1/schematic/version.py
--rw-r--r--   0        0        0      135 2023-01-19 15:31:01.474310 schematicpy-23.1.1/schematic/visualization/__init__.py
--rw-r--r--   0        0        0     8254 2023-01-19 15:31:01.474310 schematicpy-23.1.1/schematic/visualization/attributes_explorer.py
--rw-r--r--   0        0        0     3480 2023-01-19 15:31:01.474310 schematicpy-23.1.1/schematic/visualization/commands.py
--rw-r--r--   0        0        0    37113 2023-01-19 15:31:01.474310 schematicpy-23.1.1/schematic/visualization/tangled_tree.py
--rw-r--r--   0        0        0    18711 1970-01-01 00:00:00.000000 schematicpy-23.1.1/setup.py
--rw-r--r--   0        0        0    18660 1970-01-01 00:00:00.000000 schematicpy-23.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-15 23:22:47.239571 schematicpy-23.6.1/LICENSE
+-rw-r--r--   0        0        0    16389 2023-06-15 23:22:47.239571 schematicpy-23.6.1/README.md
+-rw-r--r--   0        0        0     3356 2023-06-15 23:23:20.580086 schematicpy-23.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1411 2023-06-15 23:22:47.239571 schematicpy-23.6.1/schematic/__init__.py
+-rw-r--r--   0        0        0     1421 2023-06-15 23:22:47.239571 schematicpy-23.6.1/schematic/__main__.py
+-rw-r--r--   0        0        0     4843 2023-06-15 23:22:47.239571 schematicpy-23.6.1/schematic/configuration.py
+-rw-r--r--   0        0        0      663 2023-06-15 23:22:47.239571 schematicpy-23.6.1/schematic/etc/README.md
+-rw-r--r--   0        0        0    76063 2023-06-15 23:22:47.239571 schematicpy-23.6.1/schematic/etc/data_models/biothings.model.jsonld
+-rw-r--r--   0        0        0  1387510 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/etc/data_models/schema_org.model.jsonld
+-rw-r--r--   0        0        0     4414 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/etc/validation_schemas/class.schema.json
+-rw-r--r--   0        0        0     9914 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/etc/validation_schemas/model.schema.json
+-rw-r--r--   0        0        0     5021 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/etc/validation_schemas/property.schema.json
+-rw-r--r--   0        0        0     3129 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/exceptions.py
+-rw-r--r--   0        0        0    10598 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/help.py
+-rw-r--r--   0        0        0     3415 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/loader.py
+-rw-r--r--   0        0        0       59 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/manifest/__init__.py
+-rw-r--r--   0        0        0     9375 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/manifest/commands.py
+-rw-r--r--   0        0        0    74507 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/manifest/generator.py
+-rw-r--r--   0        0        0    22894 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/models/GE_Helpers.py
+-rw-r--r--   0        0        0       52 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/models/__init__.py
+-rw-r--r--   0        0        0     6912 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/models/commands.py
+-rw-r--r--   0        0        0    16680 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/models/metadata.py
+-rw-r--r--   0        0        0    44816 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/models/validate_attribute.py
+-rw-r--r--   0        0        0    11604 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/models/validate_manifest.py
+-rw-r--r--   0        0        0      166 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/schemas/__init__.py
+-rw-r--r--   0        0        0     2470 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/schemas/commands.py
+-rw-r--r--   0        0        0     4291 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/schemas/curie.py
+-rw-r--r--   0        0        0    34388 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/schemas/df_parser.py
+-rw-r--r--   0        0        0    46753 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/schemas/explorer.py
+-rw-r--r--   0        0        0    30347 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/schemas/generator.py
+-rw-r--r--   0        0        0     7100 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/schemas/validator.py
+-rw-r--r--   0        0        0       96 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/store/__init__.py
+-rw-r--r--   0        0        0      218 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/store/base.py
+-rw-r--r--   0        0        0   113572 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/store/synapse.py
+-rw-r--r--   0        0        0      787 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/utils/__init__.py
+-rw-r--r--   0        0        0     4765 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/utils/cli_utils.py
+-rw-r--r--   0        0        0     2785 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/utils/curie_utils.py
+-rw-r--r--   0        0        0     8086 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/utils/df_utils.py
+-rw-r--r--   0        0        0     6338 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/utils/general.py
+-rw-r--r--   0        0        0     8197 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/utils/google_api_utils.py
+-rw-r--r--   0        0        0     1148 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/utils/io_utils.py
+-rw-r--r--   0        0        0     9804 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/utils/schema_utils.py
+-rw-r--r--   0        0        0     9565 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/utils/validate_rules_utils.py
+-rw-r--r--   0        0        0     2629 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/utils/validate_utils.py
+-rw-r--r--   0        0        0      236 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/utils/viz_utils.py
+-rw-r--r--   0        0        0      119 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/version.py
+-rw-r--r--   0        0        0      135 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/visualization/__init__.py
+-rw-r--r--   0        0        0    10207 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/visualization/attributes_explorer.py
+-rw-r--r--   0        0        0     3480 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/visualization/commands.py
+-rw-r--r--   0        0        0    37113 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/visualization/tangled_tree.py
+-rw-r--r--   0        0        0    18820 1970-01-01 00:00:00.000000 schematicpy-23.6.1/PKG-INFO
```

### Comparing `schematicpy-23.1.1/LICENSE` & `schematicpy-23.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `schematicpy-23.1.1/README.md` & `schematicpy-23.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 - [Contributors](#contributors)
 
 # Introduction
 SCHEMATIC is an acronym for _Schema Engine for Manifest Ingress and Curation_. The Python based infrastructure provides a _novel_ schema-based, metadata ingress ecosystem, that is meant to streamline the process of biomedical dataset annotation, metadata validation and submission to a data repository for various data contributors.
 
 # Installation
 ## Installation Requirements
-* Python 3.7.1 or higher
+* Python version 3.9.0≤x<3.11.0 
 
 Note: You need to be a registered and certified user on [`synapse.org`](https://www.synapse.org/), and also have the right permissions to download the Google credentials files from Synapse.
 
 
 ## Installation guide for data curator app
 
 Create and activate a virtual environment within which you can install the package:
```

### Comparing `schematicpy-23.1.1/pyproject.toml` & `schematicpy-23.6.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,84 +1,95 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "schematicpy"
-version = "v23.1.1"
+version = "v23.6.1"
 description = "Package for biomedical data model and metadata ingress management"
-authors = [ "Milen Nikolov <milen.nikolov@sagebase.org>", "Sujay Patil <sujay.patil@sagebase.org>", "Bruno Grande <bruno.grande@sagebase.org>", "Robert Allaway <robert.allaway@sagebionetworks.org>", "Xengie Doan <xengie.doan@sagebase.org>",]
+authors = [ "Milen Nikolov <milen.nikolov@sagebase.org>", "Lingling Peng <lingling.peng@sagebase.org>", "Mialy Defelice <mialy.defelice@sagebase.org>", "Gianna Jordan <gianna.jordan@sagebase.org>", "Bruno Grande <bruno.grande@sagebase.org>", "Robert Allaway <robert.allaway@sagebionetworks.org>",]
 readme = "README.md"
 homepage = "https://github.com/Sage-Bionetworks/schematic"
 repository = "https://github.com/Sage-Bionetworks/schematic"
 documentation = "https://github.com/Sage-Bionetworks/schematic"
 keywords = [ "schema", "metadata", "validation", "data model", "linked data",]
 classifiers = [ "Development Status :: 4 - Beta", "Environment :: Console", "Intended Audience :: Science/Research", "Topic :: Software Development :: Libraries :: Python Modules",]
 [[tool.poetry.packages]]
 include = "schematic"
 
 [tool.black]
 line-length = 88
-target-version = [ "py37",]
 include = "\\.pyi?$"
 exclude = "(\n  /(\n      \\.eggs\n    | \\.git\n    | \\.venv\n    | dist\n  )/\n)\n"
 
 [tool.poetry.scripts]
 schematic = "schematic.__main__:main"
 
 [tool.poetry.dependencies]
-python = ">=3.7.1,<3.11"
-click = "^7.1.2"
-click-log = "^0.3.2"
-google-api-python-client = "^1.12.8"
-google-auth-httplib2 = "^0.0.4"
-google-auth-oauthlib = "^0.4.2"
-graphviz = "^0.16"
+python = ">=3.9.0,<3.11"
+click = "^8.0.0"
+click-log = "^0.4.0"
+google-api-python-client = "^2.0.0"
+google-auth-httplib2 = "^0.1.0"
+google-auth-oauthlib = "^0.8.0"
+graphviz = "^0.20.0"
 inflection = "^0.5.1"
-jsonschema = "^3.2.0"
-networkx = "^2.5"
+jsonschema = "^4.0.0"
+networkx = ">=2.2.8"
 numpy = "^1.21.1"
-oauth2client = "<4.0.0"
+oauth2client = "^4.1.0"
 pandas = "^1.3.1"
 pygsheets = "^2.0.4"
-PyYAML = "^5.4.1"
-rdflib = "^5.0.0"
-setuptools = "^52.0.0"
-synapseclient = "^2.6.0"
+PyYAML = "^6.0.0"
+rdflib = "^6.0.0"
+setuptools = "^66.0.0"
+synapseclient = "^2.7.0"
 tenacity = "^8.0.1"
 toml = "^0.10.2"
-Flask = "^1.1.4"
+Flask = "^2.0.0"
 great-expectations = "^0.15.0"
-sphinx-click = "^3.1.0"
-MarkupSafe = "2.0.1"
-itsdangerous = "1.1.0"
-Jinja2 = "2.11.3"
+sphinx-click = "^4.0.0"
+MarkupSafe = "2.1.0"
+itsdangerous = "^2.0.0"
+Jinja2 = ">2.11.3"
 openpyxl = "^3.0.9"
 Flask-Cors = "^3.0.10"
 pdoc = "^12.2.0"
 dateparser = "^1.1.4"
+pandarallel = "^1.6.4"
+pyopenssl = "^23.0.0"
+typing-extensions = "<4.6.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.2"
-pytest-cov = "^2.11.1"
+pytest = "^7.0.0"
+pytest-cov = "^4.0.0"
 pytest-mock = "^3.5.1"
-flake8 = "^3.8.4"
-python-dotenv = "^0.15.0"
+flake8 = "^6.0.0"
+python-dotenv = "^0.21.0"
+black = "^22.6.0"
+mypy = "^0.982"
+pylint = "^2.16.1"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--verbose"
 testpaths = [ "tests",]
 filterwarnings = [ "ignore::DeprecationWarning",]
-markers = [ "google_credentials_needed: marks tests requiring Google credentials (skipped on GitHub CI) ", "schematic_api: marks tests requiring running API locally (skipped on GitHub CI)\n    ", "rule_combos: marks tests covering combinations of rules that aren't always necessary and can add significantly to CI runtime (skipped on GitHub CI unless prompted to run in commit message)\n    ", "table_operations: marks tests covering table operations that pass locally but fail on CI due to interactions with Synapse (skipped on GitHub CI)\n    ",]
+markers = [ "google_credentials_needed: marks tests requiring Google credentials (skipped on GitHub CI) ", "schematic_api: marks tests covering API functionality (skipped on regular GitHub CI test suite)\n    ", "rule_combos: marks tests covering combinations of rules that aren't always necessary and can add significantly to CI runtime (skipped on GitHub CI unless prompted to run in commit message)\n    ", "table_operations: marks tests covering table operations that pass locally but fail on CI due to interactions with Synapse (skipped on GitHub CI)\n    ", "rule_benchmark: marks tests covering validation rule benchmarking\n    ",]
 
 [tool.poetry.dependencies.connexion]
 extras = [ "swagger-ui",]
 version = "^2.8.0"
 
 [tool.poetry.dependencies."backports.zoneinfo"]
 markers = "python_version < \"3.9\""
 version = "^0.2.1"
 
-[tool.poetry.dev-dependencies.black]
-version = "^20.8b1"
-allow-prereleases = true
+[tool.poetry.dependencies.schematic-db]
+version = "^0.0.20"
+extras = [ "synapse",]
+
+[tool.poetry.group.aws]
+optional = true
+
+[tool.poetry.group.aws.dependencies]
+uWSGI = "^2.0.21"
```

### Comparing `schematicpy-23.1.1/schematic/__init__.py` & `schematicpy-23.6.1/schematic/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     datefmt="%Y-%m-%d %H:%M:%S",
 )
 
 
 # Suppress INFO-level logging from some dependencies
 logging.getLogger("keyring").setLevel(logging.ERROR)
 logging.getLogger("rdflib").setLevel(logging.ERROR)
+logging.getLogger("Synapse storage").setLevel(logging.INFO)
 
 logger = logging.getLogger(__name__)
 click_log.basic_config(logger)
 
 
 @click.command("init", short_help=query_dict(init_command, ("init", "short_help")))
 @click_log.simple_verbosity_option(logger)
```

### Comparing `schematicpy-23.1.1/schematic/__main__.py` & `schematicpy-23.6.1/schematic/__main__.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.1.1/schematic/configuration.py` & `schematicpy-23.6.1/schematic/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,32 @@
+from typing import Optional
 import os
 import yaml
 
 
 class Configuration(object):
     def __init__(self):
         # path to config.yml file
         self.CONFIG_PATH = None
         # entire configuration data
         self.DATA = None
 
-
     def __getattribute__(self, name):
         value = super().__getattribute__(name)
         if value is None and "SCHEMATIC_CONFIG_CONTENT" in os.environ:
             self.load_config_content_from_env()
             value = super().__getattribute__(name)
         elif value is None and "SCHEMATIC_CONFIG" in os.environ:
             self.load_config_from_env()
             value = super().__getattribute__(name)
-        elif value is None and "SCHEMATIC_CONFIG" not in os.environ and "SCHEMATIC_CONFIG_CONTENT" not in os.environ:
+        elif (
+            value is None
+            and "SCHEMATIC_CONFIG" not in os.environ
+            and "SCHEMATIC_CONFIG_CONTENT" not in os.environ
+        ):
             raise AttributeError(
                 "The '%s' configuration field was accessed, but it hasn't been "
                 "set yet, presumably because the schematic.CONFIG.load_config() "
                 "method hasn't been run yet. Alternatively, you can re-run this "
                 "code with the 'SCHEMATIC_CONFIG' environment variable set to "
                 "the config.yml file, which will be automatically loaded." % name
             )
@@ -34,24 +38,24 @@
     def get(self, key, default):
         try:
             value = self[key]
         except AttributeError or KeyError:
             value = default
         return value
 
-    def load_config_content(self, str_yaml: str) -> dict:
-        try: 
+    def load_config_content(self, str_yaml: str) -> Optional[dict]:
+        try:
             config_data = yaml.safe_load(str_yaml)
         except yaml.YAMLError as exc:
             print(exc)
             return None
         return config_data
 
     @staticmethod
-    def load_yaml(file_path: str) -> dict:
+    def load_yaml(file_path: str) -> Optional[dict]:
         with open(file_path, "r") as stream:
             try:
                 config_data = yaml.safe_load(stream)
             except yaml.YAMLError as exc:
                 print(exc)
                 return None
         return config_data
@@ -78,24 +82,22 @@
             "environment variable: %s" % schematic_config
         )
         return self.load_config(schematic_config)
 
     def load_config_content_from_env(self):
         schematic_config_content = os.environ["SCHEMATIC_CONFIG_CONTENT"]
 
-        print(
-            'Loading content of config file:  %s' % schematic_config_content
-        )
+        print("Loading content of config file:  %s" % schematic_config_content)
 
         config_content_yaml = self.load_config_content(schematic_config_content)
         self.DATA = config_content_yaml
 
         return self.DATA
 
-    def load_config(self, config_path=None, asset_view=None): 
+    def load_config(self, config_path=None, asset_view=None):
         # If config_path is None, try loading from environment
         if config_path is None and "SCHEMATIC_CONFIG" in os.environ:
             return self.load_config_from_env()
         # Otherwise, raise an error
         elif config_path is None and "SCHEMATIC_CONFIG" not in os.environ:
             raise ValueError(
                 "No configuration file provided to the `config_path` argument "
@@ -104,16 +106,16 @@
             )
         # Load configuration YAML file
         config_path = os.path.expanduser(config_path)
         config_path = os.path.abspath(config_path)
         self.DATA = self.load_yaml(config_path)
         self.CONFIG_PATH = config_path
         # handle user input (for API endpoints)
-        if asset_view: 
-            self.DATA['synapse']['master_fileview'] = asset_view
+        if asset_view:
+            self.DATA["synapse"]["master_fileview"] = asset_view
 
         # Return self.DATA as a side-effect
         return self.DATA
 
     @property
     def SERVICE_ACCT_CREDS(self):
         self._SERVICE_ACCT_CREDS = self.DATA["definitions"]["service_acct_creds"]
```

### Comparing `schematicpy-23.1.1/schematic/etc/README.md` & `schematicpy-23.6.1/schematic/etc/README.md`

 * *Files identical despite different names*

### Comparing `schematicpy-23.1.1/schematic/etc/data_models/biothings.model.jsonld` & `schematicpy-23.6.1/schematic/etc/data_models/biothings.model.jsonld`

 * *Files identical despite different names*

### Comparing `schematicpy-23.1.1/schematic/etc/data_models/schema_org.model.jsonld` & `schematicpy-23.6.1/schematic/etc/data_models/schema_org.model.jsonld`

 * *Files identical despite different names*

### Comparing `schematicpy-23.1.1/schematic/etc/validation_schemas/class.schema.json` & `schematicpy-23.6.1/schematic/etc/validation_schemas/class.schema.json`

 * *Files identical despite different names*

### Comparing `schematicpy-23.1.1/schematic/etc/validation_schemas/model.schema.json` & `schematicpy-23.6.1/schematic/etc/validation_schemas/model.schema.json`

 * *Files identical despite different names*

### Comparing `schematicpy-23.1.1/schematic/etc/validation_schemas/property.schema.json` & `schematicpy-23.6.1/schematic/etc/validation_schemas/property.schema.json`

 * *Files identical despite different names*

### Comparing `schematicpy-23.1.1/schematic/exceptions.py` & `schematicpy-23.6.1/schematic/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,62 @@
+"""Schematic Exceptions"""
 from typing import Any, Sequence
 
 
 class MissingConfigValueError(Exception):
     """Exception raised when configuration value not provided in config file.
 
     Args:
         config_keys: tuple of keys as present in config file.
         message: custom/pre-defined error message to be returned.
 
     Returns:
         message.
     """
 
-    def __init__(self, config_keys: Sequence[Any], message: str = None) -> str:
+    def __init__(self, config_keys: Sequence[Any], message: str = None) -> None:
         config_keys_str = " > ".join(config_keys)
         self.message = (
             "The configuration value corresponding to the argument "
             f"({config_keys_str}) doesn't exist. "
             "Please provide a value in the configuration file."
         )
 
         if message:
             self.message = message
 
         super().__init__(self.message)
 
-    def __str__(self):
+    def __str__(self) -> str:
+        return f"{self.message}"
+
+
+class WrongEntityTypeError(Exception):
+    """Exception raised when the entity type is not desired
+
+    Args:
+        entity id: For synapse, thi
+        message: custom/pre-defined error message to be returned.
+
+    Returns:
+        message.
+    """
+
+    def __init__(self, syn_id: str, message: str = None) -> None:
+        self.message = (
+            f"'{syn_id}'' is not a desired entity type"
+            "Please ensure that you put in the right syn_id"
+        )
+
+        if message:
+            self.message = message
+
+        super().__init__(self.message)
+
+    def __str__(self) -> str:
         return f"{self.message}"
 
 
 class MissingConfigAndArgumentValueError(Exception):
     """Exception raised when configuration value not provided in config file.
 
     Args:
@@ -39,49 +66,49 @@
 
     Returns:
         message.
     """
 
     def __init__(
         self, arg_name: str, config_keys: Sequence[Any], message: str = None
-    ) -> str:
+    ) -> None:
         config_keys_str = " > ".join(config_keys)
         self.message = (
             f"The value corresponding to the CLI argument '--{arg_name}'"
             " doesn't exist. "
             "Please provide a value for either the CLI argument or "
             f"({config_keys_str}) in the configuration file."
         )
 
         if message:
             self.message = message
 
         super().__init__(self.message)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"{self.message}"
 
 
 class AccessCredentialsError(Exception):
     """Exception raised when provided access credentials cannot be resolved.
 
     Args:
         project: Platform/project (e.g., synID of a project)
         message: custom/pre-defined error message to be returned.
 
     Returns:
         message.
     """
 
-    def __init__(self, project: str, message: str = None) -> str:
+    def __init__(self, project: str, message: str = None) -> None:
         self.message = (
             f"Your access to '{project}'' could not be resolved. "
             "Please check your credentials and try again."
         )
 
         if message:
             self.message = message
 
         super().__init__(self.message)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"{self.message}"
```

### Comparing `schematicpy-23.1.1/schematic/help.py` & `schematicpy-23.6.1/schematic/help.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Help messages for CLI commands"""
+# pylint: disable=line-too-long
 #!/usr/bin/env python3
 
 # `schematic manifest` related sub-commands description
 manifest_commands = {
     "manifest": {
         "config": (
             "Specify the path to the `config.yml` using this option. This is a required argument."
@@ -32,26 +34,28 @@
                 "in that folder, then it will be pulled with the existing annotations for further annotation/modification. "
             ),
             "sheet_url": (
                 "This is a boolean flag. If flag is provided when command line utility is executed, result will be a link/URL "
                 "to the metadata manifest file. If not it will produce a pandas dataframe for the same."
             ),
             "output_csv": ("Path to where the CSV manifest template should be stored."),
-            "output_xlsx": ("Path to where the Excel manifest template should be stored."),
+            "output_xlsx": (
+                "Path to where the Excel manifest template should be stored."
+            ),
             "use_annotations": (
                 "This is a boolean flag. If flag is provided when command line utility is executed, it will prepopulate template "
                 "with existing annotations from Synapse."
             ),
             "json_schema": (
                 "Specify the path to the JSON Validation Schema for this argument. "
                 "You can either explicitly pass the `.json` file here or provide it in the `config.yml` file "
                 "as a value for the `(model > input > validation_schema)` key."
             ),
             "alphabetize_valid_values": (
-                "Specify to alphabetize valid attribute values either ascending (a) or descending (d)." 
+                "Specify to alphabetize valid attribute values either ascending (a) or descending (d)."
                 "Optional"
             ),
         },
         "migrate": {
             "short_help": (
                 "Specify the path to the `config.yml` using this option. "
                 "This is a required argument."
@@ -98,24 +102,37 @@
                 "data filled in your manifest template."
             ),
             "use_schema_label": (
                 "Store attributes using the schema label (--use_schema_label, default) or store attributes using the display label "
                 "(--use_display_label). Attribute display names in the schema must not only include characters that are "
                 "not accepted by Synapse. Annotation names may only contain: letters, numbers, '_' and '.'"
             ),
-            "hide_blanks":(
+            "hide_blanks": (
                 "This is a boolean flag. If flag is provided when command line utility is executed, annotations with blank values will be hidden from a dataset's annotation list in Synaspe."
                 "If not, annotations with blank values will be displayed."
             ),
-            "manifest_record_type":(
-                "Specify the way the manifest should be store as on Synapse. Options are 'entity', 'table' and "
-                "'both'. 'entity' will store the manifest as a csv and create Synapse files for each row in the manifest. "
-                "'table' will store the manifest as a table and a csv on Synapse. 'both' will do both of the options specified above. "
-                "Default value is 'table'."
-            ),      
+            "manifest_record_type": (
+                "Specify the way the manifest should be store as on Synapse. Options are 'file_only', 'file_and_entities', 'table_and_file' and "
+                "'table_file_and_entities'. 'file_and_entities' will store the manifest as a csv and create Synapse files for each row in the manifest. "
+                "'table_and_file' will store the manifest as a table and a csv on Synapse. "
+                "'file_only' will store the manifest as a csv only on Synapse."
+                "'table_file_and_entities' will perform the options file_with_entites and table in combination."
+                "Default value is 'table_file_and_entities'."
+            ),
+            "table_manipulation": (
+                "Specify the way the manifest tables should be store as on Synapse when one with the same name already exists. Options are 'replace' and 'upsert'. "
+                "'replace' will remove the rows and columns from the existing table and store the new rows and columns, preserving the name and synID. "
+                "'upsert' will add the new rows to the table and preserve the exisitng rows and columns in the existing table. "
+                "Default value is 'replace'. "
+                "Upsert specific requirements: {\n}"
+                "'upsert' should be used for initial table uploads if users intend to upsert into them at a later time."
+                "Using 'upsert' at creation will generate the metadata necessary for upsert functionality."
+                "Upsert functionality requires primary keys to be specified in the data model and manfiest as <component>_id."
+                "Currently it is required to use -dl/--use_display_label with table upserts."
+            ),
         },
         "validate": {
             "short_help": ("Validation of manifest files."),
             "manifest_path": (
                 "Specify the path to the metadata manifest file that you want to submit to a dataset on Synapse. "
                 "This is a required argument."
             ),
@@ -125,15 +142,15 @@
                 "it in the `config.yml` file as a value for the `(manifest > data_type)` key."
             ),
             "json_schema": (
                 "Specify the path to the JSON Validation Schema for this argument. "
                 "You can either explicitly pass the `.json` file here or provide it in the `config.yml` file "
                 "as a value for the `(model > input > validation_schema)` key."
             ),
-            "restrict_rules":(
+            "restrict_rules": (
                 "This is a boolean flag. If flag is provided when command line utility is executed, validation suite will only run with in-house validation rules, "
                 "and Great Expectations rules and suite will not be utilized."
                 "If not, the Great Expectations suite will be utilized and all rules will be available."
             ),
             "project_scope": (
                 "Specify a comma-separated list of projects to search through for cross manifest validation."
             ),
@@ -172,15 +189,16 @@
 
 viz_commands = {
     "visualization": {
         "config": (
             "Specify the path to the `config.yml` using this option. This is a required argument."
         ),
         "tangled_tree": {
-            "figure_type": ("Specify the type of schema visualization to make. Either 'dependency' or 'component'."
-                ),
-            "text_format": ("Specify the type of text to gather for tangled tree visualization, either 'plain' or 'highlighted'."
-                ),
-        }
+            "figure_type": (
+                "Specify the type of schema visualization to make. Either 'dependency' or 'component'."
+            ),
+            "text_format": (
+                "Specify the type of text to gather for tangled tree visualization, either 'plain' or 'highlighted'."
+            ),
+        },
     }
-    
 }
```

### Comparing `schematicpy-23.1.1/schematic/loader.py` & `schematicpy-23.6.1/schematic/loader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""Loader"""
+from typing import Any
+from collections.abc import Iterable
 from errno import ENOENT
 from os import pathsep
 from re import split
 from pkg_resources import (
     resource_exists,
     resource_filename,
     resource_stream,
@@ -13,95 +16,95 @@
 class InvalidResourceError(Exception):
     """
     Args:
         uri {String}: The URI which was requested within the given loader's
         that did not exist or was malformed.
     """
 
-    def __init__(self, namespace, requested_uri):
+    def __init__(self, namespace: str, requested_uri: str) -> None:
         self.namespace = namespace
         self.requested_uri = requested_uri
         self.message = "Resource does not exist or is declared incorrectly"
         self.errno = ENOENT
-        super(InvalidResourceError, self).__init__(self.message)
+        super().__init__(self.message)
 
-    def __str__(self):
-        return '{}({}), "{}" of {}'.format(
-            self.message, self.errno, self.requested_uri, self.namespace
+    def __str__(self) -> str:
+        return (
+            f'{self.message}({self.errno}), "{self.requested_uri}" of {self.namespace}'
         )
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return self.__str__()
 
 
-class Loader(object):
+class Loader:
     """
     Args:
     namespace {String}: The namespace within the package (relative to the package root)
     to load resources from. Using the magic variable __name__ is suggested as when the script
     is run as "__main__" it will load the most recent local resources instead of the cached
     egg resources.
 
     prefix {String}: Set a prefix for all URIs. Use a prefix if resources are centrally
     located in a single place the uri's will be prefixed automatically by the loader.
     """
 
-    def __init__(self, namespace, **opts):
+    def __init__(self, namespace: str, **opts: Any) -> None:
         self.namespace = namespace
         self.prefix = opts.get("prefix", "")
         self.local = opts.get("local", False)
 
         if not self.local:
             self.namespace = split(r"\.|\\|\/", self.namespace)[0]
 
-    def _resolve(self, uri):
+    def _resolve(self, uri: str) -> tuple[str, str]:
         resource_uri = "/".join([self.prefix] + uri.split(pathsep))
-        ns = self.namespace
+        namespace = self.namespace
 
-        if not resource_exists(ns, resource_uri):
-            raise InvalidResourceError(ns, resource_uri)
+        if not resource_exists(namespace, resource_uri):
+            raise InvalidResourceError(namespace, resource_uri)
 
-        return ns, resource_uri
+        return namespace, resource_uri
 
-    def read(self, uri):
+    def read(self, uri: str) -> Any:
         """
         Read entire contents of resource. Same as open('path...').read()
 
         Args:
             uri {String}: URI of the resource.
         """
-        ns, uri = self._resolve(uri)
-        return resource_string(ns, uri)
+        namespace, uri = self._resolve(uri)
+        return resource_string(namespace, uri)
 
-    def open(self, uri):
+    def open(self, uri: str) -> Any:
         """
         Open a file object like handle to the resource. Same as open('path...')
 
         Args:
             uri {String}: URI of the resource.
         """
-        ns, uri = self._resolve(uri)
-        return resource_stream(ns, uri)
+        namespace, uri = self._resolve(uri)
+        return resource_stream(namespace, uri)
 
-    def filename(self, uri):
+    def filename(self, uri: str) -> str:
         """
         Return the "most correct" filename for a resource. Same as os.path.normpath('path...')
 
         Args:
             uri {String}: URI of the resource.
         """
-        ns, uri = self._resolve(uri)
-        return resource_filename(ns, uri)
+        namespace, uri = self._resolve(uri)
+        return resource_filename(namespace, uri)
 
-    def list(self, url):
+    def list(self, url: str) -> Iterable[str]:
         """
         Return a list of all resources within the given URL
 
         Args:
             url {String}: URL of the resources.
         """
-        ns, uri = self._resolve(url)
-        return map(lambda x: url + "/" + x, resource_listdir(ns, uri))
+        namespace, uri = self._resolve(url)
+        return map(lambda x: url + "/" + x, resource_listdir(namespace, uri))
 
 
 # call Loader() and pass `schematic`, which is the global package namespace
 LOADER = Loader("schematic", prefix="etc")
```

### Comparing `schematicpy-23.1.1/schematic/manifest/commands.py` & `schematicpy-23.6.1/schematic/manifest/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from schematic.utils.cli_utils import fill_in_from_config, query_dict, parse_synIDs
 from schematic.help import manifest_commands
 from schematic import CONFIG
 from schematic.schemas.generator import SchemaGenerator
 from schematic.utils.google_api_utils import export_manifest_csv, export_manifest_excel, export_manifest_drive_service
 from schematic.store.synapse import SynapseStorage
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger('schematic')
 click_log.basic_config(logger)
 
 CONTEXT_SETTINGS = dict(help_option_names=["--help", "-h"])  # help options
 
 
 # invoke_without_command=True -> forces the application not to show aids before losing them with a --h
 @click.group(context_settings=CONTEXT_SETTINGS, invoke_without_command=True)
@@ -138,24 +138,33 @@
             alphabetize_valid_values=alphabetize_valid_values,
         )
 
         # call get_manifest() on manifest_generator
         # if output_xlsx gets specified, output_format = "excel"
         if output_xlsx: 
             output_format = "excel"
-
             # if file name is in the path, and that file does not exist
             if not os.path.exists(output_xlsx):
                 if ".xlsx" or ".xls" in output_xlsx:
                     path = Path(output_xlsx)
                     output_path = path.parent.absolute()
-                else: 
-                    logger.error(f"{output_xlsx} does not exists. Please try a valid file path")
-
-            else: 
+                    if not os.path.exists(output_path):
+                        raise ValueError(
+                            f"{output_path} does not exists. Please try a valid file path"
+                        )
+                else:
+                    raise ValueError(
+                            f"{output_xlsx} does not exists. Please try a valid file path"
+                        )
+            else:
+                # Check if base path itself exists.
+                if not os.path.exists(os.path.dirname(output_xlsx)):
+                    raise ValueError(
+                    f"{output_xlsx} does not exists. Please try a valid file path"
+                    )
                 output_path = output_xlsx
         else: 
             output_format = None
             output_path = None
 
         result = manifest_generator.get_manifest(
             dataset_id=dataset_id, sheet_url=sheet_url, json_schema=json_schema, output_format = output_format, output_path = output_path
@@ -251,23 +260,20 @@
     dry_run: bool,
 ):
     """
     Running CLI with manifest migration options.
     """
     jsonld = fill_in_from_config("jsonld", jsonld, ("model", "input", "location"))
 
-    access_token = os.getenv("SYNAPSE_ACCESS_TOKEN")
+    
     full_scope = project_scope + [archive_project]
-    if access_token:
-        synStore = SynapseStorage(access_token = access_token, project_scope = full_scope)
-    else:
-        synStore = SynapseStorage(project_scope = full_scope)  
+    synStore = SynapseStorage(project_scope = full_scope)  
 
     for project in project_scope:
         if not return_entities:
             logging.info("Re-uploading manifests as tables")
             synStore.upload_annotated_project_manifests_to_synapse(project, jsonld, dry_run)
         if archive_project:
             logging.info("Migrating entitites")
             synStore.move_entities_to_new_project(project, archive_project, return_entities, dry_run)
         
-    return 
+    return
```

### Comparing `schematicpy-23.1.1/schematic/manifest/generator.py` & `schematicpy-23.6.1/schematic/manifest/generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-import os
-import logging
-from typing import Dict, List, Tuple, Union
 from collections import OrderedDict
-from tempfile import NamedTemporaryFile
-
+import json
+import logging
+from openpyxl.styles import Font, Alignment, PatternFill
+from openpyxl import load_workbook
+from openpyxl.utils.dataframe import dataframe_to_rows
+import os
 import pandas as pd
+from pathlib import Path
 import pygsheets as ps
-import json
+from tempfile import NamedTemporaryFile
+from typing import Dict, List, Tuple, Union
 
 from schematic.schemas.generator import SchemaGenerator
 from schematic.utils.google_api_utils import (
     execute_google_api_requests,
     build_service_account_creds,
 )
 from schematic.utils.df_utils import update_df, load_df
@@ -18,16 +21,15 @@
 
 #TODO: This module should only be aware of the store interface
 # we shouldn't need to expose Synapse functionality explicitly
 from schematic.store.synapse import SynapseStorage
 
 from schematic import CONFIG
 from schematic.utils.google_api_utils import export_manifest_drive_service
-from openpyxl import load_workbook
-from pathlib import Path
+
 
 logger = logging.getLogger(__name__)
 
 
 
 class ManifestGenerator(object):
     def __init__(
@@ -177,21 +179,21 @@
 
             # if provided with a template manifest google sheet, use it
             spreadsheet_id = self._gdrive_copy_file(
                 CONFIG["style"]["google_manifest"]["master_template_id"], title
             )
 
         else:
+            spreadsheet_body = {
+            'properties': {
+                'title': title
+            }}
+
             # if no template, create an empty spreadsheet
-            spreadsheet = (
-                self.sheet_service.spreadsheets()
-                .create(body=spreadsheet, fields="spreadsheetId")
-                .execute()
-            )
-            spreadsheet_id = spreadsheet.get("spreadsheetId")
+            spreadsheet_id = self.sheet_service.spreadsheets().create(body=spreadsheet_body, fields="spreadsheetId").execute().get("spreadsheetId")
 
         return spreadsheet_id
 
     def _get_cell_borders(self, cell_range):
 
         # set border style request
         color = {
@@ -1219,15 +1221,15 @@
                     to the manifest
                 values(list[str]): valid values
         """
         # Get required fields
         required_metadata_fields = self._get_required_metadata_fields(
             json_schema, fields
         )
-        # Add additioal dependencies
+        # Add additional dependencies
         required_metadata_fields = self._gather_dependency_requirements(
             json_schema, required_metadata_fields
         )
 
         # Add additional metadata as entries to columns
         required_metadata_fields = self._get_additional_metadata(
             required_metadata_fields
@@ -1237,106 +1239,69 @@
     def get_empty_manifest(self, json_schema_filepath=None):
         """Create an empty manifest using specifications from the
         json schema.
         Args:
             json_schema_filepath (str): path to json schema file
         Returns:
             manifest_url (str): url of the google sheet manifest.
+        TODO:
+            Refactor to not be dependent on GS.
         """
         spreadsheet_id = self._create_empty_manifest_spreadsheet(self.title)
         json_schema = self._get_json_schema(json_schema_filepath)
 
         required_metadata_fields = self._gather_all_fields(
             json_schema["properties"].keys(), json_schema
         )
 
         manifest_url = self._create_empty_gs(
             required_metadata_fields, json_schema, spreadsheet_id
         )
         return manifest_url
 
-    def _get_missing_columns(self, wb_header, manifest_df):
-        # get headers from sheet 
-        manifest_df_header = manifest_df.columns
-
-        # find missing columns present in existing manifest but missing in latest schema
-        out_of_schema_columns = set(manifest_df_header) - set(wb_header)
-
-        return out_of_schema_columns
+    def _get_missing_columns(self, headers_1:list , headers_2:list) -> list:
+        """Compare two colunm sets and get cols that are in headers_1, but not headers_2
+        Args:
+            headers_1 (list): list of column headers
+            headers_2 (list): list of column headers
+        Returns: 
+            list: column headers in headers_1 but not headers_2
 
+        """
+        return set(headers_1) - set(headers_2)
 
     def set_dataframe_by_url(
-        self, manifest_url: str, manifest_df: pd.DataFrame
+        self, manifest_url: str, manifest_df: pd.DataFrame, out_of_schema_columns: set =None,
     ) -> ps.Spreadsheet:
         """Update Google Sheets using given pandas DataFrame.
         Args:
             manifest_url (str): Google Sheets URL.
             manifest_df (pd.DataFrame): Data frame to "upload".
+            out_of_schema_columns (set): Columns that are in downloaded manifest, but not in current schema.
         Returns:
             ps.Spreadsheet: A Google Sheet object.
         """
 
         # authorize pygsheets to read from the given URL
         gc = ps.authorize(custom_credentials=self.creds)
 
         # open google sheets and extract first sheet
+        # This sheet already contains headers.
         sh = gc.open_by_url(manifest_url)
         wb = sh[0]
 
-        # Handle scenario when existing manifest does not match new
-        #       manifest template due to changes in the data model:
-        #
-        # the sheet column header reflect the latest schema
-        # the existing manifest column-set may be outdated
-        # ensure that, if missing, attributes from the latest schema are added to the
-        # column-set of the existing manifest so that the user can modify their data if needed
-        # to comply with the latest schema
-
-        # get headers from existing manifest and sheet 
-        wb_header = wb.get_row(1)
-        manifest_df_header = manifest_df.columns
-
-        # find missing columns in existing manifest
-        new_columns = set(wb_header) - set(manifest_df_header)
-
-        # clean empty columns if any are present (there should be none)
-        # TODO: Remove this line once we start preventing empty column names
-        if '' in new_columns:
-            new_columns = new_columns.remove('')
-
-        # find missing columns present in existing manifest but missing in latest schema
-        out_of_schema_columns = set(manifest_df_header) - set(wb_header)
-
-        # update existing manifest w/ missing columns, if any
-        if new_columns:
-            manifest_df = manifest_df.assign(
-                **dict(zip(new_columns, len(new_columns) * [""]))
-            )
-
-        # sort columns in the updated manifest:
-        # match latest schema order
-        # move obsolete columns at the end
-        manifest_df = manifest_df[self.sort_manifest_fields(manifest_df.columns)]
-        manifest_df = manifest_df[[c for c in manifest_df if c not in out_of_schema_columns] + list(out_of_schema_columns)]
-    
-        # The following line sets `valueInputOption = "RAW"` in pygsheets
-        sh.default_parse = False
-
-        # update spreadsheet with given manifest starting at top-left cell
         wb.set_dataframe(manifest_df, (1, 1))
 
         # update validation rules (i.e. no validation rules) for out of schema columns, if any
         # TODO: similarly clear formatting for out of schema columns, if any
-        num_out_of_schema_columns = len(out_of_schema_columns)
-        if num_out_of_schema_columns > 0: 
+        if out_of_schema_columns:
+            num_out_of_schema_columns = len(out_of_schema_columns)
             start_col = self._column_to_letter(len(manifest_df.columns) - num_out_of_schema_columns) # find start of out of schema columns
             end_col = self._column_to_letter(len(manifest_df.columns) + 1) # find end of out of schema columns
-       
             wb.set_data_validation(start = start_col, end = end_col, condition_type = None)
-
         # set permissions so that anyone with the link can edit
         sh.share("", role="writer", type="anyone")
 
         return sh
 
     def get_dataframe_by_url(self, manifest_url: str) -> pd.DataFrame:
         """Retrieve pandas DataFrame from table in Google Sheets.
@@ -1453,71 +1418,74 @@
         # trigger a warning if file path is provided but does not exist
         elif output_location and not os.path.exists(output_location):
             output_excel_file_path = os.path.abspath(os.path.join(os.getcwd(), file_name))
             logger.warning(f'{output_location} does not exist. Using current working directory {output_excel_file_path}')
         # otherwise, use the default location
         else:
             output_excel_file_path = os.path.abspath(os.path.join(os.getcwd(), file_name))
+        
         # export the manifest to excel
         export_manifest_drive_service(manifest_url, file_path=output_excel_file_path, mimeType = 'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet')
         
         return output_excel_file_path
 
-    def _handle_output_format_logic(self, output_format: str = None, output_path: str = None, sheet_url: bool = None, manifest_url: str = None, empty_manifest_url: str = None, dataframe: pd.DataFrame = None):
+    def _handle_output_format_logic(self, output_format: str = None, output_path: str = None, sheet_url: bool = None, empty_manifest_url: str = None, dataframe: pd.DataFrame = None, out_of_schema_columns: set =None):
         """
-        handle the logic between sheet_url parameter and output_format parameter to determine the type of output to return
+        Handle the logic between sheet_url parameter and output_format parameter to determine the type of output to return
         Args: 
             output_format: Determines if Google sheet URL, pandas dataframe, or Excel spreadsheet gets returned.
             sheet_url (Will be deprecated): a boolean ; determine if a pandas dataframe or a google sheet url gets return
-            manifest_url: Google sheet URL populated with metadata
             empty_manifest_url: Google sheet URL that leads to an empty manifest 
             dataframe: the pandas dataframe that contains the metadata that needs to be populated to an empty manifest
             output_path: Determines the output path of the exported manifest (only relevant if returning an excel spreadsheet)
-        return: a pandas dataframe, file path of an excel spreadsheet, or a google sheet URL 
+            out_of_schema_columns (set): Columns that are in downloaded manifest, but not in current schema.
+        Return: 
+            a pandas dataframe, file path of an excel spreadsheet, or a google sheet URL 
+        TODO:
+            Depreciate sheet URL and add google_sheet as an output_format choice.
         """
 
-        # check if output_format parameter gets set. If not, check the sheet_url parameter
-        if not output_format: 
-            # if the sheet_url parameter gets set to True, return a google sheet url 
-            if sheet_url: 
-                return manifest_url
-                # else, return a pandas dataframe
-            else: 
-                return dataframe
-        else:
-            # if the output type gets set to "dataframe", return a data frame 
-            if output_format == "dataframe":
-                return dataframe
-            # if the output type gets set to "excel", return an excel spreadsheet
-            elif output_format == "excel":                 
-                # export the manifest url to excel
-                output_file_path = self.export_sheet_to_excel(title = self.title, manifest_url = empty_manifest_url, output_location = output_path)
-
-                if not os.path.exists(output_file_path): 
-                    logger.error(f'Export to Excel spreadsheet fail. Please make sure that file path {output_file_path} is valid')
+        # if the output type gets set to "dataframe", return a data frame 
+        if output_format == "dataframe":
+            return dataframe
+        
+        # if the output type gets set to "excel", return an excel spreadsheet
+        elif output_format == "excel":              
+            # export manifest url that only contains column headers to Excel
+            output_file_path = self.export_sheet_to_excel(title = self.title,
+                                                          manifest_url = empty_manifest_url,
+                                                          output_location = output_path,
+                                                          )
 
-                # populate an excel spreadsheet with the existing dataframe
-                self.populate_existing_excel_spreadsheet(output_file_path, dataframe)
+            # populate an excel spreadsheet with the existing dataframe
+            self.populate_existing_excel_spreadsheet(output_file_path, dataframe)
 
-                return output_file_path
-            # for all other cases, return a google sheet url 
-            else: 
-                return manifest_url  
+            return output_file_path
+        
+        # Return google sheet if sheet_url flag is raised.
+        elif sheet_url: 
+            manifest_sh = self.set_dataframe_by_url(manifest_url=empty_manifest_url, manifest_df=dataframe, out_of_schema_columns=out_of_schema_columns)
+            return manifest_sh.url
+        
+        # Default return a DataFrame
+        else:
+            return dataframe
 
     def get_manifest(
-        self, dataset_id: str = None, sheet_url: bool = None, json_schema: str = None, output_format: str = None, output_path: str = None
+        self, dataset_id: str = None, sheet_url: bool = None, json_schema: str = None, output_format: str = None, output_path: str = None, access_token: str = None
     ) -> Union[str, pd.DataFrame]:
         """Gets manifest for a given dataset on Synapse.
            TODO: move this function to class MetadatModel (after MetadataModel is refactored)
 
         Args:
             dataset_id: Synapse ID of the "dataset" entity on Synapse (for a given center/project).
             sheet_url: Determines if googlesheet URL or pandas dataframe should be returned.
             output_format: Determines if Google sheet URL, pandas dataframe, or Excel spreadsheet gets returned.
             output_path: Determines the output path of the exported manifest
+            access_token: Token in .synapseConfig. Since we could not pre-load access_token as an environment variable on AWS, we have to add this variable. 
 
         Returns:
             Googlesheet URL, pandas dataframe, or an Excel spreadsheet 
         """
 
         # Handle case when no dataset ID is provided
         if not dataset_id:
@@ -1531,97 +1499,181 @@
             else: 
                 return manifest_url
 
         # Otherwise, create manifest using the given dataset
         #TODO: avoid explicitly exposing Synapse store functionality
         # just instantiate a Store class and let it decide at runtime/config
         # the store type
-
-        store = SynapseStorage()
+        if access_token: 
+            # for getting an existing manifest on AWS
+            store = SynapseStorage(access_token=access_token)
+        else: 
+            store = SynapseStorage()
 
         # Get manifest file associated with given dataset (if applicable)
         # populate manifest with set of new files (if applicable)
         manifest_record = store.updateDatasetManifestFiles(self.sg, datasetId = dataset_id, store = False)
 
         # get URL of an empty manifest file created based on schema component
         empty_manifest_url = self.get_empty_manifest()
 
         # Populate empty template with existing manifest
         if manifest_record:
-
             # TODO: Update or remove the warning in self.__init__() if
             # you change the behavior here based on self.use_annotations
-                            
-            # populate empty manifest with content from downloaded/existing manifest
-            manifest_sh = self.set_dataframe_by_url(empty_manifest_url, manifest_record[1])
+
+            # Update df with existing manifest. Agnostic to output format
+            updated_df, out_of_schema_columns = self._update_dataframe_with_existing_df(empty_manifest_url=empty_manifest_url, existing_df=manifest_record[1])
 
             # determine the format of manifest
-            result = self._handle_output_format_logic(output_format = output_format, output_path = output_path, sheet_url = sheet_url, manifest_url = manifest_sh.url, empty_manifest_url=empty_manifest_url, dataframe = manifest_record[1])
+            result = self._handle_output_format_logic(output_format = output_format,
+                                                      output_path = output_path,
+                                                      sheet_url = sheet_url,
+                                                      empty_manifest_url=empty_manifest_url,
+                                                      dataframe = updated_df,
+                                                      out_of_schema_columns=out_of_schema_columns,
+                                                      )
             return result
 
         # Generate empty template and optionally fill in with annotations
         else:
             # Using getDatasetAnnotations() to retrieve file names and subset
             # entities to files and folders (ignoring tables/views)
+
             annotations = pd.DataFrame()
             if self.is_file_based:
                 annotations = store.getDatasetAnnotations(dataset_id)
 
             # if there are no files with annotations just generate an empty manifest
             if annotations.empty:
-                manifest_url = self.get_empty_manifest() 
+                manifest_url = self.get_empty_manifest()
                 manifest_df = self.get_dataframe_by_url(manifest_url)
             else:
                 # Subset columns if no interested in user-defined annotations and there are files present
                 if self.is_file_based and not self.use_annotations:
                     annotations = annotations[["Filename", "eTag", "entityId"]]
 
                 # Update `additional_metadata` and generate manifest
                 manifest_url, manifest_df = self.get_manifest_with_annotations(annotations)
             
+            # Update df with existing manifest. Agnostic to output format
+            updated_df, out_of_schema_columns = self._update_dataframe_with_existing_df(empty_manifest_url=empty_manifest_url, existing_df=manifest_df)
+
             # determine the format of manifest that gets return 
-            result = self._handle_output_format_logic(output_format = output_format, output_path = output_path, sheet_url = sheet_url, manifest_url = manifest_url, empty_manifest_url=empty_manifest_url, dataframe = manifest_df)
+            result = self._handle_output_format_logic(output_format = output_format,
+                                                      output_path = output_path,
+                                                      sheet_url = sheet_url,
+                                                      empty_manifest_url=empty_manifest_url,
+                                                      dataframe = manifest_df,
+                                                      )
             return result
 
+    def _update_dataframe_with_existing_df(self, empty_manifest_url: str, existing_df: pd.DataFrame) -> pd.DataFrame:
+        """
+        Handle scenario when existing manifest does not match new manifest template due to changes in the data model:
+            the sheet column header reflect the latest schema the existing manifest column-set may be outdated
+            ensure that, if missing, attributes from the latest schema are added to the column-set of the existing manifest so that the user can modify their data if needed
+            to comply with the latest schema.
+        Args:
+            empty_manifest_url (str): Google Sheet URL with an empty manifest with headers.
+            existing_df (Pd.DataFrame): df of an existing manifest
+
+        Returns:
+            updated_df (Pd.DataFrame): existing_df with new_columns added.
+            out_of_schema_columns (set): Columns that are in downloaded manifest, but not in current schema.
+        """
+
+        # Get headers for the current schema and existing manifest df.
+        current_schema_headers = list(self.get_dataframe_by_url(empty_manifest_url).columns)
+        existing_manfiest_headers = list(existing_df.columns)
+
+        # Find columns that exist in the current schema, but are not in the manifest being downloaded.
+        new_columns = self._get_missing_columns(current_schema_headers, existing_manfiest_headers)
+
+        # Find columns that exist in the manifest being downloaded, but not in the current schema.
+        out_of_schema_columns = self._get_missing_columns(existing_manfiest_headers, current_schema_headers)
+
+        # clean empty columns if any are present (there should be none)
+        # TODO: Remove this line once we start preventing empty column names
+        if '' in new_columns:
+            new_columns = new_columns.remove('')
+
+        # Copy the df for updating.
+        updated_df = existing_df.copy(deep=True)
+        
+        # update existing manifest w/ missing columns, if any
+        if new_columns:
+            updated_df = updated_df.assign(
+                **dict(zip(new_columns, len(new_columns) * [""]))
+            )
+
+        # sort columns in the updated manifest:
+        # match latest schema order
+        # move obsolete columns at the end
+        updated_df = updated_df[self.sort_manifest_fields(updated_df.columns)]
+        updated_df = updated_df[[c for c in updated_df if c not in out_of_schema_columns] + list(out_of_schema_columns)]
+
+        return updated_df, out_of_schema_columns
+
+    def _format_new_excel_column(self, worksheet, new_column_index: int, col: str):
+        """Add new column to an openpyxl worksheet and format header.
+        Args:
+            worksheet: openpyxl worksheet
+            new_column_index, int: index to add new column
+        Return:
+            modified worksheet
+        """
+        # Add column header
+        worksheet.cell(row=1, column=new_column_index+1).value = col
+        # Format new column header 
+        worksheet.cell(row=1, column=new_column_index+1).font = Font(size=8, bold=True, color="FF000000")
+        worksheet.cell(row=1, column=new_column_index+1).alignment = Alignment(horizontal="center", vertical="bottom")
+        worksheet.cell(row=1, column=new_column_index+1).fill = PatternFill(start_color='FFE0E0E0', end_color='FFE0E0E0', fill_type='solid')
+        return worksheet
+
     def populate_existing_excel_spreadsheet(self, existing_excel_path: str = None, additional_df: pd.DataFrame = None):
         '''Populate an existing excel spreadsheet by using an additional dataframe (to avoid sending metadata directly to Google APIs)
+        New columns will be placed at the end of the spreadsheet.
         Args:
             existing_excel_path: path of an existing excel spreadsheet
             additional_df: additional dataframe
+        Return: 
+            added new dataframe to the existing excel path.
+        Note:
+            - Done by rows and column as a way to preserve formatting. 
+            Doing a complete replacement will remove all conditional formatting and dropdowns.
         '''
         # load workbook
         workbook = load_workbook(existing_excel_path)
+        worksheet = workbook.active
 
-        #get missing columns and sort manifest 
-        #get existing headers
-        existing_df = pd.read_excel(existing_excel_path, sheet_name="Sheet1")
-        workbook_headers = existing_df.columns
-
-        # get new column headers
-        out_of_schema_columns = self._get_missing_columns(workbook_headers, additional_df)
-        out_of_schema_columns_lst = list(out_of_schema_columns)
-        
-        # initalize excel writer
-        writer = pd.ExcelWriter(existing_excel_path, engine='openpyxl')
-        writer.book = workbook
-        writer.sheets = {ws.title: ws for ws in workbook.worksheets}
-        worksheet = writer.sheets["Sheet1"]
-
-        # add additional content to the existing spreadsheet
-        additional_df.to_excel(writer, sheet_name = "Sheet1", startrow=1, index = False, header=False)
-
-        # if there are new columns, add them to the end of spreadsheet
-        if len(out_of_schema_columns_lst) > 0:
-            for i, col_name in enumerate(out_of_schema_columns_lst):
-                col_index = len(workbook_headers) + 1 + i
-                worksheet.cell(row=1, column=col_index).value = col_name
-        
-        # save and close
-        writer.save()
-        writer.close()
+        # Add new data to existing excel
+        if not additional_df.empty:
+            existing_excel_headers = [cell.value for cell in worksheet[1] if cell.value != None]
+
+            new_column_index = len(existing_excel_headers)
+            df_columns = additional_df.columns
+
+            # Iteratively fill workbook with contents of additional_df
+            for row_num, row_contents in enumerate(dataframe_to_rows(additional_df, index=False, header=False), 2):
+                for index, col in enumerate(df_columns):
+                    if col in existing_excel_headers:
+                        # Get index of column header in existing excel to ensure no values are placed in incorrect spot.
+                        existing_column_index = existing_excel_headers.index(col)
+                        worksheet.cell(row=row_num, column=existing_column_index+1).value = row_contents[index]
+                    else:
+                        # Add new col to excel worksheet and format.
+                        worksheet = self._format_new_excel_column(worksheet=worksheet, new_column_index=new_column_index, col=col)
+                        # Add data to column
+                        worksheet.cell(row=row_num, column=new_column_index+1).value = row_contents[index]
+                        # Add new column to headers so it can be accounted for.
+                        existing_excel_headers.append(col)
+                        # Update index for adding new columns.
+                        new_column_index+=1                   
+        workbook.save(existing_excel_path)
 
     def populate_manifest_spreadsheet(self, existing_manifest_path: str = None, empty_manifest_url: str = None, return_excel: bool = False, title: str = None):
         """Creates a google sheet manifest based on existing manifest.
         Args:
             existing_manifest_path: the location of the manifest containing metadata presently stored
             empty_manifest_url: the path to a manifest template to be prepopulated with existing's manifest metadata
             return_excel: if true, return an Excel spreadsheet instead of Google sheet
@@ -1634,14 +1686,15 @@
         if return_excel: 
             '''if we are returning an Excel spreadsheet, do not populate dataframe to google'''
             # get an empty manifest 
             manifest_url = empty_manifest_url
 
             # export the manifest to excel
             output_excel_file_path = self.export_sheet_to_excel(manifest_url = manifest_url, title=title)
+            
             # populate exported sheet 
             self.populate_existing_excel_spreadsheet(output_excel_file_path, manifest)
             return output_excel_file_path
         else: 
             manifest_sh = self.set_dataframe_by_url(empty_manifest_url, manifest)
             return manifest_sh.url
```

### Comparing `schematicpy-23.1.1/schematic/models/GE_Helpers.py` & `schematicpy-23.6.1/schematic/models/GE_Helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,18 +17,20 @@
 from ruamel import yaml
 
 import great_expectations as ge
 from great_expectations.core.expectation_configuration import ExpectationConfiguration
 from great_expectations.data_context import BaseDataContext
 from great_expectations.data_context.types.base import DataContextConfig, DatasourceConfig, FilesystemStoreBackendDefaults
 from great_expectations.data_context.types.resource_identifiers import ExpectationSuiteIdentifier
+from great_expectations.exceptions.exceptions import GreatExpectationsError
+
 
 from schematic.models.validate_attribute import GenerateError
 from schematic.schemas.generator import SchemaGenerator
-from schematic.utils.validate_utils import rule_in_rule_list
+from schematic.utils.validate_utils import rule_in_rule_list, np_array_to_str_list, iterable_to_str_list
 
 logger = logging.getLogger(__name__)
 
 class GreatExpectationsHelpers(object):
     """
         Great Expectations helper class
 
@@ -123,19 +125,21 @@
             
         """
         validation_expectation = {
             "int": "expect_column_values_to_be_in_type_list",
             "float": "expect_column_values_to_be_in_type_list",
             "str": "expect_column_values_to_be_of_type",
             "num": "expect_column_values_to_be_in_type_list",
+            "date": "expect_column_values_to_be_dateutil_parseable",
             "recommended": "expect_column_values_to_not_match_regex_list",
             "protectAges": "expect_column_values_to_be_between",
             "unique": "expect_column_values_to_be_unique",
             "inRange": "expect_column_values_to_be_between",
-            
+            "IsNA": "expect_column_values_to_match_regex_list",
+
             # To be implemented rules with possible expectations
             #"list": "expect_column_values_to_not_match_regex_list",
             #"regex": "expect_column_values_to_match_regex",
             #"url": "expect_column_values_to_be_valid_urls",
             #"matchAtLeastOne": "expect_foreign_keys_in_column_a_to_exist_in_column_b",
             #"matchExactlyOne": "expect_foreign_keys_in_column_a_to_exist_in_column_b",
         }
@@ -214,14 +218,29 @@
                         meta={
                             "notes": {
                                 "format": "markdown",
                                 "content": "Expect column values to be of string type. **Markdown** `Supported`",
                             },
                             "validation_rule": rule
                         }
+
+                    #Validate date
+                    elif base_rule=='date':
+                        args["mostly"]=1.0
+                        meta={
+                            "notes": {
+                                "format": "markdown",
+                                "content": (
+                                    "Expect column values to be parsable by dateutils. "
+                                    "**Markdown** `Supported`"
+                                ),
+                            },
+                            "validation_rule": rule
+                        }
+
                     elif base_rule==("recommended"):
                         args["mostly"]=0.0000000001
                         args["regex_list"]=['^$']
                         meta={
                             "notes": {
                                 "format": "markdown",
                                 "content": "Expect column to not be empty. **Markdown** `Supported`",
@@ -232,14 +251,15 @@
                     elif base_rule==("protectAges"):
                         #Function to convert to different age limit formats
                         min_age, max_age = self.get_age_limits()
 
                         args["mostly"]=1.0
                         args["min_value"]=min_age
                         args["max_value"]=max_age
+                        #args['allow_cross_type_comparisons']=True # TODO Can allow after issue #980 is completed
                         meta={
                             "notes": {
                                 "format": "markdown",
                                 "content": "Expect ages to be between 18 years (6,570 days) and 90 years (32,850 days) of age. **Markdown** `Supported`",
                             },
                             "validation_rule": rule
                         }
@@ -252,20 +272,32 @@
                                 "content": "Expect column values to be Unique. **Markdown** `Supported`",
                             },
                             "validation_rule": rule
                         }
                     
                     elif base_rule==("inRange"):
                         args["mostly"]=1.0
-                        args["min_value"]=float(rule.split(" ")[1])
-                        args["max_value"]=float(rule.split(" ")[2])
+                        args["min_value"]=float(rule.split(" ")[1]) if rule.split(" ")[1].lower() != 'none' else None
+                        args["max_value"]=float(rule.split(" ")[2]) if rule.split(" ")[2].lower() != 'none' else None
+                        args['allow_cross_type_comparisons']=True # TODO Should follow up with issue #980
                         meta={
                             "notes": {
                                 "format": "markdown",
-                                "content": "Expect column values to be Unique. **Markdown** `Supported`",
+                                "content": "Expect column values to be within a specified range. **Markdown** `Supported`",
+                            },
+                            "validation_rule": rule
+                        }
+                        
+                    elif base_rule==("IsNA"):
+                        args["mostly"]=1.0
+                        args["regex_list"]=['Not Applicable']
+                        meta={
+                            "notes": {
+                                "format": "markdown",
+                                "content": "Expect column values to be marked Not Applicable. **Markdown** `Supported`",
                             },
                             "validation_rule": rule
                         }
                                         
                     #add expectation for attribute to suite        
                     self.add_expectation(
                         rule=rule,
@@ -322,17 +354,17 @@
             Purpose:
                 Build checkpoint to validate manifest
             Input:
             Returns:
                 adds checkpoint to self 
         """
         #create manifest checkpoint
-        checkpoint_name = "manifest_checkpoint"  
+        self.checkpoint_name = "manifest_checkpoint"  
         checkpoint_config={
-            "name": checkpoint_name,
+            "name": self.checkpoint_name,
             "config_version": 1,
             "class_name": "SimpleCheckpoint",
             "validations": [
                 {
                     "batch_request": {
                         "datasource_name": "example_datasource",
                         "data_connector_name": "default_runtime_data_connector_name",
@@ -388,16 +420,19 @@
             
             #if the expectaion failed, get infromation to generate error message
             if not result_dict['success']:
                 errColumn   = result_dict['expectation_config']['kwargs']['column']               
                 rule        = result_dict['expectation_config']['meta']['validation_rule']
 
 
+                if 'exception_info' in result_dict.keys() and result_dict['exception_info']['exception_message']:
+                    raise GreatExpectationsError(result_dict['exception_info']['exception_traceback'])
+                
                 #only some expectations explicitly list unexpected values and indices, read or find if not present
-                if 'unexpected_index_list' in result_dict['result']:
+                elif 'unexpected_index_list' in result_dict['result']:
                     indices = result_dict['result']['unexpected_index_list']
                     values  = result_dict['result']['unexpected_list']
 
                 # Technically, this shouldn't ever happen, but will keep as a failsafe in case many things go wrong
                 # because type validation is column aggregate expectation and not column map expectation when columns are not of object type, 
                 # indices and values cannot be returned
                 else:
@@ -407,57 +442,57 @@
                         values.append(item) if isinstance(item,type_dict[observed_type]) else values
 
                 #call functions to generate error messages and add to error list
                 if validation_types[rule.split(" ")[0]]['type']=='type_validation':
                     for row, value in zip(indices,values):
                         vr_errors, vr_warnings = GenerateError.generate_type_error(
                                 val_rule = rule,
-                                row_num = row+2,
+                                row_num = str(row+2),
                                 attribute_name = errColumn,
-                                invalid_entry = value,
+                                invalid_entry = str(value),
                                 sg = sg,
                             )
                         if vr_errors:
                             errors.append(vr_errors)  
                         if vr_warnings:
                             warnings.append(vr_warnings) 
                 elif validation_types[rule.split(" ")[0]]['type']=='regex_validation':
                     expression=result_dict['expectation_config']['kwargs']['regex']
                     for row, value in zip(indices,values):   
                         vr_errors, vr_warnings = GenerateError.generate_regex_error(
                                 val_rule= rule,
                                 reg_expression = expression,
-                                row_num = row+2,
+                                row_num = str(row+2),
                                 module_to_call = 'match',
                                 attribute_name = errColumn,
                                 invalid_entry = value,
                                 sg = sg,
                             )
                         if vr_errors:
                             errors.append(vr_errors)  
                         if vr_warnings:
                             warnings.append(vr_warnings)                          
                 elif validation_types[rule.split(" ")[0]]['type']=='content_validation':     
                     vr_errors, vr_warnings = GenerateError.generate_content_error(
                                                             val_rule = rule, 
                                                             attribute_name = errColumn,
-                                                            row_num = list(np.array(indices)+2),
-                                                            error_val = values,  
+                                                            row_num = np_array_to_str_list(np.array(indices)+2),
+                                                            error_val = iterable_to_str_list(values),  
                                                             sg = self.sg
                                                         )       
                     if vr_errors:
                         errors.append(vr_errors)  
                         if rule.startswith('protectAges'):
                             self.censor_ages(vr_errors,errColumn)
-                            pass
+                            
                     if vr_warnings:
                         warnings.append(vr_warnings)  
                         if rule.startswith('protectAges'):
                             self.censor_ages(vr_warnings,errColumn)
-                            pass
+                            
 
         return errors, warnings
 
     def get_age_limits(
         self,
         ):
         """
@@ -488,18 +523,21 @@
             Input:
                 message: 
                     error or warning message for age validation rule
                 col:
                     name of column containing ages
             Returns:
                 updates self.manifest with censored ages
-            
+            TODO: Speed up conversion from str list to int list
         """
+        censor_rows = []
         
-        censor_rows = list(np.array(message[0]) - 2) 
+        for row in message[0]:
+            censor_rows.append(int(row) - 2)
+
         self.manifest.loc[censor_rows,(col)] = 'age censored'
 
         # update the manifest file, so that ages are censored
         self.manifest.to_csv(self.manifestPath.replace('.csv','_censored.csv'), index=False)
         logging.info("Sensitive ages have been censored.")
 
         return
```

### Comparing `schematicpy-23.1.1/schematic/models/commands.py` & `schematicpy-23.6.1/schematic/models/commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python3
 
 from gc import callbacks
 import logging
 import sys
+from time import perf_counter
 
 import click
 import click_log
 
 from jsonschema import ValidationError
 
 from schematic.models.metadata import MetadataModel
 from schematic.utils.cli_utils import get_from_config, fill_in_from_config, query_dict, parse_synIDs, parse_comma_str_to_list
 from schematic.help import model_commands
 from schematic.exceptions import MissingConfigValueError
 from schematic import CONFIG
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger('schematic')
 click_log.basic_config(logger)
 
 CONTEXT_SETTINGS = dict(help_option_names=["--help", "-h"])  # help options
 
 # invoke_without_command=True -> forces the application not to show aids before losing them with a --h
 @click.group(context_settings=CONTEXT_SETTINGS, invoke_without_command=True)
 @click_log.simple_verbosity_option(logger)
@@ -75,85 +76,70 @@
     "-hb",
     is_flag=True,
     help=query_dict(model_commands,("model","submit","hide_blanks")),
 )
 @click.option(
     "--manifest_record_type",
     "-mrt",
-    default='both',
-    type=click.Choice(['table', 'entity', 'both'], case_sensitive=True),
+    default='table_file_and_entities',
+    type=click.Choice(['table_and_file', 'file_only', 'file_and_entities', 'table_file_and_entities'], case_sensitive=True),
     help=query_dict(model_commands, ("model", "submit", "manifest_record_type")))
 @click.option(
     "-rr",
     "--restrict_rules",
     is_flag=True,
     help=query_dict(model_commands,("model","validate","restrict_rules")),
 )
 @click.option(
     "-ps",
     "--project_scope",
     default=None,
     callback=parse_synIDs,
     help=query_dict(model_commands, ("model", "validate", "project_scope")),
 )
+@click.option(
+    "--table_manipulation",
+    "-tm",
+    default='replace',
+    type=click.Choice(['replace', 'upsert'], case_sensitive=True),
+    help=query_dict(model_commands, ("model", "submit", "table_manipulation")))
 @click.pass_obj
 def submit_manifest(
-    ctx, manifest_path, dataset_id, validate_component, manifest_record_type, use_schema_label, hide_blanks, restrict_rules, project_scope,
+    ctx, manifest_path, dataset_id, validate_component, manifest_record_type, use_schema_label, hide_blanks, restrict_rules, project_scope, table_manipulation,
 ):
     """
     Running CLI with manifest validation (optional) and submission options.
     """
-
+    
     jsonld = get_from_config(CONFIG.DATA, ("model", "input", "location"))
 
     model_file_type = get_from_config(CONFIG.DATA, ("model", "input", "file_type"))
 
     metadata_model = MetadataModel(
         inputMModelLocation=jsonld, inputMModelLocationType=model_file_type
     )
 
-    try:
-        manifest_id = metadata_model.submit_metadata_manifest(
-            path_to_json_ld = jsonld,
-            manifest_path=manifest_path,
-            dataset_id=dataset_id,
-            validate_component=validate_component,
-            manifest_record_type=manifest_record_type,
-            restrict_rules=restrict_rules,
-            use_schema_label=use_schema_label,
-            hide_blanks=hide_blanks,
-            project_scope=project_scope,
-        )
 
-        '''
-        if censored_manifest_id:
-            logger.info(
-                f"File at '{manifest_path}' was censored and successfully associated "
-                f"with dataset '{dataset_id}'. "
-                f"An uncensored version has also been associated with dataset '{dataset_id}' "
-                f"and submitted to the Synapse Access Control Team to begin the process "
-                f"of adding terms of use or review board approval."
-            )
-        '''
-        if manifest_id:
-            logger.info(
-                f"File at '{manifest_path}' was successfully associated "
-                f"with dataset '{dataset_id}'."
-            )
-    except ValueError:
-        logger.error(
-            f"Component '{validate_component}' is not present in '{jsonld}', or is invalid."
-        )
-    except ValidationError:
-        logger.error(
-            f"Validation errors resulted while validating with '{validate_component}'."
-        )
-    except LookupError:
-        logger.error(
-            f"'{dataset_id}' could not be found in the asset view (or file view for Synapse user)"
+    manifest_id = metadata_model.submit_metadata_manifest(
+        path_to_json_ld = jsonld,
+        manifest_path=manifest_path,
+        dataset_id=dataset_id,
+        validate_component=validate_component,
+        manifest_record_type=manifest_record_type,
+        restrict_rules=restrict_rules,
+        use_schema_label=use_schema_label,
+        hide_blanks=hide_blanks,
+        project_scope=project_scope,
+        table_manipulation=table_manipulation,
+    )
+    
+    if manifest_id:
+        logger.info(
+            f"File at '{manifest_path}' was successfully associated "
+            f"with dataset '{dataset_id}'."
         )
 
 
 # prototype based on validateModelManifest()
 @model.command(
     "validate",
     short_help=query_dict(model_commands, ("model", "validate", "short_help")),
@@ -191,15 +177,16 @@
     help=query_dict(model_commands, ("model", "validate", "project_scope")),
 )
 @click.pass_obj
 def validate_manifest(ctx, manifest_path, data_type, json_schema, restrict_rules,project_scope):
     """
     Running CLI for manifest validation.
     """
-    data_type = fill_in_from_config("data_type", data_type, ("manifest", "data_type"))
+    if not data_type:
+        data_type = fill_in_from_config("data_type", data_type, ("manifest", "data_type"))
     
     try:
         len(data_type) == 1
     except:
         logger.error(
             f"Can only validate a single data_type at a time. Please provide a single data_type"
         )
@@ -208,15 +195,15 @@
 
     json_schema = fill_in_from_config(
         "json_schema",
         json_schema,
         ("model", "input", "validation_schema"),
         allow_none=True,
     )
-    
+    t_validate = perf_counter()
     jsonld = get_from_config(CONFIG.DATA, ("model", "input", "location"))
 
     model_file_type = get_from_config(CONFIG.DATA, ("model", "input", "file_type"))
 
     metadata_model = MetadataModel(
         inputMModelLocation=jsonld, inputMModelLocationType=model_file_type
     )
@@ -229,7 +216,11 @@
         click.echo(
             "Your manifest has been validated successfully. "
             "There are no errors in your manifest, and it can "
             "be submitted without any modifications."
         )
     else:
         click.echo(errors)
+
+    logger.debug(
+        f"Total elapsed time {perf_counter()-t_validate} seconds"
+    )
```

### Comparing `schematicpy-23.1.1/schematic/models/metadata.py` & `schematicpy-23.6.1/schematic/models/metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -282,16 +282,17 @@
         path_to_json_ld: str,
         dataset_id: str,
         manifest_record_type: str,
         restrict_rules: bool,
         validate_component: str = None,
         use_schema_label: bool = True,
         hide_blanks: bool = False,
-        input_token: str = None,
+        access_token: str = None,
         project_scope: List = None,
+        table_manipulation: str = 'replace'
     ) -> string:
         """Wrap methods that are responsible for validation of manifests for a given component, and association of the
         same manifest file with a specified dataset.
         Args:
             manifest_path: Path to the manifest file, which contains the metadata.
             dataset_id: Synapse ID of the dataset on Synapse containing the metadata manifest file.
             validate_component: Component from the schema.org schema based on which the manifest template has been generated.
@@ -301,15 +302,15 @@
             ValueError: When validate_component is provided, but it cannot be found in the schema.
             ValidationError: If validation against data model was not successful.
         """
 
         #TODO: avoid explicitly exposing Synapse store functionality
         # just instantiate a Store class and let it decide at runtime/config
         # the store type
-        syn_store = SynapseStorage(input_token = input_token, project_scope = project_scope)
+        syn_store = SynapseStorage(access_token = access_token, project_scope = project_scope)
         manifest_id=None
         censored_manifest_id=None
         restrict_maniest=False
         censored_manifest_path=manifest_path.replace('.csv','_censored.csv')
         # check if user wants to perform validation or not
         if validate_component is not None:
 
@@ -337,25 +338,27 @@
                     censored_manifest_id = syn_store.associateMetadataWithFiles(
                         schemaGenerator = self.sg,
                         metadataManifestPath = censored_manifest_path,
                         datasetId = dataset_id, 
                         manifest_record_type = manifest_record_type,
                         useSchemaLabel = use_schema_label,
                         hideBlanks = hide_blanks,
+                        table_manipulation=table_manipulation,
                     )
                     restrict_maniest = True
                 
                 manifest_id = syn_store.associateMetadataWithFiles(
                     schemaGenerator = self.sg,
                     metadataManifestPath = manifest_path, 
                     datasetId = dataset_id, 
                     manifest_record_type = manifest_record_type,
                     useSchemaLabel = use_schema_label, 
                     hideBlanks = hide_blanks,
                     restrict_manifest=restrict_maniest,
+                    table_manipulation=table_manipulation,
                 )
 
                 logger.info(f"No validation errors occured during validation.")
                 return manifest_id
                 
             else:
                 raise ValidationError(
@@ -368,25 +371,27 @@
             censored_manifest_id = syn_store.associateMetadataWithFiles(
                 schemaGenerator = self.sg,
                 metadataManifestPath=censored_manifest_path,
                 datasetId=dataset_id,
                 manifest_record_type=manifest_record_type,
                 useSchemaLabel=use_schema_label,
                 hideBlanks=hide_blanks,
+                table_manipulation=table_manipulation,
             )
             restrict_maniest = True
         
         manifest_id = syn_store.associateMetadataWithFiles(
             schemaGenerator = self.sg,
             metadataManifestPath=manifest_path,
             datasetId=dataset_id,
             manifest_record_type=manifest_record_type,
             useSchemaLabel=use_schema_label,
             hideBlanks=hide_blanks,
             restrict_manifest=restrict_maniest,
+            table_manipulation=table_manipulation,
         )
 
         logger.debug(
             "Optional validation was not performed on manifest before association."
         )
 
         return manifest_id
```

### Comparing `schematicpy-23.1.1/schematic/models/validate_attribute.py` & `schematicpy-23.6.1/schematic/models/validate_attribute.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import builtins
 import logging
 import re
 import sys
 import time
+from time import perf_counter
 from os import getenv
 # allows specifying explicit variable types
 from typing import Any, Dict, List, Optional, Text
 from urllib import error
 from urllib.parse import urlparse
 from urllib.request import (HTTPDefaultErrorHandler, OpenerDirector, Request,
                             urlopen)
@@ -16,15 +17,20 @@
 from jsonschema import ValidationError
 
 from schematic.schemas.generator import SchemaGenerator
 from schematic.store.base import BaseStorage
 from schematic.store.synapse import SynapseStorage
 from schematic.utils.validate_rules_utils import validation_rule_info
 from schematic.utils.validate_utils import (comma_separated_list_regex,
-                                            parse_str_series_to_list)
+                                            parse_str_series_to_list,
+                                            np_array_to_str_list,
+                                            iterable_to_str_list,
+                                            rule_in_rule_list,
+                                            )
+
 
 logger = logging.getLogger(__name__)
 
 class GenerateError:
     def generate_schema_error(row_num: str, attribute_name: str, error_msg: str, invalid_entry: str, sg: SchemaGenerator,)-> List[str]:
         '''
         Purpose: Process error messages generated from schema
@@ -33,23 +39,26 @@
             - attribute_name: the attribute the error occurred on.
             - error_msg: Error message
         '''
         error_list = []
         warning_list = []
         
         #Determine which, if any, message to raise
-        raises = GenerateError.get_message_level(
-            val_rule = 'schema',
-            attribute_name = attribute_name,
-            sg = sg,
-            )
+        if attribute_name.lower() == 'wrong schema':
+            raises = 'error'
+        else:    
+            raises = GenerateError.get_message_level(
+                val_rule = 'schema',
+                attribute_name = attribute_name,
+                sg = sg,
+                )
 
         #if a message needs to be raised, get the approrpiate function to do so
         if raises:
-            logLevel = getattr(logging,raises)  
+            logLevel = getattr(logger,raises)  
         else:
             return error_list, warning_list
 
 
         error_col = attribute_name  # Attribute name
         error_row = row_num  # index row of the manifest where the error presented.
         error_message = error_msg
@@ -75,31 +84,32 @@
                 If an error is found in the string formatting, detect and record
                 an error message.
             Input:
                 - list_string: the user input list, that is represented as a string.
                 - row_num: the row the error occurred on.
                 - attribute_name: the attribute the error occurred on.
             Returns:
-                Logging.error.
-                Errors: List[str] Error details for further storage.
+            logger.error or logger.warning.
+            Errors: List[str] Error details for further storage.
+            warnings: List[str] Warning details for further storage.
             """
 
         error_list = []
         warning_list = []
         
         #Determine which, if any, message to raise
         raises = GenerateError.get_message_level(
             val_rule = val_rule,
             attribute_name = attribute_name,
             sg = sg,
             )
 
         #if a message needs to be raised, get the approrpiate function to do so
         if raises:
-            logLevel = getattr(logging,raises)  
+            logLevel = getattr(logger,raises)  
         else:
             return error_list, warning_list
 
         if list_error == "not_comma_delimited":
             error_str = (
                 f"For attribute {attribute_name} in row {row_num} it does not "
                 f"appear as if you provided a comma delimited string. Please check "
@@ -136,30 +146,31 @@
             Input:
                 val_rule: str, defined in the schema.
                 reg_expression: str, defined in the schema
                 row_num: str, row where the error was detected
                 module_to_call: re module specified in the schema
                 attribute_name: str, attribute being validated
             Returns:
-                Logging.error.
-                Errors: List[str] Error details for further storage.
+            logger.error or logger.warning.
+            Errors: List[str] Error details for further storage.
+            warnings: List[str] Warning details for further storage.
             """
         error_list = []
         warning_list = []
         
         #Determine which, if any, message to raise
         raises = GenerateError.get_message_level(
             val_rule = val_rule,
             attribute_name = attribute_name,
             sg = sg,
             )
 
         #if a message needs to be raised, get the approrpiate function to do so
         if raises:
-            logLevel = getattr(logging,raises)  
+            logLevel = getattr(logger,raises)  
         else:
             return error_list, warning_list
 
         regex_error_string = (
             f"For the attribute {attribute_name}, on row {row_num}, the string is not properly formatted. "
             f'It should follow the following re.{module_to_call} pattern "{reg_expression}".'
         )
@@ -186,51 +197,55 @@
                 Generate an logging error as well as a stored error message, when
                 a type error is encountered.
             Input:
                 val_rule: str, defined in the schema.
                 row_num: str, row where the error was detected
                 attribute_name: str, attribute being validated
             Returns:
-                Logging.error.
-                Errors: List[str] Error details for further storage.
+            logger.error or logger.warning.
+            Errors: List[str] Error details for further storage.
+            warnings: List[str] Warning details for further storage.
             """
 
         error_list = []
         warning_list = []
         
         #Determine which, if any, message to raise
         raises = GenerateError.get_message_level(
             val_rule = val_rule,
             attribute_name = attribute_name,
             sg = sg,
             )
 
         #if a message needs to be raised, get the approrpiate function to do so
         if raises:
-            logLevel = getattr(logging,raises)  
+            logLevel = getattr(logger,raises)  
         else:
             return error_list, warning_list
 
         type_error_str = (
             f"On row {row_num} the attribute {attribute_name} "
             f"does not contain the proper value type {val_rule}."
         )
-        logLevel(type_error_str)
         error_row = row_num  # index row of the manifest where the error presented.
         error_col = attribute_name  # Attribute name
         error_message = type_error_str
         error_val = invalid_entry
 
-
-        #return error and empty list for warnings
-        if raises == 'error':
-            error_list = [error_row, error_col, error_message, error_val]
-        #return warning and empty list for errors
-        elif raises == 'warning':
-            warning_list = [error_row, error_col, error_message, error_val]
+        # If IsNA rule is being used to allow `Not Applicable` entries, do not log a message
+        if error_val.lower() == 'not applicable' and rule_in_rule_list('IsNA', sg.get_node_validation_rules(sg.get_node_label(attribute_name))):
+          pass  
+        else:
+            logLevel(type_error_str)
+            #return error and empty list for warnings
+            if raises == 'error':
+                error_list = [error_row, error_col, error_message, error_val]
+            #return warning and empty list for errors
+            elif raises == 'warning':
+                warning_list = [error_row, error_col, error_message, error_val]
         
         return error_list, warning_list              
 
     def generate_url_error(
         url: str, url_error: str, row_num: str, attribute_name: str, argument: str,
         invalid_entry:str, sg: SchemaGenerator, val_rule: str,
     ) -> List[str]:
@@ -250,31 +265,32 @@
                         e.g. 'lkejrlei', '0', 'not applicable'
             Input:
                 url: str, that was input by the user.
                 url_error: str, error detected in url_validation()
                 attribute_name: str, attribute being validated
                 argument: str, argument being validated.
             Returns:
-                Logging.error.
-                Errors: List[str] Error details for further storage.
+            logger.error or logger.warning.
+            Errors: List[str] Error details for further storage.
+            warnings: List[str] Warning details for further storage.
             """
 
         error_list = []
         warning_list = []
         
         #Determine which, if any, message to raise
         raises = GenerateError.get_message_level(
             val_rule = val_rule,
             attribute_name = attribute_name,
             sg = sg,
             )
 
         #if a message needs to be raised, get the approrpiate function to do so
         if raises:
-            logLevel = getattr(logging,raises)  
+            logLevel = getattr(logger,raises)  
         else:
             return error_list, warning_list
 
 
         error_row = row_num  # index row of the manifest where the error presented.
         error_col = attribute_name  # Attribute name
         if url_error == "invalid_url":
@@ -330,30 +346,31 @@
                 val_rule: str, defined in the schema.
                 matching_manifests: list of manifests with all values in the target attribute present
                 manifest_ID: str, synID of the target manifest missing the source value
                 attribute_name: str, attribute being validated
                 invalid_entry: str, value present in source manifest that is missing in the target
                 row_num: row in source manifest with value missing in target manifests             
             Returns:
-                Logging.error.
-                Errors: List[str] Error details for further storage.
+            logger.error or logger.warning.
+            Errors: List[str] Error details for further storage.
+            warnings: List[str] Warning details for further storage.
             """
         error_list = []
         warning_list = []
         
         #Determine which, if any, message to raise
         raises = GenerateError.get_message_level(
             val_rule = val_rule,
             attribute_name = attribute_name,
             sg = sg,
             )
 
         #if a message needs to be raised, get the approrpiate function to do so
         if raises:
-            logLevel = getattr(logging,raises)  
+            logLevel = getattr(logger,raises)  
         else:
             return error_list, warning_list
 
         if val_rule.__contains__('matchAtLeast'):
             cross_error_str = (
                 f"Value(s) {invalid_entry} from row(s) {row_num} of the attribute {attribute_name} in the source manifest are missing." )
             cross_error_str += f" Manifest(s) {missing_manifest_ID} are missing the value(s)." if missing_manifest_ID else ""
@@ -408,75 +425,86 @@
                 val_rule: str, defined in the schema.
                 attribute_name: str, attribute being validated
                 sg: schemaGenerator object
                 row_num: str, row where the error was detected
                 error_val: value duplicated
 
         Returns:
-            Logging.error or Logging.warning.
-            Message: List[str] Error|Warning details for further storage.
+            logger.error or logger.warning.
+            Errors: List[str] Error details for further storage.
+            warnings: List[str] Warning details for further storage.
         """
         error_list = []
         warning_list = []
         error_col = attribute_name  # Attribute name
-        
+        if error_val:
+            error_val = iterable_to_str_list(set(error_val))
+
         #Determine which, if any, message to raise
         raises = GenerateError.get_message_level(
             val_rule=val_rule,
             attribute_name = attribute_name,
             sg = sg,
             )
 
         #if a message needs to be raised, get the approrpiate function to do so
         if raises:
-            logLevel = getattr(logging,raises)  
+            logLevel = getattr(logger,raises)  
         else:
             return error_list, warning_list
         
         #log warning or error message
         if val_rule.startswith('recommended'):
-            cross_error_str = (
+            content_error_str = (
                 f"Column {attribute_name} is recommended but empty."
             )
-            logLevel(cross_error_str)
-            error_message = cross_error_str
+            logLevel(content_error_str)
+            error_message = content_error_str
 
             if raises == 'error':
                 error_list = [error_col, error_message]
             #return warning and empty list for errors
             elif raises == 'warning':
                 warning_list = [error_col, error_message]
 
             return error_list, warning_list
 
         elif val_rule.startswith('unique'):    
-            cross_error_str = (
-                f"Column {attribute_name} has the duplicate value(s) {set(error_val)} in rows: {row_num}."
+            content_error_str = (
+                f"Column {attribute_name} has the duplicate value(s) {error_val} in rows: {row_num}."
             )
 
         elif val_rule.startswith('protectAges'):
-            cross_error_str = (
+            content_error_str = (
                 f"Column {attribute_name} contains ages that should be censored in rows: {row_num}."
             )           
 
         elif val_rule.startswith('inRange'):
-            cross_error_str = (
+            content_error_str = (
                 f"{attribute_name} values in rows {row_num} are out of the specified range."
+            )
+        elif val_rule.startswith('date'):
+            content_error_str = (
+                f"{attribute_name} values in rows {row_num} are not parsable as dates."
+            )  
+        elif val_rule.startswith('IsNA'):
+            content_error_str = (
+                f"{attribute_name} values in rows {row_num} are not marked as 'Not Applicable'."
             )  
 
-        logLevel(cross_error_str)
-        error_row = row_num 
-        error_message = cross_error_str
-
-        #return error and empty list for warnings
-        if raises == 'error':
-            error_list = [error_row, error_col, error_message, set(error_val)]
-        #return warning and empty list for errors
-        elif raises == 'warning':
-            warning_list = [error_row, error_col, error_message, set(error_val)]
+        if val_rule != "IsNA":
+            logLevel(content_error_str)
+            error_row = row_num 
+            error_message = content_error_str
+            #return error and empty list for warnings
+            if raises == 'error':
+                error_list = [error_row, error_col, error_message, error_val]
+            #return warning and empty list for errors
+            elif raises == 'warning':
+                warning_list = [error_row, error_col, error_message, error_val]
         
         return error_list, warning_list
 
     def get_message_level(
         sg: SchemaGenerator,
         attribute_name: str,
         val_rule: str,
@@ -500,33 +528,28 @@
         # TODO: recommended and other rules
         """
 
         level = None
         rule_parts = val_rule.split(" ")
         rule_info = validation_rule_info()
 
-        if not sg.is_node_required(node_display_name=attribute_name):
-            # raise warning if recommended but not required
-            if 'recommended' in val_rule:
-                level = 'warning'
-            # If not required or recommended raise warnings to notify
-            else:
-                level = 'warning' 
-                return level
-        elif sg.is_node_required(node_display_name=attribute_name) and 'recommended' in val_rule:
-            level = None
-        
-        
+        #set message level to default and change after
+        if rule_parts[0] != 'schema':
+            level = rule_info[rule_parts[0]]['default_message_level']
+
         # Parse rule for level, set to default if not specified
         if rule_parts[-1].lower() == 'error' or rule_parts[0] == 'schema':
             level = 'error'
         elif rule_parts[-1].lower() == 'warning':
-            level = 'warning'
-        else:
-            level = rule_info[rule_parts[0]]['default_message_level']
+            level = 'warning'        
+        elif not sg.is_node_required(node_display_name=attribute_name):
+            # If not required raise warnings to notify
+            level = 'warning' 
+        elif sg.is_node_required(node_display_name=attribute_name) and 'recommended' in val_rule:
+            level = None
             
         return level
 
 class ValidateAttribute(object):
     """
     A collection of functions to validate manifest attributes.
         list_validation
@@ -538,52 +561,51 @@
     See functions for more details.
     TODO:
         - Add year validator
         - Add string length validator
     """
 
     def get_target_manifests(target_component, project_scope: List):
-
+        t_manifest_search = perf_counter()
         target_manifest_IDs=[]
         target_dataset_IDs=[]
         
         #login
-        access_token = getenv("SYNAPSE_ACCESS_TOKEN")
-        if access_token:
-            synStore = SynapseStorage(access_token=access_token,project_scope=project_scope)
-        else:
-            synStore = SynapseStorage(project_scope=project_scope)        
+        synStore = SynapseStorage(project_scope=project_scope)        
 
         #Get list of all projects user has access to
         projects = synStore.getStorageProjects(project_scope=project_scope)
         for project in projects:
             
             #get all manifests associated with datasets in the projects
             target_datasets=synStore.getProjectManifests(projectId=project[0])
 
             #If the manifest includes the target component, include synID in list
             for target_dataset in target_datasets:
                 if target_component == target_dataset[-1][0].replace(" ","").lower() and target_dataset[1][0] != "":
                     target_manifest_IDs.append(target_dataset[1][0])
                     target_dataset_IDs.append(target_dataset[0][0])
 
+        logger.debug(f"Cross manifest gathering elapsed time {perf_counter()-t_manifest_search}")
         return synStore, target_manifest_IDs, target_dataset_IDs    
 
     def list_validation(
         self, val_rule: str, manifest_col: pd.core.series.Series, sg: SchemaGenerator,
     ) -> (List[List[str]], List[List[str]], pd.core.series.Series):
         """
         Purpose:
             Determine if values for a particular attribute are comma separated.
         Input:
             - val_rule: str, Validation rule
             - manifest_col: pd.core.series.Series, column for a given attribute
         Returns:
             - manifest_col: Input values in manifest arere-formatted to a list
-            - Error log, error list
+            logger.error or logger.warning.
+            Errors: List[str] Error details for further storage.
+            warnings: List[str] Warning details for further storage.
         """
 
         # For each 'list' (input as a string with a , delimiter) entered,
         # convert to a real list of strings, with leading and trailing
         # white spaces removed.
         errors = []
         warnings = []
@@ -639,16 +661,17 @@
                 regular expression.
                 - module: is the name of the module within re to run ie. search. 
                 - regular_expression: is the regular expression with which to validate
                 the user input.
         Returns:
             - This function will return errors when the user input value
             does not match schema specifications.
-            Logging.error.
+            logger.error or logger.warning.
             Errors: List[str] Error details for further storage.
+            warnings: List[str] Warning details for further storage.
         TODO: 
             move validation to convert step.
         """
 
         reg_exp_rules = val_rule.split(" ")
 
         try:
@@ -723,16 +746,17 @@
             - val_rule: str, Validation rule, specifying input type, either
                 'float', 'int', 'num', 'str'
             - manifest_col: pd.core.series.Series, column for a given
                 attribute in the manifest
         Returns:
             -This function will return errors when the user input value
             does not match schema specifications.
-            Logging.error.
+            logger.error or logger.warning.
             Errors: List[str] Error details for further storage.
+            warnings: List[str] Warning details for further storage.
         TODO:
             Convert all inputs to .lower() just to prevent any entry errors.
         """
         specified_type = {
             'num': (int, np.int64, float),
             'int': (int, np.int64),
             'float': (float),
@@ -895,14 +919,15 @@
         scope=val_rule.lower().split(" ")[2]
         target_column.name=target_attribute
 
         
         #Get IDs of manifests with target component
         synStore, target_manifest_IDs, target_dataset_IDs = ValidateAttribute.get_target_manifests(target_component,project_scope)
 
+        t_cross_manifest = perf_counter()
         #Read each manifest
         for target_manifest_ID, target_dataset_ID in zip(target_manifest_IDs,target_dataset_IDs):
             entity = synStore.getDatasetManifest(
                 datasetId = target_dataset_ID,
                 downloadFile = True
                 )
             target_manifest=pd.read_csv(entity.path)
@@ -945,33 +970,35 @@
 
         if scope.__contains__('value'):
             missing_values = manifest_col[~manifest_col.isin(target_column)]
             duplicated_values = manifest_col[manifest_col.isin(target_column[target_column.duplicated()])]
             
             if val_rule.__contains__('matchAtLeastOne') and not missing_values.empty:
                 missing_rows = missing_values.index.to_numpy() + 2
+                missing_rows = np_array_to_str_list(missing_rows)
                 vr_errors, vr_warnings = GenerateError.generate_cross_warning(
                         val_rule = val_rule,
-                        row_num = str(list(missing_rows)),
+                        row_num = missing_rows,
                         attribute_name = source_attribute,
-                        invalid_entry = str(missing_values.values.tolist()),
+                        invalid_entry = iterable_to_str_list(missing_values),
                         sg = sg,
                     )
                 if vr_errors:
                     errors.append(vr_errors)
                 if vr_warnings:
                     warnings.append(vr_warnings)
             elif val_rule.__contains__('matchExactlyOne') and (duplicated_values.any() or missing_values.any()):
                 invalid_values  = pd.merge(duplicated_values,missing_values,how='outer')
                 invalid_rows    = pd.merge(duplicated_values,missing_values,how='outer',left_index=True,right_index=True).index.to_numpy() + 2
+                invalid_rows    = np_array_to_str_list(invalid_rows)
                 vr_errors, vr_warnings = GenerateError.generate_cross_warning(
                         val_rule = val_rule,
-                        row_num = str(list(invalid_rows)), 
+                        row_num = invalid_rows,
                         attribute_name = source_attribute, 
-                        invalid_entry = str(pd.Series(invalid_values.squeeze()).values.tolist()),
+                        invalid_entry = iterable_to_str_list(invalid_values.squeeze()),
                         sg = sg,
                     )
                 if vr_errors:
                     errors.append(vr_errors)
                 if vr_warnings:
                     warnings.append(vr_warnings)
             
@@ -982,23 +1009,22 @@
             if val_rule.__contains__('matchAtLeastOne') and len(present_manifest_log) < 1:     
                 missing_entries = list(missing_manifest_log.values()) 
                 missing_manifest_IDs = list(missing_manifest_log.keys()) 
                 for missing_entry in missing_entries:
                     missing_rows.append(missing_entry.index[0]+2)
                     missing_values.append(missing_entry.values[0])
                     
-                missing_rows=list(set(missing_rows))
-                missing_values=list(set(missing_values))
-                #print(missing_rows,missing_values)
-
+                missing_rows=iterable_to_str_list(set(missing_rows))
+                missing_values=iterable_to_str_list(set(missing_values))
+                
                 vr_errors, vr_warnings = GenerateError.generate_cross_warning(
                         val_rule = val_rule,
-                        row_num = str(missing_rows),
+                        row_num = missing_rows,
                         attribute_name = source_attribute,
-                        invalid_entry = str(missing_values),
+                        invalid_entry = missing_values,
                         missing_manifest_ID = missing_manifest_IDs,
                         sg = sg,
                     )
                 if vr_errors:
                     errors.append(vr_errors)
                 if vr_warnings:
                     warnings.append(vr_warnings)
@@ -1011,10 +1037,11 @@
                     )
                 if vr_errors:
                     errors.append(vr_errors)
                 if vr_warnings:
                     warnings.append(vr_warnings)
                 
 
+        logger.debug(f"cross manifest validation time {perf_counter()-t_cross_manifest}")
         return errors, warnings
```

### Comparing `schematicpy-23.1.1/schematic/models/validate_manifest.py` & `schematicpy-23.6.1/schematic/models/validate_manifest.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import logging
 
 import numpy as np
 import os
 import pandas as pd
 import re
 import sys
+from time import perf_counter
 
 # allows specifying explicit variable types
 from typing import Any, Dict, Optional, Text, List
 from urllib.parse import urlparse
 from urllib.request import urlopen, OpenerDirector, HTTPDefaultErrorHandler
 from urllib.request import Request
 from urllib import error
@@ -43,23 +44,23 @@
             """
         error_col = attribute_name  # Attribute name
         if error_type == "too_many_rules":
             error_str = (
                 f"For attribute {attribute_name}, the provided validation rules ({validation_rules}) ."
                 f"have too many entries. We currently only specify two rules ('list :: another_rule')."
             )
-            logging.error(error_str)
+            logger.error(error_str)
             error_message = error_str
             error_val = f"Multiple Rules: too many rules"
         if error_type == "list_not_first":
             error_str = (
                 f"For attribute {attribute_name}, the provided validation rules ({validation_rules}) are improperly "
                 f"specified. 'list' must be first."
             )
-            logging.error(error_str)
+            logger.error(error_str)
             error_message = error_str
             error_val = f"Multiple Rules: list not first"
         return ["NA", error_col, error_message, error_val]
 
     def validate_manifest_rules(
         self, manifest: pd.core.frame.DataFrame, sg: SchemaGenerator, restrict_rules: bool, project_scope: List,
     ) -> (pd.core.frame.DataFrame, List[List[str]]):
@@ -121,57 +122,61 @@
         ]
 
         # initialize error and warning handling lists.
         errors = []   
         warnings = [] 
 
         if not restrict_rules:
+            t_GE = perf_counter()
             #operations necessary to set up and run ge suite validation
             ge_helpers=GreatExpectationsHelpers(
                 sg=sg,
                 unimplemented_expectations=unimplemented_expectations,
                 manifest = manifest,
                 manifestPath = self.manifestPath,
                 )
 
             ge_helpers.build_context()
             ge_helpers.build_expectation_suite()
             ge_helpers.build_checkpoint()
 
-        #run GE validation
-            results = ge_helpers.context.run_checkpoint(
-                checkpoint_name="manifest_checkpoint",
-                batch_request={
-                    "runtime_parameters": {"batch_data": manifest},
-                    "batch_identifiers": {
-                        "default_identifier_name": "manifestID"
+            try:
+                #run GE validation
+                results = ge_helpers.context.run_checkpoint(
+                    checkpoint_name=ge_helpers.checkpoint_name,
+                    batch_request={
+                        "runtime_parameters": {"batch_data": manifest},
+                        "batch_identifiers": {
+                            "default_identifier_name": "manifestID"
+                        },
                     },
-                },
-                result_format={'result_format': 'COMPLETE'},
-            )        
+                    result_format={'result_format': 'COMPLETE'},
+                )       
+            finally:
+                ge_helpers.context.delete_checkpoint(ge_helpers.checkpoint_name) 
         
-            #print(results)       
-            #results.list_validation_results()
             validation_results = results.list_validation_results()
             
 
             #parse validation results dict and generate errors
             errors, warnings = ge_helpers.generate_errors(
                 errors = errors,
                 warnings = warnings,
                 validation_results = validation_results,
                 validation_types = validation_types,
                 sg = sg,
-                )               
+                )        
+            logger.debug(f"GE elapsed time {perf_counter()-t_GE}")       
         else:             
-            logging.info("Great Expetations suite will not be utilized.")  
-
+            logger.info("Great Expetations suite will not be utilized.")  
 
+        t_err=perf_counter()
         regex_re=re.compile('regex.*')
         for col in manifest.columns:
+            
             # remove trailing/leading whitespaces from manifest
             manifest.applymap(lambda x: x.strip() if isinstance(x, str) else x)
             validation_rules = sg.get_node_validation_rules(col)
 
             # Check that attribute rules conform to limits:
             # no more than two rules for an attribute. 
             # As more combinations get added, may want to bring out into its own function / or use validate_rules_utils?
@@ -183,17 +188,18 @@
                 )
 
             # Given a validation rule, run validation. Skip validations already performed by GE
             for rule in validation_rules:
                 validation_type = rule.split(" ")[0]
                 if rule_in_rule_list(rule,unimplemented_expectations) or (rule_in_rule_list(rule,in_house_rules) and restrict_rules):
                     if not rule_in_rule_list(rule,in_house_rules):
-                        logging.warning(f"Validation rule {rule.split(' ')[0]} has not been implemented in house and cannnot be validated without Great Expectations.")
+                        logger.warning(f"Validation rule {rule.split(' ')[0]} has not been implemented in house and cannnot be validated without Great Expectations.")
                         continue  
 
+                    t_indiv_rule=perf_counter()
                     #Validate for each individual validation rule.
                     validation_method = getattr(
                             ValidateAttribute, validation_types[validation_type]['type']
                         )
 
                     if validation_type == "list":
                         vr_errors, vr_warnings, manifest_col = validation_method(
@@ -209,46 +215,48 @@
                             self, rule, manifest[col], sg,
                         )
                     # Check for validation rule errors and add them to other errors.
                     if vr_errors:
                         errors.extend(vr_errors)
                     if vr_warnings:
                         warnings.extend(vr_warnings)
-
+                    logger.debug(f"Rule {rule} elapsed time: {perf_counter()-t_indiv_rule}")
+        logger.debug(f"In House validation elapsed time {perf_counter()-t_err}")
         return manifest, errors, warnings
 
     def validate_manifest_values(self, manifest, jsonSchema, sg
     ) -> (List[List[str]], List[List[str]]):
-        
+        t_json_schema = perf_counter()
+
         errors = []
         warnings = []
         col_attr = {} # save the mapping between column index and attribute name
         
         # numerical values need to be type string for the jsonValidator
         for col in manifest.select_dtypes(include=[int, np.int64, float, np.float64]).columns:
             manifest[col]=manifest[col].astype('string')
         manifest = manifest.applymap(lambda x: str(x) if isinstance(x, (int, np.int64, float, np.float64)) else x, na_action='ignore')
 
         annotations = json.loads(manifest.to_json(orient="records"))
         for i, annotation in enumerate(annotations):
             v = Draft7Validator(jsonSchema)
             for error in sorted(v.iter_errors(annotation), key=exceptions.relevance):
-                errorRow = i + 2
+                errorRow = str(i + 2)
                 errorCol = error.path[-1] if len(error.path) > 0 else "Wrong schema"
                 errorColName = error.path[0] if len(error.path) > 0 else "Wrong schema"
                 errorMsg = error.message[0:500]
                 errorVal = error.instance if len(error.path) > 0 else "Wrong schema"
 
                 val_errors, val_warnings =  GenerateError.generate_schema_error(row_num = errorRow, attribute_name = errorColName, error_msg = errorMsg, invalid_entry = errorVal, sg = sg)
 
                 if val_errors:
                     errors.append(val_errors)
                 if val_warnings:
                     warnings.append(val_warnings)
-
+        logger.debug(f"JSON Schema validation elapsed time {perf_counter()-t_json_schema}")
         return errors, warnings
 
 
 def validate_all(self, errors, warnings, manifest, manifestPath, sg, jsonSchema, restrict_rules, project_scope: List):
     vm = ValidateManifest(errors, manifest, manifestPath, sg, jsonSchema)
     manifest, vmr_errors, vmr_warnings = vm.validate_manifest_rules(manifest, sg, restrict_rules, project_scope)
     if vmr_errors:
```

### Comparing `schematicpy-23.1.1/schematic/schemas/commands.py` & `schematicpy-23.6.1/schematic/schemas/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sys
 import re
 
 from schematic.schemas.df_parser import _convert_csv_to_data_model
 from schematic.utils.cli_utils import query_dict
 from schematic.help import schema_commands
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger('schematic')
 click_log.basic_config(logger)
 
 CONTEXT_SETTINGS = dict(help_option_names=["--help", "-h"])  # help options
 
 # invoke_without_command=True -> forces the application not to show aids before losing them with a --h
 @click.group(context_settings=CONTEXT_SETTINGS, invoke_without_command=True)
 def schema():  # use as `schematic model ...`
```

### Comparing `schematicpy-23.1.1/schematic/schemas/curie.py` & `schematicpy-23.6.1/schematic/schemas/curie.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.1.1/schematic/schemas/df_parser.py` & `schematicpy-23.6.1/schematic/schemas/df_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 )
 
 
 def get_class(
     se: SchemaExplorer,
     class_display_name: str,
     description: str = None,
-    subclass_of: list = None,
+    subclass_of: list = [],
     requires_dependencies: list = None,
     requires_range: list = None,
     requires_components: list = None,
     required: bool = None,
     validation_rules: list = None,
 ) -> dict:
 
@@ -147,51 +147,57 @@
 
     return class_attributes
 
 
 def get_property(
     se: SchemaExplorer,
     property_display_name: str,
-    property_class_name: str,
+    property_class_names: list,
     description: str = None,
     requires_range: list = None,
     requires_dependencies: list = None,
     required: bool = None,
     validation_rules: str = None,
 ) -> dict:
 
     """Constructs a new schema.org compliant property of an existing schema.org object/class; note that the property itself is a schema.org object class.
 
     Args:
         se: a schema explorer object allowing the traversal and modification of a schema graph
         property_display_name: human readable label for the schema object/attribute: key characteristic X of the assay, related protocol, or downstream data that we want to record as metadata feature
-        property_class_name: *schema* label of the class/object that this is a property of
+        property_class_name: *schema* label of the classes/objects that this is a property of
         description: definition or a reference containing the definition of attribute X. Preferably provide a source ontology link or code in addition to the definition.
         requires_range: what is the set/domain of values that this attribute can be assigned to; currently only used to specify primitive types. TODO: extend to reg exp patterns
         requires_dependencies: important characteristics, if any, of property X that need to be recorded as metadata features given property X is specified. These characteristics are attributes themselves and need to pre-exist in the schema as such
         validation_rules: a list of validation rules defined for this class (e.g. defining what is a valid object of this property)
 
 
     Returns: a json schema.org  property object
     """
     property_name = se.get_property_label_from_display_name(property_display_name)
-
+    
     property_attributes = {
         "@id": "bts:" + property_name,
         "@type": "rdf:Property",
         "rdfs:comment": description
         if description and not pd.isnull(description)
         else "TBD",
         "rdfs:label": property_name,
         "sms:displayName": property_display_name,
-        "schema:domainIncludes": {
-            "@id": "bts:" + se.get_class_label_from_display_name(property_class_name)
-        },
         "schema:isPartOf": {"@id": "http://schema.biothings.io"},
     }
+
+    domain_includes = {
+            "schema:domainIncludes": [
+                {"@id": "bts:" + se.get_class_label_from_display_name(val)}
+                for val in property_class_names
+            ]
+        }
+    property_attributes.update(domain_includes)
+
     if requires_range:
         value_constraint = {
             "schema:rangeIncludes": [
                 {"@id": "bts:" + se.get_class_label_from_display_name(val)}
                 for val in requires_range
             ]
         }
@@ -262,14 +268,30 @@
     ):
         raise ValueError(
             "The input CSV schema file contains the 'Requires' and/or the 'Requires "
             "Component' column headers. These columns were renamed to 'DependsOn' and "
             "'DependsOn Component', respectively. Switch to the new column names."
         )
 
+def _prop_2_classes(properties: dict) -> dict:
+    
+    """Create a dictionary linking all properties to their classes.
+    Args:
+        properties (dict): attributes and their properties (if applicable)
+    Returns:
+        Dictionary linking properties to all the classes in their domain.
+    """
+    prop_2_classes = {}
+    for record in properties:
+        if not pd.isnull(record["Properties"]):
+            props = record["Properties"].strip().split(",")
+            for pr in props:
+                prop_2_classes.setdefault(pr.strip(),[]).append(record["Attribute"])
+    
+    return prop_2_classes
 
 def create_nx_schema_objects(
     schema_extension: pd.DataFrame, se: SchemaExplorer
 ) -> SchemaExplorer:
     """Creates classes for all attributes and adds them to the schema.
     Args:
         schema_extension: a pandas dataframe containing schema definition; see example here: https://docs.google.com/spreadsheets/d/1J2brhqO4kpeHIkNytzlqrdIiRanXDr6KD2hqjOTC9hs/edit#gid=0
@@ -306,30 +328,25 @@
     all_properties = []
     for prop in props:
         all_properties += [p.strip() for p in prop.split(",")]
 
     # get both attributes and their properties (if any)
     properties = schema_extension[["Attribute", "Properties"]].to_dict("records")
 
-    # property to class map
-    prop_2_class = {}
-    for record in properties:
-        if not pd.isnull(record["Properties"]):
-            props = record["Properties"].strip().split(",")
-            for p in props:
-                prop_2_class[p.strip()] = record["Attribute"]
-
+    prop_2_classes = _prop_2_classes(properties)
+    
     logger.debug("Adding attributes")
     for attribute in attributes:
 
         required = None
         if not pd.isnull(attribute["Required"]):
             required = attribute["Required"]
 
         if not attribute["Attribute"] in all_properties:
+            # Attribute is not a property
             display_name = attribute["Attribute"]
 
             subclass_of = None
             if not pd.isnull(attribute["Parent"]):
                 subclass_of = [
                     parent for parent in attribute["Parent"].strip().split(",")
                 ]
@@ -349,25 +366,27 @@
             # check if attribute doesn't already exist and add it
             if not attribute_exists(se, new_class["rdfs:label"]):
                 se.add_schema_object_nx(new_class, **rel_dict)
             else:
                 print("ATTRIBUTE EXISTS")
                 print(new_class)
             """
-
+        
         else:
+            # Attribute is a property
             display_name = attribute["Attribute"]
 
             new_property = get_property(
                 se,
                 display_name,
-                prop_2_class[display_name],
+                prop_2_classes[display_name],
                 description=attribute["Description"],
                 required=required,
             )
+
             # check if attribute doesn't already exist and add it
             if not attribute_exists(se, new_property["rdfs:label"]):
                 se.add_schema_object_nx(new_property, **rel_dict)
 
     logger.debug("Done adding attributes")
 
     # TODO check if schema already contains property - may require property context in csv schema definition
@@ -447,40 +466,43 @@
             for val in range_values_list:
                 # check if value is in attributes column; add it as a class if not
                 if not val.strip() in list(schema_extension["Attribute"]):
 
                     # determine parent class of the new value class
                     # if this attribute is not a property, set it as a parent class
                     if not attribute["Attribute"] in all_properties:
-                        parent = attribute["Attribute"]
+                        parent = [attribute["Attribute"]]
                     else:
                         # this attribute is a property, set the parent to the domain class of this attribute
+                        
                         parent = se.get_class_by_property(attribute["Attribute"])
+                        
                         if not parent:
                             raise ValueError(
                                 f"Listed valid value: {val}, for attribute: {attribute['Attribute']} "
                                 "must have a class parent. The extension could not be added to the schema."
                             )
-
                     new_class = get_class(
-                        se, val, description=None, subclass_of=[parent]
+                        se, val, description=None, subclass_of=parent
                     )
+
                     # check if attribute doesn't already exist and add it
                     if not attribute_exists(se, new_class["rdfs:label"]):
                         se.add_schema_object_nx(new_class, **rel_dict)
 
                 # update rangeIncludes of attribute
                 # if attribute is not a property, then assume it is a class
                 if not attribute["Attribute"] in all_properties:
                     class_info = se.explore_class(
                         se.get_class_label_from_display_name(attribute["Attribute"])
                     )
                     class_info["range"].append(
                         se.get_class_label_from_display_name(val)
                     )
+
                     class_range_edit = get_class(
                         se,
                         attribute["Attribute"],
                         description=attribute["Description"],
                         subclass_of=[attribute["Parent"]],
                         requires_dependencies=class_info["dependencies"],
                         requires_range=class_info["range"],
@@ -493,14 +515,15 @@
                     # the attribute is a property
                     property_info = se.explore_property(
                         se.get_property_label_from_display_name(attribute["Attribute"])
                     )
                     property_info["range"].append(
                         se.get_class_label_from_display_name(val)
                     )
+                    
                     property_range_edit = get_property(
                         se,
                         attribute["Attribute"],
                         property_info["domain"],
                         description=property_info["description"],
                         requires_dependencies=property_info["dependencies"],
                         requires_range=property_info["range"],
@@ -566,16 +589,16 @@
             try:
                 logger.debug(val + "validation rules added")
             except:
                 logger.debug("Validation rules added")
 
         # get dependencies for this attribute, if any are specified
         requires_dependencies = attribute["DependsOn"]
-        if not pd.isnull(requires_dependencies):
 
+        if not pd.isnull(requires_dependencies):
             for dep in requires_dependencies.strip().split(","):
                 # check if dependency is a property or not
                 dep = dep.strip()
                 dep_is_property = dep in all_properties
                 dep_label = ""
                 # set dependency label based on kind of dependency: class or property
                 if dep_is_property:
@@ -757,8 +780,8 @@
     # load base schema (BioThings)
     base_se.load_schema(base_schema_path)
 
     # call parser code that converts a dataframe of the RFC
     # specs. into a JSON-LD data model
     base_se = create_nx_schema_objects(rfc_df, base_se)
 
-    return base_se
+    return base_se
```

### Comparing `schematicpy-23.1.1/schematic/schemas/explorer.py` & `schematicpy-23.6.1/schematic/schemas/explorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,23 +236,24 @@
             if record["@type"] == "rdf:Property":
                 if (
                     type(record["schema:domainIncludes"]) == dict
                     and record["schema:domainIncludes"]["@id"] == schema_uri
                 ):
                     properties.append(record["rdfs:label"])
                 elif (
-                    type(record["schema:domainIncludes"]) == list
-                    and [
-                        item
-                        for item in record["schema:domainIncludes"]
-                        if item["@id"] == schema_uri
-                    ]
-                    != []
-                ):
-                    properties.append(record["rdfs:label"])
+                     type(record["schema:domainIncludes"]) == list
+                     and [
+                         item
+                         for item in record["schema:domainIncludes"]
+                         if item["@id"] == schema_uri
+                     ]
+                     != []
+                     ):
+                   
+                     properties.append(record["rdfs:label"])
         return properties
 
     def find_all_class_properties(self, schema_class, display_as_table=False):
         """Find all properties associated with a given class
         # TODO : need to deal with recursive paths
         """
         parents = self.find_parent_classes(schema_class)
@@ -473,21 +474,26 @@
         schema_property = self.get_property_label_from_display_name(
             property_display_name
         )
 
         for record in self.schema["@graph"]:
             if record["@type"] == "rdf:Property":
                 if record["rdfs:label"] == schema_property:
-                    p_domain = dict2list(record["schema:domainIncludes"])
-                    return unlist(
-                        [
-                            self.uri2label(schema_class["@id"])
-                            for schema_class in p_domain
-                        ]
-                    )
+                    p_domain = record["schema:domainIncludes"]
+
+                    return [
+                            self.uri2label(record["@id"]) 
+                                for record in p_domain
+                            ]
+                    #return unlist(
+                    #    [
+                    #        self.uri2label(schema_class["@id"])
+                    #        for schema_class in p_domain
+                    #    ]
+                    #)
 
         return None
 
     def uri2label(self, uri):
         return uri.split(":")[1]
 
     def explore_property(self, schema_property):
@@ -498,18 +504,20 @@
         for record in self.schema["@graph"]:
             if record["@type"] == "rdf:Property":
                 if record["rdfs:label"] == schema_property:
                     property_info["id"] = record["rdfs:label"]
                     property_info["description"] = record["rdfs:comment"]
                     property_info["uri"] = curie2uri(record["@id"], namespaces)
 
-                    p_domain = dict2list(record["schema:domainIncludes"])
-                    property_info["domain"] = unlist(
-                        [self.uri2label(record["@id"]) for record in p_domain]
-                    )
+                    p_domain = record["schema:domainIncludes"]
+                    if type(p_domain) == list:
+                        property_info["domain"] = [self.uri2label(record["@id"]) for record in p_domain]
+                    elif type(p_domain) == dict:
+                        property_info["domain"] = [self.uri2label(record["@id"])]
+
                     if "schema:rangeIncludes" in record:
                         p_range = dict2list(record["schema:rangeIncludes"])
                         property_info["range"] = [
                             self.uri2label(record["@id"]) for record in p_range
                         ]
                     else:
                         property_info["range"] = []
@@ -1026,8 +1034,8 @@
         self.schema_nx = schema_graph_nx
 
         # print("Edited node {} successfully.".format(schema_object["rdfs:label"]))
 
         # update the JSON-LD schema after modifying the networkx graph
         # validate_class_schema(schema_object)
         self.schema["@graph"].append(schema_object)
-        # validate_schema(self.schema)
+        # validate_schema(self.schema)
```

### Comparing `schematicpy-23.1.1/schematic/schemas/generator.py` & `schematicpy-23.6.1/schematic/schemas/generator.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.1.1/schematic/schemas/validator.py` & `schematicpy-23.6.1/schematic/schemas/validator.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.1.1/schematic/store/synapse.py` & `schematicpy-23.6.1/schematic/store/synapse.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,181 @@
+from datetime import datetime, timedelta
 from copy import deepcopy
 import os
 import uuid  # used to generate unique names for entities
 import json
 import atexit
 import logging
 import secrets
+from dataclasses import dataclass
+import tempfile
 
 # allows specifying explicit variable types
 from typing import Dict, List, Tuple, Sequence, Union
 from collections import OrderedDict
 from tenacity import retry, stop_after_attempt, wait_chain, wait_fixed, retry_if_exception_type
 
 import numpy as np
 import pandas as pd
 import re
 import synapseclient
 from time import sleep
-
 from synapseclient import (
     Synapse,
     File,
     Folder,
     Table,
     Schema,
     EntityViewSchema,
     EntityViewType,
     Column,
     as_table_columns,
 )
 
-from synapseclient.table import CsvFileTable
-from synapseclient.table import build_table
+from synapseclient.entity import File
+from synapseclient.table import CsvFileTable, build_table, Schema
 from synapseclient.annotations import from_synapse_annotations
 from synapseclient.core.exceptions import SynapseHTTPError, SynapseAuthenticationError, SynapseUnmetAccessRestrictions
 from synapseutils import walk
 from synapseutils.copy_functions import changeFileMetaData
 
 import uuid
 
-from schematic.utils.df_utils import update_df, load_df
+from schematic_db.synapse.synapse import SynapseConfig
+from schematic_db.rdb.synapse_database import SynapseDatabase
+
+
+from schematic.utils.df_utils import update_df, load_df, col_in_dataframe, populate_df_col_with_another_col
 from schematic.utils.validate_utils import comma_separated_list_regex, rule_in_rule_list
+from schematic.utils.general import entity_type_mapping, get_dir_size, convert_size, convert_gb_to_bytes, create_temp_folder
 from schematic.schemas.explorer import SchemaExplorer
 from schematic.schemas.generator import SchemaGenerator
 from schematic.store.base import BaseStorage
 from schematic.exceptions import MissingConfigValueError, AccessCredentialsError
 
 from schematic import CONFIG
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("Synapse storage")
+
+@dataclass
+class ManifestDownload(object):
+    """
+    syn: an object of type synapseclient.
+    manifest_id: id of a manifest  
+    """
+    syn: synapseclient.Synapse
+    manifest_id: str
+
+    def _download_manifest_to_folder(self) -> File:
+        """
+        try downloading a manifest to local cache or a given folder
+        manifest
+        Return: 
+            manifest_data: A Synapse file entity of the downloaded manifest
+        """
+        # TO DO: potentially deprecate the if else statement because "manifest_folder" key always exist in config (See issue FDS-349 in Jira)
+        # on AWS, to avoid overriding manifest, we download the manifest to a temporary folder
+        if "SECRETS_MANAGER_SECRETS" in os.environ:
+            temporary_manifest_storage = "/var/tmp/temp_manifest_download"
+            if not os.path.exists(temporary_manifest_storage):
+                os.mkdir("/var/tmp/temp_manifest_download")
+            download_location = create_temp_folder(temporary_manifest_storage)
+
+        elif CONFIG["synapse"]["manifest_folder"]:
+            download_location=CONFIG["synapse"]["manifest_folder"]
+
+        else:
+            download_location=None
+        
+        if not download_location:
+            manifest_data = self.syn.get(
+                        self.manifest_id,
+                    )
+        # if download_location is provided and it is not an empty string
+        else:
+            manifest_data = self.syn.get(
+                    self.manifest_id,
+                    downloadLocation=download_location,
+                    ifcollision="overwrite.local",
+                )
+        return manifest_data 
+
+    def _entity_type_checking(self) -> str:
+        """
+        check the entity type of the id that needs to be downloaded
+        Return: 
+             if the entity type is wrong, raise an error
+        """
+        # check the type of entity
+        entity_type = entity_type_mapping(self.syn, self.manifest_id)
+        if entity_type  != "file":
+            logger.error(f'You are using entity type: {entity_type}. Please provide a file ID')
+
+    @staticmethod
+    def download_manifest(self, newManifestName: str="", manifest_df: pd.DataFrame=pd.DataFrame()) -> Union[str,File]:
+        """
+        Download a manifest based on a given manifest id. 
+        Args:
+            newManifestName(optional): new name of a manifest that gets downloaded.
+            manifest_df(optional): a dataframe containing name and id of manifests in a given asset view
+        Return: 
+            manifest_data: synapse entity file object
+        """
+
+        # enables retrying if user does not have access to uncensored manifest
+        # pass synID to synapseclient.Synapse.get() method to download (and overwrite) file to a location
+        manifest_data = ""
+
+        # check entity type
+        self._entity_type_checking()
+
+        # download a manifest
+        try:
+            manifest_data = self._download_manifest_to_folder()
+        except(SynapseUnmetAccessRestrictions, SynapseAuthenticationError):
+            # if there's an error getting an uncensored manifest, try getting the censored manifest
+            if not manifest_df.empty:
+                censored_regex=re.compile('.*censored.*')
+                censored = manifest_df['name'].str.contains(censored_regex)
+                new_manifest_id=manifest_df[censored]["id"][0]
+                self.manifest_id = new_manifest_id
+                try: 
+                    manifest_data = self._download_manifest_to_folder()
+                except (SynapseUnmetAccessRestrictions, SynapseAuthenticationError) as e:
+                    raise PermissionError("You don't have access to censored and uncensored manifests in this dataset.") from e
+            else:
+                logger.error(f"You don't have access to the requested resource: {self.manifest_id}")
+
+        if newManifestName and os.path.exists(manifest_data.get('path')):
+            # Rename the file we just made to the new name
+            new_manifest_filename = newManifestName + '.csv'
+
+            # get location of existing manifest. The manifest that will be renamed should live in the same folder as existing manifest.
+            parent_folder = os.path.dirname(manifest_data.get('path'))
+
+            new_manifest_path_name = os.path.join(parent_folder, new_manifest_filename)
+            os.rename(manifest_data['path'], new_manifest_path_name)
+
+            # Update file names/paths in manifest_data
+            manifest_data['name'] = new_manifest_filename
+            manifest_data['filename'] = new_manifest_filename
+            manifest_data['path'] = new_manifest_path_name
+        return manifest_data
 
 class SynapseStorage(BaseStorage):
     """Implementation of Storage interface for datasets/files stored on Synapse.
     Provides utilities to list files in a specific project; update files annotations, create fileviews, etc.
 
     TODO: Need to define the interface and rename and/or refactor some of the methods below.
     """
 
     def __init__(
         self,
         token: str = None,  # optional parameter retrieved from browser cookie
         access_token: str = None,
-        input_token: str = None,
         project_scope: List = None,
     ) -> None:
         """Initializes a SynapseStorage object.
         Args:
             syn: an object of type synapseclient.
             token: optional token parameter (typically a 'str') as found in browser cookie upon login to synapse.
             access_token: optional access token (personal or oauth)
@@ -74,15 +185,15 @@
             AttributeError: when the 'storageFileview' attribute (of class SynapseStorage) does not have a value associated with it.
             synapseclient.core.exceptions.SynapseHTTPError: check if the current user has permission to access the Synapse entity.
             ValueError: when Admin fileview cannot be found (describe further).
         Typical usage example:
             syn_store = SynapseStorage()
         """
 
-        self.syn = self.login(token, access_token, input_token)
+        self.syn = self.login(token, access_token)
         self.project_scope = project_scope
 
 
         # check if "master_fileview" has been set
         try: 
             self.storageFileview = CONFIG["synapse"]["master_fileview"]
         except KeyError: 
@@ -92,53 +203,81 @@
         try: 
             self.manifest = CONFIG["synapse"]["manifest_basename"]
         except KeyError: 
             raise MissingConfigValueError(("synapse", "manifest_basename"))
 
         self._query_fileview()
 
+    def _purge_synapse_cache(self, root_dir: str = "/var/www/.synapseCache/", maximum_storage_allowed_cache_gb=7):
+        """
+        Purge synapse cache if it exceeds 7GB
+        Args:
+            root_dir: directory of the .synapseCache function
+            maximum_storage_allowed_cache_gb: the maximum storage allowed before purging cache. Default is 7 GB. 
+
+        Returns: 
+            if size of cache reaches a certain threshold (default is 7GB), return the number of files that get deleted
+            otherwise, return the total remaining space (assuming total ephemeral storage is 20GB on AWS )
+        """
+        # try clearing the cache
+        # scan a directory and check size of files
+        cache = self.syn.cache
+        if os.path.exists(root_dir):
+            maximum_storage_allowed_cache_bytes = convert_gb_to_bytes(maximum_storage_allowed_cache_gb)
+            total_ephemeral_storag_gb = 20
+            total_ephemeral_storage_bytes = convert_gb_to_bytes(total_ephemeral_storag_gb)
+            nbytes = get_dir_size(root_dir)
+            # if 7 GB has already been taken, purge cache before 15 min
+            if nbytes >= maximum_storage_allowed_cache_bytes:
+                minutes_earlier = datetime.strftime(datetime.utcnow()- timedelta(minutes = 15), '%s')
+                num_of_deleted_files = cache.purge(before_date = int(minutes_earlier))
+                logger.info(f'{num_of_deleted_files} number of files have been deleted from {root_dir}')
+            else:
+                remaining_space = total_ephemeral_storage_bytes - nbytes
+                converted_space = convert_size(remaining_space)
+                logger.info(f'Estimated {remaining_space} bytes (which is approximately {converted_space}) remained in ephemeral storage after calculating size of .synapseCache excluding OS')
+
     def _query_fileview(self):
+        self._purge_synapse_cache()
         try:
             self.storageFileview = CONFIG["synapse"]["master_fileview"]
             self.manifest = CONFIG["synapse"]["manifest_basename"]
             if self.project_scope:
                 self.storageFileviewTable = self.syn.tableQuery(
                     f"SELECT * FROM {self.storageFileview} WHERE projectId IN {tuple(self.project_scope + [''])}"
-                ).asDataFrame()
+                    ).asDataFrame()
             else:
                 # get data in administrative fileview for this pipeline
                 self.storageFileviewTable = self.syn.tableQuery(
                     "SELECT * FROM " + self.storageFileview
                 ).asDataFrame()
+
         except AttributeError:
             raise AttributeError("storageFileview attribute has not been set.")
         except SynapseHTTPError:
-            raise AccessCredentialsError(self.storageFileview)        
+            raise AccessCredentialsError(self.storageFileview)    
 
     @staticmethod
-    def login(token=None, access_token=None, input_token=None):
+    def login(token=None, access_token=None):
         # If no token is provided, try retrieving access token from environment
-        if not token and not access_token and not input_token:
+        if not token and not access_token:
             access_token = os.getenv("SYNAPSE_ACCESS_TOKEN")
 
         # login using a token
         if token:
             syn = synapseclient.Synapse()
 
             try:
                 syn.login(sessionToken=token, silent=True)
             except synapseclient.core.exceptions.SynapseHTTPError:
                 raise ValueError("Please make sure you are logged into synapse.org.")
         elif access_token:
-            syn = synapseclient.Synapse()
-            syn.default_headers["Authorization"] = f"Bearer {access_token}"
-        elif input_token: 
-            try: 
+            try:
                 syn = synapseclient.Synapse()
-                syn.default_headers["Authorization"] = f"Bearer {input_token}"
+                syn.default_headers["Authorization"] = f"Bearer {access_token}"
             except synapseclient.core.exceptions.SynapseHTTPError:
                 raise ValueError("No access to resources. Please make sure that your token is correct")
         else:
             # login using synapse credentials provided by user in .synapseConfig (default) file
             syn = synapseclient.Synapse(configPath=CONFIG.SYNAPSE_CONFIG_PATH)
             syn.login(silent=True)
             
@@ -328,101 +467,87 @@
                         filename = (dirpath[0] + "/" + filename[0], filename[1])
 
                     # add file name file id tuple, rearranged so that id is first and name follows
                     file_list.append(filename[::-1])
 
         return file_list
 
+    def _get_manifest_id(self, manifest: pd.DataFrame) -> str:
+        """If both censored and uncensored manifests are present, return uncensored manifest; if only one manifest is present, return manifest id of that manifest; if more than two manifests are present, return the manifest id of the first one. 
+        Args:
+        manifest: a dataframe contains name and id of manifests in a given asset view
+
+        Return: 
+        manifest_syn_id: id of a given censored or uncensored manifest
+        """ 
+        censored_regex=re.compile('.*censored.*')
+        censored = manifest['name'].str.contains(censored_regex)
+        if any(censored):
+            # Try to use uncensored manifest first
+            not_censored=~censored
+            if any(not_censored):
+                manifest_syn_id=manifest[not_censored]["id"][0]
+            # if only censored manifests are available, just use the first censored manifest
+            else: 
+                manifest_syn_id = manifest["id"][0]
+
+        #otherwise, use the first (implied only) version that exists
+        else:
+            manifest_syn_id = manifest["id"][0]
+        
+        return manifest_syn_id
+
     def getDatasetManifest(
         self, datasetId: str, downloadFile: bool = False, newManifestName: str='',
-    ) -> List[str]:
+    ) -> Union[str, File]:
         """Gets the manifest associated with a given dataset.
 
         Args:
             datasetId: synapse ID of a storage dataset.
             downloadFile: boolean argument indicating if manifest file in dataset should be downloaded or not.
+            newManifestName: new name of a manifest that gets downloaded 
 
         Returns:
             manifest_syn_id (String): Synapse ID of exisiting manifest file.
             manifest_data (synapseclient.entity.File): Synapse entity if downloadFile is True.
             "" (String): No pre-exisiting manifest in dataset.
         """
+        manifest_data = ""
 
         # get a list of files containing the manifest for this dataset (if any)
         all_files = self.storageFileviewTable
 
+        # construct regex based on manifest basename in the config 
         manifest_re=re.compile(os.path.basename(self.manifest)+".*.[tc]sv")
+
+        # search manifest based on given manifest basename regex above
+        # and return a dataframe containing name and id of manifests in a given asset view
         manifest = all_files[
             (all_files['name'].str.contains(manifest_re,regex=True))
             & (all_files["parentId"] == datasetId)
         ]
 
         manifest = manifest[["id", "name"]]
-        censored_regex=re.compile('.*censored.*')
         
         # if there is no pre-exisiting manifest in the specified dataset
         if manifest.empty:
+            logger.warning(f"Could not find a manifest that fits basename {self.manifest} in asset view and dataset {datasetId}")
             return ""
 
         # if there is an exisiting manifest
         else:
-            # retrieve data from synapse
-
-            # if a censored manifest exists for this dataset
-            censored = manifest['name'].str.contains(censored_regex)
-            if any(censored):
-                # Try to use uncensored manifest first
-                not_censored=~censored
-                if any(not_censored):
-                    manifest_syn_id=manifest[not_censored]["id"][0]
-
-            #otherwise, use the first (implied only) version that exists
-            else:
-                manifest_syn_id = manifest["id"][0]
-
-
-            # if the downloadFile option is set to True
-            if downloadFile:
-                # enables retrying if user does not have access to uncensored manifest
-                while True:
-                    # pass synID to synapseclient.Synapse.get() method to download (and overwrite) file to a location
-                    try:
-                        if 'manifest_folder' in CONFIG['synapse'].keys():
-                            manifest_data = self.syn.get(
-                                manifest_syn_id,
-                                downloadLocation=CONFIG["synapse"]["manifest_folder"],
-                                ifcollision="overwrite.local",
-                            )
-                            break
-                        # if no manifest folder is set, download to cache
-                        else:
-                            manifest_data = self.syn.get(
-                                manifest_syn_id,
-                            )
-                            break
-                    # If user does not have access to uncensored manifest, use censored instead
-                    except(SynapseUnmetAccessRestrictions):
-                            manifest_syn_id=manifest[censored]["id"][0]
-                    
-                # Rename manifest file if indicated by user.
-                if newManifestName:
-                    if os.path.exists(manifest_data['path']):
-                        # Rename the file we just made to the new name
-                        new_manifest_filename = newManifestName + '.csv'
-                        new_manifest_path_name = manifest_data['path'].replace(manifest['name'][0], new_manifest_filename)
-                        os.rename(manifest_data['path'], new_manifest_path_name)
-
-                        # Update file names/paths in manifest_data
-                        manifest_data['name'] = new_manifest_filename
-                        manifest_data['filename'] = new_manifest_filename
-                        manifest_data['path'] = new_manifest_path_name
-
+            manifest_syn_id = self._get_manifest_id(manifest)
+            if downloadFile: 
+                md = ManifestDownload(self.syn, manifest_id=manifest_syn_id)
+                manifest_data = ManifestDownload.download_manifest(md, newManifestName=newManifestName, manifest_df=manifest)
+                ## TO DO: revisit how downstream code handle manifest_data. If the downstream code would break when manifest_data is an empty string, 
+                ## then we should catch the error here without returning an empty string. 
+                if not manifest_data:
+                    logger.debug(f"No manifest data returned. Please check if you have successfully downloaded manifest: {manifest_syn_id}")
                 return manifest_data
-
-
             return manifest_syn_id
 
     def getDataTypeFromManifest(self, manifestId:str):
         """Fetch a manifest and return data types of all columns
         Args: 
             manifestId: synapse ID of a manifest
         """
@@ -533,29 +658,33 @@
             manifestId = self.getDatasetManifest(datasetId)
 
             # If a manifest exists, get the annotations for it, else return base 'manifest' tuple
             if manifestId:
                 annotations = self.getFileAnnotations(manifestId)
 
                 # If manifest has annotations specifying component, use that
-                if 'Component' in annotations:
+                if annotations and 'Component' in annotations:
                     component = annotations['Component']
                     entity = self.syn.get(manifestId, downloadFile=False)
                     manifest_name = entity["properties"]["name"]
 
                 # otherwise download the manifest and parse for information
-                elif 'Component' not in annotations or not annotations:
+                elif not annotations or 'Component' not in annotations:
                     logging.debug(
                         f"No component annotations have been found for manifest {manifestId}. "
                         "The manifest will be downloaded and parsed instead. "
                         "For increased speed, add component annotations to manifest."
                         )
 
                     manifest_info = self.getDatasetManifest(datasetId,downloadFile=True)
-                    manifest_name = manifest_info["properties"]["name"]
+                    manifest_name = manifest_info["properties"].get("name", "")
+
+                    if not manifest_name:
+                        logger.error(f'Failed to download manifests from {datasetId}') 
+
                     manifest_path = manifest_info["path"]
 
                     manifest_df = load_df(manifest_path)
 
                     # Get component from component column if it exists
                     if "Component" in manifest_df and not manifest_df["Component"].empty:
                         list(set(manifest_df['Component']))
@@ -567,17 +696,18 @@
 
                         if len(component) == 1:
                             component = component[0]
                         elif len(component) > 1:
                             logging.warning(
                             f"Manifest {manifestId} is composed of multiple components. Schematic does not support mulit-component manifests at this time."
                             "Behavior of manifests with multiple components is undefined"
-                            )              
-
-            #save manifest list with applicable informaiton
+                            )
+            else:
+                manifest_name = ""
+                component = None              
             if component:
                 manifest = (
                     (datasetId, datasetName),
                     (manifestId, manifest_name),
                     (component, component),
                 )
             elif manifestId:
@@ -617,15 +747,15 @@
 
             manifest_info = self.getDatasetManifest(datasetId, downloadFile=True)
             if manifest_info:
                 manifest_id = manifest_info["properties"]["id"]
                 manifest_name = manifest_info["properties"]["name"]
                 manifest_path = manifest_info["path"]
                 manifest_df = load_df(manifest_path)
-                manifest_table_id = upload_format_manifest_table(manifest, datasetId, datasetName)
+                manifest_table_id = uploadDB(manifest, datasetId, datasetName)
                 manifest_loaded.append(datasetName)
         return manifest_loaded
 
     def upload_annotated_project_manifests_to_synapse(self, projectId:str, path_to_json_ld: str, dry_run: bool = False) -> List[str]:
         '''
         Purpose:
             For all manifests in a project, upload them as a table and add annotations manifest csv.
@@ -746,26 +876,74 @@
         tables = self._get_tables(datasetId = datasetId, projectId = projectId)
         if tables:
             return {table["name"]: table["id"] for table in tables}
         else: 
             return {None:None}
 
     @missing_entity_handler
-    def upload_format_manifest_table(self, se, manifest, datasetId, table_name, restrict, useSchemaLabel):
+    def uploadDB(self, 
+        sg: SchemaGenerator, 
+        manifest: pd.DataFrame, 
+        datasetId: str, 
+        table_name: str, 
+        restrict: bool = False, 
+        useSchemaLabel: bool = True, 
+        table_manipulation: str = 'replace',
+        ):
+        """
+        Method to upload a database to an asset store. In synapse, this will upload a metadata table
+        
+        Args:
+            se: schemaExplorer object
+            manifest: pd.Df manifest to upload
+            datasetId: synID of the dataset for the manifest
+            table_name: name of the table to be uploaded
+            restrict: bool, whether or not the manifest contains sensitive data that will need additional access restrictions 
+            useSchemaLabel: bool whether to use schemaLabel (True) or display label (False)
+            existingTableId: str of the synId of the existing table, if one already exists
+            table_manipulation: str, 'replace' or 'upsert', in the case where a manifest already exists, should the new metadata replace the existing (replace) or be added to it (upsert)
+
+        Returns:
+            manifest_table_id: synID of the uploaded table
+            manifest: the original manifset
+            table_manifest: manifest formatted appropriately for the table
+        
+        """
+        
+
+        col_schema, table_manifest = self.formatDB(sg, manifest, useSchemaLabel)
+
+        manifest_table_id = self.buildDB(datasetId, table_name, col_schema, table_manifest, table_manipulation, sg, restrict,)
+
+        return manifest_table_id, manifest, table_manifest
+
+    def formatDB(self, sg, manifest, useSchemaLabel):
+        """
+        Method to format a manifest appropriatly for upload as table
+        
+        Args:
+            se: schemaExplorer object
+            manifest: pd.Df manifest to upload
+            useSchemaLabel: bool whether to use schemaLabel (True) or display label (False)
+
+        Returns:
+            col_schema: schema for table columns: type, size, etc
+            table_manifest: formatted manifest
+        
+        """
         # Rename the manifest columns to display names to match fileview
-        table_info = self.get_table_info(datasetId = datasetId)
 
         blacklist_chars = ['(', ')', '.', ' ', '-']
         manifest_columns = manifest.columns.tolist()
 
         table_manifest=deepcopy(manifest)
 
         if useSchemaLabel:
             cols = [
-                se.get_class_label_from_display_name(
+                sg.se.get_class_label_from_display_name(
                     str(col)
                     ).translate({ord(x): '' for x in blacklist_chars})
                 for col in manifest_columns
             ]
 
             cols = list(map(lambda x: x.replace('EntityId', 'entityId'), cols))
 
@@ -776,42 +954,76 @@
         #move entity id to end of df
         entity_col = table_manifest.pop('entityId')
         table_manifest.insert(len(table_manifest.columns), 'entityId', entity_col)
 
         # Get the column schema
         col_schema = as_table_columns(table_manifest)
 
-        # Set uuid column length to 64 (for some reason not being auto set.)
+        # Set Id column length to 64 (for some reason not being auto set.)
         for i, col in enumerate(col_schema):
-            if col['name'] == 'Uuid':
+            if col['name'].lower() == 'id':
                 col_schema[i]['maximumSize'] = 64
 
+        return col_schema, table_manifest
+
+    def buildDB(self,  
+        datasetId: str, 
+        table_name: str, 
+        col_schema: List,
+        table_manifest: pd.DataFrame,
+        table_manipulation: str,
+        sg: SchemaGenerator,  
+        restrict: bool = False,
+        
+        ):
+        """
+        Method to construct the table appropriately: create new table, replace existing, or upsert new into existing
+        Calls TableOperations class to execute 
+        
+        Args:
+            datasetId: synID of the dataset for the manifest
+            table_name: name of the table to be uploaded
+            col_schema: schema for table columns: type, size, etc from `formatDB`
+            table_manifest: formatted manifest that can be uploaded as a table
+            table_manipulation: str, 'replace' or 'upsert', in the case where a manifest already exists, should the new metadata replace the existing (replace) or be added to it (upsert)
+            restrict: bool, whether or not the manifest contains sensitive data that will need additional access restrictions 
+
+        Returns:
+            manifest_table_id: synID of the uploaded table
+        
+        """
+        table_info = self.get_table_info(datasetId = datasetId)
         # Put table manifest onto synapse
         schema = Schema(name=table_name, columns=col_schema, parent=self.getDatasetProject(datasetId))
-        if table_name not in table_info.keys():
-            manifest_table_id = self.make_synapse_table(table_to_load = table_manifest, 
-                                    dataset_id = datasetId,
-                                    existingTableId = None, 
-                                    table_name = table_name, 
-                                    column_type_dictionary = col_schema, 
-                                    restrict = restrict,
-                                    manipulation = 'replace')
-        else:
-            manifest_table_id = self.make_synapse_table(table_to_load = table_manifest, 
-                                    dataset_id = datasetId,
-                                    existingTableId = table_info[table_name], 
-                                    table_name = table_name, 
-                                    column_type_dictionary = col_schema,
-                                    restrict = restrict,
-                                    manipulation = 'replace')
 
+        
+        if not table_manipulation or table_name not in table_info.keys():
+            manifest_table_id = TableOperations.createTable(self, tableToLoad=table_manifest, tableName=table_name, datasetId=datasetId, columnTypeDict=col_schema, specifySchema=True, restrict=restrict)
+        elif table_name in table_info.keys() and table_info[table_name]:
+
+            if table_manipulation.lower() == 'replace':
+                manifest_table_id = TableOperations.replaceTable(self, tableToLoad=table_manifest, tableName=table_name, existingTableId=table_info[table_name], specifySchema = True, datasetId = datasetId, columnTypeDict=col_schema, restrict=restrict)
+            elif table_manipulation.lower() == 'upsert':
+                manifest_table_id = TableOperations.upsertTable(self, sg=sg, tableToLoad = table_manifest, tableName=table_name, existingTableId=table_info[table_name], datasetId=datasetId)
+            elif table_manipulation.lower() == 'update':
+                manifest_table_id = TableOperations.updateTable(self, tableToLoad=table_manifest, existingTableId=table_info[table_name], restrict=restrict)
 
-        return manifest_table_id, manifest, table_manifest
 
-    def uplodad_manifest_file(self, manifest, metadataManifestPath, datasetId, restrict_manifest, component_name = ''):
+
+        if table_manipulation and table_manipulation.lower() == 'upsert':
+            existing_tables=self.get_table_info(datasetId=datasetId)
+            tableId=existing_tables[table_name]
+            annos = self.syn.get_annotations(tableId)
+            annos['primary_key'] = table_manifest['Component'][0] + "_id"
+            annos = self.syn.set_annotations(annos)
+
+        return manifest_table_id
+
+
+    def upload_manifest_file(self, manifest, metadataManifestPath, datasetId, restrict_manifest, component_name = ''):
         # Update manifest to have the new entityId column
         manifest.to_csv(metadataManifestPath, index=False)
 
         # store manifest to Synapse as a CSV
         # update file name
         file_name_full = metadataManifestPath.split('/')[-1]
         file_extension = file_name_full.split('.')[-1]
@@ -859,15 +1071,14 @@
             # add an explicit [truncatedByDataCuratorApp] message at the end
             # of every truncated message to indicate that the cell value
             # has been truncated
             if isinstance(v, str) and len(v) >= 500:
                 v = v[0:472] + "[truncatedByDataCuratorApp]"
 
             metadataSyn[keySyn] = v
-        
         # set annotation(s) for the various objects/items in a dataset on Synapse
         annos = self.syn.get_annotations(entityId)
         csv_list_regex=comma_separated_list_regex()
         for anno_k, anno_v in metadataSyn.items():
             
             # Remove keys with nan or empty string values from dict of annotations to be uploaded
             # if present on current data annotation
@@ -976,15 +1187,15 @@
                 row["entityId"] = manifest_synapse_table_id
                 entityId = ''
             else:
                 # get the entity id corresponding to this row
                 entityId = row["entityId"]
 
         # Load manifest to synapse as a CSV File
-        manifest_synapse_file_id = self.uplodad_manifest_file(manifest, metadataManifestPath, datasetId, restrict_manifest)
+        manifest_synapse_file_id = self.upload_manifest_file(manifest, metadataManifestPath, datasetId, restrict_manifest)
         
         # Get annotations for the file manifest.
         manifest_annotations = self.format_manifest_annotations(manifest, manifest_synapse_file_id)
         
         self.syn.set_annotations(manifest_annotations)
 
         logger.info("Associated manifest file with dataset on Synapse.")
@@ -1001,155 +1212,449 @@
         
         # Get annotations for the table manifest
         manifest_annotations = self.format_manifest_annotations(manifest, manifest_synapse_table_id)
         self.syn.set_annotations(manifest_annotations)
         return manifest_synapse_table_id
     '''
 
-    def associateMetadataWithFiles(
-        self, schemaGenerator: SchemaGenerator, metadataManifestPath: str, datasetId: str, manifest_record_type: str = 'both', 
-        useSchemaLabel: bool = True, hideBlanks: bool = False, restrict_manifest = False,
-    ) -> str:
-        """Associate metadata with files in a storage dataset already on Synapse.
-        Upload metadataManifest in the storage dataset folder on Synapse as well. Return synapseId of the uploaded manifest file.
-        
-        If this is a new manifest there could be no Synapse entities associated with the rows of this manifest
-        this may be due to data type (e.g. clinical data) being tabular
-        and not requiring files; to utilize uniform interfaces downstream
-        (i.e. fileviews), a Synapse entity (a folder) is created for each row
-        and an entity column is added to the manifest containing the resulting
-        entity IDs; a table is also created at present as an additional interface
-        for downstream query and interaction with the data.
-
+    def _read_manifest(self, metadataManifestPath:str) -> pd.DataFrame:
+        """Helper function to read in provided manifest as a pandas DataFrame for subsequent downstream processing.
         Args:
-            metadataManifestPath: path to csv containing a validated metadata manifest.
-            The manifest should include a column entityId containing synapse IDs of files/entities to be associated with metadata, if that is applicable to the dataset type.
-            Some datasets, e.g. clinical data, do not contain file id's, but data is stored in a table: one row per item.
-            In this case, the system creates a file on Synapse for each row in the table (e.g. patient, biospecimen) and associates the columnset data as metadata/annotations to his file.
-            datasetId: synapse ID of folder containing the dataset
-            useSchemaLabel: Default is True - use the schema label. If False, uses the display label from the schema. Attribute display names in the schema must not only include characters that are not accepted by Synapse. Annotation names may only contain: letters, numbers, '_' and '.'.
-            manifest_record_type: valid values are 'entity', 'table' or 'both'. Specifies whether to create entity ids and folders for each row in a manifest, a Synapse table to house the entire manifest or do both.
-            hideBlanks: Default is false. Boolean flag that does not upload annotation keys with blank values when true. Uploads Annotation keys with empty string values when false.
+            metadataManifestPath (str): path where manifest is stored
         Returns:
-            manifest_synapse_file_id: SynID of manifest csv uploaded to synapse.
-
+            manifest(pd.DataFrame): Manifest loaded as a pandas dataframe
         Raises:
-            ValueError: manifest_record_type is not 'entity', 'table' or 'both'
             FileNotFoundError: Manifest file does not exist at provided path.
-
         """
-
-        # Check that record type provided matches expected input.
-        manifest_record_types = ['entity', 'table', 'both']
-        try:
-            manifest_record_type in manifest_record_types
-        except ValueError as err:
-            raise ValueError(
-                f"manifest_record_type provided: {manifest_record_type}, is not one of the accepted "
-                f"types: {manifest_record_types}"
-            ) from err
-
         # read new manifest csv
         try:
             load_args={
                 "dtype":"string",
             }
-            manifest = load_df(metadataManifestPath, preserve_raw_input = True, **load_args) #HOTFIX: set preserve_raw_input to true to allow mixed type cols in table uploads schematic#870
+            manifest = load_df(metadataManifestPath, preserve_raw_input = False, **load_args)
         except FileNotFoundError as err:
             raise FileNotFoundError(
                 f"No manifest file was found at this path: {metadataManifestPath}"
             ) from err
+        return manifest
 
-        # Add uuid for table updates and fill.
-        if not "Uuid" in manifest.columns:
-            manifest["Uuid"] = ''
+    def _add_id_columns_to_manifest(self, manifest: pd.DataFrame, sg: SchemaGenerator):
+        """Helper function to add id and entityId columns to the manifest if they do not already exist, Fill id values per row.
+        Args:
+            Manifest loaded as a pd.Dataframe
+        Returns (pd.DataFrame):
+            Manifest df with new Id and EntityId columns (and UUID values) if they were not already present.
+        """
+
+        # Add Id for table updates and fill.
+        if not col_in_dataframe("Id", manifest):
+            # See if schema has `Uuid` column specified
+            try:
+                uuid_col_in_schema = sg.se.is_class_in_schema('Uuid') or sg.se.is_class_in_schema('uuid')      
+            except (KeyError):
+                uuid_col_in_schema = False
+
+            # Rename `Uuid` column if it wasn't specified in the schema
+            if col_in_dataframe("Uuid", manifest) and not uuid_col_in_schema:
+                manifest.rename(columns={'Uuid': 'Id'}, inplace=True)
+            # If no `Uuid` column exists or it is specified in the schema, create a new `Id` column
+            else:
+                manifest["Id"] = ''
 
         for idx,row in manifest.iterrows():
-            if not row["Uuid"]:
+            if not row["Id"]:
                 gen_uuid = str(uuid.uuid4())
-                row["Uuid"] = gen_uuid
-                manifest.loc[idx, 'Uuid'] = gen_uuid
+                row["Id"] = gen_uuid
+                manifest.loc[idx, 'Id'] = gen_uuid
 
         # add entityId as a column if not already there or
         # fill any blanks with an empty string.
-        if not "entityId" in manifest.columns:
+        if not col_in_dataframe("entityId", manifest):
             manifest["entityId"] = ""
         else:
             manifest["entityId"].fillna("", inplace=True)
 
-        # get a schema explorer object to ensure schema attribute names used in manifest are translated to schema labels for synapse annotations
-        se = SchemaExplorer()
+        return manifest
 
+    def _generate_table_name(self, manifest):
+        """Helper function to generate a table name for upload to synapse.
+        Args:
+            Manifest loaded as a pd.Dataframe
+        Returns:
+            table_name (str): Name of the table to load
+            component_name (str): Name of the manifest component (if applicable)
+        """
         # Create table name here.
         if 'Component' in manifest.columns:
             component_name = manifest['Component'][0].lower()
             table_name = component_name + '_synapse_storage_manifest_table'
         else:
             component_name = ''
             table_name = 'synapse_storage_manifest_table'
+        return table_name, component_name
 
-        # If specified, upload manifest as a table and get the SynID and manifest
-        if manifest_record_type == 'table' or manifest_record_type == 'both':
-            manifest_synapse_table_id, manifest, table_manifest = self.upload_format_manifest_table(
-                                                        se, manifest, datasetId, table_name, restrict = restrict_manifest, useSchemaLabel=useSchemaLabel)
-            
-        # Iterate over manifest rows, create Synapse entities and store corresponding entity IDs in manifest if needed
-        # also set metadata for each synapse entity as Synapse annotations
+    def _add_annotations(self, se, schemaGenerator, row, entityId, useSchemaLabel, hideBlanks):
+        """Helper function to format and add annotations to entities in Synapse.
+        Args:
+            se: schemaExplorer object,
+            schemaGenerator: schemaGenerator Object.
+            row: current row of manifest being processed
+            entityId (str): synapseId of entity to add annotations to
+            useSchemaLabel (bool): Flag to use schema label instead of display name
+            hideBlanks: Boolean flag that does not upload annotation keys with blank values when true. Uploads Annotation keys with empty string values when false.
+        Returns:
+            Annotations are added to entities in Synapse, no return.
+        """
+        # Format annotations for Synapse
+        annos = self.format_row_annotations(se, schemaGenerator, row, entityId, useSchemaLabel, hideBlanks)
+
+        if annos:
+        # Store annotations for an entity folder
+            self.syn.set_annotations(annos)
+        return
+
+    def _create_entity_id(self, idx, row, manifest, datasetId):
+        """Helper function to generate an entityId and add it to the appropriate row in the manifest.
+        Args:
+            row: current row of manifest being processed
+            manifest (pd.DataFrame): loaded df containing user supplied data.
+            datasetId (str): synapse ID of folder containing the dataset
+
+        Returns:
+            manifest (pd.DataFrame): manifest with entityId added to the appropriate row
+            entityId (str): Generated Entity Id.
+        
+        """
+        rowEntity = Folder(str(uuid.uuid4()), parent=datasetId)
+        rowEntity = self.syn.store(rowEntity)
+        entityId = rowEntity["id"]
+        row["entityId"] = entityId
+        manifest.loc[idx, "entityId"] = entityId
+        return manifest, entityId
+
+    def add_entities(
+                    self,
+                    se,
+                    schemaGenerator,
+                    manifest,
+                    manifest_record_type,
+                    datasetId,
+                    useSchemaLabel,
+                    hideBlanks,
+                    manifest_synapse_table_id=''
+                    ):
+        '''Depending on upload type add Ids to entityId row. Add anotations to connected files.
+        Args:
+            se: Schema Explorer Object
+            schemaGenerator: SchemaGenerator object
+            manifest (pd.DataFrame): loaded df containing user supplied data.
+            manifest_record_type: valid values are 'entity', 'table' or 'both'. Specifies whether to create entity ids and folders for each row in a manifest, a Synapse table to house the entire manifest or do both.
+            datasetId (str): synapse ID of folder containing the dataset
+            useSchemaLabel (bool): Default is True - use the schema label. If False, uses the display label from the schema. Attribute display names in the schema must not only include characters that are not accepted by Synapse. Annotation names may only contain: letters, numbers, '_' and '.'.
+            hideBlanks (bool): Default is false -Boolean flag that does not upload annotation keys with blank values when true. Uploads Annotation keys with empty string values when false.
+            manifest_synapse_table_id (str): Default is an empty string ''.
+        Returns:
+            manifest (pd.DataFrame): modified to add entitiyId as appropriate.
+
+        '''
         for idx, row in manifest.iterrows():
-            if not row["entityId"] and (manifest_record_type == 'entity' or 
-                manifest_record_type == 'both'):
-                # no entity exists for this row
-                # so create one
-                rowEntity = Folder(str(uuid.uuid4()), parent=datasetId)
-                rowEntity = self.syn.store(rowEntity)
-                entityId = rowEntity["id"]
-                row["entityId"] = entityId
-                manifest.loc[idx, "entityId"] = entityId
-            elif not row["entityId"] and manifest_record_type == 'table':
+            if not row["entityId"] and (manifest_record_type == 'file_and_entities' or 
+                manifest_record_type == 'table_file_and_entities'):
+                manifest, entityId = self._create_entity_id(idx, row, manifest, datasetId)
+            elif not row["entityId"] and manifest_record_type == 'table_and_file':
                 # If not using entityIds, fill with manifest_table_id so 
                 row["entityId"] = manifest_synapse_table_id
+                manifest.loc[idx, "entityId"] = manifest_synapse_table_id
                 entityId = ''
             else:
                 # get the entity id corresponding to this row
                 entityId = row["entityId"]
 
             # Adding annotations to connected files.
             if entityId:
-                # Format annotations for Synapse
-                annos = self.format_row_annotations(se, schemaGenerator, row, entityId, useSchemaLabel, hideBlanks)
+                self._add_annotations(se, schemaGenerator, row, entityId, useSchemaLabel, hideBlanks)
+        return manifest
 
-                if annos:
-                # Store annotations for an entity folder
-                    self.syn.set_annotations(annos)
+    def upload_manifest_as_table(
+                            self,
+                            se,
+                            schemaGenerator,
+                            manifest,
+                            metadataManifestPath,
+                            datasetId,
+                            table_name,
+                            component_name,
+                            restrict,
+                            manifest_record_type,
+                            useSchemaLabel,
+                            hideBlanks,
+                            table_manipulation,
+                            ):
+        """Upload manifest to Synapse as a table and csv.
+        Args:
+            se: SchemaExplorer object
+            schemaGenerator: SchemaGenerator Object
+            manifest (pd.DataFrame): loaded df containing user supplied data.
+            metadataManifestPath: path to csv containing a validated metadata manifest.
+            datasetId (str): synapse ID of folder containing the dataset
+            table_name (str): Generated to name the table being uploaded.
+            component_name (str): Name of the component manifest that is currently being uploaded.
+            restrict (bool): Flag for censored data.
+            manifest_record_type (str): valid values are 'entity', 'table' or 'both'. Specifies whether to create entity ids and folders for each row in a manifest, a Synapse table to house the entire manifest or do both.
+            useSchemaLabel(bool): Default is True - use the schema label. If False, uses the display label from the schema. Attribute display names in the schema must not only include characters that are not accepted by Synapse. Annotation names may only contain: letters, numbers, '_' and '.'.
+            hideBlanks (bool): Default is False -Boolean flag that does not upload annotation keys with blank values when true. Uploads Annotation keys with empty string values when false.
+            table_malnipulation (str): Specify the way the manifest tables should be store as on Synapse when one with the same name already exists. Options are 'replace' and 'upsert'.
+        Return:
+            manifest_synapse_file_id: SynID of manifest csv uploaded to synapse.
+        """      
+        # Upload manifest as a table, get the ID and updated manifest.
+        manifest_synapse_table_id, manifest, table_manifest = self.uploadDB(
+                                                    schemaGenerator,
+                                                    manifest,
+                                                    datasetId,
+                                                    table_name,
+                                                    restrict,
+                                                    useSchemaLabel,
+                                                    table_manipulation)
+
+        manifest = self.add_entities(se, schemaGenerator, manifest, manifest_record_type, datasetId, useSchemaLabel, hideBlanks, manifest_synapse_table_id)
+        # Load manifest to synapse as a CSV File
+        manifest_synapse_file_id = self.upload_manifest_file(manifest, metadataManifestPath, datasetId, restrict, component_name = component_name)
+        
+        # Set annotations for the file manifest.
+        manifest_annotations = self.format_manifest_annotations(manifest, manifest_synapse_file_id)
+        self.syn.set_annotations(manifest_annotations)
+        logger.info("Associated manifest file with dataset on Synapse.")
+        
+        # Update manifest Synapse table with new entity id column.
+        manifest_synapse_table_id, manifest, table_manifest = self.uploadDB(
+                                                    schemaGenerator,
+                                                    manifest, 
+                                                    datasetId, 
+                                                    table_name,  
+                                                    restrict,
+                                                    useSchemaLabel=useSchemaLabel,
+                                                    table_manipulation='update',)
+
+        # Set annotations for the table manifest
+        manifest_annotations = self.format_manifest_annotations(manifest, manifest_synapse_table_id)
+        self.syn.set_annotations(manifest_annotations)
+        return manifest_synapse_file_id
+
+    def upload_manifest_as_csv(
+                            self,
+                            se,
+                            schemaGenerator,
+                            manifest,
+                            metadataManifestPath,
+                            datasetId,
+                            restrict,
+                            manifest_record_type,
+                            useSchemaLabel,
+                            hideBlanks,
+                            component_name,
+                            with_entities = False,):
+        """Upload manifest to Synapse as a csv only.
+        Args:
+            se: SchemaExplorer object
+            schemaGenerator: SchemaGenerator Object
+            manifest (pd.DataFrame): loaded df containing user supplied data.
+            metadataManifestPath: path to csv containing a validated metadata manifest.
+            datasetId (str): synapse ID of folder containing the dataset
+            restrict (bool): Flag for censored data.
+            manifest_record_type: valid values are 'entity', 'table' or 'both'. Specifies whether to create entity ids and folders for each row in a manifest, a Synapse table to house the entire manifest or do both.
+            useSchemaLabel (bool): Default is True - use the schema label. If False, uses the display label from the schema. Attribute display names in the schema must not only include characters that are not accepted by Synapse. Annotation names may only contain: letters, numbers, '_' and '.'.
+            hideBlanks (bool): Default is False -Boolean flag that does not upload annotation keys with blank values when true. Uploads Annotation keys with empty string values when false.
+            table_malnipulation (str): Specify the way the manifest tables should be store as on Synapse when one with the same name already exists. Options are 'replace' and 'upsert'.
+            with_entities (bool): Default is False - Flag to indicate whether to create entityIds and add annotations.
+        Return:
+            manifest_synapse_file_id (str): SynID of manifest csv uploaded to synapse.
+        """
+        if with_entities:
+            manifest = self.add_entities(se, schemaGenerator, manifest, manifest_record_type, datasetId, useSchemaLabel, hideBlanks)
 
         # Load manifest to synapse as a CSV File
-        manifest_synapse_file_id = self.uplodad_manifest_file(manifest, metadataManifestPath, datasetId, restrict_manifest, component_name = component_name)
+        manifest_synapse_file_id = self.upload_manifest_file(manifest,
+                metadataManifestPath, datasetId, restrict, component_name = component_name)
         
         # Set annotations for the file manifest.
         manifest_annotations = self.format_manifest_annotations(manifest, manifest_synapse_file_id)
         self.syn.set_annotations(manifest_annotations)
 
         logger.info("Associated manifest file with dataset on Synapse.")
         
-        if manifest_record_type == 'table' or manifest_record_type == 'both':
-            # Update manifest Synapse table with new entity id column.
-            self.make_synapse_table(
-                table_to_load = table_manifest,
-                dataset_id = datasetId,
-                existingTableId = manifest_synapse_table_id,
-                table_name = table_name,
-                update_col = 'Uuid',
-                specify_schema = False,
-                restrict = restrict_manifest
-                )
-            
-            # Set annotations for the table manifest
-            manifest_annotations = self.format_manifest_annotations(manifest, manifest_synapse_table_id)
-            self.syn.set_annotations(manifest_annotations)
+        return manifest_synapse_file_id
 
+    def upload_manifest_combo(
+                            self,
+                            se,
+                            schemaGenerator,
+                            manifest,
+                            metadataManifestPath,
+                            datasetId,
+                            table_name,
+                            component_name,
+                            restrict,
+                            manifest_record_type,
+                            useSchemaLabel,
+                            hideBlanks,
+                            table_manipulation,
+                            ):
+        """Upload manifest to Synapse as a table and CSV with entities.
+        Args:
+            se: SchemaExplorer object
+            schemaGenerator: SchemaGenerator Object
+            manifest (pd.DataFrame): loaded df containing user supplied data.
+            metadataManifestPath: path to csv containing a validated metadata manifest.
+            datasetId (str): synapse ID of folder containing the dataset
+            table_name (str): Generated to name the table being uploaded.
+            component_name (str): Name of the component manifest that is currently being uploaded.
+            restrict (bool): Flag for censored data.
+            manifest_record_type: valid values are 'entity', 'table' or 'both'. Specifies whether to create entity ids and folders for each row in a manifest, a Synapse table to house the entire manifest or do both.
+            useSchemaLabel (bool): Default is True - use the schema label. If False, uses the display label from the schema. Attribute display names in the schema must not only include characters that are not accepted by Synapse. Annotation names may only contain: letters, numbers, '_' and '.'.
+            hideBlanks (bool): Default is False -Boolean flag that does not upload annotation keys with blank values when true. Uploads Annotation keys with empty string values when false.
+            table_malnipulation (str): Specify the way the manifest tables should be store as on Synapse when one with the same name already exists. Options are 'replace' and 'upsert'.
+        Return:
+            manifest_synapse_file_id (str): SynID of manifest csv uploaded to synapse.
+        """
+        manifest_synapse_table_id, manifest, table_manifest = self.uploadDB(
+                                                    se,
+                                                    manifest,
+                                                    datasetId,
+                                                    table_name,
+                                                    restrict,
+                                                    useSchemaLabel=useSchemaLabel,
+                                                    table_manipulation=table_manipulation,)
+
+        manifest = self.add_entities(se, schemaGenerator, manifest, manifest_record_type, datasetId, useSchemaLabel, hideBlanks, manifest_synapse_table_id)
+        
+        # Load manifest to synapse as a CSV File
+        manifest_synapse_file_id = self.upload_manifest_file(manifest, metadataManifestPath, datasetId, restrict, component_name)
+        
+        # Set annotations for the file manifest.
+        manifest_annotations = self.format_manifest_annotations(manifest, manifest_synapse_file_id)
+        self.syn.set_annotations(manifest_annotations)
+        logger.info("Associated manifest file with dataset on Synapse.")
+        
+        # Update manifest Synapse table with new entity id column.
+        manifest_synapse_table_id, manifest, table_manifest = self.uploadDB(
+                                                                se,
+                                                                manifest,
+                                                                datasetId,
+                                                                table_name,
+                                                                restrict,
+                                                                useSchemaLabel=useSchemaLabel,
+                                                                table_manipulation='update',)
+
+        # Set annotations for the table manifest
+        manifest_annotations = self.format_manifest_annotations(manifest, manifest_synapse_table_id)
+        self.syn.set_annotations(manifest_annotations)
+        return manifest_synapse_file_id
+
+    def associateMetadataWithFiles(
+        self, schemaGenerator: SchemaGenerator, metadataManifestPath: str, datasetId: str, manifest_record_type: str = 'table_file_and_entities', 
+        useSchemaLabel: bool = True, hideBlanks: bool = False, restrict_manifest = False, table_manipulation: str = 'replace',
+    ) -> str:
+        """Associate metadata with files in a storage dataset already on Synapse.
+        Upload metadataManifest in the storage dataset folder on Synapse as well. Return synapseId of the uploaded manifest file.
+        
+        If this is a new manifest there could be no Synapse entities associated with the rows of this manifest
+        this may be due to data type (e.g. clinical data) being tabular
+        and not requiring files; to utilize uniform interfaces downstream
+        (i.e. fileviews), a Synapse entity (a folder) is created for each row
+        and an entity column is added to the manifest containing the resulting
+        entity IDs; a table is also created at present as an additional interface
+        for downstream query and interaction with the data.
+
+        Args:
+            schemaGenerator: SchemaGenerator Object
+            metadataManifestPath: path to csv containing a validated metadata manifest.
+            The manifest should include a column entityId containing synapse IDs of files/entities to be associated with metadata, if that is applicable to the dataset type.
+            Some datasets, e.g. clinical data, do not contain file id's, but data is stored in a table: one row per item.
+            In this case, the system creates a file on Synapse for each row in the table (e.g. patient, biospecimen) and associates the columnset data as metadata/annotations to his file.
+            datasetId: synapse ID of folder containing the dataset
+            manifest_record_type: Default value is 'table_file_and_entities'. valid values are 'file_only', 'file_and_entities', 'table_and_file' or 'table_file_and_entities'. 'file_and_entities' will store the manifest as a csv and create Synapse files for each row in the manifest.'table_and_file' will store the manifest as a table and a csv on Synapse. 'file_only' will store the manifest as a csv only on Synapse. 'table_file_and_entities' will perform the options file_with_entites and table in combination.
+            useSchemaLabel: Default is True - use the schema label. If False, uses the display label from the schema. Attribute display names in the schema must not only include characters that are not accepted by Synapse. Annotation names may only contain: letters, numbers, '_' and '.'.
+            hideBlanks: Default is false. Boolean flag that does not upload annotation keys with blank values when true. Uploads Annotation keys with empty string values when false.
+            restrict_manifest (bool): Default is false. Flag for censored data.
+            table_malnipulation (str): Default is 'replace'. Specify the way the manifest tables should be store as on Synapse when one with the same name already exists. Options are 'replace' and 'upsert'.
+        Returns:
+            manifest_synapse_file_id: SynID of manifest csv uploaded to synapse.
+        """
+        # Read new manifest CSV:
+        manifest = self._read_manifest(metadataManifestPath)
+        manifest = self._add_id_columns_to_manifest(manifest, schemaGenerator)
+
+        # get a schema explorer object to ensure schema attribute names used in manifest are translated to schema labels for synapse annotations
+        se = SchemaExplorer()
+
+        table_name, component_name = self._generate_table_name(manifest)
+
+        # Upload manifest to synapse based on user input (manifest_record_type)
+        
+        if manifest_record_type == "file_only":
+            manifest_synapse_file_id = self.upload_manifest_as_csv(
+                                        se,
+                                        schemaGenerator,
+                                        manifest,
+                                        metadataManifestPath,
+                                        datasetId=datasetId,
+                                        restrict=restrict_manifest,
+                                        useSchemaLabel=useSchemaLabel,
+                                        hideBlanks=hideBlanks,
+                                        manifest_record_type=manifest_record_type,
+                                        component_name = component_name,
+                                        with_entities = False,
+                                        )
+        elif manifest_record_type == "table_and_file":
+            manifest_synapse_file_id = self.upload_manifest_as_table(
+                                        se,
+                                        schemaGenerator,
+                                        manifest,
+                                        metadataManifestPath,
+                                        datasetId=datasetId,
+                                        table_name=table_name,
+                                        component_name=component_name,
+                                        restrict=restrict_manifest,
+                                        useSchemaLabel=useSchemaLabel,
+                                        hideBlanks=hideBlanks,
+                                        manifest_record_type=manifest_record_type,
+                                        table_manipulation=table_manipulation,
+                                        )
+        elif manifest_record_type == "file_and_entities":
+            manifest_synapse_file_id = self.upload_manifest_as_csv( 
+                                        se,
+                                        schemaGenerator,
+                                        manifest,
+                                        metadataManifestPath,
+                                        datasetId=datasetId,
+                                        restrict=restrict_manifest,
+                                        useSchemaLabel=useSchemaLabel,
+                                        hideBlanks=hideBlanks,
+                                        manifest_record_type=manifest_record_type,
+                                        component_name = component_name,
+                                        with_entities=True,
+                                        )
+        elif manifest_record_type == "table_file_and_entities":
+            manifest_synapse_file_id = self.upload_manifest_combo(
+                                        se,
+                                        schemaGenerator,
+                                        manifest,
+                                        metadataManifestPath,
+                                        datasetId=datasetId,
+                                        table_name=table_name,
+                                        component_name=component_name,
+                                        restrict=restrict_manifest,
+                                        useSchemaLabel=useSchemaLabel,
+                                        hideBlanks=hideBlanks,
+                                        manifest_record_type=manifest_record_type,
+                                        table_manipulation=table_manipulation,
+                                        )
+        else:
+            raise ValueError("Please enter a valid manifest_record_type.")
         return manifest_synapse_file_id
 
     def getTableAnnotations(self, table_id:str):
         """Generate dictionary of annotations for the given Synapse file.
         Synapse returns all custom annotations as lists since they
         can contain multiple values. In all cases, the values will
         be converted into strings and concatenated with ", ".
@@ -1307,34 +1812,51 @@
 
     @retry(stop = stop_after_attempt(5), 
             wait = wait_chain(*[wait_fixed(10) for i in range (2)] + 
                     [wait_fixed(15) for i in range(2)] + 
                     [wait_fixed(20)]),
             retry=retry_if_exception_type(LookupError),
             retry_error_callback = raise_final_error)
+
+    def checkIfinAssetView(self, syn_id) -> str:
+        # get data in administrative fileview for this pipeline
+        assetViewTable = self.getStorageFileviewTable()
+        all_files = list(assetViewTable["id"])
+        if syn_id in all_files: 
+            return True
+        else: 
+            return False
+
     def getDatasetProject(self, datasetId: str) -> str:
         """Get parent project for a given dataset ID.
 
         Args:
             datasetId (str): Synapse entity ID (folder or project).
 
         Raises:
             ValueError: Raised if Synapse ID cannot be retrieved
             by the user or if it doesn't appear in the file view.
 
         Returns:
             str: The Synapse ID for the parent project.
         """
 
-        self._query_fileview()
-
         # Subset main file view
         dataset_index = self.storageFileviewTable["id"] == datasetId
         dataset_row = self.storageFileviewTable[dataset_index]
 
+        # re-query if no datasets found
+        if dataset_row.empty:
+            sleep(5)
+            self._query_fileview()
+            # Subset main file view
+            dataset_index = self.storageFileviewTable["id"] == datasetId
+            dataset_row = self.storageFileviewTable[dataset_index]
+
+
         # Return `projectId` for given row if only one found
         if len(dataset_row) == 1:
             dataset_project = dataset_row["projectId"].values[0]
             return dataset_project
 
         # Otherwise, check if already project itself
         try:
@@ -1390,160 +1912,350 @@
         for col_record in table_schema:
 
             #TODO clean up dictionary for compactness (e.g. remove redundant 'name' key)
             table_schema_by_cname[col_record["name"]] = col_record
 
         return table_schema_by_cname
 
-    def make_synapse_table(self, 
-            table_to_load: pd.DataFrame, 
-            dataset_id: str, table_name: str, 
-            existingTableId: str = None,
-            update_col: str = 'entityId', 
-            column_type_dictionary: Dict = {}, 
-            specify_schema: bool = True, 
-            restrict: bool = False, 
-            manipulation: str = 'update') -> str:
-        '''
-        Make a synapse table for record based data
+class TableOperations:
+    """
+    Object to hold functions for various table operations specific to the Synapse Asset Store.
+    
+    Currently implement operations are:
+    createTable: upload a manifest as a new table when none exist
+    replaceTable: replace a metadata in a table from one manifest with metadata from another manifest
+    updateTable: add a column to a table that already exists on synapse
+
+    Operations currently in development are:
+    upsertTable: add metadata from a manifest to an existing table that contains metadata from another manifest
+    """
+
 
+    def createTable(synStore: SynapseStorage, tableToLoad: pd.DataFrame = None, tableName: str = None, datasetId: str = None, columnTypeDict: dict = None, specifySchema: bool = True, restrict: bool = False):
+        """
+        Method to create a table from a metadata manifest and upload it to synapse
+        
         Args:
-            table_to_load (pd.DataFrame): table to upload to synapse
-            dataset_id (str): synID for dataset related to manifest to be uploaded as table
-            existingTableId (str): Optional, synID of existing table to upload to
-            table_name (str): Name of the table that will be displayed on synapse
-            update_col (str): Optional, if updating a table by aligning on index, column to use as indices
-            column_type_dictionary (Dict): dictionary of column types
-            specify_schema (bool):  specify a schema for the table at upload according to types in column_type_dictionary
-            restrict (bool): set to True if access restrictions need to be imposed on table when stored on synapse, False otherwise 
-            manipulation (str): type of manipulation to do if a table exists already. Can be either "update" or "replace". 
-                Defaults to "update" to preserve old behavior
+            tableToLoad: manifest formatted appropriately for the table
+            tableName: name of the table to be uploaded
+            datasetId: synID of the dataset for the manifest
+            columnTypeDict: dictionary schema for table columns: type, size, etc
+            specifySchema: to specify a specific schema for the table format          
+            restrict: bool, whether or not the manifest contains sensitive data that will need additional access restrictions 
+            
 
         Returns:
-            str: synId of table uploaded to synapse
+            table.schema.id: synID of the newly created table
+        """
 
-        '''
-        if existingTableId:
-            existing_table, existing_results = self.get_synapse_table(existingTableId)
+        datasetEntity = synStore.syn.get(datasetId, downloadFile = False)
+        datasetName = datasetEntity.name
+        table_schema_by_cname = synStore._get_table_schema_by_cname(columnTypeDict) 
+
+        if not tableName:
+            tableName = datasetName + 'table'
+        datasetParentProject = synStore.getDatasetProject(datasetId)
+        if specifySchema:
+            if columnTypeDict == {}:
+                logger.error("Did not provide a columnTypeDict.")
+            #create list of columns:
+            cols = []
+            for col in tableToLoad.columns:
+                if col in table_schema_by_cname:
+                    col_type = table_schema_by_cname[col]['columnType']
+                    max_size = table_schema_by_cname[col]['maximumSize'] if 'maximumSize' in table_schema_by_cname[col].keys() else 100
+                    max_list_len = 250
+                    if max_size and max_list_len:
+                        cols.append(Column(name=col, columnType=col_type, 
+                            maximumSize=max_size, maximumListLength=max_list_len))
+                    elif max_size:
+                        cols.append(Column(name=col, columnType=col_type, 
+                            maximumSize=max_size))
+                    else:
+                        cols.append(Column(name=col, columnType=col_type))
+                else:
+                    #TODO add warning that the given col was not found and it's max size is set to 100
+                    cols.append(Column(name=col, columnType='STRING', maximumSize=100))
+            schema = Schema(name=tableName, columns=cols, parent=datasetParentProject)
+            table = Table(schema, tableToLoad)
+            table = synStore.syn.store(table, isRestricted = restrict)
+            return table.schema.id
+        else:
+            # For just uploading the tables to synapse using default
+            # column types.
+            table = build_table(tableName, datasetParentProject, tableToLoad)
+            table = synStore.syn.store(table, isRestricted = restrict)
+            return table.schema.id
 
-            manipulation = manipulation.lower()
-            if manipulation not in ['update', 'replace']:
-                raise NotImplementedError(
-                    "Currently, only 'update' and 'replace' table operations are supported."
-                )
+    def replaceTable(synStore: SynapseStorage, tableToLoad: pd.DataFrame = None, tableName: str = None, existingTableId: str = None, specifySchema: bool = True, datasetId: str = None, columnTypeDict: dict = None, restrict: bool = False):
+        """
+        Method to replace an existing table on synapse with metadata from a new manifest
+        
+        Args:
+            tableToLoad: manifest formatted appropriately for the table
+            tableName: name of the table to be uploaded
+            existingTableId: synId of the existing table to be replaced
+            specifySchema: to infer a schema for the table format      
+            datasetId: synID of the dataset for the manifest    
+            columnTypeDict: dictionary schema for table columns: type, size, etc
+            restrict: bool, whether or not the manifest contains sensitive data that will need additional access restrictions 
+            
 
-            # create/update a table corresponding to this dataset in this dataset's parent project
-            # update_col is the column in the table that has a unique code that will allow Synapse to
-            # locate its position in the old and new table.
-            if manipulation == 'update':
-                table_to_load = update_df(existing_table, table_to_load, update_col)
-                # store table with existing etag data and impose restrictions as appropriate
-                self.syn.store(Table(existingTableId, table_to_load, etag = existing_results.etag), isRestricted = restrict)
-
-            elif manipulation == 'replace':
-                # remove rows
-                self.syn.delete(existing_results)
-                # wait for row deletion to finish on synapse before getting empty table
-                sleep(10)
-                
-                # removes all current columns
-                current_table = self.syn.get(existingTableId)
-                current_columns = self.syn.getTableColumns(current_table)
-                for col in current_columns:
-                    current_table.removeColumn(col)
+        Returns:
+           existingTableId: synID of the already existing table that had its metadata replaced
+        """
+        datasetEntity = synStore.syn.get(datasetId, downloadFile = False)
+        datasetName = datasetEntity.name
+        table_schema_by_cname = synStore._get_table_schema_by_cname(columnTypeDict) 
+        existing_table, existing_results = synStore.get_synapse_table(existingTableId)
+        # remove rows
+        synStore.syn.delete(existing_results)
+        # wait for row deletion to finish on synapse before getting empty table
+        sleep(10)
+        
+        # removes all current columns
+        current_table = synStore.syn.get(existingTableId)
+        current_columns = synStore.syn.getTableColumns(current_table)
+        for col in current_columns:
+            current_table.removeColumn(col)
 
-                if not table_name:
-                    table_name = datasetName + 'table'
+        if not tableName:
+            tableName = datasetName + 'table'
+        
+        # Process columns according to manifest entries
+        table_schema_by_cname = synStore._get_table_schema_by_cname(columnTypeDict) 
+        datasetParentProject = synStore.getDatasetProject(datasetId)
+        if specifySchema:
+            if columnTypeDict == {}:
+                logger.error("Did not provide a columnTypeDict.")
+            #create list of columns:
+            cols = []
+            
+            for col in tableToLoad.columns:
                 
-                # Process columns according to manifest entries
-                table_schema_by_cname = self._get_table_schema_by_cname(column_type_dictionary) 
-                datasetParentProject = self.getDatasetProject(dataset_id)
-                if specify_schema:
-                    if column_type_dictionary == {}:
-                        logger.error("Did not provide a column_type_dictionary.")
-                    #create list of columns:
-                    cols = []
-                    
-                    for col in table_to_load.columns:
-                        
-                        if col in table_schema_by_cname:
-                            col_type = table_schema_by_cname[col]['columnType']
-                            max_size = table_schema_by_cname[col]['maximumSize'] if 'maximumSize' in table_schema_by_cname[col].keys() else 100
-                            max_list_len = 250
-                            if max_size and max_list_len:
-                                cols.append(Column(name=col, columnType=col_type, 
-                                    maximumSize=max_size, maximumListLength=max_list_len))
-                            elif max_size:
-                                cols.append(Column(name=col, columnType=col_type, 
-                                    maximumSize=max_size))
-                            else:
-                                cols.append(Column(name=col, columnType=col_type))
-                        else:
-                            
-                            #TODO add warning that the given col was not found and it's max size is set to 100
-                            cols.append(Column(name=col, columnType='STRING', maximumSize=100))
+                if col in table_schema_by_cname:
+                    col_type = table_schema_by_cname[col]['columnType']
+                    max_size = table_schema_by_cname[col]['maximumSize'] if 'maximumSize' in table_schema_by_cname[col].keys() else 100
+                    max_list_len = 250
+                    if max_size and max_list_len:
+                        cols.append(Column(name=col, columnType=col_type, 
+                            maximumSize=max_size, maximumListLength=max_list_len))
+                    elif max_size:
+                        cols.append(Column(name=col, columnType=col_type, 
+                            maximumSize=max_size))
+                    else:
+                        cols.append(Column(name=col, columnType=col_type))
+                else:
                     
-                    # adds new columns to schema
-                    for col in cols:
-                        current_table.addColumn(col)
-                    self.syn.store(current_table, isRestricted = restrict)
+                    #TODO add warning that the given col was not found and it's max size is set to 100
+                    cols.append(Column(name=col, columnType='STRING', maximumSize=100))
+            
+            # adds new columns to schema
+            for col in cols:
+                current_table.addColumn(col)
+            synStore.syn.store(current_table, isRestricted = restrict)
+
+            # wait for synapse store to finish
+            sleep(1)
+
+            # build schema and table from columns and store with necessary restrictions
+            schema = Schema(name=tableName, columns=cols, parent=datasetParentProject)
+            schema.id = existingTableId
+            table = Table(schema, tableToLoad, etag = existing_results.etag)
+            table = synStore.syn.store(table, isRestricted = restrict)
+        else:
+            logging.error("Must specify a schema for table replacements")
 
-                    # wait for synapse store to finish
-                    sleep(1)
+        # remove system metadata from manifest
+        existing_table.drop(columns = ['ROW_ID', 'ROW_VERSION'], inplace = True)
+        return existingTableId
+    
+
+    def _get_schematic_db_creds(synStore: SynapseStorage):
+        username = None
+        authtoken = None
+
+
+        # Get access token from environment variable if available
+        # Primarily useful for testing environments, with other possible usefulness for containers
+        env_access_token = os.getenv("SYNAPSE_ACCESS_TOKEN")
+        if env_access_token:
+            authtoken = env_access_token
+            return username, authtoken
+
+        # Get token from authorization header
+        # Primarily useful for API endpoint functionality
+        if 'Authorization' in synStore.syn.default_headers:
+            authtoken = synStore.syn.default_headers['Authorization'].split('Bearer ')[-1]
+            return username, authtoken
+
+        # retrive credentials from synapse object
+        # Primarily useful for local users, could only be stored here when a .synapseConfig file is used, but including to be safe
+        synapse_object_creds = synStore.syn.credentials
+        if hasattr(synapse_object_creds, 'username'):
+            username = synapse_object_creds.username
+        if hasattr(synapse_object_creds, '_token'):
+            authtoken = synapse_object_creds.secret
+
+        # Try getting creds from .synapseConfig file if it exists
+        # Primarily useful for local users. Seems to correlate with credentials stored in synaspe object when logged in
+        if os.path.exists(CONFIG.SYNAPSE_CONFIG_PATH):
+            config = synStore.syn.getConfigFile(CONFIG.SYNAPSE_CONFIG_PATH)
+
+            # check which credentials are provided in file
+            if config.has_option('authentication', 'username'):
+                username = config.get('authentication', 'username')
+            if config.has_option('authentication', 'authtoken'):
+                authtoken = config.get('authentication', 'authtoken')
+        
+        # raise error if required credentials are not found
+        # providing an authtoken without a username did not prohibit upsert functionality, 
+        # but including username gathering for completeness for schematic_db
+        if not username and not authtoken:
+            raise NameError(
+                "Username and authtoken credentials could not be found in the environment, synapse object, or the .synapseConfig file"
+            )
+        if not authtoken:
+            raise NameError(
+                "authtoken credentials could not be found in the environment, synapse object, or the .synapseConfig file"
+            )
+        
+        return username, authtoken
 
-                    # build schema and table from columns and store with necessary restrictions
-                    schema = Schema(name=table_name, columns=cols, parent=datasetParentProject)
-                    schema.id = existingTableId
-                    table = Table(schema, table_to_load, etag = existing_results.etag)
-                    table = self.syn.store(table, isRestricted = restrict)
-                else:
-                    logging.error("Must specify a schema for table replacements")
+    def upsertTable(synStore: SynapseStorage, sg: SchemaGenerator, tableToLoad: pd.DataFrame = None, tableName: str = None, existingTableId: str = None,  datasetId: str = None):
+        """
+        Method to upsert rows from a new manifest into an existing table on synapse
+        For upsert functionality to work, primary keys must follow the naming convention of <componenet>_id        
+        `-tm upsert` should be used for initial table uploads if users intend to upsert into them at a later time; using 'upsert' at creation will generate the metadata necessary for upsert functionality.
+        Currently it is required to use -dl/--use_display_label with table upserts.
+        
 
-            # remove system metadata from manifest
-            existing_table.drop(columns = ['ROW_ID', 'ROW_VERSION'], inplace = True)
-            return existingTableId
-        else:
-            datasetEntity = self.syn.get(dataset_id, downloadFile = False)
-            datasetName = datasetEntity.name
-            table_schema_by_cname = self._get_table_schema_by_cname(column_type_dictionary) 
-
-            if not table_name:
-                table_name = datasetName + 'table'
-            datasetParentProject = self.getDatasetProject(dataset_id)
-            if specify_schema:
-                if column_type_dictionary == {}:
-                    logger.error("Did not provide a column_type_dictionary.")
-                #create list of columns:
-                cols = []
-                for col in table_to_load.columns:
-                    if col in table_schema_by_cname:
-                        col_type = table_schema_by_cname[col]['columnType']
-                        max_size = table_schema_by_cname[col]['maximumSize'] if 'maximumSize' in table_schema_by_cname[col].keys() else 100
-                        max_list_len = 250
-                        if max_size and max_list_len:
-                            cols.append(Column(name=col, columnType=col_type, 
-                                maximumSize=max_size, maximumListLength=max_list_len))
-                        elif max_size:
-                            cols.append(Column(name=col, columnType=col_type, 
-                                maximumSize=max_size))
-                        else:
-                            cols.append(Column(name=col, columnType=col_type))
-                    else:
-                        #TODO add warning that the given col was not found and it's max size is set to 100
-                        cols.append(Column(name=col, columnType='STRING', maximumSize=100))
-                schema = Schema(name=table_name, columns=cols, parent=datasetParentProject)
-                table = Table(schema, table_to_load)
-                table = self.syn.store(table, isRestricted = restrict)
-                return table.schema.id
+        Args:
+            tableToLoad: manifest formatted appropriately for the table
+            tableName: name of the table to be uploaded
+            existingTableId: synId of the existing table to be replaced     
+            datasetId: synID of the dataset for the manifest    
+            columnTypeDict: dictionary schema for table columns: type, size, etc
+            
+
+        Returns:
+           existingTableId: synID of the already existing table that had its metadata replaced
+        """            
+
+        username, authtoken = TableOperations._get_schematic_db_creds(synStore)
+
+        synConfig = SynapseConfig(username, authtoken, synStore.getDatasetProject(datasetId))
+        synapseDB = SynapseDatabase(synConfig)
+
+        try:
+            # Try performing upsert
+            synapseDB.upsert_table_rows(table_name=tableName, data=tableToLoad)
+        except(SynapseHTTPError) as ex:
+            # If error is raised because Table has old `Uuid` column and not new `Id` column, then handle and re-attempt upload
+            if 'Id is not a valid column name or id' in str(ex):
+                TableOperations._update_table_uuid_column(synStore, existingTableId, sg)
+                synapseDB.upsert_table_rows(table_name=tableName, data=tableToLoad)
+            # Raise if other error
             else:
-                # For just uploading the tables to synapse using default
-                # column types.
-                table = build_table(table_name, datasetParentProject, table_to_load)
-                table = self.syn.store(table, isRestricted = restrict)
-                return table.schema.id
+                raise ex
+
+        return existingTableId
+
+    def _update_table_uuid_column(synStore: SynapseStorage, table_id: str, sg: SchemaGenerator,) -> None:
+        """Removes the `Uuid` column when present, and relpaces with an `Id` column
+        Used to enable backwards compatability for manifests using the old `Uuid` convention
+
+        Args:
+            table_id (str): The Synapse id of the table to be upserted into, that needs columns updated
+
+        Returns:
+            None
+        """
+
+        # Get the columns of the schema
+        schema = synStore.syn.get(table_id)
+        cols = synStore.syn.getTableColumns(schema)
+        
+        # Iterate through columns until `Uuid` column is found
+        for col in cols:
+            if col.name.lower() == 'uuid':
+                # See if schema has `Uuid` column specified
+                try:
+                    uuid_col_in_schema = sg.se.is_class_in_schema(col.name)      
+                except (KeyError):
+                    uuid_col_in_schema = False
+
+                # If there is, then create a new `Id` column from scratch
+                if uuid_col_in_schema:
+                    new_col = Column(columnType = "STRING", maximumSize = 64, name = "Id")
+                    schema.addColumn(new_col)
+                    schema = synStore.syn.store(schema)
+                # If there is not, then use the old `Uuid` column as a basis for the new `Id` column
+                else:
+                    # Create a new `Id` column based off of the old `Uuid` column, and store (column is empty)
+                    new_col = deepcopy(col)
+                    new_col['name'] = 'Id'
+                    schema.addColumn(new_col)
+                    schema = synStore.syn.store(schema)
+                
+                
+                    # Recently stored column is empty, so populated with uuid values
+                    TableOperations._populate_new_id_column(synStore, table_id, schema)
+
+                    # get the up-to-date table, remove old `Uuid` column, and store
+                    sleep(1)
+                    schema = synStore.syn.get(table_id)
+                    schema.removeColumn(col)
+                    schema = synStore.syn.store(schema)
+
+                    # Exit iteration; only concerned with `Uuid` column
+                break
+
+        return
+
+    def _populate_new_id_column(synStore: SynapseStorage, table_id: str, schema: Schema) -> None:
+        """Copies the uuid values that were present in the column named `Uuid` to the new column named `Id`
+
+        Args:
+            table_id (str): The Synapse id of the table to be upserted into, that needs columns updated
+            schema (synapseclient.table.Schema): Schema of the table columns
+
+        Returns:
+            None
+        """
+        # Query the table for the old `Uuid` column and new `Id` column
+        results = synStore.syn.tableQuery(f"select Uuid,Id from {table_id}")
+        results_df = results.asDataFrame()
+
+        # Copy uuid values to new column, and store in table
+        results_df = populate_df_col_with_another_col(results_df, 'Uuid', 'Id')
+        table = synStore.syn.store(Table(schema, results_df, etag=results.etag))
+        return
+
+    def updateTable(synStore: SynapseStorage, tableToLoad: pd.DataFrame = None, existingTableId: str = None,  update_col: str = 'Id',  restrict: bool = False):
+        """
+        Method to update an existing table with a new column
+        
+        Args:
+            tableToLoad: manifest formatted appropriately for the table, that contains the new column
+            existingTableId: synId of the existing table to be replaced
+            updateCol: column to index the old and new tables on
+            restrict: bool, whether or not the manifest contains sensitive data that will need additional access restrictions 
+            
+
+        Returns:
+           existingTableId: synID of the already existing table that had its metadata replaced
+        """
+        existing_table, existing_results = synStore.get_synapse_table(existingTableId)
+        
+        tableToLoad = update_df(existing_table, tableToLoad, update_col)
+        # store table with existing etag data and impose restrictions as appropriate
+        synStore.syn.store(Table(existingTableId, tableToLoad, etag = existing_results.etag), isRestricted = restrict)
+
+        return existingTableId
 
 
 class DatasetFileView:
     """Helper class to create temporary dataset file views.
     This class can be used in conjunction with a 'with' statement.
     This will ensure that the file view is deleted automatically.
     See SynapseStorage.getDatasetAnnotationsBatch for example usage.
```

### Comparing `schematicpy-23.1.1/schematic/utils/__init__.py` & `schematicpy-23.6.1/schematic/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.1.1/schematic/utils/cli_utils.py` & `schematicpy-23.6.1/schematic/utils/cli_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -158,8 +158,11 @@
     else:
         return
 
 def parse_comma_str_to_list(
     ctx, param, comma_string,
 ) -> List[str]:
 
-    return comma_string.split(",")
+    if comma_string:
+        return comma_string.split(",")
+    else:
+        return None
```

### Comparing `schematicpy-23.1.1/schematic/utils/curie_utils.py` & `schematicpy-23.6.1/schematic/utils/curie_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.1.1/schematic/utils/df_utils.py` & `schematicpy-23.6.1/schematic/utils/df_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,83 @@
 import logging
-
-import pandas as pd
-import numpy as np
 from copy import deepcopy
-import dateparser as dp
+from time import perf_counter
 import datetime as dt
+import dateparser as dp
+import pandas as pd
+import numpy as np
+from pandarallel import pandarallel
 
 logger = logging.getLogger(__name__)
 
 
 def load_df(file_path, preserve_raw_input=True, data_model=False, **load_args):
     """
     Universal function to load CSVs and return DataFrames
     Parses string entries to convert as appropriate to type int, float, and pandas timestamp
+    Pandarallel is used for type inference for large manfiests to improve performance
     Args:
         file_path: path of csv to open
         preserve_raw_input: Bool. If false, convert cell datatypes to an inferred type
         data_model: bool, indicates if importing a data model
         load_args: dict of key value pairs to be passed to the pd.read_csv function
         **kwargs: keyword arguments for pd.read_csv()
 
-    Returns: a processed dataframe for manifests or unprocessed df for data models
+    Returns: a processed dataframe for manifests or unprocessed df for data models and where indicated
     """
+    large_manifest_cutoff_size = 1000
+    # start performance timer
+    t_load_df = perf_counter()
+    
     #Read CSV to df as type specified in kwargs
     org_df = pd.read_csv(file_path, keep_default_na = True, encoding='utf8', **load_args)
     
+    # If type inference not allowed: trim and return
     if preserve_raw_input:
         #only trim if not data model csv
         if not data_model:
             org_df=trim_commas_df(org_df)
-
+        
+            # log manifest load and processing time
+            logger.debug(f"Load Elapsed time {perf_counter()-t_load_df}")
         return org_df
 
+    # If type inferences is allowed: infer types, trim, and return
     else:
+        # create a separate copy of the manifest 
+        # before beginning conversions to store float values
         float_df=deepcopy(org_df)
-        #Find integers stored as strings
-        #Cast the columns in dataframe to string while preserving NaN
+        
+        # Cast the columns in the dataframe to string and
+        # replace Null values with empty strings
         null_cells = org_df.isnull() 
         org_df = org_df.astype(str).mask(null_cells, '')
-        ints = org_df.applymap(lambda x: np.int64(x) if str.isdigit(x) else False, na_action='ignore').fillna(False)
-        dates = org_df.applymap(lambda x: _parse_dates(x), na_action='ignore').fillna(False)
 
-        #convert strings to numerical dtype (float) if possible, preserve non-numerical strings
+        # Find integers stored as strings and replace with entries of type np.int64
+        if org_df.size < large_manifest_cutoff_size:  # If small manifest, iterate as normal for improved performance
+            ints = org_df.applymap(lambda x: np.int64(x) if str.isdigit(x) else False, na_action='ignore').fillna(False)
+
+        else:   # parallelize iterations for large manfiests
+            pandarallel.initialize(verbose = 1)
+            ints = org_df.parallel_applymap(lambda x: np.int64(x) if str.isdigit(x) else False, na_action='ignore').fillna(False)
+
+        # convert strings to numerical dtype (float) if possible, preserve non-numerical strings
         for col in org_df.columns:
             float_df[col]=pd.to_numeric(float_df[col], errors='coerce')
+            # replace values that couldn't be converted to float with the original str values
             float_df[col].fillna(org_df[col][float_df[col].isna()],inplace=True)
         
-        #Trim nans and empty rows and columns
+        # Trim nans and empty rows and columns
         processed_df = trim_commas_df(float_df)
         
-        #Store values that were entered as ints and dates
+        # Store values that were converted to type int in the final dataframe
         processed_df=processed_df.mask(ints != False, other = ints)  
-        processed_df=processed_df.mask(dates != False, other = dates)  
         
+        # log manifest load and processing time
+        logger.debug(f"Load Elapsed time {perf_counter()-t_load_df}")
         return processed_df
 
 
 def _parse_dates(date_string):
     try:
         date = dp.parse(date_string = date_string, settings = {'STRICT_PARSING': True})
         return date if date else False
@@ -157,7 +178,34 @@
 
     # remove all completely empty rows
     df = df.dropna(how="all", axis=0)
 
     #Fill in nan cells with empty strings
     df.fillna("", inplace=True)
     return df
+
+
+def col_in_dataframe(col: str, df: pd.DataFrame) -> bool:
+    """Check if a column is in a dataframe, without worring about case
+
+    Args:
+        col: name of column whose presence in the dataframe is being checked
+        df: pandas dataframe with data from manifest file.
+
+    Returns:
+        bool: whether or not the column name is a column in the dataframe, case agnostic
+    """
+    return col.lower() in [manifest_col.lower() for manifest_col in df.columns.to_list()]
+
+def populate_df_col_with_another_col(df: pd.DataFrame, source_col: str, target_col: str) -> pd.DataFrame:
+    """Copy the values from one column in a dataframe to another column in the same dataframe
+    Args:
+        df: pandas dataframe with data from manifest file.
+        source_col: column whose contents to copy over
+        target_col: column to be updated with other contents
+
+    Returns:
+        dataframe with contents updated
+    """
+    # Copy the contents over
+    df[target_col]=df[source_col]
+    return df
```

### Comparing `schematicpy-23.1.1/schematic/utils/google_api_utils.py` & `schematicpy-23.6.1/schematic/utils/google_api_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,20 @@
     }
 
 
 def build_service_account_creds() -> Dict[str, Any]:
     if "SERVICE_ACCOUNT_CREDS" in os.environ:
         dict_creds=json.loads(os.environ["SERVICE_ACCOUNT_CREDS"])
         credentials = service_account.Credentials.from_service_account_info(dict_creds, scopes=SCOPES)
+
+    # for AWS deployment
+    elif "SECRETS_MANAGER_SECRETS" in os.environ:
+        all_secrets_dict =json.loads(os.environ["SECRETS_MANAGER_SECRETS"])
+        dict_creds=json.loads(all_secrets_dict["SERVICE_ACCOUNT_CREDS"])
+        credentials = service_account.Credentials.from_service_account_info(dict_creds, scopes=SCOPES)
     else:
         credentials = service_account.Credentials.from_service_account_file(
             CONFIG.SERVICE_ACCT_CREDS, scopes=SCOPES
         )
 
     # get a Google Sheet API service
     sheet_service = build("sheets", "v4", credentials=credentials)
```

### Comparing `schematicpy-23.1.1/schematic/utils/io_utils.py` & `schematicpy-23.6.1/schematic/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.1.1/schematic/utils/schema_utils.py` & `schematicpy-23.6.1/schematic/utils/schema_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.1.1/schematic/utils/validate_rules_utils.py` & `schematicpy-23.6.1/schematic/utils/validate_rules_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,35 +18,42 @@
             'complementary_rules': [<rules available for pairing>]}
         }
     '''
     rule_dict = {
             "int": {
                 'arguments':(1, 0),
                 'type': "type_validation",
-                'complementary_rules': ['inRange',],
+                'complementary_rules': ['inRange', 'IsNA'],
                 'default_message_level': 'error'},
 
             "float": {
                 'arguments':(1, 0),
                 'type': "type_validation",
-                'complementary_rules': ['inRange',],
+                'complementary_rules': ['inRange', 'IsNA'],
                 'default_message_level': 'error'},
 
             "num": {
                 'arguments':(1, 0),
                 'type': "type_validation",
-                'complementary_rules': ['inRange',],
+                'complementary_rules': ['inRange', 'IsNA'],
                 'default_message_level': 'error'},
 
             "str": {
                 'arguments':(1, 0),
                 'type': "type_validation",
                 'complementary_rules': None,
                 'default_message_level': 'error'},
 
+            "date": {
+                'arguments':(1, 0),
+                'type': "content_validation",
+                'complementary_rules': None,
+                'default_message_level': 'error'
+            },
+
             "regex": {
                 'arguments':(3, 2), 
                 'fixed_arg': ['strict'], 
                 'type': "regex_validation",
                 'complementary_rules': ['list'],
                 'default_message_level': 'error'},
 
@@ -93,32 +100,31 @@
                 'default_message_level': 'error'},
                 
             "inRange": {
                 'arguments':(3, 2), 
                 'type': "content_validation",
                 'complementary_rules': ['int','float','num','protectAges'],
                 'default_message_level': 'error'},
+            
+            "IsNA":     {
+                'arguments':(1, 0), 
+                'type': "content_validation",
+                'complementary_rules': ['int', 'float', 'num', ],
+                'default_message_level': 'warning'},            
             }
 
     return rule_dict
 
 def get_error(validation_rules: list, 
         attribute_name: str, error_type: str, input_filetype:str,) -> List[str]:
     '''
     Generate error message for errors when trying to specify 
     multiple validation rules.
     '''
     error_col = attribute_name # Attribute name
-    if error_type == 'too_many_rules':
-        error_str = (f"The {input_filetype}, has an error in the validation rule "
-            f"for the attribute: {attribute_name}, the provided validation rules ({validation_rules}) ."
-        f"have too many entries. We currently only allow for pairs of rules to be used at the same time.")
-        logging.error(error_str)
-        error_message = error_str
-        error_val = f"Multiple Rules: too many rules"
     
     if error_type == 'delimiter':
         error_str = (f"The {input_filetype}, has an error in the validation rule "
             f"for the attribute: {attribute_name}, the provided validation rules ({validation_rules}) are improperly "
             f"specified. Please check your delimiter is '::'")
         logging.error(error_str)
         error_message = error_str
@@ -149,45 +155,44 @@
 
         error_str = (f"The {input_filetype}, has an error in the validation rule "
             f"for the attribute: {attribute_name}, the provided validation rules ({validation_rules}) is not "
             f"formatted properly. The number of provided arguments does not match the number allowed({no_allowed}) or required({no_required}).")
         logging.error(error_str)
         error_message = error_str
         error_val = f"Incorrect num arguments."
-
-    if error_type == 'invalid_rule_combination':
-        first_type=validation_rules[0].split(' ')[0]
-        second_type=validation_rule_info()[first_type]['complementary_rules']
-
-        error_str = (f"The {input_filetype}, has an error in the validation rule "
-            f"for the attribute: {attribute_name}, the provided validation rules ({'::'.join(validation_rules)}) are not "
-            f"a valid combination of rules. The validation rule [{first_type}] may only be used with rules of type {second_type}.")
-        logging.error(error_str)
-        error_message = error_str
-        error_val = f"Invalid rule combination."
         
     return ['NA', error_col, error_message, error_val]
 
 def validate_single_rule(validation_rule, attribute, input_filetype):
     '''
-    TODO:reformat validation_types from validate_manifest to document the 
-    arguments allowed. Keep in that location and pull into this function.
+    Perform validation for a single rule to ensure it is specified correctly with an appropriate number of arguments
+    Inputs:
+        validation_rule: single rule being validated
+        attribute: attribute validation rule was specified for
+        input_filetype: filetype of model input
+
+    Returns:
+        errors: List of errors
     '''
     errors = []
     validation_types = validation_rule_info()
     validation_rule_with_args = [
                 val_rule.strip() for val_rule in validation_rule.strip().split(" ")]
 
     rule_type = validation_rule_with_args[0]
 
+    # ensure rules are not delimited incorrectly
+    if ':' in validation_rule:
+        errors.append(get_error(validation_rule, attribute,
+            error_type = 'delimiter', input_filetype=input_filetype))
     # Check that the rule is actually a valid rule type.
-    if rule_type not in validation_types.keys():
+    elif rule_type not in validation_types.keys():
         errors.append(get_error(validation_rule, attribute,
             error_type = 'not_rule', input_filetype=input_filetype))
-
+    # if the rule is indeed a rule and formatted correctly, check that arguments are appropriate
     else:
         arguments_allowed, arguments_required = validation_types[rule_type]['arguments']
         # Remove any fixed args from our calc.
         if 'fixed_arg' in validation_types[rule_type].keys():
             fixed_args = validation_types[rule_type]['fixed_arg']
             num_args = len([vr for vr in validation_rule_with_args if vr not in fixed_args])-1 
         else:
@@ -202,62 +207,32 @@
         # There must be at least the number of args required,
         # and not more than allowed
         elif arguments_allowed:
             if (num_args < arguments_required) or (num_args > arguments_allowed):
                 errors.append(get_error(validation_rule, attribute,
                     error_type = 'incorrect_num_args', input_filetype=input_filetype))
 
-
-        if ':' in validation_rule:
-            errors.append(get_error(validation_rule, attribute,
-                error_type = 'delimiter', input_filetype=input_filetype))
     return errors
 
 def validate_schema_rules(validation_rules, attribute, input_filetype):
     '''
     validation_rules: list
     input_filetype: str, used in error generation to aid user in
         locating the source of the error.
 
     Validation Rules Formatting rules:
-    Multiple Rules:
-        max of 2 rules
     Single Rules:
-        Additional arg
+        Specified with the correct required arguments with no more than what is allowed
     '''
-    # Specify all the validation types and whether they currently
-    # allow users to pass additional arguments (when used on their own), and if there is
-    # a set number of arguments required.
-
     errors = []
-    rule_info = validation_rule_info()
-    num_validation_rules = len(validation_rules)
-
-    
-    # Check for edge case that user has entered more than 2 rules,
-    # throw an error if they have.
-    if num_validation_rules > 2:
-            errors.append(get_error(validation_rules, attribute,
-                error_type = 'too_many_rules', input_filetype=input_filetype))
-
-    elif num_validation_rules == 2: 
-        first_rule, second_rule = validation_rules
-        first_type = first_rule.split(" ")[0]  
-        second_type = second_rule.split(" ")[0]  
-
-        # validate rule combination
-        if second_type not in rule_info[first_type]['complementary_rules']:
-            errors.append(get_error(validation_rules, attribute, 
-                error_type = 'invalid_rule_combination', input_filetype=input_filetype))
         
-    # validate each rule individually in the combo
+    # validate each individual rule
     for rule in validation_rules:
         errors.extend(validate_single_rule(rule,
-            attribute, input_filetype))
-                
+            attribute, input_filetype))                
 
     if errors:
         raise ValidationError(
                         f"The {input_filetype} has an error in the validation_rules set "
                         f"for attribute {attribute}. "
                         f"Validation failed with the following errors: {errors}"
                     )
```

### Comparing `schematicpy-23.1.1/schematic/utils/validate_utils.py` & `schematicpy-23.6.1/schematic/utils/validate_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import pandas as pd
 from jsonschema import validate
 from re import compile, search, IGNORECASE
 from schematic.utils.io_utils import load_json
 from schematic import CONFIG, LOADER
 from typing import List
+import numpy as np
 
 def validate_schema(schema):
     """Validate schema against schema.org standard"""
     data_path = "validation_schemas/model.schema.json"
     json_schema_path = LOADER.filename(data_path)
     json_schema = load_json(json_schema_path)
     return validate(schema, json_schema)
@@ -61,8 +62,24 @@
         Output: ['a','b','c']     
 
     """
     col = col.apply(
         lambda x: [s.strip() for s in str(x).split(",")]
     )
 
-    return col
+    return col
+
+def np_array_to_str_list(np_array):
+    """
+    Parse a numpy array of ints to a list of strings
+    """
+    return np.char.mod('%d', np_array).tolist()
+
+def iterable_to_str_list(iterable):
+    "Parse an iterable into a list of strings"
+    strlist = []
+
+    for element in iterable:
+        strlist.append(str(element))
+
+    return strlist
+
```

### Comparing `schematicpy-23.1.1/schematic/visualization/attributes_explorer.py` & `schematicpy-23.6.1/schematic/visualization/attributes_explorer.py`

 * *Files 22% similar despite different names*

```diff
@@ -55,25 +55,67 @@
                 False: merged_df is returned.
 
         Returns:
             merged_df (pd.DataFrame): dataframe containing data relating to attributes
                 for the provided data model for all components in the data model. 
                 Dataframe is saved locally as a csv if save_file == True, or returned if
                 save_file == False. 
-        Raises:
-            ValueError:
-                If unable hits an error while attempting to get conditional requirements. 
-                This error is likely to be found if there is a mismatch in naming.
+                
         '''
         # get all components
         component_dg = self.sg.se.get_digraph_by_edge_type('requiresComponent')
         components = component_dg.nodes()
+        
         # For each data type to be loaded gather all attribtes the user would
         # have to provide.
+        return self._parse_attributes(components, save_file)
+    
+    def parse_component_attributes(self, component=None, save_file=True, include_index=True):
+        '''
+        Args: save_file (bool):
+                True: merged_df is saved locally to output_path.
+                False: merged_df is returned.
+              include_index (bool):
+                Whether to include the index in the returned dataframe (True) or not (False)
+
+        Returns:
+            merged_df (pd.DataFrame): dataframe containing data relating to attributes
+                for the provided data model for the specified component in the data model. 
+                Dataframe is saved locally as a csv if save_file == True, or returned if
+                save_file == False. 
+        '''        
+
+        if not component:
+            raise ValueError("You must provide a component to visualize.")
+        else:
+            return self._parse_attributes([component], save_file, include_index)
+
+    def _parse_attributes(self, components, save_file=True, include_index=True):
+        '''
+        Args: save_file (bool):
+                True: merged_df is saved locally to output_path.
+                False: merged_df is returned.
+              components (list):
+                list of components to parse attributes for
+              include_index (bool):
+                Whether to include the index in the returned dataframe (True) or not (False)
 
+        Returns:
+            merged_df (pd.DataFrame): dataframe containing data relating to attributes
+                for the provided data model for specified components in the data model. 
+                Dataframe is saved locally as a csv if save_file == True, or returned if
+                save_file == False. 
+        Raises:
+            ValueError:
+                If unable hits an error while attempting to get conditional requirements. 
+                This error is likely to be found if there is a mismatch in naming.
+        '''
+        
+        # For each data type to be loaded gather all attribtes the user would
+        # have to provide.
         df_store = []
         for component in components:
             data_dict = {}
             # get the json schema
             json_schema = self.sg.get_json_schema_requirements(
                 source_node=component, schema_name=self.path_to_jsonld)
 
@@ -158,10 +200,10 @@
 
         merged_attributes_df = pd.concat(df_store, join='outer')
         cols = ['Attribute', 'Label', 'Description', 'Required', 'Cond_Req', 'Valid Values', 'Conditional Requirements', 'Validation Rules', 'Component']
         cols = [col for col in cols if col in merged_attributes_df.columns]
 
         merged_attributes_df = merged_attributes_df[cols]
         if save_file == True:
-            return merged_attributes_df.to_csv(os.path.join(self.output_path, self.schema_name + 'attributes_data.vis_data.csv'))
+            return merged_attributes_df.to_csv(os.path.join(self.output_path, self.schema_name + 'attributes_data.vis_data.csv'), index=include_index)
         elif save_file == False:
-            return merged_attributes_df.to_csv()
+            return merged_attributes_df.to_csv(index=include_index)
```

### Comparing `schematicpy-23.1.1/schematic/visualization/commands.py` & `schematicpy-23.6.1/schematic/visualization/commands.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.1.1/schematic/visualization/tangled_tree.py` & `schematicpy-23.6.1/schematic/visualization/tangled_tree.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.1.1/setup.py` & `schematicpy-23.6.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,74 +1,370 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: schematicpy
+Version: 23.6.1
+Summary: Package for biomedical data model and metadata ingress management
+Home-page: https://github.com/Sage-Bionetworks/schematic
+Keywords: schema,metadata,validation,data model,linked data
+Author: Milen Nikolov
+Author-email: milen.nikolov@sagebase.org
+Requires-Python: >=3.9.0,<3.11
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: Flask (>=2.0.0,<3.0.0)
+Requires-Dist: Flask-Cors (>=3.0.10,<4.0.0)
+Requires-Dist: Jinja2 (>2.11.3)
+Requires-Dist: MarkupSafe (==2.1.0)
+Requires-Dist: PyYAML (>=6.0.0,<7.0.0)
+Requires-Dist: backports.zoneinfo (>=0.2.1,<0.3.0) ; python_version < "3.9"
+Requires-Dist: click (>=8.0.0,<9.0.0)
+Requires-Dist: click-log (>=0.4.0,<0.5.0)
+Requires-Dist: connexion[swagger-ui] (>=2.8.0,<3.0.0)
+Requires-Dist: dateparser (>=1.1.4,<2.0.0)
+Requires-Dist: google-api-python-client (>=2.0.0,<3.0.0)
+Requires-Dist: google-auth-httplib2 (>=0.1.0,<0.2.0)
+Requires-Dist: google-auth-oauthlib (>=0.8.0,<0.9.0)
+Requires-Dist: graphviz (>=0.20.0,<0.21.0)
+Requires-Dist: great-expectations (>=0.15.0,<0.16.0)
+Requires-Dist: inflection (>=0.5.1,<0.6.0)
+Requires-Dist: itsdangerous (>=2.0.0,<3.0.0)
+Requires-Dist: jsonschema (>=4.0.0,<5.0.0)
+Requires-Dist: networkx (>=2.2.8)
+Requires-Dist: numpy (>=1.21.1,<2.0.0)
+Requires-Dist: oauth2client (>=4.1.0,<5.0.0)
+Requires-Dist: openpyxl (>=3.0.9,<4.0.0)
+Requires-Dist: pandarallel (>=1.6.4,<2.0.0)
+Requires-Dist: pandas (>=1.3.1,<2.0.0)
+Requires-Dist: pdoc (>=12.2.0,<13.0.0)
+Requires-Dist: pygsheets (>=2.0.4,<3.0.0)
+Requires-Dist: pyopenssl (>=23.0.0,<24.0.0)
+Requires-Dist: rdflib (>=6.0.0,<7.0.0)
+Requires-Dist: schematic-db[synapse] (>=0.0.20,<0.0.21)
+Requires-Dist: setuptools (>=66.0.0,<67.0.0)
+Requires-Dist: sphinx-click (>=4.0.0,<5.0.0)
+Requires-Dist: synapseclient (>=2.7.0,<3.0.0)
+Requires-Dist: tenacity (>=8.0.1,<9.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: typing-extensions (<4.6.0)
+Project-URL: Documentation, https://github.com/Sage-Bionetworks/schematic
+Project-URL: Repository, https://github.com/Sage-Bionetworks/schematic
+Description-Content-Type: text/markdown
 
-packages = \
-['schematic',
- 'schematic.manifest',
- 'schematic.models',
- 'schematic.schemas',
- 'schematic.store',
- 'schematic.utils',
- 'schematic.visualization']
-
-package_data = \
-{'': ['*'],
- 'schematic': ['etc/*', 'etc/data_models/*', 'etc/validation_schemas/*']}
-
-install_requires = \
-['Flask-Cors>=3.0.10,<4.0.0',
- 'Flask>=1.1.4,<2.0.0',
- 'Jinja2==2.11.3',
- 'MarkupSafe==2.0.1',
- 'PyYAML>=5.4.1,<6.0.0',
- 'click-log>=0.3.2,<0.4.0',
- 'click>=7.1.2,<8.0.0',
- 'connexion[swagger-ui]>=2.8.0,<3.0.0',
- 'dateparser>=1.1.4,<2.0.0',
- 'google-api-python-client>=1.12.8,<2.0.0',
- 'google-auth-httplib2>=0.0.4,<0.0.5',
- 'google-auth-oauthlib>=0.4.2,<0.5.0',
- 'graphviz>=0.16,<0.17',
- 'great-expectations>=0.15.0,<0.16.0',
- 'inflection>=0.5.1,<0.6.0',
- 'itsdangerous==1.1.0',
- 'jsonschema>=3.2.0,<4.0.0',
- 'networkx>=2.5,<3.0',
- 'numpy>=1.21.1,<2.0.0',
- 'oauth2client<4.0.0',
- 'openpyxl>=3.0.9,<4.0.0',
- 'pandas>=1.3.1,<2.0.0',
- 'pdoc>=12.2.0,<13.0.0',
- 'pygsheets>=2.0.4,<3.0.0',
- 'rdflib>=5.0.0,<6.0.0',
- 'setuptools>=52.0.0,<53.0.0',
- 'sphinx-click>=3.1.0,<4.0.0',
- 'synapseclient>=2.6.0,<3.0.0',
- 'tenacity>=8.0.1,<9.0.0',
- 'toml>=0.10.2,<0.11.0']
-
-extras_require = \
-{':python_version < "3.9"': ['backports.zoneinfo>=0.2.1,<0.3.0']}
-
-entry_points = \
-{'console_scripts': ['schematic = schematic.__main__:main']}
-
-setup_kwargs = {
-    'name': 'schematicpy',
-    'version': '23.1.1',
-    'description': 'Package for biomedical data model and metadata ingress management',
-    'long_description': '# Schematic\n[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FSage-Bionetworks%2Fschematic%2Fbadge%3Fref%3Ddevelop&style=flat)](https://actions-badge.atrox.dev/Sage-Bionetworks/schematic/goto?ref=develop) [![Documentation Status](https://readthedocs.org/projects/sage-schematic/badge/?version=develop)](https://sage-schematic.readthedocs.io/en/develop/?badge=develop) [![PyPI version](https://badge.fury.io/py/schematicpy.svg)](https://badge.fury.io/py/schematicpy)\n\n# Table of contents\n- [Introduction](#introduction)\n- [Installation](#installation)\n  - [Installation Requirements](#installation-requirements)\n  - [Installation guide for data curator app](#installation-guide-for-data-curator-app)\n  - [Installation guide for developers/contributors](#installation-guide-for-developerscontributors)\n- [Other Contribution Guidelines](#other-contribution-guidelines)\n    - [Update readthedocs documentation](#update-readthedocs-documentation)\n- [Command Line Usage](#command-line-usage)\n- [Testing](#testing)\n  - [Updating Synapse test resources](#updating-synapse-test-resources)\n- [Code Style](#code-style)\n- [Contributors](#contributors)\n\n# Introduction\nSCHEMATIC is an acronym for _Schema Engine for Manifest Ingress and Curation_. The Python based infrastructure provides a _novel_ schema-based, metadata ingress ecosystem, that is meant to streamline the process of biomedical dataset annotation, metadata validation and submission to a data repository for various data contributors.\n\n# Installation\n## Installation Requirements\n* Python 3.7.1 or higher\n\nNote: You need to be a registered and certified user on [`synapse.org`](https://www.synapse.org/), and also have the right permissions to download the Google credentials files from Synapse.\n\n\n## Installation guide for data curator app\n\nCreate and activate a virtual environment within which you can install the package:\n\n```\npython3 -m venv .venv\nsource .venv/bin/activate\n```\n\nNote: Python 3 has a built-in support for virtual environment [venv](https://docs.python.org/3/library/venv.html#module-venv) so you no longer need to install virtualenv.\n\nInstall and update the package using [pip](https://pip.pypa.io/en/stable/quickstart/):\n\n```\npython3 -m pip install schematicpy\n```\n\nIf you run into error: Failed building wheel for numpy, the error might be able to resolve by upgrading pip. Please try to upgrade pip by:\n\n```\npip3 install --upgrade pip\n```\n\n## Installation guide for developers/contributors \n\nWhen contributing to this repository, please first discuss the change you wish to make via issue, email, or any other method with the owners of this repository before making a change.\n\nPlease note we have a [code of conduct](CODE_OF_CONDUCT.md), please follow it in all your interactions with the project.\n\n### Development environment setup\n1. Clone the `schematic` package repository.\n```\ngit clone https://github.com/Sage-Bionetworks/schematic.git\n```\n2. Install `poetry` (version 1.2 or later) using either the [official installer](https://python-poetry.org/docs/#installing-with-the-official-installer) or [pipx](https://python-poetry.org/docs/#installing-with-pipx). If you have an older installation of Poetry, we recommend uninstalling it first. \n\n3. Start the virtual environment by doing: \n```\npoetry shell\n```\n4. Install the dependencies by doing: \n```\npoetry install\n```\nThis command will install the dependencies based on what we specify in poetry.lock. If this step is taking a long time, try to go back to step 2 and check your version of poetry. Alternatively, you could also try deleting the lock file and regenerate it by doing `poetry install` (Please note this method should be used as a last resort because this would force other developers to change their development environment)\n\n5. Fill in credential files: \n*Note*: If you won\'t interact with Synapse, please ignore this section.\n\nThere are two main configuration files that need to be edited:\n[config.yml](https://github.com/Sage-Bionetworks/schematic/blob/develop/config.yml)\nand [synapseConfig](https://raw.githubusercontent.com/Sage-Bionetworks/synapsePythonClient/v2.3.0-rc/synapseclient/.synapseConfig)\n\n<strong>Configure .synapseConfig File</strong>\n\nDownload a copy of the ``.synapseConfig`` file, open the file in the\neditor of your choice and edit the `username` and `authtoken` attribute under the `authentication` section \n\n*Note*: You could also visit [configparser](https://docs.python.org/3/library/configparser.html#module-configparser>) doc to see the format that `.synapseConfig` must have. For instance:\n>[authentication]<br> username = ABC <br> authtoken = abc\n\n<strong>Configure config.yml File</strong>\n\n*Note*: Below is only a brief explanation of some attributes in `config.yml`. <strong>Please use the link [here](https://github.com/Sage-Bionetworks/schematic/blob/develop/config.yml) to get the latest version of `config.yml` in `develop` branch</strong>.\n\nDescription of `config.yml` attributes\n\n    definitions:\n        synapse_config: "~/path/to/.synapseConfig"\n        service_acct_creds: "~/path/to/service_account_creds.json"\n\n    synapse:\n        master_fileview: "syn23643253" # fileview of project with datasets on Synapse\n        manifest_folder: "~/path/to/manifest_folder/" # manifests will be downloaded to this folder\n        manifest_basename: "filename" # base name of the manifest file in the project dataset, without extension\n        service_acct_creds: "syn25171627" # synapse ID of service_account_creds.json file\n\n    manifest:\n        title: "example" # title of metadata manifest file\n        # to make all manifests enter only \'all manifests\'\n        data_type: \n          - "Biospecimen"\n          - "Patient"\n\n    model:\n        input:\n            location: "data/schema_org_schemas/example.jsonld" # path to JSON-LD data model\n            file_type: "local" # only type "local" is supported currently\n    style: # configuration of google sheet\n        google_manifest:\n          req_bg_color:\n            red: 0.9215\n            green: 0.9725\n            blue: 0.9803\n          opt_bg_color:\n            red: 1.0\n            green: 1.0\n            blue: 0.9019\n          master_template_id: \'1LYS5qE4nV9jzcYw5sXwCza25slDfRA1CIg3cs-hCdpU\'\n          strict_validation: true\n\n*Note*: Paths can be specified relative to the `config.yml` file or as absolute paths.\n\n6. Login to Synapse by using the command line\nOn the CLI in your virtual environment, run the following command: \n```\nsynapse login -u <synapse username> -p <synapse password> --rememberMe\n```\nPlease make sure that you run the command before running `schematic init` below\n\n7. Obtain Google credential Files\nTo obtain  ``schematic_service_account_creds.json``, please run: \n```\nschematic init --config ~/path/to/config.yml\n```\n> As v22.12.1 version of schematic, using `token` mode of authentication (in other words, using `token.pickle` and `credentials.json`) is no longer supported due to Google\'s decision to move away from using OAuth out-of-band (OOB) flow. Click [here](https://developers.google.com/identity/protocols/oauth2/resources/oob-migration) to learn more. \n\n*Notes*: Use the ``schematic_service_account_creds.json`` file for the service\naccount mode of authentication (*for Google services/APIs*). Service accounts \nare special Google accounts that can be used by applications to access Google APIs \nprogrammatically via OAuth2.0, with the advantage being that they do not require \nhuman authorization. \n\n*Background*: schematic uses Google’s API to generate google sheet templates that users fill in to provide (meta)data.\nMost Google sheet functionality could be authenticated with service account. However, more complex Google sheet functionality\nrequires token-based authentication. As browser support that requires the token-based authentication diminishes, we are hoping to deprecate\ntoken-based authentication and keep only service account authentication in the future. \n\n\n### Development process instruction\n\nFor new features, bugs, enhancements\n\n1. Pull the latest code from [develop branch in the upstream repo](https://github.com/Sage-Bionetworks/schematic)\n2. Checkout a new branch develop-<feature/fix-name> from the develop branch\n3. Do development on branch develop-<feature/fix-name>\n   a. may need to ensure that schematic poetry toml and lock files are compatible with your local environment\n4. Add changed files for tracking and commit changes using [best practices](https://www.perforce.com/blog/vcs/git-best-practices-git-commit)\n5. Have granular commits: not “too many” file changes, and not hundreds of code lines of changes\n6. Commits with work in progress are encouraged:\n   a. add WIP to the beginning of the commit message for “Work In Progress” commits\n7. Keep commit messages descriptive but less than a page long, see best practices\n8. Push code to develop-<feature/fix-name> in upstream repo\n9. Branch out off develop-<feature/fix-name> if needed to work on multiple features associated with the same code base\n10. After feature work is complete and before creating a PR to the develop branch in upstream\n    a. ensure that code runs locally\n    b. test for logical correctness locally\n    c. wait for git workflow to complete (e.g. tests are run) on github\n11. Create a PR from develop-<feature/fix-name> into the develop branch of the upstream repo\n12. Request a code review on the PR\n13. Once code is approved merge in the develop branch\n14. Delete the develop-<feature/fix-name> branch\n\n*Note*: Make sure you have the latest version of the `develop` branch on your local machine.\n\n## Installation Guide - Docker \n\n1. Install docker from https://www.docker.com/ . <br>\n2.  Identify docker image of interest from [Schematic DockerHub](https://hub.docker.com/r/sagebionetworks/schematic/tags) <br>\n    Ex `docker pull sagebionetworks/schematic:latest` from the CLI or, run `docker compose up` after cloning the schematic github repo <br>\n    in this case, `sagebionetworks/schematic:latest` is the name of the image chosen\n3. Run Schematic Command with `docker run <flags> <schematic command and args>`. <br>\n<t> - For more information on flags for `docker run` and what they do, visit the [Docker Documentation](https://docs.docker.com/engine/reference/commandline/run/) <br>\n<t> - These example commands assume that you have navigated to the directory you want to run schematic from. To specify your working directory, use `$(pwd)` on MacOS/Linux or `%cd%` on Windows.  <br>\n<t> - If not using the latest image, then the full name should be specified: ie `sagebionetworks/schematic:commit-e611e4a` <br>\n<t> - If using local image created by `docker compose up`, then the docker image name should be changed: i.e. `schematic_schematic` <br>\n<t> - Using the `--name` flag sets the name of the container running locally on your machine <br>\n\n### Example For REST API <br>\n\n#### Use file path of `config.yml` to run API endpoints: \n```\ndocker run --rm -p 3001:3001 \\\n  -v $(pwd):/schematic -w /schematic --name schematic \\\n  -e SCHEMATIC_CONFIG=/schematic/config.yml \\\n  -e GE_HOME=/usr/src/app/great_expectations/ \\\n  sagebionetworks/schematic \\\n  python /usr/src/app/run_api.py\n``` \n\n#### Use content of `config.yml` and `schematic_service_account_creds.json`as an environment variable to run API endpoints: \n1. save content of `config.yml` as to environment variable `SCHEMATIC_CONFIG_CONTENT` by doing: `export SCHEMATIC_CONFIG_CONTENT=$(cat /path/to/config.yml)`\n\n2. Similarly, save the content of `schematic_service_account_creds.json` as `SERVICE_ACCOUNT_CREDS` by doing: `export SERVICE_ACCOUNT_CREDS=$(cat /path/to/schematic_service_account_creds.json)`\n\n3. Pass `SCHEMATIC_CONFIG_CONTENT` and `schematic_service_account_creds` as environment variables by using `docker run`\n\n```\ndocker run --rm -p 3001:3001 \\\n  -v $(pwd):/schematic -w /schematic --name schematic \\\n  -e GE_HOME=/usr/src/app/great_expectations/ \\\n  -e SCHEMATIC_CONFIG_CONTENT=$SCHEMATIC_CONFIG_CONTENT \\\n  -e SERVICE_ACCOUNT_CREDS=$SERVICE_ACCOUNT_CREDS \\\n  sagebionetworks/schematic \\\n  python /usr/src/app/run_api.py\n``` \n\n\n### Example For Schematic on mac/linux <br>\nTo run example below, first clone schematic into your home directory  `git clone https://github.com/sage-bionetworks/schematic ~/schematic` <br>\nThen update .synapseConfig with your credentials\n```\ndocker run \\\n  -v ~/schematic:/schematic \\\n  -w /schematic \\\n  -e SCHEMATIC_CONFIG=/schematic/config.yml \\\n  -e GE_HOME=/usr/src/app/great_expectations/ \\\n  sagebionetworks/schematic schematic model \\\n  -c /schematic/config.yml validate \\\n  -mp /schematic/tests/data/mock_manifests/Valid_Test_Manifest.csv \\\n  -dt MockComponent \\\n  -js /schematic/tests/data/example.model.jsonld\n``` \n\n### Example For Schematic on Windows <br>\n```\ndocker run -v %cd%:/schematic \\\n  -w /schematic \\\n  -e GE_HOME=/usr/src/app/great_expectations/ \\\n  sagebionetworks/schematic \\\n  schematic model \\\n  -c config.yml validate -mp tests/data/mock_manifests/inValid_Test_Manifest.csv -dt MockComponent -js /schematic/data/example.model.jsonld\n```\n\n# Other Contribution Guidelines\n## Updating readthedocs documentation\n1. `cd docs`\n2. After making relevant changes, you could run the `make html` command to re-generate the `build` folder.\n3. Please contact the dev team to publish your updates\n\n*Other helpful resources*:\n\n1. [Getting started with Sphinx](https://haha.readthedocs.io/en/latest/intro/getting-started-with-sphinx.html)\n2. [Installing Sphinx](https://haha.readthedocs.io/en/latest/intro/getting-started-with-sphinx.html)\n\n## Update toml file and lock file\nIf you install external libraries by using `poetry add <name of library>`, please make sure that you include `pyproject.toml` and `poetry.lock` file in your commit.\n\n## Reporting bugs or feature requests\nYou can use the [`Issues`](https://github.com/Sage-Bionetworks/schematic/issues) tab to **create bug and feature requests**. Providing enough details to the developers to verify and troubleshoot your issue is paramount:\n- **Provide a clear and descriptive title as well as a concise summary** of the issue to identify the problem.\n- **Describe the exact steps which reproduce the problem** in as many details as possible.\n- **Describe the behavior you observed after following the steps** and point out what exactly is the problem with that behavior.\n- **Explain which behavior you expected to see** instead and why.\n- **Provide screenshots of the expected or actual behaviour** where applicable.\n\n# Command Line Usage\nPlease visit more documentation [here](https://sage-schematic.readthedocs.io/en/develop/cli_reference.html)\n\n\n\n# Testing \n\nAll code added to the client must have tests. The Python client uses pytest to run tests. The test code is located in the [tests](https://github.com/Sage-Bionetworks/schematic/tree/develop-docs-update/tests) subdirectory.\n\nYou can run the test suite in the following way:\n\n```\npytest -vs tests/\n```\n\n## Updating Synapse test resources\n\n1. Duplicate the entity being updated (or folder if applicable).\n2. Edit the duplicates (_e.g._ annotations, contents, name).\n3. Update the test suite in your branch to use these duplicates, including the expected values in the test assertions.\n4. Open a PR as per the usual process (see above).\n5. Once the PR is merged, leave the original copies on Synapse to maintain support for feature branches that were forked from `develop` before your update.\n   - If the old copies are problematic and need to be removed immediately (_e.g._ contain sensitive data), proceed with the deletion and alert the other contributors that they need to merge the latest `develop` branch into their feature branches for their tests to work.\n\n# Code style\n\n* Please consult the [Google Python style guide](http://google.github.io/styleguide/pyguide.html) prior to contributing code to this project.\n* Be consistent and follow existing code conventions and spirit.\n\n\n# Contributors\n\nMain contributors and developers:\n\n- [Milen Nikolov](https://github.com/milen-sage)\n- [Mialy DeFelice](https://github.com/mialy-defelice)\n- [Sujay Patil](https://github.com/sujaypatil96)\n- [Bruno Grande](https://github.com/BrunoGrandePhD)\n- [Robert Allaway](https://github.com/allaway)\n- [Gianna Jordan](https://github.com/giajordan)\n- [Lingling Peng](https://github.com/linglp)\n',
-    'author': 'Milen Nikolov',
-    'author_email': 'milen.nikolov@sagebase.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Sage-Bionetworks/schematic',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<3.11',
-}
+# Schematic
+[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FSage-Bionetworks%2Fschematic%2Fbadge%3Fref%3Ddevelop&style=flat)](https://actions-badge.atrox.dev/Sage-Bionetworks/schematic/goto?ref=develop) [![Documentation Status](https://readthedocs.org/projects/sage-schematic/badge/?version=develop)](https://sage-schematic.readthedocs.io/en/develop/?badge=develop) [![PyPI version](https://badge.fury.io/py/schematicpy.svg)](https://badge.fury.io/py/schematicpy)
 
+# Table of contents
+- [Introduction](#introduction)
+- [Installation](#installation)
+  - [Installation Requirements](#installation-requirements)
+  - [Installation guide for data curator app](#installation-guide-for-data-curator-app)
+  - [Installation guide for developers/contributors](#installation-guide-for-developerscontributors)
+- [Other Contribution Guidelines](#other-contribution-guidelines)
+    - [Update readthedocs documentation](#update-readthedocs-documentation)
+- [Command Line Usage](#command-line-usage)
+- [Testing](#testing)
+  - [Updating Synapse test resources](#updating-synapse-test-resources)
+- [Code Style](#code-style)
+- [Contributors](#contributors)
+
+# Introduction
+SCHEMATIC is an acronym for _Schema Engine for Manifest Ingress and Curation_. The Python based infrastructure provides a _novel_ schema-based, metadata ingress ecosystem, that is meant to streamline the process of biomedical dataset annotation, metadata validation and submission to a data repository for various data contributors.
+
+# Installation
+## Installation Requirements
+* Python version 3.9.0≤x<3.11.0 
+
+Note: You need to be a registered and certified user on [`synapse.org`](https://www.synapse.org/), and also have the right permissions to download the Google credentials files from Synapse.
+
+
+## Installation guide for data curator app
+
+Create and activate a virtual environment within which you can install the package:
+
+```
+python3 -m venv .venv
+source .venv/bin/activate
+```
+
+Note: Python 3 has a built-in support for virtual environment [venv](https://docs.python.org/3/library/venv.html#module-venv) so you no longer need to install virtualenv.
+
+Install and update the package using [pip](https://pip.pypa.io/en/stable/quickstart/):
+
+```
+python3 -m pip install schematicpy
+```
+
+If you run into error: Failed building wheel for numpy, the error might be able to resolve by upgrading pip. Please try to upgrade pip by:
+
+```
+pip3 install --upgrade pip
+```
+
+## Installation guide for developers/contributors 
+
+When contributing to this repository, please first discuss the change you wish to make via issue, email, or any other method with the owners of this repository before making a change.
+
+Please note we have a [code of conduct](CODE_OF_CONDUCT.md), please follow it in all your interactions with the project.
+
+### Development environment setup
+1. Clone the `schematic` package repository.
+```
+git clone https://github.com/Sage-Bionetworks/schematic.git
+```
+2. Install `poetry` (version 1.2 or later) using either the [official installer](https://python-poetry.org/docs/#installing-with-the-official-installer) or [pipx](https://python-poetry.org/docs/#installing-with-pipx). If you have an older installation of Poetry, we recommend uninstalling it first. 
+
+3. Start the virtual environment by doing: 
+```
+poetry shell
+```
+4. Install the dependencies by doing: 
+```
+poetry install
+```
+This command will install the dependencies based on what we specify in poetry.lock. If this step is taking a long time, try to go back to step 2 and check your version of poetry. Alternatively, you could also try deleting the lock file and regenerate it by doing `poetry install` (Please note this method should be used as a last resort because this would force other developers to change their development environment)
+
+5. Fill in credential files: 
+*Note*: If you won't interact with Synapse, please ignore this section.
+
+There are two main configuration files that need to be edited:
+[config.yml](https://github.com/Sage-Bionetworks/schematic/blob/develop/config.yml)
+and [synapseConfig](https://raw.githubusercontent.com/Sage-Bionetworks/synapsePythonClient/v2.3.0-rc/synapseclient/.synapseConfig)
+
+<strong>Configure .synapseConfig File</strong>
+
+Download a copy of the ``.synapseConfig`` file, open the file in the
+editor of your choice and edit the `username` and `authtoken` attribute under the `authentication` section 
+
+*Note*: You could also visit [configparser](https://docs.python.org/3/library/configparser.html#module-configparser>) doc to see the format that `.synapseConfig` must have. For instance:
+>[authentication]<br> username = ABC <br> authtoken = abc
+
+<strong>Configure config.yml File</strong>
+
+*Note*: Below is only a brief explanation of some attributes in `config.yml`. <strong>Please use the link [here](https://github.com/Sage-Bionetworks/schematic/blob/develop/config.yml) to get the latest version of `config.yml` in `develop` branch</strong>.
+
+Description of `config.yml` attributes
+
+    definitions:
+        synapse_config: "~/path/to/.synapseConfig"
+        service_acct_creds: "~/path/to/service_account_creds.json"
+
+    synapse:
+        master_fileview: "syn23643253" # fileview of project with datasets on Synapse
+        manifest_folder: "~/path/to/manifest_folder/" # manifests will be downloaded to this folder
+        manifest_basename: "filename" # base name of the manifest file in the project dataset, without extension
+        service_acct_creds: "syn25171627" # synapse ID of service_account_creds.json file
+
+    manifest:
+        title: "example" # title of metadata manifest file
+        # to make all manifests enter only 'all manifests'
+        data_type: 
+          - "Biospecimen"
+          - "Patient"
+
+    model:
+        input:
+            location: "data/schema_org_schemas/example.jsonld" # path to JSON-LD data model
+            file_type: "local" # only type "local" is supported currently
+    style: # configuration of google sheet
+        google_manifest:
+          req_bg_color:
+            red: 0.9215
+            green: 0.9725
+            blue: 0.9803
+          opt_bg_color:
+            red: 1.0
+            green: 1.0
+            blue: 0.9019
+          master_template_id: '1LYS5qE4nV9jzcYw5sXwCza25slDfRA1CIg3cs-hCdpU'
+          strict_validation: true
+
+*Note*: Paths can be specified relative to the `config.yml` file or as absolute paths.
+
+6. Login to Synapse by using the command line
+On the CLI in your virtual environment, run the following command: 
+```
+synapse login -u <synapse username> -p <synapse password> --rememberMe
+```
+Please make sure that you run the command before running `schematic init` below
+
+7. Obtain Google credential Files
+To obtain  ``schematic_service_account_creds.json``, please run: 
+```
+schematic init --config ~/path/to/config.yml
+```
+> As v22.12.1 version of schematic, using `token` mode of authentication (in other words, using `token.pickle` and `credentials.json`) is no longer supported due to Google's decision to move away from using OAuth out-of-band (OOB) flow. Click [here](https://developers.google.com/identity/protocols/oauth2/resources/oob-migration) to learn more. 
+
+*Notes*: Use the ``schematic_service_account_creds.json`` file for the service
+account mode of authentication (*for Google services/APIs*). Service accounts 
+are special Google accounts that can be used by applications to access Google APIs 
+programmatically via OAuth2.0, with the advantage being that they do not require 
+human authorization. 
+
+*Background*: schematic uses Google’s API to generate google sheet templates that users fill in to provide (meta)data.
+Most Google sheet functionality could be authenticated with service account. However, more complex Google sheet functionality
+requires token-based authentication. As browser support that requires the token-based authentication diminishes, we are hoping to deprecate
+token-based authentication and keep only service account authentication in the future. 
+
+
+### Development process instruction
+
+For new features, bugs, enhancements
+
+1. Pull the latest code from [develop branch in the upstream repo](https://github.com/Sage-Bionetworks/schematic)
+2. Checkout a new branch develop-<feature/fix-name> from the develop branch
+3. Do development on branch develop-<feature/fix-name>
+   a. may need to ensure that schematic poetry toml and lock files are compatible with your local environment
+4. Add changed files for tracking and commit changes using [best practices](https://www.perforce.com/blog/vcs/git-best-practices-git-commit)
+5. Have granular commits: not “too many” file changes, and not hundreds of code lines of changes
+6. Commits with work in progress are encouraged:
+   a. add WIP to the beginning of the commit message for “Work In Progress” commits
+7. Keep commit messages descriptive but less than a page long, see best practices
+8. Push code to develop-<feature/fix-name> in upstream repo
+9. Branch out off develop-<feature/fix-name> if needed to work on multiple features associated with the same code base
+10. After feature work is complete and before creating a PR to the develop branch in upstream
+    a. ensure that code runs locally
+    b. test for logical correctness locally
+    c. wait for git workflow to complete (e.g. tests are run) on github
+11. Create a PR from develop-<feature/fix-name> into the develop branch of the upstream repo
+12. Request a code review on the PR
+13. Once code is approved merge in the develop branch
+14. Delete the develop-<feature/fix-name> branch
+
+*Note*: Make sure you have the latest version of the `develop` branch on your local machine.
+
+## Installation Guide - Docker 
+
+1. Install docker from https://www.docker.com/ . <br>
+2.  Identify docker image of interest from [Schematic DockerHub](https://hub.docker.com/r/sagebionetworks/schematic/tags) <br>
+    Ex `docker pull sagebionetworks/schematic:latest` from the CLI or, run `docker compose up` after cloning the schematic github repo <br>
+    in this case, `sagebionetworks/schematic:latest` is the name of the image chosen
+3. Run Schematic Command with `docker run <flags> <schematic command and args>`. <br>
+<t> - For more information on flags for `docker run` and what they do, visit the [Docker Documentation](https://docs.docker.com/engine/reference/commandline/run/) <br>
+<t> - These example commands assume that you have navigated to the directory you want to run schematic from. To specify your working directory, use `$(pwd)` on MacOS/Linux or `%cd%` on Windows.  <br>
+<t> - If not using the latest image, then the full name should be specified: ie `sagebionetworks/schematic:commit-e611e4a` <br>
+<t> - If using local image created by `docker compose up`, then the docker image name should be changed: i.e. `schematic_schematic` <br>
+<t> - Using the `--name` flag sets the name of the container running locally on your machine <br>
+
+### Example For REST API <br>
+
+#### Use file path of `config.yml` to run API endpoints: 
+```
+docker run --rm -p 3001:3001 \
+  -v $(pwd):/schematic -w /schematic --name schematic \
+  -e SCHEMATIC_CONFIG=/schematic/config.yml \
+  -e GE_HOME=/usr/src/app/great_expectations/ \
+  sagebionetworks/schematic \
+  python /usr/src/app/run_api.py
+``` 
+
+#### Use content of `config.yml` and `schematic_service_account_creds.json`as an environment variable to run API endpoints: 
+1. save content of `config.yml` as to environment variable `SCHEMATIC_CONFIG_CONTENT` by doing: `export SCHEMATIC_CONFIG_CONTENT=$(cat /path/to/config.yml)`
+
+2. Similarly, save the content of `schematic_service_account_creds.json` as `SERVICE_ACCOUNT_CREDS` by doing: `export SERVICE_ACCOUNT_CREDS=$(cat /path/to/schematic_service_account_creds.json)`
+
+3. Pass `SCHEMATIC_CONFIG_CONTENT` and `schematic_service_account_creds` as environment variables by using `docker run`
+
+```
+docker run --rm -p 3001:3001 \
+  -v $(pwd):/schematic -w /schematic --name schematic \
+  -e GE_HOME=/usr/src/app/great_expectations/ \
+  -e SCHEMATIC_CONFIG_CONTENT=$SCHEMATIC_CONFIG_CONTENT \
+  -e SERVICE_ACCOUNT_CREDS=$SERVICE_ACCOUNT_CREDS \
+  sagebionetworks/schematic \
+  python /usr/src/app/run_api.py
+``` 
+
+
+### Example For Schematic on mac/linux <br>
+To run example below, first clone schematic into your home directory  `git clone https://github.com/sage-bionetworks/schematic ~/schematic` <br>
+Then update .synapseConfig with your credentials
+```
+docker run \
+  -v ~/schematic:/schematic \
+  -w /schematic \
+  -e SCHEMATIC_CONFIG=/schematic/config.yml \
+  -e GE_HOME=/usr/src/app/great_expectations/ \
+  sagebionetworks/schematic schematic model \
+  -c /schematic/config.yml validate \
+  -mp /schematic/tests/data/mock_manifests/Valid_Test_Manifest.csv \
+  -dt MockComponent \
+  -js /schematic/tests/data/example.model.jsonld
+``` 
+
+### Example For Schematic on Windows <br>
+```
+docker run -v %cd%:/schematic \
+  -w /schematic \
+  -e GE_HOME=/usr/src/app/great_expectations/ \
+  sagebionetworks/schematic \
+  schematic model \
+  -c config.yml validate -mp tests/data/mock_manifests/inValid_Test_Manifest.csv -dt MockComponent -js /schematic/data/example.model.jsonld
+```
+
+# Other Contribution Guidelines
+## Updating readthedocs documentation
+1. `cd docs`
+2. After making relevant changes, you could run the `make html` command to re-generate the `build` folder.
+3. Please contact the dev team to publish your updates
+
+*Other helpful resources*:
+
+1. [Getting started with Sphinx](https://haha.readthedocs.io/en/latest/intro/getting-started-with-sphinx.html)
+2. [Installing Sphinx](https://haha.readthedocs.io/en/latest/intro/getting-started-with-sphinx.html)
+
+## Update toml file and lock file
+If you install external libraries by using `poetry add <name of library>`, please make sure that you include `pyproject.toml` and `poetry.lock` file in your commit.
+
+## Reporting bugs or feature requests
+You can use the [`Issues`](https://github.com/Sage-Bionetworks/schematic/issues) tab to **create bug and feature requests**. Providing enough details to the developers to verify and troubleshoot your issue is paramount:
+- **Provide a clear and descriptive title as well as a concise summary** of the issue to identify the problem.
+- **Describe the exact steps which reproduce the problem** in as many details as possible.
+- **Describe the behavior you observed after following the steps** and point out what exactly is the problem with that behavior.
+- **Explain which behavior you expected to see** instead and why.
+- **Provide screenshots of the expected or actual behaviour** where applicable.
+
+# Command Line Usage
+Please visit more documentation [here](https://sage-schematic.readthedocs.io/en/develop/cli_reference.html)
+
+
+
+# Testing 
+
+All code added to the client must have tests. The Python client uses pytest to run tests. The test code is located in the [tests](https://github.com/Sage-Bionetworks/schematic/tree/develop-docs-update/tests) subdirectory.
+
+You can run the test suite in the following way:
+
+```
+pytest -vs tests/
+```
+
+## Updating Synapse test resources
+
+1. Duplicate the entity being updated (or folder if applicable).
+2. Edit the duplicates (_e.g._ annotations, contents, name).
+3. Update the test suite in your branch to use these duplicates, including the expected values in the test assertions.
+4. Open a PR as per the usual process (see above).
+5. Once the PR is merged, leave the original copies on Synapse to maintain support for feature branches that were forked from `develop` before your update.
+   - If the old copies are problematic and need to be removed immediately (_e.g._ contain sensitive data), proceed with the deletion and alert the other contributors that they need to merge the latest `develop` branch into their feature branches for their tests to work.
+
+# Code style
+
+* Please consult the [Google Python style guide](http://google.github.io/styleguide/pyguide.html) prior to contributing code to this project.
+* Be consistent and follow existing code conventions and spirit.
+
+
+# Contributors
+
+Main contributors and developers:
+
+- [Milen Nikolov](https://github.com/milen-sage)
+- [Mialy DeFelice](https://github.com/mialy-defelice)
+- [Sujay Patil](https://github.com/sujaypatil96)
+- [Bruno Grande](https://github.com/BrunoGrandePhD)
+- [Robert Allaway](https://github.com/allaway)
+- [Gianna Jordan](https://github.com/giajordan)
+- [Lingling Peng](https://github.com/linglp)
 
-setup(**setup_kwargs)
```

