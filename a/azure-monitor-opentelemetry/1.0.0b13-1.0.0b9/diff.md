# Comparing `tmp/azure-monitor-opentelemetry-1.0.0b13.tar.gz` & `tmp/azure-monitor-opentelemetry-1.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/ApplicationInsights-Python/ApplicationInsights-Python/dist/azure-monitor-opentelemetry-1.0.0b13.tar", last modified: Fri Jun 16 17:38:05 2023, max compression
+gzip compressed data, was "azure-monitor-opentelemetry-1.0.0b9.tar", last modified: Wed Feb 22 22:31:32 2023, max compression
```

## Comparing `azure-monitor-opentelemetry-1.0.0b13.tar` & `azure-monitor-opentelemetry-1.0.0b9.tar`

### file list

```diff
@@ -1,167 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/asgi/
--rw-r--r--   0 runner    (1001) docker     (123)    18329 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/asgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/asgi/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/asgi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/auto_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/auto_instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/auto_instrumentation/sitecustomize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/bootstrap_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/dbapi/
--rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/dbapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/dbapi/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/dbapi/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/distro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/django/
--rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/django/environment_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/django/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/django/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15399 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/django/middleware/otel_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/django/middleware/sqlcommenter_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/django/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/django/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/environment_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/fastapi/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/fastapi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/flask/
--rw-r--r--   0 runner    (1001) docker     (123)    16559 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/flask/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/flask/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/instrumentor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/propagators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/psycopg2/
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/psycopg2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/psycopg2/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/psycopg2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/requests/
--rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/requests/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/requests/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/sqlcommenter_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/urllib/
--rw-r--r--   0 runner    (1001) docker     (123)     9210 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/urllib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/urllib/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/urllib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/urllib3/
--rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/urllib3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/urllib3/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/urllib3/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/wsgi/
--rw-r--r--   0 runner    (1001) docker     (123)    14322 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/wsgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/wsgi/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/instrumentation/wsgi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/util/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/util/http/
--rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/util/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/util/http/httplib.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_vendor/v0_38b0/opentelemetry/util/http/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/autoinstrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/autoinstrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/autoinstrumentation/_configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/autoinstrumentation/_distro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/diagnostics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/diagnostics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/diagnostics/_diagnostic_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/diagnostics/_status_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/util/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/util/configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure_monitor_opentelemetry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure_monitor_opentelemetry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure_monitor_opentelemetry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure_monitor_opentelemetry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure_monitor_opentelemetry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure_monitor_opentelemetry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure_monitor_opentelemetry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/azure_monitor_opentelemetry.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/samples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/samples/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/logging/correlated_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/logging/custom_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/logging/exception_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/logging/logs_with_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/logging/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/samples/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/metrics/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/metrics/instruments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/db_psycopg2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/django/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/django/sample/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/django/sample/example/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/django/sample/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/django/sample/example/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/django/sample/example/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/django/sample/example/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/django/sample/example/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/django/sample/example/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/django/sample/example/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/django/sample/example/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/django/sample/example/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/django/sample/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/django/sample/sample/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/django/sample/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/django/sample/sample/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/django/sample/sample/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/django/sample/sample/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/django/sample/sample/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/http_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/http_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/http_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/http_urllib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/http_urllib3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/manual.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/samples/tracing/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/tests/autoinstrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/tests/autoinstrumentation/test_distro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/tests/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/tests/configuration/test_configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/tests/configuration/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/tests/diagnostics/
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/tests/diagnostics/test_diagnostic_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/tests/diagnostics/test_status_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/tests/exporter/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/tests/exporter/test_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:05.000000 azure-monitor-opentelemetry-1.0.0b13/tests/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/tests/instrumentation/test_django.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/tests/instrumentation/test_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/tests/instrumentation/test_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/tests/instrumentation/test_psycopg2.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/tests/instrumentation/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/tests/instrumentation/test_urllib.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/tests/instrumentation/test_urllib3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-06-16 17:37:59.000000 azure-monitor-opentelemetry-1.0.0b13/tests/test_constants.py
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.179282 azure-monitor-opentelemetry-1.0.0b9/
+-rw-rw-rw-   0        0        0     9608 2023-02-22 22:31:32.180284 azure-monitor-opentelemetry-1.0.0b9/PKG-INFO
+-rw-rw-rw-   0        0        0     8745 2023-02-22 22:28:31.000000 azure-monitor-opentelemetry-1.0.0b9/README.md
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.049037 azure-monitor-opentelemetry-1.0.0b9/azure/
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.050037 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.080216 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/
+-rw-rw-rw-   0        0        0      494 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/__init__.py
+-rw-rw-rw-   0        0        0     9163 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/_configure.py
+-rw-rw-rw-   0        0        0     2299 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/_constants.py
+-rw-rw-rw-   0        0        0      734 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/_types.py
+-rw-rw-rw-   0        0        0      334 2023-02-22 22:28:31.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/_version.py
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.094215 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/autoinstrumentation/
+-rw-rw-rw-   0        0        0      310 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/autoinstrumentation/__init__.py
+-rw-rw-rw-   0        0        0     1125 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/autoinstrumentation/_configurator.py
+-rw-rw-rw-   0        0        0     2984 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/autoinstrumentation/_distro.py
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.107694 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/diagnostics/
+-rw-rw-rw-   0        0        0        0 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/diagnostics/__init__.py
+-rw-rw-rw-   0        0        0     3209 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/diagnostics/_diagnostic_logging.py
+-rw-rw-rw-   0        0        0     1987 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/diagnostics/_status_logger.py
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.112712 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/util/
+-rw-rw-rw-   0        0        0      647 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.175279 azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/
+-rw-rw-rw-   0        0        0     9608 2023-02-22 22:31:31.000000 azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1014 2023-02-22 22:31:31.000000 azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-22 22:31:31.000000 azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      295 2023-02-22 22:31:31.000000 azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-02-22 21:49:02.000000 azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      320 2023-02-22 22:31:31.000000 azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-02-22 22:31:31.000000 azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2023-02-22 22:31:32.195109 azure-monitor-opentelemetry-1.0.0b9/setup.cfg
+-rw-rw-rw-   0        0        0     3587 2023-02-22 22:28:31.000000 azure-monitor-opentelemetry-1.0.0b9/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.178279 azure-monitor-opentelemetry-1.0.0b9/tests/
+-rw-rw-rw-   0        0        0     5452 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/tests/test_constants.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/_types.py` & `azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/_types.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# -------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License in the project root for
-# license information.
-# --------------------------------------------------------------------------
-
-from typing import Sequence, Union
-
-from opentelemetry.sdk.metrics.export import MetricReader
-from opentelemetry.sdk.metrics.view import View
-from opentelemetry.sdk.resources import Resource
-
-ConfigurationValue = Union[
-    str,
-    bool,
-    int,
-    float,
-    Resource,
-    Sequence[str],
-    Sequence[bool],
-    Sequence[int],
-    Sequence[float],
-    Sequence[MetricReader],
-    Sequence[View],
-]
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License. See License in the project root for
+# license information.
+# --------------------------------------------------------------------------
+
+from typing import Sequence, Union
+
+from opentelemetry.sdk.metrics.export import MetricReader
+from opentelemetry.sdk.metrics.view import View
+from opentelemetry.sdk.resources import Resource
+
+ConfigurationValue = Union[
+    str,
+    bool,
+    int,
+    float,
+    Resource,
+    Sequence[str],
+    Sequence[bool],
+    Sequence[int],
+    Sequence[float],
+    Sequence[MetricReader],
+    Sequence[View],
+]
```

### Comparing `azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/autoinstrumentation/_distro.py` & `azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/autoinstrumentation/_distro.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-# -------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License in the project root for
-# license information.
-# --------------------------------------------------------------------------
-import logging
-from os import environ
-
-from azure.monitor.opentelemetry._vendor.v0_38b0.opentelemetry.instrumentation.distro import (
-    BaseDistro,
-)
-from azure.monitor.opentelemetry.diagnostics._diagnostic_logging import (
-    AzureDiagnosticLogging,
-)
-from azure.monitor.opentelemetry.diagnostics._status_logger import (
-    AzureStatusLogger,
-)
-from opentelemetry.environment_variables import (
-    OTEL_LOGS_EXPORTER,
-    OTEL_METRICS_EXPORTER,
-    OTEL_TRACES_EXPORTER,
-)
-from opentelemetry.sdk.environment_variables import (
-    _OTEL_PYTHON_LOGGING_AUTO_INSTRUMENTATION_ENABLED,
-)
-
-_logger = logging.getLogger(__name__)
-_opentelemetry_logger = logging.getLogger("opentelemetry")
-# TODO: Enabled when duplicate logging issue is solved
-# _exporter_logger = logging.getLogger("azure.monitor.opentelemetry.exporter")
-
-
-class AzureMonitorDistro(BaseDistro):
-    def _configure(self, **kwargs) -> None:
-        try:
-            _configure_auto_instrumentation()
-        except Exception as ex:
-            _logger.exception(
-                ("Error occurred auto-instrumenting AzureMonitorDistro")
-            )
-            raise ex
-
-
-def _configure_auto_instrumentation() -> None:
-    try:
-        AzureStatusLogger.log_status(False, "Distro being configured.")
-        AzureDiagnosticLogging.enable(_logger)
-        AzureDiagnosticLogging.enable(_opentelemetry_logger)
-        # TODO: Enabled when duplicate logging issue is solved
-        # if _EXPORTER_DIAGNOSTICS_ENABLED:
-        #     exporter_logger = logging.getLogger(
-        #         "azure.monitor.opentelemetry.exporter"
-        #     )
-        #     AzureDiagnosticLogging.enable(_exporter_logger)
-        environ.setdefault(
-            OTEL_METRICS_EXPORTER, "azure_monitor_opentelemetry_exporter"
-        )
-        environ.setdefault(
-            OTEL_TRACES_EXPORTER, "azure_monitor_opentelemetry_exporter"
-        )
-        environ.setdefault(
-            OTEL_LOGS_EXPORTER, "azure_monitor_opentelemetry_exporter"
-        )
-        environ.setdefault(
-            _OTEL_PYTHON_LOGGING_AUTO_INSTRUMENTATION_ENABLED, "true"
-        )
-        AzureStatusLogger.log_status(True)
-        _logger.info(
-            "Azure Monitor OpenTelemetry Distro configured successfully."
-        )
-    except Exception as exc:
-        AzureStatusLogger.log_status(False, reason=exc)
-        _logger.error(
-            "Azure Monitor OpenTelemetry Distro failed during "
-            + "configuration: %s",
-            exc,
-        )
-        raise exc
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License. See License in the project root for
+# license information.
+# --------------------------------------------------------------------------
+import logging
+from os import environ
+
+from azure.monitor.opentelemetry.diagnostics._diagnostic_logging import (
+    AzureDiagnosticLogging,
+)
+from azure.monitor.opentelemetry.diagnostics._status_logger import (
+    AzureStatusLogger,
+)
+from opentelemetry.environment_variables import (
+    OTEL_LOGS_EXPORTER,
+    OTEL_METRICS_EXPORTER,
+    OTEL_TRACES_EXPORTER,
+)
+from opentelemetry.instrumentation.distro import BaseDistro
+from opentelemetry.sdk.environment_variables import (
+    _OTEL_PYTHON_LOGGING_AUTO_INSTRUMENTATION_ENABLED,
+)
+
+_logger = logging.getLogger(__name__)
+_opentelemetry_logger = logging.getLogger("opentelemetry")
+# TODO: Enabled when duplicate logging issue is solved
+# _exporter_logger = logging.getLogger("azure.monitor.opentelemetry.exporter")
+
+
+class AzureMonitorDistro(BaseDistro):
+    def _configure(self, **kwargs) -> None:
+        try:
+            _configure_auto_instrumentation()
+        except Exception as ex:
+            _logger.exception(
+                ("Error occured auto-instrumenting AzureMonitorDistro")
+            )
+            raise ex
+
+
+def _configure_auto_instrumentation() -> None:
+    try:
+        AzureStatusLogger.log_status(False, "Distro being configured.")
+        AzureDiagnosticLogging.enable(_logger)
+        AzureDiagnosticLogging.enable(_opentelemetry_logger)
+        # TODO: Enabled when duplicate logging issue is solved
+        # if _EXPORTER_DIAGNOSTICS_ENABLED:
+        #     exporter_logger = logging.getLogger(
+        #         "azure.monitor.opentelemetry.exporter"
+        #     )
+        #     AzureDiagnosticLogging.enable(_exporter_logger)
+        # TODO: Uncomment when logging is out of preview
+        # environ.setdefault(OTEL_LOGS_EXPORTER,
+        #     "azure_monitor_opentelemetry_exporter")
+        environ.setdefault(
+            OTEL_METRICS_EXPORTER, "azure_monitor_opentelemetry_exporter"
+        )
+        environ.setdefault(
+            OTEL_TRACES_EXPORTER, "azure_monitor_opentelemetry_exporter"
+        )
+        environ.setdefault(
+            OTEL_LOGS_EXPORTER, "azure_monitor_opentelemetry_exporter"
+        )
+        environ.setdefault(
+            _OTEL_PYTHON_LOGGING_AUTO_INSTRUMENTATION_ENABLED, "true"
+        )
+        AzureStatusLogger.log_status(True)
+        _logger.info(
+            "Azure Monitor OpenTelemetry Distro configured successfully."
+        )
+    except Exception as exc:
+        AzureStatusLogger.log_status(False, reason=exc)
+        _logger.error(
+            "Azure Monitor OpenTelemetry Distro failed during "
+            + f"configuration: {exc}"
+        )
+        raise exc
```

### Comparing `azure-monitor-opentelemetry-1.0.0b13/azure/monitor/opentelemetry/diagnostics/_status_logger.py` & `azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/diagnostics/_status_logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,54 @@
-# -------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License in the project root for
-# license information.
-# --------------------------------------------------------------------------
-
-from json import dumps
-from os import getpid, makedirs
-from os.path import exists, join
-from platform import node
-
-from azure.monitor.opentelemetry._constants import (
-    _CUSTOMER_IKEY,
-    _EXTENSION_VERSION,
-    _IS_DIAGNOSTICS_ENABLED,
-    _get_log_path,
-)
-from azure.monitor.opentelemetry._version import VERSION
-
-_MACHINE_NAME = node()
-_STATUS_LOG_PATH = _get_log_path(status_log_path=True)
-
-
-class AzureStatusLogger:
-    @classmethod
-    def _get_status_json(
-        cls, agent_initialized_successfully, pid, reason=None
-    ):
-        status_json = {
-            "AgentInitializedSuccessfully": agent_initialized_successfully,
-            "AppType": "python",
-            "MachineName": _MACHINE_NAME,
-            "PID": pid,
-            "SdkVersion": VERSION,
-            "Ikey": _CUSTOMER_IKEY,
-            "ExtensionVersion": _EXTENSION_VERSION,
-        }
-        if reason:
-            status_json["Reason"] = reason
-        return status_json
-
-    @classmethod
-    def log_status(cls, agent_initialized_successfully, reason=None):
-        if _IS_DIAGNOSTICS_ENABLED and _STATUS_LOG_PATH:
-            pid = getpid()
-            status_json = AzureStatusLogger._get_status_json(
-                agent_initialized_successfully, pid, reason
-            )
-            if not exists(_STATUS_LOG_PATH):
-                makedirs(_STATUS_LOG_PATH)
-            # Change to be hostname and pid
-            status_logger_file_name = f"status_{_MACHINE_NAME}_{pid}.json"
-            with open(
-                join(_STATUS_LOG_PATH, status_logger_file_name), "w"
-            ) as f:
-                f.seek(0)
-                f.write(dumps(status_json))
-                f.truncate()
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License. See License in the project root for
+# license information.
+# --------------------------------------------------------------------------
+
+from json import dumps
+from os import getpid, makedirs
+from os.path import exists, join
+from platform import node
+
+from azure.monitor.opentelemetry._constants import (
+    _CUSTOMER_IKEY,
+    _EXTENSION_VERSION,
+    _IS_DIAGNOSTICS_ENABLED,
+    _get_log_path,
+)
+from azure.monitor.opentelemetry._version import VERSION
+
+_MACHINE_NAME = node()
+_STATUS_LOG_PATH = _get_log_path(status_log_path=True)
+
+
+class AzureStatusLogger:
+    def _get_status_json(agent_initialized_successfully, pid, reason=None):
+        status_json = {
+            "AgentInitializedSuccessfully": agent_initialized_successfully,
+            "AppType": "python",
+            "MachineName": _MACHINE_NAME,
+            "PID": pid,
+            "SdkVersion": VERSION,
+            "Ikey": _CUSTOMER_IKEY,
+            "ExtensionVersion": _EXTENSION_VERSION,
+        }
+        if reason:
+            status_json["Reason"] = reason
+        return status_json
+
+    def log_status(agent_initialized_successfully, reason=None):
+        if _IS_DIAGNOSTICS_ENABLED and _STATUS_LOG_PATH:
+            pid = getpid()
+            status_json = AzureStatusLogger._get_status_json(
+                agent_initialized_successfully, pid, reason
+            )
+            if not exists(_STATUS_LOG_PATH):
+                makedirs(_STATUS_LOG_PATH)
+            # Change to be hostname and pid
+            status_logger_file_name = f"status_{_MACHINE_NAME}_{pid}.json"
+            with open(
+                join(_STATUS_LOG_PATH, status_logger_file_name), "w"
+            ) as f:
+                f.seek(0)
+                f.write(dumps(status_json))
+                f.truncate()
```

### Comparing `azure-monitor-opentelemetry-1.0.0b13/azure_monitor_opentelemetry.egg-info/entry_points.txt` & `azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,23 @@
-[azure_monitor_opentelemetry_instrumentor]
-django = azure.monitor.opentelemetry._vendor.v0_38b0.opentelemetry.instrumentation.django:DjangoInstrumentor
-fastapi = azure.monitor.opentelemetry._vendor.v0_38b0.opentelemetry.instrumentation.fastapi:FastAPIInstrumentor
-flask = azure.monitor.opentelemetry._vendor.v0_38b0.opentelemetry.instrumentation.flask:FlaskInstrumentor
-psycopg2 = azure.monitor.opentelemetry._vendor.v0_38b0.opentelemetry.instrumentation.psycopg2:Psycopg2Instrumentor
-requests = azure.monitor.opentelemetry._vendor.v0_38b0.opentelemetry.instrumentation.requests:RequestsInstrumentor
-urllib = azure.monitor.opentelemetry._vendor.v0_38b0.opentelemetry.instrumentation.urllib:URLLibInstrumentor
-urllib3 = azure.monitor.opentelemetry._vendor.v0_38b0.opentelemetry.instrumentation.urllib3:URLLib3Instrumentor
-
-[opentelemetry_configurator]
-azure_monitor_opentelemetry_configurator = azure.monitor.opentelemetry.autoinstrumentation._configurator:AzureMonitorConfigurator
-
-[opentelemetry_distro]
-azure_monitor_opentelemetry_distro = azure.monitor.opentelemetry.autoinstrumentation._distro:AzureMonitorDistro
+README.md
+setup.cfg
+setup.py
+azure/monitor/opentelemetry/__init__.py
+azure/monitor/opentelemetry/_configure.py
+azure/monitor/opentelemetry/_constants.py
+azure/monitor/opentelemetry/_types.py
+azure/monitor/opentelemetry/_version.py
+azure/monitor/opentelemetry/autoinstrumentation/__init__.py
+azure/monitor/opentelemetry/autoinstrumentation/_configurator.py
+azure/monitor/opentelemetry/autoinstrumentation/_distro.py
+azure/monitor/opentelemetry/diagnostics/__init__.py
+azure/monitor/opentelemetry/diagnostics/_diagnostic_logging.py
+azure/monitor/opentelemetry/diagnostics/_status_logger.py
+azure/monitor/opentelemetry/util/__init__.py
+azure_monitor_opentelemetry.egg-info/PKG-INFO
+azure_monitor_opentelemetry.egg-info/SOURCES.txt
+azure_monitor_opentelemetry.egg-info/dependency_links.txt
+azure_monitor_opentelemetry.egg-info/entry_points.txt
+azure_monitor_opentelemetry.egg-info/not-zip-safe
+azure_monitor_opentelemetry.egg-info/requires.txt
+azure_monitor_opentelemetry.egg-info/top_level.txt
+tests/test_constants.py
```

### Comparing `azure-monitor-opentelemetry-1.0.0b13/tests/test_constants.py` & `azure-monitor-opentelemetry-1.0.0b9/tests/test_constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,149 +1,149 @@
-# -------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License in the project root for
-# license information.
-# --------------------------------------------------------------------------
-
-from importlib import reload
-from os import environ
-from unittest import TestCase
-from unittest.mock import patch
-
-from azure.monitor.opentelemetry import _constants
-
-TEST_VALUE = "TEST_VALUE"
-TEST_IKEY = "1234abcd-ab12-34cd-ab12-a23456abcdef"
-TEST_CONN_STR = f"InstrumentationKey={TEST_IKEY};IngestionEndpoint=https://centralus-2.in.applicationinsights.azure.com/;LiveEndpoint=https://centralus.livediagnostics.monitor.azure.com/"
-
-
-def clear_env_var(env_var):
-    if env_var in environ:
-        del environ[env_var]
-
-
-class TestConstants(TestCase):
-    @patch.dict(
-        "os.environ",
-        {"ApplicationInsightsAgent_EXTENSION_VERSION": TEST_VALUE},
-    )
-    def test_extension_version(self):
-        reload(_constants)
-        self.assertEqual(_constants._EXTENSION_VERSION, TEST_VALUE)
-
-    def test_extension_version_default(self):
-        clear_env_var("ApplicationInsightsAgent_EXTENSION_VERSION")
-        reload(_constants)
-        self.assertEqual(_constants._EXTENSION_VERSION, "disabled")
-
-    @patch.dict(
-        "os.environ", {"APPLICATIONINSIGHTS_CONNECTION_STRING": TEST_CONN_STR}
-    )
-    def test_ikey(self):
-        reload(_constants)
-        self.assertEqual(_constants._CUSTOMER_IKEY, TEST_IKEY)
-
-    def test_ikey_defaults(self):
-        clear_env_var("APPLICATIONINSIGHTS_CONNECTION_STRING")
-        reload(_constants)
-        self.assertEqual(_constants._CUSTOMER_IKEY, "unknown")
-
-    # TODO: Enabled when duplicate logging issue is solved
-    # @patch.dict(
-    #     "os.environ",
-    #     {"AZURE_MONITOR_OPENTELEMETRY_DISTRO_ENABLE_EXPORTER_DIAGNOSTICS": "True"},
-    # )
-    # def test_exporter_diagnostics_enabled(self):
-    #     reload(_constants)
-    #     self.assertTrue(_constants._EXPORTER_DIAGNOSTICS_ENABLED)
-
-    # def test_exporter_diagnostics_disabled(self):
-    #     clear_env_var("AZURE_MONITOR_OPENTELEMETRY_DISTRO_ENABLE_EXPORTER_DIAGNOSTICS")
-    #     reload(_constants)
-    #     self.assertFalse(_constants._EXPORTER_DIAGNOSTICS_ENABLED)
-
-    # @patch.dict(
-    #     "os.environ",
-    #     {"AZURE_MONITOR_OPENTELEMETRY_DISTRO_ENABLE_EXPORTER_DIAGNOSTICS": "foobar"},
-    # )
-    # def test_exporter_diagnostics_other(self):
-    #     reload(_constants)
-    #     self.assertFalse(_constants._EXPORTER_DIAGNOSTICS_ENABLED)
-
-    @patch.dict("os.environ", {"WEBSITE_SITE_NAME": TEST_VALUE})
-    def test_diagnostics_enabled(self):
-        reload(_constants)
-        self.assertTrue(_constants._IS_DIAGNOSTICS_ENABLED)
-
-    def test_diagnostics_disabled(self):
-        clear_env_var("WEBSITE_SITE_NAME")
-        reload(_constants)
-        self.assertFalse(_constants._IS_DIAGNOSTICS_ENABLED)
-
-    @patch(
-        "azure.monitor.opentelemetry._constants.platform.system",
-        return_value="Linux",
-    )
-    def test_log_path_linux(self, mock_system):
-        self.assertEqual(
-            _constants._get_log_path(), "/var/log/applicationinsights"
-        )
-
-    @patch(
-        "azure.monitor.opentelemetry._constants.platform.system",
-        return_value="Linux",
-    )
-    def test_status_log_path_linux(self, mock_system):
-        self.assertEqual(
-            _constants._get_log_path(status_log_path=True),
-            "/var/log/applicationinsights",
-        )
-
-    @patch(
-        "azure.monitor.opentelemetry._constants.platform.system",
-        return_value="Windows",
-    )
-    @patch("pathlib.Path.home", return_value="\\HOME\\DIR")
-    def test_log_path_windows(self, mock_system, mock_home):
-        self.assertEqual(
-            _constants._get_log_path(),
-            "\\HOME\\DIR\\LogFiles\\ApplicationInsights",
-        )
-
-    @patch(
-        "azure.monitor.opentelemetry._constants.platform.system",
-        return_value="Windows",
-    )
-    @patch("pathlib.Path.home", return_value="\\HOME\\DIR")
-    def test_status_log_path_windows(self, mock_system, mock_home):
-        self.assertEqual(
-            _constants._get_log_path(status_log_path=True),
-            "\\HOME\\DIR\\LogFiles\\ApplicationInsights\\status",
-        )
-
-    @patch(
-        "azure.monitor.opentelemetry._constants.platform.system",
-        return_value="Window",
-    )
-    def test_log_path_other(self, mock_platform):
-        self.assertIsNone(_constants._get_log_path())
-
-    @patch(
-        "azure.monitor.opentelemetry._constants.platform.system",
-        return_value="linux",
-    )
-    def test_status_log_path_other(self, mock_platform):
-        self.assertIsNone(_constants._get_log_path(status_log_path=True))
-
-    @patch.dict("os.environ", {"key": "value"})
-    def test_env_var_or_default(self):
-        self.assertEqual(_constants._env_var_or_default("key"), "value")
-
-    @patch.dict("os.environ", {})
-    def test_env_var_or_default_empty(self):
-        self.assertEqual(_constants._env_var_or_default("key"), "")
-
-    @patch.dict("os.environ", {})
-    def test_env_var_or_default_empty_with_defaults(self):
-        self.assertEqual(
-            _constants._env_var_or_default("key", default_val="value"), "value"
-        )
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License. See License in the project root for
+# license information.
+# --------------------------------------------------------------------------
+
+from importlib import reload
+from os import environ
+from unittest import TestCase
+from unittest.mock import patch
+
+from azure.monitor.opentelemetry import _constants
+
+TEST_VALUE = "TEST_VALUE"
+TEST_IKEY = "1234abcd-ab12-34cd-ab12-a23456abcdef"
+TEST_CONN_STR = f"InstrumentationKey={TEST_IKEY};IngestionEndpoint=https://centralus-2.in.applicationinsights.azure.com/;LiveEndpoint=https://centralus.livediagnostics.monitor.azure.com/"
+
+
+def clear_env_var(env_var):
+    if env_var in environ:
+        del environ[env_var]
+
+
+class TestConstants(TestCase):
+    @patch.dict(
+        "os.environ",
+        {"ApplicationInsightsAgent_EXTENSION_VERSION": TEST_VALUE},
+    )
+    def test_extension_version(self):
+        reload(_constants)
+        self.assertEqual(_constants._EXTENSION_VERSION, TEST_VALUE)
+
+    def test_extension_version_default(self):
+        clear_env_var("ApplicationInsightsAgent_EXTENSION_VERSION")
+        reload(_constants)
+        self.assertEqual(_constants._EXTENSION_VERSION, "disabled")
+
+    @patch.dict(
+        "os.environ", {"APPLICATIONINSIGHTS_CONNECTION_STRING": TEST_CONN_STR}
+    )
+    def test_ikey(self):
+        reload(_constants)
+        self.assertEqual(_constants._CUSTOMER_IKEY, TEST_IKEY)
+
+    def test_ikey_defaults(self):
+        clear_env_var("APPLICATIONINSIGHTS_CONNECTION_STRING")
+        reload(_constants)
+        self.assertEqual(_constants._CUSTOMER_IKEY, "unknown")
+
+    # TODO: Enabled when duplciate logging issue is solved
+    # @patch.dict(
+    #     "os.environ",
+    #     {"AZURE_MONITOR_OPENTELEMETRY_DISTRO_ENABLE_EXPORTER_DIAGNOSTICS": "True"},
+    # )
+    # def test_exporter_diagnostics_enabled(self):
+    #     reload(_constants)
+    #     self.assertTrue(_constants._EXPORTER_DIAGNOSTICS_ENABLED)
+
+    # def test_exporter_diagnostics_disabled(self):
+    #     clear_env_var("AZURE_MONITOR_OPENTELEMETRY_DISTRO_ENABLE_EXPORTER_DIAGNOSTICS")
+    #     reload(_constants)
+    #     self.assertFalse(_constants._EXPORTER_DIAGNOSTICS_ENABLED)
+
+    # @patch.dict(
+    #     "os.environ",
+    #     {"AZURE_MONITOR_OPENTELEMETRY_DISTRO_ENABLE_EXPORTER_DIAGNOSTICS": "foobar"},
+    # )
+    # def test_exporter_diagnostics_other(self):
+    #     reload(_constants)
+    #     self.assertFalse(_constants._EXPORTER_DIAGNOSTICS_ENABLED)
+
+    @patch.dict("os.environ", {"WEBSITE_SITE_NAME": TEST_VALUE})
+    def test_diagnostics_enabled(self):
+        reload(_constants)
+        self.assertTrue(_constants._IS_DIAGNOSTICS_ENABLED)
+
+    def test_diagnostics_disabled(self):
+        clear_env_var("WEBSITE_SITE_NAME")
+        reload(_constants)
+        self.assertFalse(_constants._IS_DIAGNOSTICS_ENABLED)
+
+    @patch(
+        "azure.monitor.opentelemetry._constants.platform.system",
+        return_value="Linux",
+    )
+    def test_log_path_linux(self, mock_system):
+        self.assertEqual(
+            _constants._get_log_path(), "/var/log/applicationinsights"
+        )
+
+    @patch(
+        "azure.monitor.opentelemetry._constants.platform.system",
+        return_value="Linux",
+    )
+    def test_status_log_path_linux(self, mock_system):
+        self.assertEqual(
+            _constants._get_log_path(status_log_path=True),
+            "/var/log/applicationinsights",
+        )
+
+    @patch(
+        "azure.monitor.opentelemetry._constants.platform.system",
+        return_value="Windows",
+    )
+    @patch("pathlib.Path.home", return_value="\\HOME\\DIR")
+    def test_log_path_windows(self, mock_system, mock_home):
+        self.assertEqual(
+            _constants._get_log_path(),
+            "\\HOME\\DIR\\LogFiles\\ApplicationInsights",
+        )
+
+    @patch(
+        "azure.monitor.opentelemetry._constants.platform.system",
+        return_value="Windows",
+    )
+    @patch("pathlib.Path.home", return_value="\\HOME\\DIR")
+    def test_status_log_path_windows(self, mock_system, mock_home):
+        self.assertEqual(
+            _constants._get_log_path(status_log_path=True),
+            "\\HOME\\DIR\\LogFiles\\ApplicationInsights\\status",
+        )
+
+    @patch(
+        "azure.monitor.opentelemetry._constants.platform.system",
+        return_value="Window",
+    )
+    def test_log_path_other(self, mock_platform):
+        self.assertIsNone(_constants._get_log_path())
+
+    @patch(
+        "azure.monitor.opentelemetry._constants.platform.system",
+        return_value="linux",
+    )
+    def test_status_log_path_other(self, mock_platform):
+        self.assertIsNone(_constants._get_log_path(status_log_path=True))
+
+    @patch.dict("os.environ", {"key": "value"})
+    def test_env_var_or_default(self):
+        self.assertEqual(_constants._env_var_or_default("key"), "value")
+
+    @patch.dict("os.environ", {})
+    def test_env_var_or_default_empty(self):
+        self.assertEqual(_constants._env_var_or_default("key"), "")
+
+    @patch.dict("os.environ", {})
+    def test_env_var_or_default_empty_with_defaults(self):
+        self.assertEqual(
+            _constants._env_var_or_default("key", default_val="value"), "value"
+        )
```

