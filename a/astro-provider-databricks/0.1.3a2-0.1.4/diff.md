# Comparing `tmp/astro_provider_databricks-0.1.3a2.tar.gz` & `tmp/astro_provider_databricks-0.1.4.tar.gz`

## Comparing `astro_provider_databricks-0.1.3a2.tar` & `astro_provider_databricks-0.1.4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/.deepsource.toml
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/CHANGELOG.rst
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/Tiltfile
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/codecov.yml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/mlc-config.json
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/noxfile.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/yamllint-config.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/.github/CODEOWNERS
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/.github/ci-test-connections.yaml
--rwxr-xr-x   0        0        0      696 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/.github/scripts/verify_tag_and_version.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/.github/workflows/astro-deploy.yml
--rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/.github/workflows/docs.yml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/.github/workflows/mlc_config.json
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/dev/.dockerignore
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/dev/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/dev/Dockerfile
--rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/dev/docker-compose.yaml
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/dev/packages.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/dev/requirements.txt
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/dev/.astro/config.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/docs/Makefile
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/docs/conf.py
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/docs/contributing.rst
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/docs/index.rst
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/docs/make.bat
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/docs/requirements.txt
--rw-r--r--   0        0        0   737260 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/docs/_static/banner.png
--rw-r--r--   0        0        0   146128 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/docs/_static/dbt_dag.png
--rw-r--r--   0        0        0   361967 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/docs/_static/dbt_task_group.png
--rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/docs/_static/logo-dark.png
--rw-r--r--   0        0        0    11220 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/docs/_static/logo-light.png
--rw-r--r--   0        0        0    80206 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/docs/_static/connections_doc/bigquery_airflow_connection.png
--rw-r--r--   0        0        0    82236 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/docs/_static/connections_doc/databricks_airflow_connection.png
--rw-r--r--   0        0        0    72389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/docs/_static/connections_doc/postgres_airflow_connection.png
--rw-r--r--   0        0        0    75178 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/docs/_static/connections_doc/redshift_airflow_connection.png
--rw-r--r--   0        0        0   108877 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/docs/_static/connections_doc/snowflake_airflow_connection.png
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/docs/_static/css/custom.css
--rw-r--r--   0        0        0    30924 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/docs/assets/images/dbutils-notebook-success.png
--rw-r--r--   0        0        0    73030 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/docs/assets/images/repair-all-failed.png
--rw-r--r--   0        0        0   140389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/docs/assets/images/repair-single-failed.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/example_dags/.airflowignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/example_dags/__init__.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/example_dags/example_databricks_notebook.py
--rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/example_dags/example_databricks_workflow.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/astro_databricks/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/astro_databricks/constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/astro_databricks/operators/__init__.py
--rw-r--r--   0        0        0    12957 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/astro_databricks/operators/notebook.py
--rw-r--r--   0        0        0    16728 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/astro_databricks/operators/workflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/astro_databricks/plugins/__init__.py
--rw-r--r--   0        0        0    17286 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/astro_databricks/plugins/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/tests/__init__.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/tests/conftest.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/tests/pytest.ini
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/tests/test_example_dags.py
--rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/tests/databricks/__init__.py
--rw-r--r--   0        0        0    14882 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/tests/databricks/test_notebook.py
--rw-r--r--   0        0        0    11683 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/tests/databricks/test_plugin.py
--rw-r--r--   0        0        0    10682 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/tests/databricks/test_workflow.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/LICENSE
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/README.md
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/pyproject.toml
--rw-r--r--   0        0        0    10065 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.3a2/PKG-INFO
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/.deepsource.toml
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/CHANGELOG.rst
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/Tiltfile
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/codecov.yml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/mlc-config.json
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/noxfile.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/yamllint-config.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/.github/CODEOWNERS
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/.github/ci-test-connections.yaml
+-rwxr-xr-x   0        0        0      696 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/.github/scripts/verify_tag_and_version.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/.github/workflows/astro-deploy.yml
+-rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/.github/workflows/mlc_config.json
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/dev/.dockerignore
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/dev/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/dev/Dockerfile
+-rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/dev/docker-compose.yaml
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/dev/packages.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/dev/requirements.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/dev/.astro/config.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/Makefile
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/conf.py
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/contributing.rst
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/index.rst
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/make.bat
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/requirements.txt
+-rw-r--r--   0        0        0   737260 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/_static/banner.png
+-rw-r--r--   0        0        0   146128 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/_static/dbt_dag.png
+-rw-r--r--   0        0        0   361967 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/_static/dbt_task_group.png
+-rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/_static/logo-dark.png
+-rw-r--r--   0        0        0    11220 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/_static/logo-light.png
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/_static/css/custom.css
+-rw-r--r--   0        0        0   212922 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/_static/screenshots/workflow_1_airflow.png
+-rw-r--r--   0        0        0   763410 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/_static/screenshots/workflow_1_databricks.png
+-rw-r--r--   0        0        0    30924 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/assets/images/dbutils-notebook-success.png
+-rw-r--r--   0        0        0    73030 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/assets/images/repair-all-failed.png
+-rw-r--r--   0        0        0   140389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/docs/assets/images/repair-single-failed.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/example_dags/.airflowignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/example_dags/__init__.py
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/example_dags/example_databricks_notebook.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/example_dags/example_databricks_workflow.py
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/example_dags/example_task_group.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/quickstart/astro-cli.md
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/quickstart/without-astro-cli.md
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/astro_databricks/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/astro_databricks/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/astro_databricks/operators/__init__.py
+-rw-r--r--   0        0        0    14553 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/astro_databricks/operators/notebook.py
+-rw-r--r--   0        0        0    16728 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/astro_databricks/operators/workflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/astro_databricks/plugins/__init__.py
+-rw-r--r--   0        0        0    18556 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/astro_databricks/plugins/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/tests/conftest.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/tests/pytest.ini
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/tests/test_example_dags.py
+-rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/tests/databricks/__init__.py
+-rw-r--r--   0        0        0    14882 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/tests/databricks/test_notebook.py
+-rw-r--r--   0        0        0    15212 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/tests/databricks/test_plugin.py
+-rw-r--r--   0        0        0    16747 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/tests/databricks/test_workflow.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/LICENSE
+-rw-r--r--   0        0        0     6173 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/README.md
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     8134 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.4/PKG-INFO
```

### Comparing `astro_provider_databricks-0.1.3a2/.pre-commit-config.yaml` & `astro_provider_databricks-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/CHANGELOG.rst` & `astro_provider_databricks-0.1.4/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 Changelog
 =========
 
+0.1.4 (23-06-16)
+----------------
+
+Bug fixes
+
+* Fix repairing tasks declared in inner task groups (PR `#49 <https://github.com/astronomer/astro-provider-databricks/pull/49>`_ by @tatiana)
+* Fix copying dependencies from task groups to tasks inside intermediate task groups (PR `#47 <https://github.com/astronomer/astro-provider-databricks/pull/47>`_ by @tatiana)
+
+
+Enhancements
+
+* Documentation improvements (PRs `#43 <https://github.com/astronomer/astro-provider-databricks/pull/43>`_ and `#44 <https://github.com/astronomer/astro-provider-databricks/pull/44>`_ by @jlaneve)
+
+
 0.1.3 (23-04-27)
 ----------------
 
 Enhancements
 
 * Associate a **DatabricksNotebookOperator** to a **DatabricksWorkflowTaskGroup** even if there are up to three levels **TaskGroups** in between (issue `#29 <https://github.com/astronomer/astro-provider-databricks/issues/29>`_)
 * Support templating the field **notebook_params** of the **DatabricksNotebookOperator**  (issue `#33 <https://github.com/astronomer/astro-provider-databricks/issues/33>`_)
```

### Comparing `astro_provider_databricks-0.1.3a2/CODE_OF_CONDUCT.md` & `astro_provider_databricks-0.1.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/Tiltfile` & `astro_provider_databricks-0.1.4/Tiltfile`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/noxfile.py` & `astro_provider_databricks-0.1.4/noxfile.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Nox automation definitions."""
 import os
 from pathlib import Path
 
 import nox
+from packaging import version
 
 nox.options.sessions = ["dev"]
-nox.options.reuse_existing_virtualenvs = True
+nox.options.error_on_external_run = False
+# nox.options.reuse_existing_virtualenvs = True
 
 
 @nox.session(python="3.10")
 def dev(session: nox.Session) -> None:
     """Create a dev environment with everything installed.
 
     This is useful for setting up IDE for autocompletion etc. Point the
@@ -32,14 +34,19 @@
 def test(session: nox.Session, airflow) -> None:
     """Run both unit and integration tests."""
     env = {
         "AIRFLOW_HOME": f"~/airflow-{airflow}-python-{session.python}",
         "AIRFLOW__CORE__ALLOWED_DESERIALIZATION_CLASSES": "airflow\\.* astro\\.* astro_databricks\\.*",
     }
 
+    # Workaround to the issue:
+    # RuntimeError: The package `apache-airflow-providers-databricks:4.2.0` requires Apache Airflow 2.4.0+
+    if version.parse(airflow) < version.parse("2.4"):
+        session.install("apache-airflow-providers-databricks<4.2")
+
     session.install("-e", ".[tests]")
     session.install(f"apache-airflow=={airflow}")
 
     # Log all the installed dependencies
     session.log("Installed Dependencies:")
     session.run("pip3", "freeze")
```

### Comparing `astro_provider_databricks-0.1.3a2/.github/scripts/verify_tag_and_version.py` & `astro_provider_databricks-0.1.4/.github/scripts/verify_tag_and_version.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/.github/workflows/astro-deploy.yml` & `astro_provider_databricks-0.1.4/.github/workflows/astro-deploy.yml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/.github/workflows/ci.yml` & `astro_provider_databricks-0.1.4/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 #          architecture: 'x64'
 #      - uses: actions/cache@v3
 #        with:
 #          path: |
 #            ~/.cache/pip
 #            .nox
 #          key: ${{ runner.os }}-${{ hashFiles('pyproject.toml') }}
-#      - run: pip3 install nox
+#      - run: pip3 install nox packaging
 #      - run: nox -s type_check
 
   Build-Docs:
     if: github.event.action != 'labeled'
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
@@ -65,15 +65,15 @@
           architecture: 'x64'
       - uses: actions/cache@v3
         with:
           path: |
             ~/.cache/pip
             .nox
           key: ${{ runner.os }}-${{ hashFiles('pyproject.toml') }}
-      - run: pip3 install nox
+      - run: pip3 install nox packaging
       - run: nox -s build_docs
 
   Run-Unit-Tests:
     strategy:
       fail-fast: false
       matrix:
         python: [ '3.8', '3.9', '3.10' ]
@@ -107,15 +107,15 @@
           architecture: 'x64'
       - uses: actions/cache@v3
         with:
           path: |
             ~/.cache/pip
             .nox
           key: unit-tests-os-${{ runner.os }}-python-${{ matrix.python }}-airflow-${{ matrix.airflow }}-deps-${{ hashFiles('pyproject.toml') }}-version-${{ hashFiles('src/astro_databricks/__init__.py') }}
-      - run: pip3 install nox
+      - run: pip3 install nox packaging
       - run: nox -s "test-${{ matrix.python }}(airflow='${{ matrix.airflow }}')" -- --ignore "tests/test_example_dags.py" --cov-report=xml
       - name: Upload coverage
         uses: actions/upload-artifact@v2
         with:
           name: coverage-unit-tests-${{ matrix.python }}-${{ matrix.airflow }}
           path: ./.coverage
 
@@ -155,18 +155,18 @@
           python-version: ${{ matrix.python }}
           architecture: 'x64'
       - uses: actions/cache@v3
         with:
           path: |
             ~/.cache/pip
             .nox
-          key: example-dags-os-${{ runner.os }}-python-${{ matrix.python }}-airflow-${{ matrix.airflow }}-deps-${{ hashFiles('pyproject.toml') }}-version-${{ hashFiles('src/astro_databricks/__init__.py') }}
+          key: example-dags-os-${{ runner.os }}-python-${{ matrix.python }}-airflow-${{ matrix.airflow }}-deps-${{ hashFiles('pyproject.toml') }}-nox-${{ hashFiles('noxfile.py') }}-version-${{ hashFiles('src/astro_databricks/__init__.py') }}
       - run: cat .github/ci-test-connections.yaml > test-connections.yaml
       - run: sqlite3 /tmp/sqlite_default.db "VACUUM;"
-      - run: pip3 install nox
+      - run: pip3 install nox packaging
       - run: DATABRICKS_GROUP_ID="${{github.run_id}}_${{matrix.python}}_${{matrix.airflow}}" nox -s "test-${{ matrix.python }}(airflow='${{ matrix.airflow }}')" -- "tests/test_example_dags.py" --cov-report=xml
       - name: Upload coverage
         uses: actions/upload-artifact@v2
         with:
           name: coverage-example-dags-${{ matrix.python }}-${{ matrix.airflow }}
           path: ./.coverage
     env:
```

### Comparing `astro_provider_databricks-0.1.3a2/.github/workflows/docs.yml` & `astro_provider_databricks-0.1.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/dev/Dockerfile` & `astro_provider_databricks-0.1.4/dev/Dockerfile`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/dev/docker-compose.yaml` & `astro_provider_databricks-0.1.4/dev/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/docs/Makefile` & `astro_provider_databricks-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/docs/conf.py` & `astro_provider_databricks-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/docs/contributing.rst` & `astro_provider_databricks-0.1.4/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/docs/index.rst` & `astro_provider_databricks-0.1.4/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Astro Databricks Provider
 =========================
 
-This is a provider for running Databricks Jobs on Aiflow created by Astronomer.
+This is a provider for running Databricks Jobs on Airflow created by Astronomer.
 
 Databricks Workflow TaskGroup
 """"""""""""""""""""""""""""""""""""
 
 The Databricks Workflow TaskGroup is a recent addition to the Databricks platform that allows users to easily create
 and manage Databricks Jobs with multiple notebooks, SQL statements, python files, etc. One of the biggest benefits
 offered by Databricks Jobs is the use of Job Clusters, which are significantly cheaper than all-purpose clusters.
@@ -13,42 +13,45 @@
 With the DatabricksWorkflowTaskGroup, users can take advantage of the cost savings offered by using Jobs clusters,
 while also having the flexibility and multi-platform capabilities of Airflow.
 
 The DatabricksWorkflowTaskGroup is designed to look and function like a standard task group,
 with the added ability to include specific Databricks arguments.
 An example of how to use the DatabricksWorkflowTaskGroup can be seen in the following code snippet:
 
-.. literalinclude:: /../examples/databricks/example_databricks_workflow.py
+.. literalinclude:: /../example_dags/example_databricks_workflow.py
     :language: python
     :dedent: 4
     :start-after: [START howto_databricks_workflow_notebook]
     :end-before: [END howto_databricks_workflow_notebook]
 
 At the top-level Taskgroup definition, users can define workflow-level parameters such as ``notebook_params``,
 ``notebook_packages`` or ``spark_submit_params``. These parameters will be applied to all tasks within the Workflow.
 Inside of the taskgroup, users can define the individual tasks that make up the workflow. Currently the only officially
 supported operator is the DatabricksNotebookOperator, but other operators can be used as long as they contain the
 ``convert_to_databricks_workflow_task`` function. In the future we plan to support SQL and python functions via the
-ref:`https://github.com/astronomer/astro-sdk<Astro SDK>`.
+`Astro SDK`_.
+
+.. _Astro SDK: https://github.com/astronomer/astro-sdk
 
 For each notebook task, packages defined with the ``notebook_packages`` parameter defined at the task level are
 installed and additionally, all the packages supplied via the workflow-level parameter ``notebook_packages`` are also
 installed for its run. The collated ``notebook_packages`` list type parameter is transformed into the ``libraries`` list
 type parameter accepted by the Databricks API and a list of supported library types and their format for the API
-specification is mentioned at the Databricks documentation:
-https://docs.databricks.com/dev-tools/api/latest/libraries.html#managedlibrarieslibrary
+specification is mentioned at the `Databricks documentation`_.
+
+.. _Databricks documentation: https://docs.databricks.com/dev-tools/api/latest/libraries.html#managedlibrarieslibrary
 
 .. warning::
     Make sure that you do not specify duplicate libraries across workflow-level and task-level ``notebook-packages`` as
     the Databricks task will then fail complaining about duplicate installation of the library.
 
 Retries
 =======
 
-When repairing a DatabBricks workflow, we need to submit a repair request using databricks' Jobs API. One core difference between how databricks repairs work v.s. Airflow retries is that Airflow is able to retry one task at a time, while Databricks expects a single repair request for all tasks you want to rerun (this is because databricks starts a new job cluster for each repair request, and jobs clusters can't be modified once they are started).
+When repairing a Databricks workflow, we need to submit a repair request using Databricks' Jobs API. One core difference between how Databricks repairs work v.s. Airflow retries is that Airflow is able to retry one task at a time, while Databricks expects a single repair request for all tasks you want to rerun (this is because Databricks starts a new job cluster for each repair request, and jobs clusters can't be modified once they are started).
 
 To avoid creating multiple clusters for each failed task, we do not use Airflow's built-in retries. Instead, we offer a "Repair all tasks" button in the "launch" task's grid and graph node on the Airflow UI. This button finds all failed and skipped tasks and sends them to Databricks for repair. By using this approach, we can save time and resources, as we do not need to create a new cluster for each failed task.
 
 .. image:: assets/images/repair-all-failed.png
   :width: 400
   :alt: Alternative text
 In addition to the "Repair all tasks" button, we also provide a "Repair single task" button to repair a specific failed task. This button can be used if we want to retry a single task rather than all failed tasks.
@@ -61,11 +64,9 @@
 .. image:: assets/images/dbutils-notebook-success.png
   :width: 400
   :alt: Alternative text
 Limitations
 ===========
 The DatabricksWorkflowTaskGroup is currently in beta and has the following limitations:
 
-* Since Databricks Workflow Jobs do not support dynamic parameters at the task level, we recommend placing dynamic parameters
-at the TaskGroup level (e.g. the ``notebook_params`` parameter in the example above). This will ensure that the job is not changed every time
-the DAG is run.
+* Since Databricks Workflow Jobs do not support dynamic parameters at the task level, we recommend placing dynamic parameters at the TaskGroup level (e.g. the ``notebook_params`` parameter in the example above). This will ensure that the job is not changed every time the DAG is run.
 * If you plan to run the same DAG multiple times at the same time, make sure to set the ``max_concurrency`` parameter to the expected number of concurrent runs.
```

### Comparing `astro_provider_databricks-0.1.3a2/docs/make.bat` & `astro_provider_databricks-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/docs/_static/banner.png` & `astro_provider_databricks-0.1.4/docs/_static/banner.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/docs/_static/dbt_dag.png` & `astro_provider_databricks-0.1.4/docs/_static/dbt_dag.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/docs/_static/dbt_task_group.png` & `astro_provider_databricks-0.1.4/docs/_static/dbt_task_group.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/docs/_static/logo-dark.png` & `astro_provider_databricks-0.1.4/docs/_static/logo-dark.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/docs/_static/logo-light.png` & `astro_provider_databricks-0.1.4/docs/_static/logo-light.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/docs/assets/images/dbutils-notebook-success.png` & `astro_provider_databricks-0.1.4/docs/assets/images/dbutils-notebook-success.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/docs/assets/images/repair-all-failed.png` & `astro_provider_databricks-0.1.4/docs/assets/images/repair-all-failed.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/docs/assets/images/repair-single-failed.png` & `astro_provider_databricks-0.1.4/docs/assets/images/repair-single-failed.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/example_dags/example_databricks_notebook.py` & `astro_provider_databricks-0.1.4/example_dags/example_databricks_notebook.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from airflow.models.dag import DAG
 from airflow.utils.timezone import datetime
 from astro_databricks import DatabricksNotebookOperator
 
 EXECUTION_TIMEOUT = int(os.getenv("EXECUTION_TIMEOUT", 6))
 default_args = {
     "execution_timeout": timedelta(hours=EXECUTION_TIMEOUT),
-    "retries": int(os.getenv("DEFAULT_TASK_RETRIES", 2)),
+    # Users are encouraged to use the repair feature, retries may fail:
+    "retries": int(os.getenv("DEFAULT_TASK_RETRIES", 0)),
     "retry_delay": timedelta(seconds=int(os.getenv("DEFAULT_RETRY_DELAY_SECONDS", 60))),
 }
 
 DATABRICKS_CONN_ID = os.getenv("ASTRO_DATABRICKS_CONN_ID", "databricks_conn")
 NEW_CLUSTER_SPEC = {
     "cluster_name": "",
     "spark_version": "11.3.x-scala2.12",
```

### Comparing `astro_provider_databricks-0.1.3a2/example_dags/example_databricks_workflow.py` & `astro_provider_databricks-0.1.4/example_dags/example_databricks_workflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from airflow.models.dag import DAG
 from airflow.utils.timezone import datetime
 from astro_databricks import DatabricksNotebookOperator, DatabricksWorkflowTaskGroup
 
 EXECUTION_TIMEOUT = int(os.getenv("EXECUTION_TIMEOUT", 6))
 default_args = {
     "execution_timeout": timedelta(hours=EXECUTION_TIMEOUT),
-    "retries": int(os.getenv("DEFAULT_TASK_RETRIES", 2)),
+    # Users are encouraged to use the repair feature, retries may fail:
+    "retries": int(os.getenv("DEFAULT_TASK_RETRIES", 0)),
     "retry_delay": timedelta(seconds=int(os.getenv("DEFAULT_RETRY_DELAY_SECONDS", 60))),
 }
 
 DATABRICKS_CONN_ID = os.getenv("ASTRO_DATABRICKS_CONN_ID", "databricks_conn")
 DATABRICKS_NOTIFICATION_EMAIL = os.getenv(
     "ASTRO_DATABRICKS_NOTIFICATION_EMAIL", "tatiana.alchueyr@astronomer.io"
 )
```

### Comparing `astro_provider_databricks-0.1.3a2/astro_databricks/operators/notebook.py` & `astro_provider_databricks-0.1.4/astro_databricks/operators/notebook.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """DatabricksNotebookOperator for submitting notebook jobs to databricks."""
 from __future__ import annotations
 
 import time
 from typing import Any
 
+import airflow
 from airflow.exceptions import AirflowException
 from airflow.models import BaseOperator
 from airflow.providers.databricks.hooks.databricks import DatabricksHook
 from airflow.utils.context import Context
+from airflow.utils.task_group import TaskGroup
 from databricks_cli.runs.api import RunsApi
 from databricks_cli.sdk.api_client import ApiClient
 
 from astro_databricks.constants import JOBS_API_VERSION
 from astro_databricks.operators.workflow import (
     DatabricksMetaData,
     DatabricksWorkflowTaskGroup,
@@ -125,33 +127,66 @@
                 "notebook_path": self.notebook_path,
                 "source": self.source,
                 "base_parameters": self.notebook_params,
             },
             "libraries": self.notebook_packages,
         }
 
+    def merge_notebook_packages(self, databricks_task_group: TaskGroup):
+        """
+        Merge the task group notebook packages into the notebook's packages, without adding any identical duplicates.
+        Modifies self.notebook_packages in place.
+
+        Example value for self.notebook_packages:
+        [
+            {"pypi": {"package": "requests_toolbelt==1.0.0"}}
+        ]
+
+        """
+        for task_group_package in databricks_task_group.notebook_packages:
+            exists = False
+            for existing_package in self.notebook_packages:
+                if task_group_package == existing_package:
+                    exists = True
+                    break
+            if not exists:
+                self.notebook_packages.append(task_group_package)
+
+    def find_parent_databricks_workflow_task_group(self):
+        """
+        Find the closest parent_group which is an instance of DatabricksWorkflowTaskGroup.
+
+        In the case of Airflow 2.2.x, inner Task Groups do not inherit properties from Parent Task Groups like more
+        recent versions of Airflow. This lead to the issue:
+        https://github.com/astronomer/astro-provider-databricks/pull/47
+        """
+        parent_group = self.task_group
+        while parent_group:
+            if parent_group.__class__.__name__ == "DatabricksWorkflowTaskGroup":
+                return parent_group
+            parent_group = parent_group._parent_group
+
     def convert_to_databricks_workflow_task(
         self, relevant_upstreams: list[BaseOperator], context: Context | None = None
     ):
         """
         Convert the operator to a Databricks workflow task that can be a task in a workflow
         """
-        if self.databricks_task_group and hasattr(
-            self.databricks_task_group,
-            "notebook_packages",
-        ):
-            self.notebook_packages.extend(self.databricks_task_group.notebook_packages)
-
-        if self.databricks_task_group and hasattr(
-            self.databricks_task_group,
-            "notebook_params",
-        ):
+        if airflow.__version__ in ("2.2.4", "2.2.5"):
+            databricks_task_group = self.find_parent_databricks_workflow_task_group()
+        else:
+            databricks_task_group = self.databricks_task_group
+
+        if databricks_task_group and hasattr(databricks_task_group, "notebook_packages"):
+            self.merge_notebook_packages(databricks_task_group)
+
+        if databricks_task_group and hasattr(databricks_task_group, "notebook_params"):
             self.notebook_params = {
                 **self.notebook_params,
-                **self.databricks_task_group.notebook_params,
+                **databricks_task_group.notebook_params,
             }
         if context:
             # The following exception currently only happens on Airflow 2.3, with the following error:
             # airflow.exceptions.AirflowException: XComArg result from test_workflow.launch at example_databricks_workflow with key="return_value" is not found!
             try:
                 self.render_template_fields(context)
             except AirflowException:
```

### Comparing `astro_provider_databricks-0.1.3a2/astro_databricks/operators/workflow.py` & `astro_provider_databricks-0.1.4/astro_databricks/operators/workflow.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/astro_databricks/plugins/plugin.py` & `astro_provider_databricks-0.1.4/astro_databricks/plugins/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -187,14 +187,31 @@
             val = find_my_group(group, task_id)
             if val:
                 return val
 
     return find_my_group(operator.dag.task_group, operator.task_id)
 
 
+def get_launch_task_id(task_group: TaskGroup) -> str:
+    """
+    Retrieve the launch task ID from the current task group or a parent task group,
+    recursively.
+
+    :param task_group: Task Group to be inspected
+    :return: launch Task ID
+    """
+    try:
+        launch_task_id = task_group.get_child_by_label("launch").task_id
+        print("launch task id %s", launch_task_id)
+    except KeyError:
+        launch_task_id = get_launch_task_id(task_group.parent_group)
+
+    return launch_task_id
+
+
 def _get_launch_task_key(
     current_task_key: TaskInstanceKey, task_id: str
 ) -> TaskInstanceKey:
     """
     Returns the task key for the launch task. This allows us to gather databricks Metadata
     even if the current task has failed (since tasks only create xcom values if they succeed).
 
@@ -288,15 +305,15 @@
         dag = _get_flask_app().dag_bag.get_dag(ti_key.dag_id)
         dag.get_task(ti_key.task_id)
         self.log.info("Getting link for task %s", ti_key.task_id)
         if ".launch" not in ti_key.task_id:
             self.log.debug(
                 "Finding the launch task for job run metadata %s", ti_key.task_id
             )
-            launch_task_id = task_group.get_child_by_label("launch").task_id
+            launch_task_id = get_launch_task_id(task_group)
             ti_key = _get_launch_task_key(ti_key, task_id=launch_task_id)
         # Should we catch the exception here if there is no return value?
         metadata = get_xcom_result(ti_key, "return_value", ti)
 
         hook = DatabricksHook(metadata.databricks_conn_id)
         return f"https://{hook.host}/#job/{metadata.databricks_job_id}/run/{metadata.databricks_run_id}"
 
@@ -331,36 +348,56 @@
             f"/repair_databricks_job?dag_id={ti_key.dag_id}&"
             f"databricks_conn_id={metadata.databricks_conn_id}&"
             f"databricks_run_id={metadata.databricks_run_id}&"
             f"run_id={ti_key.run_id}&"
             f"tasks_to_repair={tasks_str}"
         )
 
+    @classmethod
+    def get_task_group_children(cls, task_group):
+        """
+        Given a TaskGroup, return children which are Tasks, inspecting recursively any TaskGroups within.
+
+        :param task_group: An Airflow TaskGroup
+        :return: Dictionary that contains Task IDs as keys and Tasks as values.
+        """
+        children = {}
+        for child_id, child in task_group.children.items():
+            if isinstance(child, TaskGroup):
+                child_children = cls.get_task_group_children(child)
+                children = {**children, **child_children}
+            else:
+                children[child_id] = child
+        return children
+
     def get_tasks_to_run(
         self, ti_key: TaskInstanceKey, operator: BaseOperator, log: logging.Logger
     ) -> str:
         task_group = get_task_group(operator)
         dag = _get_flask_app().dag_bag.get_dag(ti_key.dag_id)
         dr = _get_dagrun(dag, ti_key.run_id)
         log.debug("Getting failed and skipped tasks for dag run %s", dr.run_id)
+        task_group_sub_tasks = self.get_task_group_children(task_group).items()
         failed_and_skipped_tasks = self._get_failed_and_skipped_tasks(dr)
         log.debug("Failed and skipped tasks: %s", failed_and_skipped_tasks)
+
         tasks_to_run = {
             ti: t
-            for ti, t in task_group.children.items()
+            for ti, t in task_group_sub_tasks
             if ti in failed_and_skipped_tasks
         }
         log.debug(
             "Tasks to repair in databricks job %s : %s",
             task_group.group_id,
             tasks_to_run,
         )
         tasks_str = ",".join(
             get_databricks_task_ids(task_group.group_id, tasks_to_run, log)
         )
+
         return tasks_str
 
     def _get_failed_and_skipped_tasks(self, dr: DagRun) -> list[str]:
         """
         Returns a list of task IDs for tasks that have failed or have been skipped in the given DagRun.
 
         :param dr: The DagRun object for which to retrieve failed and skipped tasks.
@@ -399,15 +436,15 @@
             task_group.group_id,
             ti_key.task_id,
         )
         dag = _get_flask_app().dag_bag.get_dag(ti_key.dag_id)
         task = dag.get_task(ti_key.task_id)
         # Should we catch the exception here if there is no return value?
         if ".launch" not in ti_key.task_id:
-            launch_task_id = task_group.get_child_by_label("launch").task_id
+            launch_task_id = get_launch_task_id(task_group)
             ti_key = _get_launch_task_key(ti_key, task_id=launch_task_id)
         metadata = get_xcom_result(ti_key, "return_value", ti)
 
         return (
             f"/repair_databricks_job?dag_id={ti_key.dag_id}&"
             f"databricks_conn_id={metadata.databricks_conn_id}&"
             f"databricks_run_id={metadata.databricks_run_id}&"
@@ -434,14 +471,15 @@
         run_id = request.values.get("run_id").replace(
             " ", "+"
         )  # get run id separately since we need to modify it
         if tasks_to_repair == "":
             # If there are no tasks to repair, we return.
             flash("No tasks to repair. Not sending repair request.")
             return redirect(return_url)
+        self.log.info("Tasks to repair: %s", tasks_to_repair)
         self.log.info("Repairing databricks job %s", databricks_run_id)
         res = _repair_task(
             databricks_conn_id=databricks_conn_id,
             databricks_run_id=databricks_run_id,
             tasks_to_repair=tasks_to_repair.split(","),
             log=self.log,
         )
```

### Comparing `astro_provider_databricks-0.1.3a2/tests/conftest.py` & `astro_provider_databricks-0.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/tests/test_example_dags.py` & `astro_provider_databricks-0.1.4/tests/test_example_dags.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/tests/utils.py` & `astro_provider_databricks-0.1.4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/tests/databricks/test_notebook.py` & `astro_provider_databricks-0.1.4/tests/databricks/test_notebook.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/tests/databricks/test_plugin.py` & `astro_provider_databricks-0.1.4/tests/databricks/test_plugin.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,35 @@
 from unittest.mock import MagicMock, patch
 
 import pytest
 from airflow import DAG
 from airflow.models.dagbag import DagBag
 from airflow.models.dagrun import DagRun
 from airflow.models.taskinstance import TaskInstanceKey
+from airflow.operators.dummy import DummyOperator
 from airflow.providers.databricks.hooks.databricks import DatabricksHook
 from airflow.utils.dates import days_ago
 from airflow.utils.db import create_session
 from airflow.utils.state import State
+from airflow.utils.task_group import TaskGroup
+from databricks_cli.sdk.service import JobsService
+
+
+from astro_databricks.operators.notebook import DatabricksNotebookOperator
+from astro_databricks.operators.workflow import DatabricksWorkflowTaskGroup
 from astro_databricks.plugins.plugin import (
     DatabricksJobRepairAllFailedLink,
     DatabricksJobRepairSingleFailedLink,
     DatabricksJobRunLink,
     _clear_task_instances,
     _get_dagrun,
     _get_databricks_task_id,
     _repair_task,
+    get_launch_task_id
 )
-from databricks_cli.sdk.service import JobsService
-
 
 @pytest.fixture
 def mock_dag():
     dag = MagicMock(spec=DAG)
     dag.dag_id = "my_dag"
     dag.get_task.return_value = MagicMock(
         task_group=MagicMock(
@@ -329,7 +335,87 @@
 
     mock_xcom = MagicMock()
     mock_xcom.get_value.return_value = metadata
 
     with patch("astro_databricks.plugins.plugin.XCom", mock_xcom):
         link.get_link(mock_task, dttm=None, ti_key=ti_key)
         f"/repair_databricks_job?dag_id={dag_id}&databricks_conn_id={databricks_conn_id}&databricks_run_id={databricks_run_id}&tasks_to_repair={_get_databricks_task_id(mock_task)}"
+
+
+@mock.patch("astro_databricks.operators.workflow.DatabricksHook")
+@mock.patch("astro_databricks.operators.workflow.ApiClient")
+@mock.patch("astro_databricks.operators.workflow.JobsApi")
+@mock.patch("astro_databricks.operators.workflow._get_job_by_name")
+@mock.patch(
+    "astro_databricks.operators.workflow.RunsApi.get_run",
+    return_value={"state": {"life_cycle_state": "RUNNING"}},
+)
+def test_create_workflow_with_nested_task_groups(
+    mock_run_api, mock_get_jobs, mock_jobs_api, mock_api, mock_hook, dag
+):
+    mock_get_jobs.return_value = {"job_id": 862519602273592}
+
+    extra_job_params = {
+        "timeout_seconds": 10,  # default: 0
+        "webhook_notifications": {
+            "on_failure": [{"id": "b0aea8ab-ea8c-4a45-a2e9-9a26753fd702"}],
+        },
+        "email_notifications": {
+            "no_alert_for_skipped_runs": True,  # default: False
+            "on_start": ["user.name@databricks.com"],
+        },
+        "git_source": {  # no default value
+            "git_url": "https://github.com/astronomer/astro-provider-databricks",
+            "git_provider": "gitHub",
+            "git_branch": "main",
+        },
+    }
+    with dag:
+        outer_task_group = DatabricksWorkflowTaskGroup(
+            group_id="test_workflow",
+            databricks_conn_id="foo",
+            job_clusters=[{"job_cluster_key": "foo"}],
+            notebook_params={"notebook_path": "/foo/bar"},
+            extra_job_params=extra_job_params,
+            notebook_packages=[
+                {"pypi": {"package": "mlflow==2.4.0"}},
+            ]
+        )
+        with outer_task_group:
+            direct_notebook = DatabricksNotebookOperator(
+                task_id="direct_notebook",
+                databricks_conn_id="foo",
+                notebook_path="/foo/bar",
+                source="WORKSPACE",
+                job_cluster_key="foo",
+            )
+
+            with TaskGroup("middle_task_group") as middle_task_group:
+                with TaskGroup("inner_task_group") as inner_task_group:
+                    inner_notebook = DatabricksNotebookOperator(
+                        task_id="inner_notebook",
+                        databricks_conn_id="foo",
+                        notebook_path="/foo/bar",
+                        source="WORKSPACE",
+                        job_cluster_key="foo",
+                    )
+                    inner_notebook
+                inner_task_group
+            direct_notebook >> middle_task_group
+
+    task_id = get_launch_task_id(outer_task_group)
+    assert task_id == "test_workflow.launch"
+
+def test_get_task_group_children(dag):
+    repair_all_link = DatabricksJobRepairAllFailedLink()
+    with dag:
+        with TaskGroup("parent_task_group") as parent_task_group:
+            parent_task = DummyOperator(task_id="parent_task")
+            with TaskGroup("inner_task_group") as inner_task_group:
+                inner_task = DummyOperator(task_id="inner_task")
+            parent_task >> inner_task_group
+
+    children = repair_all_link.get_task_group_children(parent_task_group)
+    children_keys = children.keys()
+    assert len(children_keys) == 2
+    assert 'parent_task_group.parent_task' in children_keys
+    assert 'parent_task_group.inner_task_group.inner_task' in children_keys
```

### Comparing `astro_provider_databricks-0.1.3a2/tests/databricks/test_workflow.py` & `astro_provider_databricks-0.1.4/tests/databricks/test_workflow.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import logging
 from unittest import mock
 
 import pytest
 from airflow.exceptions import AirflowException
+from airflow.utils.task_group import TaskGroup
 from astro_databricks.operators.notebook import DatabricksNotebookOperator
 from astro_databricks.operators.workflow import DatabricksWorkflowTaskGroup
 
 expected_workflow_json = {
     "name": "unit_test_dag.test_workflow",
     "email_notifications": {"no_alert_for_skipped_runs": False},
     "format": "MULTI_TASK",
@@ -282,7 +283,158 @@
         kwargs["new_settings"]["webhook_notifications"]
         == extra_job_params["webhook_notifications"]
     )
     assert (
         kwargs["new_settings"]["email_notifications"]
         == extra_job_params["email_notifications"]
     )
+
+
+@mock.patch("astro_databricks.operators.workflow.DatabricksHook")
+@mock.patch("astro_databricks.operators.workflow.ApiClient")
+@mock.patch("astro_databricks.operators.workflow.JobsApi")
+@mock.patch("astro_databricks.operators.workflow._get_job_by_name")
+@mock.patch(
+    "astro_databricks.operators.workflow.RunsApi.get_run",
+    return_value={"state": {"life_cycle_state": "RUNNING"}},
+)
+def test_create_workflow_with_arbitrary_extra_job_params(
+    mock_run_api, mock_get_jobs, mock_jobs_api, mock_api, mock_hook, dag
+):
+    mock_get_jobs.return_value = {"job_id": 862519602273592}
+
+    extra_job_params = {
+        "timeout_seconds": 10,  # default: 0
+        "webhook_notifications": {
+            "on_failure": [{"id": "b0aea8ab-ea8c-4a45-a2e9-9a26753fd702"}],
+        },
+        "email_notifications": {
+            "no_alert_for_skipped_runs": True,  # default: False
+            "on_start": ["user.name@databricks.com"],
+        },
+        "git_source": {  # no default value
+            "git_url": "https://github.com/astronomer/astro-provider-databricks",
+            "git_provider": "gitHub",
+            "git_branch": "main",
+        },
+    }
+    with dag:
+        task_group = DatabricksWorkflowTaskGroup(
+            group_id="test_workflow",
+            databricks_conn_id="foo",
+            job_clusters=[{"job_cluster_key": "foo"}],
+            notebook_params={"notebook_path": "/foo/bar"},
+            extra_job_params=extra_job_params,
+        )
+        with task_group:
+            notebook_with_extra = DatabricksNotebookOperator(
+                task_id="notebook_with_extra",
+                databricks_conn_id="foo",
+                notebook_path="/foo/bar",
+                source="WORKSPACE",
+                job_cluster_key="foo",
+            )
+            notebook_with_extra
+
+    assert len(task_group.children) == 2
+
+    task_group.children["test_workflow.launch"].create_workflow_json()
+    task_group.children["test_workflow.launch"].execute(context={})
+
+    mock_jobs_api.return_value.reset_job.assert_called_once()
+    kwargs = mock_jobs_api.return_value.reset_job.call_args_list[0].kwargs["json"]
+
+    assert kwargs["job_id"] == 862519602273592
+    assert (
+        kwargs["new_settings"]["email_notifications"]
+        == extra_job_params["email_notifications"]
+    )
+    assert (
+        kwargs["new_settings"]["timeout_seconds"] == extra_job_params["timeout_seconds"]
+    )
+    assert kwargs["new_settings"]["git_source"] == extra_job_params["git_source"]
+    assert (
+        kwargs["new_settings"]["webhook_notifications"]
+        == extra_job_params["webhook_notifications"]
+    )
+    assert (
+        kwargs["new_settings"]["email_notifications"]
+        == extra_job_params["email_notifications"]
+    )
+
+
+@mock.patch("astro_databricks.operators.workflow.DatabricksHook")
+@mock.patch("astro_databricks.operators.workflow.ApiClient")
+@mock.patch("astro_databricks.operators.workflow.JobsApi")
+@mock.patch("astro_databricks.operators.workflow._get_job_by_name")
+@mock.patch(
+    "astro_databricks.operators.workflow.RunsApi.get_run",
+    return_value={"state": {"life_cycle_state": "RUNNING"}},
+)
+def test_create_workflow_with_nested_task_groups(
+    mock_run_api, mock_get_jobs, mock_jobs_api, mock_api, mock_hook, dag
+):
+    mock_get_jobs.return_value = {"job_id": 862519602273592}
+
+    extra_job_params = {
+        "timeout_seconds": 10,  # default: 0
+        "webhook_notifications": {
+            "on_failure": [{"id": "b0aea8ab-ea8c-4a45-a2e9-9a26753fd702"}],
+        },
+        "email_notifications": {
+            "no_alert_for_skipped_runs": True,  # default: False
+            "on_start": ["user.name@databricks.com"],
+        },
+        "git_source": {  # no default value
+            "git_url": "https://github.com/astronomer/astro-provider-databricks",
+            "git_provider": "gitHub",
+            "git_branch": "main",
+        },
+    }
+    with dag:
+        outer_task_group = DatabricksWorkflowTaskGroup(
+            group_id="test_workflow",
+            databricks_conn_id="foo",
+            job_clusters=[{"job_cluster_key": "foo"}],
+            notebook_params={"notebook_path": "/foo/bar"},
+            extra_job_params=extra_job_params,
+            notebook_packages=[
+                {"pypi": {"package": "mlflow==2.4.0"}},
+            ]
+        )
+        with outer_task_group:
+            direct_notebook = DatabricksNotebookOperator(
+                task_id="direct_notebook",
+                databricks_conn_id="foo",
+                notebook_path="/foo/bar",
+                source="WORKSPACE",
+                job_cluster_key="foo",
+            )
+
+            with TaskGroup("middle_task_group") as middle_task_group:
+                with TaskGroup("inner_task_group") as inner_task_group:
+                    inner_notebook = DatabricksNotebookOperator(
+                        task_id="inner_notebook",
+                        databricks_conn_id="foo",
+                        notebook_path="/foo/bar",
+                        source="WORKSPACE",
+                        job_cluster_key="foo",
+                    )
+                    inner_notebook
+                inner_task_group
+            direct_notebook >> middle_task_group
+
+    assert len(outer_task_group.children) == 3
+
+    outer_task_group.children["test_workflow.launch"].create_workflow_json()
+    outer_task_group.children["test_workflow.launch"].execute(context={})
+
+    kwargs = mock_jobs_api.return_value.reset_job.call_args_list[0].kwargs["json"]
+
+    inner_notebook_json = kwargs["new_settings"]["tasks"][0]
+    outer_notebook_json = kwargs["new_settings"]["tasks"][1]
+
+    assert inner_notebook_json["task_key"] == "unit_test_dag__test_workflow__direct_notebook"
+    assert inner_notebook_json["libraries"] == [{"pypi": {"package": "mlflow==2.4.0"}}]
+
+    assert outer_notebook_json["task_key"] == "unit_test_dag__test_workflow__middle_task_group__inner_task_group__inner_notebook"
+    assert outer_notebook_json["libraries"] == [{"pypi": {"package": "mlflow==2.4.0"}}]
```

### Comparing `astro_provider_databricks-0.1.3a2/.gitignore` & `astro_provider_databricks-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/LICENSE` & `astro_provider_databricks-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.3a2/pyproject.toml` & `astro_provider_databricks-0.1.4/pyproject.toml`

 * *Files identical despite different names*

