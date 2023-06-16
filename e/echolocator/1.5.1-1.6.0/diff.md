# Comparing `tmp/echolocator-1.5.1.tar.gz` & `tmp/echolocator-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echolocator-1.5.1.tar", last modified: Thu Jun  8 13:35:26 2023, max compression
+gzip compressed data, was "echolocator-1.6.0.tar", last modified: Fri Jun 16 11:31:46 2023, max compression
```

## Comparing `echolocator-1.5.1.tar` & `echolocator-1.6.0.tar`

### file list

```diff
@@ -1,213 +1,213 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.994854 echolocator-1.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.962853 echolocator-1.5.1/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-08 13:35:14.000000 echolocator-1.5.1/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.962853 echolocator-1.5.1/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-08 13:35:14.000000 echolocator-1.5.1/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-08 13:35:14.000000 echolocator-1.5.1/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-08 13:35:14.000000 echolocator-1.5.1/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-08 13:35:14.000000 echolocator-1.5.1/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-08 13:35:14.000000 echolocator-1.5.1/.dae-devops/docs/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-08 13:35:14.000000 echolocator-1.5.1/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-08 13:35:14.000000 echolocator-1.5.1/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-08 13:35:14.000000 echolocator-1.5.1/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-08 13:35:14.000000 echolocator-1.5.1/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.962853 echolocator-1.5.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-08 13:35:14.000000 echolocator-1.5.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-08 13:35:14.000000 echolocator-1.5.1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.966853 echolocator-1.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-08 13:35:14.000000 echolocator-1.5.1/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.946853 echolocator-1.5.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.966853 echolocator-1.5.1/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-08 13:35:14.000000 echolocator-1.5.1/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-08 13:35:14.000000 echolocator-1.5.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.966853 echolocator-1.5.1/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-08 13:35:14.000000 echolocator-1.5.1/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-08 13:35:14.000000 echolocator-1.5.1/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.966853 echolocator-1.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-06-08 13:35:14.000000 echolocator-1.5.1/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-08 13:35:14.000000 echolocator-1.5.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-08 13:35:14.000000 echolocator-1.5.1/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-08 13:35:14.000000 echolocator-1.5.1/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-08 13:35:14.000000 echolocator-1.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-08 13:35:14.000000 echolocator-1.5.1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-08 13:35:14.000000 echolocator-1.5.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.966853 echolocator-1.5.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-08 13:35:14.000000 echolocator-1.5.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-08 13:35:14.000000 echolocator-1.5.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-08 13:35:14.000000 echolocator-1.5.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-08 13:35:14.000000 echolocator-1.5.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 13:35:14.000000 echolocator-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-06-08 13:35:14.000000 echolocator-1.5.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-06-08 13:35:25.994854 echolocator-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-08 13:35:14.000000 echolocator-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.970853 echolocator-1.5.1/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-08 13:35:14.000000 echolocator-1.5.1/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.970853 echolocator-1.5.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.946853 echolocator-1.5.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.970853 echolocator-1.5.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-08 13:35:14.000000 echolocator-1.5.1/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-06-08 13:35:14.000000 echolocator-1.5.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.970853 echolocator-1.5.1/docs/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-08 13:35:14.000000 echolocator-1.5.1/docs/explanations/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-08 13:35:14.000000 echolocator-1.5.1/docs/explanations/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-08 13:35:14.000000 echolocator-1.5.1/docs/explanations/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-08 13:35:14.000000 echolocator-1.5.1/docs/explanations/todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.974853 echolocator-1.5.1/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-08 13:35:14.000000 echolocator-1.5.1/docs/how-to/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-08 13:35:14.000000 echolocator-1.5.1/docs/how-to/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-08 13:35:14.000000 echolocator-1.5.1/docs/how-to/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-08 13:35:14.000000 echolocator-1.5.1/docs/how-to/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-08 13:35:14.000000 echolocator-1.5.1/docs/how-to/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-08 13:35:14.000000 echolocator-1.5.1/docs/how-to/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.974853 echolocator-1.5.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-08 13:35:14.000000 echolocator-1.5.1/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-08 13:35:14.000000 echolocator-1.5.1/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-08 13:35:14.000000 echolocator-1.5.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.974853 echolocator-1.5.1/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-08 13:35:14.000000 echolocator-1.5.1/docs/reference/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-08 13:35:14.000000 echolocator-1.5.1/docs/reference/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-08 13:35:14.000000 echolocator-1.5.1/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-08 13:35:14.000000 echolocator-1.5.1/docs/reference/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.974853 echolocator-1.5.1/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-08 13:35:14.000000 echolocator-1.5.1/docs/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 13:35:14.000000 echolocator-1.5.1/docs/tutorials/tbd.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.974853 echolocator-1.5.1/modulefiles/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-08 13:35:14.000000 echolocator-1.5.1/modulefiles/conda
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-08 13:35:14.000000 echolocator-1.5.1/modulefiles/paths
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-08 13:35:14.000000 echolocator-1.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 13:35:25.994854 echolocator-1.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.950853 echolocator-1.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.978853 echolocator-1.5.1/src/echolocator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-06-08 13:35:25.000000 echolocator-1.5.1/src/echolocator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-06-08 13:35:25.000000 echolocator-1.5.1/src/echolocator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:35:25.000000 echolocator-1.5.1/src/echolocator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-08 13:35:25.000000 echolocator-1.5.1/src/echolocator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-08 13:35:25.000000 echolocator-1.5.1/src/echolocator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-08 13:35:25.000000 echolocator-1.5.1/src/echolocator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.978853 echolocator-1.5.1/src/echolocator_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_api/aiohttp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.978853 echolocator-1.5.1/src/echolocator_api/databases/
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_api/databases/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.982854 echolocator-1.5.1/src/echolocator_api/guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_api/guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_api/guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_api/guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_api/guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_api/guis/guis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.982854 echolocator-1.5.1/src/echolocator_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.982854 echolocator-1.5.1/src/echolocator_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.986853 echolocator-1.5.1/src/echolocator_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 13:35:25.000000 echolocator-1.5.1/src/echolocator_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.986853 echolocator-1.5.1/src/echolocator_lib/composers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/composers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/composers/composers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/composers/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/composers/prettyhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/composers/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/envvar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.986853 echolocator-1.5.1/src/echolocator_lib/guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28857 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/guis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.986853 echolocator-1.5.1/src/echolocator_lib/guis/html/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.986853 echolocator-1.5.1/src/echolocator_lib/guis/html/css/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/css/image_edit_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/css/image_list_ux.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.986853 echolocator-1.5.1/src/echolocator_lib/guis/html/css/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/css/pixel_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/css/plate_list_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/css/styles.css
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/css/system_health_ux.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.986853 echolocator-1.5.1/src/echolocator_lib/guis/html/images/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/images/green_dot_crosshair.png
--rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/images/radial1.666.png
--rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.986853 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.986853 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/common/base.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.990854 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/echolocator/
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/echolocator/centroid_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/echolocator/events.js
--rw-r--r--   0 runner    (1001) docker     (123)    22820 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/echolocator/page.js
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/echolocator/plate_list_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.954853 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.990854 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.954853 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.990854 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/
--rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   255077 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.954853 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.990854 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.990854 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.954853 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/raphael/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.990854 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/runtime.js
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/version.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.990854 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/webviz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.994854 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/webviz/hair/
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/webviz/spreader.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.994854 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/webviz/sprite/
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/webviz/sprite/ring.js
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/webviz/transformer.js
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-08 13:35:14.000000 echolocator-1.5.1/src/echolocator_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.994854 echolocator-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:14.000000 echolocator-1.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-06-08 13:35:14.000000 echolocator-1.5.1/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.994854 echolocator-1.5.1/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-08 13:35:14.000000 echolocator-1.5.1/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    27821 2023-06-08 13:35:14.000000 echolocator-1.5.1/tests/configurations/store.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-08 13:35:14.000000 echolocator-1.5.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.994854 echolocator-1.5.1/tests/example_images/
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-08 13:35:14.000000 echolocator-1.5.1/tests/example_images/1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-06-08 13:35:14.000000 echolocator-1.5.1/tests/example_images/2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-06-08 13:35:14.000000 echolocator-1.5.1/tests/example_images/3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-06-08 13:35:14.000000 echolocator-1.5.1/tests/example_images/4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:35:25.994854 echolocator-1.5.1/tests/images/
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-08 13:35:14.000000 echolocator-1.5.1/tests/images/1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-06-08 13:35:14.000000 echolocator-1.5.1/tests/images/2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-06-08 13:35:14.000000 echolocator-1.5.1/tests/images/3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-06-08 13:35:14.000000 echolocator-1.5.1/tests/test_droplocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-06-08 13:35:14.000000 echolocator-1.5.1/tests/test_export_to_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-06-08 13:35:14.000000 echolocator-1.5.1/tests/test_export_to_soakdb3.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-06-08 13:35:14.000000 echolocator-1.5.1/tests/test_fetch_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-06-08 13:35:14.000000 echolocator-1.5.1/tests/test_fetch_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-08 13:35:14.000000 echolocator-1.5.1/tests/test_report_plates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.213967 echolocator-1.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.185967 echolocator-1.6.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-16 11:31:37.000000 echolocator-1.6.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.185967 echolocator-1.6.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-16 11:31:37.000000 echolocator-1.6.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-16 11:31:37.000000 echolocator-1.6.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-16 11:31:37.000000 echolocator-1.6.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-16 11:31:37.000000 echolocator-1.6.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-16 11:31:37.000000 echolocator-1.6.0/.dae-devops/docs/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-16 11:31:37.000000 echolocator-1.6.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-16 11:31:37.000000 echolocator-1.6.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-16 11:31:37.000000 echolocator-1.6.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-16 11:31:37.000000 echolocator-1.6.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.185967 echolocator-1.6.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-16 11:31:37.000000 echolocator-1.6.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-16 11:31:37.000000 echolocator-1.6.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.185967 echolocator-1.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-16 11:31:37.000000 echolocator-1.6.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.181967 echolocator-1.6.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.185967 echolocator-1.6.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-16 11:31:37.000000 echolocator-1.6.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-16 11:31:37.000000 echolocator-1.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.185967 echolocator-1.6.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-16 11:31:37.000000 echolocator-1.6.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-16 11:31:37.000000 echolocator-1.6.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.185967 echolocator-1.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-06-16 11:31:37.000000 echolocator-1.6.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-16 11:31:37.000000 echolocator-1.6.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-16 11:31:37.000000 echolocator-1.6.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-16 11:31:37.000000 echolocator-1.6.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-16 11:31:37.000000 echolocator-1.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-16 11:31:37.000000 echolocator-1.6.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-16 11:31:37.000000 echolocator-1.6.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.185967 echolocator-1.6.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-16 11:31:37.000000 echolocator-1.6.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-16 11:31:37.000000 echolocator-1.6.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-16 11:31:37.000000 echolocator-1.6.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-16 11:31:37.000000 echolocator-1.6.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-16 11:31:37.000000 echolocator-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-06-16 11:31:37.000000 echolocator-1.6.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-06-16 11:31:46.213967 echolocator-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-16 11:31:37.000000 echolocator-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.185967 echolocator-1.6.0/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-16 11:31:37.000000 echolocator-1.6.0/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.185967 echolocator-1.6.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.181967 echolocator-1.6.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.185967 echolocator-1.6.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-16 11:31:37.000000 echolocator-1.6.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-06-16 11:31:37.000000 echolocator-1.6.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.185967 echolocator-1.6.0/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-16 11:31:37.000000 echolocator-1.6.0/docs/explanations/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-16 11:31:37.000000 echolocator-1.6.0/docs/explanations/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-16 11:31:37.000000 echolocator-1.6.0/docs/explanations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-16 11:31:37.000000 echolocator-1.6.0/docs/explanations/todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.189967 echolocator-1.6.0/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-16 11:31:37.000000 echolocator-1.6.0/docs/how-to/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-16 11:31:37.000000 echolocator-1.6.0/docs/how-to/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-16 11:31:37.000000 echolocator-1.6.0/docs/how-to/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-16 11:31:37.000000 echolocator-1.6.0/docs/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-16 11:31:37.000000 echolocator-1.6.0/docs/how-to/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-16 11:31:37.000000 echolocator-1.6.0/docs/how-to/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.189967 echolocator-1.6.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-16 11:31:37.000000 echolocator-1.6.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-16 11:31:37.000000 echolocator-1.6.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-16 11:31:37.000000 echolocator-1.6.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.189967 echolocator-1.6.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-16 11:31:37.000000 echolocator-1.6.0/docs/reference/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-16 11:31:37.000000 echolocator-1.6.0/docs/reference/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-16 11:31:37.000000 echolocator-1.6.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-16 11:31:37.000000 echolocator-1.6.0/docs/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.189967 echolocator-1.6.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-16 11:31:37.000000 echolocator-1.6.0/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-16 11:31:37.000000 echolocator-1.6.0/docs/tutorials/tbd.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.189967 echolocator-1.6.0/modulefiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-16 11:31:37.000000 echolocator-1.6.0/modulefiles/conda
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-16 11:31:37.000000 echolocator-1.6.0/modulefiles/paths
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-16 11:31:37.000000 echolocator-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 11:31:46.213967 echolocator-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.181967 echolocator-1.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.193967 echolocator-1.6.0/src/echolocator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-06-16 11:31:46.000000 echolocator-1.6.0/src/echolocator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-06-16 11:31:46.000000 echolocator-1.6.0/src/echolocator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:31:46.000000 echolocator-1.6.0/src/echolocator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-16 11:31:46.000000 echolocator-1.6.0/src/echolocator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-16 11:31:46.000000 echolocator-1.6.0/src/echolocator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 11:31:46.000000 echolocator-1.6.0/src/echolocator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.193967 echolocator-1.6.0/src/echolocator_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_api/aiohttp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.193967 echolocator-1.6.0/src/echolocator_api/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_api/databases/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.193967 echolocator-1.6.0/src/echolocator_api/guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_api/guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_api/guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_api/guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_api/guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_api/guis/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.193967 echolocator-1.6.0/src/echolocator_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.193967 echolocator-1.6.0/src/echolocator_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.197967 echolocator-1.6.0/src/echolocator_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-16 11:31:46.000000 echolocator-1.6.0/src/echolocator_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.197967 echolocator-1.6.0/src/echolocator_lib/composers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/composers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/composers/composers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/composers/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/composers/prettyhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/composers/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/envvar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.197967 echolocator-1.6.0/src/echolocator_lib/guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29334 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.197967 echolocator-1.6.0/src/echolocator_lib/guis/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.201967 echolocator-1.6.0/src/echolocator_lib/guis/html/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/css/image_edit_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/css/image_list_ux.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.201967 echolocator-1.6.0/src/echolocator_lib/guis/html/css/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/css/pixel_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/css/plate_list_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/css/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/css/system_health_ux.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.201967 echolocator-1.6.0/src/echolocator_lib/guis/html/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/images/green_dot_crosshair.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/images/radial1.666.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.201967 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.201967 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/common/base.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.201967 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/echolocator/
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/echolocator/centroid_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/echolocator/events.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22820 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/echolocator/page.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/echolocator/plate_list_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.181967 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.205967 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.181967 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.205967 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   255077 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.181967 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.205967 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.205967 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.181967 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/raphael/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.205967 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/runtime.js
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/version.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.209967 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/webviz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.209967 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/webviz/hair/
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/webviz/spreader.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.209967 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/webviz/sprite/
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/webviz/sprite/ring.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/webviz/transformer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-16 11:31:37.000000 echolocator-1.6.0/src/echolocator_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.209967 echolocator-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:37.000000 echolocator-1.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-06-16 11:31:37.000000 echolocator-1.6.0/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.209967 echolocator-1.6.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-16 11:31:37.000000 echolocator-1.6.0/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    27821 2023-06-16 11:31:37.000000 echolocator-1.6.0/tests/configurations/store.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-16 11:31:37.000000 echolocator-1.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.209967 echolocator-1.6.0/tests/example_images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-16 11:31:37.000000 echolocator-1.6.0/tests/example_images/1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-06-16 11:31:37.000000 echolocator-1.6.0/tests/example_images/2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-06-16 11:31:37.000000 echolocator-1.6.0/tests/example_images/3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-06-16 11:31:37.000000 echolocator-1.6.0/tests/example_images/4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:46.213967 echolocator-1.6.0/tests/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-16 11:31:37.000000 echolocator-1.6.0/tests/images/1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-06-16 11:31:37.000000 echolocator-1.6.0/tests/images/2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-06-16 11:31:37.000000 echolocator-1.6.0/tests/images/3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-06-16 11:31:37.000000 echolocator-1.6.0/tests/test_droplocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-06-16 11:31:37.000000 echolocator-1.6.0/tests/test_export_to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-06-16 11:31:37.000000 echolocator-1.6.0/tests/test_export_to_soakdb3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-06-16 11:31:37.000000 echolocator-1.6.0/tests/test_fetch_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-06-16 11:31:37.000000 echolocator-1.6.0/tests/test_fetch_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-16 11:31:37.000000 echolocator-1.6.0/tests/test_report_plates.py
```

### Comparing `echolocator-1.5.1/.dae-devops/Makefile` & `echolocator-1.6.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/.dae-devops/docs/conventions.rst` & `echolocator-1.6.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/.dae-devops/docs/developing.rst` & `echolocator-1.6.0/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/.dae-devops/docs/devops.rst` & `echolocator-1.6.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/.dae-devops/docs/docs_structure.rst` & `echolocator-1.6.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/.dae-devops/docs/documenting.rst` & `echolocator-1.6.0/.dae-devops/docs/documenting.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/.dae-devops/docs/installing.rst` & `echolocator-1.6.0/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/.dae-devops/docs/testing.rst` & `echolocator-1.6.0/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/.dae-devops/project.yaml` & `echolocator-1.6.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/.devcontainer/Dockerfile` & `echolocator-1.6.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/.devcontainer/devcontainer.json` & `echolocator-1.6.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/.github/CONTRIBUTING.rst` & `echolocator-1.6.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/.github/actions/install_requirements/action.yml` & `echolocator-1.6.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/.github/dependabot.yml` & `echolocator-1.6.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/.github/pages/make_switcher.py` & `echolocator-1.6.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/.github/workflows/code.yml` & `echolocator-1.6.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/.github/workflows/docs.yml` & `echolocator-1.6.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/.github/workflows/docs_clean.yml` & `echolocator-1.6.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/.github/workflows/linkcheck.yml` & `echolocator-1.6.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/.gitignore` & `echolocator-1.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/.gitlab-ci.yml` & `echolocator-1.6.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/.vscode/launch.json` & `echolocator-1.6.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/LICENSE` & `echolocator-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/Makefile` & `echolocator-1.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/PKG-INFO` & `echolocator-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echolocator
-Version: 1.5.1
+Version: 1.6.0
 Summary: XChem GUI for manually targeting drop points for the Echo dispenser.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `echolocator-1.5.1/configurations/development.yaml` & `echolocator-1.6.0/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/docs/conf.py` & `echolocator-1.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/docs/images/dls-favicon.ico` & `echolocator-1.6.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/docs/images/dls-logo.svg` & `echolocator-1.6.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/modulefiles/conda` & `echolocator-1.6.0/modulefiles/conda`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/pyproject.toml` & `echolocator-1.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator.egg-info/PKG-INFO` & `echolocator-1.6.0/src/echolocator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echolocator
-Version: 1.5.1
+Version: 1.6.0
 Summary: XChem GUI for manually targeting drop points for the Echo dispenser.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `echolocator-1.5.1/src/echolocator.egg-info/SOURCES.txt` & `echolocator-1.6.0/src/echolocator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_api/databases/constants.py` & `echolocator-1.6.0/src/echolocator_api/databases/constants.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_api/exceptions.py` & `echolocator-1.6.0/src/echolocator_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_api/guis/aiohttp.py` & `echolocator-1.6.0/src/echolocator_api/guis/aiohttp.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_api/guis/context.py` & `echolocator-1.6.0/src/echolocator_api/guis/context.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_api/guis/guis.py` & `echolocator-1.6.0/src/echolocator_api/guis/guis.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_cli/main.py` & `echolocator-1.6.0/src/echolocator_cli/main.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_cli/subcommands/base.py` & `echolocator-1.6.0/src/echolocator_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_cli/subcommands/service.py` & `echolocator-1.6.0/src/echolocator_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_cli/version.py` & `echolocator-1.6.0/src/echolocator_cli/version.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/__main__.py` & `echolocator-1.6.0/src/echolocator_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/composers/composers.py` & `echolocator-1.6.0/src/echolocator_lib/composers/composers.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/composers/html.py` & `echolocator-1.6.0/src/echolocator_lib/composers/html.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/composers/prettyhelper.py` & `echolocator-1.6.0/src/echolocator_lib/composers/prettyhelper.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/composers/text.py` & `echolocator-1.6.0/src/echolocator_lib/composers/text.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/envvar.py` & `echolocator-1.6.0/src/echolocator_lib/envvar.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/aiohttp.py` & `echolocator-1.6.0/src/echolocator_lib/guis/aiohttp.py`

 * *Files 4% similar despite different names*

```diff
@@ -567,18 +567,24 @@
         # Fetch the list of wells according to the filter.
         crystal_well_models: List[
             CrystalWellNeedingDroplocationModel
         ] = await self.__xchembku.fetch_crystal_wells_needing_droplocation(
             crystal_well_filter, why="[EXPFIL] get list to be epxorted"
         )
 
+        # Sort the list based on the (computed) row_first_position field.
+        sorted_models = sorted(
+            crystal_well_models,
+            key=lambda crystal_well_model: crystal_well_model.row_first_position(),
+        )
+
         logger.debug(f"[EXPFIL] found {len(crystal_well_models)} to be exported")
 
         # Export the crystal wells to the appropriate soakdb3 visit.
-        await self.__export_to_soakdb3_visit(visit_filter, crystal_well_models)
+        await self.__export_to_soakdb3_visit(visit_filter, sorted_models)
 
         # Make the list of droplocations to update with the exported flag.
         crystal_well_droplocation_models: List[CrystalWellDroplocationModel] = list()
         for crystal_well_model in crystal_well_models:
             # We only need the crystal_well_uuid for upserting.
             # This will have to be revisited if we ever want multiple droplocations on a single well.
             crystal_well_droplocation_model = CrystalWellDroplocationModel(
@@ -688,17 +694,24 @@
         confirmations = []
 
         # Go through each plate separately.
         for (
             crystal_plate_uuid,
             plate_crystal_well_models,
         ) in plates_crystal_well_models.items():
+
+            # Sort the list based on the (computed) row_first_position field.
+            sorted_models = sorted(
+                plate_crystal_well_models,
+                key=lambda crystal_well_model: crystal_well_model.row_first_position(),
+            )
+
             # Export the crystal wells for this plate to the appropriate csv file named for the plate.
             filename = await self.__export_to_csv_plate(
-                visit_filter, crystal_plate_uuid, plate_crystal_well_models
+                visit_filter, crystal_plate_uuid, sorted_models
             )
 
             confirmations.append(
                 f"exported {len(plate_crystal_well_models)} rows to {filename}"
             )
 
         response = {"confirmation": "\n".join(confirmations)}
```

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/constants.py` & `echolocator-1.6.0/src/echolocator_lib/guis/constants.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/context.py` & `echolocator-1.6.0/src/echolocator_lib/guis/context.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/guis.py` & `echolocator-1.6.0/src/echolocator_lib/guis/guis.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/css/image_list_ux.css` & `echolocator-1.6.0/src/echolocator_lib/guis/html/css/image_list_ux.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png` & `echolocator-1.6.0/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/css/plate_list_ux.css` & `echolocator-1.6.0/src/echolocator_lib/guis/html/css/plate_list_ux.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/css/styles.css` & `echolocator-1.6.0/src/echolocator_lib/guis/html/css/styles.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/images/green_dot_crosshair.png` & `echolocator-1.6.0/src/echolocator_lib/guis/html/images/green_dot_crosshair.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/images/radial1.666.png` & `echolocator-1.6.0/src/echolocator_lib/guis/html/images/radial1.666.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/index.html` & `echolocator-1.6.0/src/echolocator_lib/guis/html/index.html`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/index.js` & `echolocator-1.6.0/src/echolocator_lib/guis/html/index.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/common/base.js` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/common/base.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/echolocator/centroid_ux.js` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/echolocator/centroid_ux.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/echolocator/plate_list_ux.js` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/echolocator/plate_list_ux.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/webviz/spreader.js` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/webviz/spreader.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/webviz/sprite/ring.js` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/webviz/sprite/ring.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/guis/html/javascript/webviz/transformer.js` & `echolocator-1.6.0/src/echolocator_lib/guis/html/javascript/webviz/transformer.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/src/echolocator_lib/version.py` & `echolocator-1.6.0/src/echolocator_lib/version.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/tests/base.py` & `echolocator-1.6.0/tests/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     This is a base class for tests which use Context.
     """
 
     def __init__(self):
         self.tasks_execution_outputs = {}
         self.residuals = ["stdout.txt", "stderr.txt", "main.log"]
 
-        self.injected_count = 0
+        self.__injected_count = 0
         self.visit = "cm00001-1"
         self.__barcode_template = "98a%d"
         self.crystal_plate_uuid = None
         self.__rockminer_collected_stem_template = "98a%d_2021-09-14_RI1000-0276-3drop"
 
         self.crystal_plate_models = []
 
@@ -127,45 +127,65 @@
 
     async def inject(self, xchembku, autolocation: bool, droplocation: bool):
         """ """
 
         if self.crystal_plate_uuid is None:
             await self.inject_plate(xchembku)
 
-        self.injected_count += 1
-
-        filename = "/tmp/%03d.jpg" % (self.injected_count)
+        letter = "A"
+        if self.__injected_count > 3:
+            letter = "B"
+
+        self.__injected_count += 1
+        filename = "/tmp/%02d%s_1.jpg" % (self.__injected_count, letter)
+        position = "%s%02da" % (letter, self.__injected_count)
+
+        positions = [
+            "A01a",
+            "A02a",
+            "A03a",
+            "B01a",
+            "B02a",
+            "B02a",
+            "C01a",
+            "C02a",
+            "C03a",
+            "D01a",
+            "D02a",
+            "D03a",
+        ]
+        position = positions[self.__injected_count - 1]
 
         # Write well record.
         m = CrystalWellModel(
-            position="%02dA_1" % (self.injected_count),
+            position=position,
             filename=filename,
             crystal_plate_uuid=self.crystal_plate_uuid,
         )
 
         await xchembku.upsert_crystal_wells([m])
 
         if autolocation:
             # Add a crystal well autolocation.
             t = CrystalWellAutolocationModel(
                 crystal_well_uuid=m.uuid,
-                number_of_crystals=self.injected_count,
+                number_of_crystals=self.__injected_count,
                 well_centroid_x=400,
                 well_centroid_y=500,
-                auto_target_x=self.injected_count * 10 + 0,
-                auto_target_y=self.injected_count * 10 + 1,
+                auto_target_x=self.__injected_count * 10 + 0,
+                auto_target_y=self.__injected_count * 10 + 1,
             )
 
             await xchembku.originate_crystal_well_autolocations([t])
 
         if droplocation:
             # Add a crystal well droplocation.
             t = CrystalWellDroplocationModel(
                 crystal_well_uuid=m.uuid,
-                confirmed_target_x=self.injected_count * 100 + 2,
-                confirmed_target_y=self.injected_count * 100 + 3,
+                confirmed_target_x=self.__injected_count * 100 + 2,
+                confirmed_target_y=self.__injected_count * 100 + 3,
                 is_usable=True,
             )
 
             await xchembku.upsert_crystal_well_droplocations([t])
 
         return m
```

### Comparing `echolocator-1.5.1/tests/configurations/service.yaml` & `echolocator-1.6.0/tests/configurations/service.yaml`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/tests/configurations/store.csv` & `echolocator-1.6.0/tests/configurations/store.csv`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/tests/conftest.py` & `echolocator-1.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/tests/example_images/1.jpg` & `echolocator-1.6.0/tests/example_images/1.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/tests/example_images/2.jpg` & `echolocator-1.6.0/tests/example_images/2.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/tests/example_images/3.jpg` & `echolocator-1.6.0/tests/example_images/3.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/tests/example_images/4.png` & `echolocator-1.6.0/tests/example_images/4.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/tests/images/1.jpg` & `echolocator-1.6.0/tests/images/1.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/tests/images/2.jpg` & `echolocator-1.6.0/tests/images/2.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/tests/images/3.jpg` & `echolocator-1.6.0/tests/images/3.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/tests/test_droplocation.py` & `echolocator-1.6.0/tests/test_droplocation.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/tests/test_export_to_csv.py` & `echolocator-1.6.0/tests/test_export_to_csv.py`

 * *Files 5% similar despite different names*

```diff
@@ -191,21 +191,24 @@
 
         # Check each row has 3 parts.
         for row in rows:
             assert len(row) == 3
 
         # Check the well positions are those that are considered "confirmed".
         # The position constants are fromt the Swiss3 microns computation.
-        assert rows[0][0] == "02A_1"
-        assert int(rows[0][1]) == -561
-        assert int(rows[0][2]) == -842
-        assert rows[1][0] == "04A_1"
-        assert int(rows[1][1]) == 6
-        assert int(rows[1][2]) == -274
-        assert rows[2][0] == "05A_1"
+        # Note the order here: row_first_position gives get all letters in row 01 before any letters in row 02.
+        assert rows[0][0] == "B01a"
+        assert int(rows[0][1]) == 6
+        assert int(rows[0][2]) == -274
+
+        assert rows[1][0] == "A02a"
+        assert int(rows[1][1]) == -561
+        assert int(rows[1][2]) == -842
+
+        assert rows[2][0] == "B02a"
         assert int(rows[2][1]) == 289
         assert int(rows[2][2]) == 9
 
         # ----------------------------------------------------------------------
         # Check the second csv file got written.
         csv_path = (
             self.__crystal_targets_directory
```

### Comparing `echolocator-1.5.1/tests/test_export_to_soakdb3.py` & `echolocator-1.6.0/tests/test_export_to_soakdb3.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,21 +207,24 @@
         # Check the results stored in soakdbb3, there should be no change to the first ones.
         queried_models = await self.__xchembku.fetch_soakdb3_crystal_wells(
             str(self.__visit_directory / "processing")
         )
         assert len(queried_models) == 3
 
         # The position constants are fromt the Swiss3 microns computation.
-        assert queried_models[0].CrystalWell == "02A_1"
-        assert int(queried_models[0].EchoX) == -561
-        assert int(queried_models[0].EchoY) == -842
-        assert queried_models[1].CrystalWell == "04A_1"
-        assert int(queried_models[1].EchoX) == 6
-        assert int(queried_models[1].EchoY) == -274
-        assert queried_models[2].CrystalWell == "05A_1"
+        # Note the order here: row_first_position gives get all letters in row 01 before any letters in row 02.
+        assert queried_models[0].CrystalWell == "B01a"
+        assert int(queried_models[0].EchoX) == 6
+        assert int(queried_models[0].EchoY) == -274
+
+        assert queried_models[1].CrystalWell == "A02a"
+        assert int(queried_models[1].EchoX) == -561
+        assert int(queried_models[1].EchoY) == -842
+
+        assert queried_models[2].CrystalWell == "B02a"
         assert int(queried_models[2].EchoX) == 289
         assert int(queried_models[2].EchoY) == 9
 
         # Check the results stored in xchembku, the exported flag should be set.
         crystal_well_models = (
             await self.__xchembku.fetch_crystal_wells_needing_droplocation(
                 CrystalWellFilterModel(is_exported_to_soakdb3=True)
```

### Comparing `echolocator-1.5.1/tests/test_fetch_image.py` & `echolocator-1.6.0/tests/test_fetch_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,33 +201,33 @@
         logger.debug("[AT] ----------------- requesting anchor -----------------")
         request = {
             ProtocoljKeywords.ENABLE_COOKIES: [
                 Cookies.IMAGE_EDIT_UX,
                 Cookies.IMAGE_LIST_UX,
             ],
             Keywords.COMMAND: Commands.FETCH_IMAGE,
-            Keywords.CRYSTAL_WELL_INDEX: 2,  # 04A_1
+            Keywords.CRYSTAL_WELL_INDEX: 2,  # B01a
         }
 
         response = await echolocator_guis_get_default().client_protocolj(
             request,
             cookies=self.__cookies,
         )
 
         # Keep now we have both cookies.
         self.__cookies = response["__cookies"]
 
         record = response["record"]
         assert record is not None
-        assert record["position"] == "04A_1"
+        assert record["position"] == "B01a"
 
         # -------------------------------------------------------------------------------------
         # Same query again, but rely on cookie for index.
         request.pop(Keywords.CRYSTAL_WELL_INDEX)
 
         response = await echolocator_guis_get_default().client_protocolj(
             request,
             cookies=self.__cookies,
         )
 
         record = response["record"]
-        assert record["position"] == "04A_1"
+        assert record["position"] == "B01a"
```

### Comparing `echolocator-1.5.1/tests/test_fetch_images.py` & `echolocator-1.6.0/tests/test_fetch_images.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.5.1/tests/test_report_plates.py` & `echolocator-1.6.0/tests/test_report_plates.py`

 * *Files identical despite different names*

