# Comparing `tmp/kiara_plugin.service-0.4.0.tar.gz` & `tmp/kiara_plugin.service-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.service-0.4.0.tar", last modified: Wed Jun 14 14:49:32 2023, max compression
+gzip compressed data, was "kiara_plugin.service-0.4.1.tar", last modified: Fri Jun 16 07:21:04 2023, max compression
```

## Comparing `kiara_plugin.service-0.4.0.tar` & `kiara_plugin.service-0.4.1.tar`

### file list

```diff
@@ -1,134 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.919880 kiara_plugin.service-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.887880 kiara_plugin.service-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.899880 kiara_plugin.service-0.4.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.899880 kiara_plugin.service-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-06-14 14:49:32.919880 kiara_plugin.service-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.887880 kiara_plugin.service-0.4.0/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.899880 kiara_plugin.service-0.4.0/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/ci/conda/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.899880 kiara_plugin.service-0.4.0/ci/conda/kiara_plugin.service/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/ci/conda/kiara_plugin.service/meta.yaml.template
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.903880 kiara_plugin.service-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.903880 kiara_plugin.service-0.4.0/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.887880 kiara_plugin.service-0.4.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.903880 kiara_plugin.service-0.4.0/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.903880 kiara_plugin.service-0.4.0/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.903880 kiara_plugin.service-0.4.0/examples/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/examples/jobs/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.903880 kiara_plugin.service-0.4.0/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/examples/pipelines/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/examples/pipelines/example_pipeline_service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.891880 kiara_plugin.service-0.4.0/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.907880 kiara_plugin.service-0.4.0/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-14 14:49:32.923879 kiara_plugin.service-0.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.891880 kiara_plugin.service-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.891880 kiara_plugin.service-0.4.0/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.907880 kiara_plugin.service-0.4.0/src/kiara_plugin/service/
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.907880 kiara_plugin.service-0.4.0/src/kiara_plugin/service/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.911880 kiara_plugin.service-0.4.0/src/kiara_plugin/service/interfaces/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/interfaces/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.911880 kiara_plugin.service-0.4.0/src/kiara_plugin/service/interfaces/cli/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/interfaces/cli/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/interfaces/cli/service/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.911880 kiara_plugin.service-0.4.0/src/kiara_plugin/service/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.911880 kiara_plugin.service-0.4.0/src/kiara_plugin/service/openapi/
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/openapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.911880 kiara_plugin.service-0.4.0/src/kiara_plugin/service/openapi/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/openapi/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/openapi/controllers/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/openapi/controllers/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/openapi/controllers/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/openapi/controllers/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     9575 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/openapi/controllers/values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/openapi/controllers/workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/openapi/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.915880 kiara_plugin.service-0.4.0/src/kiara_plugin/service/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.915880 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.915880 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/static/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/static/input.css
--rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/static/main.css
--rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/static/simple.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.915880 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.915880 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/jobs/job_finished.html
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/jobs/job_monitor.html
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/macros.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.919880 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/operations/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/operations/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/operations/operation_view.html
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/operations/operations.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.919880 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/values/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/values/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.919880 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/values/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/values/inputs/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/values/inputs/base_scalar.html
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/values/inputs/boolean.html
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/values/inputs/generic-scalar.html
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/values/inputs/generic.html
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/values/inputs/table.html
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/values/value_inputs_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/values/value_select.html
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/values/value_view.html
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/values/values.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.907880 kiara_plugin.service-0.4.0/src/kiara_plugin.service.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-06-14 14:49:32.000000 kiara_plugin.service-0.4.0/src/kiara_plugin.service.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-14 14:49:32.000000 kiara_plugin.service-0.4.0/src/kiara_plugin.service.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:49:32.000000 kiara_plugin.service-0.4.0/src/kiara_plugin.service.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-14 14:49:32.000000 kiara_plugin.service-0.4.0/src/kiara_plugin.service.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:49:03.000000 kiara_plugin.service-0.4.0/src/kiara_plugin.service.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-14 14:49:32.000000 kiara_plugin.service-0.4.0/src/kiara_plugin.service.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 14:49:32.000000 kiara_plugin.service-0.4.0/src/kiara_plugin.service.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/tailwind.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.919880 kiara_plugin.service-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:49:32.919880 kiara_plugin.service-0.4.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/tests/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/tests/test_job_descs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      227 2023-06-14 14:48:53.000000 kiara_plugin.service-0.4.0/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.848020 kiara_plugin.service-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.836020 kiara_plugin.service-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.840020 kiara_plugin.service-0.4.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.840020 kiara_plugin.service-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-06-16 07:21:04.848020 kiara_plugin.service-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.836020 kiara_plugin.service-0.4.1/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.840020 kiara_plugin.service-0.4.1/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/ci/conda/conda-pkg-patch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.840020 kiara_plugin.service-0.4.1/ci/conda/kiara_plugin.service/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/ci/conda/kiara_plugin.service/meta.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.840020 kiara_plugin.service-0.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.840020 kiara_plugin.service-0.4.1/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.836020 kiara_plugin.service-0.4.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.840020 kiara_plugin.service-0.4.1/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.840020 kiara_plugin.service-0.4.1/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.840020 kiara_plugin.service-0.4.1/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/examples/jobs/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.840020 kiara_plugin.service-0.4.1/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/examples/pipelines/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/examples/pipelines/example_pipeline_service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.836020 kiara_plugin.service-0.4.1/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.840020 kiara_plugin.service-0.4.1/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-16 07:21:04.848020 kiara_plugin.service-0.4.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.836020 kiara_plugin.service-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.836020 kiara_plugin.service-0.4.1/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/interfaces/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/interfaces/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/interfaces/cli/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/interfaces/cli/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/interfaces/cli/service/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10324 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/static/input.css
+-rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/static/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/static/simple.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/jobs/job_finished.html
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/jobs/job_monitor.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/macros.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.848020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/operations/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/operations/operation_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/operations/operations.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.848020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.848020 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/inputs/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/inputs/base_scalar.html
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/inputs/boolean.html
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/inputs/generic-scalar.html
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/inputs/generic.html
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/inputs/table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/value_inputs_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/value_select.html
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/value_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/values.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.844020 kiara_plugin.service-0.4.1/src/kiara_plugin.service.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-06-16 07:21:04.000000 kiara_plugin.service-0.4.1/src/kiara_plugin.service.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-06-16 07:21:04.000000 kiara_plugin.service-0.4.1/src/kiara_plugin.service.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:21:04.000000 kiara_plugin.service-0.4.1/src/kiara_plugin.service.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-16 07:21:04.000000 kiara_plugin.service-0.4.1/src/kiara_plugin.service.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:20:37.000000 kiara_plugin.service-0.4.1/src/kiara_plugin.service.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-16 07:21:04.000000 kiara_plugin.service-0.4.1/src/kiara_plugin.service.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 07:21:04.000000 kiara_plugin.service-0.4.1/src/kiara_plugin.service.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/tailwind.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.848020 kiara_plugin.service-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:21:04.848020 kiara_plugin.service-0.4.1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/tests/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      227 2023-06-16 07:20:29.000000 kiara_plugin.service-0.4.1/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.service-0.4.0/.cruft.json` & `kiara_plugin.service-0.4.1/.cruft.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin.service-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin.service-0.4.1/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/.github/workflows/build-darwin.yaml` & `kiara_plugin.service-0.4.1/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/.github/workflows/build-linux.yaml` & `kiara_plugin.service-0.4.1/.github/workflows/build-linux.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/.github/workflows/build-windows.yaml` & `kiara_plugin.service-0.4.1/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/.gitignore` & `kiara_plugin.service-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/.pre-commit-config.yaml` & `kiara_plugin.service-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/LICENSE` & `kiara_plugin.service-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/Makefile` & `kiara_plugin.service-0.4.1/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/PKG-INFO` & `kiara_plugin.service-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.service
-Version: 0.4.0
+Version: 0.4.1
 Summary: A plugin to create, run and manage a service for kiara functionality.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.service
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.service
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.service
 Keywords: kiara
```

### Comparing `kiara_plugin.service-0.4.0/README.md` & `kiara_plugin.service-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/ci/conda/kiara_plugin.service/meta.yaml.template` & `kiara_plugin.service-0.4.1/ci/conda/kiara_plugin.service/meta.yaml.template`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/docs/development.md` & `kiara_plugin.service-0.4.1/docs/development.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/docs/index.md` & `kiara_plugin.service-0.4.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin.service-0.4.1/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin.service-0.4.1/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/examples/pipelines/example_pipeline_service.yaml` & `kiara_plugin.service-0.4.1/examples/pipelines/example_pipeline_service.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/mkdocs.yml` & `kiara_plugin.service-0.4.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/pyproject.toml` & `kiara_plugin.service-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 dependencies = [
-    "kiara>=0.4.40",
+    "kiara>=0.4.41",
     "kiara_plugin.core_types>=0.4.18",
     "starlite==1.39.0"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev_documentation = [
```

### Comparing `kiara_plugin.service-0.4.0/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin.service-0.4.1/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/scripts/documentation/gen_info_pages.py` & `kiara_plugin.service-0.4.1/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/scripts/documentation/gen_module_doc.py` & `kiara_plugin.service-0.4.1/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/setup.cfg` & `kiara_plugin.service-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/setup.py` & `kiara_plugin.service-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/src/kiara_plugin/service/__init__.py` & `kiara_plugin.service-0.4.1/src/kiara_plugin/service/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/src/kiara_plugin/service/defaults.py` & `kiara_plugin.service-0.4.1/src/kiara_plugin/service/defaults.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/src/kiara_plugin/service/interfaces/cli/service/commands.py` & `kiara_plugin.service-0.4.1/src/kiara_plugin/service/interfaces/cli/service/commands.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/src/kiara_plugin/service/models.py` & `kiara_plugin.service-0.4.1/src/kiara_plugin/service/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/src/kiara_plugin/service/modules/__init__.py` & `kiara_plugin.service-0.4.1/src/kiara_plugin/service/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/src/kiara_plugin/service/openapi/__init__.py` & `kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/src/kiara_plugin/service/openapi/controllers/jobs.py` & `kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/jobs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 from typing import Any, Mapping
 
 from pydantic import BaseModel, Extra, Field
-from starlite import Controller, get, post
+from starlite import Controller
 
 from kiara.api import KiaraAPI
 from kiara.models.module.jobs import ActiveJob
+from kiara_plugin.service.openapi.controllers import get, post
 
 
 class RunJobRequest(BaseModel):
     class Config:
         extra = Extra.allow
 
     operation_id: str = Field(description="The id of the operation or module.")
@@ -23,15 +24,15 @@
 
     job_id: str = Field(description="The id of the job to monitor.")
 
 
 class JobControllerJson(Controller):
     path = "/"
 
-    @post(path="/queue_job")
+    @post(path="/queue_job", api_func=KiaraAPI.queue_job)
     async def queue_job(self, kiara_api: KiaraAPI, data: RunJobRequest) -> ActiveJob:
 
         print(f"JOB RUN REQUEST: {data.dict()}")
 
         try:
             operation_id = data.operation_id
             if not data.operation_config:
@@ -47,15 +48,15 @@
 
         except Exception as e:
             import traceback
 
             traceback.print_exc()
             raise e
 
-    @get(path="/monitor_job/{job_id:str}")
+    @get(path="/monitor_job/{job_id:str}", api_func=KiaraAPI.get_job)
     async def monitor_job(self, kiara_api: KiaraAPI, job_id: str) -> ActiveJob:
 
         print(f"MONITOR REQUEST: {job_id}")
 
         job = kiara_api.get_job(job_id=job_id)
 
         return job
```

### Comparing `kiara_plugin.service-0.4.0/src/kiara_plugin/service/openapi/controllers/operations.py` & `kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/operations.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,18 @@
 # -*- coding: utf-8 -*-
-import uuid
 from typing import Dict, List, Union
 
 from pydantic import BaseModel, Extra, Field
 from starlite import (
-    Body,
     Controller,
-    MediaType,
-    RequestEncodingType,
-    Template,
-    get,
-    post,
 )
 
-from kiara.api import Kiara, KiaraAPI
+from kiara.api import KiaraAPI
 from kiara.interfaces.python_api import OperationInfo
-from kiara.models.module.jobs import JobStatus
-from kiara.models.values.value import ValueMap
-from kiara.registries.templates import TemplateRegistry
+from kiara_plugin.service.openapi.controllers import get, post
 
 
 class OperationRequest(BaseModel):
     element_id: str = Field(description="The id of the element to be created.")
     operation_id: str = Field(description="The id of the operation.")
 
 
@@ -45,191 +36,207 @@
         description="The (optional) filter strings, an operation must match all of them to be included in the result.",
         default_factory=list,
     )
     include_internal: bool = Field(
         description="Whether to include internal operations in the result.",
         default=False,
     )
+    python_package: Union[str, None] = Field(
+        description="If specified, only operations that are contained in this Python package are returned.",
+        default=None,
+    )
 
 
 class OperationControllerJson(Controller):
     path = "/"
 
-    @post(path="/")
+    @post(path="/", api_func=KiaraAPI.retrieve_operations_info)
     async def list_operations(
         self, kiara_api: KiaraAPI, data: OperationMatcher
     ) -> Dict[str, OperationInfo]:
 
         filters = data.filters
         include_internal = data.include_internal
 
+        if data.python_package is not None:
+            python_packages = [data.python_package]
+        else:
+            python_packages = None
+
         operations = kiara_api.retrieve_operations_info(
-            *filters, include_internal=include_internal
+            *filters, include_internal=include_internal, python_packages=python_packages
         )
         return operations.item_infos  # type: ignore
 
-    @post(path="/ids")
+    @post(path="/ids", api_func=KiaraAPI.list_operation_ids)
     async def list_operation_ids(
         self, kiara_api: KiaraAPI, data: OperationMatcher
     ) -> List[str]:
         """List the ids of all available operations."""
 
         filters = data.filters
         include_internal = data.include_internal
 
+        if data.python_package is not None:
+            python_packages = [data.python_package]
+        else:
+            python_packages = None
+
         operation_ids = kiara_api.list_operation_ids(
-            filter=filters, include_internal=include_internal
+            filter=filters,
+            include_internal=include_internal,
+            python_packages=python_packages,
         )
         return operation_ids
 
-    @get(path="/{operation_id:str}")
+    @get(path="/{operation_id:str}", api_func=KiaraAPI.retrieve_operation_info)
     async def get_operation_info(
         self, kiara_api: KiaraAPI, operation_id: str
     ) -> OperationInfo:
 
         op = kiara_api.retrieve_operation_info(operation=operation_id)
         return op
 
 
-class OperationControllerHtmx(Controller):
-    path = "/"
-
-    @get(path="/", media_type=MediaType.HTML)
-    async def get_root_page(self, kiara: Kiara) -> Template:
-
-        print("OPERATION ROOT REQUEST")
-        return Template(
-            name="kiara_plugin.service/operations/index.html", context={"kiara": kiara}
-        )
-
-    @post(path="/operation_info", media_type=MediaType.HTML)
-    async def render_operation_info(
-        self,
-        kiara_api: KiaraAPI,
-        data: OperationRequest = Body(media_type=RequestEncodingType.URL_ENCODED),
-    ) -> Template:
-
-        print(f"Operation info request: {data}")
-
-        op_info = kiara_api.retrieve_operation_info(operation=data.operation_id)
-
-        return Template(
-            name="kiara_plugin.service/operations/operation_view.html",
-            context={"element_id": data.element_id, "operation_info": op_info},
-        )
-
-    @post(path="/inputs_form", media_type=MediaType.HTML)
-    async def get_input_form(
-        self,
-        kiara_api: KiaraAPI,
-        template_registry: TemplateRegistry,
-        data: OperationRequest = Body(media_type=RequestEncodingType.URL_ENCODED),
-    ) -> Template:
-
-        print(f"INPUTS FORM REQUEST: {data}")
-        op = kiara_api.get_operation(data.operation_id)
-
-        fields = {}
-        for field_name, schema in op.inputs_schema.items():
-
-            data_type_cls = kiara_api.context.type_registry.get_data_type_cls(
-                type_name=schema.type
-            )
-
-            template_name = f"kiara_plugin.service/values/inputs/{schema.type}.html"
-            if template_name not in template_registry.template_names:
-                data_type_instance = data_type_cls(**schema.type_config)
-                if data_type_instance.characteristics.is_scalar:
-                    template_name = (
-                        "kiara_plugin.service/values/inputs/generic-scalar.html"
-                    )
-                else:
-                    template_name = "kiara_plugin.service/values/inputs/generic.html"
-            try:
-                template = template_registry.get_template(template_name)
-                rendered = template.render(
-                    field_name=field_name,
-                    data_type=schema.type,
-                    desc=schema.doc.description,
-                    doc=schema.doc.doc,
-                )
-            except Exception as e:
-                import traceback
-
-                traceback.print_exc()
-                rendered = str(e)
-
-            fields[field_name] = rendered
-
-        return Template(
-            name="kiara_plugin.service/values/value_inputs_form.html",
-            context={"fields": fields},
-        )
-
-    @post(path="/queue_job", media_type=MediaType.HTML)
-    async def queue_job(
-        self,
-        kiara_api: KiaraAPI,
-        data: OperationRunRequest = Body(media_type=RequestEncodingType.URL_ENCODED),
-    ) -> Union[Template, str]:
-
-        print(f"RUN REQUEST: {data.dict()}")
-
-        try:
-            inputs = data.dict()
-            operation_id = inputs.pop("operation_id")
-            element_id = inputs.pop("element_id")
-
-            # because html forms don't send values for unchecked boxes
-            op = kiara_api.get_operation(operation_id)
-            for field_name, schema in op.inputs_schema.items():
-                if field_name not in inputs.keys():
-                    if schema.type == "boolean":
-                        inputs[field_name] = False
-
-            job_id = kiara_api.queue_job(operation=operation_id, inputs=inputs)
-
-            job = kiara_api.get_job(job_id=job_id)
-            return Template(
-                name="kiara_plugin.service/jobs/job_monitor.html",
-                context={"job": job, "element_id": element_id},
-            )
-
-        except Exception as e:
-            import traceback
-
-            traceback.print_exc()
-            return f"<div>Can't submit job: {e}"
-
-    @post(path="/monitor_job", media_type=MediaType.HTML)
-    async def monitor_job(
-        self,
-        kiara_api: KiaraAPI,
-        data: MonitorJobRequest = Body(media_type=RequestEncodingType.URL_ENCODED),
-    ) -> Template:
-
-        print(f"MONITOR REQUEST: {data.dict()}")
-
-        job_id = uuid.UUID(data.job_id)
-        job = kiara_api.get_job(job_id=job_id)
-
-        if job.finished is None:
-            return Template(
-                name="kiara_plugin.service/jobs/job_monitor.html",
-                context={"job": job, "element_id": data.element_id},
-            )
-        else:
-            if job.status == JobStatus.SUCCESS:
-                results: Union[Dict, ValueMap] = kiara_api.get_job_result(job_id)
-                error = None
-            else:
-                results = {}
-                error = job.error
-            return Template(
-                name="kiara_plugin.service/jobs/job_finished.html",
-                context={
-                    "job": job,
-                    "element_id": data.element_id,
-                    "results": results,
-                    "error": error,
-                },
-            )
+# class OperationControllerHtmx(Controller):
+#     path = "/"
+#
+#     @get(path="/", media_type=MediaType.HTML)
+#     async def get_root_page(self, kiara: Kiara) -> Template:
+#
+#         print("OPERATION ROOT REQUEST")
+#         return Template(
+#             name="kiara_plugin.service/operations/index.html", context={"kiara": kiara}
+#         )
+#
+#     @post(path="/operation_info", media_type=MediaType.HTML)
+#     async def render_operation_info(
+#         self,
+#         kiara_api: KiaraAPI,
+#         data: OperationRequest = Body(media_type=RequestEncodingType.URL_ENCODED),
+#     ) -> Template:
+#
+#         print(f"Operation info request: {data}")
+#
+#         op_info = kiara_api.retrieve_operation_info(operation=data.operation_id)
+#
+#         return Template(
+#             name="kiara_plugin.service/operations/operation_view.html",
+#             context={"element_id": data.element_id, "operation_info": op_info},
+#         )
+#
+#     @post(path="/inputs_form", media_type=MediaType.HTML)
+#     async def get_input_form(
+#         self,
+#         kiara_api: KiaraAPI,
+#         template_registry: TemplateRegistry,
+#         data: OperationRequest = Body(media_type=RequestEncodingType.URL_ENCODED),
+#     ) -> Template:
+#
+#         print(f"INPUTS FORM REQUEST: {data}")
+#         op = kiara_api.get_operation(data.operation_id)
+#
+#         fields = {}
+#         for field_name, schema in op.inputs_schema.items():
+#
+#             data_type_cls = kiara_api.context.type_registry.get_data_type_cls(
+#                 type_name=schema.type
+#             )
+#
+#             template_name = f"kiara_plugin.service/values/inputs/{schema.type}.html"
+#             if template_name not in template_registry.template_names:
+#                 data_type_instance = data_type_cls(**schema.type_config)
+#                 if data_type_instance.characteristics.is_scalar:
+#                     template_name = (
+#                         "kiara_plugin.service/values/inputs/generic-scalar.html"
+#                     )
+#                 else:
+#                     template_name = "kiara_plugin.service/values/inputs/generic.html"
+#             try:
+#                 template = template_registry.get_template(template_name)
+#                 rendered = template.render(
+#                     field_name=field_name,
+#                     data_type=schema.type,
+#                     desc=schema.doc.description,
+#                     doc=schema.doc.doc,
+#                 )
+#             except Exception as e:
+#                 import traceback
+#
+#                 traceback.print_exc()
+#                 rendered = str(e)
+#
+#             fields[field_name] = rendered
+#
+#         return Template(
+#             name="kiara_plugin.service/values/value_inputs_form.html",
+#             context={"fields": fields},
+#         )
+#
+#     @post(path="/queue_job", media_type=MediaType.HTML)
+#     async def queue_job(
+#         self,
+#         kiara_api: KiaraAPI,
+#         data: OperationRunRequest = Body(media_type=RequestEncodingType.URL_ENCODED),
+#     ) -> Union[Template, str]:
+#
+#         print(f"RUN REQUEST: {data.dict()}")
+#
+#         try:
+#             inputs = data.dict()
+#             operation_id = inputs.pop("operation_id")
+#             element_id = inputs.pop("element_id")
+#
+#             # because html forms don't send values for unchecked boxes
+#             op = kiara_api.get_operation(operation_id)
+#             for field_name, schema in op.inputs_schema.items():
+#                 if field_name not in inputs.keys():
+#                     if schema.type == "boolean":
+#                         inputs[field_name] = False
+#
+#             job_id = kiara_api.queue_job(operation=operation_id, inputs=inputs)
+#
+#             job = kiara_api.get_job(job_id=job_id)
+#             return Template(
+#                 name="kiara_plugin.service/jobs/job_monitor.html",
+#                 context={"job": job, "element_id": element_id},
+#             )
+#
+#         except Exception as e:
+#             import traceback
+#
+#             traceback.print_exc()
+#             return f"<div>Can't submit job: {e}"
+#
+#     @post(path="/monitor_job", media_type=MediaType.HTML)
+#     async def monitor_job(
+#         self,
+#         kiara_api: KiaraAPI,
+#         data: MonitorJobRequest = Body(media_type=RequestEncodingType.URL_ENCODED),
+#     ) -> Template:
+#
+#         print(f"MONITOR REQUEST: {data.dict()}")
+#
+#         job_id = uuid.UUID(data.job_id)
+#         job = kiara_api.get_job(job_id=job_id)
+#
+#         if job.finished is None:
+#             return Template(
+#                 name="kiara_plugin.service/jobs/job_monitor.html",
+#                 context={"job": job, "element_id": data.element_id},
+#             )
+#         else:
+#             if job.status == JobStatus.SUCCESS:
+#                 results: Union[Dict, ValueMap] = kiara_api.get_job_result(job_id)
+#                 error = None
+#             else:
+#                 results = {}
+#                 error = job.error
+#             return Template(
+#                 name="kiara_plugin.service/jobs/job_finished.html",
+#                 context={
+#                     "job": job,
+#                     "element_id": data.element_id,
+#                     "results": results,
+#                     "error": error,
+#                 },
+#             )
```

### Comparing `kiara_plugin.service-0.4.0/src/kiara_plugin/service/openapi/controllers/render.py` & `kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/render.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 # -*- coding: utf-8 -*-
 from typing import Any, Dict, List, Mapping, Union
 
 from pydantic import BaseModel, Field
-from starlite import Controller, get, post
+from starlite import Controller
 
 from kiara.api import KiaraAPI, ValueSchema
 from kiara.models.module.operation import Operation
 from kiara.models.rendering import RenderValueResult
+from kiara_plugin.service.openapi.controllers import get, post
 
 
 class InputsValidationData(BaseModel):
 
     inputs: Mapping[str, Any] = Field(description="The provided inputs.")
     inputs_schema: Mapping[str, ValueSchema] = Field(description="The inputs schemas.")
 
 
 class RenderControllerJson(Controller):
     path = "/"
 
-    @get(path="/create_render_manifest/{data_type:str}")
+    @get(
+        path="/create_render_manifest/{data_type:str}",
+        api_func=KiaraAPI.assemble_render_pipeline,
+    )
     async def create_render_manifest(
         self, kiara_api: KiaraAPI, data_type: str
     ) -> Operation:
         """Create a render manifest for the specified data type."""
 
         filters = ["select_columns"]
         operation = kiara_api.assemble_render_pipeline(
             data_type=data_type, target_format="html", filters=filters
         )
         return operation
 
-    @post(path="/value/{value:str}/{target_format:str}")
+    @post(path="/value/{value:str}/{target_format:str}", api_func=KiaraAPI.render_value)
     async def render_data(
         self,
         kiara_api: KiaraAPI,
         value: str,
         target_format: str = "html",
         data: Union[None, Dict[str, Any]] = None,
     ) -> RenderValueResult:
@@ -53,15 +57,18 @@
         filters: List[str] = []
         v = kiara_api.get_value(value)
         result = kiara_api.render_value(
             value=v, target_format=target_format, filters=filters, render_config=data
         )
         return result
 
-    @post(path="/value_info/{value:str}/{target_format:str}")
+    @post(
+        path="/value_info/{value:str}/{target_format:str}",
+        summary="Render value info as HTML",
+    )
     async def render_operation_info(
         self,
         kiara_api: KiaraAPI,
         value: str,
         target_format: str = "html",
         data: Union[Dict[str, Any], None] = None,
     ) -> str:
```

### Comparing `kiara_plugin.service-0.4.0/src/kiara_plugin/service/openapi/controllers/values.py` & `kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/values.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,181 +2,183 @@
 import uuid
 from typing import Any, Dict, List, Mapping, Union
 
 from networkx import DiGraph
 from networkx.readwrite import json_graph
 from pydantic import BaseModel, Field
 from starlite import (
-    Body,
     Controller,
-    MediaType,
-    RequestEncodingType,
-    Template,
-    get,
-    post,
 )
 
 from kiara.api import Kiara, KiaraAPI, Value, ValueSchema
 from kiara.exceptions import InvalidValuesException
 from kiara.interfaces.python_api import ValueInfo, ValuesInfo
 from kiara.models.values.matchers import ValueMatcher
 from kiara.models.values.value import SerializedData
-from kiara.registries.templates import TemplateRegistry
-from kiara_plugin.service.openapi import DataTypeModel, DataTypeRequest, RenderRequest
+from kiara_plugin.service.openapi.controllers import get, post
 
 
 class InputsValidationData(BaseModel):
 
     inputs: Mapping[str, Any] = Field(description="The provided inputs.")
     inputs_schema: Mapping[str, ValueSchema] = Field(description="The inputs schemas.")
 
 
 class ValueControllerJson(Controller):
     path = "/"
 
-    @get(path="/ids")
-    async def list_valueids(self, kiara_api: KiaraAPI) -> List[uuid.UUID]:
+    @get(path="/ids", api_func=KiaraAPI.list_value_ids)
+    async def list_value_ids(self, kiara_api: KiaraAPI) -> List[uuid.UUID]:
 
         result = kiara_api.list_value_ids()
         return result
 
-    @get(path="/value_info/{value: str}")
+    @get(path="/value_info/{value: str}", api_func=KiaraAPI.retrieve_value_info)
     async def get_value_info(self, kiara_api: KiaraAPI, value: str) -> ValueInfo:
 
         value_info = kiara_api.retrieve_value_info(value=value)
         return value_info
 
-    @post(path="/values")
-    async def find_values(
-        self, kiara_api: KiaraAPI, data: ValueMatcher
-    ) -> Dict[str, ValueInfo]:
-
-        matcher_data = data.dict()
+    # @post(path="/values", api_func=KiaraAPI.retrieve_values_info)
+    # async def find_values(
+    #     self, kiara_api: KiaraAPI, data: ValueMatcher
+    # ) -> Dict[str, ValueInfo]:
+    #
+    #     matcher_data = data.dict()
+    #
+    #     result = kiara_api.retrieve_values_info(**matcher_data).item_infos
+    #     return result  # type: ignore
 
-        result = kiara_api.retrieve_values_info(**matcher_data).item_infos
-        return result  # type: ignore
-
-    @post(path="/values_info")
+    @post(path="/values_info", api_func=KiaraAPI.retrieve_values_info)
     async def get_values_info(
         self, kiara_api: KiaraAPI, data: ValueMatcher
     ) -> Dict[str, ValueInfo]:
 
         matcher_data = data.dict()
 
         result = kiara_api.retrieve_values_info(**matcher_data)
         return result.item_infos  # type: ignore
 
-    @get(path="/type/{data_type:str}/values")
+    @get(path="/type/{data_type:str}/values", api_func=KiaraAPI.list_values)
     async def find_values_of_type(
         self, kiara_api: KiaraAPI, data_type: str
     ) -> Dict[str, Value]:
 
         matcher = ValueMatcher(data_types=[data_type])
 
         result = kiara_api.list_values(**matcher.dict())
         return result  # type: ignore
         # return {str(k): v for k, v in result.items()}
 
-    @get(path="/type/{data_type:str}/values_info")
+    @get(
+        path="/type/{data_type:str}/values_info",
+        summary="List values info of specific data type.",
+    )
     async def find_values_info_of_type(
         self, kiara_api: KiaraAPI, data_type: str
     ) -> ValuesInfo:
 
         matcher = ValueMatcher(data_types=[data_type])
 
         result = kiara_api.retrieve_values_info(**matcher.dict())
         return result
 
-    @post(path="/alias_names")
+    @post(path="/alias_names", api_func=KiaraAPI.list_alias_names)
     async def list_alias_names(
         self, kiara_api: KiaraAPI, data: ValueMatcher
     ) -> List[str]:
 
         matcher_data = data.dict()
         result = kiara_api.list_alias_names(**matcher_data)
         return result
 
-    @post(path="/aliases")
+    @post(path="/aliases", api_func=KiaraAPI.list_aliases)
     async def list_aliases(
         self, kiara_api: KiaraAPI, data: ValueMatcher
     ) -> Dict[str, Value]:
 
         matcher_data = data.dict()
 
         result = kiara_api.list_aliases(**matcher_data)
         return result  # type: ignore
 
-    @post(path="/aliases_info")
+    @post(path="/aliases_info", api_func=KiaraAPI.retrieve_aliases_info)
     async def list_aliases_info(
         self, kiara_api: KiaraAPI, data: ValueMatcher
     ) -> Dict[str, ValueInfo]:
 
         if data is None:
             matcher_data = {}
         else:
             matcher_data = data.dict()
 
         result = kiara_api.retrieve_aliases_info(**matcher_data)
         return result.item_infos  # type: ignore
 
-    @get(path="/type/{data_type:str}/aliases")
+    @get(path="/type/{data_type:str}/aliases", api_func=KiaraAPI.list_aliases)
     async def find_value_aliases_of_type(
         self, kiara_api: KiaraAPI, data_type: str
     ) -> Dict[str, Value]:
 
         matcher = ValueMatcher(data_types=[data_type], has_alias=True)
 
         result = kiara_api.list_aliases(**matcher.dict())
         return result  # type: ignore
 
-    @get(path="/type/{data_type:str}/alias_names")
+    @get(path="/type/{data_type:str}/alias_names", api_func=KiaraAPI.list_alias_names)
     async def find_value_aliase_names_of_type(
         self, kiara_api: KiaraAPI, data_type: str
     ) -> List[str]:
         matcher = ValueMatcher(data_types=[data_type], has_alias=True)
 
         result = kiara_api.list_alias_names(**matcher.dict())
         return result
 
-    @get(path="/type/{data_type:str}/aliases_info")
+    @get(
+        path="/type/{data_type:str}/aliases_info",
+        api_func=KiaraAPI.retrieve_aliases_info,
+    )
     async def find_value_aliases_info_of_type(
         self, kiara_api: KiaraAPI, data_type: str
     ) -> ValuesInfo:
 
         matcher = ValueMatcher(data_types=[data_type], has_alias=True)
 
         result = kiara_api.retrieve_aliases_info(**matcher.dict())
         return result
 
-    @get(path="/serialized/{value:uuid}")
+    @get(
+        path="/serialized/{value:uuid}",
+        summary="Retrieve the serialized form of the values data.",
+    )
     async def retrieve_data(
         self, kiara_api: KiaraAPI, value: Union[str, uuid.UUID]
     ) -> SerializedData:
 
         _value = kiara_api.get_value(value)
         return _value.serialized_data
 
     async def filter_data(self, kiara: Kiara, value):
         raise NotImplementedError()
 
-    @post(path="/validate/inputs")
+    @post(path="/validate/inputs", summary="Validate inputs against a schema.")
     async def validate_inputs(
         self, kiara_api: KiaraAPI, data: InputsValidationData
     ) -> Dict[str, str]:
 
         print("VALIDATE REQUEST")
         try:
             value_map = kiara_api.context.data_registry.create_valuemap(
                 data=data.inputs, schema=data.inputs_schema
             )
             return value_map.check_invalid()
         except InvalidValuesException as ive:
             return dict(ive.invalid_inputs)
 
-    @get(path="/lineage/{value:str}")
+    @get(path="/lineage/{value:str}", summary="Retrieve the lineage data for a value.")
     async def get_value_lineage(
         self, kiara_api: KiaraAPI, value: str
     ) -> Dict[str, Any]:
 
         print(f"LINEAGE REQUEST: {value}")
         _value = kiara_api.get_value(value=value)
         try:
@@ -186,124 +188,124 @@
         except Exception as e:
             import traceback
 
             traceback.print_exc()
             raise e
 
 
-class ValueControllerHtmx(Controller):
-    path = "/"
-
-    @get(path="/", media_type=MediaType.HTML)
-    async def get_root_page(self, kiara: Kiara) -> Template:
-
-        return Template(
-            name="kiara_plugin.service/values/index.html", context={"kiara": kiara}
-        )
-
-    # @get(path="/values/aliases", media_type=MediaType.HTML)
-    # def get_alias_select_box(self, kiara: Kiara) -> Template:
-    #     return Template(name="kiara_plugin.service/values/alias_select.html", context={"kiara": kiara})
-
-    @post(path="/select", media_type=MediaType.HTML)
-    async def get_value_select(
-        self,
-        kiara_api: KiaraAPI,
-        data: DataTypeRequest = Body(media_type=RequestEncodingType.URL_ENCODED),
-    ) -> Template:
-
-        if data and data.data_type:
-            data_types = [data.data_type]
-        else:
-            data_types = []
-
-        print(f"DATA_SELECT: {data_types}")
-
-        if data and data.data_type:
-            data_types = [data.data_type]
-        else:
-            data_types = []
-
-        return Template(
-            name="kiara_plugin.service/values/value_select.html",
-            context={"data_types": data_types, "field_name": "__no_field_name__"},
-        )
-
-    @post(path="/render", media_type=MediaType.HTML)
-    async def render_value(
-        self,
-        kiara_api: KiaraAPI,
-        data: RenderRequest = Body(media_type=RequestEncodingType.URL_ENCODED),
-    ) -> Template:
-
-        print(f"RENDER REQUEST: {data}")
-        try:
-
-            if not hasattr(data, data.field_name):
-                raise Exception(
-                    f"Request is missing the value attribute '{data.field_name}'."
-                )
-
-            value_id = getattr(data, data.field_name)
-
-            value = kiara_api.get_value(value=value_id)
-
-            print("-------")
-            print(value)
-            render_conf = data.render_conf
-            if render_conf is None:
-                render_conf = {}
-
-            print(render_conf)
-
-            render_result = kiara_api.render_value(
-                value=value,
-                target_format=["html", "string"],
-                render_config=render_conf,
-            )
-        except Exception as e:
-            import traceback
-
-            traceback.print_exc()
-            raise e
-
-        return Template(
-            name="kiara_plugin.service/values/value_view.html",
-            context={
-                "element_id": data.target_id,
-                "render_value_result": render_result,
-                "value_id": str(value.value_id),
-                "field_name": data.field_name,
-            },
-        )
-
-    @post(path="/input_widget", media_type=MediaType.HTML)
-    async def get_input_element_for_type(
-        self,
-        kiara_api: KiaraAPI,
-        template_registry: TemplateRegistry,
-        data: DataTypeModel = Body(media_type=RequestEncodingType.URL_ENCODED),
-    ) -> str:
-
-        print(f"INPUT FIELD REQUEST: {data.data_type}")
-
-        data_type_cls = kiara_api.context.type_registry.get_data_type_cls(
-            type_name=data.data_type
-        )
-        data_type_instance = data_type_cls(**data.type_config)
-
-        alias_map = kiara_api.list_aliases(data_types=[data.data_type])
-
-        try:
-            template = template_registry.get_template(
-                f"kiara_plugin.service/values/inputs/{data.data_type}.html"
-            )
-            rendered = template.render(
-                data_type_instance=data_type_instance,
-                alias_map=alias_map,
-                data_type_name=data.data_type,
-                field_name=data.field_name,
-            )
-        except Exception as e:
-            rendered = str(e)
-
-        return rendered
+# class ValueControllerHtmx(Controller):
+#     path = "/"
+#
+#     @get(path="/", media_type=MediaType.HTML)
+#     async def get_root_page(self, kiara: Kiara) -> Template:
+#
+#         return Template(
+#             name="kiara_plugin.service/values/index.html", context={"kiara": kiara}
+#         )
+#
+#     # @get(path="/values/aliases", media_type=MediaType.HTML)
+#     # def get_alias_select_box(self, kiara: Kiara) -> Template:
+#     #     return Template(name="kiara_plugin.service/values/alias_select.html", context={"kiara": kiara})
+#
+#     @post(path="/select", media_type=MediaType.HTML)
+#     async def get_value_select(
+#         self,
+#         kiara_api: KiaraAPI,
+#         data: DataTypeRequest = Body(media_type=RequestEncodingType.URL_ENCODED),
+#     ) -> Template:
+#
+#         if data and data.data_type:
+#             data_types = [data.data_type]
+#         else:
+#             data_types = []
+#
+#         print(f"DATA_SELECT: {data_types}")
+#
+#         if data and data.data_type:
+#             data_types = [data.data_type]
+#         else:
+#             data_types = []
+#
+#         return Template(
+#             name="kiara_plugin.service/values/value_select.html",
+#             context={"data_types": data_types, "field_name": "__no_field_name__"},
+#         )
+#
+#     @post(path="/render", media_type=MediaType.HTML)
+#     async def render_value(
+#         self,
+#         kiara_api: KiaraAPI,
+#         data: RenderRequest = Body(media_type=RequestEncodingType.URL_ENCODED),
+#     ) -> Template:
+#
+#         print(f"RENDER REQUEST: {data}")
+#         try:
+#
+#             if not hasattr(data, data.field_name):
+#                 raise Exception(
+#                     f"Request is missing the value attribute '{data.field_name}'."
+#                 )
+#
+#             value_id = getattr(data, data.field_name)
+#
+#             value = kiara_api.get_value(value=value_id)
+#
+#             print("-------")
+#             print(value)
+#             render_conf = data.render_conf
+#             if render_conf is None:
+#                 render_conf = {}
+#
+#             print(render_conf)
+#
+#             render_result = kiara_api.render_value(
+#                 value=value,
+#                 target_format=["html", "string"],
+#                 render_config=render_conf,
+#             )
+#         except Exception as e:
+#             import traceback
+#
+#             traceback.print_exc()
+#             raise e
+#
+#         return Template(
+#             name="kiara_plugin.service/values/value_view.html",
+#             context={
+#                 "element_id": data.target_id,
+#                 "render_value_result": render_result,
+#                 "value_id": str(value.value_id),
+#                 "field_name": data.field_name,
+#             },
+#         )
+#
+#     @post(path="/input_widget", media_type=MediaType.HTML)
+#     async def get_input_element_for_type(
+#         self,
+#         kiara_api: KiaraAPI,
+#         template_registry: TemplateRegistry,
+#         data: DataTypeModel = Body(media_type=RequestEncodingType.URL_ENCODED),
+#     ) -> str:
+#
+#         print(f"INPUT FIELD REQUEST: {data.data_type}")
+#
+#         data_type_cls = kiara_api.context.type_registry.get_data_type_cls(
+#             type_name=data.data_type
+#         )
+#         data_type_instance = data_type_cls(**data.type_config)
+#
+#         alias_map = kiara_api.list_aliases(data_types=[data.data_type])
+#
+#         try:
+#             template = template_registry.get_template(
+#                 f"kiara_plugin.service/values/inputs/{data.data_type}.html"
+#             )
+#             rendered = template.render(
+#                 data_type_instance=data_type_instance,
+#                 alias_map=alias_map,
+#                 data_type_name=data.data_type,
+#                 field_name=data.field_name,
+#             )
+#         except Exception as e:
+#             rendered = str(e)
+#
+#         return rendered
```

### Comparing `kiara_plugin.service-0.4.0/src/kiara_plugin/service/openapi/controllers/workflows.py` & `kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/controllers/workflows.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 # -*- coding: utf-8 -*-
 from typing import Dict, List, Union
 
 from pydantic import BaseModel, Field
-from starlite import Controller, get, post
+from starlite import Controller
 
 from kiara.api import KiaraAPI
 from kiara.models.workflow import WorkflowInfo
+from kiara_plugin.service.openapi.controllers import get, post
 
 
 class WorkflowMatcher(BaseModel):
 
     filters: List[str] = Field(
         description="The (optional) filter strings, an operation must match all of them to be included in the result.",
         default_factory=list,
     )
 
 
 class WorkflowControllerJson(Controller):
     path = "/"
 
-    @post(path="/ids")
+    @post(path="/ids", api_func=KiaraAPI.retrieve_workflows_info)
     async def list_workflows(
         self, kiara_api: KiaraAPI, data: Union[WorkflowMatcher, None] = None
     ) -> Dict[str, WorkflowInfo]:
 
         # if data is None:
         #     filters: List[str] = []
         # else:
         #     filters = data.filters
 
         result = kiara_api.retrieve_workflows_info().item_infos
         return result  # type: ignore
 
-    @post(path="/aliases")
+    @post(path="/aliases", api_func=KiaraAPI.list_workflow_alias_names)
     async def list_workflow_aliases(
         self, kiara_api: KiaraAPI, data: Union[WorkflowMatcher, None] = None
     ) -> List[str]:
 
         # if data is None:
         #     filters: List[str] = []
         # else:
         #     filters = data.filters
 
         result = kiara_api.list_workflow_alias_names()
         return result
 
-    @get(path="/workflow_info/{workflow: str}")
+    @get(
+        path="/workflow_info/{workflow: str}", api_func=KiaraAPI.retrieve_workflow_info
+    )
     async def get_workflow_info(
         self, kiara_api: KiaraAPI, workflow: str
     ) -> WorkflowInfo:
 
         print(f"INFO: {workflow}")
         workflow_info = kiara_api.retrieve_workflow_info(workflow=workflow)
         return workflow_info
```

### Comparing `kiara_plugin.service-0.4.0/src/kiara_plugin/service/openapi/service.py` & `kiara_plugin.service-0.4.1/src/kiara_plugin/service/openapi/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,22 +38,21 @@
 from kiara.context import Kiara
 from kiara.interfaces.python_api import KiaraAPI
 from kiara.models import KiaraModel
 from kiara.registries.templates import TemplateRegistry
 from kiara.utils import is_debug, is_develop
 from kiara_plugin.service.defaults import KIARA_SERVICE_RESOURCES_FOLDER
 from kiara_plugin.service.openapi.controllers.jobs import JobControllerJson
+from kiara_plugin.service.openapi.controllers.modules import ModuleControllerJson
 from kiara_plugin.service.openapi.controllers.operations import (
-    OperationControllerHtmx,
     OperationControllerJson,
 )
 from kiara_plugin.service.openapi.controllers.pipeline import PipelineControllerJson
 from kiara_plugin.service.openapi.controllers.render import RenderControllerJson
 from kiara_plugin.service.openapi.controllers.values import (
-    ValueControllerHtmx,
     ValueControllerJson,
 )
 from kiara_plugin.service.openapi.controllers.workflows import WorkflowControllerJson
 
 T = TypeVar("T")
 
 
@@ -165,14 +164,15 @@
     def app(self) -> Starlite:
         if self._app is not None:
             return self._app
 
         from starlite import Router
 
         value_router = Router(path="/data", route_handlers=[ValueControllerJson])
+        module_router = Router(path="/modules", route_handlers=[ModuleControllerJson])
         operation_router = Router(
             path="/operations", route_handlers=[OperationControllerJson]
         )
         job_router = Router(path="/jobs", route_handlers=[JobControllerJson])
         render_router = Router(path="/render", route_handlers=[RenderControllerJson])
         workflow_router = Router(
             path="/workflows", route_handlers=[WorkflowControllerJson]
@@ -180,19 +180,20 @@
         pipeline_router = Router(
             path="/pipelines", route_handlers=[PipelineControllerJson]
         )
 
         # info_router_html = Router(
         #     path="/html/info", route_handlers=[OperationControllerHtml]
         # )
-        Router(path="/html/values", route_handlers=[ValueControllerHtmx])
-        Router(path="/html/operations", route_handlers=[OperationControllerHtmx])
+        # Router(path="/html/values", route_handlers=[ValueControllerHtmx])
+        # Router(path="/html/operations", route_handlers=[OperationControllerHtmx])
 
         route_handlers: List[ControllerRouterHandler] = []
         route_handlers.append(value_router)
+        route_handlers.append(module_router)
         route_handlers.append(operation_router)
         route_handlers.append(job_router)
         route_handlers.append(render_router)
         route_handlers.append(workflow_router)
         route_handlers.append(pipeline_router)
 
         # route_handlers.append(value_router_htmx)
```

### Comparing `kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/static/favicon.ico` & `kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/static/main.css` & `kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/static/main.css`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/static/simple.css` & `kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/static/simple.css`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/jobs/job_finished.html` & `kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/jobs/job_finished.html`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/macros.html` & `kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/macros.html`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/src/kiara_plugin/service/resources/templates/values/inputs/base_scalar.html` & `kiara_plugin.service-0.4.1/src/kiara_plugin/service/resources/templates/values/inputs/base_scalar.html`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/src/kiara_plugin.service.egg-info/PKG-INFO` & `kiara_plugin.service-0.4.1/src/kiara_plugin.service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara-plugin.service
-Version: 0.4.0
+Version: 0.4.1
 Summary: A plugin to create, run and manage a service for kiara functionality.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.service
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.service
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.service
 Keywords: kiara
```

### Comparing `kiara_plugin.service-0.4.0/src/kiara_plugin.service.egg-info/SOURCES.txt` & `kiara_plugin.service-0.4.1/src/kiara_plugin.service.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 src/kiara_plugin/service/interfaces/cli/service/__init__.py
 src/kiara_plugin/service/interfaces/cli/service/commands.py
 src/kiara_plugin/service/modules/__init__.py
 src/kiara_plugin/service/openapi/__init__.py
 src/kiara_plugin/service/openapi/service.py
 src/kiara_plugin/service/openapi/controllers/__init__.py
 src/kiara_plugin/service/openapi/controllers/jobs.py
+src/kiara_plugin/service/openapi/controllers/modules.py
 src/kiara_plugin/service/openapi/controllers/operations.py
 src/kiara_plugin/service/openapi/controllers/pipeline.py
 src/kiara_plugin/service/openapi/controllers/render.py
 src/kiara_plugin/service/openapi/controllers/values.py
 src/kiara_plugin/service/openapi/controllers/workflows.py
 src/kiara_plugin/service/pipelines/.gitkeep
 src/kiara_plugin/service/pipelines/__init__.py
```

### Comparing `kiara_plugin.service-0.4.0/tests/conftest.py` & `kiara_plugin.service-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.0/tests/test_job_descs.py` & `kiara_plugin.service-0.4.1/tests/test_job_descs.py`

 * *Files identical despite different names*

