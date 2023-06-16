# Comparing `tmp/propan-0.1.3.2.tar.gz` & `tmp/propan-0.1.3.3.tar.gz`

## Comparing `propan-0.1.3.2.tar` & `propan-0.1.3.3.tar`

### file list

```diff
@@ -1,171 +1,171 @@
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.3.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.3.2/SECURITY.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.3.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.3.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.3.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 propan-0.1.3.2/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.3.2/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.3.2/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 propan-0.1.3.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/grpc/gen_py_code.sh
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/grpc/grpc_encoding.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/grpc/message.proto
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/grpc/requirements.txt
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/kafka/1_direct.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/nats/1_basic.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/redis/pattern.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.3.2/examples/sqs/1_basic.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/__about__.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/__main__.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/py.typed
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/types.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/asyncapi/__init__.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/asyncapi/channels.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/asyncapi/info.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/asyncapi/main.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/asyncapi/message.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/asyncapi/security.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/asyncapi/servers.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/asyncapi/subscription.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/asyncapi/utils.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/asyncapi/bindings/__init__.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/asyncapi/bindings/amqp.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/asyncapi/bindings/kafka.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/asyncapi/bindings/main.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/asyncapi/bindings/nats.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/asyncapi/bindings/redis.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/asyncapi/bindings/sqs.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/exceptions.py
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/_model/__init__.py
--rw-r--r--   0        0        0    11701 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/_model/broker_usecase.py
--rw-r--r--   0        0        0     6693 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/_model/schemas.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/_model/utils.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/kafka/__init__.py
--rw-r--r--   0        0        0    12787 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/kafka/kafka_broker.py
--rw-r--r--   0        0        0     8201 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/kafka/kafka_broker.pyi
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/kafka/schemas.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0    14744 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0    10826 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     6852 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     9015 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/sqs/__init__.py
--rw-r--r--   0        0        0     9494 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/sqs/schema.py
--rw-r--r--   0        0        0    12691 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/sqs/sqs_broker.py
--rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/brokers/sqs/sqs_broker.pyi
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/__init__.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/app.py
--rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/main.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/docs/__init__.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/docs/app.py
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/docs/gen.py
--rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/docs/serving.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/startproject/async_app/kafka.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/startproject/async_app/sqs.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     7596 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/fastapi/kafka/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/fastapi/kafka/router.py
--rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/fastapi/kafka/router.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/fastapi/nats/__init__.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/fastapi/nats/router.py
--rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/fastapi/nats/router.pyi
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/fastapi/sqs/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/fastapi/sqs/router.py
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/fastapi/sqs/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/log/__init__.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/log/formatter.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/log/logging.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/test/__init__.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/test/kafka.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/test/nats.py
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/test/rabbit.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/test/redis.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/test/sqs.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/test/utils.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/utils/__init__.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/utils/classes.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/utils/functions.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/utils/no_cast.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/utils/context/main.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.3.2/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.3.2/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.3.2/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.3.2/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.3.2/scripts/test.sh
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.3.2/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.3.2/LICENSE
--rw-r--r--   0        0        0    13471 2020-02-02 00:00:00.000000 propan-0.1.3.2/README.md
--rw-r--r--   0        0        0     5898 2020-02-02 00:00:00.000000 propan-0.1.3.2/pyproject.toml
--rw-r--r--   0        0        0    17588 2020-02-02 00:00:00.000000 propan-0.1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.3.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.3.3/SECURITY.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.3.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.3.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.3.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 propan-0.1.3.3/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.3.3/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.3.3/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 propan-0.1.3.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/grpc/gen_py_code.sh
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/grpc/grpc_encoding.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/grpc/message.proto
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/grpc/requirements.txt
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/kafka/1_direct.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/nats/1_basic.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/redis/pattern.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.3.3/examples/sqs/1_basic.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/__about__.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/__main__.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/py.typed
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/types.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/asyncapi/__init__.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/asyncapi/channels.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/asyncapi/info.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/asyncapi/main.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/asyncapi/message.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/asyncapi/security.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/asyncapi/servers.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/asyncapi/subscription.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/asyncapi/utils.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/asyncapi/bindings/__init__.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/asyncapi/bindings/amqp.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/asyncapi/bindings/kafka.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/asyncapi/bindings/main.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/asyncapi/bindings/nats.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/asyncapi/bindings/redis.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/asyncapi/bindings/sqs.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/exceptions.py
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/_model/__init__.py
+-rw-r--r--   0        0        0    11701 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/_model/broker_usecase.py
+-rw-r--r--   0        0        0     6693 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/_model/schemas.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/_model/utils.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/kafka/__init__.py
+-rw-r--r--   0        0        0    12787 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     8201 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/kafka/kafka_broker.pyi
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/kafka/schemas.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0    15192 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0    10826 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     6852 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     9015 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/sqs/__init__.py
+-rw-r--r--   0        0        0     9494 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/sqs/schema.py
+-rw-r--r--   0        0        0    12691 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/sqs/sqs_broker.py
+-rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/brokers/sqs/sqs_broker.pyi
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/__init__.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/app.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/main.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/docs/__init__.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/docs/app.py
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/docs/gen.py
+-rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/docs/serving.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/startproject/async_app/kafka.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/startproject/async_app/sqs.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     7596 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/fastapi/kafka/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/fastapi/kafka/router.py
+-rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/fastapi/kafka/router.pyi
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/fastapi/nats/__init__.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/fastapi/nats/router.py
+-rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/fastapi/nats/router.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/fastapi/sqs/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/fastapi/sqs/router.py
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/fastapi/sqs/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/log/__init__.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/log/formatter.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/log/logging.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/test/__init__.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/test/kafka.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/test/nats.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/test/redis.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/test/sqs.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/test/utils.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/utils/__init__.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/utils/classes.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/utils/functions.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/utils/no_cast.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/utils/context/main.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.3.3/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.3.3/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.3.3/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.3.3/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.3.3/scripts/test.sh
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.3.3/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.3.3/LICENSE
+-rw-r--r--   0        0        0    13471 2020-02-02 00:00:00.000000 propan-0.1.3.3/README.md
+-rw-r--r--   0        0        0     5898 2020-02-02 00:00:00.000000 propan-0.1.3.3/pyproject.toml
+-rw-r--r--   0        0        0    17588 2020-02-02 00:00:00.000000 propan-0.1.3.3/PKG-INFO
```

### Comparing `propan-0.1.3.2/CONTRIBUTING.md` & `propan-0.1.3.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/SECURITY.md` & `propan-0.1.3.3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/.github/PULL_REQUEST_TEMPLATE.md` & `propan-0.1.3.3/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/.github/ISSUE_TEMPLATE/bug_report.md` & `propan-0.1.3.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/.github/ISSUE_TEMPLATE/config.yml` & `propan-0.1.3.3/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/.github/workflows/documentation.yml` & `propan-0.1.3.3/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/.github/workflows/publish_coverage.yml` & `propan-0.1.3.3/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/.github/workflows/publish_pypi.yml` & `propan-0.1.3.3/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/.github/workflows/tests.yml` & `propan-0.1.3.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/3_lifespan_events.py` & `propan-0.1.3.3/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/4_cli_attributes_promotion.py` & `propan-0.1.3.3/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/5_publishing.py` & `propan-0.1.3.3/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/6_arguments_casting.py` & `propan-0.1.3.3/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/7_handler_errors_processing.py` & `propan-0.1.3.3/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/dependencies/1_dependency_injection.py` & `propan-0.1.3.3/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.3.3/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.3.3/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.3.3/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.3.3/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/dependencies/7_annotated.py` & `propan-0.1.3.3/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/grpc/grpc_encoding.py` & `propan-0.1.3.3/examples/grpc/grpc_encoding.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.3.3/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.3.3/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.3.3/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.3.3/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/http_frameworks_integrations/quart.py` & `propan-0.1.3.3/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.3.3/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.3.3/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/rabbit/direct.py` & `propan-0.1.3.3/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/rabbit/fanout.py` & `propan-0.1.3.3/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/rabbit/header.py` & `propan-0.1.3.3/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/rabbit/topic.py` & `propan-0.1.3.3/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/redis/direct.py` & `propan-0.1.3.3/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/examples/redis/pattern.py` & `propan-0.1.3.3/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/__about__.py` & `propan-0.1.3.3/propan/__about__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Simple and fast framework to create message brokers based microservices"""
 
 from unittest.mock import Mock
 
-__version__ = "0.1.3.2"
+__version__ = "0.1.3.3"
 
 
 INSTALL_MESSAGE = (
     "You should specify using broker!\n"
     "Install it using one of the following commands:\n"
     'pip install "propan[async-rabbit]"\n'
     'pip install "propan[async-nats]"\n'
```

### Comparing `propan-0.1.3.2/propan/__init__.py` & `propan-0.1.3.3/propan/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/annotations.py` & `propan-0.1.3.3/propan/annotations.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/types.py` & `propan-0.1.3.3/propan/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/asyncapi/__init__.py` & `propan-0.1.3.3/propan/asyncapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/asyncapi/channels.py` & `propan-0.1.3.3/propan/asyncapi/channels.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/asyncapi/info.py` & `propan-0.1.3.3/propan/asyncapi/info.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/asyncapi/main.py` & `propan-0.1.3.3/propan/asyncapi/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/asyncapi/message.py` & `propan-0.1.3.3/propan/asyncapi/message.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/asyncapi/security.py` & `propan-0.1.3.3/propan/asyncapi/security.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/asyncapi/servers.py` & `propan-0.1.3.3/propan/asyncapi/servers.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/asyncapi/subscription.py` & `propan-0.1.3.3/propan/asyncapi/subscription.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/asyncapi/utils.py` & `propan-0.1.3.3/propan/asyncapi/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/asyncapi/bindings/amqp.py` & `propan-0.1.3.3/propan/asyncapi/bindings/amqp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/asyncapi/bindings/kafka.py` & `propan-0.1.3.3/propan/asyncapi/bindings/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/asyncapi/bindings/main.py` & `propan-0.1.3.3/propan/asyncapi/bindings/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/asyncapi/bindings/nats.py` & `propan-0.1.3.3/propan/asyncapi/bindings/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/asyncapi/bindings/redis.py` & `propan-0.1.3.3/propan/asyncapi/bindings/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/asyncapi/bindings/sqs.py` & `propan-0.1.3.3/propan/asyncapi/bindings/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/brokers/push_back_watcher.py` & `propan-0.1.3.3/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/brokers/_model/broker_usecase.py` & `propan-0.1.3.3/propan/brokers/_model/broker_usecase.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/brokers/_model/schemas.py` & `propan-0.1.3.3/propan/brokers/_model/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/brokers/_model/utils.py` & `propan-0.1.3.3/propan/brokers/_model/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/brokers/kafka/kafka_broker.py` & `propan-0.1.3.3/propan/brokers/kafka/kafka_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/brokers/kafka/kafka_broker.pyi` & `propan-0.1.3.3/propan/brokers/kafka/kafka_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/brokers/kafka/schemas.py` & `propan-0.1.3.3/propan/brokers/kafka/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/brokers/nats/nats_broker.py` & `propan-0.1.3.3/propan/brokers/nats/nats_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.3.3/propan/brokers/nats/nats_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.3.3/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/brokers/nats/schemas.py` & `propan-0.1.3.3/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.3.3/propan/brokers/rabbit/rabbit_broker.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 from propan.utils import context
 
 TimeoutType = Optional[Union[int, float]]
 PikaSendableMessage: TypeAlias = Union[aio_pika.message.Message, SendableMessage]
 RabbitMessage: TypeAlias = PropanMessage[aio_pika.message.IncomingMessage]
 T = TypeVar("T")
 
+RABBIT_REPLY = "amq.rabbitmq.reply-to"
+
 
 class RabbitBroker(BrokerUsecase):
     handlers: List[Handler]
     _connection: Optional[aio_pika.RobustConnection]
     _channel: Optional[aio_pika.RobustChannel]
     _queues: Dict[RabbitQueue, aio_pika.RobustQueue]
     _exchanges: Dict[RabbitExchange, aio_pika.RobustExchange]
@@ -174,32 +176,40 @@
     ) -> Union[aiormq.abc.ConfirmationFrameType, Dict, str, bytes, None]:
         if self._channel is None:
             raise ValueError("RabbitBroker channel not started yet")
 
         queue, exchange = _validate_queue(queue), _validate_exchange(exchange)
 
         if callback is True:
+            response_queue: asyncio.Queue[PropanMessage] = asyncio.Queue(1)
+
             if reply_to is not None:
                 raise ValueError(
                     "You should use `reply_to` to send response to long-living queue "
                     "and `callback` to get response in sync mode."
                 )
 
-            callback_queue = await self._channel.declare_queue(exclusive=True)
+            callback_queue = await self._channel.get_queue(RABBIT_REPLY)
+            reply_to = RABBIT_REPLY
+
+            async def handle_response(msg: RabbitMessage) -> None:
+                propan_message = await self._parse_message(msg)
+                await response_queue.put(propan_message)
+
+            consumer_tag = await callback_queue.consume(handle_response, no_ack=True)
         else:
-            callback_queue = None
+            callback_queue = consumer_tag = response_queue = None
 
         if exchange is None:
             exchange_obj = self._channel.default_exchange
         else:
             exchange_obj = await self.declare_exchange(exchange)
 
         message = self._validate_message(
             message=message,
-            callback_queue=callback_queue,
             persist=persist,
             reply_to=reply_to,
             **message_kwargs,
         )
 
         r = await exchange_obj.publish(
             message=message,
@@ -207,24 +217,24 @@
             mandatory=mandatory,
             immediate=immediate,
             timeout=timeout,
         )
         if callback_queue is None:
             return r
 
-        else:
-            iter = callback_queue.iterator()
-            await iter.consume()
+        elif response_queue and consumer_tag:
             try:
-                msg = await asyncio.wait_for(iter._queue.get(), callback_timeout)
+                msg = await asyncio.wait_for(response_queue.get(), callback_timeout)
             except asyncio.TimeoutError as e:
                 if raise_timeout is True:  # pragma: no branch
                     raise e
             else:
                 return await self._decode_message(msg)
+            finally:
+                await callback_queue.cancel(consumer_tag)
 
     async def _init_handler(
         self,
         handler: Handler,
     ) -> aio_pika.abc.AbstractRobustQueue:
         queue = await self.declare_queue(handler.queue)
         if handler.exchange is not None and handler.exchange.name != "default":
```

### Comparing `propan-0.1.3.2/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.3.3/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/brokers/rabbit/schemas.py` & `propan-0.1.3.3/propan/brokers/rabbit/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/brokers/redis/redis_broker.py` & `propan-0.1.3.3/propan/brokers/redis/redis_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/brokers/redis/redis_broker.pyi` & `propan-0.1.3.3/propan/brokers/redis/redis_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/brokers/redis/schemas.py` & `propan-0.1.3.3/propan/brokers/redis/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/brokers/sqs/schema.py` & `propan-0.1.3.3/propan/brokers/sqs/schema.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/brokers/sqs/sqs_broker.py` & `propan-0.1.3.3/propan/brokers/sqs/sqs_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/brokers/sqs/sqs_broker.pyi` & `propan-0.1.3.3/propan/brokers/sqs/sqs_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/cli/app.py` & `propan-0.1.3.3/propan/cli/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/cli/main.py` & `propan-0.1.3.3/propan/cli/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/cli/docs/app.py` & `propan-0.1.3.3/propan/cli/docs/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/cli/docs/gen.py` & `propan-0.1.3.3/propan/cli/docs/gen.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/cli/docs/serving.py` & `propan-0.1.3.3/propan/cli/docs/serving.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/cli/startproject/core.py` & `propan-0.1.3.3/propan/cli/startproject/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/cli/startproject/async_app/app.py` & `propan-0.1.3.3/propan/cli/startproject/async_app/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/cli/startproject/async_app/core.py` & `propan-0.1.3.3/propan/cli/startproject/async_app/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/cli/startproject/async_app/kafka.py` & `propan-0.1.3.3/propan/cli/startproject/async_app/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/cli/startproject/async_app/nats.py` & `propan-0.1.3.3/propan/cli/startproject/async_app/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.3.3/propan/cli/startproject/async_app/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/cli/startproject/async_app/redis.py` & `propan-0.1.3.3/propan/cli/startproject/async_app/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/cli/startproject/async_app/sqs.py` & `propan-0.1.3.3/propan/cli/startproject/async_app/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/cli/supervisors/basereload.py` & `propan-0.1.3.3/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/cli/supervisors/multiprocess.py` & `propan-0.1.3.3/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/cli/supervisors/utils.py` & `propan-0.1.3.3/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/cli/supervisors/watchfiles.py` & `propan-0.1.3.3/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/cli/utils/imports.py` & `propan-0.1.3.3/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/cli/utils/logs.py` & `propan-0.1.3.3/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/cli/utils/parser.py` & `propan-0.1.3.3/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/fastapi/__init__.py` & `propan-0.1.3.3/propan/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/fastapi/core/route.py` & `propan-0.1.3.3/propan/fastapi/core/route.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/fastapi/core/router.py` & `propan-0.1.3.3/propan/fastapi/core/router.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/fastapi/kafka/router.pyi` & `propan-0.1.3.3/propan/fastapi/kafka/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/fastapi/nats/router.pyi` & `propan-0.1.3.3/propan/fastapi/nats/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/fastapi/rabbit/router.pyi` & `propan-0.1.3.3/propan/fastapi/rabbit/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/fastapi/redis/router.pyi` & `propan-0.1.3.3/propan/fastapi/redis/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/fastapi/sqs/router.pyi` & `propan-0.1.3.3/propan/fastapi/sqs/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/log/formatter.py` & `propan-0.1.3.3/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/log/logging.py` & `propan-0.1.3.3/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/test/__init__.py` & `propan-0.1.3.3/propan/test/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/test/kafka.py` & `propan-0.1.3.3/propan/test/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/test/nats.py` & `propan-0.1.3.3/propan/test/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/test/rabbit.py` & `propan-0.1.3.3/propan/test/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/test/redis.py` & `propan-0.1.3.3/propan/test/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/test/sqs.py` & `propan-0.1.3.3/propan/test/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/test/utils.py` & `propan-0.1.3.3/propan/test/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/utils/functions.py` & `propan-0.1.3.3/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/utils/context/main.py` & `propan-0.1.3.3/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/propan/utils/context/types.py` & `propan-0.1.3.3/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/LICENSE` & `propan-0.1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/README.md` & `propan-0.1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/pyproject.toml` & `propan-0.1.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.2/PKG-INFO` & `propan-0.1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.3.2
+Version: 0.1.3.3
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
```

