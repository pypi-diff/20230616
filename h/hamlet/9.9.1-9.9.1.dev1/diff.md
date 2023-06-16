# Comparing `tmp/hamlet-9.9.1.tar.gz` & `tmp/hamlet-9.9.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hamlet-9.9.1.tar", last modified: Thu Dec 23 23:09:21 2021, max compression
+gzip compressed data, was "hamlet-9.9.1.dev1.tar", last modified: Wed Dec  8 00:35:22 2021, max compression
```

## Comparing `hamlet-9.9.1.tar` & `hamlet-9.9.1.dev1.tar`

### file list

```diff
@@ -1,444 +1,444 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.390816 hamlet-9.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)      225 2021-12-23 23:08:12.000000 hamlet-9.9.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      148 2021-12-23 23:08:12.000000 hamlet-9.9.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.334817 hamlet-9.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.350817 hamlet-9.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1159 2021-12-23 23:08:12.000000 hamlet-9.9.1/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1400 2021-12-23 23:08:12.000000 hamlet-9.9.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      544 2021-12-23 23:08:12.000000 hamlet-9.9.1/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (121)      222 2021-12-23 23:08:12.000000 hamlet-9.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    18719 2021-12-23 23:08:12.000000 hamlet-9.9.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2021-12-23 23:08:12.000000 hamlet-9.9.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-12-23 23:08:12.000000 hamlet-9.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      207 2021-12-23 23:08:12.000000 hamlet-9.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      531 2021-12-23 23:08:12.000000 hamlet-9.9.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     2337 2021-12-23 23:09:21.390816 hamlet-9.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1714 2021-12-23 23:08:12.000000 hamlet-9.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.350817 hamlet-9.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-12-23 23:08:12.000000 hamlet-9.9.1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      603 2021-12-23 23:08:12.000000 hamlet-9.9.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      780 2021-12-23 23:08:12.000000 hamlet-9.9.1/docs/backend_reference.rst
--rw-r--r--   0 runner    (1001) docker     (121)      174 2021-12-23 23:08:12.000000 hamlet-9.9.1/docs/command_reference.rst
--rw-r--r--   0 runner    (1001) docker     (121)      446 2021-12-23 23:08:12.000000 hamlet-9.9.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1159 2021-12-23 23:08:12.000000 hamlet-9.9.1/docs/config_files.rst
--rw-r--r--   0 runner    (1001) docker     (121)      525 2021-12-23 23:08:12.000000 hamlet-9.9.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.350817 hamlet-9.9.1/hamlet/
--rw-r--r--   0 runner    (1001) docker     (121)      463 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)      753 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      106 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-12-23 23:09:21.000000 hamlet-9.9.1/hamlet/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.350817 hamlet-9.9.1/hamlet/backend/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.350817 hamlet-9.9.1/hamlet/backend/automation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/automation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.350817 hamlet-9.9.1/hamlet/backend/automation/confirm_builds/
--rw-r--r--   0 runner    (1001) docker     (121)      730 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/automation/confirm_builds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.350817 hamlet-9.9.1/hamlet/backend/automation/construct_tree/
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/automation/construct_tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.354817 hamlet-9.9.1/hamlet/backend/automation/manage_build_references/
--rw-r--r--   0 runner    (1001) docker     (121)      982 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/automation/manage_build_references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.354817 hamlet-9.9.1/hamlet/backend/automation/manage_images/
--rw-r--r--   0 runner    (1001) docker     (121)      707 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/automation/manage_images/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.354817 hamlet-9.9.1/hamlet/backend/automation/properties_file/
--rw-r--r--   0 runner    (1001) docker     (121)      532 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/automation/properties_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.354817 hamlet-9.9.1/hamlet/backend/automation/save_cmdb_repos/
--rw-r--r--   0 runner    (1001) docker     (121)      623 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/automation/save_cmdb_repos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.354817 hamlet-9.9.1/hamlet/backend/automation/set_automation_context/
--rw-r--r--   0 runner    (1001) docker     (121)      768 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/automation/set_automation_context/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.354817 hamlet-9.9.1/hamlet/backend/automation/update_build_references/
--rw-r--r--   0 runner    (1001) docker     (121)      648 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/automation/update_build_references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.354817 hamlet-9.9.1/hamlet/backend/automation_tasks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/automation_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1411 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/automation_tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.354817 hamlet-9.9.1/hamlet/backend/automation_tasks/save_repos/
--rw-r--r--   0 runner    (1001) docker     (121)     1330 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/automation_tasks/save_repos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.354817 hamlet-9.9.1/hamlet/backend/automation_tasks/transfer_image/
--rw-r--r--   0 runner    (1001) docker     (121)     1960 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/automation_tasks/transfer_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.354817 hamlet-9.9.1/hamlet/backend/automation_tasks/update_build/
--rw-r--r--   0 runner    (1001) docker     (121)     1431 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/automation_tasks/update_build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.354817 hamlet-9.9.1/hamlet/backend/automation_tasks/upload_image/
--rw-r--r--   0 runner    (1001) docker     (121)     1918 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/automation_tasks/upload_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.354817 hamlet-9.9.1/hamlet/backend/common/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9008 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/common/context.py
--rw-r--r--   0 runner    (1001) docker     (121)      164 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7029 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/common/fsutils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3282 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/common/runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/common/shell_vars_to_json.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1304 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/common/shell_vars_to_json.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.354817 hamlet-9.9.1/hamlet/backend/container_registry/
--rw-r--r--   0 runner    (1001) docker     (121)     7451 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/container_registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.354817 hamlet-9.9.1/hamlet/backend/create/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.358816 hamlet-9.9.1/hamlet/backend/create/template/
--rw-r--r--   0 runner    (1001) docker     (121)     1406 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/create/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    49724 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/create/template/context_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/create/template/create_template.py
--rw-r--r--   0 runner    (1001) docker     (121)      858 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/create/template/environment.py
--rw-r--r--   0 runner    (1001) docker     (121)    11245 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/create/template/set_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     4477 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/create/template/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.358816 hamlet-9.9.1/hamlet/backend/deploy/
--rw-r--r--   0 runner    (1001) docker     (121)     3398 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/deploy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.358816 hamlet-9.9.1/hamlet/backend/draw/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/draw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/draw/diagram.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/draw/diagram_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     8372 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/draw/render.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.358816 hamlet-9.9.1/hamlet/backend/engine/
--rw-r--r--   0 runner    (1001) docker     (121)     6367 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/engine/common.py
--rw-r--r--   0 runner    (1001) docker     (121)    11737 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (121)     1923 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/engine/engine_code_source.py
--rw-r--r--   0 runner    (1001) docker     (121)      438 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/engine/engine_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/engine/engine_part.py
--rw-r--r--   0 runner    (1001) docker     (121)     4551 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/engine/engine_source.py
--rw-r--r--   0 runner    (1001) docker     (121)      822 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/engine/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.358816 hamlet-9.9.1/hamlet/backend/engine/loaders/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/engine/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3121 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/engine/loaders/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3873 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/engine/loaders/train.py
--rw-r--r--   0 runner    (1001) docker     (121)     3872 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/engine/loaders/tram.py
--rw-r--r--   0 runner    (1001) docker     (121)     2689 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/engine/loaders/unicycle.py
--rw-r--r--   0 runner    (1001) docker     (121)     7540 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/engine/loaders/user.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.358816 hamlet-9.9.1/hamlet/backend/generate/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.358816 hamlet-9.9.1/hamlet/backend/generate/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      176 2021-12-23 23:09:03.000000 hamlet-9.9.1/hamlet/backend/generate/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1645 2021-12-23 23:09:03.000000 hamlet-9.9.1/hamlet/backend/generate/__pycache__/utils.cpython-38.pyc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.358816 hamlet-9.9.1/hamlet/backend/generate/cmdb/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.362816 hamlet-9.9.1/hamlet/backend/generate/cmdb/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      181 2021-12-23 23:09:03.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.362816 hamlet-9.9.1/hamlet/backend/generate/cmdb/account/
--rw-r--r--   0 runner    (1001) docker     (121)      337 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.362816 hamlet-9.9.1/hamlet/backend/generate/cmdb/account/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      703 2021-12-23 23:09:03.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/account/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.362816 hamlet-9.9.1/hamlet/backend/generate/cmdb/account/template/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/account/template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.362816 hamlet-9.9.1/hamlet/backend/generate/cmdb/account/template/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      198 2021-12-23 23:09:03.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/account/template/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      384 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/account/template/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.338817 hamlet-9.9.1/hamlet/backend/generate/cmdb/account/template/{{cookiecutter.account_name}}/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.362816 hamlet-9.9.1/hamlet/backend/generate/cmdb/account/template/{{cookiecutter.account_name}}/config/
--rw-r--r--   0 runner    (1001) docker     (121)      283 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/account/template/{{cookiecutter.account_name}}/config/account.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.334817 hamlet-9.9.1/hamlet/backend/generate/cmdb/account/template/{{cookiecutter.account_name}}/config/settings/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.362816 hamlet-9.9.1/hamlet/backend/generate/cmdb/account/template/{{cookiecutter.account_name}}/config/settings/shared/
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/account/template/{{cookiecutter.account_name}}/config/settings/shared/settings.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.338817 hamlet-9.9.1/hamlet/backend/generate/cmdb/account/template/{{cookiecutter.account_name}}/infrastructure/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.338817 hamlet-9.9.1/hamlet/backend/generate/cmdb/account/template/{{cookiecutter.account_name}}/infrastructure/operations/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.362816 hamlet-9.9.1/hamlet/backend/generate/cmdb/account/template/{{cookiecutter.account_name}}/infrastructure/operations/shared/
--rw-r--r--   0 runner    (1001) docker     (121)        3 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/account/template/{{cookiecutter.account_name}}/infrastructure/operations/shared/credentials.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.362816 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/
--rw-r--r--   0 runner    (1001) docker     (121)      168 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.362816 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      441 2021-12-23 23:09:03.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.362816 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.362816 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      198 2021-12-23 23:09:03.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      271 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.338817 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.362816 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/
--rw-r--r--   0 runner    (1001) docker     (121)      536 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/product.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.338817 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/settings/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.362816 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/settings/shared/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/settings/shared/settings.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.362816 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/settings/{{cookiecutter.environment_name}}/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/settings/{{cookiecutter.environment_name}}/settings.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.362816 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/settings/{{cookiecutter.environment_name}}/{{cookiecutter.segment_name}}/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/settings/{{cookiecutter.environment_name}}/{{cookiecutter.segment_name}}/settings.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.338817 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/solutionsv2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.338817 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/solutionsv2/shared/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.362816 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/solutionsv2/shared/{{cookiecutter.segment_name}}/
--rw-r--r--   0 runner    (1001) docker     (121)      111 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/solutionsv2/shared/{{cookiecutter.segment_name}}/segment.json
--rw-r--r--   0 runner    (1001) docker     (121)       78 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/solutionsv2/shared/{{cookiecutter.segment_name}}/solution.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.362816 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/solutionsv2/{{cookiecutter.environment_name}}/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/solutionsv2/{{cookiecutter.environment_name}}/environment.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.362816 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/solutionsv2/{{cookiecutter.environment_name}}/{{cookiecutter.segment_name}}/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/solutionsv2/{{cookiecutter.environment_name}}/{{cookiecutter.segment_name}}/segment.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.338817 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/infrastructure/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.338817 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/infrastructure/operations/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.362816 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/infrastructure/operations/{{cookiecutter.environment_name}}/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/infrastructure/operations/{{cookiecutter.environment_name}}/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.362816 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/infrastructure/operations/{{cookiecutter.environment_name}}/{{cookiecutter.segment_name}}/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/infrastructure/operations/{{cookiecutter.environment_name}}/{{cookiecutter.segment_name}}/credentials.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.362816 hamlet-9.9.1/hamlet/backend/generate/cmdb/tenant/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/tenant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.362816 hamlet-9.9.1/hamlet/backend/generate/cmdb/tenant/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      439 2021-12-23 23:09:03.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/tenant/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.366816 hamlet-9.9.1/hamlet/backend/generate/cmdb/tenant/template/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/tenant/template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.366816 hamlet-9.9.1/hamlet/backend/generate/cmdb/tenant/template/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      197 2021-12-23 23:09:03.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/tenant/template/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      217 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/tenant/template/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.338817 hamlet-9.9.1/hamlet/backend/generate/cmdb/tenant/template/{{cookiecutter._base_dir}}/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.366816 hamlet-9.9.1/hamlet/backend/generate/cmdb/tenant/template/{{cookiecutter._base_dir}}/{{cookiecutter.tenant_name}}/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/tenant/template/{{cookiecutter._base_dir}}/{{cookiecutter.tenant_name}}/ipaddressgroups.json
--rw-r--r--   0 runner    (1001) docker     (121)      440 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/cmdb/tenant/template/{{cookiecutter._base_dir}}/{{cookiecutter.tenant_name}}/tenant.json
--rw-r--r--   0 runner    (1001) docker     (121)     1847 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/generate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.366816 hamlet-9.9.1/hamlet/backend/manage/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/manage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.366816 hamlet-9.9.1/hamlet/backend/manage/credential_crypto/
--rw-r--r--   0 runner    (1001) docker     (121)      927 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/manage/credential_crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.366816 hamlet-9.9.1/hamlet/backend/manage/crypto/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/manage/crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.366816 hamlet-9.9.1/hamlet/backend/manage/deployment/
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/manage/deployment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.366816 hamlet-9.9.1/hamlet/backend/manage/file_crypto/
--rw-r--r--   0 runner    (1001) docker     (121)      675 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/manage/file_crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.366816 hamlet-9.9.1/hamlet/backend/manage/stack/
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/manage/stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.366816 hamlet-9.9.1/hamlet/backend/query/
--rw-r--r--   0 runner    (1001) docker     (121)     4714 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/query/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.366816 hamlet-9.9.1/hamlet/backend/run/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.366816 hamlet-9.9.1/hamlet/backend/run/expo_app_publish/
--rw-r--r--   0 runner    (1001) docker     (121)     1144 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/run/expo_app_publish/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.366816 hamlet-9.9.1/hamlet/backend/run/lambda_func/
--rw-r--r--   0 runner    (1001) docker     (121)      754 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/run/lambda_func/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.366816 hamlet-9.9.1/hamlet/backend/run/pipeline/
--rw-r--r--   0 runner    (1001) docker     (121)      846 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/run/pipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.366816 hamlet-9.9.1/hamlet/backend/run/sentry_release/
--rw-r--r--   0 runner    (1001) docker     (121)      789 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/run/sentry_release/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.366816 hamlet-9.9.1/hamlet/backend/run/task/
--rw-r--r--   0 runner    (1001) docker     (121)     1025 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/run/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.366816 hamlet-9.9.1/hamlet/backend/setup/
--rw-r--r--   0 runner    (1001) docker     (121)      527 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/setup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.366816 hamlet-9.9.1/hamlet/backend/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1818 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/test/generate.py
--rw-r--r--   0 runner    (1001) docker     (121)      253 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/test/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.366816 hamlet-9.9.1/hamlet/backend/test/renderer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/test/renderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1883 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/test/renderer/testcases_template.py
--rw-r--r--   0 runner    (1001) docker     (121)     1537 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/test/run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.370817 hamlet-9.9.1/hamlet/backend/test/templates/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/test/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      700 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/test/templates/cfn_lint_test_func_block.py
--rw-r--r--   0 runner    (1001) docker     (121)     1734 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/test/templates/cfn_structure_obj_block.py
--rw-r--r--   0 runner    (1001) docker     (121)     1674 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/test/templates/cfn_testcase_block.py.tmpl
--rw-r--r--   0 runner    (1001) docker     (121)     1498 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/test/templates/checkov_test_func_block.py
--rw-r--r--   0 runner    (1001) docker     (121)     2276 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/test/templates/json_structure_obj_block.py
--rw-r--r--   0 runner    (1001) docker     (121)     2385 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/test/templates/json_validator_obj_block.py
--rw-r--r--   0 runner    (1001) docker     (121)      758 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/test/templates/test_template_base.py.tmpl
--rw-r--r--   0 runner    (1001) docker     (121)     1392 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/test/testcase_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.370817 hamlet-9.9.1/hamlet/backend/unitlist/
--rw-r--r--   0 runner    (1001) docker     (121)      871 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/backend/unitlist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.370817 hamlet-9.9.1/hamlet/command/
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.370817 hamlet-9.9.1/hamlet/command/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (121)     2413 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/autocomplete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.370817 hamlet-9.9.1/hamlet/command/autocomplete/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      669 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/autocomplete/scripts/.hamlet-complete.bash
--rw-r--r--   0 runner    (1001) docker     (121)      669 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/autocomplete/scripts/.hamlet-complete.fish
--rw-r--r--   0 runner    (1001) docker     (121)      966 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/autocomplete/scripts/.hamlet-complete.zsh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.370817 hamlet-9.9.1/hamlet/command/cmdb/
--rw-r--r--   0 runner    (1001) docker     (121)     2291 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/cmdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.370817 hamlet-9.9.1/hamlet/command/common/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7465 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/common/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     5202 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/common/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1341 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/common/display.py
--rw-r--r--   0 runner    (1001) docker     (121)     1707 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/common/engine_setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1932 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/common/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.374817 hamlet-9.9.1/hamlet/command/component/
--rw-r--r--   0 runner    (1001) docker     (121)     1137 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      695 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/component/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     2815 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/component/component_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     3458 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/component/describe_occurrence.py
--rw-r--r--   0 runner    (1001) docker     (121)     1364 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/component/list_occurrences.py
--rw-r--r--   0 runner    (1001) docker     (121)      637 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/component/query_occurrences.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.374817 hamlet-9.9.1/hamlet/command/deploy/
--rw-r--r--   0 runner    (1001) docker     (121)      601 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2503 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/deploy/create.py
--rw-r--r--   0 runner    (1001) docker     (121)     2346 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/deploy/list.py
--rw-r--r--   0 runner    (1001) docker     (121)     4182 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/deploy/run.py
--rw-r--r--   0 runner    (1001) docker     (121)     3802 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/deploy/test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.374817 hamlet-9.9.1/hamlet/command/engine/
--rw-r--r--   0 runner    (1001) docker     (121)     9848 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.374817 hamlet-9.9.1/hamlet/command/entrance/
--rw-r--r--   0 runner    (1001) docker     (121)     3266 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/entrance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.374817 hamlet-9.9.1/hamlet/command/generate/
--rw-r--r--   0 runner    (1001) docker     (121)      521 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4262 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/generate/cmdb.py
--rw-r--r--   0 runner    (1001) docker     (121)      491 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/generate/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)      492 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/generate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.374817 hamlet-9.9.1/hamlet/command/layer/
--rw-r--r--   0 runner    (1001) docker     (121)     5109 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/layer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.374817 hamlet-9.9.1/hamlet/command/manage/
--rw-r--r--   0 runner    (1001) docker     (121)      592 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/manage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2134 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/manage/credentials_crypto.py
--rw-r--r--   0 runner    (1001) docker     (121)     3181 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/manage/crypto.py
--rw-r--r--   0 runner    (1001) docker     (121)     1941 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/manage/deployment.py
--rw-r--r--   0 runner    (1001) docker     (121)     1007 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/manage/file_crypto.py
--rw-r--r--   0 runner    (1001) docker     (121)     2224 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/manage/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.374817 hamlet-9.9.1/hamlet/command/reference/
--rw-r--r--   0 runner    (1001) docker     (121)     5126 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/reference/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.374817 hamlet-9.9.1/hamlet/command/release/
--rw-r--r--   0 runner    (1001) docker     (121)     3777 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/release/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.378816 hamlet-9.9.1/hamlet/command/run/
--rw-r--r--   0 runner    (1001) docker     (121)      598 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2182 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/run/expo_app_publish.py
--rw-r--r--   0 runner    (1001) docker     (121)     1017 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/run/lambda_func.py
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/run/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)      979 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/run/sentry_release.py
--rw-r--r--   0 runner    (1001) docker     (121)     1936 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/run/task.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.378816 hamlet-9.9.1/hamlet/command/schema/
--rw-r--r--   0 runner    (1001) docker     (121)     3344 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.378816 hamlet-9.9.1/hamlet/command/setup/
--rw-r--r--   0 runner    (1001) docker     (121)      507 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/setup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.378816 hamlet-9.9.1/hamlet/command/test/
--rw-r--r--   0 runner    (1001) docker     (121)      342 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3054 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/test/generate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/test/run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.378816 hamlet-9.9.1/hamlet/command/visual/
--rw-r--r--   0 runner    (1001) docker     (121)     5044 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/command/visual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/env.py
--rw-r--r--   0 runner    (1001) docker     (121)      541 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.378816 hamlet-9.9.1/hamlet/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     2180 2021-12-23 23:08:12.000000 hamlet-9.9.1/hamlet/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.350817 hamlet-9.9.1/hamlet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2337 2021-12-23 23:09:21.000000 hamlet-9.9.1/hamlet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13705 2021-12-23 23:09:21.000000 hamlet-9.9.1/hamlet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-23 23:09:21.000000 hamlet-9.9.1/hamlet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-12-23 23:09:21.000000 hamlet-9.9.1/hamlet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      403 2021-12-23 23:09:21.000000 hamlet-9.9.1/hamlet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-12-23 23:09:21.000000 hamlet-9.9.1/hamlet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      197 2021-12-23 23:08:12.000000 hamlet-9.9.1/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.378816 hamlet-9.9.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      146 2021-12-23 23:08:12.000000 hamlet-9.9.1/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      128 2021-12-23 23:08:12.000000 hamlet-9.9.1/setup-hamlet.sh
--rw-r--r--   0 runner    (1001) docker     (121)      102 2021-12-23 23:09:21.394816 hamlet-9.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2807 2021-12-23 23:08:12.000000 hamlet-9.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.378816 hamlet-9.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2476 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.342817 hamlet-9.9.1/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.342817 hamlet-9.9.1/tests/data/integration/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.342817 hamlet-9.9.1/tests/data/integration/backend/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.342817 hamlet-9.9.1/tests/data/integration/backend/test/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.378816 hamlet-9.9.1/tests/data/integration/backend/test/cf/
--rw-r--r--   0 runner    (1001) docker     (121)      515 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/data/integration/backend/test/cf/insecure.json
--rw-r--r--   0 runner    (1001) docker     (121)     3296 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/data/integration/backend/test/cf/invalid-syntax.json
--rw-r--r--   0 runner    (1001) docker     (121)      901 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/data/integration/backend/test/cf/secure.json
--rw-r--r--   0 runner    (1001) docker     (121)      354 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/data/integration/backend/test/cf/structure.json
--rw-r--r--   0 runner    (1001) docker     (121)     3439 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/data/integration/backend/test/cf/valid-syntax.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.378816 hamlet-9.9.1/tests/data/integration/backend/test/testcase/
--rw-r--r--   0 runner    (1001) docker     (121)      168 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/data/integration/backend/test/testcase/insecure-testcase.json
--rw-r--r--   0 runner    (1001) docker     (121)      134 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/data/integration/backend/test/testcase/invalid-syntax-testcase.json
--rw-r--r--   0 runner    (1001) docker     (121)     2009 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/data/integration/backend/test/testcase/json-structure-bad-testcase.json
--rw-r--r--   0 runner    (1001) docker     (121)     2217 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/data/integration/backend/test/testcase/json-structure-good-testcase.json
--rw-r--r--   0 runner    (1001) docker     (121)      220 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/data/integration/backend/test/testcase/secure-testcase.json
--rw-r--r--   0 runner    (1001) docker     (121)     1729 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/data/integration/backend/test/testcase/structure-bad-testcase.json
--rw-r--r--   0 runner    (1001) docker     (121)     1492 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/data/integration/backend/test/testcase/structure-good-testcase.json
--rw-r--r--   0 runner    (1001) docker     (121)      134 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/data/integration/backend/test/testcase/valid-syntax-testcase.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.382816 hamlet-9.9.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.382816 hamlet-9.9.1/tests/integration/backend/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/integration/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.382816 hamlet-9.9.1/tests/integration/backend/create/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/integration/backend/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.382816 hamlet-9.9.1/tests/integration/backend/create/template/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/integration/backend/create/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/integration/backend/create/template/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    29098 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/integration/backend/create/template/test_context_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     1792 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/integration/backend/create/template/test_set_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1464 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/integration/backend/create/template/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.382816 hamlet-9.9.1/tests/integration/backend/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/integration/backend/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       75 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/integration/backend/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3534 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/integration/backend/test/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (121)     2131 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/integration/backend/test/test_run.py
--rw-r--r--   0 runner    (1001) docker     (121)     5114 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/integration/backend/test/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.382816 hamlet-9.9.1/tests/system/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.382816 hamlet-9.9.1/tests/system/cmdb/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/system/cmdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.382816 hamlet-9.9.1/tests/system/cmdb/product/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/system/cmdb/product/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      879 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/system/cmdb/product/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      510 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/system/cmdb/product/step_1_install_engine.py
--rw-r--r--   0 runner    (1001) docker     (121)      420 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/system/cmdb/product/step_2_create_cmdb.py
--rw-r--r--   0 runner    (1001) docker     (121)     2632 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/system/cmdb/product/step_3_create_account_templates.py
--rw-r--r--   0 runner    (1001) docker     (121)     2239 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/system/cmdb/product/step_4_create_segment_templates.py
--rw-r--r--   0 runner    (1001) docker     (121)      443 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/system/cmdb/product/test_scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.382816 hamlet-9.9.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.382816 hamlet-9.9.1/tests/unit/backend/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.382816 hamlet-9.9.1/tests/unit/backend/automation_tasks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/backend/automation_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      684 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/backend/automation_tasks/test_automation_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.386816 hamlet-9.9.1/tests/unit/backend/common/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5919 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/backend/common/test_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     9131 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/backend/common/test_fsutils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.386816 hamlet-9.9.1/tests/unit/backend/engine/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/backend/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6453 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/backend/engine/test_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.386816 hamlet-9.9.1/tests/unit/command/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.386816 hamlet-9.9.1/tests/unit/command/component/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3176 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/component/test_component_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     7455 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/component/test_occurrence.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.386816 hamlet-9.9.1/tests/unit/command/deploy/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4360 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/deploy/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5497 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/deploy/test_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     4563 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/deploy/test_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.386816 hamlet-9.9.1/tests/unit/command/engine/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3175 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/engine/test_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.386816 hamlet-9.9.1/tests/unit/command/entrance/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/entrance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1335 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/entrance/test_invoke.py
--rw-r--r--   0 runner    (1001) docker     (121)     2348 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/entrance/test_list.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.386816 hamlet-9.9.1/tests/unit/command/generate/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.386816 hamlet-9.9.1/tests/unit/command/generate/cmdb/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/generate/cmdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      898 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/generate/cmdb/test_account.py
--rw-r--r--   0 runner    (1001) docker     (121)     1035 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/generate/cmdb/test_product.py
--rw-r--r--   0 runner    (1001) docker     (121)      833 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/generate/cmdb/test_tenant.py
--rw-r--r--   0 runner    (1001) docker     (121)     5037 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/generate/test_generate_command.py
--rw-r--r--   0 runner    (1001) docker     (121)       56 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/generate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.386816 hamlet-9.9.1/tests/unit/command/layer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4802 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/layer/test_describe.py
--rw-r--r--   0 runner    (1001) docker     (121)     4817 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/layer/test_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     4637 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/layer/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.390816 hamlet-9.9.1/tests/unit/command/manage/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/manage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1856 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/manage/test_credentials_crypto.py
--rw-r--r--   0 runner    (1001) docker     (121)     1683 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/manage/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/manage/test_deployment.py
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/manage/test_file_crypto.py
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/manage/test_stack.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.390816 hamlet-9.9.1/tests/unit/command/reference/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/reference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4814 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/reference/test_describe.py
--rw-r--r--   0 runner    (1001) docker     (121)     4663 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/reference/test_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     4623 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/reference/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.390816 hamlet-9.9.1/tests/unit/command/release/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1506 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/release/test_transfer_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     1342 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/release/test_update_image_reference.py
--rw-r--r--   0 runner    (1001) docker     (121)     1432 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/release/test_upload_image.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.390816 hamlet-9.9.1/tests/unit/command/run/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1535 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/run/test_expo_app_publish.py
--rw-r--r--   0 runner    (1001) docker     (121)      724 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/run/test_lambda_func.py
--rw-r--r--   0 runner    (1001) docker     (121)      798 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/run/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)      789 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/run/test_sentry_release.py
--rw-r--r--   0 runner    (1001) docker     (121)     1417 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/run/test_task.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.390816 hamlet-9.9.1/tests/unit/command/schema/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3223 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/schema/test_create.py
--rw-r--r--   0 runner    (1001) docker     (121)     3097 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/schema/test_list.py
--rw-r--r--   0 runner    (1001) docker     (121)    16139 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/test_option_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 23:09:21.390816 hamlet-9.9.1/tests/unit/command/visual/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/visual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2833 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/visual/test_draw.py
--rw-r--r--   0 runner    (1001) docker     (121)     3443 2021-12-23 23:08:12.000000 hamlet-9.9.1/tests/unit/command/visual/test_list.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.570519 hamlet-9.9.1.dev1/
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.538519 hamlet-9.9.1.dev1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.546519 hamlet-9.9.1.dev1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1159 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1400 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      544 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      222 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)    17804 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1166 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      531 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     2342 2021-12-08 00:35:22.570519 hamlet-9.9.1.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1714 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.550519 hamlet-9.9.1.dev1/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      603 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      780 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/docs/backend_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/docs/command_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      446 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1159 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/docs/config_files.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      525 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.550519 hamlet-9.9.1.dev1/hamlet/
+-rw-r--r--   0 runner    (1001) docker     (121)      463 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      753 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2021-12-08 00:35:22.000000 hamlet-9.9.1.dev1/hamlet/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.550519 hamlet-9.9.1.dev1/hamlet/backend/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.550519 hamlet-9.9.1.dev1/hamlet/backend/automation/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/automation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.550519 hamlet-9.9.1.dev1/hamlet/backend/automation/confirm_builds/
+-rw-r--r--   0 runner    (1001) docker     (121)      730 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/automation/confirm_builds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.550519 hamlet-9.9.1.dev1/hamlet/backend/automation/construct_tree/
+-rw-r--r--   0 runner    (1001) docker     (121)     1125 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/automation/construct_tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.550519 hamlet-9.9.1.dev1/hamlet/backend/automation/manage_build_references/
+-rw-r--r--   0 runner    (1001) docker     (121)      982 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/automation/manage_build_references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.550519 hamlet-9.9.1.dev1/hamlet/backend/automation/manage_images/
+-rw-r--r--   0 runner    (1001) docker     (121)      707 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/automation/manage_images/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.550519 hamlet-9.9.1.dev1/hamlet/backend/automation/properties_file/
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/automation/properties_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.550519 hamlet-9.9.1.dev1/hamlet/backend/automation/save_cmdb_repos/
+-rw-r--r--   0 runner    (1001) docker     (121)      623 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/automation/save_cmdb_repos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.550519 hamlet-9.9.1.dev1/hamlet/backend/automation/set_automation_context/
+-rw-r--r--   0 runner    (1001) docker     (121)      768 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/automation/set_automation_context/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.550519 hamlet-9.9.1.dev1/hamlet/backend/automation/update_build_references/
+-rw-r--r--   0 runner    (1001) docker     (121)      648 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/automation/update_build_references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.550519 hamlet-9.9.1.dev1/hamlet/backend/automation_tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/automation_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1411 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/automation_tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.550519 hamlet-9.9.1.dev1/hamlet/backend/automation_tasks/save_repos/
+-rw-r--r--   0 runner    (1001) docker     (121)     1330 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/automation_tasks/save_repos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.550519 hamlet-9.9.1.dev1/hamlet/backend/automation_tasks/transfer_image/
+-rw-r--r--   0 runner    (1001) docker     (121)     1960 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/automation_tasks/transfer_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.550519 hamlet-9.9.1.dev1/hamlet/backend/automation_tasks/update_build/
+-rw-r--r--   0 runner    (1001) docker     (121)     1431 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/automation_tasks/update_build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.550519 hamlet-9.9.1.dev1/hamlet/backend/automation_tasks/upload_image/
+-rw-r--r--   0 runner    (1001) docker     (121)     1918 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/automation_tasks/upload_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.550519 hamlet-9.9.1.dev1/hamlet/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9008 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/common/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7029 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/common/fsutils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3275 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/common/runner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1004 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/common/shell_vars_to_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1304 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/common/shell_vars_to_json.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.550519 hamlet-9.9.1.dev1/hamlet/backend/container_registry/
+-rw-r--r--   0 runner    (1001) docker     (121)     7451 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/container_registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.550519 hamlet-9.9.1.dev1/hamlet/backend/create/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.550519 hamlet-9.9.1.dev1/hamlet/backend/create/template/
+-rw-r--r--   0 runner    (1001) docker     (121)     1341 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/create/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    49724 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/create/template/context_tree.py
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/create/template/create_template.py
+-rw-r--r--   0 runner    (1001) docker     (121)      858 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/create/template/environment.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11245 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/create/template/set_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4477 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/create/template/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.550519 hamlet-9.9.1.dev1/hamlet/backend/deploy/
+-rw-r--r--   0 runner    (1001) docker     (121)     3398 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/deploy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/draw/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/draw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1972 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/draw/diagram.py
+-rw-r--r--   0 runner    (1001) docker     (121)      777 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/draw/diagram_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8372 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/draw/render.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/engine/
+-rw-r--r--   0 runner    (1001) docker     (121)     6367 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/engine/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11737 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1923 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/engine/engine_code_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)      438 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/engine/engine_loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1162 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/engine/engine_part.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4551 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/engine/engine_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)      822 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/engine/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/engine/loaders/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/engine/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3121 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/engine/loaders/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3873 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/engine/loaders/train.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3872 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/engine/loaders/tram.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2689 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/engine/loaders/unicycle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7540 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/engine/loaders/user.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2021-12-08 00:35:07.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (121)     1645 2021-12-08 00:35:07.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/__pycache__/utils.cpython-38.pyc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2021-12-08 00:35:07.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/account/
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/account/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (121)      703 2021-12-08 00:35:07.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/account/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/account/template/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/account/template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/account/template/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (121)      198 2021-12-08 00:35:07.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/account/template/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/account/template/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.542519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/account/template/{{cookiecutter.account_name}}/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/account/template/{{cookiecutter.account_name}}/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      283 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/account/template/{{cookiecutter.account_name}}/config/account.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.542519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/account/template/{{cookiecutter.account_name}}/config/settings/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/account/template/{{cookiecutter.account_name}}/config/settings/shared/
+-rw-r--r--   0 runner    (1001) docker     (121)     1329 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/account/template/{{cookiecutter.account_name}}/config/settings/shared/settings.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.542519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/account/template/{{cookiecutter.account_name}}/infrastructure/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.542519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/account/template/{{cookiecutter.account_name}}/infrastructure/operations/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/account/template/{{cookiecutter.account_name}}/infrastructure/operations/shared/
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/account/template/{{cookiecutter.account_name}}/infrastructure/operations/shared/credentials.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (121)      441 2021-12-08 00:35:07.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (121)      198 2021-12-08 00:35:07.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (121)      271 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.542519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      536 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/product.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.542519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/settings/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/settings/shared/
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/settings/shared/settings.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/settings/{{cookiecutter.environment_name}}/
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/settings/{{cookiecutter.environment_name}}/settings.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/settings/{{cookiecutter.environment_name}}/{{cookiecutter.segment_name}}/
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/settings/{{cookiecutter.environment_name}}/{{cookiecutter.segment_name}}/settings.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.542519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/solutionsv2/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.542519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/solutionsv2/shared/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/solutionsv2/shared/{{cookiecutter.segment_name}}/
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/solutionsv2/shared/{{cookiecutter.segment_name}}/segment.json
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/solutionsv2/shared/{{cookiecutter.segment_name}}/solution.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/solutionsv2/{{cookiecutter.environment_name}}/
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/solutionsv2/{{cookiecutter.environment_name}}/environment.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/solutionsv2/{{cookiecutter.environment_name}}/{{cookiecutter.segment_name}}/
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/solutionsv2/{{cookiecutter.environment_name}}/{{cookiecutter.segment_name}}/segment.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.542519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/infrastructure/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.542519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/infrastructure/operations/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/infrastructure/operations/{{cookiecutter.environment_name}}/
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/infrastructure/operations/{{cookiecutter.environment_name}}/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/infrastructure/operations/{{cookiecutter.environment_name}}/{{cookiecutter.segment_name}}/
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/infrastructure/operations/{{cookiecutter.environment_name}}/{{cookiecutter.segment_name}}/credentials.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/tenant/
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/tenant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.554519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/tenant/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (121)      439 2021-12-08 00:35:07.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/tenant/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/tenant/template/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/tenant/template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/tenant/template/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (121)      197 2021-12-08 00:35:07.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/tenant/template/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (121)      217 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/tenant/template/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.542519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/tenant/template/{{cookiecutter._base_dir}}/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/tenant/template/{{cookiecutter._base_dir}}/{{cookiecutter.tenant_name}}/
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/tenant/template/{{cookiecutter._base_dir}}/{{cookiecutter.tenant_name}}/ipaddressgroups.json
+-rw-r--r--   0 runner    (1001) docker     (121)      440 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/tenant/template/{{cookiecutter._base_dir}}/{{cookiecutter.tenant_name}}/tenant.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1847 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/generate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/backend/manage/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/manage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/backend/manage/credential_crypto/
+-rw-r--r--   0 runner    (1001) docker     (121)      927 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/manage/credential_crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/backend/manage/crypto/
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/manage/crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/backend/manage/deployment/
+-rw-r--r--   0 runner    (1001) docker     (121)     1139 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/manage/deployment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/backend/manage/file_crypto/
+-rw-r--r--   0 runner    (1001) docker     (121)      675 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/manage/file_crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/backend/manage/stack/
+-rw-r--r--   0 runner    (1001) docker     (121)     1092 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/manage/stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/backend/query/
+-rw-r--r--   0 runner    (1001) docker     (121)     4714 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/query/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/backend/run/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/backend/run/expo_app_publish/
+-rw-r--r--   0 runner    (1001) docker     (121)     1144 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/run/expo_app_publish/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/backend/run/lambda_func/
+-rw-r--r--   0 runner    (1001) docker     (121)      754 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/run/lambda_func/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/backend/run/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (121)      846 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/run/pipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/backend/run/sentry_release/
+-rw-r--r--   0 runner    (1001) docker     (121)      789 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/run/sentry_release/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/backend/run/task/
+-rw-r--r--   0 runner    (1001) docker     (121)     1025 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/run/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/backend/setup/
+-rw-r--r--   0 runner    (1001) docker     (121)      527 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/setup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/backend/test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1818 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/test/generate.py
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/test/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/backend/test/renderer/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/test/renderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1883 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/test/renderer/testcases_template.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1537 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/test/run.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/backend/test/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/test/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      700 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/test/templates/cfn_lint_test_func_block.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1734 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/test/templates/cfn_structure_obj_block.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1674 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/test/templates/cfn_testcase_block.py.tmpl
+-rw-r--r--   0 runner    (1001) docker     (121)     1498 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/test/templates/checkov_test_func_block.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2276 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/test/templates/json_structure_obj_block.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2385 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/test/templates/json_validator_obj_block.py
+-rw-r--r--   0 runner    (1001) docker     (121)      758 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/test/templates/test_template_base.py.tmpl
+-rw-r--r--   0 runner    (1001) docker     (121)     1392 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/test/testcase_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/backend/unitlist/
+-rw-r--r--   0 runner    (1001) docker     (121)      871 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/backend/unitlist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/command/
+-rw-r--r--   0 runner    (1001) docker     (121)     1132 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/command/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (121)     2413 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/autocomplete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/command/autocomplete/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)      669 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/autocomplete/scripts/.hamlet-complete.bash
+-rw-r--r--   0 runner    (1001) docker     (121)      669 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/autocomplete/scripts/.hamlet-complete.fish
+-rw-r--r--   0 runner    (1001) docker     (121)      966 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/autocomplete/scripts/.hamlet-complete.zsh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/command/cmdb/
+-rw-r--r--   0 runner    (1001) docker     (121)     2291 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/cmdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.558519 hamlet-9.9.1.dev1/hamlet/command/common/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7465 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5202 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/common/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1341 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/common/display.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1707 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/common/engine_setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1932 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/common/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.562519 hamlet-9.9.1.dev1/hamlet/command/component/
+-rw-r--r--   0 runner    (1001) docker     (121)     1137 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      695 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/component/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2815 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/component/component_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3458 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/component/describe_occurrence.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1364 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/component/list_occurrences.py
+-rw-r--r--   0 runner    (1001) docker     (121)      637 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/component/query_occurrences.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.562519 hamlet-9.9.1.dev1/hamlet/command/deploy/
+-rw-r--r--   0 runner    (1001) docker     (121)      601 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2503 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/deploy/create.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2346 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/deploy/list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4182 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/deploy/run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3802 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/deploy/test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.562519 hamlet-9.9.1.dev1/hamlet/command/engine/
+-rw-r--r--   0 runner    (1001) docker     (121)     9848 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.562519 hamlet-9.9.1.dev1/hamlet/command/entrance/
+-rw-r--r--   0 runner    (1001) docker     (121)     3266 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/entrance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.562519 hamlet-9.9.1.dev1/hamlet/command/generate/
+-rw-r--r--   0 runner    (1001) docker     (121)      521 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4262 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/generate/cmdb.py
+-rw-r--r--   0 runner    (1001) docker     (121)      491 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/generate/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      492 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/generate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.562519 hamlet-9.9.1.dev1/hamlet/command/layer/
+-rw-r--r--   0 runner    (1001) docker     (121)     5109 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/layer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.562519 hamlet-9.9.1.dev1/hamlet/command/manage/
+-rw-r--r--   0 runner    (1001) docker     (121)      592 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/manage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2134 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/manage/credentials_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3181 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/manage/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1941 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/manage/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1007 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/manage/file_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2224 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/manage/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.562519 hamlet-9.9.1.dev1/hamlet/command/reference/
+-rw-r--r--   0 runner    (1001) docker     (121)     5126 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/reference/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.562519 hamlet-9.9.1.dev1/hamlet/command/release/
+-rw-r--r--   0 runner    (1001) docker     (121)     3777 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/release/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.562519 hamlet-9.9.1.dev1/hamlet/command/run/
+-rw-r--r--   0 runner    (1001) docker     (121)      598 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2182 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/run/expo_app_publish.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1017 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/run/lambda_func.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1362 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/run/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)      979 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/run/sentry_release.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1907 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/run/task.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.562519 hamlet-9.9.1.dev1/hamlet/command/schema/
+-rw-r--r--   0 runner    (1001) docker     (121)     4168 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.562519 hamlet-9.9.1.dev1/hamlet/command/setup/
+-rw-r--r--   0 runner    (1001) docker     (121)      507 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/setup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.562519 hamlet-9.9.1.dev1/hamlet/command/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      342 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3054 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/test/generate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1088 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/test/run.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.562519 hamlet-9.9.1.dev1/hamlet/command/visual/
+-rw-r--r--   0 runner    (1001) docker     (121)     5044 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/command/visual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1271 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/env.py
+-rw-r--r--   0 runner    (1001) docker     (121)      541 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.562519 hamlet-9.9.1.dev1/hamlet/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     2180 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/hamlet/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.550519 hamlet-9.9.1.dev1/hamlet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2342 2021-12-08 00:35:22.000000 hamlet-9.9.1.dev1/hamlet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    13705 2021-12-08 00:35:22.000000 hamlet-9.9.1.dev1/hamlet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-08 00:35:22.000000 hamlet-9.9.1.dev1/hamlet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-12-08 00:35:22.000000 hamlet-9.9.1.dev1/hamlet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2021-12-08 00:35:22.000000 hamlet-9.9.1.dev1/hamlet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-12-08 00:35:22.000000 hamlet-9.9.1.dev1/hamlet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      197 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.562519 hamlet-9.9.1.dev1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)      128 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/setup-hamlet.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2021-12-08 00:35:22.570519 hamlet-9.9.1.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2807 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.562519 hamlet-9.9.1.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2476 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.546519 hamlet-9.9.1.dev1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.546519 hamlet-9.9.1.dev1/tests/data/integration/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.546519 hamlet-9.9.1.dev1/tests/data/integration/backend/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.546519 hamlet-9.9.1.dev1/tests/data/integration/backend/test/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.562519 hamlet-9.9.1.dev1/tests/data/integration/backend/test/cf/
+-rw-r--r--   0 runner    (1001) docker     (121)      515 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/data/integration/backend/test/cf/insecure.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3296 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/data/integration/backend/test/cf/invalid-syntax.json
+-rw-r--r--   0 runner    (1001) docker     (121)      901 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/data/integration/backend/test/cf/secure.json
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/data/integration/backend/test/cf/structure.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3439 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/data/integration/backend/test/cf/valid-syntax.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.566519 hamlet-9.9.1.dev1/tests/data/integration/backend/test/testcase/
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/data/integration/backend/test/testcase/insecure-testcase.json
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/data/integration/backend/test/testcase/invalid-syntax-testcase.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2009 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/data/integration/backend/test/testcase/json-structure-bad-testcase.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2217 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/data/integration/backend/test/testcase/json-structure-good-testcase.json
+-rw-r--r--   0 runner    (1001) docker     (121)      220 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/data/integration/backend/test/testcase/secure-testcase.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1729 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/data/integration/backend/test/testcase/structure-bad-testcase.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1492 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/data/integration/backend/test/testcase/structure-good-testcase.json
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/data/integration/backend/test/testcase/valid-syntax-testcase.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.566519 hamlet-9.9.1.dev1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.566519 hamlet-9.9.1.dev1/tests/integration/backend/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/integration/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.566519 hamlet-9.9.1.dev1/tests/integration/backend/create/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/integration/backend/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.566519 hamlet-9.9.1.dev1/tests/integration/backend/create/template/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/integration/backend/create/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1024 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/integration/backend/create/template/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29098 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/integration/backend/create/template/test_context_tree.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1792 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/integration/backend/create/template/test_set_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1464 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/integration/backend/create/template/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.566519 hamlet-9.9.1.dev1/tests/integration/backend/test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/integration/backend/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/integration/backend/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3534 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/integration/backend/test/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2131 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/integration/backend/test/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5114 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/integration/backend/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.566519 hamlet-9.9.1.dev1/tests/system/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.566519 hamlet-9.9.1.dev1/tests/system/cmdb/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/system/cmdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.566519 hamlet-9.9.1.dev1/tests/system/cmdb/product/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/system/cmdb/product/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      879 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/system/cmdb/product/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      510 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/system/cmdb/product/step_1_install_engine.py
+-rw-r--r--   0 runner    (1001) docker     (121)      420 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/system/cmdb/product/step_2_create_cmdb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2632 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/system/cmdb/product/step_3_create_account_templates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2239 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/system/cmdb/product/step_4_create_segment_templates.py
+-rw-r--r--   0 runner    (1001) docker     (121)      443 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/system/cmdb/product/test_scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.566519 hamlet-9.9.1.dev1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.566519 hamlet-9.9.1.dev1/tests/unit/backend/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.566519 hamlet-9.9.1.dev1/tests/unit/backend/automation_tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/backend/automation_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      684 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/backend/automation_tasks/test_automation_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.566519 hamlet-9.9.1.dev1/tests/unit/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5919 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/backend/common/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9131 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/backend/common/test_fsutils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.566519 hamlet-9.9.1.dev1/tests/unit/backend/engine/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/backend/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6453 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/backend/engine/test_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.566519 hamlet-9.9.1.dev1/tests/unit/command/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.566519 hamlet-9.9.1.dev1/tests/unit/command/component/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3176 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/component/test_component_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7455 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/component/test_occurrence.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.566519 hamlet-9.9.1.dev1/tests/unit/command/deploy/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4360 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/deploy/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5497 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/deploy/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4563 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/deploy/test_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.566519 hamlet-9.9.1.dev1/tests/unit/command/engine/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3175 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/engine/test_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.570519 hamlet-9.9.1.dev1/tests/unit/command/entrance/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/entrance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1335 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/entrance/test_invoke.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2348 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/entrance/test_list.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.570519 hamlet-9.9.1.dev1/tests/unit/command/generate/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.570519 hamlet-9.9.1.dev1/tests/unit/command/generate/cmdb/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/generate/cmdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      898 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/generate/cmdb/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1035 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/generate/cmdb/test_product.py
+-rw-r--r--   0 runner    (1001) docker     (121)      833 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/generate/cmdb/test_tenant.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5037 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/generate/test_generate_command.py
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/generate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.570519 hamlet-9.9.1.dev1/tests/unit/command/layer/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4802 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/layer/test_describe.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4817 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/layer/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4637 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/layer/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.570519 hamlet-9.9.1.dev1/tests/unit/command/manage/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/manage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1856 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/manage/test_credentials_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1683 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/manage/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1512 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/manage/test_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1374 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/manage/test_file_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1310 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/manage/test_stack.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.570519 hamlet-9.9.1.dev1/tests/unit/command/reference/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/reference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4814 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/reference/test_describe.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4663 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/reference/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4623 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/reference/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.570519 hamlet-9.9.1.dev1/tests/unit/command/release/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1506 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/release/test_transfer_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1342 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/release/test_update_image_reference.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1432 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/release/test_upload_image.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.570519 hamlet-9.9.1.dev1/tests/unit/command/run/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1535 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/run/test_expo_app_publish.py
+-rw-r--r--   0 runner    (1001) docker     (121)      724 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/run/test_lambda_func.py
+-rw-r--r--   0 runner    (1001) docker     (121)      798 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/run/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)      789 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/run/test_sentry_release.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1417 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/run/test_task.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.570519 hamlet-9.9.1.dev1/tests/unit/command/schema/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3419 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/schema/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3816 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/schema/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16139 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/test_option_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 00:35:22.570519 hamlet-9.9.1.dev1/tests/unit/command/visual/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/visual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2833 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/visual/test_draw.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3443 2021-12-08 00:34:27.000000 hamlet-9.9.1.dev1/tests/unit/command/visual/test_list.py
```

### Comparing `hamlet-9.9.1/.github/workflows/changelog.yml` & `hamlet-9.9.1.dev1/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/.github/workflows/release.yml` & `hamlet-9.9.1.dev1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/.github/workflows/style.yml` & `hamlet-9.9.1.dev1/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/CHANGELOG.md` & `hamlet-9.9.1.dev1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,10 @@
 # Changelog
 
-## latest (2021-12-22)
-
-#### Fixes
-
-* variable naming for schema
-#### Refactorings
-
-* schema generation commands
-
-Full set of changes: [`9.10.1...latest`](https://github.com/hamlet-io/executor-python/compare/9.10.1...latest)
-
-## 9.10.1 (2021-12-18)
-
-#### Fixes
-
-* quoting for shell params ([#268](https://github.com/hamlet-io/executor-python/issues/268))
-#### Others
-
-* changelog bump ([#267](https://github.com/hamlet-io/executor-python/issues/267))
-
-Full set of changes: [`9.10.0...9.10.1`](https://github.com/hamlet-io/executor-python/compare/9.10.0...9.10.1)
-
-## 9.10.0 (2021-12-10)
-
-#### New Features
-
-* layer info updates
-#### Others
-
-* changelog bump ([#265](https://github.com/hamlet-io/executor-python/issues/265))
-
-Full set of changes: [`9.9.0...9.10.0`](https://github.com/hamlet-io/executor-python/compare/9.9.0...9.10.0)
-
-## 9.9.0 (2021-11-29)
+## latest (2021-11-27)
 
 #### New Features
 
 * (testing): enable full scenario testing
 * extend autocomplete support
 * update to click 8.x
 * add layer and component type info
@@ -47,18 +14,17 @@
 * tests with command update
 #### Refactorings
 
 * osx support for testing
 * align account infra to state dir
 #### Others
 
-* changelog bump ([#258](https://github.com/hamlet-io/executor-python/issues/258))
 * fix formatting
 
-Full set of changes: [`9.8.1...9.9.0`](https://github.com/hamlet-io/executor-python/compare/9.8.1...9.9.0)
+Full set of changes: [`9.8.1...latest`](https://github.com/hamlet-io/executor-python/compare/9.8.1...latest)
 
 ## 9.8.1 (2021-11-07)
 
 #### Fixes
 
 * (docs): updates to README
 #### Others
```

### Comparing `hamlet-9.9.1/CONTRIBUTING.md` & `hamlet-9.9.1.dev1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/LICENSE` & `hamlet-9.9.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/Makefile` & `hamlet-9.9.1.dev1/Makefile`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/PKG-INFO` & `hamlet-9.9.1.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hamlet
-Version: 9.9.1
+Version: 9.9.1.dev1
 Summary: Building your infrastructure
 Home-page: https://hamlet.io
 Author: Hamlet
 License: GPLv3
 Project-URL: Repository, https://github.com/hamlet-io/executor-python
 Platform: UNKNOWN
 Classifier: Natural Language :: English
```

### Comparing `hamlet-9.9.1/README.md` & `hamlet-9.9.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/docs/Makefile` & `hamlet-9.9.1.dev1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/docs/backend_reference.rst` & `hamlet-9.9.1.dev1/docs/backend_reference.rst`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/docs/config_files.rst` & `hamlet-9.9.1.dev1/docs/config_files.rst`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/docs/index.rst` & `hamlet-9.9.1.dev1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/__init__.py` & `hamlet-9.9.1.dev1/hamlet/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/automation/confirm_builds/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/automation/confirm_builds/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/automation/construct_tree/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/automation/construct_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/automation/manage_build_references/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/automation/manage_build_references/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/automation/manage_images/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/automation/manage_images/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/automation/properties_file/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/automation/properties_file/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/automation/save_cmdb_repos/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/automation/save_cmdb_repos/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/automation/set_automation_context/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/automation/set_automation_context/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/automation/update_build_references/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/automation/update_build_references/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/automation_tasks/base.py` & `hamlet-9.9.1.dev1/hamlet/backend/automation_tasks/base.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/automation_tasks/save_repos/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/automation_tasks/save_repos/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/automation_tasks/transfer_image/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/automation_tasks/transfer_image/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/automation_tasks/update_build/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/automation_tasks/update_build/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/automation_tasks/upload_image/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/automation_tasks/upload_image/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/common/context.py` & `hamlet-9.9.1.dev1/hamlet/backend/common/context.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/common/fsutils.py` & `hamlet-9.9.1.dev1/hamlet/backend/common/fsutils.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/common/runner.py` & `hamlet-9.9.1.dev1/hamlet/backend/common/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         if value is not None:
             if isinstance(value, bool):
                 if value:
                     options_list.append(str(key))
             elif isinstance(value, tuple):
                 for instance in value:
                     options_list.append(str(key))
-                    options_list.append(str(f"'{instance}'"))
+                    options_list.append(str(instance))
             else:
                 options_list.append(str(key))
                 options_list.append(str(f"'{value}'"))
     script_fullpath = os.path.join(script_path, script_name)
     return " ".join([script_fullpath] + options_list + args)
```

### Comparing `hamlet-9.9.1/hamlet/backend/common/shell_vars_to_json.py` & `hamlet-9.9.1.dev1/hamlet/backend/common/shell_vars_to_json.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/common/shell_vars_to_json.sh` & `hamlet-9.9.1.dev1/hamlet/backend/common/shell_vars_to_json.sh`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/container_registry/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/container_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/create/template/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/create/template/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     deployment_unit_subset=None,
     deployment_mode=None,
     generation_provider=None,
     generation_framework=None,
     generation_input_source=None,
     output_dir=None,
     disable_output_cleanup=None,
-    entrance_parameters=None,
     log_level=None,
     root_dir=None,
     tenant=None,
     account=None,
     product=None,
     environment=None,
     segment=None,
@@ -38,15 +37,14 @@
         "-z": deployment_unit_subset,
         "-d": deployment_mode,
         "-p": generation_provider,
         "-f": generation_framework,
         "-i": generation_input_source,
         "-o": output_dir,
         "-x": disable_output_cleanup,
-        "-y": entrance_parameters,
     }
     env = {
         "GENERATION_LOG_LEVEL": log_level,
         "ROOT_DIR": root_dir,
         "TENANT": tenant,
         "ACCOUNT": account,
         "PRODUCT": product,
```

### Comparing `hamlet-9.9.1/hamlet/backend/create/template/context_tree.py` & `hamlet-9.9.1.dev1/hamlet/backend/create/template/context_tree.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/create/template/environment.py` & `hamlet-9.9.1.dev1/hamlet/backend/create/template/environment.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/create/template/set_context.py` & `hamlet-9.9.1.dev1/hamlet/backend/create/template/set_context.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/create/template/utils.py` & `hamlet-9.9.1.dev1/hamlet/backend/create/template/utils.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/deploy/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/draw/diagram.py` & `hamlet-9.9.1.dev1/hamlet/backend/draw/diagram.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/draw/diagram_schema.py` & `hamlet-9.9.1.dev1/hamlet/backend/draw/diagram_schema.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/draw/render.py` & `hamlet-9.9.1.dev1/hamlet/backend/draw/render.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/engine/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/engine/engine.py` & `hamlet-9.9.1.dev1/hamlet/backend/engine/engine.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/engine/engine_code_source.py` & `hamlet-9.9.1.dev1/hamlet/backend/engine/engine_code_source.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/engine/engine_part.py` & `hamlet-9.9.1.dev1/hamlet/backend/engine/engine_part.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/engine/engine_source.py` & `hamlet-9.9.1.dev1/hamlet/backend/engine/engine_source.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/engine/exceptions.py` & `hamlet-9.9.1.dev1/hamlet/backend/engine/exceptions.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/engine/loaders/base.py` & `hamlet-9.9.1.dev1/hamlet/backend/engine/loaders/base.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/engine/loaders/train.py` & `hamlet-9.9.1.dev1/hamlet/backend/engine/loaders/train.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/engine/loaders/tram.py` & `hamlet-9.9.1.dev1/hamlet/backend/engine/loaders/tram.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/engine/loaders/unicycle.py` & `hamlet-9.9.1.dev1/hamlet/backend/engine/loaders/unicycle.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/engine/loaders/user.py` & `hamlet-9.9.1.dev1/hamlet/backend/engine/loaders/user.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/generate/__pycache__/utils.cpython-38.pyc` & `hamlet-9.9.1.dev1/hamlet/backend/generate/__pycache__/utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Dec 23 23:08:12 2021 UTC, .py size: 1847 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 5c01 c561 3707 0000  U.......\..a7...
+00000000: 550d 0d0a 0000 0000 93fd af61 3707 0000  U..........a7...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a06 0100 6400 6403 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6404 6405 8400 5a09 640a  m.Z...d.d...Z.d.
 00000070: 6406 6407 8401 5a0a 6408 6409 8400 5a05  d.d...Z.d.d...Z.
```

### Comparing `hamlet-9.9.1/hamlet/backend/generate/cmdb/account/__pycache__/__init__.cpython-38.pyc` & `hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/account/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Dec 23 23:08:12 2021 UTC, .py size: 337 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 5c01 c561 5101 0000  U.......\..aQ...
+00000000: 550d 0d0a 0000 0000 93fd af61 5101 0000  U..........aQ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6403 6404 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a06 0100 6405 6406 8400 5a07 6407  m.Z...d.d...Z.d.
 00000060: 6408 8400 5a08 6401 5300 2909 e900 0000  d...Z.d.S.).....
 00000070: 004e 2901 da05 7574 696c 73e9 0100 0000  .N)...utils.....
```

### Comparing `hamlet-9.9.1/hamlet/backend/generate/cmdb/account/template/{{cookiecutter.account_name}}/config/settings/shared/settings.json` & `hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/account/template/{{cookiecutter.account_name}}/config/settings/shared/settings.json`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/product.json` & `hamlet-9.9.1.dev1/hamlet/backend/generate/cmdb/product/template/{{cookiecutter.product_name}}/config/product.json`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/generate/utils.py` & `hamlet-9.9.1.dev1/hamlet/backend/generate/utils.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/manage/credential_crypto/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/manage/credential_crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/manage/crypto/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/manage/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/manage/deployment/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/manage/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/manage/file_crypto/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/manage/file_crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/manage/stack/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/manage/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/query/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/query/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/run/expo_app_publish/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/run/expo_app_publish/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/run/lambda_func/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/run/lambda_func/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/run/pipeline/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/run/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/run/sentry_release/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/run/sentry_release/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/run/task/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/run/task/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/setup/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/test/generate.py` & `hamlet-9.9.1.dev1/hamlet/backend/test/generate.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/test/renderer/testcases_template.py` & `hamlet-9.9.1.dev1/hamlet/backend/test/renderer/testcases_template.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/test/run.py` & `hamlet-9.9.1.dev1/hamlet/backend/test/run.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/test/templates/cfn_lint_test_func_block.py` & `hamlet-9.9.1.dev1/hamlet/backend/test/templates/cfn_lint_test_func_block.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/test/templates/cfn_structure_obj_block.py` & `hamlet-9.9.1.dev1/hamlet/backend/test/templates/cfn_structure_obj_block.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/test/templates/cfn_testcase_block.py.tmpl` & `hamlet-9.9.1.dev1/hamlet/backend/test/templates/cfn_testcase_block.py.tmpl`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/test/templates/checkov_test_func_block.py` & `hamlet-9.9.1.dev1/hamlet/backend/test/templates/checkov_test_func_block.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/test/templates/json_structure_obj_block.py` & `hamlet-9.9.1.dev1/hamlet/backend/test/templates/json_structure_obj_block.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/test/templates/json_validator_obj_block.py` & `hamlet-9.9.1.dev1/hamlet/backend/test/templates/json_validator_obj_block.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/test/templates/test_template_base.py.tmpl` & `hamlet-9.9.1.dev1/hamlet/backend/test/templates/test_template_base.py.tmpl`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/test/testcase_schema.py` & `hamlet-9.9.1.dev1/hamlet/backend/test/testcase_schema.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/backend/unitlist/__init__.py` & `hamlet-9.9.1.dev1/hamlet/backend/unitlist/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/__init__.py` & `hamlet-9.9.1.dev1/hamlet/command/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/autocomplete/__init__.py` & `hamlet-9.9.1.dev1/hamlet/command/autocomplete/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/autocomplete/scripts/.hamlet-complete.bash` & `hamlet-9.9.1.dev1/hamlet/command/autocomplete/scripts/.hamlet-complete.bash`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/autocomplete/scripts/.hamlet-complete.fish` & `hamlet-9.9.1.dev1/hamlet/command/autocomplete/scripts/.hamlet-complete.fish`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/autocomplete/scripts/.hamlet-complete.zsh` & `hamlet-9.9.1.dev1/hamlet/command/autocomplete/scripts/.hamlet-complete.zsh`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/cmdb/__init__.py` & `hamlet-9.9.1.dev1/hamlet/command/cmdb/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/common/config.py` & `hamlet-9.9.1.dev1/hamlet/command/common/config.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/common/decorators.py` & `hamlet-9.9.1.dev1/hamlet/command/common/decorators.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/common/display.py` & `hamlet-9.9.1.dev1/hamlet/command/common/display.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/common/engine_setup.py` & `hamlet-9.9.1.dev1/hamlet/command/common/engine_setup.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/common/exceptions.py` & `hamlet-9.9.1.dev1/hamlet/command/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/component/__init__.py` & `hamlet-9.9.1.dev1/hamlet/command/component/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/component/common.py` & `hamlet-9.9.1.dev1/hamlet/command/component/common.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/component/component_types.py` & `hamlet-9.9.1.dev1/hamlet/command/component/component_types.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/component/describe_occurrence.py` & `hamlet-9.9.1.dev1/hamlet/command/component/describe_occurrence.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/component/list_occurrences.py` & `hamlet-9.9.1.dev1/hamlet/command/component/list_occurrences.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/component/query_occurrences.py` & `hamlet-9.9.1.dev1/hamlet/command/component/query_occurrences.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/deploy/__init__.py` & `hamlet-9.9.1.dev1/hamlet/command/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/deploy/create.py` & `hamlet-9.9.1.dev1/hamlet/command/deploy/create.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/deploy/list.py` & `hamlet-9.9.1.dev1/hamlet/command/deploy/list.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/deploy/run.py` & `hamlet-9.9.1.dev1/hamlet/command/deploy/run.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/deploy/test.py` & `hamlet-9.9.1.dev1/hamlet/command/deploy/test.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/engine/__init__.py` & `hamlet-9.9.1.dev1/hamlet/command/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/entrance/__init__.py` & `hamlet-9.9.1.dev1/hamlet/command/entrance/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/generate/__init__.py` & `hamlet-9.9.1.dev1/hamlet/command/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/generate/cmdb.py` & `hamlet-9.9.1.dev1/hamlet/command/generate/cmdb.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/layer/__init__.py` & `hamlet-9.9.1.dev1/hamlet/command/layer/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/manage/__init__.py` & `hamlet-9.9.1.dev1/hamlet/command/manage/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/manage/credentials_crypto.py` & `hamlet-9.9.1.dev1/hamlet/command/manage/credentials_crypto.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/manage/crypto.py` & `hamlet-9.9.1.dev1/hamlet/command/manage/crypto.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/manage/deployment.py` & `hamlet-9.9.1.dev1/hamlet/command/manage/deployment.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/manage/file_crypto.py` & `hamlet-9.9.1.dev1/hamlet/command/manage/file_crypto.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/manage/stack.py` & `hamlet-9.9.1.dev1/hamlet/command/manage/stack.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/reference/__init__.py` & `hamlet-9.9.1.dev1/hamlet/command/reference/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/release/__init__.py` & `hamlet-9.9.1.dev1/hamlet/command/release/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/run/__init__.py` & `hamlet-9.9.1.dev1/hamlet/command/run/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/run/expo_app_publish.py` & `hamlet-9.9.1.dev1/hamlet/command/run/expo_app_publish.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/run/lambda_func.py` & `hamlet-9.9.1.dev1/hamlet/command/run/lambda_func.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/run/pipeline.py` & `hamlet-9.9.1.dev1/hamlet/command/run/pipeline.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/run/sentry_release.py` & `hamlet-9.9.1.dev1/hamlet/command/run/sentry_release.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/run/task.py` & `hamlet-9.9.1.dev1/hamlet/command/run/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,65 +4,63 @@
 from hamlet.command.common.config import pass_options
 
 
 @click.command(
     "task", short_help="Run an ECS task", context_settings=dict(max_content_width=240)
 )
 @click.option(
-    "-t",
-    "--tier",
-    required=True,
-    help="name of the tier in the solution where the task is defined",
+    "-c",
+    "--container-id",
+    help="name of the container that environment details are applied to",
+)
+@click.option(
+    "-d",
+    "--delay",
+    help="interval between checking the progress of the task",
+    type=click.INT,
+    default=30,
+    show_default=True,
+)
+@click.option(
+    "-e",
+    "--env",
+    "env_name",
+    help="name of an environment variable to define for the task",
 )
 @click.option(
     "-i",
     "--component",
     required=True,
     help="name of the ecs component in the solution where the task is defined",
 )
 @click.option(
     "-j", "--component-instance", help="instance of the ecs cluster to run the task on"
 )
 @click.option(
     "-k", "--component-version", help="version of the ecs clsuter to run the task on"
 )
 @click.option(
-    "-w",
-    "--task",
+    "-t",
+    "--tier",
     required=True,
-    help="name of the task to be run",
-)
-@click.option("-x", "--instance", help="instance of the task to be run")
-@click.option("-y", "--version", help="version of the task to be run")
-@click.option(
-    "-c",
-    "--container-id",
-    help="name of the container that environment details are applied to",
-)
-@click.option(
-    "-e",
-    "--env",
-    "env_name",
-    help="name of an environment variable to define for the task",
-    multiple=True,
+    help="name of the tier in the solution where the task is defined",
 )
 @click.option(
     "-v",
     "--value",
-    help="value for the last environment value defined for the task",
-    multiple=True,
+    help="value for the last environment value defined (via -e) for the task",
 )
 @click.option(
-    "-d",
-    "--delay",
-    help="interval between checking the progress of the task",
-    type=click.INT,
-    default=30,
-    show_default=True,
+    "-w",
+    "--task",
+    required=True,
+    help="name of the task to be run",
 )
+@click.option("-x", "--instance", help="instance of the task to be run")
+@click.option("-y", "--version", help="version of the task to be run")
 @exceptions.backend_handler()
 @pass_options
 def task(options, **kwargs):
     """
     Run an ECS task
 
     \b
```

### Comparing `hamlet-9.9.1/hamlet/command/schema/__init__.py` & `hamlet-9.9.1.dev1/hamlet/command/schema/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,86 +8,113 @@
 from hamlet.command.common.display import json_or_table_option, wrap_text
 from hamlet.command.common import exceptions
 from hamlet.command.common.config import pass_options
 from hamlet.backend import query as query_backend
 from hamlet.backend.create import template as create_template_backend
 
 
-def find_schemas_from_options(options, schema):
+def find_schemas_from_options(options, schema_type, schema_instances):
     query_args = {
         **options.opts,
         "deployment_mode": None,
-        "generation_entrance": "schemalist",
-        "output_filename": "schemalist-schemacontract.json",
+        "generation_entrance": "schemaset",
+        "output_filename": "schemaset-schemacontract.json",
         "use_cache": False,
     }
     available_schemas = query_backend.run(
         **query_args, cwd=os.getcwd(), query_text=LIST_SCHEMAS_QUERY
     )
 
     schemas = []
 
-    for available_schema in available_schemas:
-        if re.fullmatch(schema, available_schema["Schema"]):
-            schemas.append(available_schema)
+    for schema in available_schemas:
+        if re.fullmatch(schema_type, schema["SchemaType"]):
+            for schema_instance in schema_instances:
+                if re.fullmatch(schema_instance, schema["SchemaInstance"]):
+                    schemas.append(schema)
     return schemas
 
 
 @cli.group("schema", context_settings=dict(max_content_width=240))
 def group():
     """
-    Generates JSONSchemas for Hamlet Configuration Scopes
+    Generates JSONSchema files for Hamlet data types
     """
     pass
 
 
-LIST_SCHEMAS_QUERY = "Stages[].Steps[]" ".{" "Schema:Parameters.Schema" "}"
+LIST_SCHEMAS_QUERY = (
+    "Stages[].Steps[]"
+    ".{"
+    "SchemaType:Parameters.SchemaType,"
+    "SchemaInstance:Parameters.SchemaInstance"
+    "}"
+)
 
 
 def schema_table(data):
     tablerows = []
     for row in data:
         tablerows.append(
             [
-                wrap_text(row["Schema"]),
+                wrap_text(row["SchemaType"]),
+                wrap_text(row["SchemaInstance"]),
             ]
         )
-    return tabulate(tablerows, headers=["Schema"], tablefmt="github")
+    return tabulate(
+        tablerows, headers=["SchemaType", "SchemaInstance"], tablefmt="github"
+    )
 
 
 @group.command(
     "list-schemas", short_help="", context_settings=dict(max_content_width=240)
 )
 @click.option(
-    "-s",
-    "--schema",
+    "-t",
+    "--schema-type",
     default=".*",
     show_default=True,
-    help="A schema name pattern to filter results",
+    help="A schema type name pattern to filter results",
+)
+@click.option(
+    "-i",
+    "--schema-instance",
+    default=[".*"],
+    show_default=True,
+    multiple=True,
+    help="A schema instance name pattern to filter results",
 )
 @json_or_table_option(schema_table)
 @exceptions.backend_handler()
 @pass_options
-def list_schemas(options, schema):
+def list_schemas(options, schema_type, schema_instance):
     """
-    List the available JSONSchemas that can be created
+    List the available JSON schemas by data type
     """
 
-    return find_schemas_from_options(options, schema)
+    return find_schemas_from_options(options, schema_type, schema_instance)
 
 
 @group.command(
     "create-schemas", short_help="", context_settings=dict(max_content_width=240)
 )
 @click.option(
-    "-s",
-    "--schema",
+    "-t",
+    "--schema-type",
     default=".*",
     show_default=True,
-    help="A schema name pattern to filter the schemas that will be generated",
+    help="A schema type name pattern to filter results",
+)
+@click.option(
+    "-i",
+    "--schema-instance",
+    default=[".*"],
+    show_default=True,
+    multiple=True,
+    help="A schema instance name pattern to filter results",
 )
 @click.option(
     "-o",
     "--output-dir",
     type=click.Path(
         file_okay=False,
         dir_okay=True,
@@ -95,38 +122,41 @@
         readable=True,
     ),
     required=True,
     help="the directory where the outputs will be saved",
 )
 @exceptions.backend_handler()
 @pass_options
-def create_schemas(options, schema, output_dir, **kwargs):
+def create_schemas(options, schema_type, schema_instance, output_dir, **kwargs):
     """
-    Create the JSON schema files available
+    Create Hamlet data type schemas
     """
 
-    schema_list = find_schemas_from_options(options, schema)
+    schemas = find_schemas_from_options(options, schema_type, schema_instance)
 
-    if len(schema_list) == 0:
+    if len(schemas) == 0:
         raise exceptions.CommandError("No schemas found")
 
-    for schema_task in schema_list:
+    for schema in schemas:
+        schema_type = schema["SchemaType"]
+        schema_instance = schema["SchemaInstance"]
         click.echo("")
         click.echo(
             (
                 click.style(
-                    f"[*] Schema: {schema_task['Schema']}",
+                    f"[*] Schema: {schema_type}/{schema_instance}",
                     bold=True,
                     fg="green",
                 )
             )
         )
         click.echo("")
 
         template_args = {
             **options.opts,
             "entrance": "schema",
+            "deployment_group": schema_type,
+            "deployment_unit": schema_instance,
             "output_dir": output_dir,
-            "entrance_parameters": f"Schema={schema_task['Schema']}",
         }
 
         create_template_backend.run(**template_args, _is_cli=True)
```

### Comparing `hamlet-9.9.1/hamlet/command/test/generate.py` & `hamlet-9.9.1.dev1/hamlet/command/test/generate.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/test/run.py` & `hamlet-9.9.1.dev1/hamlet/command/test/run.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/command/visual/__init__.py` & `hamlet-9.9.1.dev1/hamlet/command/visual/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/env.py` & `hamlet-9.9.1.dev1/hamlet/env.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/loggers.py` & `hamlet-9.9.1.dev1/hamlet/loggers.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet/utils/__init__.py` & `hamlet-9.9.1.dev1/hamlet/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/hamlet.egg-info/PKG-INFO` & `hamlet-9.9.1.dev1/hamlet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hamlet
-Version: 9.9.1
+Version: 9.9.1.dev1
 Summary: Building your infrastructure
 Home-page: https://hamlet.io
 Author: Hamlet
 License: GPLv3
 Project-URL: Repository, https://github.com/hamlet-io/executor-python
 Platform: UNKNOWN
 Classifier: Natural Language :: English
```

### Comparing `hamlet-9.9.1/hamlet.egg-info/SOURCES.txt` & `hamlet-9.9.1.dev1/hamlet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/setup.py` & `hamlet-9.9.1.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/conftest.py` & `hamlet-9.9.1.dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/data/integration/backend/test/cf/insecure.json` & `hamlet-9.9.1.dev1/tests/data/integration/backend/test/cf/insecure.json`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/data/integration/backend/test/cf/invalid-syntax.json` & `hamlet-9.9.1.dev1/tests/data/integration/backend/test/cf/invalid-syntax.json`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/data/integration/backend/test/cf/secure.json` & `hamlet-9.9.1.dev1/tests/data/integration/backend/test/cf/secure.json`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/data/integration/backend/test/cf/valid-syntax.json` & `hamlet-9.9.1.dev1/tests/data/integration/backend/test/cf/valid-syntax.json`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/data/integration/backend/test/testcase/json-structure-bad-testcase.json` & `hamlet-9.9.1.dev1/tests/data/integration/backend/test/testcase/json-structure-bad-testcase.json`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/data/integration/backend/test/testcase/json-structure-good-testcase.json` & `hamlet-9.9.1.dev1/tests/data/integration/backend/test/testcase/json-structure-good-testcase.json`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/data/integration/backend/test/testcase/structure-bad-testcase.json` & `hamlet-9.9.1.dev1/tests/data/integration/backend/test/testcase/structure-bad-testcase.json`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/data/integration/backend/test/testcase/structure-good-testcase.json` & `hamlet-9.9.1.dev1/tests/data/integration/backend/test/testcase/structure-good-testcase.json`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/integration/backend/create/template/conftest.py` & `hamlet-9.9.1.dev1/tests/integration/backend/create/template/conftest.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/integration/backend/create/template/test_context_tree.py` & `hamlet-9.9.1.dev1/tests/integration/backend/create/template/test_context_tree.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/integration/backend/create/template/test_set_context.py` & `hamlet-9.9.1.dev1/tests/integration/backend/create/template/test_set_context.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/integration/backend/create/template/test_utils.py` & `hamlet-9.9.1.dev1/tests/integration/backend/create/template/test_utils.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/integration/backend/test/test_generate.py` & `hamlet-9.9.1.dev1/tests/integration/backend/test/test_generate.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/integration/backend/test/test_run.py` & `hamlet-9.9.1.dev1/tests/integration/backend/test/test_run.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/integration/backend/test/test_utils.py` & `hamlet-9.9.1.dev1/tests/integration/backend/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/system/cmdb/product/conftest.py` & `hamlet-9.9.1.dev1/tests/system/cmdb/product/conftest.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/system/cmdb/product/step_3_create_account_templates.py` & `hamlet-9.9.1.dev1/tests/system/cmdb/product/step_3_create_account_templates.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/system/cmdb/product/step_4_create_segment_templates.py` & `hamlet-9.9.1.dev1/tests/system/cmdb/product/step_4_create_segment_templates.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/backend/automation_tasks/test_automation_runner.py` & `hamlet-9.9.1.dev1/tests/unit/backend/automation_tasks/test_automation_runner.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/backend/common/test_context.py` & `hamlet-9.9.1.dev1/tests/unit/backend/common/test_context.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/backend/common/test_fsutils.py` & `hamlet-9.9.1.dev1/tests/unit/backend/common/test_fsutils.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/backend/engine/test_engine.py` & `hamlet-9.9.1.dev1/tests/unit/backend/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/component/test_component_types.py` & `hamlet-9.9.1.dev1/tests/unit/command/component/test_component_types.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/component/test_occurrence.py` & `hamlet-9.9.1.dev1/tests/unit/command/component/test_occurrence.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/deploy/test_deploy.py` & `hamlet-9.9.1.dev1/tests/unit/command/deploy/test_deploy.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/deploy/test_list.py` & `hamlet-9.9.1.dev1/tests/unit/command/deploy/test_list.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/deploy/test_test.py` & `hamlet-9.9.1.dev1/tests/unit/command/deploy/test_test.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/engine/test_engine.py` & `hamlet-9.9.1.dev1/tests/unit/command/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/entrance/test_invoke.py` & `hamlet-9.9.1.dev1/tests/unit/command/entrance/test_invoke.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/entrance/test_list.py` & `hamlet-9.9.1.dev1/tests/unit/command/entrance/test_list.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/generate/cmdb/test_account.py` & `hamlet-9.9.1.dev1/tests/unit/command/generate/cmdb/test_account.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/generate/cmdb/test_product.py` & `hamlet-9.9.1.dev1/tests/unit/command/generate/cmdb/test_product.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/generate/cmdb/test_tenant.py` & `hamlet-9.9.1.dev1/tests/unit/command/generate/cmdb/test_tenant.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/generate/test_generate_command.py` & `hamlet-9.9.1.dev1/tests/unit/command/generate/test_generate_command.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/layer/test_describe.py` & `hamlet-9.9.1.dev1/tests/unit/command/layer/test_describe.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/layer/test_list.py` & `hamlet-9.9.1.dev1/tests/unit/command/layer/test_list.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/layer/test_query.py` & `hamlet-9.9.1.dev1/tests/unit/command/layer/test_query.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/manage/test_credentials_crypto.py` & `hamlet-9.9.1.dev1/tests/unit/command/manage/test_credentials_crypto.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/manage/test_crypto.py` & `hamlet-9.9.1.dev1/tests/unit/command/manage/test_crypto.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/manage/test_deployment.py` & `hamlet-9.9.1.dev1/tests/unit/command/manage/test_deployment.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/manage/test_file_crypto.py` & `hamlet-9.9.1.dev1/tests/unit/command/manage/test_file_crypto.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/manage/test_stack.py` & `hamlet-9.9.1.dev1/tests/unit/command/manage/test_stack.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/reference/test_describe.py` & `hamlet-9.9.1.dev1/tests/unit/command/reference/test_describe.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/reference/test_list.py` & `hamlet-9.9.1.dev1/tests/unit/command/reference/test_list.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/reference/test_query.py` & `hamlet-9.9.1.dev1/tests/unit/command/reference/test_query.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/release/test_transfer_image.py` & `hamlet-9.9.1.dev1/tests/unit/command/release/test_transfer_image.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/release/test_update_image_reference.py` & `hamlet-9.9.1.dev1/tests/unit/command/release/test_update_image_reference.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/release/test_upload_image.py` & `hamlet-9.9.1.dev1/tests/unit/command/release/test_upload_image.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/run/test_expo_app_publish.py` & `hamlet-9.9.1.dev1/tests/unit/command/run/test_expo_app_publish.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/run/test_lambda_func.py` & `hamlet-9.9.1.dev1/tests/unit/command/run/test_lambda_func.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/run/test_pipeline.py` & `hamlet-9.9.1.dev1/tests/unit/command/run/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/run/test_sentry_release.py` & `hamlet-9.9.1.dev1/tests/unit/command/run/test_sentry_release.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/run/test_task.py` & `hamlet-9.9.1.dev1/tests/unit/command/run/test_task.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/schema/test_create.py` & `hamlet-9.9.1.dev1/tests/unit/command/schema/test_create.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,105 +10,107 @@
 from tests.unit.command.test_option_generation import (
     run_options_test,
     run_validatable_option_test,
 )
 
 ALL_VALID_OPTIONS = collections.OrderedDict()
 ALL_VALID_OPTIONS["!-o,--output-dir"] = "output_dir"
-ALL_VALID_OPTIONS["-s,--schema"] = "Schema1"
+ALL_VALID_OPTIONS["-t,--schema-type"] = "SchemaType1"
+ALL_VALID_OPTIONS["-i,--schema-instance"] = "SchemaInstance1"
 
 
 def template_backend_run_mock(data):
     def run(
-        entrance="schemalist",
-        output_filename="schemalist-schemacontract.json",
+        entrance="schemaset",
+        output_filename="schemaset-schemacontract.json",
         deployment_mode=None,
         output_dir=None,
         generation_input_source=None,
         generation_provider=None,
         generation_framework=None,
         log_level=None,
         root_dir=None,
         tenant=None,
         account=None,
         product=None,
         environment=None,
         segment=None,
-        entrance_parameters=None,
     ):
         os.makedirs(output_dir, exist_ok=True)
         unitlist_filename = os.path.join(output_dir, output_filename)
         with open(unitlist_filename, "wt+") as f:
             json.dump(data, f)
 
     return run
 
 
-def mock_backend(schemalist=None):
+def mock_backend(schemaset=None):
     def decorator(func):
         @mock.patch("hamlet.command.schema.create_template_backend")
         @mock.patch("hamlet.backend.query.context.Context")
         @mock.patch("hamlet.backend.query.template")
         def wrapper(
             blueprint_mock, ContextClassMock, create_template_backend, *args, **kwargs
         ):
             with tempfile.TemporaryDirectory() as temp_cache_dir:
 
                 ContextObjectMock = ContextClassMock()
                 ContextObjectMock.md5_hash.return_value = str(
-                    hashlib.md5(str(schemalist).encode()).hexdigest()
+                    hashlib.md5(str(schemaset).encode()).hexdigest()
                 )
                 ContextObjectMock.cache_dir = temp_cache_dir
 
-                blueprint_mock.run.side_effect = template_backend_run_mock(schemalist)
+                blueprint_mock.run.side_effect = template_backend_run_mock(schemaset)
 
                 return func(
                     blueprint_mock,
                     ContextClassMock,
                     create_template_backend,
                     *args,
                     **kwargs
                 )
 
         return wrapper
 
     return decorator
 
 
-schema_list = {
+schema_set = {
     "Stages": [
         {
             "Id": "StageId1",
             "Steps": [
                 {
                     "Id": "StepId1",
                     "Parameters": {
-                        "Schema": "Schema1",
+                        "SchemaType": "SchemaType1",
+                        "SchemaInstance": "SchemaInstance1",
                     },
                 },
                 {
                     "Id": "StepId2",
                     "Parameters": {
-                        "Schema": "Schema2",
+                        "SchemaType": "SchemaType2",
+                        "SchemaInstance": "SchemaInstance2",
                     },
                 },
             ],
         }
     ]
 }
 
 
-@mock_backend(schema_list)
+@mock_backend(schema_set)
 def test_input_valid(blueprint_mock, ContextClassMock, create_template_backend):
     run_options_test(CliRunner(), create_schemas, ALL_VALID_OPTIONS, blueprint_mock.run)
 
 
-@mock_backend(schema_list)
+@mock_backend(schema_set)
 def test_input_validation(blueprint_mock, ContextClassMock, create_template_backend):
     runner = CliRunner()
     run_validatable_option_test(
         runner,
         create_schemas,
         create_template_backend.run,
-        {"-s": "Schema1", "-o": "."},
+        {"-t": "SchemaType1", "-i": "SchemaInstance1", "-o": "."},
         [],
     )
```

### Comparing `hamlet-9.9.1/tests/unit/command/test_option_generation.py` & `hamlet-9.9.1.dev1/tests/unit/command/test_option_generation.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/visual/test_draw.py` & `hamlet-9.9.1.dev1/tests/unit/command/visual/test_draw.py`

 * *Files identical despite different names*

### Comparing `hamlet-9.9.1/tests/unit/command/visual/test_list.py` & `hamlet-9.9.1.dev1/tests/unit/command/visual/test_list.py`

 * *Files identical despite different names*

