# Comparing `tmp/oenv2config-1.0.1.tar.gz` & `tmp/oenv2config-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oenv2config-1.0.1.tar", last modified: Fri Jun  2 14:33:14 2023, max compression
+gzip compressed data, was "oenv2config-1.1.0.tar", last modified: Fri Jun 16 14:20:12 2023, max compression
```

## Comparing `oenv2config-1.0.1.tar` & `oenv2config-1.1.0.tar`

### file list

```diff
@@ -1,119 +1,121 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.118942 oenv2config-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     1885 2023-05-05 10:29:38.000000 oenv2config-1.0.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-05-06 10:18:20.000000 oenv2config-1.0.1/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.098942 oenv2config-1.0.1/.idea/
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-05-02 08:56:52.000000 oenv2config-1.0.1/.idea/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      201 2023-05-02 08:56:52.000000 oenv2config-1.0.1/.idea/misc.xml
--rw-rw-rw-   0 root         (0) root         (0)      275 2023-05-02 08:56:52.000000 oenv2config-1.0.1/.idea/modules.xml
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-05-02 08:56:52.000000 oenv2config-1.0.1/.idea/oenv2config.iml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.098942 oenv2config-1.0.1/.idea/runConfigurations/
--rw-rw-rw-   0 root         (0) root         (0)     1458 2023-05-05 10:29:38.000000 oenv2config-1.0.1/.idea/runConfigurations/Python_tests__no_Odoo_.xml
--rw-rw-rw-   0 root         (0) root         (0)     1565 2023-05-05 10:29:38.000000 oenv2config-1.0.1/.idea/runConfigurations/Python_tests_in_tests_odoo.xml
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-05-02 08:56:52.000000 oenv2config-1.0.1/.idea/vcs.xml
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-05-02 08:56:52.000000 oenv2config-1.0.1/.local-antora-playbook.yml
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-05 10:29:38.000000 oenv2config-1.0.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 10:31:13.000000 oenv2config-1.0.1/.ruff
--rw-r--r--   0 root         (0) root         (0)      182 2023-06-02 14:33:14.114942 oenv2config-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      857 2023-05-02 08:56:52.000000 oenv2config-1.0.1/README.adoc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.098942 oenv2config-1.0.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/antora.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.098942 oenv2config-1.0.1/docs/mkdocs/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/mkdocs/cli.md
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/mkdocs/db_options.md
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/mkdocs/entry.md
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/mkdocs/index.md
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/mkdocs/mappers.md
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/mkdocs/options.md
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/mkdocs/reference.md
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/mkdocs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/mkdocs/utils.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.090942 oenv2config-1.0.1/docs/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.098942 oenv2config-1.0.1/docs/modules/ROOT/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.102942 oenv2config-1.0.1/docs/modules/ROOT/images/
--rw-rw-rw-   0 root         (0) root         (0)    44111 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/modules/ROOT/images/run_odoo_test.png
--rw-rw-rw-   0 root         (0) root         (0)    35877 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/modules/ROOT/images/run_test.png
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/modules/ROOT/nav.adoc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.102942 oenv2config-1.0.1/docs/modules/ROOT/pages/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/modules/ROOT/pages/antora.adoc
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/modules/ROOT/pages/contribute.adoc
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/modules/ROOT/pages/index.adoc
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/modules/ROOT/pages/mkdocs.adoc
--rw-rw-rw-   0 root         (0) root         (0)      754 2023-06-02 13:54:32.000000 oenv2config-1.0.1/docs/modules/ROOT/pages/tests.adoc
--rw-rw-rw-   0 root         (0) root         (0)     1872 2023-06-02 13:54:32.000000 oenv2config-1.0.1/docs/modules/ROOT/pages/tests_odoo.adoc
--rwxrwxrwx   0 root         (0) root         (0)      320 2023-05-05 10:29:38.000000 oenv2config-1.0.1/in_docker_test.sh
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-05-02 08:56:52.000000 oenv2config-1.0.1/mkdocs-plugins.txt
--rw-rw-rw-   0 root         (0) root         (0)     1032 2023-05-02 08:56:52.000000 oenv2config-1.0.1/mkdocs.yml
--rw-rw-rw-   0 root         (0) root         (0)      753 2023-05-05 10:29:38.000000 oenv2config-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 14:33:14.118942 oenv2config-1.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      399 2023-05-02 08:56:52.000000 oenv2config-1.0.1/setup.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.090942 oenv2config-1.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.102942 oenv2config-1.0.1/src/odoo_env_config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.0.1/src/odoo_env_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-06-02 14:33:13.000000 oenv2config-1.0.1/src/odoo_env_config/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     4690 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/api.py
--rw-rw-rw-   0 root         (0) root         (0)     4121 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/entry.py
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-05-02 08:56:52.000000 oenv2config-1.0.1/src/odoo_env_config/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4475 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/mappers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.090942 oenv2config-1.0.1/src/odoo_env_config/odoo_modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.106942 oenv2config-1.0.1/src/odoo_env_config/odoo_modules/env2config/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-05 10:31:13.000000 oenv2config-1.0.1/src/odoo_env_config/odoo_modules/env2config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-05-02 08:56:52.000000 oenv2config-1.0.1/src/odoo_env_config/odoo_modules/env2config/__manifest__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.106942 oenv2config-1.0.1/src/odoo_env_config/odoo_modules/env2config/cli/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-02 08:56:52.000000 oenv2config-1.0.1/src/odoo_env_config/odoo_modules/env2config/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.106942 oenv2config-1.0.1/src/odoo_env_config/section/
--rw-rw-rw-   0 root         (0) root         (0)      802 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/section/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      659 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/section/addons_path_section.py
--rw-rw-rw-   0 root         (0) root         (0)     4172 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/section/db_section.py
--rw-rw-rw-   0 root         (0) root         (0)      961 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/section/http_section.py
--rw-rw-rw-   0 root         (0) root         (0)     2151 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/section/limit_section.py
--rw-rw-rw-   0 root         (0) root         (0)     1512 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/section/log_section.py
--rw-rw-rw-   0 root         (0) root         (0)      972 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/section/misc_section.py
--rw-rw-rw-   0 root         (0) root         (0)      861 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/section/test_section.py
--rw-rw-rw-   0 root         (0) root         (0)      611 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/section/update_init_section.py
--rw-rw-rw-   0 root         (0) root         (0)     1030 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/section/widemodule_section.py
--rw-rw-rw-   0 root         (0) root         (0)     2322 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/section/worker_section.py
--rw-rw-rw-   0 root         (0) root         (0)    10125 2023-05-02 08:56:52.000000 oenv2config-1.0.1/src/odoo_env_config/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.110942 oenv2config-1.0.1/src/oenv2config.egg-info/
--rw-r--r--   0 root         (0) root         (0)      182 2023-06-02 14:33:14.000000 oenv2config-1.0.1/src/oenv2config.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3205 2023-06-02 14:33:14.000000 oenv2config-1.0.1/src/oenv2config.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 14:33:14.000000 oenv2config-1.0.1/src/oenv2config.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2023-06-02 14:33:14.000000 oenv2config-1.0.1/src/oenv2config.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       72 2023-06-02 14:33:14.000000 oenv2config-1.0.1/src/oenv2config.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-02 14:33:14.000000 oenv2config-1.0.1/src/oenv2config.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.110942 oenv2config-1.0.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2148 2023-05-05 10:29:38.000000 oenv2config-1.0.1/tests/_decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     3154 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_doctests.py
--rw-rw-rw-   0 root         (0) root         (0)     1942 2023-06-02 13:54:32.000000 oenv2config-1.0.1/tests/test_entry.py
--rw-rw-rw-   0 root         (0) root         (0)      740 2023-06-02 13:54:32.000000 oenv2config-1.0.1/tests/test_libs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.110942 oenv2config-1.0.1/tests/test_mapper/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_mapper/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7703 2023-06-02 13:54:32.000000 oenv2config-1.0.1/tests/test_mapper/test_mapper_clever_cloud_cellar.py
--rw-rw-rw-   0 root         (0) root         (0)    10835 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_mapper/test_mapper_clever_cloud_postgres.py
--rw-rw-rw-   0 root         (0) root         (0)     6535 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_mapper/test_mapper_odoo_compatibility.py
--rw-rw-rw-   0 root         (0) root         (0)     5002 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_mapper/test_mapper_queue_job.py
--rw-rw-rw-   0 root         (0) root         (0)     3921 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_mapper/test_mapper_redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.114942 oenv2config-1.0.1/tests/test_section/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_section/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1366 2023-05-05 10:29:38.000000 oenv2config-1.0.1/tests/test_section/test_addons_path_section.py
--rw-rw-rw-   0 root         (0) root         (0)     7581 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_section/test_db_section.py
--rw-rw-rw-   0 root         (0) root         (0)     2339 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_section/test_http_section.py
--rw-rw-rw-   0 root         (0) root         (0)     5567 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_section/test_limit_section.py
--rw-rw-rw-   0 root         (0) root         (0)     2489 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_section/test_log_section.py
--rw-rw-rw-   0 root         (0) root         (0)     1389 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_section/test_misc_section.py
--rw-rw-rw-   0 root         (0) root         (0)     1989 2023-05-05 10:29:38.000000 oenv2config-1.0.1/tests/test_section/test_test_section.py
--rw-rw-rw-   0 root         (0) root         (0)     1259 2023-05-05 10:29:38.000000 oenv2config-1.0.1/tests/test_section/test_update_init_section.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_section/test_widemodule_section.py
--rw-rw-rw-   0 root         (0) root         (0)     6727 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_section/test_worker_section.py
--rw-rw-rw-   0 root         (0) root         (0)     2436 2023-06-02 13:54:32.000000 oenv2config-1.0.1/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.114942 oenv2config-1.0.1/tests/tests_odoo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/tests_odoo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4906 2023-05-05 10:29:38.000000 oenv2config-1.0.1/tests/tests_odoo/_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.114942 oenv2config-1.0.1/tests/tests_odoo/profiles/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/tests_odoo/profiles/filestore_s3.env
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/tests_odoo/profiles/filestore_s3_cellar.env
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/tests_odoo/profiles/test_db_clever.env
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/tests_odoo/profiles/test_db_clever_direct.env
--rw-rw-rw-   0 root         (0) root         (0)     4115 2023-05-05 10:29:38.000000 oenv2config-1.0.1/tests/tests_odoo/test_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.556730 oenv2config-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1885 2023-05-05 10:29:38.000000 oenv2config-1.1.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2023-06-14 10:38:37.000000 oenv2config-1.1.0/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.456730 oenv2config-1.1.0/.idea/
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-05-02 08:56:52.000000 oenv2config-1.1.0/.idea/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      201 2023-05-02 08:56:52.000000 oenv2config-1.1.0/.idea/misc.xml
+-rw-rw-rw-   0 root         (0) root         (0)      275 2023-06-14 09:09:25.000000 oenv2config-1.1.0/.idea/modules.xml
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-05-02 08:56:52.000000 oenv2config-1.1.0/.idea/oenv2config.iml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.460730 oenv2config-1.1.0/.idea/runConfigurations/
+-rw-rw-rw-   0 root         (0) root         (0)     1712 2023-06-14 09:09:25.000000 oenv2config-1.1.0/.idea/runConfigurations/Python_tests__no_Odoo_.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2023-05-05 10:29:38.000000 oenv2config-1.1.0/.idea/runConfigurations/Python_tests_in_tests_odoo.xml
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-05-02 08:56:52.000000 oenv2config-1.1.0/.idea/vcs.xml
+-rw-rw-rw-   0 root         (0) root         (0)      426 2023-05-02 08:56:52.000000 oenv2config-1.1.0/.local-antora-playbook.yml
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-05 10:29:38.000000 oenv2config-1.1.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 10:31:13.000000 oenv2config-1.1.0/.ruff
+-rw-r--r--   0 root         (0) root         (0)      182 2023-06-16 14:20:12.556730 oenv2config-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      857 2023-05-02 08:56:52.000000 oenv2config-1.1.0/README.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.460730 oenv2config-1.1.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/antora.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.464730 oenv2config-1.1.0/docs/mkdocs/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/mkdocs/cli.md
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/mkdocs/db_options.md
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/mkdocs/entry.md
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/mkdocs/index.md
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/mkdocs/mappers.md
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/mkdocs/options.md
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/mkdocs/reference.md
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/mkdocs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/mkdocs/utils.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.448730 oenv2config-1.1.0/docs/modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.464730 oenv2config-1.1.0/docs/modules/ROOT/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.500730 oenv2config-1.1.0/docs/modules/ROOT/images/
+-rw-rw-rw-   0 root         (0) root         (0)    44111 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/modules/ROOT/images/run_odoo_test.png
+-rw-rw-rw-   0 root         (0) root         (0)    35877 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/modules/ROOT/images/run_test.png
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/modules/ROOT/nav.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.504730 oenv2config-1.1.0/docs/modules/ROOT/pages/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/modules/ROOT/pages/antora.adoc
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/modules/ROOT/pages/contribute.adoc
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/modules/ROOT/pages/index.adoc
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/modules/ROOT/pages/mkdocs.adoc
+-rw-rw-rw-   0 root         (0) root         (0)      769 2023-06-09 15:06:52.000000 oenv2config-1.1.0/docs/modules/ROOT/pages/tests.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     1878 2023-06-09 15:06:52.000000 oenv2config-1.1.0/docs/modules/ROOT/pages/tests_odoo.adoc
+-rwxrwxrwx   0 root         (0) root         (0)      320 2023-05-05 10:29:38.000000 oenv2config-1.1.0/in_docker_test.sh
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-05-02 08:56:52.000000 oenv2config-1.1.0/mkdocs-plugins.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2023-05-02 08:56:52.000000 oenv2config-1.1.0/mkdocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)      753 2023-05-05 10:29:38.000000 oenv2config-1.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 14:20:12.556730 oenv2config-1.1.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      399 2023-05-02 08:56:52.000000 oenv2config-1.1.0/setup.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.448730 oenv2config-1.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.508730 oenv2config-1.1.0/src/odoo_env_config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.1.0/src/odoo_env_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-16 14:20:12.000000 oenv2config-1.1.0/src/odoo_env_config/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     4656 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     4121 2023-06-14 09:03:06.000000 oenv2config-1.1.0/src/odoo_env_config/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     3782 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/entry.py
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-05-02 08:56:52.000000 oenv2config-1.1.0/src/odoo_env_config/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4853 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/mappers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.448730 oenv2config-1.1.0/src/odoo_env_config/odoo_modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.512730 oenv2config-1.1.0/src/odoo_env_config/odoo_modules/env2config/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-05 10:31:13.000000 oenv2config-1.1.0/src/odoo_env_config/odoo_modules/env2config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-05-02 08:56:52.000000 oenv2config-1.1.0/src/odoo_env_config/odoo_modules/env2config/__manifest__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.512730 oenv2config-1.1.0/src/odoo_env_config/odoo_modules/env2config/cli/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-02 08:56:52.000000 oenv2config-1.1.0/src/odoo_env_config/odoo_modules/env2config/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.516730 oenv2config-1.1.0/src/odoo_env_config/section/
+-rw-rw-rw-   0 root         (0) root         (0)      853 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/section/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/section/addons_path_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     4176 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/section/db_section.py
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/section/http_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     2155 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/section/limit_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/section/log_section.py
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/section/misc_section.py
+-rw-rw-rw-   0 root         (0) root         (0)      830 2023-06-16 12:49:50.000000 oenv2config-1.1.0/src/odoo_env_config/section/s3_section.py
+-rw-rw-rw-   0 root         (0) root         (0)      865 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/section/test_section.py
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/section/update_init_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/section/widemodule_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     2326 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/section/worker_section.py
+-rw-rw-rw-   0 root         (0) root         (0)    10125 2023-05-02 08:56:52.000000 oenv2config-1.1.0/src/odoo_env_config/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.516730 oenv2config-1.1.0/src/oenv2config.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      182 2023-06-16 14:20:12.000000 oenv2config-1.1.0/src/oenv2config.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3285 2023-06-16 14:20:12.000000 oenv2config-1.1.0/src/oenv2config.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 14:20:12.000000 oenv2config-1.1.0/src/oenv2config.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-06-16 14:20:12.000000 oenv2config-1.1.0/src/oenv2config.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2023-06-16 14:20:12.000000 oenv2config-1.1.0/src/oenv2config.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-16 14:20:12.000000 oenv2config-1.1.0/src/oenv2config.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.520730 oenv2config-1.1.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2148 2023-05-05 10:29:38.000000 oenv2config-1.1.0/tests/_decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     3154 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_doctests.py
+-rw-rw-rw-   0 root         (0) root         (0)     4551 2023-06-09 15:06:52.000000 oenv2config-1.1.0/tests/test_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)      740 2023-06-09 15:06:52.000000 oenv2config-1.1.0/tests/test_libs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.520730 oenv2config-1.1.0/tests/test_mapper/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_mapper/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9833 2023-06-14 09:03:06.000000 oenv2config-1.1.0/tests/test_mapper/test_mapper_clever_cloud_cellar.py
+-rw-rw-rw-   0 root         (0) root         (0)    10835 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_mapper/test_mapper_clever_cloud_postgres.py
+-rw-rw-rw-   0 root         (0) root         (0)     6535 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_mapper/test_mapper_odoo_compatibility.py
+-rw-rw-rw-   0 root         (0) root         (0)     5002 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_mapper/test_mapper_queue_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     3921 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_mapper/test_mapper_redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.524730 oenv2config-1.1.0/tests/test_section/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_section/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1366 2023-05-05 10:29:38.000000 oenv2config-1.1.0/tests/test_section/test_addons_path_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     7581 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_section/test_db_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     2339 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_section/test_http_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     5567 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_section/test_limit_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     2489 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_section/test_log_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1389 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_section/test_misc_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     2040 2023-06-16 13:07:56.000000 oenv2config-1.1.0/tests/test_section/test_s3_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1989 2023-05-05 10:29:38.000000 oenv2config-1.1.0/tests/test_section/test_test_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2023-05-05 10:29:38.000000 oenv2config-1.1.0/tests/test_section/test_update_init_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_section/test_widemodule_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     6727 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_section/test_worker_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     2436 2023-06-09 15:06:52.000000 oenv2config-1.1.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.528730 oenv2config-1.1.0/tests/tests_odoo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/tests_odoo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4906 2023-05-05 10:29:38.000000 oenv2config-1.1.0/tests/tests_odoo/_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.556730 oenv2config-1.1.0/tests/tests_odoo/profiles/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/tests_odoo/profiles/filestore_s3.env
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/tests_odoo/profiles/filestore_s3_cellar.env
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/tests_odoo/profiles/test_db_clever.env
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/tests_odoo/profiles/test_db_clever_direct.env
+-rw-rw-rw-   0 root         (0) root         (0)     4115 2023-05-05 10:29:38.000000 oenv2config-1.1.0/tests/tests_odoo/test_base.py
```

### Comparing `oenv2config-1.0.1/.gitignore` & `oenv2config-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/.gitlab-ci.yml` & `oenv2config-1.1.0/.gitlab-ci.yml`

 * *Files 23% similar despite different names*

```diff
@@ -4,17 +4,25 @@
     file:
       - pipeline/classic_workflow.yml
       - python/sexy_code.yml
       - python/pyunit.yml
       - python/build.yml
       - python/deploy.yml
       - python/deploy-tag.yml
+services:
+- name: minio/minio
+  command: ['server', '/minio']
+  alias: minio
 
 variables:
   SUPPORT_PYTHON_VERSION: "3.8;3.9;3.10;3.11;latest"
+  MINIO_SECRET_KEY: "test_access_key"
+  MINIO_ACCESS_KEY: "test_secret_key"
+  MINIO_DOMAIN: "http://minio:9000"
+  ODOO_S3_SECURE: "False"
 
 stages:
   - test
   - test_odoo
   - build
   - deploy
```

### Comparing `oenv2config-1.0.1/.idea/oenv2config.iml` & `oenv2config-1.1.0/.idea/oenv2config.iml`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/.idea/runConfigurations/Python_tests__no_Odoo_.xml` & `oenv2config-1.1.0/.idea/runConfigurations/Python_tests_in_tests_odoo.xml`

 * *Files 6% similar despite different names*

#### Comparing `oenv2config-1.0.1/.idea/runConfigurations/Python_tests__no_Odoo_.xml` & `oenv2config-1.1.0/.idea/runConfigurations/Python_tests_in_tests_odoo.xml`

```diff
@@ -1,29 +1,32 @@
 <?xml version="1.0" encoding="utf-8"?>
 <component name="ProjectRunConfigurationManager">
-  <configuration default="false" name="Python tests (no Odoo)" type="tests" factoryName="Autodetect">
+  <configuration default="false" name="Python tests in tests_odoo" type="tests" factoryName="Autodetect" nameIsGenerated="true">
     <module name="oenv2config"/>
     <option name="INTERPRETER_OPTIONS" value=""/>
     <option name="PARENT_ENVS" value="true"/>
-    <option name="SDK_HOME" value="$USER_HOME$/.pyenv/versions/oenv2config/bin/python"/>
-    <option name="SDK_NAME" value="Python 3.11 (oenv2config)"/>
+    <envs>
+      <env name="ODOO_VERSION" value="15.0"/>
+    </envs>
+    <option name="SDK_HOME" value="$PROJECT_DIR$/../../../python/odoo/v15/venv/bin/python"/>
+    <option name="SDK_NAME" value="Odoo v15 - py3.10"/>
     <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
-    <option name="IS_MODULE_SDK" value="true"/>
-    <option name="ADD_CONTENT_ROOTS" value="true"/>
-    <option name="ADD_SOURCE_ROOTS" value="true"/>
+    <option name="IS_MODULE_SDK" value="false"/>
+    <option name="ADD_CONTENT_ROOTS" value="false"/>
+    <option name="ADD_SOURCE_ROOTS" value="false"/>
     <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
     <EXTENSION ID="net.ashald.envfile">
       <option name="IS_ENABLED" value="false"/>
       <option name="IS_SUBST" value="false"/>
       <option name="IS_PATH_MACRO_SUPPORTED" value="false"/>
       <option name="IS_IGNORE_MISSING_FILES" value="false"/>
       <option name="IS_ENABLE_EXPERIMENTAL_INTEGRATIONS" value="false"/>
       <ENTRIES>
         <ENTRY IS_ENABLED="true" PARSER="runconfig" IS_EXECUTABLE="false"/>
       </ENTRIES>
     </EXTENSION>
     <option name="_new_additionalArguments" value="&quot;&quot;"/>
-    <option name="_new_target" value="&quot;$PROJECT_DIR$/tests&quot;"/>
+    <option name="_new_target" value="&quot;$PROJECT_DIR$/tests/tests_odoo&quot;"/>
     <option name="_new_targetType" value="&quot;PATH&quot;"/>
     <method v="2"/>
   </configuration>
 </component>
```

### Comparing `oenv2config-1.0.1/.idea/runConfigurations/Python_tests_in_tests_odoo.xml` & `oenv2config-1.1.0/.idea/runConfigurations/Python_tests__no_Odoo_.xml`

 * *Files 10% similar despite different names*

#### Comparing `oenv2config-1.0.1/.idea/runConfigurations/Python_tests_in_tests_odoo.xml` & `oenv2config-1.1.0/.idea/runConfigurations/Python_tests__no_Odoo_.xml`

```diff
@@ -1,32 +1,35 @@
 <?xml version="1.0" encoding="utf-8"?>
 <component name="ProjectRunConfigurationManager">
-  <configuration default="false" name="Python tests in tests_odoo" type="tests" factoryName="Autodetect" nameIsGenerated="true">
+  <configuration default="false" name="Python tests (no Odoo)" type="tests" factoryName="Autodetect">
     <module name="oenv2config"/>
     <option name="INTERPRETER_OPTIONS" value=""/>
     <option name="PARENT_ENVS" value="true"/>
+    <option name="SDK_HOME" value="$USER_HOME$/.pyenv/versions/oenv2config/bin/python"/>
+    <option name="SDK_NAME" value="Python 3.11 (oenv2config)"/>
     <envs>
-      <env name="ODOO_VERSION" value="15.0"/>
+      <env name="MINIO_ACCESS_KEY" value="weak_access_key"/>
+      <env name="MINIO_DOMAIN" value="localhost:9000"/>
+      <env name="MINIO_SECRET_KEY" value="weak_secret_key"/>
+      <env name="ODOO_S3_SECURE" value="False"/>
     </envs>
-    <option name="SDK_HOME" value="$PROJECT_DIR$/../../../python/odoo/v15/venv/bin/python"/>
-    <option name="SDK_NAME" value="Odoo v15 - py3.10"/>
     <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
-    <option name="IS_MODULE_SDK" value="false"/>
-    <option name="ADD_CONTENT_ROOTS" value="false"/>
-    <option name="ADD_SOURCE_ROOTS" value="false"/>
+    <option name="IS_MODULE_SDK" value="true"/>
+    <option name="ADD_CONTENT_ROOTS" value="true"/>
+    <option name="ADD_SOURCE_ROOTS" value="true"/>
     <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
     <EXTENSION ID="net.ashald.envfile">
       <option name="IS_ENABLED" value="false"/>
       <option name="IS_SUBST" value="false"/>
       <option name="IS_PATH_MACRO_SUPPORTED" value="false"/>
       <option name="IS_IGNORE_MISSING_FILES" value="false"/>
       <option name="IS_ENABLE_EXPERIMENTAL_INTEGRATIONS" value="false"/>
       <ENTRIES>
         <ENTRY IS_ENABLED="true" PARSER="runconfig" IS_EXECUTABLE="false"/>
       </ENTRIES>
     </EXTENSION>
     <option name="_new_additionalArguments" value="&quot;&quot;"/>
-    <option name="_new_target" value="&quot;$PROJECT_DIR$/tests/tests_odoo&quot;"/>
+    <option name="_new_target" value="&quot;$PROJECT_DIR$/tests&quot;"/>
     <option name="_new_targetType" value="&quot;PATH&quot;"/>
     <method v="2"/>
   </configuration>
 </component>
```

### Comparing `oenv2config-1.0.1/.pre-commit-config.yaml` & `oenv2config-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/README.adoc` & `oenv2config-1.1.0/README.adoc`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/docs/modules/ROOT/images/run_odoo_test.png` & `oenv2config-1.1.0/docs/modules/ROOT/images/run_odoo_test.png`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/docs/modules/ROOT/images/run_test.png` & `oenv2config-1.1.0/docs/modules/ROOT/images/run_test.png`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/docs/modules/ROOT/pages/tests.adoc` & `oenv2config-1.1.0/docs/modules/ROOT/pages/tests.adoc`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-= Test unitaire
+= Test
 
-Ce projet est testé  grace a la lib `unittest`. Tous les tests se trouve dans le dossier `tests` à la racine du projet.
+== Test unitaire
+
+Ce projet est testé  grâce à la lib `unittest`. Tous les tests se trouvent dans le dossier `tests` à la racine du projet.
 
 Pour lancer les tests, vous avez besoin d'aucune library en plus dans votre environment.
 
 .En ligne de commande
 [source, shell, subs="+attributes"]
 ----
 python --version
 # Python 3.11.x
 python -m unittest
 ----
 ou sinon utiliser la configuration fournie `Python tests (no Odoo)`.
 
-= Tests doctests
+== Tests doctests
 
-Certaines classe ou méthodes sont couvertes par des tests **doctes**, qui sont des tests inclus directement dans le docstring. Le fichier `test_doctests.py` sert de point d'entrée pour ces tests. +
+Certaines classes ou méthodes sont couvertes par des tests **doctes**, qui sont des tests inclus directement dans le docstring. Le fichier `test_doctests.py` sert de point d'entrée pour ces tests. +
 Ces tests se lancent en faisant :
 [source, shell, subs="+attributes"]
 ----
 python tests tests/test_doctests.py
 ----
```

### Comparing `oenv2config-1.0.1/docs/modules/ROOT/pages/tests_odoo.adoc` & `oenv2config-1.1.0/docs/modules/ROOT/pages/tests_odoo.adoc`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 = Test unitaire
 
-Cette lib contient **2** types de tests. Les tests classique python, et des test pensépour être joué dans un container Odoo.
+Cette lib contient **2** types de tests. Les tests classique python, et des tests pensés pour être joué dans un container Odoo.
 
 Ces tests sont disponibles dans le dossier `tests`. Il y a une particularité pour certain.
 Vous pouvez lancer tous les tests de cette lib en ligne de commande.
 
 == Unittests
-Ce sont tous les tests ne necessistant pas d'être lancé dans un environment Odoo
+Ce sont tous les tests ne nécessitant pas d'être lancé dans un environment Odoo
 
 
 
 === Lancer en local
 
 [source, shell]
 ----
@@ -27,16 +27,16 @@
 ODOO_VERSION=15.0 \ <1>
     python -m unittest discover \ <2>
     -s tests/tests_odoo \ <3>
     -t ./ <4>
 ----
 <1> Set la variable `ODOO_VERSION` à la version voulu
 <2> Lance les tests
-<3> Precise ou sont les tests, pour ne pas lancer les tests simple
-<4> Force le path au niveau de `./`, pour eviter que python oubli les top level package et avoir des soucis d'import
+<3> Precise où sont les tests, pour ne pas lancer les tests simple
+<4> Force le path au niveau de `./`, pour éviter que python oubli les top level package et avoir des soucis d'import
 
 === Lancer avec une image docker
 
 
 [source, shell]
 ----
 docker run \ <1>
@@ -45,14 +45,14 @@
     --workdir=/builds/oenv2config \ <4>
     --rm \ <5>
     -t registry.ndp-systemes.fr/dockers/odoo:15.0 <6>
 ----
 <1> Run une image docker
 <2> Créer un volume du path local `pwd` vers `/builds/oenv2config` dans le container
 <3> Change l'entrypoint, pour ne pas lancer Odoo, mais lancer `in_docker_test.sh`
-<4> Set le `workdir` au point de montage, pour que lors de l'éxecution de l'entrypoint, nous soyont dans le bon path
+<4> Set le `workdir` au point de montage, pour que lors de l'exécution de l'entrypoint, nous sommes dans le bon path
 <5> Supprime le container apres le run
 <6> l'image docker, ici la v15
 
-Il existe des décorateurs particulier pour ne jouer les tests que dans un environment Odoo.
+Il existe des décorateurs particuliers pour ne jouer les tests que dans un environment Odoo.
 
-Pour les Utiliser if faut les importer dans votre fichier de tests, et ensuite décorer votre focntion avec.
+Pour les Utiliser if faut les importer dans votre fichier de tests, et ensuite décorer votre fonction avec.
```

### Comparing `oenv2config-1.0.1/mkdocs.yml` & `oenv2config-1.1.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/pyproject.toml` & `oenv2config-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/src/odoo_env_config/api.py` & `oenv2config-1.1.0/src/odoo_env_config/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         Returns:
             current self after the `update`
         """
         self.update(*arg, **kwargs)
         return self
 
     def get_bool(self, *keys: str, default: bool = False) -> bool:
-        return utils.is_true(self.gets(*keys, default=str(default)))
+        return utils.to_bool(self.gets(*keys, default=str(default)))
 
     def get_int(self, *keys: str, default: int = 0) -> int:
         return utils.to_int(self.gets(*keys, default=str(default)))
 
     def get_enum(self, key: str, enum_type: Type[ET], *, default: ET) -> ET:
         value = self.get(key)
         if not value or value not in enum_type.__members__:
@@ -157,10 +157,7 @@
         ...
 
     def init(self, curr_env: Env) -> Self:
         return self
 
     def to_values(self) -> OdooCliFlag:
         return OdooCliFlag()
-
-
-EnvConverter = EnvConfigSection
```

### Comparing `oenv2config-1.0.1/src/odoo_env_config/cli.py` & `oenv2config-1.1.0/src/odoo_env_config/cli.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/src/odoo_env_config/mappers.py` & `oenv2config-1.1.0/src/odoo_env_config/mappers.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,19 +16,27 @@
 ]
 
 
 def clevercloud_cellar(curr_env: Env) -> Env:
     """ """
     return curr_env.copy().mutate(
         {
-            "S3_FILESTORE_HOST": curr_env.gets("S3_FILESTORE_HOST", "CELLAR_ADDON_HOST"),
-            "S3_FILESTORE_SECRET_KEY": curr_env.gets("S3_FILESTORE_SECRET_KEY", "CELLAR_ADDON_KEY_SECRET"),
-            "S3_FILESTORE_ACCESS_KEY": curr_env.gets("S3_FILESTORE_ACCESS_KEY", "CELLAR_ADDON_KEY_ID"),
+            "S3_FILESTORE_HOST": curr_env.gets(
+                "S3_FILESTORE_HOST", "CELLAR_ADDON_HOST", "ODOO_S3_HOST", "MINIO_DOMAIN"
+            ),
+            "S3_FILESTORE_SECRET_KEY": curr_env.gets(
+                "S3_FILESTORE_SECRET_KEY", "CELLAR_ADDON_KEY_SECRET", "ODOO_S3_SECRET_KEY", "MINIO_SECRET_KEY"
+            ),
+            "S3_FILESTORE_ACCESS_KEY": curr_env.gets(
+                "S3_FILESTORE_ACCESS_KEY", "CELLAR_ADDON_KEY_ID", "ODOO_S3_ACCESS_KEY", "MINIO_ACCESS_KEY"
+            ),
+            "S3_FILESTORE_BUCKET": curr_env.gets("S3_FILESTORE_BUCKET", "ODOO_S3_BUCKET"),
             # Pas de region fournit par S3 CleverCloud
-            "S3_FILESTORE_REGION": curr_env.gets("S3_FILESTORE_REGION", "CELLAR_ADDON_REGION", default="fr-par"),
+            "S3_FILESTORE_REGION": curr_env.gets("S3_FILESTORE_REGION", "CELLAR_ADDON_REGION", "ODOO_S3_REGION"),
+            "S3_SECURE": curr_env.gets("S3_FILESTORE_SECURE", "ODOO_S3_SECURE"),
         },
     )
 
 
 def clevercloud_postgresql(curr_env: Env) -> Env:
     """ """
     return curr_env.copy().mutate(
@@ -57,15 +65,15 @@
         }
     )
 
 
 def queue_job(curr_env: Env) -> Env:
     """ """
     new_env = curr_env.copy()
-    enable = utils.is_true(curr_env.get("ODOO_QUEUE_JOB_ENABLE"))
+    enable = utils.to_bool(curr_env.get("ODOO_QUEUE_JOB_ENABLE"))
     if not enable:
         return new_env.mutate(ODOO_QUEUE_JOB_ENABLE=str(False))
 
     def copy(s):
         return [p + s for p in ["ODOO_QUEUE_JOB_", "ODOO_CONNECTOR_"]]
 
     return new_env.mutate(
```

### Comparing `oenv2config-1.0.1/src/odoo_env_config/odoo_modules/env2config/__manifest__.py` & `oenv2config-1.1.0/src/odoo_env_config/odoo_modules/env2config/__manifest__.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/src/odoo_env_config/section/__init__.py` & `oenv2config-1.1.0/src/odoo_env_config/section/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,18 +5,20 @@
     "LimitOdooConfigSection",
     "LoggerSection",
     "MiscSection",
     "TestOdooConfigSection",
     "UpdateInstallSection",
     "ServerWideModuleConfigSection",
     "WorkersOdooConfigSection",
+    "S3Section",
 ]
 from .addons_path_section import AddonsPathConfigSection
 from .db_section import DatabaseOdooConfigSection
 from .http_section import HttpOdooConfigSection
 from .limit_section import LimitOdooConfigSection
 from .log_section import LoggerSection
 from .misc_section import MiscSection
 from .test_section import TestOdooConfigSection
 from .update_init_section import UpdateInstallSection
 from .widemodule_section import ServerWideModuleConfigSection
 from .worker_section import WorkersOdooConfigSection
+from .s3_section import S3Section
```

### Comparing `oenv2config-1.0.1/src/odoo_env_config/section/addons_path_section.py` & `oenv2config-1.1.0/src/odoo_env_config/section/addons_path_section.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from addons_installer import addons_installer
 from typing_extensions import Self
 
 from .. import api
 
 
-class AddonsPathConfigSection(api.EnvConverter):
+class AddonsPathConfigSection(api.EnvConfigSection):
     def __init__(self):
         super().__init__()
         self.registry = addons_installer.AddonsFinder()
         self.addons_path: List[str] = []
 
     def init(self, curr_env: api.Env) -> Self:
         result = self.registry.parse_env(env_vars=curr_env)
```

### Comparing `oenv2config-1.0.1/src/odoo_env_config/section/db_section.py` & `oenv2config-1.1.0/src/odoo_env_config/section/db_section.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         FIXED: the value is taken from `"DB_MAX_CONN"` is [os.environ][os.environ]
     """
 
     AUTO = "AUTO"
     FIXED = "FIXED"
 
 
-class DatabaseOdooConfigSection(api.EnvConverter):
+class DatabaseOdooConfigSection(api.EnvConfigSection):
     """
     A dataclass to hold the database Odoo config group option
 
     Attributes:
         name: Name of the database
         host: The URI of the postgresql service get from `"DB_HOST"` in
         user: The URI of the postgresql service get from `"DB_HOST"` in
```

### Comparing `oenv2config-1.0.1/src/odoo_env_config/section/http_section.py` & `oenv2config-1.1.0/src/odoo_env_config/section/http_section.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Union
 
 from typing_extensions import Self
 
 from .. import api
 
 
-class HttpOdooConfigSection(api.EnvConverter):
+class HttpOdooConfigSection(api.EnvConfigSection):
     def __init__(self):
         super().__init__()
         self.enable: bool = False
         self.interface: Union[str, None] = None
         self.port: int = 0
         self.longpolling_port: int = 0
```

### Comparing `oenv2config-1.0.1/src/odoo_env_config/section/limit_section.py` & `oenv2config-1.1.0/src/odoo_env_config/section/limit_section.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing_extensions import Self
 
 from .. import api
 from .worker_section import WorkersOdooConfigSection
 
 
-class LimitOdooConfigSection(api.EnvConverter):
+class LimitOdooConfigSection(api.EnvConfigSection):
     def __init__(self):
         super().__init__()
         self.limit_request = 0
         self.limit_time_cpu = 0
         self.limit_time_real = 0
         self.osv_memory_count_limit = 0
         self.osv_memory_age_limit = 0
```

### Comparing `oenv2config-1.0.1/src/odoo_env_config/section/log_section.py` & `oenv2config-1.1.0/src/odoo_env_config/section/log_section.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing_extensions import Self
 
 from .. import api
 
 
-class LoggerSection(api.EnvConverter):
+class LoggerSection(api.EnvConfigSection):
     def __init__(self) -> None:
         super().__init__()
         self.logfile = None
         self.log_handler = None
         self.log_request = False
         self.log_response = False
         self.log_web = False
```

### Comparing `oenv2config-1.0.1/src/odoo_env_config/section/misc_section.py` & `oenv2config-1.1.0/src/odoo_env_config/section/misc_section.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List
 
 from typing_extensions import Self
 
 from .. import api
 
 
-class MiscSection(api.EnvConverter):
+class MiscSection(api.EnvConfigSection):
     def __init__(self):
         super().__init__()
         self.unaccent = False
         self.without_demo: List[str] = []
         self.stop_after_init = False
         self.save_config_file = False
```

### Comparing `oenv2config-1.0.1/src/odoo_env_config/section/test_section.py` & `oenv2config-1.1.0/src/odoo_env_config/section/test_section.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing_extensions import Self
 
 from .. import api
 
 
-class TestOdooConfigSection(api.EnvConverter):
+class TestOdooConfigSection(api.EnvConfigSection):
     def __init__(self):
         super().__init__()
         self.enable = False
         self.test_tags = None
         self.test_file = None
 
     def init(self, curr_env: api.Env) -> Self:
```

### Comparing `oenv2config-1.0.1/src/odoo_env_config/section/update_init_section.py` & `oenv2config-1.1.0/src/odoo_env_config/section/update_init_section.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing_extensions import Self
 
 from .. import api
 
 
-class UpdateInstallSection(api.EnvConverter):
+class UpdateInstallSection(api.EnvConfigSection):
     def __init__(self):
         super().__init__()
         self.update = []
         self.install = []
 
     def init(self, curr_env: api.Env) -> Self:
         self.update = curr_env.get_list("UPDATE")
```

### Comparing `oenv2config-1.0.1/src/odoo_env_config/section/widemodule_section.py` & `oenv2config-1.1.0/src/odoo_env_config/section/widemodule_section.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections import OrderedDict
 
 from typing_extensions import Self
 
 from .. import api, utils
 
 
-class ServerWideModuleConfigSection(api.EnvConverter):
+class ServerWideModuleConfigSection(api.EnvConfigSection):
     def __init__(self):
         super().__init__()
         self.server_wide_modules = []
 
     def init(self, curr_env: api.Env) -> Self:
         str_server_wide_modules = curr_env.get("SERVER_WIDE_MODULES")
         server_wide_modules = (
```

### Comparing `oenv2config-1.0.1/src/odoo_env_config/section/worker_section.py` & `oenv2config-1.1.0/src/odoo_env_config/section/worker_section.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing_extensions import Self
 
 from .. import api
 from .test_section import TestOdooConfigSection
 
 
-class WorkersOdooConfigSection(api.EnvConverter):
+class WorkersOdooConfigSection(api.EnvConfigSection):
     def __init__(self):
         super().__init__()
         self.http: int = 0
         self.cron: int = 0
         self.job: int = 0
         self.odoo_use_case: api.ServerUseCase = api.ServerUseCase.WORKER
         self._force_set_cron: bool = False
```

### Comparing `oenv2config-1.0.1/src/odoo_env_config/utils.py` & `oenv2config-1.1.0/src/odoo_env_config/utils.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/src/oenv2config.egg-info/SOURCES.txt` & `oenv2config-1.1.0/src/oenv2config.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 src/odoo_env_config/section/__init__.py
 src/odoo_env_config/section/addons_path_section.py
 src/odoo_env_config/section/db_section.py
 src/odoo_env_config/section/http_section.py
 src/odoo_env_config/section/limit_section.py
 src/odoo_env_config/section/log_section.py
 src/odoo_env_config/section/misc_section.py
+src/odoo_env_config/section/s3_section.py
 src/odoo_env_config/section/test_section.py
 src/odoo_env_config/section/update_init_section.py
 src/odoo_env_config/section/widemodule_section.py
 src/odoo_env_config/section/worker_section.py
 src/oenv2config.egg-info/PKG-INFO
 src/oenv2config.egg-info/SOURCES.txt
 src/oenv2config.egg-info/dependency_links.txt
@@ -79,14 +80,15 @@
 tests/test_section/__init__.py
 tests/test_section/test_addons_path_section.py
 tests/test_section/test_db_section.py
 tests/test_section/test_http_section.py
 tests/test_section/test_limit_section.py
 tests/test_section/test_log_section.py
 tests/test_section/test_misc_section.py
+tests/test_section/test_s3_section.py
 tests/test_section/test_test_section.py
 tests/test_section/test_update_init_section.py
 tests/test_section/test_widemodule_section.py
 tests/test_section/test_worker_section.py
 tests/tests_odoo/__init__.py
 tests/tests_odoo/_helpers.py
 tests/tests_odoo/test_base.py
```

### Comparing `oenv2config-1.0.1/tests/_decorators.py` & `oenv2config-1.1.0/tests/_decorators.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/tests/test_cli.py` & `oenv2config-1.1.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/tests/test_libs.py` & `oenv2config-1.1.0/tests/test_libs.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,11 +8,11 @@
     def test_all_mappers_are_register(self):
         number_of_mapper = 5
         self.assertEqual(len(mappers.__all__), number_of_mapper)
         self.assertEqual(len(entry.MAPPER), number_of_mapper)
         self.assertSetEqual(set(mappers.__all__), {mapper.__name__ for mapper in entry.MAPPER})
 
     def test_all_section_are_register(self):
-        number_of_section = 10
+        number_of_section = 11
         self.assertEqual(len(section.__all__), number_of_section)
         self.assertEqual(len(entry.CONVERTER), number_of_section)
         self.assertSetEqual(set(section.__all__), {mapper.__name__ for mapper in entry.CONVERTER})
```

### Comparing `oenv2config-1.0.1/tests/test_mapper/test_mapper_clever_cloud_cellar.py` & `oenv2config-1.1.0/tests/test_mapper/test_mapper_clever_cloud_cellar.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,22 @@
+import os
 import unittest
 
 from odoo_env_config import api
 from odoo_env_config.mappers import clevercloud_cellar
 from tests._decorators import MultiOdooVersion
 
 
 class TestCleverCloudMapperCellar(unittest.TestCase):
     def _test_priority(self, key, to_map, expected):
         result = clevercloud_cellar(api.Env(to_map))
-        self.assertEqual(6, len(result.keys()))
+        self.assertIn(key, result)
         self.assertEqual(
             expected, result[key], "Value of key [%s] is not expected '%s' result : '%s'" % (key, expected, result[key])
         )
-        for key_result, value in result.items():
-            if key_result == "S3_FILESTORE_REGION" and key != key_result:
-                self.assertEqual("fr-par", value)
-                continue
 
     @MultiOdooVersion.with_args
     def test_map_cellar(self, version):
         host = "my-host.com"
         secret_key = "SECRET_KEY"
         key_id = "KEY_ID"
         region = "fr-par"
@@ -30,15 +27,43 @@
                     "CELLAR_ADDON_HOST": host,
                     "CELLAR_ADDON_KEY_SECRET": secret_key,
                     "CELLAR_ADDON_KEY_ID": key_id,
                     "CELLAR_ADDON_REGION": region,
                 }
             )
         )
-        self.assertEqual(9, len(result.keys()))
+        self.assertEqual(11, len(result.keys()))
+
+    @MultiOdooVersion.with_args
+    def test_map_minio(self, version):
+        host = "my-host.com"
+        secret_key = "SECRET_KEY"
+        key_id = "KEY_ID"
+        secure = False
+        result = clevercloud_cellar(
+            api.Env(
+                {
+                    "ODOO_VERSION": str(version),
+                    "MINIO_DOMAIN": host,
+                    "MINIO_SECRET_KEY": secret_key,
+                    "MINIO_ACCESS_KEY": key_id,
+                    "S3_FILESTORE_SECURE": secure,
+                }
+            )
+        )
+        self.assertEqual(11, len(result.keys()))
+
+    def test_service_minio(self):
+        env = api.Env(os.environ)
+        if "MINIO_ACCESS_KEY" in env.keys():
+            result = clevercloud_cellar(env)
+            self.assertTrue(result["S3_FILESTORE_HOST"])
+            self.assertTrue(result["S3_FILESTORE_SECRET_KEY"])
+            self.assertTrue(result["S3_FILESTORE_ACCESS_KEY"])
+            self.assertTrue(result["S3_SECURE"])
 
     @MultiOdooVersion.with_args
     def test_host(self, version):
         """
         Host definition argument are mapped to S3_... corresponding parameters
         """
         host = "my-host.com"
@@ -52,15 +77,15 @@
                     "CELLAR_ADDON_HOST": host,
                     "CELLAR_ADDON_KEY_SECRET": secret_key,
                     "CELLAR_ADDON_KEY_ID": key_id,
                     "CELLAR_ADDON_REGION": region,
                 }
             )
         )
-        self.assertEqual(9, len(result.keys()), "mapper has added 4 parameters S3_FILESTORE_HOST, S3_...")
+        self.assertEqual(11, len(result.keys()), "mapper has added 4 parameters S3_FILESTORE_HOST, S3_...")
         self.assertEqual(host, result["S3_FILESTORE_HOST"])
         self.assertEqual(secret_key, result["S3_FILESTORE_SECRET_KEY"])
         self.assertEqual(key_id, result["S3_FILESTORE_ACCESS_KEY"])
         self.assertEqual(region, result["S3_FILESTORE_REGION"])
 
     @MultiOdooVersion.with_args
     def test_priority(self, version):
@@ -84,15 +109,15 @@
                     "S3_FILESTORE_ACCESS_KEY": key_id + origin,
                     "CELLAR_ADDON_KEY_ID": key_id,
                     "S3_FILESTORE_REGION": region + origin,
                     "CELLAR_ADDON_REGION": region,
                 }
             )
         )
-        self.assertEqual(9, len(result.keys()))
+        self.assertEqual(11, len(result.keys()))
         self.assertEqual(host + origin, result["S3_FILESTORE_HOST"])
         self.assertEqual(secret_key + origin, result["S3_FILESTORE_SECRET_KEY"])
         self.assertEqual(key_id + origin, result["S3_FILESTORE_ACCESS_KEY"])
         self.assertEqual(region + origin, result["S3_FILESTORE_REGION"])
 
     @MultiOdooVersion.with_args
     def test_default_region(self, version):
@@ -105,117 +130,161 @@
                     "ODOO_VERSION": str(version),
                     "CELLAR_ADDON_HOST": host,
                     "CELLAR_ADDON_KEY_SECRET": secret_key,
                     "CELLAR_ADDON_KEY_ID": key_id,
                 }
             )
         )
-        self.assertEqual(8, len(result.keys()), "mapper has set S3_FILESTORE_ENABLE and generated 4 S3_xx parameter")
+        self.assertEqual(10, len(result.keys()), "mapper has set S3_FILESTORE_ENABLE and generated 4 S3_xx parameter")
         self.assertEqual(host, result["S3_FILESTORE_HOST"])
         self.assertEqual(secret_key, result["S3_FILESTORE_SECRET_KEY"])
         self.assertEqual(key_id, result["S3_FILESTORE_ACCESS_KEY"])
-        self.assertEqual("fr-par", result["S3_FILESTORE_REGION"], "internal default value has been used by mapper")
+        self.assertIsNone(result["S3_FILESTORE_REGION"], "internal default value has been used by mapper")
 
     @MultiOdooVersion.with_args
     def test_priority_s3_host(self, version):
         """
         Test the priority of the key
         S3_FILESTORE_HOST > CELLAR_ADDON_HOST
         """
         value1 = "value1"
         value2 = "value2"
+        value3 = "value3"
         self._test_priority(
             key="S3_FILESTORE_HOST",
             to_map={
                 "ODOO_VERSION": str(version),
+                "ODOO_S3_HOST": value3,
                 "S3_FILESTORE_HOST": value1,
                 "CELLAR_ADDON_HOST": value2,
             },
             expected=value1,
         )
+        to_map2 = {
+            "ODOO_VERSION": str(version),
+            "ODOO_S3_HOST": value3,
+            "CELLAR_ADDON_HOST": value2,
+        }
+        self._test_priority(
+            key="S3_FILESTORE_HOST",
+            to_map=to_map2,
+            expected=value2,
+        )
         self._test_priority(
             key="S3_FILESTORE_HOST",
             to_map={
                 "ODOO_VERSION": str(version),
-                # "S3_FILESTORE_HOST": value1,
-                "CELLAR_ADDON_HOST": value2,
+                "ODOO_S3_HOST": value3,
             },
-            expected=value2,
+            expected=value3,
         )
 
     @MultiOdooVersion.with_args
     def test_priority_s3_secret_key(self, version):
         """
         Test the priority of the key
         S3_FILESTORE_SECRET_KEY > CELLAR_ADDON_KEY_SECRET
         """
         value1 = "value1"
         value2 = "value2"
+        value3 = "value3"
         self._test_priority(
             key="S3_FILESTORE_SECRET_KEY",
             to_map={
                 "ODOO_VERSION": str(version),
+                "ODOO_S3_SECRET_KEY": value3,
                 "S3_FILESTORE_SECRET_KEY": value1,
                 "CELLAR_ADDON_KEY_SECRET": value2,
             },
             expected=value1,
         )
         self._test_priority(
             key="S3_FILESTORE_SECRET_KEY",
             to_map={
                 "ODOO_VERSION": str(version),
                 "CELLAR_ADDON_KEY_SECRET": value2,
+                "ODOO_S3_SECRET_KEY": value3,
             },
             expected=value2,
         )
+        self._test_priority(
+            key="S3_FILESTORE_SECRET_KEY",
+            to_map={
+                "ODOO_VERSION": str(version),
+                "ODOO_S3_SECRET_KEY": value3,
+            },
+            expected=value3,
+        )
 
     @MultiOdooVersion.with_args
     def test_priority_s3_acces_key(self, version):
         """
         Test the priority of the key
         S3_FILESTORE_ACCESS_KEY > CELLAR_ADDON_KEY_ID
         """
         value1 = "value1"
         value2 = "value2"
+        value3 = "value3"
         self._test_priority(
             key="S3_FILESTORE_ACCESS_KEY",
             to_map={
                 "ODOO_VERSION": str(version),
-                "S3_FILESTORE_ACCESS_KEY": value1,
                 "CELLAR_ADDON_KEY_ID": value2,
+                "ODOO_S3_ACCESS_KEY": value3,
+                "S3_FILESTORE_ACCESS_KEY": value1,
             },
             expected=value1,
         )
         self._test_priority(
             key="S3_FILESTORE_ACCESS_KEY",
             to_map={
                 "ODOO_VERSION": str(version),
+                "ODOO_S3_ACCESS_KEY": value3,
                 "CELLAR_ADDON_KEY_ID": value2,
             },
             expected=value2,
         )
+        self._test_priority(
+            key="S3_FILESTORE_ACCESS_KEY",
+            to_map={
+                "ODOO_VERSION": str(version),
+                "ODOO_S3_ACCESS_KEY": value3,
+            },
+            expected=value3,
+        )
 
     @MultiOdooVersion.with_args
     def test_priority_s3_region(self, version):
         """
         Test the priority of the key
         S3_FILESTORE_REGION > CELLAR_ADDON_REGION
         """
         value1 = "value1"
         value2 = "value2"
+        value3 = "value3"
         self._test_priority(
             key="S3_FILESTORE_REGION",
             to_map={
                 "ODOO_VERSION": str(version),
+                "ODOO_S3_REGION": value3,
                 "S3_FILESTORE_REGION": value1,
                 "CELLAR_ADDON_REGION": value2,
             },
             expected=value1,
         )
         self._test_priority(
             key="S3_FILESTORE_REGION",
             to_map={
                 "ODOO_VERSION": str(version),
+                "ODOO_S3_REGION": value3,
                 "CELLAR_ADDON_REGION": value2,
             },
             expected=value2,
         )
+        self._test_priority(
+            key="S3_FILESTORE_REGION",
+            to_map={
+                "ODOO_VERSION": str(version),
+                "ODOO_S3_REGION": value3,
+            },
+            expected=value3,
+        )
```

### Comparing `oenv2config-1.0.1/tests/test_mapper/test_mapper_clever_cloud_postgres.py` & `oenv2config-1.1.0/tests/test_mapper/test_mapper_clever_cloud_postgres.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/tests/test_mapper/test_mapper_odoo_compatibility.py` & `oenv2config-1.1.0/tests/test_mapper/test_mapper_odoo_compatibility.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/tests/test_mapper/test_mapper_queue_job.py` & `oenv2config-1.1.0/tests/test_mapper/test_mapper_queue_job.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/tests/test_mapper/test_mapper_redis.py` & `oenv2config-1.1.0/tests/test_mapper/test_mapper_redis.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/tests/test_section/test_addons_path_section.py` & `oenv2config-1.1.0/tests/test_section/test_addons_path_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/tests/test_section/test_db_section.py` & `oenv2config-1.1.0/tests/test_section/test_db_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/tests/test_section/test_http_section.py` & `oenv2config-1.1.0/tests/test_section/test_http_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/tests/test_section/test_limit_section.py` & `oenv2config-1.1.0/tests/test_section/test_limit_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/tests/test_section/test_log_section.py` & `oenv2config-1.1.0/tests/test_section/test_log_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/tests/test_section/test_misc_section.py` & `oenv2config-1.1.0/tests/test_section/test_misc_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/tests/test_section/test_test_section.py` & `oenv2config-1.1.0/tests/test_section/test_test_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/tests/test_section/test_update_init_section.py` & `oenv2config-1.1.0/tests/test_section/test_update_init_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/tests/test_section/test_widemodule_section.py` & `oenv2config-1.1.0/tests/test_section/test_widemodule_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/tests/test_section/test_worker_section.py` & `oenv2config-1.1.0/tests/test_section/test_worker_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/tests/test_utils.py` & `oenv2config-1.1.0/tests/test_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import unittest
 
 from odoo_env_config import utils
 
 
 class TestUtils(unittest.TestCase):
     def test_is_true(self):
-        self.assertTrue(utils.is_true(str(True)))
-        self.assertTrue(utils.is_true(str(1)))
+        self.assertTrue(utils.to_bool(str(True)))
+        self.assertTrue(utils.to_bool(str(1)))
 
-        self.assertTrue(utils.is_true(True))
-        self.assertTrue(utils.is_true(1))
+        self.assertTrue(utils.to_bool(True))
+        self.assertTrue(utils.to_bool(1))
 
-        self.assertFalse(utils.is_true(str(False)))
-        self.assertFalse(utils.is_true(str(0)))
-        self.assertFalse(utils.is_true(str(0.0)))
-        self.assertFalse(utils.is_true(str(None)))
-
-        self.assertFalse(utils.is_true(False))
-        self.assertFalse(utils.is_true(0))
-        self.assertFalse(utils.is_true(0.0))
-        self.assertFalse(utils.is_true(1.0))
-
-        self.assertFalse(utils.is_true(object()))
-        self.assertFalse(utils.is_true(None))
-        self.assertFalse(utils.is_true([]))
-        self.assertFalse(utils.is_true([1, 2, 3]))
-        self.assertFalse(utils.is_true((1, 2, 3)))
-        self.assertFalse(utils.is_true({1, 2, 3}))
-        self.assertFalse(utils.is_true({"key": "value"}))
+        self.assertFalse(utils.to_bool(str(False)))
+        self.assertFalse(utils.to_bool(str(0)))
+        self.assertFalse(utils.to_bool(str(0.0)))
+        self.assertFalse(utils.to_bool(str(None)))
+
+        self.assertFalse(utils.to_bool(False))
+        self.assertFalse(utils.to_bool(0))
+        self.assertFalse(utils.to_bool(0.0))
+        self.assertFalse(utils.to_bool(1.0))
+
+        self.assertFalse(utils.to_bool(object()))
+        self.assertFalse(utils.to_bool(None))
+        self.assertFalse(utils.to_bool([]))
+        self.assertFalse(utils.to_bool([1, 2, 3]))
+        self.assertFalse(utils.to_bool((1, 2, 3)))
+        self.assertFalse(utils.to_bool({1, 2, 3}))
+        self.assertFalse(utils.to_bool({"key": "value"}))
 
     def test_to_int(self):
         self.assertEqual(0, utils.to_int(str(True)))
         self.assertEqual(0, utils.to_int(True))
         self.assertEqual(1, utils.to_int(str(1)))
 
         self.assertEqual(1, utils.to_int(1))
```

### Comparing `oenv2config-1.0.1/tests/tests_odoo/_helpers.py` & `oenv2config-1.1.0/tests/tests_odoo/_helpers.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.1/tests/tests_odoo/test_base.py` & `oenv2config-1.1.0/tests/tests_odoo/test_base.py`

 * *Files identical despite different names*

