# Comparing `tmp/flytekit-1.7.0.tar.gz` & `tmp/flytekit-1.7.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekit-1.7.0.tar", last modified: Wed Jun 14 04:33:19 2023, max compression
+gzip compressed data, was "flytekit-1.7.1b0.tar", last modified: Fri Jun 16 18:14:08 2023, max compression
```

## Comparing `flytekit-1.7.0.tar` & `flytekit-1.7.1b0.tar`

### file list

```diff
@@ -1,254 +1,254 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.741187 flytekit-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-14 04:33:05.000000 flytekit-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-14 04:33:05.000000 flytekit-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-14 04:33:19.741187 flytekit-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-14 04:33:05.000000 flytekit-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.705186 flytekit-1.7.0/flytekit/
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-06-14 04:33:17.000000 flytekit-1.7.0/flytekit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.705186 flytekit-1.7.0/flytekit/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23182 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/bin/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.705186 flytekit-1.7.0/flytekit/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.709186 flytekit-1.7.0/flytekit/clients/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/auth/auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/auth/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/auth/default_html.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/auth/keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/auth/token_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    50793 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/friendly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.709186 flytekit-1.7.0/flytekit/clients/grpc_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/grpc_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/grpc_utils/auth_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28489 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clients/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.709186 flytekit-1.7.0/flytekit/clis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.709186 flytekit-1.7.0/flytekit/clis/flyte_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/flyte_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/flyte_cli/example.config
--rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/flyte_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.713186 flytekit-1.7.0/flytekit/clis/sdk_in_container/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/launchplan.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/pyflyte.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/register.py
--rw-r--r--   0 runner    (1001) docker     (123)    31991 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/clis/sdk_in_container/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.713186 flytekit-1.7.0/flytekit/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    36185 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/configuration/default_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/configuration/feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/configuration/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/configuration/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.717187 flytekit-1.7.0/flytekit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/base_sql_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    31002 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/base_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/class_based_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    36384 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/data_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/dynamic_workflow_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/map_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/mock_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/node_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/pod_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    46442 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/promise.py
--rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/python_auto_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/python_customized_container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/python_function_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/reference_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/shim_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/tracked_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    77072 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/type_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/type_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    41135 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/deck/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/deck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/deck/deck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/deck/html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/deck/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/deck/html/template.html
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/deck/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/exceptions/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/exceptions/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/exceptions/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/extend/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/extend/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extend/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extend/backend/agent_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extend/backend/base_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/cloud_pickle_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/extras/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/pytorch/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/pytorch/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/extras/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/sklearn/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/extras/sqlite3/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/sqlite3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/sqlite3/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/extras/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/tasks/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/extras/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/tensorflow/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/extras/tensorflow/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/image_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/image_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/image_spec/image_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/interaction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/interaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/interaction/parse_stdin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/interfaces/cli_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/interfaces/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/interfaces/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/interfaces/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/interfaces/stats/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/interfaces/stats/taggable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.721186 flytekit-1.7.0/flytekit/lazy_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/lazy_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/lazy_import/lazy_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.725186 flytekit-1.7.0/flytekit/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.725186 flytekit-1.7.0/flytekit/models/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/admin/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/admin/task_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/admin/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/array_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.725186 flytekit-1.7.0/flytekit/models/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/core/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/core/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/core/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/dynamic_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    25993 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/matchable_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/named_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/node_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/presto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/qubole.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/models/workflow_closure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.725186 flytekit-1.7.0/flytekit/remote/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/remote/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/remote/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/remote/executions.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/remote/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/remote/lazy_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    87310 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/remote/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/remote/remote_callable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.725186 flytekit-1.7.0/flytekit/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.733187 flytekit-1.7.0/flytekit/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/tools/fast_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/tools/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/tools/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/tools/module_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/tools/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/tools/script_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/tools/serialize_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/tools/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/tools/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.733187 flytekit-1.7.0/flytekit/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.737187 flytekit-1.7.0/flytekit/types/directory/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/directory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/directory/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.737187 flytekit-1.7.0/flytekit/types/file/
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23925 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/file/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.737187 flytekit-1.7.0/flytekit/types/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/numpy/ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.737187 flytekit-1.7.0/flytekit/types/pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/pickle/pickle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.737187 flytekit-1.7.0/flytekit/types/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/schema/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/schema/types_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.741187 flytekit-1.7.0/flytekit/types/structured/
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/structured/basic_dfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/structured/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    44541 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit/types/structured/structured_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.705186 flytekit-1.7.0/flytekit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-14 04:33:19.000000 flytekit-1.7.0/flytekit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-06-14 04:33:19.000000 flytekit-1.7.0/flytekit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 04:33:19.000000 flytekit-1.7.0/flytekit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-14 04:33:19.000000 flytekit-1.7.0/flytekit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-14 04:33:19.000000 flytekit-1.7.0/flytekit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 04:33:19.000000 flytekit-1.7.0/flytekit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:19.741187 flytekit-1.7.0/flytekit_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit_scripts/Readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit_scripts/flytekit_build_image.sh
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-14 04:33:05.000000 flytekit-1.7.0/flytekit_scripts/flytekit_venv
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-14 04:33:05.000000 flytekit-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-14 04:33:19.741187 flytekit-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-14 04:33:17.000000 flytekit-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.246565 flytekit-1.7.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-16 18:14:08.246565 flytekit-1.7.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.210566 flytekit-1.7.1b0/flytekit/
+-rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-06-16 18:14:06.000000 flytekit-1.7.1b0/flytekit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.218566 flytekit-1.7.1b0/flytekit/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23210 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/bin/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.218566 flytekit-1.7.1b0/flytekit/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.218566 flytekit-1.7.1b0/flytekit/clients/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/auth/auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/auth/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/auth/default_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/auth/keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/auth/token_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50793 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/friendly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.218566 flytekit-1.7.1b0/flytekit/clients/grpc_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/grpc_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/grpc_utils/auth_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28489 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.218566 flytekit-1.7.1b0/flytekit/clis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.218566 flytekit-1.7.1b0/flytekit/clis/flyte_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/flyte_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/flyte_cli/example.config
+-rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/flyte_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.218566 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/launchplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/pyflyte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31991 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.222566 flytekit-1.7.1b0/flytekit/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    36185 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/configuration/default_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/configuration/feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/configuration/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/configuration/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.226566 flytekit-1.7.1b0/flytekit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/base_sql_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31002 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/checkpointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/class_based_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36384 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/data_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/dynamic_workflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18343 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/map_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/mock_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/node_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/pod_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46442 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/promise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/python_auto_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/python_customized_container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/python_function_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/reference_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/shim_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/tracked_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77560 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/type_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/type_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41135 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.230566 flytekit-1.7.1b0/flytekit/deck/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/deck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/deck/deck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.230566 flytekit-1.7.1b0/flytekit/deck/html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/deck/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/deck/html/template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/deck/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.230566 flytekit-1.7.1b0/flytekit/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/exceptions/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/exceptions/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/exceptions/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.230566 flytekit-1.7.1b0/flytekit/extend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.230566 flytekit-1.7.1b0/flytekit/extend/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extend/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extend/backend/agent_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extend/backend/base_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.230566 flytekit-1.7.1b0/flytekit/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/cloud_pickle_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.230566 flytekit-1.7.1b0/flytekit/extras/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/pytorch/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/pytorch/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.230566 flytekit-1.7.1b0/flytekit/extras/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/sklearn/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.230566 flytekit-1.7.1b0/flytekit/extras/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/sqlite3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/sqlite3/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.230566 flytekit-1.7.1b0/flytekit/extras/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/tasks/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.234566 flytekit-1.7.1b0/flytekit/extras/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/tensorflow/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/tensorflow/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.234566 flytekit-1.7.1b0/flytekit/image_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/image_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/image_spec/image_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.234566 flytekit-1.7.1b0/flytekit/interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/interaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/interaction/parse_stdin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.234566 flytekit-1.7.1b0/flytekit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/interfaces/cli_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/interfaces/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.234566 flytekit-1.7.1b0/flytekit/interfaces/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/interfaces/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/interfaces/stats/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/interfaces/stats/taggable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.234566 flytekit-1.7.1b0/flytekit/lazy_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/lazy_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/lazy_import/lazy_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.238566 flytekit-1.7.1b0/flytekit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.238566 flytekit-1.7.1b0/flytekit/models/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/admin/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/admin/task_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/admin/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/array_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.238566 flytekit-1.7.1b0/flytekit/models/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/core/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/core/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/core/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/dynamic_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25993 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/matchable_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/named_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/node_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/presto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/qubole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/workflow_closure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.242565 flytekit-1.7.1b0/flytekit/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/remote/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/remote/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/remote/executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/remote/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/remote/lazy_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87310 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/remote/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/remote/remote_callable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.242565 flytekit-1.7.1b0/flytekit/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.242565 flytekit-1.7.1b0/flytekit/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/tools/fast_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/tools/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/tools/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/tools/module_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/tools/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/tools/script_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/tools/serialize_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/tools/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/tools/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.242565 flytekit-1.7.1b0/flytekit/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.242565 flytekit-1.7.1b0/flytekit/types/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/directory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/directory/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.242565 flytekit-1.7.1b0/flytekit/types/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23925 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.246565 flytekit-1.7.1b0/flytekit/types/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/numpy/ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.246565 flytekit-1.7.1b0/flytekit/types/pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/pickle/pickle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.246565 flytekit-1.7.1b0/flytekit/types/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/schema/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/schema/types_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.246565 flytekit-1.7.1b0/flytekit/types/structured/
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/structured/basic_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/structured/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44541 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/structured/structured_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.218566 flytekit-1.7.1b0/flytekit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-16 18:14:08.000000 flytekit-1.7.1b0/flytekit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-06-16 18:14:08.000000 flytekit-1.7.1b0/flytekit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:14:08.000000 flytekit-1.7.1b0/flytekit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-16 18:14:08.000000 flytekit-1.7.1b0/flytekit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-16 18:14:08.000000 flytekit-1.7.1b0/flytekit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 18:14:08.000000 flytekit-1.7.1b0/flytekit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.246565 flytekit-1.7.1b0/flytekit_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit_scripts/Readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit_scripts/flytekit_build_image.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit_scripts/flytekit_venv
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-16 18:14:08.246565 flytekit-1.7.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-16 18:14:06.000000 flytekit-1.7.1b0/setup.py
```

### Comparing `flytekit-1.7.0/LICENSE` & `flytekit-1.7.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/MANIFEST.in` & `flytekit-1.7.1b0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/PKG-INFO` & `flytekit-1.7.1b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.7.0
+Version: 1.7.1b0
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.7.0 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.7.1b0 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.7.0/README.md` & `flytekit-1.7.1b0/README.md`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/__init__.py` & `flytekit-1.7.1b0/flytekit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,14 +188,15 @@
    :toctree: generated/
 
    Description
    Documentation
    SourceCode
 
 """
+import os
 import sys
 from typing import Generator
 
 from rich import traceback
 
 from flytekit.lazy_import.lazy_module import lazy_module
 
@@ -238,15 +239,15 @@
 from flytekit.types.structured.structured_dataset import (
     StructuredDataset,
     StructuredDatasetFormat,
     StructuredDatasetTransformerEngine,
     StructuredDatasetType,
 )
 
-__version__ = "1.7.0"
+__version__ = "1.7.1b0"
 
 
 def current_context() -> ExecutionParameters:
     """
     Use this method to get a handle of specific parameters available in a flyte task.
 
     Usage
@@ -299,8 +300,9 @@
         p.load()
 
 
 # Load all implicit plugins
 load_implicit_plugins()
 
 # Pretty-print exception messages
-traceback.install(width=None, extra_lines=0)
+if os.environ.get("FLYTE_SDK_RICH_TRACEBACKS") != "0":
+    traceback.install(width=None, extra_lines=0)
```

### Comparing `flytekit-1.7.0/flytekit/bin/entrypoint.py` & `flytekit-1.7.1b0/flytekit/bin/entrypoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -510,15 +510,16 @@
     for arg in task_execute_cmd:
         if arg == "--resolver":
             cmd.extend(["--dynamic-addl-distro", additional_distribution, "--dynamic-dest-dir", dest_dir])
         cmd.append(arg)
 
     # Use the commandline to run the task execute command rather than calling it directly in python code
     # since the current runtime bytecode references the older user code, rather than the downloaded distribution.
-    subprocess.run(cmd, check=True)
+    p = subprocess.run(cmd, check=False)
+    exit(p.returncode)
 
 
 @_pass_through.command("pyflyte-map-execute")
 @_click.option("--inputs", required=True)
 @_click.option("--output-prefix", required=True)
 @_click.option("--raw-output-data-prefix", required=False)
 @_click.option("--max-concurrency", type=int, required=False)
```

### Comparing `flytekit-1.7.0/flytekit/clients/auth/auth_client.py` & `flytekit-1.7.1b0/flytekit/clients/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/clients/auth/authenticator.py` & `flytekit-1.7.1b0/flytekit/clients/auth/authenticator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/clients/auth/keyring.py` & `flytekit-1.7.1b0/flytekit/clients/auth/keyring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/clients/auth/token_client.py` & `flytekit-1.7.1b0/flytekit/clients/auth/token_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/clients/auth_helper.py` & `flytekit-1.7.1b0/flytekit/clients/auth_helper.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/clients/friendly.py` & `flytekit-1.7.1b0/flytekit/clients/friendly.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/clients/grpc_utils/auth_interceptor.py` & `flytekit-1.7.1b0/flytekit/clients/grpc_utils/auth_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py` & `flytekit-1.7.1b0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/clients/helpers.py` & `flytekit-1.7.1b0/flytekit/clients/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/clients/raw.py` & `flytekit-1.7.1b0/flytekit/clients/raw.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/clis/flyte_cli/main.py` & `flytekit-1.7.1b0/flytekit/clis/flyte_cli/main.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/clis/helpers.py` & `flytekit-1.7.1b0/flytekit/clis/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/clis/sdk_in_container/backfill.py` & `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/clis/sdk_in_container/build.py` & `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/build.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/clis/sdk_in_container/constants.py` & `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/constants.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/clis/sdk_in_container/helpers.py` & `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/clis/sdk_in_container/init.py` & `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/init.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/clis/sdk_in_container/launchplan.py` & `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/launchplan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/clis/sdk_in_container/metrics.py` & `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/metrics.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/clis/sdk_in_container/package.py` & `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/package.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/clis/sdk_in_container/pyflyte.py` & `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/pyflyte.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/clis/sdk_in_container/register.py` & `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/register.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/clis/sdk_in_container/run.py` & `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/run.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/clis/sdk_in_container/serialize.py` & `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/serialize.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/clis/sdk_in_container/serve.py` & `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/serve.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/configuration/__init__.py` & `flytekit-1.7.1b0/flytekit/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/configuration/default_images.py` & `flytekit-1.7.1b0/flytekit/configuration/default_images.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/configuration/feature_flags.py` & `flytekit-1.7.1b0/flytekit/configuration/feature_flags.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/configuration/file.py` & `flytekit-1.7.1b0/flytekit/configuration/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/configuration/internal.py` & `flytekit-1.7.1b0/flytekit/configuration/internal.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/annotation.py` & `flytekit-1.7.1b0/flytekit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/base_sql_task.py` & `flytekit-1.7.1b0/flytekit/core/base_sql_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/base_task.py` & `flytekit-1.7.1b0/flytekit/core/base_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/checkpointer.py` & `flytekit-1.7.1b0/flytekit/core/checkpointer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/class_based_resolver.py` & `flytekit-1.7.1b0/flytekit/core/class_based_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/condition.py` & `flytekit-1.7.1b0/flytekit/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/constants.py` & `flytekit-1.7.1b0/flytekit/core/constants.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/container_task.py` & `flytekit-1.7.1b0/flytekit/core/container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/context_manager.py` & `flytekit-1.7.1b0/flytekit/core/context_manager.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/data_persistence.py` & `flytekit-1.7.1b0/flytekit/core/data_persistence.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/docstring.py` & `flytekit-1.7.1b0/flytekit/core/docstring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/dynamic_workflow_task.py` & `flytekit-1.7.1b0/flytekit/core/dynamic_workflow_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/gate.py` & `flytekit-1.7.1b0/flytekit/core/gate.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/interface.py` & `flytekit-1.7.1b0/flytekit/core/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 import collections
 import copy
 import inspect
 import typing
 from collections import OrderedDict
 from typing import Any, Dict, Generator, List, Optional, Tuple, Type, TypeVar, Union, cast
 
-from typing_extensions import Annotated, get_args, get_origin, get_type_hints
+from typing_extensions import get_args, get_origin, get_type_hints
 
 from flytekit.core import context_manager
 from flytekit.core.docstring import Docstring
 from flytekit.core.type_engine import TypeEngine
 from flytekit.exceptions.user import FlyteValidationException
 from flytekit.loggers import logger
 from flytekit.models import interface as _interface_models
 from flytekit.models.literals import Void
-from flytekit.types.pickle import FlytePickle
 
 T = typing.TypeVar("T")
 
 
 def repr_kv(k: str, v: Union[Type, Tuple[Type, Any]]) -> str:
     if isinstance(v, tuple):
         if v[1]:
@@ -290,60 +289,35 @@
     """
     map_inputs = transform_types_to_list_of_type(interface.inputs, bound_inputs)
     map_outputs = transform_types_to_list_of_type(interface.outputs, set())
 
     return Interface(inputs=map_inputs, outputs=map_outputs)
 
 
-def _change_unrecognized_type_to_pickle(t: Type[T]) -> typing.Union[Tuple[Type[T]], Type[T]]:
-    try:
-        if hasattr(t, "__origin__") and hasattr(t, "__args__"):
-            ot = get_origin(t)
-            args = getattr(t, "__args__")
-            if ot is list:
-                return typing.List[_change_unrecognized_type_to_pickle(args[0])]  # type: ignore
-            elif ot is dict and args[0] == str:
-                return typing.Dict[str, _change_unrecognized_type_to_pickle(args[1])]  # type: ignore
-            elif ot is typing.Union:
-                return typing.Union[tuple(_change_unrecognized_type_to_pickle(v) for v in get_args(t))]  # type: ignore
-            elif ot is Annotated:
-                base_type, *config = get_args(t)
-                return Annotated[(_change_unrecognized_type_to_pickle(base_type), *config)]  # type: ignore
-        TypeEngine.get_transformer(t)
-    except ValueError:
-        logger.warning(
-            f"Unsupported Type {t} found, Flyte will default to use PickleFile as the transport. "
-            f"Pickle can only be used to send objects between the exact same version of Python, "
-            f"and we strongly recommend to use python type that flyte support."
-        )
-        return FlytePickle[t]
-    return t
-
-
 def transform_function_to_interface(fn: typing.Callable, docstring: Optional[Docstring] = None) -> Interface:
     """
     From the annotations on a task function that the user should have provided, and the output names they want to use
     for each output parameter, construct the TypedInterface object
 
     For now the fancy object, maybe in the future a dumb object.
 
     """
     type_hints = get_type_hints(fn, include_extras=True)
     signature = inspect.signature(fn)
     return_annotation = type_hints.get("return", None)
 
     outputs = extract_return_annotation(return_annotation)
     for k, v in outputs.items():
-        outputs[k] = _change_unrecognized_type_to_pickle(v)  # type: ignore
+        outputs[k] = v  # type: ignore
     inputs: Dict[str, Tuple[Type, Any]] = OrderedDict()
     for k, v in signature.parameters.items():  # type: ignore
         annotation = type_hints.get(k, None)
         default = v.default if v.default is not inspect.Parameter.empty else None
         # Inputs with default values are currently ignored, we may want to look into that in the future
-        inputs[k] = (_change_unrecognized_type_to_pickle(annotation), default)  # type: ignore
+        inputs[k] = (annotation, default)  # type: ignore
 
     # This is just for typing.NamedTuples - in those cases, the user can select a name to call the NamedTuple. We
     # would like to preserve that name in our custom collections.namedtuple.
     custom_name = None
     if hasattr(return_annotation, "__bases__"):
         bases = return_annotation.__bases__
         if len(bases) == 1 and bases[0] == tuple and hasattr(return_annotation, "_fields"):
@@ -361,28 +335,14 @@
     Given a map of str (names of inputs for instance) to their Python native types, return a map of the name to a
     Flyte Variable object with that type.
     """
     res = OrderedDict()
     if variable_map:
         for k, v in variable_map.items():
             res[k] = transform_type(v, descriptions.get(k, k))
-            sub_type: type = v
-            if hasattr(v, "__origin__") and hasattr(v, "__args__"):
-                if getattr(v, "__origin__") is list:
-                    sub_type = getattr(v, "__args__")[0]
-                elif getattr(v, "__origin__") is dict:
-                    sub_type = getattr(v, "__args__")[1]
-            if hasattr(sub_type, "__origin__") and getattr(sub_type, "__origin__") is FlytePickle:
-                original_type = cast(FlytePickle, sub_type).python_type()
-                if hasattr(original_type, "__name__"):
-                    res[k].type.metadata = {"python_class_name": original_type.__name__}
-                elif hasattr(original_type, "_name"):
-                    # If the class doesn't have the __name__ attribute, like typing.Sequence, use _name instead.
-                    res[k].type.metadata = {"python_class_name": original_type._name}
-
     return res
 
 
 def transform_type(x: type, description: Optional[str] = None) -> _interface_models.Variable:
     return _interface_models.Variable(type=TypeEngine.to_literal_type(x), description=description)
```

### Comparing `flytekit-1.7.0/flytekit/core/launch_plan.py` & `flytekit-1.7.1b0/flytekit/core/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/local_cache.py` & `flytekit-1.7.1b0/flytekit/core/local_cache.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/map_task.py` & `flytekit-1.7.1b0/flytekit/core/map_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/mock_stats.py` & `flytekit-1.7.1b0/flytekit/core/mock_stats.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/node.py` & `flytekit-1.7.1b0/flytekit/core/node.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/node_creation.py` & `flytekit-1.7.1b0/flytekit/core/node_creation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/notification.py` & `flytekit-1.7.1b0/flytekit/core/notification.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/pod_template.py` & `flytekit-1.7.1b0/flytekit/core/pod_template.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/promise.py` & `flytekit-1.7.1b0/flytekit/core/promise.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/python_auto_container.py` & `flytekit-1.7.1b0/flytekit/core/python_auto_container.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/python_customized_container_task.py` & `flytekit-1.7.1b0/flytekit/core/python_customized_container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/python_function_task.py` & `flytekit-1.7.1b0/flytekit/core/python_function_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/reference.py` & `flytekit-1.7.1b0/flytekit/core/reference.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/reference_entity.py` & `flytekit-1.7.1b0/flytekit/core/reference_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/resources.py` & `flytekit-1.7.1b0/flytekit/core/resources.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/schedule.py` & `flytekit-1.7.1b0/flytekit/core/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/shim_task.py` & `flytekit-1.7.1b0/flytekit/core/shim_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/task.py` & `flytekit-1.7.1b0/flytekit/core/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/testing.py` & `flytekit-1.7.1b0/flytekit/core/testing.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/tracker.py` & `flytekit-1.7.1b0/flytekit/core/tracker.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/type_engine.py` & `flytekit-1.7.1b0/flytekit/core/type_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -775,15 +775,19 @@
                 # is the case for one of the restricted types, namely NamedTuple.
                 logger.debug(f"Invalid base type {base_type} in call to isinstance", exc_info=True)
 
         # Step 4
         if dataclasses.is_dataclass(python_type):
             return cls._DATACLASS_TRANSFORMER
 
-        raise ValueError(f"Type {python_type} not supported currently in Flytekit. Please register a new transformer")
+        # Step 5
+        display_pickle_warning(str(python_type))
+        from flytekit.types.pickle.pickle import FlytePickleTransformer
+
+        return FlytePickleTransformer()
 
     @classmethod
     def lazy_import_transformers(cls):
         """
         Only load the transformers if needed.
         """
         if cls.has_lazy_import:
@@ -1081,14 +1085,24 @@
     def guess_python_type(self, literal_type: LiteralType) -> list:  # type: ignore
         if literal_type.collection_type:
             ct: Type = TypeEngine.guess_python_type(literal_type.collection_type)
             return typing.List[ct]  # type: ignore
         raise ValueError(f"List transformer cannot reverse {literal_type}")
 
 
+@lru_cache
+def display_pickle_warning(python_type: str):
+    # This is a warning that is only displayed once per python type
+    logger.warning(
+        f"Unsupported Type {python_type} found, Flyte will default to use PickleFile as the transport. "
+        f"Pickle can only be used to send objects between the exact same version of Python, "
+        f"and we strongly recommend to use python type that flyte support."
+    )
+
+
 def _add_tag_to_type(x: LiteralType, tag: str) -> LiteralType:
     x._structure = TypeStructure(tag=tag)
     return x
 
 
 def _type_essence(x: LiteralType) -> LiteralType:
     if x.metadata is not None or x.structure is not None or x.annotation is not None:
```

### Comparing `flytekit-1.7.0/flytekit/core/type_helpers.py` & `flytekit-1.7.1b0/flytekit/core/type_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/utils.py` & `flytekit-1.7.1b0/flytekit/core/utils.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/core/workflow.py` & `flytekit-1.7.1b0/flytekit/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/deck/deck.py` & `flytekit-1.7.1b0/flytekit/deck/deck.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/deck/html/template.html` & `flytekit-1.7.1b0/flytekit/deck/html/template.html`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/deck/renderer.py` & `flytekit-1.7.1b0/flytekit/deck/renderer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/exceptions/scopes.py` & `flytekit-1.7.1b0/flytekit/exceptions/scopes.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/exceptions/system.py` & `flytekit-1.7.1b0/flytekit/exceptions/system.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/exceptions/user.py` & `flytekit-1.7.1b0/flytekit/exceptions/user.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/extend/__init__.py` & `flytekit-1.7.1b0/flytekit/extend/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/extend/backend/agent_service.py` & `flytekit-1.7.1b0/flytekit/extend/backend/agent_service.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/extend/backend/base_agent.py` & `flytekit-1.7.1b0/flytekit/extend/backend/base_agent.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/extras/cloud_pickle_resolver.py` & `flytekit-1.7.1b0/flytekit/extras/cloud_pickle_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/extras/pytorch/__init__.py` & `flytekit-1.7.1b0/flytekit/extras/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/extras/pytorch/checkpoint.py` & `flytekit-1.7.1b0/flytekit/extras/pytorch/checkpoint.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/extras/pytorch/native.py` & `flytekit-1.7.1b0/flytekit/extras/pytorch/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/extras/sklearn/__init__.py` & `flytekit-1.7.1b0/flytekit/extras/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/extras/sklearn/native.py` & `flytekit-1.7.1b0/flytekit/extras/sklearn/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/extras/sqlite3/task.py` & `flytekit-1.7.1b0/flytekit/extras/sqlite3/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/extras/tasks/shell.py` & `flytekit-1.7.1b0/flytekit/extras/tasks/shell.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/extras/tensorflow/__init__.py` & `flytekit-1.7.1b0/flytekit/extras/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/extras/tensorflow/model.py` & `flytekit-1.7.1b0/flytekit/extras/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/extras/tensorflow/record.py` & `flytekit-1.7.1b0/flytekit/extras/tensorflow/record.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/image_spec/image_spec.py` & `flytekit-1.7.1b0/flytekit/image_spec/image_spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,58 @@
 import base64
 import hashlib
 import os
 import typing
 from abc import abstractmethod
 from copy import copy
-from dataclasses import dataclass
+from dataclasses import asdict, dataclass
 from functools import lru_cache
 from typing import List, Optional
 
 import click
 import requests
-from dataclasses_json import dataclass_json
 
 DOCKER_HUB = "docker.io"
 _F_IMG_ID = "_F_IMG_ID"
 
 
-@dataclass_json
 @dataclass
 class ImageSpec:
     """
     This class is used to specify the docker image that will be used to run the task.
 
     Args:
         name: name of the image.
         python_version: python version of the image. Use default python in the base image if None.
         builder: Type of plugin to build the image. Use envd by default.
         source_root: source root of the image.
         env: environment variables of the image.
         registry: registry of the image.
         packages: list of python packages to install.
         apt_packages: list of apt packages to install.
+        cuda: version of cuda to install.
+        cudnn: version of cudnn to install.
         base_image: base image of the image.
         platform: Specify the target platforms for the build output (for example, windows/amd64 or linux/amd64,darwin/arm64
+        pip_index: Specify the custom pip index url
     """
 
     name: str = "flytekit"
     python_version: str = None  # Use default python in the base image if None.
     builder: str = "envd"
     source_root: Optional[str] = None
     env: Optional[typing.Dict[str, str]] = None
     registry: Optional[str] = None
     packages: Optional[List[str]] = None
     apt_packages: Optional[List[str]] = None
+    cuda: Optional[str] = None
+    cudnn: Optional[str] = None
     base_image: Optional[str] = None
     platform: str = "linux/amd64"
+    pip_index: Optional[str] = None
 
     def image_name(self) -> str:
         """
         return full image name with tag.
         """
         tag = calculate_hash_from_image_spec(self)
         container_image = f"{self.name}:{tag}"
@@ -100,15 +104,15 @@
                     return False
 
             click.secho(f"Failed to check if the image exists with error : {e}", fg="red")
             click.secho("Flytekit assumes that the image already exists.", fg="blue")
             return True
 
     def __hash__(self):
-        return hash(self.to_json())
+        return hash(asdict(self).__str__())
 
 
 class ImageSpecBuilder:
     @abstractmethod
     def build_image(self, image_spec: ImageSpec):
         """
         Build the docker image and push it to the registry.
@@ -145,18 +149,18 @@
 def calculate_hash_from_image_spec(image_spec: ImageSpec):
     """
     Calculate the hash from the image spec.
     """
     # copy the image spec to avoid modifying the original image spec. otherwise, the hash will be different.
     spec = copy(image_spec)
     spec.source_root = hash_directory(image_spec.source_root) if image_spec.source_root else b""
-    image_spec_bytes = bytes(spec.to_json(), "utf-8")
+    image_spec_bytes = asdict(spec).__str__().encode("utf-8")
     tag = base64.urlsafe_b64encode(hashlib.md5(image_spec_bytes).digest()).decode("ascii")
-    # replace "=" with "." to make it a valid tag
-    return tag.replace("=", ".")
+    # replace "=" with "." and replace "-" with "_" to make it a valid tag
+    return tag.replace("=", ".").replace("-", "_")
 
 
 def hash_directory(path):
     """
     Return the SHA-256 hash of the directory at the given path.
     """
     hasher = hashlib.sha256()
```

### Comparing `flytekit-1.7.0/flytekit/interaction/parse_stdin.py` & `flytekit-1.7.1b0/flytekit/interaction/parse_stdin.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/interfaces/cli_identifiers.py` & `flytekit-1.7.1b0/flytekit/interfaces/cli_identifiers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/interfaces/random.py` & `flytekit-1.7.1b0/flytekit/interfaces/random.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/interfaces/stats/client.py` & `flytekit-1.7.1b0/flytekit/interfaces/stats/client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/interfaces/stats/taggable.py` & `flytekit-1.7.1b0/flytekit/interfaces/stats/taggable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/lazy_import/lazy_module.py` & `flytekit-1.7.1b0/flytekit/lazy_import/lazy_module.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/loggers.py` & `flytekit-1.7.1b0/flytekit/loggers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/admin/common.py` & `flytekit-1.7.1b0/flytekit/models/admin/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/admin/task_execution.py` & `flytekit-1.7.1b0/flytekit/models/admin/task_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/admin/workflow.py` & `flytekit-1.7.1b0/flytekit/models/admin/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/annotation.py` & `flytekit-1.7.1b0/flytekit/models/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/array_job.py` & `flytekit-1.7.1b0/flytekit/models/array_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/common.py` & `flytekit-1.7.1b0/flytekit/models/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/core/catalog.py` & `flytekit-1.7.1b0/flytekit/models/core/catalog.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/core/compiler.py` & `flytekit-1.7.1b0/flytekit/models/core/compiler.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/core/condition.py` & `flytekit-1.7.1b0/flytekit/models/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/core/errors.py` & `flytekit-1.7.1b0/flytekit/models/core/errors.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/core/execution.py` & `flytekit-1.7.1b0/flytekit/models/core/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/core/identifier.py` & `flytekit-1.7.1b0/flytekit/models/core/identifier.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/core/types.py` & `flytekit-1.7.1b0/flytekit/models/core/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/core/workflow.py` & `flytekit-1.7.1b0/flytekit/models/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/documentation.py` & `flytekit-1.7.1b0/flytekit/models/documentation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/dynamic_job.py` & `flytekit-1.7.1b0/flytekit/models/dynamic_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/execution.py` & `flytekit-1.7.1b0/flytekit/models/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/filters.py` & `flytekit-1.7.1b0/flytekit/models/filters.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/interface.py` & `flytekit-1.7.1b0/flytekit/models/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/launch_plan.py` & `flytekit-1.7.1b0/flytekit/models/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/literals.py` & `flytekit-1.7.1b0/flytekit/models/literals.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/matchable_resource.py` & `flytekit-1.7.1b0/flytekit/models/matchable_resource.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/named_entity.py` & `flytekit-1.7.1b0/flytekit/models/named_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/node_execution.py` & `flytekit-1.7.1b0/flytekit/models/node_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/presto.py` & `flytekit-1.7.1b0/flytekit/models/presto.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/project.py` & `flytekit-1.7.1b0/flytekit/models/project.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/qubole.py` & `flytekit-1.7.1b0/flytekit/models/qubole.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/schedule.py` & `flytekit-1.7.1b0/flytekit/models/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/security.py` & `flytekit-1.7.1b0/flytekit/models/security.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/task.py` & `flytekit-1.7.1b0/flytekit/models/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/types.py` & `flytekit-1.7.1b0/flytekit/models/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/models/workflow_closure.py` & `flytekit-1.7.1b0/flytekit/models/workflow_closure.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/remote/__init__.py` & `flytekit-1.7.1b0/flytekit/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/remote/backfill.py` & `flytekit-1.7.1b0/flytekit/remote/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/remote/entities.py` & `flytekit-1.7.1b0/flytekit/remote/entities.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/remote/executions.py` & `flytekit-1.7.1b0/flytekit/remote/executions.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/remote/lazy_entity.py` & `flytekit-1.7.1b0/flytekit/remote/lazy_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/remote/remote.py` & `flytekit-1.7.1b0/flytekit/remote/remote.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/remote/remote_callable.py` & `flytekit-1.7.1b0/flytekit/remote/remote_callable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/testing/__init__.py` & `flytekit-1.7.1b0/flytekit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/tools/fast_registration.py` & `flytekit-1.7.1b0/flytekit/tools/fast_registration.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/tools/ignore.py` & `flytekit-1.7.1b0/flytekit/tools/ignore.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/tools/module_loader.py` & `flytekit-1.7.1b0/flytekit/tools/module_loader.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/tools/repo.py` & `flytekit-1.7.1b0/flytekit/tools/repo.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/tools/script_mode.py` & `flytekit-1.7.1b0/flytekit/tools/script_mode.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/tools/serialize_helpers.py` & `flytekit-1.7.1b0/flytekit/tools/serialize_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/tools/subprocess.py` & `flytekit-1.7.1b0/flytekit/tools/subprocess.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/tools/translator.py` & `flytekit-1.7.1b0/flytekit/tools/translator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/types/directory/__init__.py` & `flytekit-1.7.1b0/flytekit/types/directory/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/types/directory/types.py` & `flytekit-1.7.1b0/flytekit/types/directory/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/types/file/__init__.py` & `flytekit-1.7.1b0/flytekit/types/file/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/types/file/file.py` & `flytekit-1.7.1b0/flytekit/types/file/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/types/numpy/ndarray.py` & `flytekit-1.7.1b0/flytekit/types/numpy/ndarray.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/types/pickle/pickle.py` & `flytekit-1.7.1b0/flytekit/types/pickle/pickle.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,17 @@
             and literal_type.blob.format == FlytePickleTransformer.PYTHON_PICKLE_FORMAT
         ):
             return FlytePickle
 
         raise ValueError(f"Transformer {self} cannot reverse {literal_type}")
 
     def get_literal_type(self, t: Type[T]) -> LiteralType:
-        return LiteralType(
+        lt = LiteralType(
             blob=_core_types.BlobType(
                 format=self.PYTHON_PICKLE_FORMAT, dimensionality=_core_types.BlobType.BlobDimensionality.SINGLE
             )
         )
+        lt.metadata = {"python_class_name": str(t)}
+        return lt
 
 
 TypeEngine.register(FlytePickleTransformer())
```

### Comparing `flytekit-1.7.0/flytekit/types/schema/types.py` & `flytekit-1.7.1b0/flytekit/types/schema/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/types/schema/types_pandas.py` & `flytekit-1.7.1b0/flytekit/types/schema/types_pandas.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/types/structured/__init__.py` & `flytekit-1.7.1b0/flytekit/types/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/types/structured/basic_dfs.py` & `flytekit-1.7.1b0/flytekit/types/structured/basic_dfs.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/types/structured/bigquery.py` & `flytekit-1.7.1b0/flytekit/types/structured/bigquery.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit/types/structured/structured_dataset.py` & `flytekit-1.7.1b0/flytekit/types/structured/structured_dataset.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit.egg-info/PKG-INFO` & `flytekit-1.7.1b0/flytekit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.7.0
+Version: 1.7.1b0
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.7.0 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.7.1b0 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.7.0/flytekit.egg-info/SOURCES.txt` & `flytekit-1.7.1b0/flytekit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit.egg-info/requires.txt` & `flytekit-1.7.1b0/flytekit.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/flytekit_scripts/flytekit_build_image.sh` & `flytekit-1.7.1b0/flytekit_scripts/flytekit_build_image.sh`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.0/setup.py` & `flytekit-1.7.1b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup  # noqa
 
 extras_require = {}
 
-__version__ = "1.7.0"
+__version__ = "1.7.1b0"
 
 setup(
     name="flytekit",
     version=__version__,
     maintainer="Flyte Contributors",
     maintainer_email="admin@flyte.org",
     packages=find_packages(
```

