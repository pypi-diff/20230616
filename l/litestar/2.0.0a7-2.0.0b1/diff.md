# Comparing `tmp/litestar-2.0.0a7.tar.gz` & `tmp/litestar-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litestar-2.0.0a7.tar", max compression
+gzip compressed data, was "litestar-2.0.0b1.tar", max compression
```

## Comparing `litestar-2.0.0a7.tar` & `litestar-2.0.0b1.tar`

### file list

```diff
@@ -1,307 +1,313 @@
--rw-r--r--   0        0        0     1092 2023-05-14 12:46:25.414940 litestar-2.0.0a7/LICENSE
--rw-r--r--   0        0        0    50912 2023-05-14 12:46:25.414940 litestar-2.0.0a7/README.md
--rw-r--r--   0        0        0      744 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/__init__.py
--rw-r--r--   0        0        0      103 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/__main__.py
--rw-r--r--   0        0        0       77 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_asgi/__init__.py
--rw-r--r--   0        0        0     6380 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_asgi/asgi_router.py
--rw-r--r--   0        0        0      349 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_asgi/routing_trie/__init__.py
--rw-r--r--   0        0        0     7823 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_asgi/routing_trie/mapping.py
--rw-r--r--   0        0        0     5938 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_asgi/routing_trie/traversal.py
--rw-r--r--   0        0        0     2598 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_asgi/routing_trie/types.py
--rw-r--r--   0        0        0     1267 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_asgi/routing_trie/validate.py
--rw-r--r--   0        0        0     1528 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_asgi/utils.py
--rw-r--r--   0        0        0       66 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_kwargs/__init__.py
--rw-r--r--   0        0        0     3868 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_kwargs/cleanup.py
--rw-r--r--   0        0        0     4239 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_kwargs/dependencies.py
--rw-r--r--   0        0        0    14907 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_kwargs/extractors.py
--rw-r--r--   0        0        0    20450 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_kwargs/kwargs_model.py
--rw-r--r--   0        0        0     2759 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_kwargs/parameter_definition.py
--rw-r--r--   0        0        0        0 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_layers/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_layers/utils.py
--rw-r--r--   0        0        0     5935 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_multipart.py
--rw-r--r--   0        0        0        0 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/__init__.py
--rw-r--r--   0        0        0    10147 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/parameters.py
--rw-r--r--   0        0        0     5525 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/path_item.py
--rw-r--r--   0        0        0     1476 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/request_body.py
--rw-r--r--   0        0        0    10196 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/responses.py
--rw-r--r--   0        0        0       64 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/schema_generation/__init__.py
--rw-r--r--   0        0        0     7074 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/schema_generation/constrained_fields.py
--rw-r--r--   0        0        0     2104 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/schema_generation/examples.py
--rw-r--r--   0        0        0    31771 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/schema_generation/schema.py
--rw-r--r--   0        0        0      524 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/schema_generation/utils.py
--rw-r--r--   0        0        0        0 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/typescript_converter/__init__.py
--rw-r--r--   0        0        0    10970 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/typescript_converter/converter.py
--rw-r--r--   0        0        0     5240 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/typescript_converter/schema_parsing.py
--rw-r--r--   0        0        0     7685 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/typescript_converter/types.py
--rw-r--r--   0        0        0     1464 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_openapi/utils.py
--rw-r--r--   0        0        0     2338 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_parsers.py
--rw-r--r--   0        0        0      182 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_signature/__init__.py
--rw-r--r--   0        0        0     8190 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_signature/field.py
--rw-r--r--   0        0        0       64 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_signature/models/__init__.py
--rw-r--r--   0        0        0    13459 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_signature/models/attrs_signature_model.py
--rw-r--r--   0        0        0     3736 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_signature/models/base.py
--rw-r--r--   0        0        0     6680 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_signature/models/pydantic_signature_model.py
--rw-r--r--   0        0        0     6510 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/_signature/utils.py
--rw-r--r--   0        0        0    35626 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/app.py
--rw-r--r--   0        0        0     2200 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/background_tasks.py
--rw-r--r--   0        0        0      176 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/channels/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/channels/backends/__init__.py
--rw-r--r--   0        0        0      346 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/channels/backends/_redis_flushall_streams.lua
--rw-r--r--   0        0        0      101 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/channels/backends/_redis_pubsub_publish.lua
--rw-r--r--   0        0        0      401 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/channels/backends/_redis_xadd_expire.lua
--rw-r--r--   0        0        0     1300 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/channels/backends/base.py
--rw-r--r--   0        0        0     2768 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/channels/backends/memory.py
--rw-r--r--   0        0        0     9208 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/channels/backends/redis.py
--rw-r--r--   0        0        0    15649 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/channels/plugin.py
--rw-r--r--   0        0        0     4647 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/channels/subscriber.py
--rw-r--r--   0        0        0        0 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/cli/__init__.py
--rw-r--r--   0        0        0    11640 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/cli/_utils.py
--rw-r--r--   0        0        0        0 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/cli/commands/__init__.py
--rw-r--r--   0        0        0     4571 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/cli/commands/core.py
--rw-r--r--   0        0        0     2365 2023-05-14 12:46:25.442940 litestar-2.0.0a7/litestar/cli/commands/schema.py
--rw-r--r--   0        0        0     2224 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/cli/commands/sessions.py
--rw-r--r--   0        0        0     1210 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/cli/main.py
--rw-r--r--   0        0        0        0 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/config/__init__.py
--rw-r--r--   0        0        0     1747 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/config/allowed_hosts.py
--rw-r--r--   0        0        0    11509 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/config/app.py
--rw-r--r--   0        0        0     2742 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/config/compression.py
--rw-r--r--   0        0        0     5177 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/config/cors.py
--rw-r--r--   0        0        0     1771 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/config/csrf.py
--rw-r--r--   0        0        0     1991 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/config/response_cache.py
--rw-r--r--   0        0        0     1922 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/connection/__init__.py
--rw-r--r--   0        0        0    10821 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/connection/base.py
--rw-r--r--   0        0        0     7698 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/connection/request.py
--rw-r--r--   0        0        0    11256 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/connection/websocket.py
--rw-r--r--   0        0        0     1098 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/constants.py
--rw-r--r--   0        0        0        0 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/htmx/__init__.py
--rw-r--r--   0        0        0     4917 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/htmx/_utils.py
--rw-r--r--   0        0        0     4051 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/htmx/request.py
--rw-r--r--   0        0        0     8324 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/htmx/response.py
--rw-r--r--   0        0        0     1261 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/htmx/types.py
--rw-r--r--   0        0        0     2557 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/jinja.py
--rw-r--r--   0        0        0      521 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/jwt/__init__.py
--rw-r--r--   0        0        0    28722 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/jwt/jwt_auth.py
--rw-r--r--   0        0        0     3978 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/jwt/jwt_token.py
--rw-r--r--   0        0        0     6970 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/jwt/middleware.py
--rw-r--r--   0        0        0     3916 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/mako.py
--rw-r--r--   0        0        0        0 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/msgspec/__init__.py
--rw-r--r--   0        0        0      180 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/opentelemetry/__init__.py
--rw-r--r--   0        0        0      845 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/opentelemetry/_utils.py
--rw-r--r--   0        0        0     4206 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/opentelemetry/config.py
--rw-r--r--   0        0        0     2206 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/opentelemetry/middleware.py
--rw-r--r--   0        0        0        0 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/pydantic/__init__.py
--rw-r--r--   0        0        0      290 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/repository/__init__.py
--rw-r--r--   0        0        0     9259 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/repository/abc.py
--rw-r--r--   0        0        0      328 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/repository/exceptions.py
--rw-r--r--   0        0        0     1759 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/repository/filters.py
--rw-r--r--   0        0        0      641 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/repository/handlers.py
--rw-r--r--   0        0        0        0 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/repository/testing/__init__.py
--rw-r--r--   0        0        0    13453 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/repository/testing/generic_mock_repository.py
--rw-r--r--   0        0        0        0 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5258 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/base.py
--rw-r--r--   0        0        0     3414 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/dto.py
--rw-r--r--   0        0        0      742 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/__init__.py
--rw-r--r--   0        0        0      319 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/_slots_base.py
--rw-r--r--   0        0        0      504 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/init/__init__.py
--rw-r--r--   0        0        0      458 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/init/config/__init__.py
--rw-r--r--   0        0        0     3620 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py
--rw-r--r--   0        0        0    11339 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/init/config/common.py
--rw-r--r--   0        0        0    11500 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/init/config/engine.py
--rw-r--r--   0        0        0     2867 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/init/config/sync.py
--rw-r--r--   0        0        0     1644 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/init/plugin.py
--rw-r--r--   0        0        0     1447 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/serialization.py
--rw-r--r--   0        0        0    21972 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/repository.py
--rw-r--r--   0        0        0     2759 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/contrib/sqlalchemy/types.py
--rw-r--r--   0        0        0     9559 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/controller.py
--rw-r--r--   0        0        0    16460 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/data_extractors.py
--rw-r--r--   0        0        0      883 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/datastructures/__init__.py
--rw-r--r--   0        0        0     3757 2023-05-14 12:46:25.446940 litestar-2.0.0a7/litestar/datastructures/cookie.py
--rw-r--r--   0        0        0    17316 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/datastructures/headers.py
--rw-r--r--   0        0        0     2977 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/datastructures/multi_dicts.py
--rw-r--r--   0        0        0     5027 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/datastructures/response_header.py
--rw-r--r--   0        0        0     9302 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/datastructures/state.py
--rw-r--r--   0        0        0     3360 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/datastructures/upload_file.py
--rw-r--r--   0        0        0     7273 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/datastructures/url.py
--rw-r--r--   0        0        0     2783 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/di.py
--rw-r--r--   0        0        0        0 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/__init__.py
--rw-r--r--   0        0        0      337 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/exceptions.py
--rw-r--r--   0        0        0      240 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/__init__.py
--rw-r--r--   0        0        0      245 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/_backends/__init__.py
--rw-r--r--   0        0        0    16643 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/_backends/abc.py
--rw-r--r--   0        0        0        0 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/_backends/msgspec/__init__.py
--rw-r--r--   0        0        0     1339 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/_backends/msgspec/backend.py
--rw-r--r--   0        0        0     1836 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/_backends/msgspec/utils.py
--rw-r--r--   0        0        0        0 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/_backends/pydantic/__init__.py
--rw-r--r--   0        0        0     1299 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/_backends/pydantic/backend.py
--rw-r--r--   0        0        0     1681 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/_backends/pydantic/utils.py
--rw-r--r--   0        0        0     3334 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/_backends/types.py
--rw-r--r--   0        0        0    10628 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/_backends/utils.py
--rw-r--r--   0        0        0     7691 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/abc.py
--rw-r--r--   0        0        0     1261 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/config.py
--rw-r--r--   0        0        0     1449 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/data_structures.py
--rw-r--r--   0        0        0      313 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/exc.py
--rw-r--r--   0        0        0     1269 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/field.py
--rw-r--r--   0        0        0       65 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/stdlib/__init__.py
--rw-r--r--   0        0        0     2112 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/stdlib/dataclass.py
--rw-r--r--   0        0        0     1088 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/types.py
--rw-r--r--   0        0        0     1594 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/factory/utils.py
--rw-r--r--   0        0        0     4455 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/interface.py
--rw-r--r--   0        0        0      309 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/dto/types.py
--rw-r--r--   0        0        0     1728 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/enums.py
--rw-r--r--   0        0        0      201 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/events/__init__.py
--rw-r--r--   0        0        0     4368 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/events/emitter.py
--rw-r--r--   0        0        0     1305 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/events/listener.py
--rw-r--r--   0        0        0     1165 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/exceptions/__init__.py
--rw-r--r--   0        0        0     1702 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/exceptions/base_exceptions.py
--rw-r--r--   0        0        0     4629 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/exceptions/http_exceptions.py
--rw-r--r--   0        0        0     1351 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/exceptions/websocket_exceptions.py
--rw-r--r--   0        0        0     5330 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/file_system.py
--rw-r--r--   0        0        0      559 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/handlers/__init__.py
--rw-r--r--   0        0        0     3877 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/handlers/asgi_handlers.py
--rw-r--r--   0        0        0    20395 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/handlers/base.py
--rw-r--r--   0        0        0      263 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/handlers/http_handlers/__init__.py
--rw-r--r--   0        0        0     8104 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/handlers/http_handlers/_utils.py
--rw-r--r--   0        0        0    26009 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/handlers/http_handlers/base.py
--rw-r--r--   0        0        0    60853 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/handlers/http_handlers/decorators.py
--rw-r--r--   0        0        0      340 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/handlers/websocket_handlers/__init__.py
--rw-r--r--   0        0        0     7151 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/handlers/websocket_handlers/_utils.py
--rw-r--r--   0        0        0    18553 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/handlers/websocket_handlers/listener.py
--rw-r--r--   0        0        0     3619 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/handlers/websocket_handlers/route_handler.py
--rw-r--r--   0        0        0      147 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/logging/__init__.py
--rw-r--r--   0        0        0      569 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/logging/_utils.py
--rw-r--r--   0        0        0    12050 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/logging/config.py
--rw-r--r--   0        0        0     1129 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/logging/picologging.py
--rw-r--r--   0        0        0      860 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/logging/standard.py
--rw-r--r--   0        0        0      385 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/middleware/__init__.py
--rw-r--r--   0        0        0     2081 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/middleware/_utils.py
--rw-r--r--   0        0        0     2967 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/middleware/allowed_hosts.py
--rw-r--r--   0        0        0     3430 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/middleware/authentication.py
--rw-r--r--   0        0        0     5284 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/middleware/base.py
--rw-r--r--   0        0        0     8359 2023-05-14 12:46:25.450940 litestar-2.0.0a7/litestar/middleware/compression.py
--rw-r--r--   0        0        0     2565 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/cors.py
--rw-r--r--   0        0        0     6466 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/csrf.py
--rw-r--r--   0        0        0      124 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/exceptions/__init__.py
--rw-r--r--   0        0        0     7210 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/exceptions/_debug_response.py
--rw-r--r--   0        0        0     8990 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/exceptions/middleware.py
--rw-r--r--   0        0        0      398 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/exceptions/templates/body.html
--rw-r--r--   0        0        0      344 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/exceptions/templates/frame.html
--rw-r--r--   0        0        0      920 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/exceptions/templates/scripts.js
--rw-r--r--   0        0        0     1830 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/exceptions/templates/styles.css
--rw-r--r--   0        0        0    13372 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/logging.py
--rw-r--r--   0        0        0    10811 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/rate_limit.py
--rw-r--r--   0        0        0       70 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/session/__init__.py
--rw-r--r--   0        0        0     7935 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/session/base.py
--rw-r--r--   0        0        0    10365 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/session/client_side.py
--rw-r--r--   0        0        0     8558 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/middleware/session/server_side.py
--rw-r--r--   0        0        0      231 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/__init__.py
--rw-r--r--   0        0        0     5226 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/config.py
--rw-r--r--   0        0        0    16544 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/controller.py
--rw-r--r--   0        0        0      898 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/datastructures.py
--rw-r--r--   0        0        0     1691 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/__init__.py
--rw-r--r--   0        0        0     1648 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/base.py
--rw-r--r--   0        0        0      961 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/callback.py
--rw-r--r--   0        0        0     2936 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/components.py
--rw-r--r--   0        0        0      592 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/contact.py
--rw-r--r--   0        0        0      950 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/discriminator.py
--rw-r--r--   0        0        0     3290 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/encoding.py
--rw-r--r--   0        0        0      974 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/enums.py
--rw-r--r--   0        0        0     1168 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/example.py
--rw-r--r--   0        0        0      614 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/external_documentation.py
--rw-r--r--   0        0        0     5669 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/header.py
--rw-r--r--   0        0        0     1413 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/info.py
--rw-r--r--   0        0        0      752 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/license.py
--rw-r--r--   0        0        0     2876 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/link.py
--rw-r--r--   0        0        0     1882 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/media_type.py
--rw-r--r--   0        0        0     1195 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/oauth_flow.py
--rw-r--r--   0        0        0      897 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/oauth_flows.py
--rw-r--r--   0        0        0     4218 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/open_api.py
--rw-r--r--   0        0        0     4842 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/operation.py
--rw-r--r--   0        0        0     6242 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/parameter.py
--rw-r--r--   0        0        0     3245 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/path_item.py
--rw-r--r--   0        0        0     1255 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/paths.py
--rw-r--r--   0        0        0     1351 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/reference.py
--rw-r--r--   0        0        0     1095 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/request_body.py
--rw-r--r--   0        0        0     1854 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/response.py
--rw-r--r--   0        0        0     2367 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/responses.py
--rw-r--r--   0        0        0    34574 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/schema.py
--rw-r--r--   0        0        0     1686 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/security_requirement.py
--rw-r--r--   0        0        0     2690 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/security_scheme.py
--rw-r--r--   0        0        0     1077 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/server.py
--rw-r--r--   0        0        0     1171 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/server_variable.py
--rw-r--r--   0        0        0      923 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/tag.py
--rw-r--r--   0        0        0     1702 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/openapi/spec/xml.py
--rw-r--r--   0        0        0    10984 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/pagination.py
--rw-r--r--   0        0        0    16805 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/params.py
--rw-r--r--   0        0        0     7100 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/partial.py
--rw-r--r--   0        0        0     3926 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/plugins.py
--rw-r--r--   0        0        0        0 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/py.typed
--rw-r--r--   0        0        0      278 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/response/__init__.py
--rw-r--r--   0        0        0    12404 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/response/base.py
--rw-r--r--   0        0        0     9225 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/response/file.py
--rw-r--r--   0        0        0     2952 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/response/redirect.py
--rw-r--r--   0        0        0     4883 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/response/streaming.py
--rw-r--r--   0        0        0     2994 2023-05-14 12:46:25.454940 litestar-2.0.0a7/litestar/response/template.py
--rw-r--r--   0        0        0    14975 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/response_containers.py
--rw-r--r--   0        0        0    14997 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/router.py
--rw-r--r--   0        0        0      191 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/routes/__init__.py
--rw-r--r--   0        0        0     1757 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/routes/asgi.py
--rw-r--r--   0        0        0     6437 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/routes/base.py
--rw-r--r--   0        0        0    13307 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/routes/http.py
--rw-r--r--   0        0        0     3052 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/routes/websocket.py
--rw-r--r--   0        0        0       97 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/security/__init__.py
--rw-r--r--   0        0        0     7165 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/security/base.py
--rw-r--r--   0        0        0      188 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/security/session_auth/__init__.py
--rw-r--r--   0        0        0     5602 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/security/session_auth/auth.py
--rw-r--r--   0        0        0     4952 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/security/session_auth/middleware.py
--rw-r--r--   0        0        0     7355 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/serialization.py
--rw-r--r--   0        0        0      158 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/static_files/__init__.py
--rw-r--r--   0        0        0     5019 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/static_files/base.py
--rw-r--r--   0        0        0     3598 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/static_files/config.py
--rw-r--r--   0        0        0     9536 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/status_codes.py
--rw-r--r--   0        0        0        0 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/stores/__init__.py
--rw-r--r--   0        0        0     4396 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/stores/base.py
--rw-r--r--   0        0        0     5425 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/stores/file.py
--rw-r--r--   0        0        0     3625 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/stores/memory.py
--rw-r--r--   0        0        0     6231 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/stores/redis.py
--rw-r--r--   0        0        0     2233 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/stores/registry.py
--rw-r--r--   0        0        0      204 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/template/__init__.py
--rw-r--r--   0        0        0     4113 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/template/base.py
--rw-r--r--   0        0        0     1894 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/template/config.py
--rw-r--r--   0        0        0      581 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/testing/__init__.py
--rw-r--r--   0        0        0     1816 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/testing/client/__init__.py
--rw-r--r--   0        0        0    17445 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/testing/client/async_client.py
--rw-r--r--   0        0        0     5132 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/testing/client/base.py
--rw-r--r--   0        0        0    19555 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/testing/client/sync_client.py
--rw-r--r--   0        0        0    29563 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/testing/helpers.py
--rw-r--r--   0        0        0     2532 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/testing/life_span_handler.py
--rw-r--r--   0        0        0    21927 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/testing/request_factory.py
--rw-r--r--   0        0        0     8086 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/testing/transport.py
--rw-r--r--   0        0        0     8527 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/testing/websocket_test_session.py
--rw-r--r--   0        0        0     4047 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/types/__init__.py
--rw-r--r--   0        0        0     8697 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/types/asgi_types.py
--rw-r--r--   0        0        0      453 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/types/builtin_types.py
--rw-r--r--   0        0        0     2235 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/types/callable_types.py
--rw-r--r--   0        0        0     1678 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/types/composite_types.py
--rw-r--r--   0        0        0      183 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/types/empty.py
--rw-r--r--   0        0        0     2662 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/types/file_types.py
--rw-r--r--   0        0        0      344 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/types/helper_types.py
--rw-r--r--   0        0        0     1720 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/types/internal_types.py
--rw-r--r--   0        0        0     2607 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/types/protocols.py
--rw-r--r--   0        0        0     1820 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/types/serialization.py
--rw-r--r--   0        0        0     1906 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/utils/__init__.py
--rw-r--r--   0        0        0      729 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/utils/compat.py
--rw-r--r--   0        0        0     3578 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/utils/dataclass.py
--rw-r--r--   0        0        0     3520 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/utils/deprecation.py
--rw-r--r--   0        0        0     1732 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/utils/helpers.py
--rw-r--r--   0        0        0      723 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/utils/path.py
--rw-r--r--   0        0        0    10434 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/utils/predicates.py
--rw-r--r--   0        0        0     2720 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/utils/scope.py
--rw-r--r--   0        0        0     1003 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/utils/sequence.py
--rw-r--r--   0        0        0    14118 2023-05-14 12:46:25.458940 litestar-2.0.0a7/litestar/utils/signature.py
--rw-r--r--   0        0        0     5337 2023-05-14 12:46:25.462940 litestar-2.0.0a7/litestar/utils/sync.py
--rw-r--r--   0        0        0     6405 2023-05-14 12:46:25.462940 litestar-2.0.0a7/litestar/utils/typing.py
--rw-r--r--   0        0        0     1921 2023-05-14 12:46:25.462940 litestar-2.0.0a7/litestar/utils/version.py
--rw-r--r--   0        0        0     1331 2023-05-14 12:46:25.462940 litestar-2.0.0a7/litestar/utils/warnings.py
--rw-r--r--   0        0        0    10041 2023-05-14 12:46:25.462940 litestar-2.0.0a7/pyproject.toml
--rw-r--r--   0        0        0    54547 1970-01-01 00:00:00.000000 litestar-2.0.0a7/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-06-16 11:23:18.734701 litestar-2.0.0b1/LICENSE
+-rw-r--r--   0        0        0    51150 2023-06-16 11:23:18.734701 litestar-2.0.0b1/docs/PYPI_README.md
+-rw-r--r--   0        0        0      744 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/__init__.py
+-rw-r--r--   0        0        0      228 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/__main__.py
+-rw-r--r--   0        0        0       77 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_asgi/__init__.py
+-rw-r--r--   0        0        0     6380 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_asgi/asgi_router.py
+-rw-r--r--   0        0        0      349 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_asgi/routing_trie/__init__.py
+-rw-r--r--   0        0        0     7823 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_asgi/routing_trie/mapping.py
+-rw-r--r--   0        0        0     5938 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_asgi/routing_trie/traversal.py
+-rw-r--r--   0        0        0     2598 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_asgi/routing_trie/types.py
+-rw-r--r--   0        0        0     1267 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_asgi/routing_trie/validate.py
+-rw-r--r--   0        0        0     1528 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_asgi/utils.py
+-rw-r--r--   0        0        0       66 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_kwargs/__init__.py
+-rw-r--r--   0        0        0     3868 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_kwargs/cleanup.py
+-rw-r--r--   0        0        0     4239 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_kwargs/dependencies.py
+-rw-r--r--   0        0        0    14894 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_kwargs/extractors.py
+-rw-r--r--   0        0        0    20450 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_kwargs/kwargs_model.py
+-rw-r--r--   0        0        0     2759 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_kwargs/parameter_definition.py
+-rw-r--r--   0        0        0        0 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_layers/__init__.py
+-rw-r--r--   0        0        0     1288 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_layers/utils.py
+-rw-r--r--   0        0        0     5922 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_multipart.py
+-rw-r--r--   0        0        0        0 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/__init__.py
+-rw-r--r--   0        0        0    10215 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/parameters.py
+-rw-r--r--   0        0        0     5491 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/path_item.py
+-rw-r--r--   0        0        0     1523 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/request_body.py
+-rw-r--r--   0        0        0    10471 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/responses.py
+-rw-r--r--   0        0        0       64 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/schema_generation/__init__.py
+-rw-r--r--   0        0        0     7191 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/schema_generation/constrained_fields.py
+-rw-r--r--   0        0        0     2104 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/schema_generation/examples.py
+-rw-r--r--   0        0        0    35844 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/schema_generation/schema.py
+-rw-r--r--   0        0        0      524 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/schema_generation/utils.py
+-rw-r--r--   0        0        0        0 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/typescript_converter/__init__.py
+-rw-r--r--   0        0        0    10970 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/typescript_converter/converter.py
+-rw-r--r--   0        0        0     5240 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/typescript_converter/schema_parsing.py
+-rw-r--r--   0        0        0     7685 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/typescript_converter/types.py
+-rw-r--r--   0        0        0     1464 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/utils.py
+-rw-r--r--   0        0        0     2338 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/_parsers.py
+-rw-r--r--   0        0        0      182 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/_signature/__init__.py
+-rw-r--r--   0        0        0     7023 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/_signature/field.py
+-rw-r--r--   0        0        0     4334 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/_signature/metadata.py
+-rw-r--r--   0        0        0       64 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/_signature/models/__init__.py
+-rw-r--r--   0        0        0    13948 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/_signature/models/attrs_signature_model.py
+-rw-r--r--   0        0        0     3736 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/_signature/models/base.py
+-rw-r--r--   0        0        0     6689 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/_signature/models/pydantic_signature_model.py
+-rw-r--r--   0        0        0     5639 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/_signature/utils.py
+-rw-r--r--   0        0        0    36313 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/app.py
+-rw-r--r--   0        0        0     2200 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/background_tasks.py
+-rw-r--r--   0        0        0      176 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/channels/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/channels/backends/__init__.py
+-rw-r--r--   0        0        0      346 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/channels/backends/_redis_flushall_streams.lua
+-rw-r--r--   0        0        0      101 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/channels/backends/_redis_pubsub_publish.lua
+-rw-r--r--   0        0        0      401 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/channels/backends/_redis_xadd_expire.lua
+-rw-r--r--   0        0        0     1300 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/channels/backends/base.py
+-rw-r--r--   0        0        0     2768 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/channels/backends/memory.py
+-rw-r--r--   0        0        0     9364 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/channels/backends/redis.py
+-rw-r--r--   0        0        0    15726 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/channels/plugin.py
+-rw-r--r--   0        0        0     4647 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/channels/subscriber.py
+-rw-r--r--   0        0        0        0 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/cli/__init__.py
+-rw-r--r--   0        0        0    12595 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/cli/_utils.py
+-rw-r--r--   0        0        0        0 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/cli/commands/__init__.py
+-rw-r--r--   0        0        0     6630 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/cli/commands/core.py
+-rw-r--r--   0        0        0     2568 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/cli/commands/schema.py
+-rw-r--r--   0        0        0     2381 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/cli/commands/sessions.py
+-rw-r--r--   0        0        0     2125 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/cli/main.py
+-rw-r--r--   0        0        0        0 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/config/__init__.py
+-rw-r--r--   0        0        0     1747 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/config/allowed_hosts.py
+-rw-r--r--   0        0        0    11442 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/config/app.py
+-rw-r--r--   0        0        0     2742 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/config/compression.py
+-rw-r--r--   0        0        0     5177 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/config/cors.py
+-rw-r--r--   0        0        0     1771 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/config/csrf.py
+-rw-r--r--   0        0        0     1991 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/config/response_cache.py
+-rw-r--r--   0        0        0     1922 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/connection/__init__.py
+-rw-r--r--   0        0        0    10821 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/connection/base.py
+-rw-r--r--   0        0        0     7698 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/connection/request.py
+-rw-r--r--   0        0        0    11274 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/connection/websocket.py
+-rw-r--r--   0        0        0     1363 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/constants.py
+-rw-r--r--   0        0        0        0 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/htmx/__init__.py
+-rw-r--r--   0        0        0     4917 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/htmx/_utils.py
+-rw-r--r--   0        0        0     4051 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/htmx/request.py
+-rw-r--r--   0        0        0     6401 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/htmx/response.py
+-rw-r--r--   0        0        0     1261 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/htmx/types.py
+-rw-r--r--   0        0        0     2557 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/jinja.py
+-rw-r--r--   0        0        0      521 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/jwt/__init__.py
+-rw-r--r--   0        0        0    28722 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/jwt/jwt_auth.py
+-rw-r--r--   0        0        0     4463 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/jwt/jwt_token.py
+-rw-r--r--   0        0        0     6970 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/jwt/middleware.py
+-rw-r--r--   0        0        0     3961 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/mako.py
+-rw-r--r--   0        0        0     2167 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/msgspec.py
+-rw-r--r--   0        0        0      180 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      845 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/opentelemetry/_utils.py
+-rw-r--r--   0        0        0     4206 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/opentelemetry/config.py
+-rw-r--r--   0        0        0     2206 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/opentelemetry/middleware.py
+-rw-r--r--   0        0        0     2341 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/pydantic.py
+-rw-r--r--   0        0        0      364 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/repository/__init__.py
+-rw-r--r--   0        0        0      162 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/repository/abc/__init__.py
+-rw-r--r--   0        0        0     8889 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/repository/abc/_async.py
+-rw-r--r--   0        0        0     8907 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/repository/abc/_sync.py
+-rw-r--r--   0        0        0      328 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/repository/exceptions.py
+-rw-r--r--   0        0        0     2064 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/repository/filters.py
+-rw-r--r--   0        0        0      641 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/repository/handlers.py
+-rw-r--r--   0        0        0        0 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/repository/testing/__init__.py
+-rw-r--r--   0        0        0    26054 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/repository/testing/generic_mock_repository.py
+-rw-r--r--   0        0        0        0 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5571 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/base.py
+-rw-r--r--   0        0        0     8465 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/dto.py
+-rw-r--r--   0        0        0      941 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/__init__.py
+-rw-r--r--   0        0        0      319 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/_slots_base.py
+-rw-r--r--   0        0        0      504 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/init/__init__.py
+-rw-r--r--   0        0        0      458 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/init/config/__init__.py
+-rw-r--r--   0        0        0     4575 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py
+-rw-r--r--   0        0        0    11408 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/init/config/common.py
+-rw-r--r--   0        0        0    11500 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/init/config/engine.py
+-rw-r--r--   0        0        0     3787 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/init/config/sync.py
+-rw-r--r--   0        0        0     1647 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/init/plugin.py
+-rw-r--r--   0        0        0     1426 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/serialization.py
+-rw-r--r--   0        0        0      288 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/repository/__init__.py
+-rw-r--r--   0        0        0    23050 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/repository/_async.py
+-rw-r--r--   0        0        0    22806 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/repository/_sync.py
+-rw-r--r--   0        0        0     1033 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/repository/_util.py
+-rw-r--r--   0        0        0      754 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/repository/types.py
+-rw-r--r--   0        0        0     6349 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/types.py
+-rw-r--r--   0        0        0     9546 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/controller.py
+-rw-r--r--   0        0        0    16508 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/data_extractors.py
+-rw-r--r--   0        0        0      883 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/datastructures/__init__.py
+-rw-r--r--   0        0        0     3757 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/datastructures/cookie.py
+-rw-r--r--   0        0        0    17316 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/datastructures/headers.py
+-rw-r--r--   0        0        0     2977 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/datastructures/multi_dicts.py
+-rw-r--r--   0        0        0     5027 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/datastructures/response_header.py
+-rw-r--r--   0        0        0     9646 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/datastructures/state.py
+-rw-r--r--   0        0        0     3310 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/datastructures/upload_file.py
+-rw-r--r--   0        0        0     7273 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/datastructures/url.py
+-rw-r--r--   0        0        0     3117 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/di.py
+-rw-r--r--   0        0        0        0 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/__init__.py
+-rw-r--r--   0        0        0      240 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/__init__.py
+-rw-r--r--   0        0        0      245 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/_backends/__init__.py
+-rw-r--r--   0        0        0    18470 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/_backends/abc.py
+-rw-r--r--   0        0        0        0 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/_backends/msgspec/__init__.py
+-rw-r--r--   0        0        0     1339 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/_backends/msgspec/backend.py
+-rw-r--r--   0        0        0     1691 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/_backends/msgspec/utils.py
+-rw-r--r--   0        0        0        0 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/_backends/pydantic/__init__.py
+-rw-r--r--   0        0        0     1299 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/_backends/pydantic/backend.py
+-rw-r--r--   0        0        0     1936 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/_backends/pydantic/utils.py
+-rw-r--r--   0        0        0     3704 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/_backends/types.py
+-rw-r--r--   0        0        0    14227 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/_backends/utils.py
+-rw-r--r--   0        0        0     7720 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/abc.py
+-rw-r--r--   0        0        0     1405 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/config.py
+-rw-r--r--   0        0        0     3276 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/data_structures.py
+-rw-r--r--   0        0        0      313 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/exc.py
+-rw-r--r--   0        0        0     1388 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/field.py
+-rw-r--r--   0        0        0       65 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/stdlib/__init__.py
+-rw-r--r--   0        0        0     2144 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/stdlib/dataclass.py
+-rw-r--r--   0        0        0      363 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/types.py
+-rw-r--r--   0        0        0     4457 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/utils.py
+-rw-r--r--   0        0        0     4474 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/interface.py
+-rw-r--r--   0        0        0      309 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/types.py
+-rw-r--r--   0        0        0     1728 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/enums.py
+-rw-r--r--   0        0        0      201 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/events/__init__.py
+-rw-r--r--   0        0        0     4355 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/events/emitter.py
+-rw-r--r--   0        0        0     1305 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/events/listener.py
+-rw-r--r--   0        0        0     1165 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/exceptions/__init__.py
+-rw-r--r--   0        0        0     1702 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/exceptions/base_exceptions.py
+-rw-r--r--   0        0        0     4629 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/exceptions/http_exceptions.py
+-rw-r--r--   0        0        0     1351 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/exceptions/websocket_exceptions.py
+-rw-r--r--   0        0        0     5336 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/file_system.py
+-rw-r--r--   0        0        0      559 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/handlers/__init__.py
+-rw-r--r--   0        0        0     3868 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/handlers/asgi_handlers.py
+-rw-r--r--   0        0        0    20477 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/handlers/base.py
+-rw-r--r--   0        0        0      263 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/handlers/http_handlers/__init__.py
+-rw-r--r--   0        0        0     6658 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/handlers/http_handlers/_utils.py
+-rw-r--r--   0        0        0    26422 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/handlers/http_handlers/base.py
+-rw-r--r--   0        0        0    62224 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/handlers/http_handlers/decorators.py
+-rw-r--r--   0        0        0      340 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/handlers/websocket_handlers/__init__.py
+-rw-r--r--   0        0        0     7151 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/handlers/websocket_handlers/_utils.py
+-rw-r--r--   0        0        0    18876 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/handlers/websocket_handlers/listener.py
+-rw-r--r--   0        0        0     3605 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/handlers/websocket_handlers/route_handler.py
+-rw-r--r--   0        0        0      147 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/logging/__init__.py
+-rw-r--r--   0        0        0      569 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/logging/_utils.py
+-rw-r--r--   0        0        0    12050 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/logging/config.py
+-rw-r--r--   0        0        0     1129 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/logging/picologging.py
+-rw-r--r--   0        0        0      860 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/logging/standard.py
+-rw-r--r--   0        0        0      385 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/__init__.py
+-rw-r--r--   0        0        0     2081 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/_utils.py
+-rw-r--r--   0        0        0     3086 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/allowed_hosts.py
+-rw-r--r--   0        0        0     3430 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/authentication.py
+-rw-r--r--   0        0        0     5284 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/base.py
+-rw-r--r--   0        0        0     8395 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/compression.py
+-rw-r--r--   0        0        0     2565 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/cors.py
+-rw-r--r--   0        0        0     6466 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/csrf.py
+-rw-r--r--   0        0        0      124 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/exceptions/__init__.py
+-rw-r--r--   0        0        0     7210 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/exceptions/_debug_response.py
+-rw-r--r--   0        0        0     9275 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/exceptions/middleware.py
+-rw-r--r--   0        0        0      398 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/exceptions/templates/body.html
+-rw-r--r--   0        0        0      344 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/exceptions/templates/frame.html
+-rw-r--r--   0        0        0      920 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/exceptions/templates/scripts.js
+-rw-r--r--   0        0        0     1830 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/exceptions/templates/styles.css
+-rw-r--r--   0        0        0    13330 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/logging.py
+-rw-r--r--   0        0        0    10811 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/rate_limit.py
+-rw-r--r--   0        0        0       70 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/session/__init__.py
+-rw-r--r--   0        0        0     7935 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/session/base.py
+-rw-r--r--   0        0        0    10365 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/session/client_side.py
+-rw-r--r--   0        0        0     8558 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/session/server_side.py
+-rw-r--r--   0        0        0      183 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/__init__.py
+-rw-r--r--   0        0        0     5226 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/config.py
+-rw-r--r--   0        0        0    15696 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/controller.py
+-rw-r--r--   0        0        0      898 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/datastructures.py
+-rw-r--r--   0        0        0     1691 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/__init__.py
+-rw-r--r--   0        0        0     1915 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/base.py
+-rw-r--r--   0        0        0      961 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/callback.py
+-rw-r--r--   0        0        0     2936 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/components.py
+-rw-r--r--   0        0        0      592 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/contact.py
+-rw-r--r--   0        0        0      950 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/discriminator.py
+-rw-r--r--   0        0        0     3290 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/encoding.py
+-rw-r--r--   0        0        0      974 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/enums.py
+-rw-r--r--   0        0        0     1168 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/example.py
+-rw-r--r--   0        0        0      614 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/external_documentation.py
+-rw-r--r--   0        0        0     5669 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/header.py
+-rw-r--r--   0        0        0     1413 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/info.py
+-rw-r--r--   0        0        0      752 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/license.py
+-rw-r--r--   0        0        0     2876 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/link.py
+-rw-r--r--   0        0        0     1882 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/media_type.py
+-rw-r--r--   0        0        0     1195 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/oauth_flow.py
+-rw-r--r--   0        0        0      897 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/oauth_flows.py
+-rw-r--r--   0        0        0     4218 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/open_api.py
+-rw-r--r--   0        0        0     4842 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/operation.py
+-rw-r--r--   0        0        0     6242 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/parameter.py
+-rw-r--r--   0        0        0     3245 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/path_item.py
+-rw-r--r--   0        0        0     1255 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/paths.py
+-rw-r--r--   0        0        0     1351 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/reference.py
+-rw-r--r--   0        0        0     1095 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/request_body.py
+-rw-r--r--   0        0        0     1854 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/response.py
+-rw-r--r--   0        0        0     2367 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/responses.py
+-rw-r--r--   0        0        0    34574 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/schema.py
+-rw-r--r--   0        0        0     1686 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/security_requirement.py
+-rw-r--r--   0        0        0     2690 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/security_scheme.py
+-rw-r--r--   0        0        0     1077 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/server.py
+-rw-r--r--   0        0        0     1171 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/server_variable.py
+-rw-r--r--   0        0        0      923 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/tag.py
+-rw-r--r--   0        0        0     1702 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/xml.py
+-rw-r--r--   0        0        0    11029 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/pagination.py
+-rw-r--r--   0        0        0    14871 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/params.py
+-rw-r--r--   0        0        0     7100 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/partial.py
+-rw-r--r--   0        0        0     3905 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/plugins.py
+-rw-r--r--   0        0        0        0 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/py.typed
+-rw-r--r--   0        0        0      208 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/response/__init__.py
+-rw-r--r--   0        0        0    15231 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/response/base.py
+-rw-r--r--   0        0        0    14298 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/response/file.py
+-rw-r--r--   0        0        0     5440 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/response/redirect.py
+-rw-r--r--   0        0        0     7943 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/response/streaming.py
+-rw-r--r--   0        0        0     5229 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/response/template.py
+-rw-r--r--   0        0        0    14998 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/router.py
+-rw-r--r--   0        0        0      191 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/routes/__init__.py
+-rw-r--r--   0        0        0     1719 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/routes/asgi.py
+-rw-r--r--   0        0        0     6437 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/routes/base.py
+-rw-r--r--   0        0        0    13244 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/routes/http.py
+-rw-r--r--   0        0        0     3002 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/routes/websocket.py
+-rw-r--r--   0        0        0       97 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/security/__init__.py
+-rw-r--r--   0        0        0     7165 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/security/base.py
+-rw-r--r--   0        0        0      188 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/security/session_auth/__init__.py
+-rw-r--r--   0        0        0     5602 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/security/session_auth/auth.py
+-rw-r--r--   0        0        0     4952 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/security/session_auth/middleware.py
+-rw-r--r--   0        0        0     7714 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/serialization.py
+-rw-r--r--   0        0        0      158 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/static_files/__init__.py
+-rw-r--r--   0        0        0     5046 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/static_files/base.py
+-rw-r--r--   0        0        0     3598 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/static_files/config.py
+-rw-r--r--   0        0        0     9536 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/status_codes.py
+-rw-r--r--   0        0        0        0 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/stores/__init__.py
+-rw-r--r--   0        0        0     4396 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/stores/base.py
+-rw-r--r--   0        0        0     5425 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/stores/file.py
+-rw-r--r--   0        0        0     3625 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/stores/memory.py
+-rw-r--r--   0        0        0     6231 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/stores/redis.py
+-rw-r--r--   0        0        0     2233 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/stores/registry.py
+-rw-r--r--   0        0        0      204 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/template/__init__.py
+-rw-r--r--   0        0        0     4083 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/template/base.py
+-rw-r--r--   0        0        0     1894 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/template/config.py
+-rw-r--r--   0        0        0      581 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/testing/__init__.py
+-rw-r--r--   0        0        0     1816 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/testing/client/__init__.py
+-rw-r--r--   0        0        0    17445 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/testing/client/async_client.py
+-rw-r--r--   0        0        0     5132 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/testing/client/base.py
+-rw-r--r--   0        0        0    19555 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/testing/client/sync_client.py
+-rw-r--r--   0        0        0    29657 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/testing/helpers.py
+-rw-r--r--   0        0        0     2532 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/testing/life_span_handler.py
+-rw-r--r--   0        0        0    21927 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/testing/request_factory.py
+-rw-r--r--   0        0        0     8057 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/testing/transport.py
+-rw-r--r--   0        0        0     8559 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/testing/websocket_test_session.py
+-rw-r--r--   0        0        0     4047 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/types/__init__.py
+-rw-r--r--   0        0        0     8671 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/types/asgi_types.py
+-rw-r--r--   0        0        0      453 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/types/builtin_types.py
+-rw-r--r--   0        0        0     2222 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/types/callable_types.py
+-rw-r--r--   0        0        0     1705 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/types/composite_types.py
+-rw-r--r--   0        0        0      183 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/types/empty.py
+-rw-r--r--   0        0        0     2666 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/types/file_types.py
+-rw-r--r--   0        0        0      344 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/types/helper_types.py
+-rw-r--r--   0        0        0     1720 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/types/internal_types.py
+-rw-r--r--   0        0        0     2965 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/types/protocols.py
+-rw-r--r--   0        0        0     1820 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/types/serialization.py
+-rw-r--r--   0        0        0     6483 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/typing.py
+-rw-r--r--   0        0        0     1953 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/__init__.py
+-rw-r--r--   0        0        0      729 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/compat.py
+-rw-r--r--   0        0        0     3635 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/dataclass.py
+-rw-r--r--   0        0        0     3520 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/deprecation.py
+-rw-r--r--   0        0        0     3334 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/helpers.py
+-rw-r--r--   0        0        0      723 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/path.py
+-rw-r--r--   0        0        0    11750 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/predicates.py
+-rw-r--r--   0        0        0     2823 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/scope.py
+-rw-r--r--   0        0        0     1003 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/sequence.py
+-rw-r--r--   0        0        0     8410 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/signature.py
+-rw-r--r--   0        0        0     4374 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/sync.py
+-rw-r--r--   0        0        0     8302 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/typing.py
+-rw-r--r--   0        0        0     1921 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/version.py
+-rw-r--r--   0        0        0     1992 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/warnings.py
+-rw-r--r--   0        0        0    12666 2023-06-16 11:23:18.794701 litestar-2.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0    55082 1970-01-01 00:00:00.000000 litestar-2.0.0b1/PKG-INFO
```

### Comparing `litestar-2.0.0a7/LICENSE` & `litestar-2.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/README.md` & `litestar-2.0.0b1/docs/PYPI_README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 <!-- markdownlint-disable -->
 <p align="center">
-  <img src="artwork/banner-light.svg#gh-light-mode-only" alt="Litestar Logo - Light" width="100%" height="auto" />
-  <img src="artwork/banner-dark.svg#gh-dark-mode-only" alt="Litestar Logo - Dark" width="100%" height="auto" />
+  <img src="artwork/banner-light.svg" alt="Litestar Logo - Light" width="100%" height="auto" />
 </p>
 <!-- markdownlint-restore -->
 
 <div align="center">
 
 [![ci](https://github.com/litestar-org/litestar/actions/workflows/ci.yaml/badge.svg)](https://github.com/litestar-org/litestar/actions/workflows/ci.yaml)
 [![PyPI - Version](https://badge.fury.io/py/litestar.svg)](https://badge.fury.io/py/litestar)
@@ -16,15 +15,15 @@
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 
 <!-- prettier-ignore-start -->
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-101-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-102-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 <!-- prettier-ignore-end -->
 
 [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestarapi?label=r%2FLitestar&logo=reddit)](https://reddit.com/r/litestarapi)
 [![Discord](https://img.shields.io/discord/919193495116337154?color=blue&label=chat%20on%20discord&logo=discord)](https://discord.gg/X3FJqy8d2j)
 [![Matrix](https://img.shields.io/badge/%5Bm%5D%20chat%20on%20Matrix-bridged-blue)](https://matrix.to/#/#litestar:matrix.org)
 [![Medium](https://img.shields.io/badge/Medium-12100E?style=flat&logo=medium&logoColor=white)](https://blog.litestar.dev)
@@ -49,15 +48,15 @@
 pip install litestar
 ```
 
 **Litestar 2.0 is coming out soon**, bringing many new features and improvements.
 You can check out the alpha version by instead running
 
 ```shell
-pip install litestar==2.0.0alpha6
+pip install litestar==2.0.0alpha7
 ```
 
 ## Quick Start
 
 ```python
 from litestar import Litestar, get
 
@@ -410,14 +409,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://sanderwegter.nl"><img src="https://avatars.githubusercontent.com/u/7465799?v=4?s=100" width="100px;" alt="Sander"/><br /><sub><b>Sander</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=SanderWegter" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/erhuabushuo"><img src="https://avatars.githubusercontent.com/u/1642364?v=4?s=100" width="100px;" alt="疯人院主任"/><br /><sub><b>疯人院主任</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=erhuabushuo" title="Documentation">📖</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/aviral-nayya"><img src="https://avatars.githubusercontent.com/u/121891493?v=4?s=100" width="100px;" alt="aviral-nayya"/><br /><sub><b>aviral-nayya</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=aviral-nayya" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/whiskeyriver"><img src="https://avatars.githubusercontent.com/u/162092?v=4?s=100" width="100px;" alt="whiskeyriver"/><br /><sub><b>whiskeyriver</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=whiskeyriver" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://hexcode.tech"><img src="https://avatars.githubusercontent.com/u/419606?v=4?s=100" width="100px;" alt="Phyo Arkar Lwin"/><br /><sub><b>Phyo Arkar Lwin</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=v3ss0n" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/MatthewNewland"><img src="https://avatars.githubusercontent.com/u/9618670?v=4?s=100" width="100px;" alt="MatthewNewland"/><br /><sub><b>MatthewNewland</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3AMatthewNewland" title="Bug reports">🐛</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `litestar-2.0.0a7/litestar/__init__.py` & `litestar-2.0.0b1/litestar/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/_asgi/asgi_router.py` & `litestar-2.0.0b1/litestar/_asgi/asgi_router.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/_asgi/routing_trie/mapping.py` & `litestar-2.0.0b1/litestar/_asgi/routing_trie/mapping.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/_asgi/routing_trie/traversal.py` & `litestar-2.0.0b1/litestar/_asgi/routing_trie/traversal.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/_asgi/routing_trie/types.py` & `litestar-2.0.0b1/litestar/_asgi/routing_trie/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/_asgi/routing_trie/validate.py` & `litestar-2.0.0b1/litestar/_asgi/routing_trie/validate.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/_asgi/utils.py` & `litestar-2.0.0b1/litestar/_asgi/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/_kwargs/cleanup.py` & `litestar-2.0.0b1/litestar/_kwargs/cleanup.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/_kwargs/dependencies.py` & `litestar-2.0.0b1/litestar/_kwargs/dependencies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/_kwargs/extractors.py` & `litestar-2.0.0b1/litestar/_kwargs/extractors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from collections import defaultdict
 from functools import lru_cache
-from typing import TYPE_CHECKING, Any, Callable, Coroutine, DefaultDict, cast
+from typing import TYPE_CHECKING, Any, Callable, Coroutine, cast
 
 from litestar._multipart import parse_multipart_form
 from litestar._parsers import (
     parse_headers,
     parse_query_string,
     parse_url_encoded_form_data,
 )
@@ -86,25 +86,25 @@
 
     return extractor
 
 
 @lru_cache(1024)
 def create_query_default_dict(
     parsed_query: tuple[tuple[str, str], ...], sequence_query_parameter_names: tuple[str, ...]
-) -> DefaultDict[str, list[str] | str]:
+) -> defaultdict[str, list[str] | str]:
     """Transform a list of tuples into a default dict. Ensures non-list values are not wrapped in a list.
 
     Args:
         parsed_query: The parsed query list of tuples.
         sequence_query_parameter_names: A set of query parameters that should be wrapped in list.
 
     Returns:
         A default dict
     """
-    output: DefaultDict[str, list[str] | str] = defaultdict(list)
+    output: defaultdict[str, list[str] | str] = defaultdict(list)
 
     for k, v in parsed_query:
         if k in sequence_query_parameter_names:
             output[k].append(v)  # type: ignore
         else:
             output[k] = v
```

### Comparing `litestar-2.0.0a7/litestar/_kwargs/kwargs_model.py` & `litestar-2.0.0b1/litestar/_kwargs/kwargs_model.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/_kwargs/parameter_definition.py` & `litestar-2.0.0b1/litestar/_kwargs/parameter_definition.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/_layers/utils.py` & `litestar-2.0.0b1/litestar/_layers/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/_multipart.py` & `litestar-2.0.0b1/litestar/_multipart.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 SOFTWARE.
 """
 from __future__ import annotations
 
 import re
 from collections import defaultdict
 from email.utils import decode_rfc2231
-from typing import Any, DefaultDict
+from typing import Any
 from urllib.parse import unquote
 
 from litestar.datastructures.upload_file import UploadFile
 from litestar.exceptions import SerializationException, ValidationException
 from litestar.serialization import decode_json
 
 __all__ = ("parse_body", "parse_content_header", "parse_multipart_form")
@@ -98,15 +98,15 @@
         boundary: Boundary of the multipart message.
         multipart_form_part_limit: Limit of the number of parts allowed.
 
     Returns:
         A dictionary of parsed results.
     """
 
-    fields: DefaultDict[str, list[Any]] = defaultdict(list)
+    fields: defaultdict[str, list[Any]] = defaultdict(list)
 
     for form_part in parse_body(body=body, boundary=boundary, multipart_form_part_limit=multipart_form_part_limit):
         file_name = None
         content_type = "text/plain"
         content_charset = "utf-8"
         field_name = None
         line_index = 2
```

### Comparing `litestar-2.0.0a7/litestar/_openapi/parameters.py` & `litestar-2.0.0b1/litestar/_openapi/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
             field_type=path_parameter.type,
             kwarg_model=field.kwarg_model,
             name=field.name,
         ),
         generate_examples=generate_examples,
         plugins=[],
         schemas=schemas,
+        prefer_alias=True,
     )
 
 
 class ParameterCollection:
     """Facilitates conditional deduplication of parameters.
 
     If multiple parameters with the same name are produced for a handler, the condition is ignored if the two
@@ -124,15 +125,17 @@
         is_required = signature_field.is_required
     else:
         is_required = signature_field.is_required
         param_in = ParamType.QUERY
         parameter_name = kwargs_model.query if kwargs_model and kwargs_model.query else parameter_name
 
     if not result:
-        result = create_schema(field=signature_field, generate_examples=generate_examples, plugins=[], schemas=schemas)
+        result = create_schema(
+            field=signature_field, generate_examples=generate_examples, plugins=[], schemas=schemas, prefer_alias=True
+        )
 
     schema = result if isinstance(result, Schema) else schemas[result.value]
 
     return Parameter(
         description=schema.description,
         name=parameter_name,
         param_in=param_in,
```

### Comparing `litestar-2.0.0a7/litestar/_openapi/path_item.py` & `litestar-2.0.0b1/litestar/_openapi/path_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from inspect import cleandoc
 from typing import TYPE_CHECKING
 
 from litestar._openapi.parameters import create_parameter_for_handler
 from litestar._openapi.request_body import create_request_body
 from litestar._openapi.responses import create_responses
 from litestar._openapi.utils import SEPARATORS_CLEANUP_PATTERN
-from litestar.openapi.spec.operation import Operation
 from litestar.openapi.spec.path_item import PathItem
 from litestar.utils.helpers import unwrap_partial
 
 __all__ = ("create_path_item", "extract_layered_values", "get_description_for_handler")
 
 
 if TYPE_CHECKING:
@@ -113,15 +112,15 @@
                     plugins=plugins,
                     schemas=schemas,
                 )
             operation_id = route_handler.operation_id or operation_id_creator(
                 route_handler, http_method, route.path_components
             )
             tags, security = extract_layered_values(route_handler)
-            operation = Operation(
+            operation = route_handler.operation_class(
                 operation_id=operation_id,
                 tags=tags,
                 summary=route_handler.summary or SEPARATORS_CLEANUP_PATTERN.sub("", route_handler.handler_name.title()),
                 description=get_description_for_handler(route_handler, use_handler_docstrings),
                 deprecated=route_handler.deprecated,
                 responses=create_responses(
                     route_handler=route_handler,
```

### Comparing `litestar-2.0.0a7/litestar/_openapi/request_body.py` & `litestar-2.0.0b1/litestar/_openapi/request_body.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,12 +27,14 @@
 ) -> RequestBody | None:
     """Create a RequestBody model for the given RouteHandler or return None."""
     media_type: RequestEncodingType | str = RequestEncodingType.JSON
     if isinstance(field.kwarg_model, BodyKwarg) and field.kwarg_model.media_type:
         media_type = field.kwarg_model.media_type
 
     if dto := route_handler.resolve_dto():
-        schema = dto.create_openapi_schema("data", str(route_handler), generate_examples, schemas)
+        schema = dto.create_openapi_schema("data", str(route_handler), generate_examples, schemas, True)
     else:
-        schema = create_schema(field=field, generate_examples=generate_examples, plugins=plugins, schemas=schemas)
+        schema = create_schema(
+            field=field, generate_examples=generate_examples, plugins=plugins, schemas=schemas, prefer_alias=True
+        )
 
     return RequestBody(required=True, content={media_type: OpenAPIMediaType(schema=schema)})
```

### Comparing `litestar-2.0.0a7/litestar/_openapi/responses.py` & `litestar-2.0.0b1/litestar/_openapi/responses.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,29 +4,35 @@
 from copy import copy
 from dataclasses import asdict
 from http import HTTPStatus
 from inspect import Signature
 from operator import attrgetter
 from typing import TYPE_CHECKING, Any, Iterator
 
-from typing_extensions import get_args, get_origin
-
 from litestar._openapi.schema_generation import create_schema
 from litestar._signature.field import SignatureField
 from litestar.enums import MediaType
 from litestar.exceptions import HTTPException, ValidationException
 from litestar.openapi.spec import OpenAPIResponse
 from litestar.openapi.spec.enums import OpenAPIFormat, OpenAPIType
 from litestar.openapi.spec.header import OpenAPIHeader
 from litestar.openapi.spec.media_type import OpenAPIMediaType
 from litestar.openapi.spec.schema import Schema
-from litestar.response import Response as LitestarResponse
-from litestar.response_containers import File, Redirect, Stream, Template
+from litestar.response import (
+    File,
+    Redirect,
+    Stream,
+    Template,
+)
+from litestar.response import (
+    Response as LitestarResponse,
+)
+from litestar.response.base import ASGIResponse
 from litestar.types.builtin_types import NoneType
-from litestar.utils import get_enum_string_value, get_name, is_class_and_subclass
+from litestar.utils import get_enum_string_value, get_name
 
 if TYPE_CHECKING:
     from litestar.datastructures.cookie import Cookie
     from litestar.handlers.http_handlers import HTTPRouteHandler
     from litestar.openapi.spec.responses import Responses
     from litestar.plugins import OpenAPISchemaPluginProtocol
 
@@ -65,69 +71,71 @@
 def create_success_response(  # noqa: C901
     route_handler: HTTPRouteHandler,
     generate_examples: bool,
     plugins: list[OpenAPISchemaPluginProtocol],
     schemas: dict[str, Schema],
 ) -> OpenAPIResponse:
     """Create the schema for a success response."""
-    return_annotation = route_handler.parsed_fn_signature.return_type.annotation
+    return_type = route_handler.parsed_fn_signature.return_type
+    return_annotation = return_type.annotation
     default_descriptions: dict[Any, str] = {
         Stream: "Stream Response",
         Redirect: "Redirect Response",
         File: "File Download",
     }
     description = (
         route_handler.response_description
         or default_descriptions.get(return_annotation)
         or HTTPStatus(route_handler.status_code).description
     )
 
-    if return_annotation not in {Signature.empty, None, NoneType, Redirect, File, Stream}:
+    if return_annotation is not Signature.empty and not return_type.is_subclass_of(
+        (NoneType, File, Redirect, Stream, ASGIResponse)
+    ):
         if return_annotation is Template:
             return_annotation = str
             route_handler.media_type = get_enum_string_value(MediaType.HTML)
-        elif is_class_and_subclass(get_origin(return_annotation), LitestarResponse):
-            return_annotation = get_args(return_annotation)[0] or Any
+        elif return_type.is_subclass_of(LitestarResponse):
+            return_annotation = return_type.inner_types[0].annotation if return_type.inner_types else Any
+            if not route_handler.media_type:
+                route_handler.media_type = get_enum_string_value(MediaType.JSON)
 
         if dto := route_handler.resolve_return_dto():
-            result = dto.create_openapi_schema("return", str(route_handler), generate_examples, schemas)
+            result = dto.create_openapi_schema("return", str(route_handler), generate_examples, schemas, False)
         else:
             result = create_schema(
                 field=SignatureField.create(field_type=return_annotation),
                 generate_examples=generate_examples,
                 plugins=plugins,
                 schemas=schemas,
+                prefer_alias=False,
             )
 
         schema = result if isinstance(result, Schema) else schemas[result.value]
 
         schema.content_encoding = route_handler.content_encoding
         schema.content_media_type = route_handler.content_media_type
 
         response = OpenAPIResponse(
-            content={
-                route_handler.media_type: OpenAPIMediaType(
-                    schema=result,
-                )
-            },
+            content={route_handler.media_type: OpenAPIMediaType(schema=result)},
             description=description,
         )
 
-    elif return_annotation is Redirect:
+    elif return_type.is_subclass_of(Redirect):
         response = OpenAPIResponse(
             content=None,
             description=description,
             headers={
                 "location": OpenAPIHeader(
                     schema=Schema(type=OpenAPIType.STRING), description="target path for the redirect"
                 )
             },
         )
 
-    elif return_annotation in (File, Stream):
+    elif return_type.is_subclass_of((File, Stream)):
         response = OpenAPIResponse(
             content={
                 route_handler.media_type: OpenAPIMediaType(
                     schema=Schema(
                         type=OpenAPIType.STRING,
                         content_encoding=route_handler.content_encoding or "application/octet-stream",
                         content_media_type=route_handler.content_media_type,
@@ -161,14 +169,15 @@
         for attribute_name, attribute_value in ((k, v) for k, v in asdict(response_header).items() if v is not None):
             if attribute_name == "value":
                 header.schema = create_schema(
                     field=SignatureField.create(field_type=type(attribute_value)),
                     generate_examples=False,
                     plugins=plugins,
                     schemas=schemas,
+                    prefer_alias=False,
                 )
 
             elif attribute_name != "documentation_only":
                 setattr(header, attribute_name, attribute_value)
 
         response.headers[response_header.name] = header
 
@@ -227,14 +236,15 @@
 
     for status_code, additional_response in route_handler.responses.items():
         schema = create_schema(
             field=SignatureField.create(field_type=additional_response.data_container),
             generate_examples=additional_response.generate_examples,
             plugins=plugins,
             schemas=schemas,
+            prefer_alias=False,
         )
         yield str(status_code), OpenAPIResponse(
             description=additional_response.description,
             content={additional_response.media_type: OpenAPIMediaType(schema=schema)},
         )
```

### Comparing `litestar-2.0.0a7/litestar/_openapi/schema_generation/examples.py` & `litestar-2.0.0b1/litestar/_openapi/schema_generation/examples.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/_openapi/schema_generation/schema.py` & `litestar-2.0.0b1/litestar/_openapi/schema_generation/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     DefaultDict,
     Deque,
     Dict,
     FrozenSet,
     Hashable,
     Iterable,
     List,
+    Literal,
     Mapping,
     MutableMapping,
     MutableSequence,
     OrderedDict,
     Pattern,
     Sequence,
     Set,
@@ -38,18 +39,19 @@
 )
 from litestar._openapi.schema_generation.examples import create_examples_for_field
 from litestar._openapi.schema_generation.utils import sort_schemas_and_references
 from litestar._signature.field import SignatureField
 from litestar.constants import UNDEFINED_SENTINELS
 from litestar.datastructures import UploadFile
 from litestar.exceptions import ImproperlyConfiguredException
-from litestar.openapi.spec import Reference
+from litestar.openapi.spec import Example, Reference
 from litestar.openapi.spec.enums import OpenAPIFormat, OpenAPIType
 from litestar.openapi.spec.schema import Schema, SchemaDataContainer
 from litestar.pagination import ClassicPagination, CursorPagination, OffsetPagination
+from litestar.params import BodyKwarg, ParameterKwarg
 from litestar.serialization import encode_json
 from litestar.types import DataclassProtocol, Empty, TypedDictClass
 from litestar.utils.predicates import (
     is_attrs_class,
     is_dataclass_class,
     is_optional_union,
     is_pydantic_constrained_field,
@@ -73,25 +75,27 @@
             ConstrainedFloat,
             ConstrainedFrozenSet,
             ConstrainedInt,
             ConstrainedList,
             ConstrainedSet,
             ConstrainedStr,
         )
+        from pydantic.fields import ModelField
     except ImportError:
         BaseModel = Any  # type: ignore
         ConstrainedBytes = Any  # type: ignore
         ConstrainedDate = Any  # type: ignore
         ConstrainedDecimal = Any  # type: ignore
         ConstrainedFloat = Any  # type: ignore
         ConstrainedFrozenSet = Any  # type: ignore
         ConstrainedInt = Any  # type: ignore
         ConstrainedList = Any  # type: ignore
         ConstrainedSet = Any  # type: ignore
         ConstrainedStr = Any  # type: ignore
+        ModelField = Any  # type: ignore
 
     try:
         from attrs import AttrsInstance
     except ImportError:
         AttrsInstance = Any  # type: ignore
 try:
     import pydantic
@@ -208,15 +212,15 @@
     "le": "maximum",
     "lt": "exclusiveMaximum",
     "gt": "exclusiveMinimum",
     "max_length": "maxLength",
     "min_length": "minLength",
     "max_items": "maxItems",
     "min_items": "minItems",
-    "regex": "pattern",
+    "pattern": "pattern",
     "title": "title",
     "description": "description",
     "examples": "examples",
     "external_docs": "externalDocs",
     "content_encoding": "contentEncoding",
 }
 
@@ -257,20 +261,16 @@
     int: Schema(type=OpenAPIType.INTEGER),
     list: Schema(type=OpenAPIType.ARRAY),
     set: Schema(type=OpenAPIType.ARRAY),
     str: Schema(type=OpenAPIType.STRING),
     time: Schema(type=OpenAPIType.STRING, format=OpenAPIFormat.DURATION),
     timedelta: Schema(type=OpenAPIType.STRING, format=OpenAPIFormat.DURATION),
     tuple: Schema(type=OpenAPIType.ARRAY),
-    # litestar types,
-    # the following is a hack -https://www.openapis.org/blog/2021/02/16/migrating-from-openapi-3-0-to-3-1-0
-    # the format for OA 3.1 is type + contentMediaType, for 3.0.* is type + format, we do both.
     UploadFile: Schema(
         type=OpenAPIType.STRING,
-        format="binary",  # type: ignore
         content_media_type="application/octet-stream",
     ),
     # pydantic types
     **PYDANTIC_TYPE_MAP,
 }
 
 
@@ -296,24 +296,40 @@
         A schema instance.
     """
     enum_values: list[str | int] = [v.value for v in annotation]  # type: ignore
     openapi_type = OpenAPIType.STRING if isinstance(enum_values[0], str) else OpenAPIType.INTEGER
     return Schema(type=openapi_type, enum=enum_values)
 
 
+def iter_flat_literal_args(annotation: Any) -> Iterable[Any]:
+    """Iterate over the flattened arguments of a Literal.
+
+    Args:
+        annotation: An Literal annotation.
+
+    Yields:
+        The flattened arguments of the Literal.
+    """
+    for arg in get_args(annotation):
+        if get_origin_or_inner_type(arg) is Literal:
+            yield from iter_flat_literal_args(arg)
+        else:
+            yield arg
+
+
 def create_literal_schema(annotation: Any) -> Schema:
     """Create a schema instance for a Literal.
 
     Args:
         annotation: An Literal annotation.
 
     Returns:
         A schema instance.
     """
-    args = get_args(annotation)
+    args = tuple(iter_flat_literal_args(annotation))
     schema = copy(TYPE_MAP[type(args[0])])
     if len(args) > 1:
         schema.enum = args
     else:
         schema.const = args[0]
     return schema
 
@@ -338,35 +354,38 @@
 
 
 def create_schema_for_optional_field(
     field: SignatureField,
     generate_examples: bool,
     plugins: list[OpenAPISchemaPluginProtocol],
     schemas: dict[str, Schema],
+    prefer_alias: bool,
 ) -> Schema:
     """Create a Schema for an optional SignatureField.
 
     Args:
         field: A signature field instance.
         generate_examples: Whether to generate examples if none are given.
         plugins: A list of plugins.
         schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
+        prefer_alias: Whether to prefer the alias name for the schema.
 
     Returns:
         A schema instance.
     """
     schema_or_reference = create_schema(
         field=SignatureField.create(
             field_type=make_non_optional_union(field.field_type),
             name=field.name,
             default_value=field.default_value,
         ),
         generate_examples=generate_examples,
         plugins=plugins,
         schemas=schemas,
+        prefer_alias=prefer_alias,
     )
 
     if isinstance(schema_or_reference, Schema) and isinstance(schema_or_reference.one_of, list):
         result: list[Schema | Reference] = schema_or_reference.one_of
     else:
         result = [schema_or_reference]
 
@@ -379,59 +398,88 @@
 
 
 def create_schema_for_union_field(
     field: SignatureField,
     generate_examples: bool,
     plugins: list[OpenAPISchemaPluginProtocol],
     schemas: dict[str, Schema],
+    prefer_alias: bool,
 ) -> Schema:
     """Create a Schema for a union SignatureField.
 
     Args:
         field: A signature field instance.
         generate_examples: Whether to generate examples if none are given.
         plugins: A list of plugins.
         schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
+        prefer_alias: Whether to prefer the alias name for the schema.
 
     Returns:
         A schema instance.
     """
     return Schema(
         one_of=sort_schemas_and_references(
             [
-                create_schema(field=sub_field, generate_examples=generate_examples, plugins=plugins, schemas=schemas)
+                create_schema(
+                    field=sub_field,
+                    generate_examples=generate_examples,
+                    plugins=plugins,
+                    schemas=schemas,
+                    prefer_alias=prefer_alias,
+                )
                 for sub_field in field.children or []
             ]
         )
     )
 
 
 def create_schema_for_object_type(
     field: SignatureField,
     generate_examples: bool,
     plugins: list[OpenAPISchemaPluginProtocol],
     schemas: dict[str, Schema],
+    prefer_alias: bool,
 ) -> Schema:
     """Create schema for object types (dict, Mapping, list, Sequence etc.) types.
 
     Args:
         field: A signature field instance.
         generate_examples: Whether to generate examples if none are given.
         plugins: A list of plugins.
         schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
+        prefer_alias: Whether to prefer the alias name for the schema.
 
     Returns:
         A schema instance.
     """
     if field.is_mapping:
-        return Schema(type=OpenAPIType.OBJECT)
+        return Schema(
+            type=OpenAPIType.OBJECT,
+            additional_properties=(
+                create_schema(
+                    field=field.children[1],
+                    generate_examples=generate_examples,
+                    plugins=plugins,
+                    schemas=schemas,
+                    prefer_alias=prefer_alias,
+                )
+                if field.children and len(field.children) == 2
+                else None
+            ),
+        )
 
     if field.is_non_string_sequence or field.is_non_string_iterable:
         items = [
-            create_schema(field=sub_field, generate_examples=generate_examples, plugins=plugins, schemas=schemas)
+            create_schema(
+                field=sub_field,
+                generate_examples=generate_examples,
+                plugins=plugins,
+                schemas=schemas,
+                prefer_alias=prefer_alias,
+            )
             for sub_field in (field.children or ())
         ]
 
         return Schema(
             type=OpenAPIType.ARRAY,
             items=Schema(one_of=sort_schemas_and_references(items)) if len(items) > 1 else items[0],
         )
@@ -448,22 +496,24 @@
 
 
 def create_schema_for_builtin_generics(
     field: SignatureField,
     generate_examples: bool,
     plugins: list[OpenAPISchemaPluginProtocol],
     schemas: dict[str, Schema],
+    prefer_alias: bool,
 ) -> Schema:
     """Handle builtin generic types.
 
     Args:
         field: A signature field instance.
         generate_examples: Whether to generate examples if none are given.
         plugins: A list of plugins.
         schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
+        prefer_alias: Whether to prefer the alias name for the schema.
 
     Returns:
         A schema instance.
     """
     origin = get_origin_or_inner_type(field.field_type)
 
     if origin is ClassicPagination:
@@ -473,14 +523,15 @@
                 "items": Schema(
                     type=OpenAPIType.ARRAY,
                     items=create_schema(
                         field=field.children[0],  # type: ignore[index]
                         generate_examples=generate_examples,
                         plugins=plugins,
                         schemas=schemas,
+                        prefer_alias=prefer_alias,
                     ),
                 ),
                 "page_size": Schema(type=OpenAPIType.INTEGER, description="Number of items per page."),
                 "current_page": Schema(type=OpenAPIType.INTEGER, description="Current page number."),
                 "total_pages": Schema(type=OpenAPIType.INTEGER, description="Total number of pages."),
             },
         )
@@ -492,95 +543,116 @@
                 "items": Schema(
                     type=OpenAPIType.ARRAY,
                     items=create_schema(
                         field=field.children[0],  # type: ignore[index]
                         generate_examples=generate_examples,
                         plugins=plugins,
                         schemas=schemas,
+                        prefer_alias=prefer_alias,
                     ),
                 ),
                 "limit": Schema(type=OpenAPIType.INTEGER, description="Maximal number of items to send."),
                 "offset": Schema(type=OpenAPIType.INTEGER, description="Offset from the beginning of the query."),
                 "total": Schema(type=OpenAPIType.INTEGER, description="Total number of items."),
             },
         )
 
     cursor_schema = create_schema(
-        field=field.children[0], generate_examples=False, plugins=plugins, schemas=schemas  # type: ignore[index]
+        field=field.children[0],  # type: ignore[index]
+        generate_examples=False,
+        plugins=plugins,
+        schemas=schemas,
+        prefer_alias=prefer_alias,
     )
     cursor_schema.description = "Unique ID, designating the last identifier in the given data set. This value can be used to request the 'next' batch of records."
 
     return Schema(
         type=OpenAPIType.OBJECT,
         properties={
             "items": Schema(
                 type=OpenAPIType.ARRAY,
                 items=create_schema(
                     field=field.children[1],  # type: ignore[index]
                     generate_examples=generate_examples,
                     plugins=plugins,
                     schemas=schemas,
+                    prefer_alias=prefer_alias,
                 ),
             ),
             "cursor": cursor_schema,
             "results_per_page": Schema(type=OpenAPIType.INTEGER, description="Maximal number of items to send."),
         },
     )
 
 
 def create_schema_for_pydantic_model(
     field_type: type[BaseModel],
     generate_examples: bool,
     plugins: list[OpenAPISchemaPluginProtocol],
     schemas: dict[str, Schema],
+    prefer_alias: bool,
 ) -> Schema:
     """Create a schema object for a given pydantic model class.
 
     Args:
         field_type: A pydantic model class.
         generate_examples: Whether to generate examples if none are given.
         plugins: A list of plugins.
         schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
+        prefer_alias: Whether to prefer the alias over the field name.
 
     Returns:
         A schema instance.
     """
 
     field_type_hints = get_type_hints(field_type)
+    model_config = getattr(field_type, "__config__", getattr(field_type, "model_config", Empty))
+    title = getattr(model_config, "title", None) if not isinstance(model_config, dict) else model_config.get("title")
+    example = (
+        getattr(model_config, "example", None) if not isinstance(model_config, dict) else model_config.get("example")
+    )
+
+    def get_name(f: ModelField) -> str:
+        return (f.alias or f.name) if prefer_alias else f.name
+
     return Schema(
-        required=sorted([field.alias or field.name for field in field_type.__fields__.values() if field.required]),
+        required=sorted(get_name(field) for field in field_type.__fields__.values() if field.required),
         properties={
-            (f.alias or f.name): create_schema(
+            get_name(f): create_schema(
                 field=SignatureField.create(
-                    field_type=field_type_hints[f.name], name=f.alias or f.name, default_value=f.field_info
+                    field_type=field_type_hints[f.name], name=get_name(f), default_value=f.field_info
                 ),
                 generate_examples=generate_examples,
                 plugins=plugins,
                 schemas=schemas,
+                prefer_alias=prefer_alias,
             )
             for f in field_type.__fields__.values()
         },
         type=OpenAPIType.OBJECT,
-        title=_get_type_schema_name(field_type),
+        title=title or _get_type_schema_name(field_type),
+        examples=[Example(example)] if example else None,
     )
 
 
 def create_schema_for_attrs_class(
     field_type: type[AttrsInstance],
     generate_examples: bool,
     plugins: list[OpenAPISchemaPluginProtocol],
     schemas: dict[str, Schema],
+    prefer_alias: bool,
 ) -> Schema:
     """Create a schema object for a given attrs class.
 
     Args:
         field_type: An attrs class.
         generate_examples: Whether to generate examples if none are given.
         plugins: A list of plugins.
         schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
+        prefer_alias: Whether to prefer the alias name for the schema.
 
     Returns:
         A schema instance.
     """
     from attr import NOTHING
     from attrs import fields_dict
 
@@ -595,35 +667,38 @@
         ),
         properties={
             k: create_schema(
                 field=SignatureField.create(field_type=v, name=k),
                 generate_examples=generate_examples,
                 plugins=plugins,
                 schemas=schemas,
+                prefer_alias=prefer_alias,
             )
             for k, v in field_type_hints.items()
         },
         type=OpenAPIType.OBJECT,
         title=_get_type_schema_name(field_type),
     )
 
 
 def create_schema_for_struct_class(
     field_type: type[Struct],
     generate_examples: bool,
     plugins: list[OpenAPISchemaPluginProtocol],
     schemas: dict[str, Schema],
+    prefer_alias: bool,
 ) -> Schema:
     """Create a schema object for a given msgspec.Struct class.
 
     Args:
         field_type: A msgspec.Struct class.
         generate_examples: Whether to generate examples if none are given.
         plugins: A list of plugins.
         schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
+        prefer_alias: Whether to prefer the alias name for the schema.
 
     Returns:
         A schema instance.
     """
 
     return Schema(
         required=sorted(
@@ -635,35 +710,38 @@
         ),
         properties={
             field.encode_name: create_schema(
                 field=SignatureField.create(field_type=field.type, name=field.encode_name),
                 generate_examples=generate_examples,
                 plugins=plugins,
                 schemas=schemas,
+                prefer_alias=prefer_alias,
             )
             for field in msgspec_struct_fields(field_type)
         },
         type=OpenAPIType.OBJECT,
         title=_get_type_schema_name(field_type),
     )
 
 
 def create_schema_for_dataclass(
     field_type: type[DataclassProtocol],
     generate_examples: bool,
     plugins: list[OpenAPISchemaPluginProtocol],
     schemas: dict[str, Schema],
+    prefer_alias: bool,
 ) -> Schema:
     """Create a schema object for a given dataclass class.
 
     Args:
         field_type: A dataclass class.
         generate_examples: Whether to generate examples if none are given.
         plugins: A list of plugins.
         schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
+        prefer_alias: Whether to prefer the alias name for the schema.
 
     Returns:
         A schema instance.
     """
     field_type_hints = get_type_hints(field_type)
     return Schema(
         required=sorted(
@@ -679,69 +757,75 @@
         ),
         properties={
             k: create_schema(
                 field=SignatureField.create(field_type=v, name=k),
                 generate_examples=generate_examples,
                 plugins=plugins,
                 schemas=schemas,
+                prefer_alias=prefer_alias,
             )
             for k, v in field_type_hints.items()
         },
         type=OpenAPIType.OBJECT,
         title=_get_type_schema_name(field_type),
     )
 
 
 def create_schema_for_typed_dict(
     field_type: TypedDictClass,
     generate_examples: bool,
     plugins: list[OpenAPISchemaPluginProtocol],
     schemas: dict[str, Schema],
+    prefer_alias: bool,
 ) -> Schema:
     """Create a schema object for a given typed dict.
 
     Args:
         field_type: A typed-dict class.
         generate_examples: Whether to generate examples if none are given.
         plugins: A list of plugins.
         schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
+        prefer_alias: Whether to prefer the alias name for the schema.
 
     Returns:
         A schema instance.
     """
     return Schema(
         required=sorted(getattr(field_type, "__required_keys__", [])),
         properties={
             k: create_schema(
                 field=SignatureField.create(field_type=v, name=k),
                 generate_examples=generate_examples,
                 plugins=plugins,
                 schemas=schemas,
+                prefer_alias=prefer_alias,
             )
             for k, v in get_type_hints(field_type).items()
         },
         type=OpenAPIType.OBJECT,
         title=_get_type_schema_name(field_type),
     )
 
 
 def create_schema_for_plugin(
     field: SignatureField,
     generate_examples: bool,
     plugins: list[OpenAPISchemaPluginProtocol],
     schemas: dict[str, Schema],
+    prefer_alias: bool,
     plugin: OpenAPISchemaPluginProtocol,
 ) -> Schema | Reference:
     """Create a schema using a plugin.
 
     Args:
         field: A signature field instance.
         generate_examples: Whether to generate examples if none are given.
         plugins: A list of plugins.
         schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
+        prefer_alias: Whether to prefer the alias name for the schema.
         plugin: A plugin for the field type.
 
     Returns:
         A schema instance.
     """
 
     schema: Schema | Reference = plugin.to_openapi_schema(field.field_type)
@@ -753,14 +837,15 @@
                 default_value=field.default_value,
                 extra=field.extra,
                 kwarg_model=field.kwarg_model,
             ),
             generate_examples=generate_examples,
             plugins=plugins,
             schemas=schemas,
+            prefer_alias=prefer_alias,
         )
     return schema  # pragma: no cover
 
 
 def _process_schema_result(
     field: SignatureField,
     schema: Schema,
@@ -795,85 +880,131 @@
 
 
 def create_schema(
     field: SignatureField,
     generate_examples: bool,
     plugins: list[OpenAPISchemaPluginProtocol],
     schemas: dict[str, Schema],
+    prefer_alias: bool,
 ) -> Schema | Reference:
     """Create a Schema for a given SignatureField.
 
     Args:
         field: A signature field instance.
         generate_examples: Whether to generate examples if none are given.
         plugins: A list of plugins.
         schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
+        prefer_alias: Whether to prefer the alias name for the schema.
 
     Returns:
         A schema instance.
     """
     if field.is_optional:
         result: Schema | Reference = create_schema_for_optional_field(
-            field=field, generate_examples=generate_examples, plugins=plugins, schemas=schemas
+            field=field,
+            generate_examples=generate_examples,
+            plugins=plugins,
+            schemas=schemas,
+            prefer_alias=prefer_alias,
         )
 
     elif field.is_union:
         result = create_schema_for_union_field(
-            field=field, generate_examples=generate_examples, plugins=plugins, schemas=schemas
+            field=field,
+            generate_examples=generate_examples,
+            plugins=plugins,
+            schemas=schemas,
+            prefer_alias=prefer_alias,
         )
 
     elif is_pydantic_model_class(annotation=field.field_type):
         result = create_schema_for_pydantic_model(
-            field_type=field.field_type, generate_examples=generate_examples, plugins=plugins, schemas=schemas
+            field_type=field.field_type,
+            generate_examples=generate_examples,
+            plugins=plugins,
+            schemas=schemas,
+            prefer_alias=prefer_alias,
         )
 
     elif is_attrs_class(annotation=field.field_type):
         result = create_schema_for_attrs_class(
-            field_type=field.field_type, generate_examples=generate_examples, plugins=plugins, schemas=schemas
+            field_type=field.field_type,
+            generate_examples=generate_examples,
+            plugins=plugins,
+            schemas=schemas,
+            prefer_alias=prefer_alias,
         )
 
     elif is_struct_class(annotation=field.field_type):
         result = create_schema_for_struct_class(
-            field_type=field.field_type, generate_examples=generate_examples, plugins=plugins, schemas=schemas
+            field_type=field.field_type,
+            generate_examples=generate_examples,
+            plugins=plugins,
+            schemas=schemas,
+            prefer_alias=prefer_alias,
         )
 
     elif is_dataclass_class(annotation=field.field_type):
         result = create_schema_for_dataclass(
-            field_type=field.field_type, generate_examples=generate_examples, plugins=plugins, schemas=schemas
+            field_type=field.field_type,
+            generate_examples=generate_examples,
+            plugins=plugins,
+            schemas=schemas,
+            prefer_alias=prefer_alias,
         )
 
     elif is_typed_dict(annotation=field.field_type):
         result = create_schema_for_typed_dict(
-            field_type=field.field_type, generate_examples=generate_examples, plugins=plugins, schemas=schemas
+            field_type=field.field_type,
+            generate_examples=generate_examples,
+            plugins=plugins,
+            schemas=schemas,
+            prefer_alias=prefer_alias,
         )
 
     elif plugins_for_annotation := [plugin for plugin in plugins if plugin.is_plugin_supported_type(field.field_type)]:
         result = create_schema_for_plugin(
             field=field,
             generate_examples=generate_examples,
             plugins=plugins,
             schemas=schemas,
+            prefer_alias=prefer_alias,
             plugin=plugins_for_annotation[0],
         )
 
-    elif is_pydantic_constrained_field(field.field_type):
+    elif is_pydantic_constrained_field(field.field_type) or (
+        isinstance(field.kwarg_model, (ParameterKwarg, BodyKwarg)) and field.kwarg_model.is_constrained
+    ):
         result = create_constrained_field_schema(
-            field_type=field.field_type, children=field.children, plugins=plugins, schemas=schemas
+            field_type=field.field_type,
+            children=field.children,
+            plugins=plugins,
+            schemas=schemas,
+            prefer_alias=prefer_alias,
+            kwargs_model=field.kwarg_model,  # type: ignore[arg-type]
         )
 
     elif field.children and not field.is_generic:
         result = create_schema_for_object_type(
-            field=field, generate_examples=generate_examples, plugins=plugins, schemas=schemas
+            field=field,
+            generate_examples=generate_examples,
+            plugins=plugins,
+            schemas=schemas,
+            prefer_alias=prefer_alias,
         )
 
     elif field.is_generic and (
         get_origin_or_inner_type(field.field_type) in (ClassicPagination, CursorPagination, OffsetPagination)
     ):
         result = create_schema_for_builtin_generics(
-            field=field, generate_examples=generate_examples, plugins=plugins, schemas=schemas
+            field=field,
+            generate_examples=generate_examples,
+            plugins=plugins,
+            schemas=schemas,
+            prefer_alias=prefer_alias,
         )
     else:
         result = create_schema_for_annotation(annotation=field.field_type) or Schema()
 
     if isinstance(result, Reference):
         return result
```

### Comparing `litestar-2.0.0a7/litestar/_openapi/schema_generation/utils.py` & `litestar-2.0.0b1/litestar/_openapi/schema_generation/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/_openapi/typescript_converter/converter.py` & `litestar-2.0.0b1/litestar/_openapi/typescript_converter/converter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/_openapi/typescript_converter/schema_parsing.py` & `litestar-2.0.0b1/litestar/_openapi/typescript_converter/schema_parsing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/_openapi/typescript_converter/types.py` & `litestar-2.0.0b1/litestar/_openapi/typescript_converter/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/_openapi/utils.py` & `litestar-2.0.0b1/litestar/_openapi/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/_parsers.py` & `litestar-2.0.0b1/litestar/_parsers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/_signature/field.py` & `litestar-2.0.0b1/litestar/_signature/field.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,34 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Any, Literal
 
-from msgspec import Meta
 from pydantic.fields import FieldInfo
 from typing_extensions import Annotated, get_args, get_origin
 
+from litestar._signature.metadata import _create_metadata_from_type
 from litestar.constants import UNDEFINED_SENTINELS
 from litestar.params import BodyKwarg, DependencyKwarg, ParameterKwarg
 from litestar.types import Empty
 from litestar.utils.predicates import (
     is_any,
     is_generic,
     is_mapping,
     is_non_string_iterable,
     is_non_string_sequence,
     is_optional_union,
+    is_pydantic_constrained_field,
     is_union,
 )
-from litestar.utils.typing import make_non_optional_union
+from litestar.utils.typing import make_non_optional_union, normalize_type_annotation
 
 __all__ = ("SignatureField",)
 
 
-def _create_metadata_from_type(
-    value: Any, model: type[ParameterKwarg] | type[BodyKwarg], field_type: Any
-) -> ParameterKwarg | BodyKwarg | None:
-    if isinstance(value, Meta):
-        is_sequence_container = is_non_string_sequence(field_type)
-        return model(
-            gt=value.gt,
-            ge=value.ge,
-            lt=value.lt,
-            le=value.le,
-            multiple_of=value.multiple_of,
-            regex=value.pattern,
-            min_length=value.min_length if not is_sequence_container else None,
-            max_length=value.max_length if not is_sequence_container else None,
-            min_items=value.min_length if is_sequence_container else None,
-            max_items=value.max_length if is_sequence_container else None,
-        )
-    if isinstance(value, FieldInfo):
-        values: dict[str, Any] = {
-            k: v
-            for k, v in {
-                "gt": value.gt,
-                "ge": value.ge,
-                "lt": value.lt,
-                "le": value.le,
-                "multiple_of": value.multiple_of,
-                "regex": value.regex,
-                "min_length": value.min_length,
-                "max_length": value.max_length,
-                "min_items": value.min_items,
-                "max_items": value.max_items,
-                "description": value.description,
-                "title": value.title,
-                "const": value.const is not None,
-            }.items()
-            if v is not None
-        }
-        if values:
-            return model(**values)
-    return None
-
-
 @dataclass(unsafe_hash=True, frozen=True)
 class SignatureField:
     """Abstraction representing a model field. This class is meant to replace equivalent datastructures from other
     libraries, for example, pydantic or msgspec.
     """
 
     __slots__ = (
@@ -207,34 +166,39 @@
             children: A mapping of subtypes, if any.
             kwarg_model: Kwarg Parameter.
             extra: A mapping of extra values.
 
         Returns:
             SignatureField instance.
         """
-        if kwarg_model and default_value is Empty:
-            default_value = kwarg_model.default
+        if kwarg_model:
+            if default_value is Empty:
+                default_value = kwarg_model.default
 
-        elif isinstance(default_value, FieldInfo) and not kwarg_model:
+        elif isinstance(default_value, FieldInfo):
             kwarg_model = _create_metadata_from_type(
-                default_value, BodyKwarg if name == "data" else ParameterKwarg, field_type=field_type
+                value=default_value, model=BodyKwarg if name == "data" else ParameterKwarg, field_type=field_type
             )
 
+        # this is for pydantic v1 only
+        elif is_pydantic_constrained_field(field_type):
+            kwarg_model = _create_metadata_from_type(value=field_type, model=ParameterKwarg, field_type=field_type)
+
         origin = get_origin(field_type)
 
         if not children and origin and (type_args := get_args(field_type)):
             if origin is Annotated:
-                field_type = type_args[0]
+                field_type = normalize_type_annotation(type_args[0])
                 kwarg_model = kwarg_model or _create_metadata_from_type(
-                    type_args[1], BodyKwarg if name == "data" else ParameterKwarg, field_type=field_type
+                    value=type_args[1], model=BodyKwarg if name == "data" else ParameterKwarg, field_type=field_type
                 )
             else:
                 children = tuple(SignatureField.create(arg) for arg in type_args)
 
         return SignatureField(
             name=name,
-            field_type=field_type if field_type is not Empty else Any,
+            field_type=normalize_type_annotation(field_type) if field_type is not Empty else Any,
             default_value=default_value if default_value not in UNDEFINED_SENTINELS else Empty,
             children=children,
             kwarg_model=kwarg_model,
             extra=extra or {},
         )
```

### Comparing `litestar-2.0.0a7/litestar/_signature/models/attrs_signature_model.py` & `litestar-2.0.0b1/litestar/_signature/models/attrs_signature_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,16 +217,21 @@
         self._structure_func._function_dispatch._handler_pairs[-1] = (
             *_create_default_structuring_hooks(self),
             False,
         )
 
         # ensure attrs instances are not unstructured into dict
         self.register_unstructure_hook_factory(
-            lambda value: attrs.has(value) and AttrsSignatureModel not in list(value.__mro__),
-            _pass_through_unstructure_hook,
+            # the first parameter is a predicate that tests the value. In this case we are testing for an attrs
+            # decorated class that does not have the AttrsSignatureModel anywhere in its mro chain.
+            lambda x: attrs.has(x) and AttrsSignatureModel not in list(x.__mro__),
+            # the "unstructuring" hook we are registering is a lambda that receives the class constructor and returns
+            # another lambda that will take a value and receive it unmodified.
+            # this is a hack to ensure that no attrs constructors are called during unstructuring.
+            lambda x: lambda x: x,
         )
 
         for cls, structure_hook in hooks:
             self.register_structure_hook(cls, structure_hook)
             self.register_unstructure_hook(cls, _pass_through_unstructure_hook)
 
 
@@ -270,15 +275,15 @@
         (kwargs_model.ge, attrs.validators.ge),
         (kwargs_model.lt, attrs.validators.lt),
         (kwargs_model.le, attrs.validators.le),
         (kwargs_model.min_length, attrs.validators.min_len),
         (kwargs_model.max_length, attrs.validators.max_len),
         (kwargs_model.min_items, attrs.validators.min_len),
         (kwargs_model.max_items, attrs.validators.max_len),
-        (kwargs_model.regex, partial(attrs.validators.matches_re, flags=0)),
+        (kwargs_model.pattern, partial(attrs.validators.matches_re, flags=0)),
     ]:
         if value is not None:
             validators.append(validator(value))  # type: ignore
 
     if is_optional_union(annotation):
         annotation = make_non_optional_union(annotation)
         instance_of_validator = attrs.validators.instance_of(
```

### Comparing `litestar-2.0.0a7/litestar/_signature/models/base.py` & `litestar-2.0.0b1/litestar/_signature/models/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/_signature/models/pydantic_signature_model.py` & `litestar-2.0.0b1/litestar/_signature/models/pydantic_signature_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,28 +71,30 @@
             A SignatureField
         """
         children = (
             tuple(cls.signature_field_from_model_field(sub_field) for sub_field in model_field.sub_fields)
             if model_field.sub_fields
             else None
         )
+
         default_value = (
             model_field.field_info.default if model_field.field_info.default not in UNDEFINED_SENTINELS else Empty
         )
 
         kwarg_model: ParameterKwarg | DependencyKwarg | BodyKwarg | None = model_field.field_info.extra.pop(
             "kwargs_model", None
         )
         if kwarg_model:
             default_value = kwarg_model.default
+
         elif isinstance(default_value, (ParameterKwarg, DependencyKwarg, BodyKwarg)):
             kwarg_model = default_value
             default_value = default_value.default
 
-        return SignatureField(
+        return SignatureField.create(
             children=children,
             default_value=default_value,
             extra=model_field.field_info.extra or {},
             field_type=model_field.annotation if model_field.annotation is not Empty else Any,
             kwarg_model=kwarg_model,
             name=model_field.name,
         )
```

### Comparing `litestar-2.0.0a7/litestar/_signature/utils.py` & `litestar-2.0.0b1/litestar/_signature/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,26 @@
 from __future__ import annotations
 
 from inspect import getmembers, isclass
 from typing import TYPE_CHECKING, Any, Literal, cast
 
+import pydantic
+
+from litestar._signature.models.pydantic_signature_model import PydanticSignatureModel
 from litestar.constants import SKIP_VALIDATION_NAMES
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.params import DependencyKwarg
 from litestar.types import AnyCallable, Empty
 from litestar.utils.helpers import unwrap_partial
 from litestar.utils.predicates import is_attrs_class
 
-try:
-    import pydantic
-
-    from litestar._signature.models.pydantic_signature_model import PydanticSignatureModel
+pydantic_types: tuple[Any, ...] = tuple(
+    cls for _, cls in getmembers(pydantic.types, isclass) if "pydantic.types" in repr(cls)
+)
 
-    pydantic_types: tuple[Any, ...] = tuple(
-        cls for _, cls in getmembers(pydantic.types, isclass) if "pydantic.types" in repr(cls)
-    )
-except ImportError:  # pragma: no cover
-    PydanticSignatureModel = Empty  # type: ignore
-    pydantic_types = ()
-
-try:
-    from litestar._signature.models.attrs_signature_model import AttrsSignatureModel
-except ImportError:
-    AttrsSignatureModel = Empty  # type: ignore
 
 if TYPE_CHECKING:
     from typing_extensions import TypeAlias
 
     from litestar._signature.models.base import SignatureModel
     from litestar.utils.signature import ParsedParameter, ParsedSignature
 
@@ -43,23 +34,25 @@
 
 
 def create_signature_model(
     dependency_name_set: set[str],
     fn: AnyCallable,
     preferred_validation_backend: Literal["pydantic", "attrs"],
     parsed_signature: ParsedSignature,
+    has_data_dto: bool = False,
 ) -> type[SignatureModel]:
     """Create a model for a callable's signature. The model can than be used to parse and validate before passing it to
     the callable.
 
     Args:
         dependency_name_set: A set of dependency names
         fn: A callable.
         preferred_validation_backend: Validation/Parsing backend to prefer, if installed
         parsed_signature: A parsed signature for the handler/dependency function.
+        has_data_dto: Is a data DTO defined for the handler?
 
     Returns:
         A signature model.
     """
 
     unwrapped_fn = cast("AnyCallable", unwrap_partial(fn))
     fn_name = getattr(fn, "__name__", "anonymous")
@@ -72,15 +65,15 @@
         dependency_name_set=dependency_name_set, fn=unwrapped_fn, parsed_signature=parsed_signature
     )
 
     model_class = _get_signature_model_type(
         preferred_validation_backend=preferred_validation_backend, parsed_signature=parsed_signature
     )
 
-    type_overrides = _create_type_overrides(parsed_signature)
+    type_overrides = _create_type_overrides(parsed_signature, has_data_dto)
 
     return model_class.create(
         fn_name=fn_name,
         fn_module=fn_module,
         parsed_signature=parsed_signature,
         dependency_names={*dependency_name_set, *dependency_names},
         type_overrides=type_overrides,
@@ -99,49 +92,33 @@
     for parameter in parsed_signature.parameters.values():
         parsed_type = parameter.parsed_type
         if any(is_attrs_class(t.annotation) for t in parsed_type.inner_types) or is_attrs_class(parsed_type.annotation):
             return True
     return False
 
 
-def _any_pydantic_annotation(parsed_signature: ParsedSignature) -> bool:
-    for parameter in parsed_signature.parameters.values():
-        parsed_type = parameter.parsed_type
-        if any(_is_pydantic_annotation(t.annotation) for t in parsed_type.inner_types) or _is_pydantic_annotation(
-            parsed_type.annotation
-        ):
-            return True
-    return False
-
-
-def _create_type_overrides(parsed_signature: ParsedSignature) -> dict[str, Any]:
+def _create_type_overrides(parsed_signature: ParsedSignature, has_data_dto: bool) -> dict[str, Any]:
     type_overrides = {}
     for parameter in parsed_signature.parameters.values():
         if _should_skip_validation(parameter):
             type_overrides[parameter.name] = Any
+        if has_data_dto and "data" in parsed_signature.parameters:
+            type_overrides["data"] = Any
     return type_overrides
 
 
 def _get_signature_model_type(
     preferred_validation_backend: Literal["pydantic", "attrs"],
     parsed_signature: ParsedSignature,
 ) -> type[SignatureModel]:
-    pydantic_installed = PydanticSignatureModel is not Empty  # type: ignore[comparison-overlap]
-    attrs_installed = AttrsSignatureModel is not Empty  # type: ignore[comparison-overlap]
-    if (
-        pydantic_installed
-        and (not attrs_installed or not _any_attrs_annotation(parsed_signature))
-        and (preferred_validation_backend == "pydantic" or _any_pydantic_annotation(parsed_signature))
-    ):
-        return cast(SignatureModelType, PydanticSignatureModel)
-    return cast(SignatureModelType, AttrsSignatureModel)
-
+    if preferred_validation_backend == "attrs" or _any_attrs_annotation(parsed_signature):
+        from litestar._signature.models.attrs_signature_model import AttrsSignatureModel
 
-def _is_pydantic_annotation(annotation: Any) -> bool:
-    return annotation in pydantic_types or hasattr(annotation, "__get_validators__")
+        return AttrsSignatureModel
+    return PydanticSignatureModel
 
 
 def _should_skip_validation(parameter: ParsedParameter) -> bool:
     """Whether the parameter should skip validation.
 
     Returns:
         A boolean indicating whether the parameter should be validated.
```

### Comparing `litestar-2.0.0a7/litestar/app.py` & `litestar-2.0.0b1/litestar/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from __future__ import annotations
 
 import inspect
 import logging
+import os
 from contextlib import AbstractAsyncContextManager, AsyncExitStack, asynccontextmanager
 from datetime import date, datetime, time, timedelta
 from functools import partial
 from itertools import chain
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, AsyncGenerator, Callable, Literal, Mapping, Sequence, cast
-
-from typing_extensions import Self, TypedDict
+from typing import TYPE_CHECKING, Any, AsyncGenerator, Callable, Literal, Mapping, Sequence, TypedDict, cast
 
 from litestar._asgi import ASGIRouter
 from litestar._asgi.utils import get_route_handlers, wrap_in_exception_handler
 from litestar._openapi.path_item import create_path_item
 from litestar.config.allowed_hosts import AllowedHostsConfig
 from litestar.config.app import AppConfig
 from litestar.config.response_cache import ResponseCacheConfig
@@ -36,23 +35,22 @@
 )
 from litestar.router import Router
 from litestar.routes import ASGIRoute, HTTPRoute, WebSocketRoute
 from litestar.static_files.base import StaticFiles
 from litestar.stores.registry import StoreRegistry
 from litestar.types import Empty
 from litestar.types.internal_types import PathParameterDefinition
-from litestar.utils import (
-    as_async_callable_list,
-    is_async_callable,
-    join_paths,
-    unique,
-)
+from litestar.utils import AsyncCallable, join_paths, unique, warn_deprecation
 from litestar.utils.dataclass import extract_dataclass_items
+from litestar.utils.predicates import is_async_callable
+from litestar.utils.warnings import warn_pdb_on_exception
 
 if TYPE_CHECKING:
+    from typing_extensions import Self
+
     from litestar.config.compression import CompressionConfig
     from litestar.config.cors import CORSConfig
     from litestar.config.csrf import CSRFConfig
     from litestar.datastructures import CacheControlHeader, ETag, ResponseHeader
     from litestar.dto.interface import DTOInterface
     from litestar.events.listener import EventListener
     from litestar.logging.config import BaseLoggingConfig
@@ -127,14 +125,15 @@
     and Route Handlers should be registered on it.
     """
 
     __slots__ = (
         "_lifespan_managers",
         "_debug",
         "_openapi_schema",
+        "_preferred_validation_backend",
         "after_exception",
         "allowed_hosts",
         "asgi_handler",
         "asgi_router",
         "before_send",
         "compression_config",
         "cors_config",
@@ -144,25 +143,25 @@
         "logger",
         "logging_config",
         "multipart_form_part_limit",
         "on_shutdown",
         "on_startup",
         "openapi_config",
         "openapi_schema_plugins",
-        "preferred_validation_backend",
         "request_class",
         "response_cache_config",
         "route_map",
         "serialization_plugins",
         "signature_namespace",
         "state",
         "static_files_config",
         "stores",
         "template_engine",
         "websocket_class",
+        "pdb_on_exception",
     )
 
     def __init__(
         self,
         route_handlers: OptionalSequence[ControllerRouterHandler] = None,
         *,
         after_exception: OptionalSequence[AfterExceptionHookHandler] = None,
@@ -172,15 +171,15 @@
         before_request: BeforeRequestHookHandler | None = None,
         before_send: OptionalSequence[BeforeMessageSendHookHandler] = None,
         cache_control: CacheControlHeader | None = None,
         compression_config: CompressionConfig | None = None,
         cors_config: CORSConfig | None = None,
         csrf_config: CSRFConfig | None = None,
         dto: type[DTOInterface] | None | EmptyType = Empty,
-        debug: bool = False,
+        debug: bool | None = None,
         dependencies: Dependencies | None = None,
         etag: ETag | None = None,
         event_emitter_backend: type[BaseEventEmitterBackend] = SimpleEventEmitter,
         exception_handlers: ExceptionHandlersMap | None = None,
         guards: OptionalSequence[Guard] = None,
         listeners: OptionalSequence[EventListener] = None,
         logging_config: BaseLoggingConfig | EmptyType | None = Empty,
@@ -189,15 +188,14 @@
         on_app_init: OptionalSequence[OnAppInitHandler] = None,
         on_shutdown: OptionalSequence[LifespanHook] = None,
         on_startup: OptionalSequence[LifespanHook] = None,
         openapi_config: OpenAPIConfig | None = DEFAULT_OPENAPI_CONFIG,
         opt: Mapping[str, Any] | None = None,
         parameters: ParametersMap | None = None,
         plugins: OptionalSequence[PluginProtocol] = None,
-        preferred_validation_backend: Literal["pydantic", "attrs"] | None = None,
         request_class: type[Request] | None = None,
         response_cache_config: ResponseCacheConfig | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: OptionalSequence[ResponseHeader] = None,
         return_dto: type[DTOInterface] | None | EmptyType = Empty,
         security: OptionalSequence[SecurityRequirement] = None,
@@ -206,14 +204,16 @@
         static_files_config: OptionalSequence[StaticFilesConfig] = None,
         stores: StoreRegistry | dict[str, Store] | None = None,
         tags: Sequence[str] | None = None,
         template_config: TemplateConfig | None = None,
         type_encoders: TypeEncodersMap | None = None,
         websocket_class: type[WebSocket] | None = None,
         lifespan: list[Callable[[Litestar], AbstractAsyncContextManager] | AbstractAsyncContextManager] | None = None,
+        pdb_on_exception: bool | None = None,
+        _preferred_validation_backend: Literal["attrs", "pydantic"] | None = None,
     ) -> None:
         """Initialize a ``Litestar`` application.
 
         Args:
             after_exception: A sequence of :class:`exception hook handlers <.types.AfterExceptionHookHandler>`. This
                 hook is called after an exception occurs. In difference to exception handlers, it is not meant to
                 return a response - only to process the exception (e.g. log it, send it to Sentry etc.).
@@ -262,16 +262,16 @@
                 application startup.
             openapi_config: Defaults to :attr:`DEFAULT_OPENAPI_CONFIG`
             opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
                 wherever you have access to :class:`Request <litestar.connection.request.Request>` or
                 :class:`ASGI Scope <.types.Scope>`.
             parameters: A mapping of :class:`Parameter <.params.Parameter>` definitions available to all application
                 paths.
+            pdb_on_exception: Drop into the PDB when an exception occurs.
             plugins: Sequence of plugins.
-            preferred_validation_backend: Validation backend to use, if multiple are installed.
             request_class: An optional subclass of :class:`Request <.connection.Request>` to use for http connections.
             response_class: A custom subclass of :class:`Response <.response.Response>` to be used as the app's default
                 response.
             response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>`.
             response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
             response_cache_config: Configures caching behavior of the application.
             return_dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for serializing
@@ -295,14 +295,27 @@
             type_encoders: A mapping of types to callables that transform them into types supported for serialization.
             websocket_class: An optional subclass of :class:`WebSocket <.connection.WebSocket>` to use for websocket
                 connections.
         """
         if logging_config is Empty:
             logging_config = LoggingConfig()
 
+        if debug is None:
+            debug = os.getenv("LITESTAR_DEBUG", "0") == "1"
+
+        if pdb_on_exception is None:
+            pdb_on_exception = os.getenv("LITESTAR_PDB", "0") == "1"
+
+        if _preferred_validation_backend is not None:
+            warn_deprecation(
+                version="2.0.0beta1",
+                kind="parameter",
+                deprecated_name="_preferred_validation_backend",
+            )
+
         config = AppConfig(
             after_exception=list(after_exception or []),
             after_request=after_request,
             after_response=after_response,
             allowed_hosts=allowed_hosts if isinstance(allowed_hosts, AllowedHostsConfig) else list(allowed_hosts or []),
             before_request=before_request,
             before_send=list(before_send or []),
@@ -323,16 +336,16 @@
             middleware=list(middleware or []),
             multipart_form_part_limit=multipart_form_part_limit,
             on_shutdown=list(on_shutdown or []),
             on_startup=list(on_startup or []),
             openapi_config=openapi_config,
             opt=dict(opt or {}),
             parameters=parameters or {},
+            pdb_on_exception=pdb_on_exception,
             plugins=list(plugins or []),
-            preferred_validation_backend=preferred_validation_backend or "pydantic",
             request_class=request_class,
             response_cache_config=response_cache_config or ResponseCacheConfig(),
             response_class=response_class,
             response_cookies=response_cookies or [],
             response_headers=response_headers or [],
             return_dto=return_dto,
             route_handlers=list(route_handlers) if route_handlers is not None else [],
@@ -358,36 +371,40 @@
 
         self.get_logger: GetLogger = get_logger_placeholder
         self.logger: Logger | None = None
         self.routes: list[HTTPRoute | ASGIRoute | WebSocketRoute] = []
         self.asgi_router = ASGIRouter(app=self)
 
         self.allowed_hosts = cast("AllowedHostsConfig | None", config.allowed_hosts)
-        self.after_exception = as_async_callable_list(config.after_exception)
+        self.after_exception = [AsyncCallable(h) for h in config.after_exception]
         self.allowed_hosts = cast("AllowedHostsConfig | None", config.allowed_hosts)
-        self.before_send = as_async_callable_list(config.before_send)
+        self.before_send = [AsyncCallable(h) for h in config.before_send]
         self.compression_config = config.compression_config
         self.cors_config = config.cors_config
         self.csrf_config = config.csrf_config
         self.event_emitter = config.event_emitter_backend(listeners=config.listeners)
         self.logging_config = config.logging_config
         self.multipart_form_part_limit = config.multipart_form_part_limit
         self.on_shutdown = config.on_shutdown
         self.on_startup = config.on_startup
         self.openapi_config = config.openapi_config
         self.openapi_schema_plugins = [p for p in config.plugins if isinstance(p, OpenAPISchemaPluginProtocol)]
-        self.preferred_validation_backend: Literal["pydantic", "attrs"] = config.preferred_validation_backend
+        self._preferred_validation_backend: Literal["attrs", "pydantic"] = _preferred_validation_backend or "pydantic"
         self.request_class = config.request_class or Request
         self.response_cache_config = config.response_cache_config
         self.serialization_plugins = [p for p in config.plugins if isinstance(p, SerializationPluginProtocol)]
         self.state = config.state
         self.static_files_config = config.static_files_config
         self.template_engine = config.template_config.engine_instance if config.template_config else None
         self.websocket_class = config.websocket_class or WebSocket
         self.debug = config.debug
+        self.pdb_on_exception: bool = config.pdb_on_exception
+
+        if self.pdb_on_exception:
+            warn_pdb_on_exception()
 
         super().__init__(
             after_request=config.after_request,
             after_response=config.after_response,
             before_request=config.before_request,
             cache_control=config.cache_control,
             dependencies=config.dependencies,
@@ -737,15 +754,15 @@
         Returns:
             An ASGI send function.
         """
         if self.before_send:
 
             async def wrapped_send(message: Message) -> None:
                 for hook in self.before_send:
-                    await hook(message, self.state, scope)
+                    await hook(message, scope)
                 await send(message)
 
             return wrapped_send
         return send
 
     def update_openapi_schema(self) -> None:
         """Update the OpenAPI schema to reflect the route handlers registered on the app.
```

### Comparing `litestar-2.0.0a7/litestar/background_tasks.py` & `litestar-2.0.0b1/litestar/background_tasks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/channels/backends/base.py` & `litestar-2.0.0b1/litestar/channels/backends/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/channels/backends/memory.py` & `litestar-2.0.0b1/litestar/channels/backends/memory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/channels/backends/redis.py` & `litestar-2.0.0b1/litestar/channels/backends/redis.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,17 +54,23 @@
             key_prefix: Key prefix to use for storing data in redis
             stream_sleep_no_subscriptions: Amount of time in milliseconds to pause the
                 :meth:`stream_events` generator, should no subscribers exist
         """
         super().__init__(
             redis=redis, stream_sleep_no_subscriptions=stream_sleep_no_subscriptions, key_prefix=key_prefix
         )
-        self._pub_sub: PubSub = self._redis.pubsub()
+        self.__pub_sub: PubSub | None = None
         self._publish_script = self._redis.register_script(_PUBSUB_PUBLISH_SCRIPT)
 
+    @property
+    def _pub_sub(self) -> PubSub:
+        if self.__pub_sub is None:
+            self.__pub_sub = self._redis.pubsub()
+        return self.__pub_sub
+
     async def on_startup(self) -> None:
         pass
 
     async def on_shutdown(self) -> None:
         await self._pub_sub.reset()
 
     async def subscribe(self, channels: Iterable[str]) -> None:
```

### Comparing `litestar-2.0.0a7/litestar/channels/plugin.py` & `litestar-2.0.0b1/litestar/channels/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 
         return self._encode_json(data)
 
     def on_app_init(self, app_config: AppConfig) -> AppConfig:
         """Plugin hook. Set up a ``channels`` dependency, add route handlers and register application hooks"""
         app_config.dependencies["channels"] = Provide(lambda: self, use_cache=True, sync_to_thread=False)
         app_config.lifespan.append(self)
+        app_config.signature_namespace.update(ChannelsPlugin=ChannelsPlugin)
 
         if self._create_route_handlers:
             if self._arbitrary_channels_allowed:
                 path = join_path(self._handler_root_path, "{channel_name:str}")  # noqa: PTH118
                 route_handlers = [WebsocketRouteHandler(path)(self._ws_handler_func)]
             else:
                 route_handlers = [
```

### Comparing `litestar-2.0.0a7/litestar/channels/subscriber.py` & `litestar-2.0.0b1/litestar/channels/subscriber.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/cli/_utils.py` & `litestar-2.0.0b1/litestar/cli/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,40 @@
 from dataclasses import dataclass
 from functools import wraps
 from itertools import chain
 from os import getenv
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable, Generator, Iterable, Sequence, TypeVar, cast
 
-from click import ClickException, Command, Context, Group, pass_context, style
-from rich.console import Console
+from rich import get_console
 from rich.table import Table
 from typing_extensions import Concatenate, ParamSpec
 
 from litestar import Litestar, __version__
 from litestar.middleware import DefineMiddleware
 from litestar.utils import get_name
 
+RICH_CLICK_INSTALLED = False
+try:
+    import rich_click  # noqa: F401
+
+    RICH_CLICK_INSTALLED = True
+except ImportError:
+    pass
+
+if TYPE_CHECKING or not RICH_CLICK_INSTALLED:
+    from click import ClickException, Command, Context, Group, pass_context
+else:
+    from rich_click import ClickException, Context, pass_context
+    from rich_click.rich_command import RichCommand as Command  # noqa: TCH002
+    from rich_click.rich_group import RichGroup as Group
+
+
 __all__ = (
+    "RICH_CLICK_INSTALLED",
     "LoadedApp",
     "LitestarCLIException",
     "LitestarEnv",
     "LitestarExtensionGroup",
     "LitestarGroup",
     "show_app_info",
 )
@@ -41,36 +57,39 @@
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
 AUTODISCOVERY_FILE_NAMES = ["app", "application"]
 
-console = Console()
+console = get_console()
 
 
 class LitestarCLIException(ClickException):
     """Base class for Litestar CLI exceptions."""
 
     def __init__(self, message: str) -> None:
         """Initialize exception and style error message."""
-        super().__init__(style(message, fg="red"))
+        super().__init__(message)
 
 
 @dataclass
 class LitestarEnv:
     """Information about the current Litestar environment variables."""
 
     app_path: str
     debug: bool
     app: Litestar
     cwd: Path
     host: str | None = None
     port: int | None = None
+    fd: int | None = None
+    uds: str | None = None
     reload: bool | None = None
+    reload_dirs: tuple[str, ...] | None = None
     web_concurrency: int | None = None
     is_app_factory: bool = False
 
     @classmethod
     def from_env(cls, app_path: str | None) -> LitestarEnv:
         """Load environment variables.
 
@@ -93,22 +112,28 @@
             console.print(f"Using Litestar app from env: [bright_blue]{app_path!r}")
             loaded_app = _load_app_from_path(app_path)
         else:
             loaded_app = _autodiscover_app(cwd)
 
         port = getenv("LITESTAR_PORT")
         web_concurrency = getenv("WEB_CONCURRENCY")
+        uds = getenv("LITESTAR_UNIX_DOMAIN_SOCKET")
+        fd = getenv("LITESTAR_FILE_DESCRIPTOR")
+        reload_dirs = tuple(s.strip() for s in getenv("LITESTAR_RELOAD_DIRS", "").split(",") if s) or None
 
         return cls(
             app_path=loaded_app.app_path,
             app=loaded_app.app,
             debug=_bool_from_env("LITESTAR_DEBUG"),
             host=getenv("LITESTAR_HOST"),
             port=int(port) if port else None,
+            uds=uds,
+            fd=int(fd) if fd else None,
             reload=_bool_from_env("LITESTAR_RELOAD"),
+            reload_dirs=reload_dirs,
             web_concurrency=int(web_concurrency) if web_concurrency else None,
             is_app_factory=loaded_app.is_factory,
             cwd=cwd,
         )
 
 
 @dataclass
@@ -195,14 +220,18 @@
             if not isinstance(ctx.obj, LitestarEnv):
                 ctx.obj = ctx.obj()
             env = ctx.ensure_object(LitestarEnv)
             if needs_app:
                 kwargs["app"] = env.app
             if needs_env:
                 kwargs["env"] = env
+
+        if "ctx" in params:
+            kwargs["ctx"] = ctx
+
         return func(*args, **kwargs)
 
     return pass_context(wrapped)
 
 
 def _wrap_commands(commands: Iterable[Command]) -> None:
     for command in commands:
@@ -301,14 +330,15 @@
 
     table = Table(show_header=False)
     table.add_column("title", style="cyan")
     table.add_column("value", style="bright_blue")
 
     table.add_row("Litestar version", f"{__version__.major}.{__version__.minor}.{__version__.patch}")
     table.add_row("Debug mode", _format_is_enabled(app.debug))
+    table.add_row("Python Debugger on exception", _format_is_enabled(app.pdb_on_exception))
     table.add_row("CORS", _format_is_enabled(app.cors_config))
     table.add_row("CSRF", _format_is_enabled(app.csrf_config))
     if app.allowed_hosts:
         allowed_hosts = app.allowed_hosts
 
         table.add_row("Allowed hosts", ", ".join(allowed_hosts.allowed_hosts))
```

### Comparing `litestar-2.0.0a7/litestar/cli/commands/schema.py` & `litestar-2.0.0b1/litestar/cli/commands/schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 from json import dumps
 from pathlib import Path
+from typing import TYPE_CHECKING
 
-from click import Path as ClickPath
-from click import group, option
 from jsbeautifier import Beautifier
 from yaml import dump as dump_yaml
 
 from litestar import Litestar
 from litestar._openapi.typescript_converter.converter import (
     convert_openapi_to_typescript,
 )
-from litestar.cli._utils import LitestarCLIException, LitestarGroup
+from litestar.cli._utils import RICH_CLICK_INSTALLED, LitestarCLIException, LitestarGroup
+
+if TYPE_CHECKING or not RICH_CLICK_INSTALLED:
+    from click import Path as ClickPath
+    from click import group, option
+else:
+    from rich_click import Path as ClickPath
+    from rich_click import group, option
+
 
 __all__ = ("generate_openapi_schema", "generate_typescript_specs", "schema_group")
 
 
 beautifier = Beautifier()
```

### Comparing `litestar-2.0.0a7/litestar/cli/commands/sessions.py` & `litestar-2.0.0b1/litestar/cli/commands/sessions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,24 @@
-from click import argument, group
+from typing import TYPE_CHECKING
+
 from rich.prompt import Confirm
 
 from litestar import Litestar
-from litestar.cli._utils import LitestarCLIException, LitestarGroup, console
+from litestar.cli._utils import RICH_CLICK_INSTALLED, LitestarCLIException, LitestarGroup, console
 from litestar.middleware import DefineMiddleware
 from litestar.middleware.session import SessionMiddleware
 from litestar.middleware.session.server_side import ServerSideSessionBackend
 from litestar.utils import is_class_and_subclass
 
+if TYPE_CHECKING or not RICH_CLICK_INSTALLED:
+    from click import argument, group
+else:
+    from rich_click import argument, group
+
+
 __all__ = ("clear_sessions_command", "delete_session_command", "get_session_backend", "sessions_group")
 
 
 def get_session_backend(app: Litestar) -> ServerSideSessionBackend:
     """Get the session backend used by a ``Litestar`` app."""
     for middleware in app.middleware:
         if isinstance(middleware, DefineMiddleware):
```

### Comparing `litestar-2.0.0a7/litestar/config/allowed_hosts.py` & `litestar-2.0.0b1/litestar/config/allowed_hosts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/config/app.py` & `litestar-2.0.0b1/litestar/config/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any, Callable, Literal, Sequence
+from typing import TYPE_CHECKING, Any, Callable, Sequence
 
 from litestar.config.allowed_hosts import AllowedHostsConfig
 from litestar.config.response_cache import ResponseCacheConfig
 from litestar.datastructures import State
 from litestar.events.emitter import SimpleEventEmitter
 from litestar.types.empty import Empty
 
@@ -140,18 +140,18 @@
     """A string keyed dictionary of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
     wherever you have access to :class:`Request <.connection.Request>` or :class:`ASGI Scope <litestar.types.Scope>`.
 
     Can be overridden by routers and router handlers.
     """
     parameters: ParametersMap = field(default_factory=dict)
     """A mapping of :class:`Parameter <.params.Parameter>` definitions available to all application paths."""
+    pdb_on_exception: bool = field(default=False)
+    """Drop into the PDB on an exception"""
     plugins: list[PluginProtocol] = field(default_factory=list)
     """List of :class:`SerializationPluginProtocol <.plugins.SerializationPluginProtocol>`."""
-    preferred_validation_backend: Literal["pydantic", "attrs"] = field(default="attrs")
-    """Validation backend to use, if multiple are installed."""
     request_class: type[Request] | None = field(default=None)
     """An optional subclass of :class:`Request <.connection.Request>` to use for http connections."""
     response_class: ResponseType | None = field(default=None)
     """A custom subclass of :class:`Response <.response.Response>` to be used as the app's default response."""
     response_cookies: ResponseCookies = field(default_factory=list)  # type: ignore
     """A list of :class:`Cookie <.datastructures.Cookie>`."""
     response_headers: Sequence[ResponseHeader] = field(default_factory=list)
```

### Comparing `litestar-2.0.0a7/litestar/config/compression.py` & `litestar-2.0.0b1/litestar/config/compression.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/config/cors.py` & `litestar-2.0.0b1/litestar/config/cors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/config/csrf.py` & `litestar-2.0.0b1/litestar/config/csrf.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/config/response_cache.py` & `litestar-2.0.0b1/litestar/config/response_cache.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/connection/__init__.py` & `litestar-2.0.0b1/litestar/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/connection/base.py` & `litestar-2.0.0b1/litestar/connection/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/connection/request.py` & `litestar-2.0.0b1/litestar/connection/request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/connection/websocket.py` & `litestar-2.0.0b1/litestar/connection/websocket.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
     def iter_data(self, mode: Literal["text"]) -> AsyncGenerator[str, None]:
         ...
 
     @overload
     def iter_data(self, mode: Literal["binary"]) -> AsyncGenerator[bytes, None]:
         ...
 
-    async def iter_data(self, mode: WebSocketMode) -> AsyncGenerator[str | bytes, None]:
+    async def iter_data(self, mode: WebSocketMode = "text") -> AsyncGenerator[str | bytes, None]:
         """Continuously receive data and yield it
 
         Args:
             mode: Socket mode to use. Either ``text`` or ``binary``
         """
         try:
             while True:
@@ -227,15 +227,15 @@
 
         Returns:
             An arbitrary value
         """
         data = await self.receive_data(mode="binary")
         return decode_msgpack(data)
 
-    async def iter_json(self, mode: WebSocketMode) -> AsyncGenerator[Any, None]:
+    async def iter_json(self, mode: WebSocketMode = "text") -> AsyncGenerator[Any, None]:
         """Continuously receive data and yield it, decoding it as JSON in the process.
 
         Args:
             mode: Socket mode to use. Either ``text`` or ``binary``
         """
         async for data in self.iter_data(mode):
             yield decode_json(data)
```

### Comparing `litestar-2.0.0a7/litestar/contrib/htmx/_utils.py` & `litestar-2.0.0b1/litestar/contrib/htmx/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/contrib/htmx/request.py` & `litestar-2.0.0b1/litestar/contrib/htmx/request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/contrib/htmx/response.py` & `litestar-2.0.0b1/litestar/contrib/htmx/response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from __future__ import annotations
 
-from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any, Generic, TypeVar
+from typing import Any, Generic, TypeVar
 from urllib.parse import quote
 
-from litestar import Litestar, MediaType, Request, Response
+from litestar import Response
 from litestar.contrib.htmx._utils import HTMX_STOP_POLLING, get_headers
 from litestar.contrib.htmx.types import (
     EventAfterType,
     HtmxHeaderType,
     LocationType,
     PushUrlType,
     ReSwapMethod,
     TriggerEventType,
 )
-from litestar.response import TemplateResponse
-from litestar.response_containers import ResponseContainer, Template
+from litestar.response import Template
 from litestar.status_codes import HTTP_200_OK
 
 __all__ = (
     "ClientRedirect",
     "ClientRefresh",
     "HTMXTemplate",
     "HXLocation",
@@ -27,18 +25,14 @@
     "PushUrl",
     "ReplaceUrl",
     "Reswap",
     "Retarget",
     "TriggerEvent",
 )
 
-if TYPE_CHECKING:
-    from litestar.background_tasks import BackgroundTask, BackgroundTasks
-    from litestar.datastructures import Cookie
-
 
 # HTMX defined HTTP status code.
 # Response carrying this status code will ask client to stop Polling.
 T = TypeVar("T")
 
 
 class HXStopPolling(Response):
@@ -166,72 +160,41 @@
                 )
             )
         )
         del self.headers["Location"]
         self.headers.update(spec)
 
 
-@dataclass
-class HTMXTemplate(ResponseContainer[TemplateResponse]):
+class HTMXTemplate(Template):
     """HTMX template wrapper"""
 
-    name: str
-    """Path-like name for the template to be rendered, e.g. "index.html"."""
-    context: dict[str, Any] = field(default_factory=dict)
-    """A dictionary of key/value pairs to be passed to the temple engine's render method.
-
-    Defaults to None.
-    """
-    background: BackgroundTask | BackgroundTasks | None = field(default=None)
-    """A :class:`BackgroundTask <.background_tasks.BackgroundTask>` instance or
-    :class:`BackgroundTasks <.background_tasks.BackgroundTasks>` to execute after the response is finished. Defaults to
-    ``None``.
-    """
-    headers: dict[str, Any] = field(default_factory=dict)
-    """A string/string dictionary of response headers.Header keys are insensitive. Defaults to ``None``."""
-    cookies: list[Cookie] = field(default_factory=list)
-    """A list of :class:`Cookies <.datastructures.Cookie>` to be set under the response ``Set-Cookie`` header. Defaults
-    to ``None``.
-    """
-    media_type: MediaType | str | None = field(default=None)
-    """If defined, overrides the media type configured in the route decorator."""
-    encoding: str = field(default="utf-8")
-    """The encoding to be used for the response headers."""
-    push_url: PushUrlType | None = field(default=None)
-    """Either a string value specifying a URL to push to browser history or ``False`` to prevent HTMX client from
-    pushing a url to browser history."""
-    re_swap: ReSwapMethod | None = field(default=None)
-    """Method value to instruct HTMX which swapping method to use."""
-    re_target: str | None = field(default=None)
-    """Value for 'id of target element' to apply changes to."""
-    trigger_event: str | None = field(default=None)
-    """Event name to trigger."""
-    params: dict[str, Any] | None = field(default=None)
-    """Dictionary of parameters if any required with trigger event parameter."""
-    after: EventAfterType | None = field(default=None)
-    """Changes to apply after ``receive``, ``settle`` or ``swap`` event."""
-
-    def to_response(
+    def __init__(
         self,
-        headers: dict[str, Any],
-        media_type: MediaType | str,
-        status_code: int,
-        app: Litestar,
-        request: Request,
-    ) -> TemplateResponse:
-        """Add HTMX headers and return a :class:`TemplateResponse <.response.TemplateResponse>`."""
-
-        event: TriggerEventType | None = None
-        if self.trigger_event:
-            event = TriggerEventType(name=str(self.trigger_event), params=self.params, after=self.after)
+        push_url: PushUrlType | None = None,
+        re_swap: ReSwapMethod | None = None,
+        re_target: str | None = None,
+        trigger_event: str | None = None,
+        params: dict[str, Any] | None = None,
+        after: EventAfterType | None = None,
+        **kwargs: Any,
+    ) -> None:
+        """Create HTMXTemplate response.
 
-        hx_headers: dict[str, Any] = get_headers(
-            hx_headers=HtmxHeaderType(
-                push_url=self.push_url, re_swap=self.re_swap, re_target=self.re_target, trigger_event=event
-            )
-        )
+        Args:
+            push_url: Either a string value specifying a URL to push to browser history or ``False`` to prevent HTMX client from
+                pushing a url to browser history.
+            re_swap: Method value to instruct HTMX which swapping method to use.
+            re_target: Value for 'id of target element' to apply changes to.
+            trigger_event: Event name to trigger.
+            params: Dictionary of parameters if any required with trigger event parameter.
+            after: Changes to apply after ``receive``, ``settle`` or ``swap`` event.
+            **kwargs: Additional arguments to pass to ``Template``.
+        """
+        super().__init__(**kwargs)
 
-        template = Template(name=self.name, background=self.background, context=self.context, encoding=self.encoding)
+        event: TriggerEventType | None = None
+        if trigger_event:
+            event = TriggerEventType(name=str(trigger_event), params=params, after=after)
 
-        return template.to_response(
-            headers=hx_headers, media_type=media_type, app=app, status_code=status_code, request=request
+        self.headers.update(
+            get_headers(HtmxHeaderType(push_url=push_url, re_swap=re_swap, re_target=re_target, trigger_event=event))
         )
```

### Comparing `litestar-2.0.0a7/litestar/contrib/htmx/types.py` & `litestar-2.0.0b1/litestar/contrib/htmx/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/contrib/jinja.py` & `litestar-2.0.0b1/litestar/contrib/jinja.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/contrib/jwt/__init__.py` & `litestar-2.0.0b1/litestar/contrib/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/contrib/jwt/jwt_auth.py` & `litestar-2.0.0b1/litestar/contrib/jwt/jwt_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/contrib/jwt/jwt_token.py` & `litestar-2.0.0b1/litestar/contrib/jwt/jwt_token.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from __future__ import annotations
 
+import dataclasses
 from dataclasses import asdict, dataclass, field
 from datetime import datetime, timezone
-from typing import cast
+from typing import TYPE_CHECKING, Any, cast
 
 from jose import JWSError, JWTError, jwt
 
 from litestar.exceptions import ImproperlyConfiguredException, NotAuthorizedException
 
+if TYPE_CHECKING:
+    from typing_extensions import Self
+
+
 __all__ = ("Token",)
 
 
 def _normalize_datetime(value: datetime) -> datetime:
     """Convert the given value into UTC and strip microseconds.
 
     Args:
@@ -38,14 +43,16 @@
     """Issued at - should always be current now."""
     iss: str | None = field(default=None)
     """Issuer - optional unique identifier for the issuer."""
     aud: str | None = field(default=None)
     """Audience - intended audience."""
     jti: str | None = field(default=None)
     """JWT ID - a unique identifier of the JWT between different issuers."""
+    extras: dict[str, Any] = field(default_factory=dict)
+    """Extra fields that were found on the JWT token."""
 
     def __post_init__(self) -> None:
         if len(self.sub) < 1:
             raise ImproperlyConfiguredException("sub must be a string with a length greater than 0")
 
         if isinstance(self.exp, datetime) and (
             (exp := _normalize_datetime(self.exp))
@@ -59,16 +66,16 @@
             (iat := _normalize_datetime(self.iat))
             and iat.timestamp() <= _normalize_datetime(datetime.now(timezone.utc)).timestamp()
         ):
             self.iat = iat
         else:
             raise ImproperlyConfiguredException("iat must be a current or past time")
 
-    @staticmethod
-    def decode(encoded_token: str, secret: str | dict[str, str], algorithm: str) -> Token:
+    @classmethod
+    def decode(cls, encoded_token: str, secret: str | dict[str, str], algorithm: str) -> Self:
         """Decode a passed in token string and returns a Token instance.
 
         Args:
             encoded_token: A base64 string containing an encoded JWT.
             secret: The secret with which the JWT is encoded. It may optionally be an individual JWK or JWS set dict
             algorithm: The algorithm used to encode the JWT.
 
@@ -78,15 +85,20 @@
         Raises:
             NotAuthorizedException: If the token is invalid.
         """
         try:
             payload = jwt.decode(token=encoded_token, key=secret, algorithms=[algorithm], options={"verify_aud": False})
             exp = datetime.fromtimestamp(payload.pop("exp"), tz=timezone.utc)
             iat = datetime.fromtimestamp(payload.pop("iat"), tz=timezone.utc)
-            return Token(exp=exp, iat=iat, **payload)
+            field_names = {f.name for f in dataclasses.fields(Token)}
+            extra_fields = payload.keys() - field_names
+            extras = payload.pop("extras", {})
+            for key in extra_fields:
+                extras[key] = payload.pop(key)
+            return cls(exp=exp, iat=iat, **payload, extras=extras)
         except (KeyError, JWTError, ImproperlyConfiguredException) as e:
             raise NotAuthorizedException("Invalid token") from e
 
     def encode(self, secret: str, algorithm: str) -> str:
         """Encode the token instance into a string.
 
         Args:
```

### Comparing `litestar-2.0.0a7/litestar/contrib/jwt/middleware.py` & `litestar-2.0.0b1/litestar/contrib/jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/contrib/mako.py` & `litestar-2.0.0b1/litestar/contrib/mako.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,17 @@
     def __init__(self, directory: DirectoryPath | list[DirectoryPath]) -> None:
         """Initialize template engine.
 
         Args:
             directory: Direct path or list of directory paths from which to serve templates.
         """
         super().__init__(directory=directory)
-        self.engine = TemplateLookup(directories=directory if isinstance(directory, (list, tuple)) else [directory])
+        self.engine = TemplateLookup(
+            directories=directory if isinstance(directory, (list, tuple)) else [directory], default_filters=["h"]
+        )
         self._template_callables: list[tuple[str, Callable[[dict[str, Any]], Any]]] = []
         self.register_template_callable(key="url_for_static_asset", template_callable=url_for_static_asset)  # type: ignore
         self.register_template_callable(key="csrf_token", template_callable=csrf_token)  # type: ignore
         self.register_template_callable(key="url_for", template_callable=url_for)  # type: ignore
 
     def get_template(self, template_name: str) -> MakoTemplate:
         """Retrieve a template by matching its name (dotted path) with files in the directory or directories provided.
```

### Comparing `litestar-2.0.0a7/litestar/contrib/opentelemetry/_utils.py` & `litestar-2.0.0b1/litestar/contrib/opentelemetry/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/contrib/opentelemetry/config.py` & `litestar-2.0.0b1/litestar/contrib/opentelemetry/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/contrib/opentelemetry/middleware.py` & `litestar-2.0.0b1/litestar/contrib/opentelemetry/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/contrib/repository/abc.py` & `litestar-2.0.0b1/litestar/contrib/repository/abc/_async.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,20 @@
-"""Data persistence interface."""
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
 from typing import TYPE_CHECKING, Any, Generic, TypeVar
 
-from .exceptions import NotFoundError
+from litestar.contrib.repository.exceptions import NotFoundError
 
 if TYPE_CHECKING:
-    from typing_extensions import TypeAlias
-
-    from .filters import BeforeAfter, CollectionFilter, LimitOffset, OrderBy, SearchFilter
-
-__all__ = ("AbstractAsyncRepository", "FilterTypes")
+    from litestar.contrib.repository.filters import FilterTypes
 
 T = TypeVar("T")
-RepoT = TypeVar("RepoT", bound="AbstractAsyncRepository")
 CollectionT = TypeVar("CollectionT")
 
-FilterTypes: TypeAlias = "BeforeAfter | CollectionFilter[Any] | LimitOffset | OrderBy | SearchFilter"
-"""Aggregate type alias of the types supported for collection filtering."""
-
 
 class AbstractAsyncRepository(Generic[T], metaclass=ABCMeta):
     """Interface for persistent data interaction."""
 
     model_type: type[T]
     """Type of object represented by the repository."""
     id_attribute = "id"
```

### Comparing `litestar-2.0.0a7/litestar/contrib/repository/filters.py` & `litestar-2.0.0b1/litestar/contrib/repository/filters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,32 @@
 """Collection filter datastructures."""
 from __future__ import annotations
 
 from collections import abc  # noqa: TCH003
 from dataclasses import dataclass
 from datetime import datetime  # noqa: TCH003
-from typing import Generic, Literal, TypeVar
+from typing import TYPE_CHECKING, Any, Generic, Literal, TypeVar
+
+if TYPE_CHECKING:
+    from typing_extensions import TypeAlias
 
 T = TypeVar("T")
 
-__all__ = ["BeforeAfter", "CollectionFilter", "LimitOffset", "OrderBy", "SearchFilter"]
+__all__ = (
+    "BeforeAfter",
+    "CollectionFilter",
+    "FilterTypes",
+    "LimitOffset",
+    "OrderBy",
+    "SearchFilter",
+)
+
+
+FilterTypes: TypeAlias = "BeforeAfter | CollectionFilter[Any] | LimitOffset | OrderBy | SearchFilter"
+"""Aggregate type alias of the types supported for collection filtering."""
 
 
 @dataclass
 class BeforeAfter:
     """Data required to filter a query on a ``datetime`` column."""
 
     field_name: str
```

### Comparing `litestar-2.0.0a7/litestar/contrib/repository/handlers.py` & `litestar-2.0.0b1/litestar/contrib/repository/handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/contrib/repository/testing/generic_mock_repository.py` & `litestar-2.0.0b1/litestar/contrib/repository/testing/generic_mock_repository.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 """
 from __future__ import annotations
 
 from datetime import datetime, timezone, tzinfo
 from typing import TYPE_CHECKING, Generic, Protocol, TypeVar
 from uuid import uuid4
 
-from litestar.contrib.repository.abc import AbstractAsyncRepository
+from litestar.contrib.repository import AbstractAsyncRepository, AbstractSyncRepository, FilterTypes
 from litestar.contrib.repository.exceptions import ConflictError, RepositoryError
 
 if TYPE_CHECKING:
     from collections.abc import Callable, Hashable, Iterable, MutableMapping
     from typing import Any
 
-    from litestar.contrib.repository import FilterTypes
 
 ModelT = TypeVar("ModelT", bound="HasID")
-MockRepoT = TypeVar("MockRepoT", bound="GenericAsyncMockRepository")
+AsyncMockRepoT = TypeVar("AsyncMockRepoT", bound="GenericAsyncMockRepository")
+SyncMockRepoT = TypeVar("SyncMockRepoT", bound="GenericSyncMockRepository")
 
 
 class HasID(Protocol):
     id: Any
 
 
 class GenericAsyncMockRepository(AbstractAsyncRepository[ModelT], Generic[ModelT]):
@@ -31,55 +31,55 @@
     Uses a :class:`dict` for storage.
     """
 
     collection: MutableMapping[Hashable, ModelT]
     model_type: type[ModelT]
     match_fields: list[str] | str | None = None
 
-    _model_has_created: bool
-    _model_has_updated: bool
+    _model_has_created_at: bool
+    _model_has_updated_at: bool
 
     def __init__(
         self, id_factory: Callable[[], Any] = uuid4, tz: tzinfo = timezone.utc, allow_ids_on_add: bool = False, **_: Any
     ) -> None:
         super().__init__()
         self._id_factory = id_factory
         self.tz = tz
         self.allow_ids_on_add = allow_ids_on_add
 
     @classmethod
-    def __class_getitem__(cls: type[MockRepoT], item: type[ModelT]) -> type[MockRepoT]:
+    def __class_getitem__(cls: type[AsyncMockRepoT], item: type[ModelT]) -> type[AsyncMockRepoT]:
         """Add collection to ``_collections`` for the type.
 
         Args:
             item: The type that the class has been parametrized with.
         """
         return type(  # pyright:ignore
             f"{cls.__name__}[{item.__name__}]",
             (cls,),
             {
                 "collection": {},
                 "model_type": item,
-                "_model_has_created": hasattr(item, "created"),
-                "_model_has_updated": hasattr(item, "updated"),
+                "_model_has_created_at": hasattr(item, "created_at"),
+                "_model_has_updated_at": hasattr(item, "updated_at"),
             },
         )
 
     def _find_or_raise_not_found(self, item_id: Any) -> ModelT:
         return self.check_not_found(self.collection.get(item_id))
 
     def _now(self) -> datetime:
         return datetime.now(tz=self.tz).replace(tzinfo=None)
 
     def _update_audit_attributes(self, data: ModelT, now: datetime | None = None, do_created: bool = False) -> ModelT:
         now = now or self._now()
-        if self._model_has_updated:
-            data.updated = now  # type:ignore[attr-defined]
-        if self._model_has_updated and do_created:
-            data.created = now  # type:ignore[attr-defined]
+        if self._model_has_updated_at:
+            data.updated_at = now  # type:ignore[attr-defined]
+        if self._model_has_updated_at and do_created:
+            data.created_at = now  # type:ignore[attr-defined]
         return data
 
     async def add(self, data: ModelT) -> ModelT:
         """Add ``data`` to the collection.
 
         Args:
             data: Instance to be added to the collection.
@@ -262,17 +262,15 @@
             The updated instance.
 
         Raises:
             NotFoundError: If no instance found with same identifier as ``data``.
         """
         item = self._find_or_raise_not_found(self.get_id_attribute_value(data))
         self._update_audit_attributes(data, do_created=False)
-        for key, val in data.__dict__.items():
-            if key.startswith("_"):
-                continue
+        for key, val in model_items(data):
             setattr(item, key, val)
         return item
 
     async def update_many(self, data: list[ModelT]) -> list[ModelT]:
         """Update instances with the attribute values present on ``data``.
 
         Args:
@@ -285,17 +283,15 @@
         Raises:
             NotFoundError: If no instance found with same identifier as ``data``.
         """
         items = [self._find_or_raise_not_found(self.get_id_attribute_value(row)) for row in data]
         now = self._now()
         for item in items:
             self._update_audit_attributes(item, do_created=False, now=now)
-            for key, val in item.__dict__.items():
-                if key.startswith("_"):
-                    continue
+            for key, val in model_items(item):
                 setattr(item, key, val)
         return items
 
     async def upsert(self, data: ModelT) -> ModelT:
         """Update or create instance.
 
         Updates instance with the attribute values present on ``data``, or creates a new instance if
@@ -374,7 +370,366 @@
         for instance in instances:
             cls.collection[cls.get_id_attribute_value(instance)] = instance
 
     @classmethod
     def clear_collection(cls) -> None:
         """Empty the collection for repository type."""
         cls.collection = {}
+
+
+class GenericSyncMockRepository(AbstractSyncRepository[ModelT], Generic[ModelT]):
+    """A repository implementation for tests.
+
+    Uses a :class:`dict` for storage.
+    """
+
+    collection: MutableMapping[Hashable, ModelT]
+    model_type: type[ModelT]
+    match_fields: list[str] | str | None = None
+
+    _model_has_created_at: bool
+    _model_has_updated_at: bool
+
+    def __init__(
+        self,
+        id_factory: Callable[[], Any] = uuid4,
+        tz: tzinfo = timezone.utc,
+        allow_ids_on_add: bool = False,
+        **_: Any,
+    ) -> None:
+        super().__init__()
+        self._id_factory = id_factory
+        self.tz = tz
+        self.allow_ids_on_add = allow_ids_on_add
+
+    @classmethod
+    def __class_getitem__(cls: type[SyncMockRepoT], item: type[ModelT]) -> type[SyncMockRepoT]:
+        """Add collection to ``_collections`` for the type.
+
+        Args:
+            item: The type that the class has been parametrized with.
+        """
+        return type(  # pyright:ignore
+            f"{cls.__name__}[{item.__name__}]",
+            (cls,),
+            {
+                "collection": {},
+                "model_type": item,
+                "_model_has_created_at": hasattr(item, "created_at"),
+                "_model_has_updated_at": hasattr(item, "updated_at"),
+            },
+        )
+
+    def _find_or_raise_not_found(self, item_id: Any) -> ModelT:
+        return self.check_not_found(self.collection.get(item_id))
+
+    def _now(self) -> datetime:
+        return datetime.now(tz=self.tz).replace(tzinfo=None)
+
+    def _update_audit_attributes(self, data: ModelT, now: datetime | None = None, do_created: bool = False) -> ModelT:
+        now = now or self._now()
+        if self._model_has_updated_at:
+            data.updated_at = now  # type:ignore[attr-defined]
+        if self._model_has_updated_at and do_created:
+            data.created_at = now  # type:ignore[attr-defined]
+        return data
+
+    def add(self, data: ModelT) -> ModelT:
+        """Add ``data`` to the collection.
+
+        Args:
+            data: Instance to be added to the collection.
+
+        Returns:
+            The added instance.
+        """
+        if self.allow_ids_on_add is False and self.get_id_attribute_value(data) is not None:
+            raise ConflictError("`add()` received identified item.")
+        self._update_audit_attributes(data, do_created=True)
+        if self.allow_ids_on_add is False:
+            id_ = self._id_factory()
+            self.set_id_attribute_value(id_, data)
+        self.collection[data.id] = data
+        return data
+
+    def add_many(self, data: Iterable[ModelT]) -> list[ModelT]:
+        """Add multiple ``data`` to the collection.
+
+        Args:
+            data: Instance to be added to the collection.
+
+        Returns:
+            The added instance.
+        """
+        now = self._now()
+        for data_row in data:
+            if self.allow_ids_on_add is False and self.get_id_attribute_value(data_row) is not None:
+                raise ConflictError("`add()` received identified item.")
+
+            self._update_audit_attributes(data_row, do_created=True, now=now)
+            if self.allow_ids_on_add is False:
+                id_ = self._id_factory()
+                self.set_id_attribute_value(id_, data_row)
+                self.collection[data_row.id] = data_row
+        return list(data)
+
+    def delete(self, item_id: Any) -> ModelT:
+        """Delete instance identified by ``item_id``.
+
+        Args:
+            item_id: Identifier of instance to be deleted.
+
+        Returns:
+            The deleted instance.
+
+        Raises:
+            NotFoundError: If no instance found identified by ``item_id``.
+        """
+        try:
+            return self._find_or_raise_not_found(item_id)
+        finally:
+            del self.collection[item_id]
+
+    def delete_many(self, item_ids: list[Any]) -> list[ModelT]:
+        """Delete instances identified by list of identifiers ``item_ids``.
+
+        Args:
+            item_ids: list of identifiers of instances to be deleted.
+
+        Returns:
+            The deleted instances.
+
+        """
+        instances: list[ModelT] = []
+        for item_id in item_ids:
+            obj = self.get_one_or_none(**{self.id_attribute: item_id})
+            if obj:
+                obj = self.delete(obj.id)
+                instances.append(obj)
+        return instances
+
+    def exists(self, **kwargs: Any) -> bool:
+        """Return true if the object specified by ``kwargs`` exists.
+
+        Args:
+            **kwargs: Identifier of the instance to be retrieved.
+
+        Returns:
+            True if the instance was found.  False if not found..
+
+        """
+        existing = self.get_one_or_none(**kwargs)
+        return bool(existing)
+
+    def get(self, item_id: Any, **kwargs: Any) -> ModelT:
+        """Get instance identified by ``item_id``.
+
+        Args:
+            item_id: Identifier of the instance to be retrieved.
+            **kwargs: additional arguments
+
+        Returns:
+            The retrieved instance.
+
+        Raises:
+            NotFoundError: If no instance found identified by ``item_id``.
+        """
+        return self._find_or_raise_not_found(item_id)
+
+    def get_or_create(self, match_fields: list[str] | str | None = None, **kwargs: Any) -> tuple[ModelT, bool]:
+        """Get instance identified by ``kwargs`` or create if it doesn't exist.
+
+        Args:
+            match_fields: a list of keys to use to match the existing model.  When empty, all fields are matched.
+            **kwargs: Identifier of the instance to be retrieved.
+
+        Returns:
+            a tuple that includes the instance and whether it needed to be created.
+
+        """
+        match_fields = match_fields if match_fields else self.match_fields
+        if isinstance(match_fields, str):
+            match_fields = [match_fields]
+        if match_fields:
+            match_filter = {
+                field_name: field_value
+                for field_name in match_fields
+                if (field_value := kwargs.get(field_name)) is not None
+            }
+        else:
+            match_filter = kwargs
+        existing = self.get_one_or_none(**match_filter)
+        if existing:
+            for field_name, new_field_value in kwargs.items():
+                field = getattr(existing, field_name, None)
+                if field and field != new_field_value:
+                    setattr(existing, field_name, new_field_value)
+
+            return existing, False
+        return self.add(self.model_type(**kwargs)), True  # pyright: ignore[reportGeneralTypeIssues]
+
+    def get_one(self, **kwargs: Any) -> ModelT:
+        """Get instance identified by query filters.
+
+        Args:
+            **kwargs: Instance attribute value filters.
+
+        Returns:
+            The retrieved instance or None
+
+        Raises:
+            NotFoundError: If no instance found identified by ``kwargs``.
+        """
+        data = self.list(**kwargs)
+        return self.check_not_found(data[0] if data else None)
+
+    def get_one_or_none(self, **kwargs: Any) -> ModelT | None:
+        """Get instance identified by query filters or None if not found.
+
+        Args:
+            **kwargs: Instance attribute value filters.
+
+        Returns:
+            The retrieved instance or None
+        """
+        data = self.list(**kwargs)
+        return data[0] if data else None
+
+    def count(self, *filters: FilterTypes, **kwargs: Any) -> int:
+        """Count of rows returned by query.
+
+        Args:
+            *filters: Types for specific filtering operations.
+            **kwargs: Instance attribute value filters.
+
+        Returns:
+            Count of instances in collection, ignoring pagination.
+        """
+        return len(self.list(*filters, **kwargs))
+
+    def update(self, data: ModelT) -> ModelT:
+        """Update instance with the attribute values present on ``data``.
+
+        Args:
+            data: An instance that should have a value for :attr:`id_attribute <AsyncGenericMockRepository.id_attribute>` that exists in the
+                collection.
+
+        Returns:
+            The updated instance.
+
+        Raises:
+            NotFoundError: If no instance found with same identifier as ``data``.
+        """
+        item = self._find_or_raise_not_found(self.get_id_attribute_value(data))
+        self._update_audit_attributes(data, do_created=False)
+        for key, val in model_items(data):
+            setattr(item, key, val)
+        return item
+
+    def update_many(self, data: list[ModelT]) -> list[ModelT]:
+        """Update instances with the attribute values present on ``data``.
+
+        Args:
+            data: A list of instances that should have a value for :attr:`id_attribute <AsyncGenericMockRepository.id_attribute>`
+                that exists in the collection.
+
+        Returns:
+            The updated instances.
+
+        Raises:
+            NotFoundError: If no instance found with same identifier as ``data``.
+        """
+        items = [self._find_or_raise_not_found(self.get_id_attribute_value(row)) for row in data]
+        now = self._now()
+        for item in items:
+            self._update_audit_attributes(item, do_created=False, now=now)
+            for key, val in model_items(item):
+                setattr(item, key, val)
+        return items
+
+    def upsert(self, data: ModelT) -> ModelT:
+        """Update or create instance.
+
+        Updates instance with the attribute values present on ``data``, or creates a new instance if
+        one doesn't exist.
+
+        Args:
+            data: Instance to update existing, or be created. Identifier used to determine if an
+                existing instance exists is the value of an attribute on `data` named as value of
+                :attr:`id_attribute <AsyncGenericMockRepository.id_attribute>`.
+
+        Returns:
+            The updated or created instance.
+
+        Raises:
+            NotFoundError: If no instance found with same identifier as ``data``.
+        """
+        item_id = self.get_id_attribute_value(data)
+        if item_id in self.collection:
+            return self.update(data)
+        return self.add(data)
+
+    def list_and_count(
+        self,
+        *filters: FilterTypes,
+        **kwargs: Any,
+    ) -> tuple[list[ModelT], int]:
+        """Get a list of instances, optionally filtered with a total row count.
+
+        Args:
+            *filters: Types for specific filtering operations.
+            **kwargs: Instance attribute value filters.
+
+        Returns:
+            List of instances, and count of records returned by query, ignoring pagination.
+        """
+        return self.list(*filters, **kwargs), self.count(*filters, **kwargs)
+
+    def list(self, *filters: FilterTypes, **kwargs: Any) -> list[ModelT]:
+        """Get a list of instances, optionally filtered.
+
+        Args:
+            *filters: Types for specific filtering operations.
+            **kwargs: Instance attribute value filters.
+
+        Returns:
+            The list of instances, after filtering applied.
+        """
+        return list(self.filter_collection_by_kwargs(self.collection, **kwargs).values())
+
+    def filter_collection_by_kwargs(  # type:ignore[override]
+        self, collection: MutableMapping[Hashable, ModelT], /, **kwargs: Any
+    ) -> MutableMapping[Hashable, ModelT]:
+        """Filter the collection by kwargs.
+
+        Args:
+            collection: set of objects to filter
+            **kwargs: key/value pairs such that objects remaining in the collection after filtering
+                have the property that their attribute named ``key`` has value equal to ``value``.
+        """
+        new_collection: dict[Hashable, ModelT] = {}
+        for item in self.collection.values():
+            try:
+                if all(getattr(item, name) == value for name, value in kwargs.items()):
+                    new_collection[item.id] = item
+            except AttributeError as orig:
+                raise RepositoryError from orig
+        return new_collection
+
+    @classmethod
+    def seed_collection(cls, instances: Iterable[ModelT]) -> None:
+        """Seed the collection for repository type.
+
+        Args:
+            instances: the instances to be added to the collection.
+        """
+        for instance in instances:
+            cls.collection[cls.get_id_attribute_value(instance)] = instance
+
+    @classmethod
+    def clear_collection(cls) -> None:
+        """Empty the collection for repository type."""
+        cls.collection = {}
+
+
+def model_items(model: Any) -> list[tuple[str, Any]]:
+    return [(k, v) for k, v in model.__dict__.items() if not k.startswith("_")]
```

### Comparing `litestar-2.0.0a7/litestar/contrib/sqlalchemy/base.py` & `litestar-2.0.0b1/litestar/contrib/sqlalchemy/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 """Application ORM configuration."""
 from __future__ import annotations
 
 import re
-from datetime import datetime
+from datetime import date, datetime, timezone
 from typing import TYPE_CHECKING, Any, ClassVar, Protocol, TypeVar, runtime_checkable
 from uuid import UUID, uuid4
 
 from pydantic import AnyHttpUrl, AnyUrl, EmailStr
-from sqlalchemy import Identity, MetaData, String
+from sqlalchemy import Date, MetaData, Sequence, String
 from sqlalchemy.event import listens_for
 from sqlalchemy.orm import (
     DeclarativeBase,
     Mapped,
     Session,
-    declarative_mixin,
     declared_attr,
     mapped_column,
     orm_insert_sentinel,
     registry,
 )
 
-from .types import GUID, JSON, BigIntIdentity
+from .types import GUID, BigIntIdentity, DateTimeUTC, JsonB
 
 if TYPE_CHECKING:
     from sqlalchemy.sql import FromClause
 
 __all__ = (
     "AuditColumns",
     "BigIntAuditBase",
@@ -62,16 +61,16 @@
     timestamp on modified instances.
 
     Args:
         session: The sync :class:`Session <sqlalchemy.orm.Session>` instance that underlies the async
             session.
     """
     for instance in session.dirty:
-        if hasattr(instance, "updated"):
-            instance.updated = datetime.now()  # noqa: DTZ005
+        if hasattr(instance, "updated_at"):
+            instance.updated = (datetime.now(timezone.utc),)
 
 
 @runtime_checkable
 class ModelProtocol(Protocol):
     """The base SQLAlchemy model protocol."""
 
     __table__: FromClause
@@ -82,51 +81,56 @@
 
         Returns:
             dict[str, Any]: A dict representation of the model
         """
         ...
 
 
-@declarative_mixin
 class UUIDPrimaryKey:
     """UUID Primary Key Field Mixin."""
 
-    __abstract__ = True
-
     id: Mapped[UUID] = mapped_column(default=uuid4, primary_key=True)  # pyright: ignore
     """UUID Primary key column."""
 
+    @declared_attr
+    def _sentinel(cls) -> Mapped[int]:
+        return orm_insert_sentinel()
+
 
-@declarative_mixin
 class BigIntPrimaryKey:
     """BigInt Primary Key Field Mixin."""
 
-    __abstract__ = True
-
-    id: Mapped[int] = mapped_column(BigIntIdentity, Identity(always=True), primary_key=True)  # pyright: ignore
-    """BigInt Primary key column."""
+    @declared_attr
+    def id(cls) -> Mapped[int]:
+        """BigInt Primary key column."""
+        return mapped_column(
+            BigIntIdentity,
+            Sequence(f"{cls.__tablename__}_id_seq", optional=False),  # type: ignore[attr-defined] # pyright: ignore
+            primary_key=True,
+        )
 
 
-@declarative_mixin
 class AuditColumns:
     """Created/Updated At Fields Mixin."""
 
-    __abstract__ = True
-
-    created: Mapped[datetime] = mapped_column(default=datetime.now)  # pyright: ignore
+    created_at: Mapped[datetime] = mapped_column(  # pyright: ignore
+        DateTimeUTC(timezone=True),
+        default=datetime.now(timezone.utc),
+    )
     """Date/time of instance creation."""
-    updated: Mapped[datetime] = mapped_column(default=datetime.now)  # pyright: ignore
+    updated_at: Mapped[datetime] = mapped_column(  # pyright: ignore
+        DateTimeUTC(timezone=True),
+        default=datetime.now(timezone.utc),
+    )
     """Date/time of instance last update."""
 
 
-@declarative_mixin
 class CommonTableAttributes:
     """Common attributes for SQLALchemy tables."""
 
-    __abstract__ = True
     __name__: ClassVar[str]
     __table__: FromClause
 
     # noinspection PyMethodParameters
     @declared_attr.directive
     def __tablename__(cls) -> str:  # pylint: disable=no-self-argument
         """Infer table name from class name."""
@@ -135,28 +139,32 @@
 
     def to_dict(self, exclude: set[str] | None = None) -> dict[str, Any]:
         """Convert model to dictionary.
 
         Returns:
             dict[str, Any]: A dict representation of the model
         """
-        exclude = exclude.union("_sentinel") if exclude else {"_sentinel"}
+        exclude = {"_sentinel"}.union(self._sa_instance_state.unloaded).union(exclude or [])  # type: ignore[attr-defined]
         return {field.name: getattr(self, field.name) for field in self.__table__.columns if field.name not in exclude}
 
-    @declared_attr
-    def _sentinel(cls) -> Mapped[int]:
-        return orm_insert_sentinel()
-
 
 def create_registry() -> registry:
     """Create a new SQLAlchemy registry."""
     meta = MetaData(naming_convention=convention)
     return registry(
         metadata=meta,
-        type_annotation_map={UUID: GUID, EmailStr: String, AnyUrl: String, AnyHttpUrl: String, dict: JSON},
+        type_annotation_map={
+            UUID: GUID,
+            EmailStr: String,
+            AnyUrl: String,
+            AnyHttpUrl: String,
+            dict: JsonB,
+            datetime: DateTimeUTC,
+            date: Date,
+        },
     )
 
 
 orm_registry = create_registry()
 
 
 class UUIDBase(UUIDPrimaryKey, CommonTableAttributes, DeclarativeBase):
```

### Comparing `litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/__init__.py` & `litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 )
 from .serialization import SQLAlchemySerializationPlugin
 
 
 class SQLAlchemyPlugin(SQLAlchemyInitPlugin, SQLAlchemySerializationPlugin):
     """A plugin that provides SQLAlchemy integration."""
 
+    def __init__(self, config: SQLAlchemyAsyncConfig | SQLAlchemySyncConfig) -> None:
+        SQLAlchemyInitPlugin.__init__(self, config=config)
+        SQLAlchemySerializationPlugin.__init__(self)
+
 
 __all__ = (
     "AsyncSessionConfig",
     "EngineConfig",
     "GenericSQLAlchemyConfig",
     "GenericSessionConfig",
     "SQLAlchemyAsyncConfig",
```

### Comparing `litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py` & `litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, cast
 
 from sqlalchemy.ext.asyncio import AsyncConnection, AsyncEngine, AsyncSession, async_sessionmaker, create_async_engine
 
+from litestar.constants import HTTP_RESPONSE_START
 from litestar.types import Empty
 from litestar.utils import delete_litestar_scope_state, get_litestar_scope_state
 
 from .common import SESSION_SCOPE_KEY, SESSION_TERMINUS_ASGI_EVENTS, GenericSessionConfig, GenericSQLAlchemyConfig
 
 if TYPE_CHECKING:
     from typing import Any, Callable
 
     from sqlalchemy.orm import Session
 
     from litestar import Litestar
-    from litestar.datastructures.state import State
     from litestar.types import BeforeMessageSendHookHandler, EmptyType, Message, Scope
+    from litestar.types.asgi_types import HTTPResponseStartEvent
 
-__all__ = ("SQLAlchemyAsyncConfig", "AsyncSessionConfig")
+__all__ = (
+    "SQLAlchemyAsyncConfig",
+    "AsyncSessionConfig",
+    "default_before_send_handler",
+    "autocommit_before_send_handler",
+)
 
 
-async def default_before_send_handler(message: Message, _: State, scope: Scope) -> None:
+async def default_before_send_handler(message: Message, scope: Scope) -> None:
     """Handle closing and cleaning up sessions before sending.
 
     Args:
         message: ASGI-``Message``
         _: A ``State`` (not used)
         scope: An ASGI-``Scope``
 
@@ -35,14 +41,37 @@
     """
     session = cast("AsyncSession | None", get_litestar_scope_state(scope, SESSION_SCOPE_KEY))
     if session and message["type"] in SESSION_TERMINUS_ASGI_EVENTS:
         await session.close()
         delete_litestar_scope_state(scope, SESSION_SCOPE_KEY)
 
 
+async def autocommit_before_send_handler(message: Message, scope: Scope) -> None:
+    """Handle commit/rollback, closing and cleaning up sessions before sending.
+
+    Args:
+        message: ASGI-``Message``
+        scope: An ASGI-``Scope``
+
+    Returns:
+        None
+    """
+    session = cast("AsyncSession | None", get_litestar_scope_state(scope, SESSION_SCOPE_KEY))
+    try:
+        if session is not None and message["type"] == HTTP_RESPONSE_START:
+            if 200 <= cast("HTTPResponseStartEvent", message)["status"] < 300:
+                await session.commit()
+            else:
+                await session.rollback()
+    finally:
+        if session and message["type"] in SESSION_TERMINUS_ASGI_EVENTS:
+            await session.close()
+            delete_litestar_scope_state(scope, SESSION_SCOPE_KEY)
+
+
 @dataclass
 class AsyncSessionConfig(GenericSessionConfig[AsyncConnection, AsyncEngine, AsyncSession]):
     """SQLAlchemy async session config."""
 
     sync_session_class: type[Session] | None | EmptyType = Empty
     """A :class:`Session <sqlalchemy.orm.Session>` subclass or other callable which will be used to construct the
     :class:`Session <sqlalchemy.orm.Session>` which will be proxied. This parameter may be used to provide custom
```

### Comparing `litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/init/config/common.py` & `litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/init/config/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,20 +181,22 @@
             return self.engine_instance
 
         if self.connection_string is None:
             raise ImproperlyConfiguredException("One of 'connection_string' or 'engine_instance' must be provided.")
 
         engine_config = self.engine_config_dict
         try:
-            return self.create_engine_callable(self.connection_string, **engine_config)
+            self.engine_instance = self.create_engine_callable(self.connection_string, **engine_config)
         except ValueError:
             # likely due to a dialect that doesn't support json type
             del engine_config["json_deserializer"]
             del engine_config["json_serializer"]
-            return self.create_engine_callable(self.connection_string, **engine_config)
+            self.engine_instance = self.create_engine_callable(self.connection_string, **engine_config)
+
+        return self.engine_instance
 
     def create_session_maker(self) -> Callable[[], SessionT]:
         """Get a session maker. If none exists yet, create one.
 
         Returns:
             Session factory used by the plugin.
         """
```

### Comparing `litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/init/config/engine.py` & `litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/init/config/engine.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/init/config/sync.py` & `litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/init/config/sync.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,29 +2,35 @@
 
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, cast
 
 from sqlalchemy import Connection, Engine, create_engine
 from sqlalchemy.orm import Session, sessionmaker
 
+from litestar.constants import HTTP_RESPONSE_START
 from litestar.utils import delete_litestar_scope_state, get_litestar_scope_state
 
 from .common import SESSION_SCOPE_KEY, SESSION_TERMINUS_ASGI_EVENTS, GenericSessionConfig, GenericSQLAlchemyConfig
 
 if TYPE_CHECKING:
     from typing import Any, Callable
 
     from litestar import Litestar
-    from litestar.datastructures.state import State
     from litestar.types import BeforeMessageSendHookHandler, Message, Scope
+    from litestar.types.asgi_types import HTTPResponseStartEvent
 
-__all__ = ("SQLAlchemySyncConfig", "SyncSessionConfig")
+__all__ = (
+    "SQLAlchemySyncConfig",
+    "SyncSessionConfig",
+    "default_before_send_handler",
+    "autocommit_before_send_handler",
+)
 
 
-async def default_before_send_handler(message: Message, _: State, scope: Scope) -> None:
+def default_before_send_handler(message: Message, scope: Scope) -> None:
     """Handle closing and cleaning up sessions before sending.
 
     Args:
         message: ASGI-``Message``
         _: A ``State`` (not used)
         scope: An ASGI-``Scope``
 
@@ -33,14 +39,37 @@
     """
     session = cast("Session | None", get_litestar_scope_state(scope, SESSION_SCOPE_KEY))
     if session and message["type"] in SESSION_TERMINUS_ASGI_EVENTS:
         session.close()
         delete_litestar_scope_state(scope, SESSION_SCOPE_KEY)
 
 
+def autocommit_before_send_handler(message: Message, scope: Scope) -> None:
+    """Handle commit/rollback, closing and cleaning up sessions before sending.
+
+    Args:
+        message: ASGI-``Message``
+        scope: An ASGI-``Scope``
+
+    Returns:
+        None
+    """
+    session = cast("Session | None", get_litestar_scope_state(scope, SESSION_SCOPE_KEY))
+    try:
+        if session is not None and message["type"] == HTTP_RESPONSE_START:
+            if 200 <= cast("HTTPResponseStartEvent", message)["status"] < 300:
+                session.commit()
+            else:
+                session.rollback()
+    finally:
+        if session and message["type"] in SESSION_TERMINUS_ASGI_EVENTS:
+            session.close()
+            delete_litestar_scope_state(scope, SESSION_SCOPE_KEY)
+
+
 class SyncSessionConfig(GenericSessionConfig[Connection, Engine, Session]):
     pass
 
 
 @dataclass
 class SQLAlchemySyncConfig(GenericSQLAlchemyConfig[Engine, Session, sessionmaker]):
     """Sync SQLAlchemy Configuration."""
```

### Comparing `litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/init/plugin.py` & `litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/init/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,11 +36,11 @@
         app_config.dependencies.update(
             {
                 self._config.engine_dependency_key: Provide(self._config.provide_engine, sync_to_thread=False),
                 self._config.session_dependency_key: Provide(self._config.provide_session, sync_to_thread=False),
             }
         )
         app_config.before_send.append(self._config.before_send_handler)
-        app_config.on_startup.append(self._config.update_app_state)
+        app_config.on_startup.insert(0, self._config.update_app_state)
         app_config.on_shutdown.append(self._config.on_shutdown)
         app_config.signature_namespace.update(self._config.signature_namespace)
         return app_config
```

### Comparing `litestar-2.0.0a7/litestar/contrib/sqlalchemy/plugins/serialization.py` & `litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/serialization.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,25 +6,24 @@
 
 from litestar.contrib.sqlalchemy.dto import SQLAlchemyDTO
 from litestar.plugins import SerializationPluginProtocol
 
 from . import _slots_base
 
 if TYPE_CHECKING:
-    from litestar.utils.signature import ParsedType
+    from litestar.typing import ParsedType
 
 
 class SQLAlchemySerializationPlugin(SerializationPluginProtocol, _slots_base.SlotsBase):
     __slots__ = ()
 
     def __init__(self) -> None:
         self._type_dto_map: dict[type[DeclarativeBase], type[SQLAlchemyDTO]] = {}
 
-    @staticmethod
-    def supports_type(parsed_type: ParsedType) -> bool:
+    def supports_type(self, parsed_type: ParsedType) -> bool:
         return (
             parsed_type.is_collection and parsed_type.has_inner_subclass_of(DeclarativeBase)
         ) or parsed_type.is_subclass_of(DeclarativeBase)
 
     def create_dto_for_type(self, parsed_type: ParsedType) -> type[SQLAlchemyDTO]:
         # assumes that the type is a container of SQLAlchemy models or a single SQLAlchemy model
         for inner_type in parsed_type.inner_types:
```

### Comparing `litestar-2.0.0a7/litestar/contrib/sqlalchemy/repository.py` & `litestar-2.0.0b1/litestar/contrib/sqlalchemy/repository/_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,71 +1,38 @@
-"""SQLAlchemy-based implementation of the repository protocol."""
 from __future__ import annotations
 
-from contextlib import contextmanager
-from typing import TYPE_CHECKING, Any, Generic, Literal, Tuple, TypeVar, cast
+from typing import TYPE_CHECKING, Any, Generic, Literal, cast
 
-from sqlalchemy import Select, delete, over, select, text, update
+from sqlalchemy import Result, Select, delete, over, select, text, update
 from sqlalchemy import func as sql_func
-from sqlalchemy.exc import IntegrityError, SQLAlchemyError
 
-from litestar.contrib.repository.abc import AbstractAsyncRepository
-from litestar.contrib.repository.exceptions import ConflictError, RepositoryError
+from litestar.contrib.repository import (  # noqa: RUF100, F401
+    AbstractAsyncRepository,
+    AbstractSyncRepository,
+    RepositoryError,
+)
 from litestar.contrib.repository.filters import (
     BeforeAfter,
     CollectionFilter,
+    FilterTypes,
     LimitOffset,
     OrderBy,
     SearchFilter,
 )
 
+from ._util import wrap_sqlalchemy_exception
+from .types import ModelT, RowT, SelectT
+
 if TYPE_CHECKING:
     from collections import abc
     from datetime import datetime
 
-    from sqlalchemy.engine import Result
-    from sqlalchemy.ext.asyncio import AsyncSession
-
-    from litestar.contrib.repository import FilterTypes
-
-    from . import base
-
-__all__ = (
-    "SQLAlchemyAsyncRepository",
-    "ModelT",
-)
-
-T = TypeVar("T")
-ModelT = TypeVar("ModelT", bound="base.ModelProtocol")
-SQLARepoT = TypeVar("SQLARepoT", bound="SQLAlchemyAsyncRepository")
-SelectT = TypeVar("SelectT", bound="Select[Any]")
-RowT = TypeVar("RowT", bound=Tuple[Any, ...])
-
-
-@contextmanager
-def wrap_sqlalchemy_exception() -> Any:
-    """Do something within context to raise a `RepositoryError` chained
-    from an original `SQLAlchemyError`.
-
-        >>> try:
-        ...     with wrap_sqlalchemy_exception():
-        ...         raise SQLAlchemyError("Original Exception")
-        ... except RepositoryError as exc:
-        ...     print(f"caught repository exception from {type(exc.__context__)}")
-        ...
-        caught repository exception from <class 'sqlalchemy.exc.SQLAlchemyError'>
-    """
-    try:
-        yield
-    except IntegrityError as exc:
-        raise ConflictError from exc
-    except SQLAlchemyError as exc:
-        raise RepositoryError(f"An exception occurred: {exc}") from exc
-    except AttributeError as exc:
-        raise RepositoryError from exc
+    from sqlalchemy.engine.interfaces import _CoreSingleExecuteParams
+    from sqlalchemy.ext.asyncio import AsyncSession  # noqa: RUF100, F401
+    from sqlalchemy.orm import Session  # noqa: RUF100, F401
 
 
 class SQLAlchemyAsyncRepository(AbstractAsyncRepository[ModelT], Generic[ModelT]):
     """SQLAlchemy based implementation of the repository interface."""
 
     match_fields: list[str] | str | None = None
 
@@ -77,14 +44,19 @@
             session: Session managing the unit-of-work for the operation.
             **kwargs: Additional arguments.
 
         """
         super().__init__(**kwargs)
         self.session = session
         self.statement = statement if statement is not None else select(self.model_type)
+        if not self.session.bind:
+            # this shouldn't actually ever happen, but we include it anyway to properly
+            # narrow down the types
+            raise ValueError("Session improperly configure")
+        self._dialect = self.session.bind.dialect
 
     async def add(self, data: ModelT) -> ModelT:
         """Add `data` to the collection.
 
         Args:
             data: Instance to be added to the collection.
 
@@ -145,15 +117,15 @@
 
         """
         with wrap_sqlalchemy_exception():
             instances: list[ModelT] = []
             chunk_size = 450
             for idx in range(0, len(item_ids), chunk_size):
                 chunk = item_ids[idx : min(idx + chunk_size, len(item_ids))]
-                if self.session.bind.dialect.delete_executemany_returning:
+                if self._dialect.delete_executemany_returning:
                     instances.extend(
                         await self.session.scalars(
                             delete(self.model_type)
                             .where(getattr(self.model_type, self.id_attribute).in_(chunk))
                             .returning(self.model_type)
                         )
                     )
@@ -270,16 +242,17 @@
         if not existing:
             return await self.add(self.model_type(**kwargs)), True  # pyright: ignore[reportGeneralTypeIssues]
         if upsert:
             for field_name, new_field_value in kwargs.items():
                 field = getattr(existing, field_name, None)
                 if field and field != new_field_value:
                     setattr(existing, field_name, new_field_value)
-            if existing in self.session.dirty:
-                return (await self.update(existing)), False
+            existing = await self._attach_to_session(existing, strategy="merge")
+            await self.session.flush()
+            self.session.expunge(existing)
         return existing, False
 
     async def count(self, *filters: FilterTypes, **kwargs: Any) -> int:
         """Get the count of records returned by a query.
 
         Args:
             *filters: Types for specific filtering operations.
@@ -314,15 +287,14 @@
         with wrap_sqlalchemy_exception():
             item_id = self.get_id_attribute_value(data)
             # this will raise for not found, and will put the item in the session
             await self.get(item_id)
             # this will merge the inbound data to the instance we just put in the session
             instance = await self._attach_to_session(data, strategy="merge")
             await self.session.flush()
-            await self.session.refresh(instance)
             self.session.expunge(instance)
             return instance
 
     async def update_many(self, data: list[ModelT]) -> list[ModelT]:
         """Update one or more instances with the attribute values present on `data`.
 
         This function has an optimized bulk insert based on the configured SQL dialect:
@@ -337,19 +309,21 @@
             The updated instances.
 
         Raises:
             NotFoundError: If no instance found with same identifier as `data`.
         """
         data_to_update: list[dict[str, Any]] = [v.to_dict() if isinstance(v, self.model_type) else v for v in data]  # type: ignore
         with wrap_sqlalchemy_exception():
-            if self.session.bind.dialect.update_executemany_returning:
+            if self._dialect.update_executemany_returning and self._dialect.name != "oracle":
                 instances = list(
-                    await self.session.scalars(  # type: ignore
+                    await self.session.scalars(
                         update(self.model_type).returning(self.model_type),
-                        data_to_update,  # pyright: ignore[reportGeneralTypeIssues]
+                        cast("_CoreSingleExecuteParams", data_to_update),  # this is not correct but the only way
+                        # currently to deal with an SQLAlchemy typing issue. See
+                        # https://github.com/sqlalchemy/sqlalchemy/discussions/9925
                     )
                 )
                 await self.session.flush()
                 for instance in instances:
                     self.session.expunge(instance)
                 return instances
             await self.session.execute(
@@ -369,14 +343,32 @@
         Args:
             *filters: Types for specific filtering operations.
             **kwargs: Instance attribute value filters.
 
         Returns:
             Count of records returned by query, ignoring pagination.
         """
+        if self._dialect.name in {"spanner", "spanner+spanner"}:
+            return await self._list_and_count_basic(*filters, **kwargs)
+        return await self._list_and_count_window(*filters, **kwargs)
+
+    async def _list_and_count_window(
+        self,
+        *filters: FilterTypes,
+        **kwargs: Any,
+    ) -> tuple[list[ModelT], int]:
+        """List records with total count.
+
+        Args:
+            *filters: Types for specific filtering operations.
+            **kwargs: Instance attribute value filters.
+
+        Returns:
+            Count of records returned by query using an analytical window function, ignoring pagination.
+        """
         statement = kwargs.pop("statement", self.statement)
         statement = statement.add_columns(over(sql_func.count(self.get_id_attribute_value(self.model_type))))
         statement = self._apply_filters(*filters, statement=statement)
         statement = self._filter_select_by_kwargs(statement, **kwargs)
         with wrap_sqlalchemy_exception():
             result = await self._execute(statement)
             count: int = 0
@@ -384,14 +376,45 @@
             for i, (instance, count_value) in enumerate(result):
                 self.session.expunge(instance)
                 instances.append(instance)
                 if i == 0:
                     count = count_value
             return instances, count
 
+    async def _list_and_count_basic(
+        self,
+        *filters: FilterTypes,
+        **kwargs: Any,
+    ) -> tuple[list[ModelT], int]:
+        """List records with total count.
+
+        Args:
+            *filters: Types for specific filtering operations.
+            **kwargs: Instance attribute value filters.
+
+        Returns:
+            Count of records returned by query using 2 queries, ignoring pagination.
+        """
+        statement = kwargs.pop("statement", self.statement)
+        statement = self._apply_filters(*filters, statement=statement)
+        statement = self._filter_select_by_kwargs(statement, **kwargs)
+        count_statement = statement.with_only_columns(
+            sql_func.count(self.get_id_attribute_value(self.model_type)),
+            maintain_column_froms=True,
+        ).order_by(None)
+        with wrap_sqlalchemy_exception():
+            count_result = await self.session.execute(count_statement)
+            count = count_result.scalar_one()
+            result = await self._execute(statement)
+            instances: list[ModelT] = []
+            for (instance,) in result:
+                self.session.expunge(instance)
+                instances.append(instance)
+            return instances, count
+
     async def list(self, *filters: FilterTypes, **kwargs: Any) -> list[ModelT]:
         """Get a list of instances, optionally filtered.
 
         Args:
             *filters: Types for specific filtering operations.
             **kwargs: Instance attribute value filters.
 
@@ -425,15 +448,14 @@
 
         Raises:
             NotFoundError: If no instance found with same identifier as `data`.
         """
         with wrap_sqlalchemy_exception():
             instance = await self._attach_to_session(data, strategy="merge")
             await self.session.flush()
-            await self.session.refresh(instance)
             self.session.expunge(instance)
             return instance
 
     def filter_collection_by_kwargs(  # type:ignore[override]
         self, collection: SelectT, /, **kwargs: Any
     ) -> SelectT:
         """Filter the collection by kwargs.
@@ -456,19 +478,14 @@
         Returns:
             `True` if healthy.
         """
         return (  # type:ignore[no-any-return]  # pragma: no cover
             await session.execute(text("SELECT 1"))
         ).scalar_one() == 1
 
-    # the following is all sqlalchemy implementation detail, and shouldn't be directly accessed
-
-    def _apply_limit_offset_pagination(self, limit: int, offset: int, statement: SelectT) -> SelectT:
-        return statement.limit(limit).offset(offset)
-
     async def _attach_to_session(self, model: ModelT, strategy: Literal["add", "merge"] = "add") -> ModelT:
         """Attach detached instance to the session.
 
         Args:
             model: The instance to be attached to the session.
             strategy: How the instance should be attached.
                 - "add": New instance added to session
@@ -484,14 +501,17 @@
         if strategy == "merge":
             return await self.session.merge(model)
         raise ValueError("Unexpected value for `strategy`, must be `'add'` or `'merge'`")
 
     async def _execute(self, statement: Select[RowT]) -> Result[RowT]:
         return cast("Result[RowT]", await self.session.execute(statement))
 
+    def _apply_limit_offset_pagination(self, limit: int, offset: int, statement: SelectT) -> SelectT:
+        return statement.limit(limit).offset(offset)
+
     def _apply_filters(self, *filters: FilterTypes, apply_pagination: bool = True, statement: SelectT) -> SelectT:
         """Apply filters to a select statement.
 
         Args:
             *filters: filter types to apply to the query
             apply_pagination: applies pagination filters if true
             statement: select statement to apply filters
@@ -530,15 +550,15 @@
     def _filter_on_datetime_field(
         self, field_name: str, before: datetime | None, after: datetime | None, statement: SelectT
     ) -> SelectT:
         field = getattr(self.model_type, field_name)
         if before is not None:
             statement = statement.where(field < before)
         if after is not None:
-            statement = statement.where(field > before)
+            statement = statement.where(field > after)
         return statement
 
     def _filter_select_by_kwargs(self, statement: SelectT, **kwargs: Any) -> SelectT:
         for key, val in kwargs.items():
             statement = statement.where(getattr(self.model_type, key) == val)
         return statement
```

### Comparing `litestar-2.0.0a7/litestar/controller.py` & `litestar-2.0.0b1/litestar/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from collections import defaultdict
 from copy import copy
-from typing import TYPE_CHECKING, Any, DefaultDict, Mapping, cast
+from typing import TYPE_CHECKING, Any, Mapping, cast
 
 from litestar._layers.utils import narrow_response_cookies, narrow_response_headers
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.handlers.base import BaseRouteHandler
 from litestar.handlers.http_handlers import HTTPRouteHandler
 from litestar.handlers.websocket_handlers import WebsocketRouteHandler
 from litestar.types.empty import Empty
@@ -210,15 +210,15 @@
 
         Raises:
             ImproperlyConfiguredException
 
         Returns:
             None
         """
-        paths: DefaultDict[str, set[str]] = defaultdict(set)
+        paths: defaultdict[str, set[str]] = defaultdict(set)
 
         for route_handler in route_handlers:
             if isinstance(route_handler, HTTPRouteHandler):
                 methods: set[str] = cast("set[str]", route_handler.http_methods)
             elif isinstance(route_handler, WebsocketRouteHandler):
                 methods = {"websocket"}
             else:
```

### Comparing `litestar-2.0.0a7/litestar/data_extractors.py` & `litestar-2.0.0b1/litestar/data_extractors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Callable, Coroutine, Literal, cast
-
-from typing_extensions import TypedDict
+from typing import TYPE_CHECKING, Any, Callable, Coroutine, Literal, TypedDict, cast
 
 from litestar._parsers import parse_cookie_string
 from litestar.connection.request import Request
 from litestar.datastructures.upload_file import UploadFile
 from litestar.enums import HttpMethod, RequestEncodingType
 
-__all__ = ("ConnectionDataExtractor", "ExtractedRequestData", "ExtractedResponseData", "ResponseDataExtractor")
+__all__ = (
+    "ConnectionDataExtractor",
+    "ExtractedRequestData",
+    "ExtractedResponseData",
+    "ResponseDataExtractor",
+    "RequestExtractorField",
+    "ResponseExtractorField",
+)
 
 
 if TYPE_CHECKING:
     from litestar.connection import ASGIConnection
     from litestar.types import Method
     from litestar.types.asgi_types import HTTPResponseBodyEvent, HTTPResponseStartEvent
```

### Comparing `litestar-2.0.0a7/litestar/datastructures/__init__.py` & `litestar-2.0.0b1/litestar/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/datastructures/cookie.py` & `litestar-2.0.0b1/litestar/datastructures/cookie.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/datastructures/headers.py` & `litestar-2.0.0b1/litestar/datastructures/headers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/datastructures/multi_dicts.py` & `litestar-2.0.0b1/litestar/datastructures/multi_dicts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/datastructures/response_header.py` & `litestar-2.0.0b1/litestar/datastructures/response_header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/datastructures/state.py` & `litestar-2.0.0b1/litestar/datastructures/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 from __future__ import annotations
 
 from copy import copy, deepcopy
 from threading import RLock
-from typing import Any, Callable, Generator, Iterable, Iterator, Mapping, MutableMapping
+from typing import TYPE_CHECKING, Any, Callable, Generator, Iterable, Iterator, Mapping, MutableMapping
+
+if TYPE_CHECKING:
+    from typing_extensions import Self
 
 __all__ = ("ImmutableState", "State")
 
 
 class ImmutableState(Mapping[str, Any]):
     """An object meant to store arbitrary state.
 
     It can be accessed using dot notation while exposing dict like functionalities.
     """
 
-    __slots__ = ("_state",)
+    __slots__ = (
+        "_state",
+        "_deep_copy",
+    )
 
     _state: dict[str, Any]
 
     def __init__(
         self, state: ImmutableState | Mapping[str, Any] | Iterable[tuple[str, Any]], deep_copy: bool = True
     ) -> None:
         """Initialize an ``ImmutableState`` instance.
@@ -52,21 +58,21 @@
 
                 # you can also retrieve a mutable State by calling 'mutable_copy'
                 mutable_state = state.mutable_copy()
                 del state["first"]
                 assert "first" not in state
 
         """
-
         if isinstance(state, ImmutableState):
             state = state._state
 
         if not isinstance(state, dict) and isinstance(state, Iterable):
             state = dict(state)
 
+        super().__setattr__("_deep_copy", deep_copy)
         super().__setattr__("_state", deepcopy(state) if deep_copy else state)
 
     def __bool__(self) -> bool:
         """Return a boolean indicating whether the wrapped dict instance has values."""
         return bool(self._state)
 
     def __getitem__(self, key: str) -> Any:
@@ -112,28 +118,28 @@
             The retrieved value
         """
         try:
             return self._state[key]
         except KeyError as e:
             raise AttributeError from e
 
-    def __copy__(self) -> ImmutableState:
+    def __copy__(self) -> Self:
         """Return a shallow copy of the given state object.
 
         Customizes how the builtin "copy" function will work.
         """
-        return self.__class__(deepcopy(self._state))
+        return self.__class__(self._state, deep_copy=self._deep_copy)
 
     def mutable_copy(self) -> State:
         """Return a mutable copy of the state object.
 
         Returns:
             A ``State``
         """
-        return State(self._state)
+        return State(self._state, deep_copy=self._deep_copy)
 
     def dict(self) -> dict[str, Any]:
         """Return a shallow copy of the wrapped dict.
 
         Returns:
             A dict
         """
@@ -143,25 +149,26 @@
     def __get_validators__(
         cls,
     ) -> Generator[Callable[[ImmutableState | dict[str, Any] | Iterable[tuple[str, Any]]], ImmutableState], None, None]:  # type: ignore[valid-type]
         """Pydantic compatible method to allow custom parsing of state instances in a SignatureModel."""
         yield cls.validate
 
     @classmethod
-    def validate(cls, value: ImmutableState | dict[str, Any] | Iterable[tuple[str, Any]]) -> ImmutableState:  # type: ignore[valid-type]
+    def validate(cls, value: ImmutableState | dict[str, Any] | Iterable[tuple[str, Any]]) -> Self:  # type: ignore[valid-type]
         """Parse a value and instantiate state inside a SignatureModel. This allows us to use custom subclasses of
         state, as well as allows users to decide whether state is mutable or immutable.
 
         Args:
             value: The value from which to initialize the state instance.
 
         Returns:
             An ImmutableState instance
         """
-        return cls(value)
+        deep_copy = value._deep_copy if isinstance(value, ImmutableState) else False
+        return cls(value, deep_copy=deep_copy)
 
 
 class State(ImmutableState, MutableMapping[str, Any]):
     """An object meant to store arbitrary state.
 
     It can be accessed using dot notation while exposing dict like functionalities.
     """
@@ -285,22 +292,22 @@
 
         try:
             with self._lock:
                 del self._state[key]
         except KeyError as e:
             raise AttributeError from e
 
-    def copy(self) -> State:
+    def copy(self) -> Self:
         """Return a shallow copy of the state object.
 
         Returns:
             A ``State``
         """
-        return self.__class__(self.dict())
+        return self.__class__(self.dict(), deep_copy=self._deep_copy)
 
     def immutable_copy(self) -> ImmutableState:
         """Return a shallow copy of the state object, setting it to be frozen.
 
         Returns:
             A ``State``
         """
-        return ImmutableState(self)
+        return ImmutableState(self, deep_copy=self._deep_copy)
```

### Comparing `litestar-2.0.0a7/litestar/datastructures/upload_file.py` & `litestar-2.0.0b1/litestar/datastructures/upload_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,10 +115,8 @@
             field_schema: The schema being generated for the field.
             field: the model class field.
 
         Returns:
             None
         """
         if field:
-            field_schema.update(
-                {"type": OpenAPIType.STRING.value, "contentMediaType": "application/octet-stream", "format": "binary"}
-            )
+            field_schema.update({"type": OpenAPIType.STRING.value, "contentMediaType": "application/octet-stream"})
```

### Comparing `litestar-2.0.0a7/litestar/datastructures/url.py` & `litestar-2.0.0b1/litestar/datastructures/url.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/di.py` & `litestar-2.0.0b1/litestar/di.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from __future__ import annotations
 
 from inspect import isclass
 from typing import TYPE_CHECKING, Any
 
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.types import Empty
-from litestar.utils import Ref, is_async_callable
-from litestar.utils.warnings import warn_implicit_sync_to_thread, warn_sync_to_thread_with_async_callable
+from litestar.utils import Ref
+from litestar.utils.predicates import is_async_callable, is_sync_or_async_generator
+from litestar.utils.warnings import (
+    warn_implicit_sync_to_thread,
+    warn_sync_to_thread_with_async_callable,
+    warn_sync_to_thread_with_generator,
+)
 
 __all__ = ("Provide",)
 
 
 if TYPE_CHECKING:
     from litestar._signature import SignatureModel
     from litestar.types import AnyCallable
@@ -46,19 +51,22 @@
             sync_to_thread: Run sync code in an async thread. Defaults to False.
         """
         if not callable(dependency):
             raise ImproperlyConfiguredException("Provider dependency must a callable value")
 
         self.dependency = Ref["AnyCallable"](dependency)
         self.has_sync_callable = isclass(dependency) or not is_async_callable(dependency)
-        if self.has_sync_callable and sync_to_thread is None:
+        if self.has_sync_callable and sync_to_thread is None and not is_sync_or_async_generator(dependency):
             warn_implicit_sync_to_thread(dependency, stacklevel=3)
 
-        if not self.has_sync_callable and sync_to_thread is not None:
-            warn_sync_to_thread_with_async_callable(dependency, stacklevel=3)
+        if sync_to_thread is not None:
+            if is_sync_or_async_generator(dependency):
+                warn_sync_to_thread_with_generator(dependency, stacklevel=3)
+            elif not self.has_sync_callable:
+                warn_sync_to_thread_with_async_callable(dependency, stacklevel=3)  # pyright: ignore
 
         self.sync_to_thread = bool(sync_to_thread)
         self.use_cache = use_cache
         self.value: Any = Empty
 
     async def __call__(self, **kwargs: Any) -> Any:
         """Call the provider's dependency."""
```

### Comparing `litestar-2.0.0a7/litestar/dto/factory/_backends/abc.py` & `litestar-2.0.0b1/litestar/dto/factory/_backends/abc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """DTO backends do the heavy lifting of decoding and validating raw bytes into domain models, and
 back again, to bytes.
 """
 from __future__ import annotations
 
 import secrets
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Final, Generic, TypeVar, Union
-
-from msgspec import UNSET, UnsetType
+from typing import TYPE_CHECKING, Any, Final, Generic, TypeVar, cast
 
 from litestar._openapi.schema_generation import create_schema
 from litestar._signature.field import SignatureField
-from litestar.dto.factory import DTOData
+from litestar.dto.factory import DTOData, Mark
+from litestar.typing import ParsedType
 from litestar.utils.helpers import get_fully_qualified_class_name
-from litestar.utils.signature import ParsedType
 
 from .types import (
     CollectionType,
     CompositeType,
     MappingType,
     NestedFieldInfo,
     SimpleType,
@@ -25,22 +23,24 @@
     TupleType,
     UnionType,
 )
 from .utils import (
     RenameStrategies,
     build_annotation_for_backend,
     should_exclude_field,
+    should_ignore_field,
+    should_mark_private,
     transfer_data,
 )
 
 if TYPE_CHECKING:
-    from typing import AbstractSet, Any, Callable, Generator
+    from typing import AbstractSet, Callable, Generator
 
     from litestar.dto.factory import DTOConfig
-    from litestar.dto.factory.types import FieldDefinition
+    from litestar.dto.factory.data_structures import FieldDefinition
     from litestar.dto.interface import ConnectionContext
     from litestar.dto.types import ForType
     from litestar.openapi.spec import Reference, Schema
     from litestar.types.serialization import LitestarEncodableType
 
     from .types import FieldDefinitionsType
 
@@ -55,44 +55,49 @@
     __slots__ = (
         "config",
         "dto_for",
         "field_definition_generator",
         "is_nested_field_predicate",
         "model_type",
         "parsed_type",
+        "wrapper_attribute_name",
     )
 
     def __init__(
         self,
         dto_config: DTOConfig,
         dto_for: ForType,
         parsed_type: ParsedType,
         field_definition_generator: Callable[[Any], Generator[FieldDefinition, None, None]],
         is_nested_field_predicate: Callable[[ParsedType], bool],
         model_type: type[Any],
+        wrapper_attribute_name: str | None,
     ) -> None:
         """Create a backend context.
 
         Args:
             dto_config: DTO config.
             dto_for: "data" or "return"
             parsed_type: Parsed type.
             field_definition_generator: Generator that produces
                 :class:`FieldDefinition <.dto.factory.types.FieldDefinition>` instances given ``model_type``.
             is_nested_field_predicate: Function that detects if a field is nested.
             model_type: Model type.
+            wrapper_attribute_name: If the data that DTO should operate upon is wrapped in a generic datastructure, this is the
+                name of the attribute that the data is stored in.
         """
         self.config: Final[DTOConfig] = dto_config
         self.dto_for: Final[ForType] = dto_for
         self.parsed_type: Final[ParsedType] = parsed_type
         self.field_definition_generator: Final[
             Callable[[Any], Generator[FieldDefinition, None, None]]
         ] = field_definition_generator
         self.is_nested_field_predicate: Final[Callable[[ParsedType], bool]] = is_nested_field_predicate
         self.model_type: Final[type[Any]] = model_type
+        self.wrapper_attribute_name = wrapper_attribute_name
 
 
 class NestedDepthExceededError(Exception):
     """Raised when a nested type exceeds the maximum allowed depth.
 
     Not an exception that is intended to be raised into userland, rather a signal to the process that is iterating over
     the field definitions that the current field should be skipped.
@@ -119,25 +124,20 @@
         self.parsed_field_definitions = self.parse_model(context.model_type, context.config.exclude)
         self.transfer_model_type = self.create_transfer_model_type(
             get_fully_qualified_class_name(context.model_type), self.parsed_field_definitions
         )
         self.dto_data_type: type[DTOData] | None = None
         if context.parsed_type.is_subclass_of(DTOData):
             self.dto_data_type = context.parsed_type.annotation
-            annotation = self.dto_data_type.parsed_type.annotation
+            annotation = self.context.parsed_type.inner_types[0].annotation
         else:
             annotation = context.parsed_type.annotation
         self.annotation = build_annotation_for_backend(annotation, self.transfer_model_type)
 
-    def parse_model(
-        self,
-        model_type: Any,
-        exclude: AbstractSet[str],
-        nested_depth: int = 0,
-    ) -> FieldDefinitionsType:
+    def parse_model(self, model_type: Any, exclude: AbstractSet[str], nested_depth: int = 0) -> FieldDefinitionsType:
         """Reduce :attr:`model_type` to :class:`FieldDefinitionsType`.
 
         .. important::
             Implementations must respect the :attr:`config` object. For example:
                 - fields marked private must never be included in the field definitions.
                 - if a ``purpose`` is declared, then read-only fields must be taken into account.
                 - field renaming must be implemented.
@@ -156,21 +156,19 @@
             {"new_field": (str, "default")}
 
             Add a new field called "new_field", that may be `None`:
             {"new_field": (str | None, None)}
         """
         defined_fields = []
         for field_definition in self.context.field_definition_generator(model_type):
-            if should_exclude_field(field_definition, exclude, self.context.dto_for):
+            if should_ignore_field(field_definition, self.context.dto_for):
                 continue
 
-            if self.context.config.partial:
-                field_definition = field_definition.copy_with(
-                    parsed_type=ParsedType(Union[field_definition.parsed_type.annotation, UnsetType]), default=UNSET
-                )
+            if should_mark_private(field_definition, self.context.config.underscore_fields_private):
+                field_definition.dto_field.mark = Mark.PRIVATE
 
             try:
                 transfer_type = self._create_transfer_type(
                     field_definition.parsed_type,
                     exclude,
                     field_definition.name,
                     field_definition.unique_name(),
@@ -187,14 +185,15 @@
                 serialization_name = field_definition.name
 
             transfer_field_definition = TransferFieldDefinition.from_field_definition(
                 field_definition=field_definition,
                 serialization_name=serialization_name,
                 transfer_type=transfer_type,
                 is_partial=self.context.config.partial,
+                is_excluded=should_exclude_field(field_definition, exclude, self.context.dto_for),
             )
             defined_fields.append(transfer_field_definition)
         return tuple(defined_fields)
 
     @abstractmethod
     def create_transfer_model_type(self, unique_name: str, field_definitions: FieldDefinitionsType) -> type[BackendT]:
         """Create a model for data transfer.
@@ -241,29 +240,35 @@
         Returns:
             Instance or collection of ``model_type`` instances.
         """
         if self.dto_data_type:
             return self.dto_data_type(
                 backend=self,
                 data_as_builtins=transfer_data(
-                    dict, self.parse_builtins(builtins, connection_context), self.parsed_field_definitions, "data"
+                    dict,
+                    self.parse_builtins(builtins, connection_context),
+                    self.parsed_field_definitions,
+                    "data",
+                    self.context.parsed_type,
                 ),
             )
         return self.transfer_data_from_builtins(self.parse_builtins(builtins, connection_context))
 
     def transfer_data_from_builtins(self, builtins: Any) -> Any:
         """Populate model instance from builtin types.
 
         Args:
             builtins: Builtin type.
 
         Returns:
             Instance or collection of ``model_type`` instances.
         """
-        return transfer_data(self.context.model_type, builtins, self.parsed_field_definitions, "data")
+        return transfer_data(
+            self.context.model_type, builtins, self.parsed_field_definitions, "data", self.context.parsed_type
+        )
 
     def populate_data_from_raw(self, raw: bytes, connection_context: ConnectionContext) -> Any:
         """Parse raw bytes into instance of `model_type`.
 
         Args:
             raw: bytes
             connection_context: Information about the active connection.
@@ -271,39 +276,71 @@
         Returns:
             Instance or collection of ``model_type`` instances.
         """
         if self.dto_data_type:
             return self.dto_data_type(
                 backend=self,
                 data_as_builtins=transfer_data(
-                    dict, self.parse_raw(raw, connection_context), self.parsed_field_definitions, "data"
+                    dict,
+                    self.parse_raw(raw, connection_context),
+                    self.parsed_field_definitions,
+                    "data",
+                    self.context.parsed_type,
                 ),
             )
         return transfer_data(
-            self.context.model_type, self.parse_raw(raw, connection_context), self.parsed_field_definitions, "data"
+            self.context.model_type,
+            self.parse_raw(raw, connection_context),
+            self.parsed_field_definitions,
+            "data",
+            self.context.parsed_type,
         )
 
     def encode_data(self, data: Any, connection_context: ConnectionContext) -> LitestarEncodableType:
         """Encode data into a ``LitestarEncodableType``.
 
         Args:
             data: Data to encode.
             connection_context: Information about the active connection.
 
         Returns:
             Encoded data.
         """
+        if self.context.wrapper_attribute_name:
+            setattr(
+                data,
+                self.context.wrapper_attribute_name,
+                transfer_data(
+                    destination_type=self.transfer_model_type,
+                    source_data=getattr(data, self.context.wrapper_attribute_name),
+                    field_definitions=self.parsed_field_definitions,
+                    dto_for="return",
+                    parsed_type=self.context.parsed_type,
+                ),
+            )
+            # cast() here because we take for granted that whatever ``data`` is, it must be something
+            # that litestar can natively encode.
+            return cast("LitestarEncodableType", data)
+
         return transfer_data(
-            self.transfer_model_type, data, self.parsed_field_definitions, "return"  # type: ignore[arg-type]
+            destination_type=self.transfer_model_type,  # type: ignore[arg-type]
+            source_data=data,
+            field_definitions=self.parsed_field_definitions,
+            dto_for="return",
+            parsed_type=self.context.parsed_type,
         )
 
-    def create_openapi_schema(self, generate_examples: bool, schemas: dict[str, Schema]) -> Reference | Schema:
+    def create_openapi_schema(
+        self, generate_examples: bool, schemas: dict[str, Schema], prefer_alias: bool
+    ) -> Reference | Schema:
         """Create a RequestBody model for the given RouteHandler or return None."""
         field = SignatureField.create(self.annotation)
-        return create_schema(field=field, generate_examples=generate_examples, plugins=[], schemas=schemas)
+        return create_schema(
+            field=field, generate_examples=generate_examples, plugins=[], schemas=schemas, prefer_alias=prefer_alias
+        )
 
     def _create_transfer_type(
         self, parsed_type: ParsedType, exclude: AbstractSet[str], field_name: str, unique_name: str, nested_depth: int
     ) -> CompositeType | SimpleType:
         exclude = _filter_exclude(exclude, field_name)
 
         if parsed_type.is_union:
@@ -313,15 +350,15 @@
             if len(parsed_type.inner_types) == 2 and parsed_type.inner_types[1].annotation is Ellipsis:
                 return self._create_collection_type(parsed_type, exclude, unique_name, nested_depth)
             return self._create_tuple_type(parsed_type, exclude, unique_name, nested_depth)
 
         if parsed_type.is_mapping:
             return self._create_mapping_type(parsed_type, exclude, unique_name, nested_depth)
 
-        if parsed_type.is_collection:
+        if parsed_type.is_non_string_collection:
             return self._create_collection_type(parsed_type, exclude, unique_name, nested_depth)
 
         transfer_model: NestedFieldInfo | None = None
         if self.context.is_nested_field_predicate(parsed_type):
             if nested_depth == self.context.config.max_nested_depth:
                 raise NestedDepthExceededError()
 
@@ -332,37 +369,39 @@
             )
 
         return SimpleType(parsed_type, nested_field_info=transfer_model)
 
     def _create_collection_type(
         self, parsed_type: ParsedType, exclude: AbstractSet[str], unique_name: str, nested_depth: int
     ) -> CollectionType:
+        inner_types = parsed_type.inner_types
         inner_type = self._create_transfer_type(
-            parsed_type=parsed_type.inner_types[0],
+            parsed_type=ParsedType(Any) if not inner_types else inner_types[0],
             exclude=exclude,
             field_name="0",
             unique_name=_enumerate_name(unique_name, 0),
             nested_depth=nested_depth,
         )
         return CollectionType(
             parsed_type=parsed_type, inner_type=inner_type, has_nested=_determine_has_nested(inner_type)
         )
 
     def _create_mapping_type(
         self, parsed_type: ParsedType, exclude: AbstractSet[str], unique_name: str, nested_depth: int
     ) -> MappingType:
+        inner_types = parsed_type.inner_types
         key_type = self._create_transfer_type(
-            parsed_type=parsed_type.inner_types[0],
+            parsed_type=ParsedType(Any) if not inner_types else inner_types[0],
             exclude=exclude,
             field_name="0",
             unique_name=_enumerate_name(unique_name, 0),
             nested_depth=nested_depth,
         )
         value_type = self._create_transfer_type(
-            parsed_type=parsed_type.inner_types[1],
+            parsed_type=ParsedType(Any) if not inner_types else inner_types[1],
             exclude=exclude,
             field_name="1",
             unique_name=_enumerate_name(unique_name, 1),
             nested_depth=nested_depth,
         )
         return MappingType(
             parsed_type=parsed_type,
@@ -413,15 +452,15 @@
         # Generate a unique ID
         # Convert the ID to a short alphanumeric string
         return f"{unique_name}-{secrets.token_hex(8)}"
 
 
 def _filter_exclude(exclude: AbstractSet[str], field_name: str) -> AbstractSet[str]:
     """Filter exclude set to only include exclusions for the given field name."""
-    return {split[1] for s in exclude if (split := s.split(".", 1))[0] == field_name}
+    return {split[1] for s in exclude if (split := s.split(".", 1))[0] == field_name and len(split) > 1}
 
 
 def _enumerate_name(name: str, index: int) -> str:
     """Enumerate ``name`` with ``index``."""
     return f"{name}_{index}"
```

### Comparing `litestar-2.0.0a7/litestar/dto/factory/_backends/msgspec/backend.py` & `litestar-2.0.0b1/litestar/dto/factory/_backends/msgspec/backend.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/dto/factory/_backends/msgspec/utils.py` & `litestar-2.0.0b1/litestar/dto/factory/_backends/msgspec/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,55 +1,48 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, NewType, TypeVar
+from typing import TYPE_CHECKING, NewType, TypeVar, Union
 
-from msgspec import Struct, defstruct, field
+from msgspec import UNSET, Struct, UnsetType, defstruct, field
 
 from litestar.dto.factory._backends.utils import create_transfer_model_type_annotation
 from litestar.types import Empty
 
 if TYPE_CHECKING:
     from typing import Any
 
-    from litestar.dto.factory._backends.types import FieldDefinitionsType
-    from litestar.dto.factory.types import FieldDefinition
+    from litestar.dto.factory._backends.types import FieldDefinitionsType, TransferFieldDefinition
 
 
 MsgspecField = NewType("MsgspecField", type)
 StructT = TypeVar("StructT", bound=Struct)
 T = TypeVar("T")
 
 
-def _create_msgspec_field(field_definition: FieldDefinition) -> MsgspecField | None:
+def _create_msgspec_field(field_definition: TransferFieldDefinition) -> MsgspecField:
     kws: dict[str, Any] = {}
-    if field_definition.default is not Empty:
+    if field_definition.is_partial:
+        kws["default"] = UNSET
+
+    elif field_definition.default is not Empty:
         kws["default"] = field_definition.default
 
-    if field_definition.default_factory is not None:
+    elif field_definition.default_factory is not None:
         kws["default_factory"] = field_definition.default_factory
 
-    if not kws:
-        return None
-
     return field(**kws)  # type:ignore[no-any-return]
 
 
-def _create_struct_field_def(
-    name: str, type_: type[Any], field_: MsgspecField | None
-) -> tuple[str, type[Any]] | tuple[str, type[Any], MsgspecField]:
-    if field_ is None:
-        return name, type_
-    return name, type_, field_
-
-
 def _create_struct_for_field_definitions(model_name: str, field_definitions: FieldDefinitionsType) -> type[Struct]:
     struct_fields: list[tuple[str, type] | tuple[str, type, MsgspecField]] = []
     for field_def in field_definitions:
+        if field_def.is_excluded:
+            continue
+
         field_name = field_def.serialization_name or field_def.name
-        struct_fields.append(
-            _create_struct_field_def(
-                field_name,
-                create_transfer_model_type_annotation(field_def.transfer_type),
-                _create_msgspec_field(field_def),
-            )
-        )
+
+        field_type = create_transfer_model_type_annotation(field_def.transfer_type)
+        if field_def.is_partial:
+            field_type = Union[field_type, UnsetType]
+
+        struct_fields.append((field_name, field_type, _create_msgspec_field(field_def)))
     return defstruct(model_name, struct_fields, frozen=True, kw_only=True)
```

### Comparing `litestar-2.0.0a7/litestar/dto/factory/_backends/pydantic/backend.py` & `litestar-2.0.0b1/litestar/dto/factory/_backends/pydantic/backend.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/dto/factory/_backends/pydantic/utils.py` & `litestar-2.0.0b1/litestar/dto/factory/_backends/pydantic/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, TypeVar
+from typing import TYPE_CHECKING, TypeVar, Union
 
+from msgspec import UNSET, UnsetType
 from pydantic import BaseModel, create_model
 from pydantic.fields import FieldInfo
 
 from litestar.dto.factory._backends.utils import create_transfer_model_type_annotation
 from litestar.types import Empty
 
 if TYPE_CHECKING:
@@ -23,31 +24,38 @@
     class Config:
         arbitrary_types_allowed = True
         orm_mode = True
 
 
 def _create_field_info(field_definition: TransferFieldDefinition) -> FieldInfo:
     kws: dict[str, Any] = {}
-    if field_definition.default is not Empty:
+    if field_definition.is_partial:
+        kws["default"] = UNSET
+    elif field_definition.default is not Empty:
         kws["default"] = field_definition.default
     elif field_definition.default_factory is not Empty:
         kws["default_factory"] = field_definition.default_factory
     else:
         kws["default"] = ...
 
     return FieldInfo(**kws)
 
 
 def _create_model_for_field_definitions(model_name: str, field_definitions: FieldDefinitionsType) -> type[BaseModel]:
     model_fields: dict[str, tuple[type, FieldInfo]] = {}
     for field_def in field_definitions:
-        model_fields[field_def.serialization_name] = (
-            create_transfer_model_type_annotation(field_def.transfer_type),
-            _create_field_info(field_def),
-        )
+        if field_def.is_excluded:
+            continue
+
+        field_type = create_transfer_model_type_annotation(field_def.transfer_type)
+        if field_def.is_partial:
+            field_type = Union[field_type, UnsetType]
+
+        model_fields[field_def.serialization_name] = (field_type, _create_field_info(field_def))
+
     return create_model(
         model_name,
         __config__=None,
         __base__=_OrmModeBase,
         __module__=BaseModel.__module__,
         __validators__={},
         __cls_kwargs__={},
```

### Comparing `litestar-2.0.0a7/litestar/dto/factory/_backends/types.py` & `litestar-2.0.0b1/litestar/dto/factory/_backends/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
-from litestar.dto.factory.types import FieldDefinition
+from litestar.dto.factory.data_structures import FieldDefinition
 
 if TYPE_CHECKING:
     from typing import Any
 
     from typing_extensions import Self, TypeAlias
 
-    from litestar.utils.signature import ParsedType
+    from litestar.typing import ParsedType
 
 
 @dataclass(frozen=True)
 class NestedFieldInfo:
     """Type for representing fields and model type of nested model type."""
 
     __slots__ = ("model", "field_definitions")
@@ -88,38 +88,53 @@
     key_type: CompositeType | SimpleType
     value_type: CompositeType | SimpleType
 
 
 @dataclass(frozen=True)
 class TransferFieldDefinition(FieldDefinition):
     __slots__ = (
+        "default_factory",
+        "dto_field",
+        "dto_for",
+        "unique_model_name",
+        "is_excluded",
         "is_partial",
         "serialization_name",
         "transfer_type",
+        "unique_name",
     )
 
     transfer_type: TransferType
     """Type of the field for transfer."""
     serialization_name: str
     """Name of the field as it should feature on the transfer model."""
     is_partial: bool
     """Whether the field is optional for transfer."""
+    is_excluded: bool
+    """Whether the field should be excluded from transfer."""
 
     @classmethod
     def from_field_definition(
-        cls, field_definition: FieldDefinition, transfer_type: TransferType, serialization_name: str, is_partial: bool
+        cls,
+        field_definition: FieldDefinition,
+        transfer_type: TransferType,
+        serialization_name: str,
+        is_partial: bool,
+        is_excluded: bool,
     ) -> Self:
         return cls(
             name=field_definition.name,
             default=field_definition.default,
             parsed_type=field_definition.parsed_type,
             default_factory=field_definition.default_factory,
             serialization_name=serialization_name,
             unique_model_name=field_definition.unique_model_name,
             transfer_type=transfer_type,
             dto_field=field_definition.dto_field,
             is_partial=is_partial,
+            is_excluded=is_excluded,
+            dto_for=field_definition.dto_for,
         )
 
 
 FieldDefinitionsType: TypeAlias = "tuple[TransferFieldDefinition, ...]"
 """Generic representation of names and types."""
```

### Comparing `litestar-2.0.0a7/litestar/dto/factory/abc.py` & `litestar-2.0.0b1/litestar/dto/factory/abc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
 from typing import TYPE_CHECKING, Generic, TypeVar
 
 from litestar.dto.interface import ConnectionContext, DTOInterface
 from litestar.enums import RequestEncodingType
-from litestar.utils.signature import ParsedType
+from litestar.typing import ParsedType
 
 from ._backends import MsgspecDTOBackend, PydanticDTOBackend
 from ._backends.abc import BackendContext
 from .config import DTOConfig
-from .data_structures import DTOData
 from .exc import InvalidAnnotation
-from .utils import parse_configs_from_annotation
+from .utils import (
+    parse_configs_from_annotation,
+    resolve_generic_wrapper_type,
+    resolve_model_type,
+)
 
 if TYPE_CHECKING:
     from typing import Any, ClassVar, Collection, Generator
 
     from typing_extensions import Self
 
     from litestar.dto.interface import HandlerContext
     from litestar.dto.types import ForType
     from litestar.openapi.spec import Reference, Schema
     from litestar.types.serialization import LitestarEncodableType
 
     from ._backends import AbstractDTOBackend
-    from .types import FieldDefinition
+    from .data_structures import FieldDefinition
 
-__all__ = ["AbstractDTOFactory"]
+__all__ = ("AbstractDTOFactory",)
 
-DataT = TypeVar("DataT")
+T = TypeVar("T")
 
 
-class AbstractDTOFactory(DTOInterface, Generic[DataT], metaclass=ABCMeta):
+class AbstractDTOFactory(DTOInterface, Generic[T], metaclass=ABCMeta):
     """Base class for DTO types."""
 
     __slots__ = ("connection_context",)
 
     config: ClassVar[DTOConfig]
     """Config objects to define properties of the DTO."""
     model_type: ClassVar[type[Any]]
@@ -94,15 +97,15 @@
         return backend.populate_data_from_builtins(builtins, self.connection_context)
 
     def bytes_to_data_type(self, raw: bytes) -> Any:
         """Return the data held by the DTO."""
         backend = self._get_backend("data", self.connection_context.handler_id)
         return backend.populate_data_from_raw(raw, self.connection_context)
 
-    def data_to_encodable_type(self, data: DataT | Collection[DataT]) -> LitestarEncodableType:
+    def data_to_encodable_type(self, data: T | Collection[T]) -> LitestarEncodableType:
         backend = self._get_backend("return", self.connection_context.handler_id)
         return backend.encode_data(data, self.connection_context)
 
     @classmethod
     @abstractmethod
     def generate_field_definitions(cls, model_type: type[Any]) -> Generator[FieldDefinition, None, None]:
         """Generate ``FieldDefinition`` instances from ``model_type``.
@@ -127,67 +130,60 @@
     def on_registration(cls, handler_context: HandlerContext) -> None:
         """Called each time the DTO type is encountered during signature modelling.
 
         Args:
             handler_context: A :class:`HandlerContext <.HandlerContext>` instance. Provides information about the
                 handler and application of the DTO.
         """
-        if handler_context.parsed_type.is_subclass_of(DTOData):
-            parsed_type = handler_context.parsed_type.annotation.parsed_type
-        else:
-            parsed_type = handler_context.parsed_type
-
-        if parsed_type.is_collection:
-            if len(parsed_type.inner_types) != 1:
-                raise InvalidAnnotation("AbstractDTOFactory only supports homogeneous collection types")
-            handler_type = parsed_type.inner_types[0]
-        else:
-            handler_type = parsed_type
-
-        if not handler_type.is_subclass_of(cls.model_type):
-            raise InvalidAnnotation(
-                f"DTO narrowed with '{cls.model_type}', handler type is '{handler_context.parsed_type.annotation}'"
-            )
+        parsed_type = handler_context.parsed_type
+        model_type = resolve_model_type(parsed_type)
+        wrapper_attribute_name: str | None = None
+
+        if not model_type.is_subclass_of(cls.model_type):
+            resolved_generic_result = resolve_generic_wrapper_type(model_type, cls.model_type)
+            if resolved_generic_result is not None:
+                model_type, parsed_type, wrapper_attribute_name = resolved_generic_result
+            else:
+                raise InvalidAnnotation(
+                    f"DTO narrowed with '{cls.model_type}', handler type is '{parsed_type.annotation}'"
+                )
 
-        key = (handler_context.dto_for, handler_context.parsed_type, handler_context.request_encoding_type)
+        key = (handler_context.dto_for, parsed_type, handler_context.request_encoding_type)
         backend = cls._type_backend_map.get(key)
         if backend is None:
             backend_type: type[AbstractDTOBackend]
             if handler_context.request_encoding_type in {
                 RequestEncodingType.URL_ENCODED,
                 RequestEncodingType.MULTI_PART,
             }:
                 backend_type = PydanticDTOBackend
             else:
                 backend_type = MsgspecDTOBackend
 
             backend_context = BackendContext(
-                cls.config,
-                handler_context.dto_for,
-                handler_context.parsed_type,
-                cls.generate_field_definitions,
-                cls.detect_nested_field,
-                handler_type.annotation,
+                dto_config=cls.config,
+                dto_for=handler_context.dto_for,
+                parsed_type=parsed_type,
+                field_definition_generator=cls.generate_field_definitions,
+                is_nested_field_predicate=cls.detect_nested_field,
+                model_type=model_type.annotation,
+                wrapper_attribute_name=wrapper_attribute_name,
             )
             backend = cls._type_backend_map.setdefault(key, backend_type(backend_context))
         cls._handler_backend_map[(handler_context.dto_for, handler_context.handler_id)] = backend
 
     @classmethod
     def create_openapi_schema(
-        cls,
-        dto_for: ForType,
-        handler_id: str,
-        generate_examples: bool,
-        schemas: dict[str, Schema],
+        cls, dto_for: ForType, handler_id: str, generate_examples: bool, schemas: dict[str, Schema], prefer_alias: bool
     ) -> Reference | Schema:
         """Create an OpenAPI request body.
 
         Returns:
             OpenAPI request body.
         """
         backend = cls._get_backend(dto_for, handler_id)
-        return backend.create_openapi_schema(generate_examples, schemas)
+        return backend.create_openapi_schema(generate_examples, schemas, prefer_alias)
 
     @classmethod
     def _get_backend(cls, dto_for: ForType, handler_id: str) -> AbstractDTOBackend:
         """Return the backend for the handler/dto_for combo."""
         return cls._handler_backend_map[(dto_for, handler_id)]
```

### Comparing `litestar-2.0.0a7/litestar/dto/factory/config.py` & `litestar-2.0.0b1/litestar/dto/factory/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,7 +34,9 @@
     return a string.
 
     Fields defined in ``rename_fields`` are ignored."""
     max_nested_depth: int = 1
     """The maximum depth of nested items allowed for data transfer."""
     partial: bool = False
     """Allow transfer of partial data."""
+    underscore_fields_private: bool = True
+    """Fields starting with an underscore are considered private and excluded from data transfer."""
```

### Comparing `litestar-2.0.0a7/litestar/dto/factory/field.py` & `litestar-2.0.0b1/litestar/dto/factory/field.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,23 +16,25 @@
 
 
 class Mark(str, Enum):
     """For marking field definitions on domain models."""
 
     READ_ONLY = "read-only"
     """To mark a field that can be read, but not updated by clients."""
+    WRITE_ONLY = "write-only"
+    """To mark a field that can be written to, but not read by clients."""
     PRIVATE = "private"
     """To mark a field that can neither be read or updated by clients."""
 
 
 @dataclass
 class DTOField:
     """For configuring DTO behavior on model fields."""
 
-    mark: Mark | Literal["read-only", "private"] | None = None
+    mark: Mark | Literal["read-only", "write-only", "private"] | None = None
     """Mark the field as read-only, or private."""
 
 
 def dto_field(mark: Literal["read-only", "private"] | Mark) -> dict[str, DTOField]:
     """Create a field metadata mapping.
 
     Args:
```

### Comparing `litestar-2.0.0a7/litestar/dto/factory/stdlib/dataclass.py` & `litestar-2.0.0b1/litestar/dto/factory/stdlib/dataclass.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 from __future__ import annotations
 
 from dataclasses import MISSING, fields
 from typing import TYPE_CHECKING, Generic, TypeVar
 
 from litestar.dto.factory.abc import AbstractDTOFactory
-from litestar.dto.factory.field import DTO_FIELD_META_KEY
-from litestar.dto.factory.types import FieldDefinition
+from litestar.dto.factory.data_structures import FieldDefinition
+from litestar.dto.factory.field import DTO_FIELD_META_KEY, DTOField
 from litestar.dto.factory.utils import get_model_type_hints
 from litestar.types.empty import Empty
 from litestar.utils.helpers import get_fully_qualified_class_name
 
 if TYPE_CHECKING:
     from typing import ClassVar, Collection, Generator
 
     from litestar.types.protocols import DataclassProtocol
-    from litestar.utils.signature import ParsedType
+    from litestar.typing import ParsedType
 
+__all__ = ("DataclassDTO", "T")
 
-__all__ = ("DataclassDTO", "DataT")
-
-DataT = TypeVar("DataT", bound="DataclassProtocol | Collection[DataclassProtocol]")
+T = TypeVar("T", bound="DataclassProtocol | Collection[DataclassProtocol]")
 AnyDataclass = TypeVar("AnyDataclass", bound="DataclassProtocol")
 
 
-class DataclassDTO(AbstractDTOFactory[DataT], Generic[DataT]):
+class DataclassDTO(AbstractDTOFactory[T], Generic[T]):
     """Support for domain modelling with dataclasses."""
 
     __slots__ = ()
 
     model_type: ClassVar[type[DataclassProtocol]]
 
     @classmethod
@@ -42,16 +41,17 @@
             default_factory = dc_field.default_factory if dc_field.default_factory is not MISSING else None
 
             field_def = FieldDefinition(
                 name=key,
                 parsed_type=parsed_type,
                 default=default,
                 default_factory=default_factory,
-                dto_field=dc_field.metadata.get(DTO_FIELD_META_KEY),
+                dto_field=dc_field.metadata.get(DTO_FIELD_META_KEY, DTOField()),
                 unique_model_name=get_fully_qualified_class_name(model_type),
+                dto_for=None,
             )
 
             yield field_def
 
     @classmethod
     def detect_nested_field(cls, parsed_type: ParsedType) -> bool:
         return hasattr(parsed_type.annotation, "__dataclass_fields__")
```

### Comparing `litestar-2.0.0a7/litestar/dto/interface.py` & `litestar-2.0.0b1/litestar/dto/interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from typing import Any, Final
 
     from typing_extensions import Self
 
     from litestar.openapi.spec import Reference
     from litestar.types import LitestarEncodableType
     from litestar.types.internal_types import AnyConnection
-    from litestar.utils.signature import ParsedType
+    from litestar.typing import ParsedType
 
     from .types import ForType
 
 __all__ = (
     "ConnectionContext",
     "DTOInterface",
     "HandlerContext",
@@ -110,14 +110,15 @@
     @classmethod
     def create_openapi_schema(
         cls,
         dto_for: ForType,
         handler_id: str,
         generate_examples: bool,
         schemas: dict[str, Schema],
+        prefer_alias: bool,
     ) -> Reference | Schema:
         """Create an OpenAPI request body for the DTO.
 
         Returns:
             An optional :class:`RequestBody <.openapi.spec.request_body.RequestBody>` instance.
         """
         return Schema()
```

### Comparing `litestar-2.0.0a7/litestar/enums.py` & `litestar-2.0.0b1/litestar/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/events/emitter.py` & `litestar-2.0.0b1/litestar/events/emitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import math
 import sys
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from contextlib import AsyncExitStack
-from typing import TYPE_CHECKING, Any, DefaultDict, Sequence
+from typing import TYPE_CHECKING, Any, Sequence
 
 if sys.version_info < (3, 9):
     from typing import AsyncContextManager
 else:
     from contextlib import AbstractAsyncContextManager as AsyncContextManager
 
 import anyio
@@ -28,15 +28,15 @@
 
 
 class BaseEventEmitterBackend(AsyncContextManager["BaseEventEmitterBackend"], ABC):
     """Abstract class used to define event emitter backends."""
 
     __slots__ = ("listeners",)
 
-    listeners: DefaultDict[str, set[EventListener]]
+    listeners: defaultdict[str, set[EventListener]]
 
     def __init__(self, listeners: Sequence[EventListener]):
         """Create an event emitter instance.
 
         Args:
             listeners: A list of listeners.
         """
```

### Comparing `litestar-2.0.0a7/litestar/events/listener.py` & `litestar-2.0.0b1/litestar/events/listener.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/exceptions/__init__.py` & `litestar-2.0.0b1/litestar/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/exceptions/base_exceptions.py` & `litestar-2.0.0b1/litestar/exceptions/base_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/exceptions/http_exceptions.py` & `litestar-2.0.0b1/litestar/exceptions/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/exceptions/websocket_exceptions.py` & `litestar-2.0.0b1/litestar/exceptions/websocket_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/file_system.py` & `litestar-2.0.0b1/litestar/file_system.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import TYPE_CHECKING, Any, AnyStr, cast
 
 from anyio import AsyncFile, Path, open_file
 from anyio.to_thread import run_sync
 
 from litestar.exceptions import InternalServerException, NotAuthorizedException
 from litestar.types.file_types import FileSystemProtocol
-from litestar.utils.sync import is_async_callable
+from litestar.utils.predicates import is_async_callable
 
 __all__ = ("BaseLocalFileSystem", "FileSystemAdapter")
 
 
 if TYPE_CHECKING:
     from os import stat_result
```

### Comparing `litestar-2.0.0a7/litestar/handlers/__init__.py` & `litestar-2.0.0b1/litestar/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/handlers/asgi_handlers.py` & `litestar-2.0.0b1/litestar/handlers/asgi_handlers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Mapping, Sequence
 
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.handlers.base import BaseRouteHandler
 from litestar.types.builtin_types import NoneType
-from litestar.utils import is_async_callable
+from litestar.utils.predicates import is_async_callable
 
 __all__ = ("ASGIRouteHandler", "asgi")
 
 
 if TYPE_CHECKING:
     from litestar.types import (
         ExceptionHandlersMap,
         Guard,
         MaybePartial,  # noqa: F401
     )
 
 
-class ASGIRouteHandler(BaseRouteHandler["ASGIRouteHandler"]):
+class ASGIRouteHandler(BaseRouteHandler):
     """ASGI Route Handler decorator.
 
     Use this decorator to decorate ASGI applications.
     """
 
     __slots__ = ("is_mount", "is_static")
```

### Comparing `litestar-2.0.0a7/litestar/handlers/base.py` & `litestar-2.0.0b1/litestar/handlers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
 from copy import copy
 from functools import partial
-from typing import TYPE_CHECKING, Any, Generic, Mapping, Sequence, TypeVar, cast
+from typing import TYPE_CHECKING, Any, Mapping, Sequence, cast
 
 from litestar._signature import create_signature_model
 from litestar._signature.field import SignatureField
 from litestar.di import Provide
 from litestar.dto.interface import HandlerContext
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.types import Dependencies, Empty, ExceptionHandlersMap, Guard, Middleware, TypeEncodersMap
-from litestar.utils import AsyncCallable, Ref, async_partial, get_name, is_async_callable, normalize_path
+from litestar.utils import AsyncCallable, Ref, async_partial, get_name, normalize_path
 from litestar.utils.helpers import unwrap_partial
+from litestar.utils.predicates import is_async_callable
 from litestar.utils.signature import ParsedSignature, infer_request_encoding_from_parameter
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
     from litestar import Litestar
     from litestar._signature.models import SignatureModel
@@ -27,18 +28,16 @@
     from litestar.router import Router
     from litestar.types import AnyCallable, AsyncAnyCallable, ExceptionHandler
     from litestar.types.composite_types import MaybePartial
     from litestar.types.empty import EmptyType
 
 __all__ = ("BaseRouteHandler",)
 
-T = TypeVar("T", bound="BaseRouteHandler")
 
-
-class BaseRouteHandler(Generic[T]):
+class BaseRouteHandler:
     """Base route handler.
 
     Serves as a subclass for all route handlers
     """
 
     __slots__ = (
         "_fn",
@@ -181,15 +180,15 @@
     @property
     def dependency_name_set(self) -> set[str]:
         """Set of all dependency names provided in the handler's ownership layers."""
         layered_dependencies = (layer.dependencies or {} for layer in self.ownership_layers)
         return {name for layer in layered_dependencies for name in layer}  # pyright: ignore
 
     @property
-    def ownership_layers(self) -> list[T | Controller | Router]:
+    def ownership_layers(self) -> list[Self | Controller | Router]:
         """Return the handler layers from the app down to the route handler.
 
         ``app -> ... -> route handler``
         """
         layers = []
 
         cur: Any = self
@@ -423,29 +422,31 @@
 
     def _create_signature_model(self, app: Litestar) -> None:
         """Create signature model for handler function."""
         if not self.signature_model:
             self.signature_model = create_signature_model(
                 dependency_name_set=self.dependency_name_set,
                 fn=cast("AnyCallable", self.fn.value),
-                preferred_validation_backend=app.preferred_validation_backend,
+                preferred_validation_backend=app._preferred_validation_backend,
                 parsed_signature=self.parsed_fn_signature,
+                has_data_dto=bool(self.resolve_dto()),
             )
 
     def _create_provider_signature_models(self, app: Litestar) -> None:
         """Create signature models for dependency providers."""
         for provider in self.resolve_dependencies().values():
             if not getattr(provider, "signature_model", None):
                 provider.signature_model = create_signature_model(
                     dependency_name_set=self.dependency_name_set,
                     fn=provider.dependency.value,
-                    preferred_validation_backend=app.preferred_validation_backend,
+                    preferred_validation_backend=app._preferred_validation_backend,
                     parsed_signature=ParsedSignature.from_fn(
                         unwrap_partial(provider.dependency.value), self.resolve_signature_namespace()
                     ),
+                    has_data_dto=bool(self.resolve_dto()),
                 )
 
     def _handle_serialization_plugins(self, plugins: list[SerializationPluginProtocol]) -> None:
         """Handle the serialization plugins for the handler."""
         # must do the return dto first, otherwise it will resolve to the same as the data dto
         if self.resolve_return_dto() is None:
             return_type = self.parsed_fn_signature.return_type
```

### Comparing `litestar-2.0.0a7/litestar/handlers/http_handlers/_utils.py` & `litestar-2.0.0b1/litestar/handlers/http_handlers/_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 from __future__ import annotations
 
 from functools import lru_cache
 from inspect import isawaitable
 from typing import TYPE_CHECKING, Any, Sequence, cast
 
-from litestar.dto.interface import ConnectionContext
 from litestar.enums import HttpMethod
 from litestar.exceptions import ValidationException
 from litestar.status_codes import HTTP_200_OK, HTTP_201_CREATED, HTTP_204_NO_CONTENT
+from litestar.utils import encode_headers
 
 if TYPE_CHECKING:
     from litestar.app import Litestar
     from litestar.background_tasks import BackgroundTask, BackgroundTasks
     from litestar.connection import Request
     from litestar.datastructures import Cookie, ResponseHeader
-    from litestar.dto.interface import DTOInterface
     from litestar.response import Response
-    from litestar.response_containers import ResponseContainer
     from litestar.types import (
         AfterRequestHookHandler,
         ASGIApp,
         AsyncAnyCallable,
         Method,
         ResponseType,
         TypeEncodersMap,
     )
 
 __all__ = (
     "create_data_handler",
     "create_generic_asgi_response_handler",
-    "create_response_container_handler",
     "create_response_handler",
-    "filter_cookies",
     "get_default_status_code",
     "normalize_headers",
     "normalize_http_method",
 )
 
 
 def create_data_handler(
@@ -60,66 +56,41 @@
         status_code: The response status code.
         type_encoders: A mapping of types to encoder functions.
 
     Returns:
         A handler function.
 
     """
-    normalized_headers = [
-        (name.lower().encode("latin-1"), value.encode("latin-1")) for name, value in normalize_headers(headers).items()
-    ]
-    cookie_headers = [cookie.to_encoded_header() for cookie in cookies if not cookie.documentation_only]
-    raw_headers = [*normalized_headers, *cookie_headers]
+    raw_headers = encode_headers(normalize_headers(headers).items(), cookies, [])
+
+    async def handler(
+        data: Any,
+        request: Request[Any, Any, Any],
+        app: Litestar,
+        **kwargs: Any,
+    ) -> ASGIApp:
+        if isawaitable(data):
+            data = await data
 
-    async def create_response(data: Any) -> ASGIApp:
         response = response_class(
             background=background,
             content=data,
             media_type=media_type,
             status_code=status_code,
             type_encoders=type_encoders,
         )
-        response.raw_headers = raw_headers
 
         if after_request:
-            return await after_request(response)  # type: ignore
+            response = await after_request(response)  # type: ignore[arg-type,misc]
 
-        return response
-
-    async def handler(
-        data: Any,
-        return_dto: type[DTOInterface] | None,
-        request: Request[Any, Any, Any],
-        **kwargs: Any,
-    ) -> ASGIApp:
-        if isawaitable(data):
-            data = await data
-
-        if return_dto:
-            ctx = ConnectionContext.from_connection(request)
-            data = return_dto(ctx).data_to_encodable_type(data)
-
-        return await create_response(data=data)
+        return response.to_asgi_response(app=app, request=request, encoded_headers=raw_headers)
 
     return handler
 
 
-def filter_cookies(local_cookies: frozenset[Cookie], layered_cookies: frozenset[Cookie]) -> list[Cookie]:
-    """Given two sets of cookies, return a unique list of cookies, that are not marked as documentation_only.
-
-    Args:
-        local_cookies: Cookies returned from the local scope.
-        layered_cookies: Cookies returned from the layers.
-
-    Returns:
-        A unified list of cookies
-    """
-    return [cookie for cookie in {*local_cookies, *layered_cookies} if not cookie.documentation_only]
-
-
 def create_generic_asgi_response_handler(
     after_request: AfterRequestHookHandler | None,
     cookies: frozenset[Cookie],
 ) -> AsyncAnyCallable:
     """Create a handler function for Responses.
 
     Args:
@@ -153,66 +124,55 @@
         header.name: cast("str", header.value)  # we know value to be a string at this point because we validate it
         # that it's not None when initializing a header with documentation_only=True
         for header in headers
         if not header.documentation_only
     }
 
 
-def create_response_container_handler(
+def create_response_handler(
     after_request: AfterRequestHookHandler | None,
+    background: BackgroundTask | BackgroundTasks | None,
     cookies: frozenset[Cookie],
     headers: frozenset[ResponseHeader],
     media_type: str,
     status_code: int,
+    type_encoders: TypeEncodersMap | None,
 ) -> AsyncAnyCallable:
-    """Create a handler function for ResponseContainers.
+    """Create a handler function for Litestar Responses.
 
     Args:
         after_request: An after request handler.
+        background: A background task or background tasks.
         cookies: A set of pre-defined cookies.
         headers: A set of response headers.
         media_type: The response media type.
         status_code: The response status code.
+        type_encoders: A mapping of types to encoder functions.
 
     Returns:
         A handler function.
     """
+
     normalized_headers = normalize_headers(headers)
+    cookie_list = list(cookies)
 
-    async def handler(data: ResponseContainer, app: Litestar, request: Request, **kwargs: Any) -> ASGIApp:
-        response = data.to_response(
+    async def handler(
+        data: Response, app: Litestar, request: Request, **kwargs: Any  # kwargs is for return dto
+    ) -> ASGIApp:
+        response = await after_request(data) if after_request else data  # type:ignore[arg-type,misc]
+        return response.to_asgi_response(  # type: ignore
             app=app,
-            headers={**normalized_headers, **data.headers},
-            status_code=status_code,
-            media_type=data.media_type or media_type,
+            background=background,
+            cookies=cookie_list,
+            headers=normalized_headers,
+            media_type=media_type,
             request=request,
+            status_code=status_code,
+            type_encoders=type_encoders,
         )
-        response.cookies = filter_cookies(frozenset(data.cookies), cookies)
-        return await after_request(response) if after_request else response  # type: ignore
-
-    return handler
-
-
-def create_response_handler(
-    after_request: AfterRequestHookHandler | None,
-    cookies: frozenset[Cookie],
-) -> AsyncAnyCallable:
-    """Create a handler function for Litestar Responses.
-
-    Args:
-        after_request: An after request handler.
-        cookies: A set of pre-defined cookies.
-
-    Returns:
-        A handler function.
-    """
-
-    async def handler(data: Response, **kwargs: Any) -> ASGIApp:
-        data.cookies = filter_cookies(frozenset(data.cookies), cookies)
-        return await after_request(data) if after_request else data  # type: ignore
 
     return handler
 
 
 def normalize_http_method(http_methods: HttpMethod | Method | Sequence[HttpMethod | Method]) -> set[Method]:
     """Normalize HTTP method(s) into a set of upper-case method names.
```

### Comparing `litestar-2.0.0a7/litestar/handlers/http_handlers/base.py` & `litestar-2.0.0b1/litestar/handlers/http_handlers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from __future__ import annotations
 
 from enum import Enum
-from typing import TYPE_CHECKING, AnyStr, Mapping, cast
-
-from typing_extensions import TypedDict
+from typing import TYPE_CHECKING, AnyStr, Mapping, TypedDict, cast
 
 from litestar._layers.utils import narrow_response_cookies, narrow_response_headers
 from litestar.datastructures.cookie import Cookie
 from litestar.datastructures.response_header import ResponseHeader
+from litestar.dto.interface import ConnectionContext
 from litestar.enums import HttpMethod, MediaType
 from litestar.exceptions import (
     HTTPException,
     ImproperlyConfiguredException,
 )
 from litestar.handlers.base import BaseRouteHandler
 from litestar.handlers.http_handlers._utils import (
     create_data_handler,
     create_generic_asgi_response_handler,
-    create_response_container_handler,
     create_response_handler,
     get_default_status_code,
     normalize_http_method,
 )
-from litestar.response import FileResponse, Response
-from litestar.response_containers import File, Redirect, ResponseContainer
+from litestar.openapi.spec import Operation
+from litestar.response import Response
 from litestar.status_codes import HTTP_204_NO_CONTENT, HTTP_304_NOT_MODIFIED
 from litestar.types import (
     AfterRequestHookHandler,
     AfterResponseHookHandler,
     AnyCallable,
     ASGIApp,
     BeforeRequestHookHandler,
@@ -41,15 +39,16 @@
     Middleware,
     ResponseCookies,
     ResponseHeaders,
     ResponseType,
     TypeEncodersMap,
 )
 from litestar.types.builtin_types import NoneType
-from litestar.utils import AsyncCallable, async_partial, is_async_callable
+from litestar.utils import AsyncCallable, async_partial
+from litestar.utils.predicates import is_async_callable
 from litestar.utils.warnings import warn_implicit_sync_to_thread, warn_sync_to_thread_with_async_callable
 
 if TYPE_CHECKING:
     from typing import Any, Awaitable, Callable, Sequence
 
     from litestar.app import Litestar
     from litestar.background_tasks import BackgroundTask, BackgroundTasks
@@ -67,15 +66,15 @@
 
 
 class ResponseHandlerMap(TypedDict):
     default_handler: Callable[[Any], Awaitable[ASGIApp]] | EmptyType
     response_type_handler: Callable[[Any], Awaitable[ASGIApp]] | EmptyType
 
 
-class HTTPRouteHandler(BaseRouteHandler["HTTPRouteHandler"]):
+class HTTPRouteHandler(BaseRouteHandler):
     """HTTP Route Decorator.
 
     Use this decorator to decorate an HTTP handler with multiple methods.
     """
 
     __slots__ = (
         "_resolved_after_response",
@@ -93,14 +92,15 @@
         "deprecated",
         "description",
         "etag",
         "has_sync_callable",
         "http_methods",
         "include_in_schema",
         "media_type",
+        "operation_class",
         "operation_id",
         "raises",
         "response_class",
         "response_cookies",
         "response_description",
         "response_headers",
         "responses",
@@ -143,14 +143,15 @@
         sync_to_thread: bool | None = None,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
         include_in_schema: bool = True,
+        operation_class: type[Operation] = Operation,
         operation_id: str | None = None,
         raises: Sequence[type[HTTPException]] | None = None,
         response_description: str | None = None,
         responses: Mapping[int, ResponseSpec] | None = None,
         signature_namespace: Mapping[str, Any] | None = None,
         security: Sequence[SecurityRequirement] | None = None,
         summary: str | None = None,
@@ -211,14 +212,15 @@
             sync_to_thread: A boolean dictating whether the handler function will be executed in a worker thread or the
                 main event loop. This has an effect only for sync handler functions. See using sync handler functions.
             content_encoding: A string describing the encoding of the content, e.g. ``"base64"``.
             content_media_type: A string designating the media-type of the content, e.g. ``"image/png"``.
             deprecated:  A boolean dictating whether this route should be marked as deprecated in the OpenAPI schema.
             description: Text used for the route's schema description section.
             include_in_schema: A boolean flag dictating whether  the route handler should be documented in the OpenAPI schema.
+            operation_class: :class:`Operation <.openapi.spec.operation.Operation>` to be used with the route's OpenAPI schema.
             operation_id: An identifier used for the route's schema operationId. Defaults to the ``__name__`` of the wrapped function.
             raises:  A list of exception classes extending from litestar.HttpException that is used for the OpenAPI documentation.
                 This list should describe all exceptions raised within the route handler's function/method. The Litestar
                 ValidationException will be added automatically for the schema if any validation is involved.
             response_description: Text used for the route's response schema description section.
             security: A sequence of dictionaries that contain information about which security scheme can be used on the endpoint.
             summary: Text used for the route's schema summary section.
@@ -263,14 +265,15 @@
         self.sync_to_thread = sync_to_thread
         # OpenAPI related attributes
         self.content_encoding = content_encoding
         self.content_media_type = content_media_type
         self.deprecated = deprecated
         self.description = description
         self.include_in_schema = include_in_schema
+        self.operation_class = operation_class
         self.operation_id = operation_id
         self.raises = raises
         self.response_description = response_description
         self.summary = summary
         self.tags = tags
         self.security = security
         self.responses = responses
@@ -413,33 +416,30 @@
             return_type = self.parsed_fn_signature.return_type
             return_annotation = return_type.annotation
 
             if before_request_handler := self.resolve_before_request():
                 handler_return_type = before_request_handler.parsed_signature.return_type
                 if not handler_return_type.is_subclass_of((Empty, NoneType)):
                     return_annotation = handler_return_type.annotation
-            self._response_handler_mapping["response_type_handler"] = create_response_handler(
-                cookies=cookies, after_request=after_request
+
+            self._response_handler_mapping["response_type_handler"] = response_type_handler = create_response_handler(
+                after_request=after_request,
+                background=self.background,
+                cookies=cookies,
+                headers=headers,
+                media_type=media_type,
+                status_code=self.status_code,
+                type_encoders=type_encoders,
             )
 
             if return_type.is_subclass_of(Response):
-                self._response_handler_mapping["default_handler"] = self._response_handler_mapping[
-                    "response_type_handler"
-                ]
-            elif return_type.is_subclass_of(ResponseContainer):
-                self._response_handler_mapping["default_handler"] = create_response_container_handler(
-                    after_request=after_request,
-                    cookies=cookies,
-                    headers=headers,
-                    media_type=media_type,
-                    status_code=self.status_code,
-                )
+                self._response_handler_mapping["default_handler"] = response_type_handler
             elif is_async_callable(return_annotation) or return_annotation is ASGIApp:
                 self._response_handler_mapping["default_handler"] = create_generic_asgi_response_handler(
-                    cookies=cookies, after_request=after_request
+                    after_request=after_request, cookies=cookies
                 )
             else:
                 self._response_handler_mapping["default_handler"] = create_data_handler(
                     after_request=after_request,
                     background=self.background,
                     cookies=cookies,
                     headers=headers,
@@ -457,28 +457,33 @@
         )
 
     async def to_response(self, app: Litestar, data: Any, request: Request) -> ASGIApp:
         """Return a :class:`Response <.response.Response>` from the handler by resolving and calling it.
 
         Args:
             app: The :class:`Litestar <litestar.app.Litestar>` app instance
-            data: Either an instance of a :class:`ResponseContainer <.response_containers.ResponseContainer>`,
+            data: Either an instance of a :class:`Response <.response.Response>`,
                 a Response instance or an arbitrary value.
             request: A :class:`Request <.connection.Request>` instance
 
         Returns:
             A Response instance
         """
+        if return_dto_type := self.resolve_return_dto():
+            ctx = ConnectionContext.from_connection(request)
+            data = return_dto_type(ctx).data_to_encodable_type(data)
+
         response_handler = self.get_response_handler(is_response_type_data=isinstance(data, Response))
-        return await response_handler(app=app, data=data, request=request, return_dto=self.resolve_return_dto())  # type: ignore
+        return await response_handler(app=app, data=data, request=request)  # type: ignore
 
     def on_registration(self, app: Litestar) -> None:
-        super().on_registration(app)
         if before_request := self.resolve_before_request():
             before_request.set_parsed_signature(self.resolve_signature_namespace())
+
+        super().on_registration(app)
         self.resolve_after_response()
 
     def _validate_handler_function(self) -> None:
         """Validate the route handler function once it is set by inspecting its return annotations."""
         super()._validate_handler_function()
 
         return_type = self.parsed_fn_signature.return_type
@@ -493,20 +498,25 @@
             self.status_code < 200 or self.status_code in {HTTP_204_NO_CONTENT, HTTP_304_NOT_MODIFIED}
         ) and not return_type.is_subclass_of(NoneType):
             raise ImproperlyConfiguredException(
                 "A status code 204, 304 or in the range below 200 does not support a response body."
                 "If the function should return a value, change the route handler status code to an appropriate value.",
             )
 
+        if (
+            (before_request := self.resolve_before_request())
+            and not before_request.parsed_signature.return_type.is_subclass_of(NoneType)
+            and not before_request.parsed_signature.return_type.is_optional
+        ):
+            return_type = before_request.parsed_signature.return_type
+
         if not self.media_type:
-            if return_type.annotation is AnyStr or return_type.is_subclass_of(
-                (str, bytes, Redirect, File, FileResponse)
-            ):
+            if return_type.is_subclass_of((str, bytes)) or return_type.annotation is AnyStr:
                 self.media_type = MediaType.TEXT
-            else:
+            elif not return_type.is_subclass_of(Response):
                 self.media_type = MediaType.JSON
 
         if "socket" in self.parsed_fn_signature.parameters:
             raise ImproperlyConfiguredException("The 'socket' kwarg is not supported with http handlers")
 
         if "data" in self.parsed_fn_signature.parameters and "GET" in self.http_methods:
             raise ImproperlyConfiguredException("'data' kwarg is unsupported for 'GET' request handlers")
```

### Comparing `litestar-2.0.0a7/litestar/handlers/http_handlers/decorators.py` & `litestar-2.0.0b1/litestar/handlers/http_handlers/decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from litestar.enums import HttpMethod, MediaType
 from litestar.exceptions import HTTPException, ImproperlyConfiguredException
-from litestar.response import FileResponse
-from litestar.response_containers import File
+from litestar.openapi.spec import Operation
+from litestar.response.file import ASGIFileResponse, File
 from litestar.types.builtin_types import NoneType
 from litestar.types.empty import Empty
 from litestar.utils import is_class_and_subclass
 
 from .base import HTTPRouteHandler
 
 if TYPE_CHECKING:
@@ -78,14 +78,15 @@
         sync_to_thread: bool | None = None,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
         include_in_schema: bool = True,
+        operation_class: type[Operation] = Operation,
         operation_id: str | None = None,
         raises: list[type[HTTPException]] | None = None,
         response_description: str | None = None,
         responses: dict[int, ResponseSpec] | None = None,
         security: list[SecurityRequirement] | None = None,
         summary: str | None = None,
         tags: list[str] | None = None,
@@ -144,14 +145,15 @@
             sync_to_thread: A boolean dictating whether the handler function will be executed in a worker thread or the
                 main event loop. This has an effect only for sync handler functions. See using sync handler functions.
             content_encoding: A string describing the encoding of the content, e.g. ``base64``.
             content_media_type: A string designating the media-type of the content, e.g. ``image/png``.
             deprecated:  A boolean dictating whether this route should be marked as deprecated in the OpenAPI schema.
             description: Text used for the route's schema description section.
             include_in_schema: A boolean flag dictating whether  the route handler should be documented in the OpenAPI schema.
+            operation_class: :class:`Operation <.openapi.spec.operation.Operation>` to be used with the route's OpenAPI schema.
             operation_id: An identifier used for the route's schema operationId. Defaults to the ``__name__`` of the wrapped function.
             raises:  A list of exception classes extending from litestar.HttpException that is used for the OpenAPI documentation.
                 This list should describe all exceptions raised within the route handler's function/method. The Litestar
                 ValidationException will be added automatically for the schema if any validation is involved.
             response_description: Text used for the route's response schema description section.
             security: A sequence of dictionaries that contain information about which security scheme can be used on the endpoint.
             summary: Text used for the route's schema summary section.
@@ -179,14 +181,15 @@
             exception_handlers=exception_handlers,
             guards=guards,
             http_method=HttpMethod.DELETE,
             include_in_schema=include_in_schema,
             media_type=media_type,
             middleware=middleware,
             name=name,
+            operation_class=operation_class,
             operation_id=operation_id,
             opt=opt,
             path=path,
             raises=raises,
             response_class=response_class,
             response_cookies=response_cookies,
             response_description=response_description,
@@ -239,14 +242,15 @@
         sync_to_thread: bool | None = None,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
         include_in_schema: bool = True,
+        operation_class: type[Operation] = Operation,
         operation_id: str | None = None,
         raises: list[type[HTTPException]] | None = None,
         response_description: str | None = None,
         responses: dict[int, ResponseSpec] | None = None,
         security: list[SecurityRequirement] | None = None,
         summary: str | None = None,
         tags: list[str] | None = None,
@@ -305,14 +309,15 @@
             sync_to_thread: A boolean dictating whether the handler function will be executed in a worker thread or the
                 main event loop. This has an effect only for sync handler functions. See using sync handler functions.
             content_encoding: A string describing the encoding of the content, e.g. ``base64``.
             content_media_type: A string designating the media-type of the content, e.g. ``image/png``.
             deprecated:  A boolean dictating whether this route should be marked as deprecated in the OpenAPI schema.
             description: Text used for the route's schema description section.
             include_in_schema: A boolean flag dictating whether  the route handler should be documented in the OpenAPI schema.
+            operation_class: :class:`Operation <.openapi.spec.operation.Operation>` to be used with the route's OpenAPI schema.
             operation_id: An identifier used for the route's schema operationId. Defaults to the ``__name__`` of the wrapped function.
             raises:  A list of exception classes extending from litestar.HttpException that is used for the OpenAPI documentation.
                 This list should describe all exceptions raised within the route handler's function/method. The Litestar
                 ValidationException will be added automatically for the schema if any validation is involved.
             response_description: Text used for the route's response schema description section.
             security: A sequence of dictionaries that contain information about which security scheme can be used on the endpoint.
             summary: Text used for the route's schema summary section.
@@ -341,14 +346,15 @@
             exception_handlers=exception_handlers,
             guards=guards,
             http_method=HttpMethod.GET,
             include_in_schema=include_in_schema,
             media_type=media_type,
             middleware=middleware,
             name=name,
+            operation_class=operation_class,
             operation_id=operation_id,
             opt=opt,
             path=path,
             raises=raises,
             response_class=response_class,
             response_cookies=response_cookies,
             response_description=response_description,
@@ -400,14 +406,15 @@
         sync_to_thread: bool | None = None,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
         include_in_schema: bool = True,
+        operation_class: type[Operation] = Operation,
         operation_id: str | None = None,
         raises: list[type[HTTPException]] | None = None,
         response_description: str | None = None,
         responses: dict[int, ResponseSpec] | None = None,
         return_dto: type[DTOInterface] | None | EmptyType = Empty,
         security: list[SecurityRequirement] | None = None,
         summary: str | None = None,
@@ -471,14 +478,15 @@
             sync_to_thread: A boolean dictating whether the handler function will be executed in a worker thread or the
                 main event loop. This has an effect only for sync handler functions. See using sync handler functions.
             content_encoding: A string describing the encoding of the content, e.g. ``base64``.
             content_media_type: A string designating the media-type of the content, e.g. ``image/png``.
             deprecated:  A boolean dictating whether this route should be marked as deprecated in the OpenAPI schema.
             description: Text used for the route's schema description section.
             include_in_schema: A boolean flag dictating whether  the route handler should be documented in the OpenAPI schema.
+            operation_class: :class:`Operation <.openapi.spec.operation.Operation>` to be used with the route's OpenAPI schema.
             operation_id: An identifier used for the route's schema operationId. Defaults to the ``__name__`` of the wrapped function.
             raises:  A list of exception classes extending from litestar.HttpException that is used for the OpenAPI documentation.
                 This list should describe all exceptions raised within the route handler's function/method. The Litestar
                 ValidationException will be added automatically for the schema if any validation is involved.
             response_description: Text used for the route's response schema description section.
             security: A sequence of dictionaries that contain information about which security scheme can be used on the endpoint.
             summary: Text used for the route's schema summary section.
@@ -507,14 +515,15 @@
             exception_handlers=exception_handlers,
             guards=guards,
             http_method=HttpMethod.HEAD,
             include_in_schema=include_in_schema,
             media_type=media_type,
             middleware=middleware,
             name=name,
+            operation_class=operation_class,
             operation_id=operation_id,
             opt=opt,
             path=path,
             raises=raises,
             response_class=response_class,
             response_cookies=response_cookies,
             response_description=response_description,
@@ -531,20 +540,20 @@
             **kwargs,
         )
 
     def _validate_handler_function(self) -> None:
         """Validate the route handler function once it is set by inspecting its return annotations."""
         super()._validate_handler_function()
 
-        # we allow here File and FileResponse because these have special setting for head responses
+        # we allow here File and File because these have special setting for head responses
         return_annotation = self.parsed_fn_signature.return_type.annotation
         if not (
             return_annotation in {NoneType, None}
             or is_class_and_subclass(return_annotation, File)
-            or is_class_and_subclass(return_annotation, FileResponse)
+            or is_class_and_subclass(return_annotation, ASGIFileResponse)
         ):
             raise ImproperlyConfiguredException("A response to a head request should not have a body")
 
 
 class patch(HTTPRouteHandler):
     """PATCH Route Decorator.
 
@@ -580,14 +589,15 @@
         sync_to_thread: bool | None = None,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
         include_in_schema: bool = True,
+        operation_class: type[Operation] = Operation,
         operation_id: str | None = None,
         raises: list[type[HTTPException]] | None = None,
         response_description: str | None = None,
         responses: dict[int, ResponseSpec] | None = None,
         security: list[SecurityRequirement] | None = None,
         summary: str | None = None,
         tags: list[str] | None = None,
@@ -646,14 +656,15 @@
             sync_to_thread: A boolean dictating whether the handler function will be executed in a worker thread or the
                 main event loop. This has an effect only for sync handler functions. See using sync handler functions.
             content_encoding: A string describing the encoding of the content, e.g. ``base64``.
             content_media_type: A string designating the media-type of the content, e.g. ``image/png``.
             deprecated:  A boolean dictating whether this route should be marked as deprecated in the OpenAPI schema.
             description: Text used for the route's schema description section.
             include_in_schema: A boolean flag dictating whether  the route handler should be documented in the OpenAPI schema.
+            operation_class: :class:`Operation <.openapi.spec.operation.Operation>` to be used with the route's OpenAPI schema.
             operation_id: An identifier used for the route's schema operationId. Defaults to the ``__name__`` of the wrapped function.
             raises:  A list of exception classes extending from litestar.HttpException that is used for the OpenAPI documentation.
                 This list should describe all exceptions raised within the route handler's function/method. The Litestar
                 ValidationException will be added automatically for the schema if any validation is involved.
             response_description: Text used for the route's response schema description section.
             security: A sequence of dictionaries that contain information about which security scheme can be used on the endpoint.
             summary: Text used for the route's schema summary section.
@@ -681,14 +692,15 @@
             exception_handlers=exception_handlers,
             guards=guards,
             http_method=HttpMethod.PATCH,
             include_in_schema=include_in_schema,
             media_type=media_type,
             middleware=middleware,
             name=name,
+            operation_class=operation_class,
             operation_id=operation_id,
             opt=opt,
             path=path,
             raises=raises,
             response_class=response_class,
             response_cookies=response_cookies,
             response_description=response_description,
@@ -741,14 +753,15 @@
         sync_to_thread: bool | None = None,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
         include_in_schema: bool = True,
+        operation_class: type[Operation] = Operation,
         operation_id: str | None = None,
         raises: list[type[HTTPException]] | None = None,
         response_description: str | None = None,
         responses: dict[int, ResponseSpec] | None = None,
         security: list[SecurityRequirement] | None = None,
         summary: str | None = None,
         tags: list[str] | None = None,
@@ -807,14 +820,15 @@
             sync_to_thread: A boolean dictating whether the handler function will be executed in a worker thread or the
                 main event loop. This has an effect only for sync handler functions. See using sync handler functions.
             content_encoding: A string describing the encoding of the content, e.g. ``base64``.
             content_media_type: A string designating the media-type of the content, e.g. ``image/png``.
             deprecated:  A boolean dictating whether this route should be marked as deprecated in the OpenAPI schema.
             description: Text used for the route's schema description section.
             include_in_schema: A boolean flag dictating whether  the route handler should be documented in the OpenAPI schema.
+            operation_class: :class:`Operation <.openapi.spec.operation.Operation>` to be used with the route's OpenAPI schema.
             operation_id: An identifier used for the route's schema operationId. Defaults to the ``__name__`` of the wrapped function.
             raises:  A list of exception classes extending from litestar.HttpException that is used for the OpenAPI documentation.
                 This list should describe all exceptions raised within the route handler's function/method. The Litestar
                 ValidationException will be added automatically for the schema if any validation is involved.
             response_description: Text used for the route's response schema description section.
             security: A sequence of dictionaries that contain information about which security scheme can be used on the endpoint.
             summary: Text used for the route's schema summary section.
@@ -842,14 +856,15 @@
             etag=etag,
             guards=guards,
             http_method=HttpMethod.POST,
             include_in_schema=include_in_schema,
             media_type=media_type,
             middleware=middleware,
             name=name,
+            operation_class=operation_class,
             operation_id=operation_id,
             opt=opt,
             path=path,
             raises=raises,
             response_class=response_class,
             response_cookies=response_cookies,
             response_description=response_description,
@@ -902,14 +917,15 @@
         sync_to_thread: bool | None = None,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
         include_in_schema: bool = True,
+        operation_class: type[Operation] = Operation,
         operation_id: str | None = None,
         raises: list[type[HTTPException]] | None = None,
         response_description: str | None = None,
         responses: dict[int, ResponseSpec] | None = None,
         security: list[SecurityRequirement] | None = None,
         summary: str | None = None,
         tags: list[str] | None = None,
@@ -968,14 +984,15 @@
             sync_to_thread: A boolean dictating whether the handler function will be executed in a worker thread or the
                 main event loop. This has an effect only for sync handler functions. See using sync handler functions.
             content_encoding: A string describing the encoding of the content, e.g. ``base64``.
             content_media_type: A string designating the media-type of the content, e.g. ``image/png``.
             deprecated:  A boolean dictating whether this route should be marked as deprecated in the OpenAPI schema.
             description: Text used for the route's schema description section.
             include_in_schema: A boolean flag dictating whether  the route handler should be documented in the OpenAPI schema.
+            operation_class: :class:`Operation <.openapi.spec.operation.Operation>` to be used with the route's OpenAPI schema.
             operation_id: An identifier used for the route's schema operationId. Defaults to the ``__name__`` of the wrapped function.
             raises:  A list of exception classes extending from litestar.HttpException that is used for the OpenAPI documentation.
                 This list should describe all exceptions raised within the route handler's function/method. The Litestar
                 ValidationException will be added automatically for the schema if any validation is involved.
             response_description: Text used for the route's response schema description section.
             security: A sequence of dictionaries that contain information about which security scheme can be used on the endpoint.
             summary: Text used for the route's schema summary section.
@@ -1003,14 +1020,15 @@
             etag=etag,
             guards=guards,
             http_method=HttpMethod.PUT,
             include_in_schema=include_in_schema,
             media_type=media_type,
             middleware=middleware,
             name=name,
+            operation_class=operation_class,
             operation_id=operation_id,
             opt=opt,
             path=path,
             raises=raises,
             response_class=response_class,
             response_cookies=response_cookies,
             response_description=response_description,
```

### Comparing `litestar-2.0.0a7/litestar/handlers/websocket_handlers/_utils.py` & `litestar-2.0.0b1/litestar/handlers/websocket_handlers/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/handlers/websocket_handlers/listener.py` & `litestar-2.0.0b1/litestar/handlers/websocket_handlers/listener.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 from . import _utils
 from .route_handler import WebsocketRouteHandler
 
 if TYPE_CHECKING:
     from typing import Coroutine
 
-    from litestar import Litestar
+    from litestar import Litestar, Router
     from litestar.dto.interface import DTOInterface
     from litestar.types.asgi_types import WebSocketMode
 
 
 __all__ = ("WebsocketListener", "websocket_listener")
 
 
@@ -278,15 +278,15 @@
         if not self.signature_model:
             new_signature = _utils.create_handler_signature(
                 self._listener_context.listener_callback_signature.original_signature
             )
             self.signature_model = create_signature_model(
                 dependency_name_set=self.dependency_name_set,
                 fn=cast("AnyCallable", self.fn.value),
-                preferred_validation_backend=app.preferred_validation_backend,
+                preferred_validation_backend=app._preferred_validation_backend,
                 parsed_signature=ParsedSignature.from_signature(new_signature, self.resolve_signature_namespace()),
             )
 
     def _set_listener_context(self) -> None:
         listener_context = self._listener_context
         listener_context.listener_callback_signature = listener_callback_signature = ParsedSignature.from_fn(
             listener_context.listener_callback, self.resolve_signature_namespace()
@@ -354,16 +354,24 @@
     A mapping of names to types for use in forward reference resolution during signature modelling.
     """
     type_encoders: TypeEncodersMap | None = None
     """
     type_encoders: A mapping of types to callables that transform them into types supported for serialization.
     """
 
-    def __init__(self) -> None:
-        self._handler = websocket_listener(
+    def __init__(self, owner: Router) -> None:
+        """Initialize a WebsocketListener instance.
+
+        Args:
+            owner: The :class:`Router <.router.Router>` instance that owns this listener.
+        """
+        self._owner = owner
+
+    def to_handler(self) -> websocket_listener:
+        handler = websocket_listener(
             dependencies=self.dependencies,
             dto=self.dto,
             exception_handlers=self.exception_handlers,
             guards=self.guards,
             middleware=self.middleware,
             send_mode=self.send_mode,
             receive_mode=self.receive_mode,
@@ -372,14 +380,16 @@
             on_disconnect=self.on_disconnect,
             opt=self.opt,
             path=self.path,
             return_dto=self.return_dto,
             signature_namespace=self.signature_namespace,
             type_encoders=self.type_encoders,
         )(self.on_receive)
+        handler.owner = self._owner
+        return handler
 
     @abstractmethod
     def on_receive(self, *args: Any, **kwargs: Any) -> Any:
         """Called after data has been received from the WebSocket.
 
         This should take a ``data`` argument, receiving the processed WebSocket data,
         and can additionally include handler dependencies such as ``state``, or other
```

### Comparing `litestar-2.0.0a7/litestar/handlers/websocket_handlers/route_handler.py` & `litestar-2.0.0b1/litestar/handlers/websocket_handlers/route_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Mapping
 
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.handlers import BaseRouteHandler
 from litestar.types.builtin_types import NoneType
-from litestar.utils import is_async_callable
+from litestar.utils.predicates import is_async_callable
 
 if TYPE_CHECKING:
     from litestar.types import Dependencies, ExceptionHandler, Guard, Middleware
 
 
-class WebsocketRouteHandler(BaseRouteHandler["WebsocketRouteHandler"]):
+class WebsocketRouteHandler(BaseRouteHandler):
     """Websocket route handler decorator.
 
     Use this decorator to decorate websocket handler functions.
     """
 
     __slots__ = ()
```

### Comparing `litestar-2.0.0a7/litestar/logging/_utils.py` & `litestar-2.0.0b1/litestar/logging/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/logging/config.py` & `litestar-2.0.0b1/litestar/logging/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/logging/picologging.py` & `litestar-2.0.0b1/litestar/logging/picologging.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/logging/standard.py` & `litestar-2.0.0b1/litestar/logging/standard.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/middleware/_utils.py` & `litestar-2.0.0b1/litestar/middleware/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/middleware/allowed_hosts.py` & `litestar-2.0.0b1/litestar/middleware/allowed_hosts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 import re
 from typing import TYPE_CHECKING, Pattern
 
 from litestar.datastructures import URL, MutableScopeHeaders
 from litestar.middleware.base import AbstractMiddleware
-from litestar.response import RedirectResponse, Response
+from litestar.response.base import ASGIResponse
+from litestar.response.redirect import ASGIRedirectResponse
 from litestar.status_codes import HTTP_400_BAD_REQUEST
 
 __all__ = ("AllowedHostsMiddleware",)
 
 
 if TYPE_CHECKING:
     from litestar.config.allowed_hosts import AllowedHostsConfig
@@ -70,13 +71,13 @@
             if self.allowed_hosts_regex.fullmatch(host):
                 await self.app(scope, receive, send)
                 return
 
             if self.redirect_domains is not None and self.redirect_domains.fullmatch(host):
                 url = URL.from_scope(scope)
                 redirect_url = url.with_replacements(netloc="www." + url.netloc)
-                await RedirectResponse(url=str(redirect_url))(scope, receive, send)
+                redirect_response = ASGIRedirectResponse(path=str(redirect_url))
+                await redirect_response(scope, receive, send)
                 return
 
-        await Response(content={"message": "invalid host header"}, status_code=HTTP_400_BAD_REQUEST)(
-            scope, receive, send
-        )
+        response = ASGIResponse(body=b'{"message":"invalid host header"}', status_code=HTTP_400_BAD_REQUEST)
+        await response(scope, receive, send)
```

### Comparing `litestar-2.0.0a7/litestar/middleware/authentication.py` & `litestar-2.0.0b1/litestar/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/middleware/base.py` & `litestar-2.0.0b1/litestar/middleware/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/middleware/compression.py` & `litestar-2.0.0b1/litestar/middleware/compression.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,15 @@
             None
         """
 
         if self.compression_encoding == CompressionEncoding.BROTLI:
             self.buffer.write(self.compressor.process(body) + self.compressor.flush())  # type: ignore
         else:
             self.compressor.write(body)
+            self.compressor.flush()
 
     def close(self) -> None:
         """Close the compression stream.
 
         Returns:
             None
         """
```

### Comparing `litestar-2.0.0a7/litestar/middleware/cors.py` & `litestar-2.0.0b1/litestar/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/middleware/csrf.py` & `litestar-2.0.0b1/litestar/middleware/csrf.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/middleware/exceptions/_debug_response.py` & `litestar-2.0.0b1/litestar/middleware/exceptions/_debug_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/middleware/exceptions/middleware.py` & `litestar-2.0.0b1/litestar/middleware/exceptions/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from __future__ import annotations
 
+import pdb  # noqa: T100
 from dataclasses import asdict, dataclass, field
 from inspect import getmro
 from sys import exc_info
 from traceback import format_exception
 from typing import TYPE_CHECKING, Any, Type, cast
 
 from litestar.connection import Request
 from litestar.datastructures import Headers
-from litestar.enums import ScopeType
+from litestar.enums import MediaType, ScopeType
 from litestar.exceptions import WebSocketException
 from litestar.middleware.cors import CORSMiddleware
 from litestar.middleware.exceptions._debug_response import create_debug_response
 from litestar.status_codes import HTTP_500_INTERNAL_SERVER_ERROR
 
-__all__ = ("ExceptionHandlerMiddleware",)
+__all__ = ("ExceptionHandlerMiddleware", "ExceptionResponseContent", "create_exception_response")
 
 
 if TYPE_CHECKING:
     from litestar import Response
     from litestar.app import Litestar
     from litestar.logging import BaseLoggingConfig
     from litestar.types import (
@@ -86,14 +87,15 @@
         """
         from litestar.response import Response
 
         return Response(
             content={k: v for k, v in asdict(self).items() if k != "headers" and v is not None},
             headers=self.headers,
             status_code=self.status_code,
+            media_type=MediaType.JSON,
         )
 
 
 def create_exception_response(exc: Exception) -> Response:
     """Construct a response from an exception.
 
     Notes:
@@ -150,15 +152,18 @@
         except Exception as e:  # noqa: BLE001
             litestar_app = scope["app"]
 
             if litestar_app.logging_config and (logger := litestar_app.logger):
                 self.handle_exception_logging(logger=logger, logging_config=litestar_app.logging_config, scope=scope)
 
             for hook in litestar_app.after_exception:
-                await hook(e, scope, litestar_app.state)
+                await hook(e, scope)
+
+            if litestar_app.pdb_on_exception:
+                pdb.post_mortem()
 
             if scope["type"] == ScopeType.HTTP:
                 await self.handle_request_exception(
                     litestar_app=litestar_app, scope=scope, receive=receive, send=send, exc=e
                 )
             else:
                 await self.handle_websocket_exception(send=send, exc=e)
@@ -181,16 +186,17 @@
 
         headers = Headers.from_scope(scope=scope)
         if litestar_app.cors_config and (origin := headers.get("origin")):
             cors_middleware = CORSMiddleware(app=self.app, config=litestar_app.cors_config)
             send = cors_middleware.send_wrapper(send=send, origin=origin, has_cookie="cookie" in headers)
 
         exception_handler = get_exception_handler(self.exception_handlers, exc) or self.default_http_exception_handler
-        response = exception_handler(Request(scope=scope, receive=receive, send=send), exc)
-        await response(scope=scope, receive=receive, send=send)
+        request = Request[Any, Any, Any](scope=scope, receive=receive, send=send)
+        response = exception_handler(request, exc)
+        await response.to_asgi_response(app=litestar_app, request=request)(scope=scope, receive=receive, send=send)
 
     @staticmethod
     async def handle_websocket_exception(send: Send, exc: Exception) -> None:
         """Handle exception raised inside 'websocket' scope routes.
 
         Args:
             send: The ASGI send function.
```

### Comparing `litestar-2.0.0a7/litestar/middleware/exceptions/templates/scripts.js` & `litestar-2.0.0b1/litestar/middleware/exceptions/templates/scripts.js`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/middleware/exceptions/templates/styles.css` & `litestar-2.0.0b1/litestar/middleware/exceptions/templates/styles.css`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/middleware/logging.py` & `litestar-2.0.0b1/litestar/middleware/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     RequestExtractorField,
     ResponseDataExtractor,
     ResponseExtractorField,
 )
 from litestar.enums import ScopeType
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.middleware.base import AbstractMiddleware, DefineMiddleware
-from litestar.serialization import default_serializer, encode_json
+from litestar.serialization import encode_json
 from litestar.utils import (
     get_litestar_scope_state,
     get_serializer_from_scope,
     set_litestar_scope_state,
 )
 
 __all__ = ("LoggingMiddleware", "LoggingMiddlewareConfig")
@@ -191,15 +191,15 @@
         Args:
             scope: The ASGI connection scope.
 
         Returns:
             An dict.
         """
         data: dict[str, Any] = {"message": self.config.response_log_message}
-        serializer = get_serializer_from_scope(scope) or default_serializer
+        serializer = get_serializer_from_scope(scope)
         extracted_data = self.response_extractor(
             messages=(
                 get_litestar_scope_state(scope, HTTP_RESPONSE_START, pop=True),
                 get_litestar_scope_state(scope, HTTP_RESPONSE_BODY, pop=True),
             ),
         )
         response_body_compressed = get_litestar_scope_state(scope, SCOPE_STATE_RESPONSE_COMPRESSED, default=False)
```

### Comparing `litestar-2.0.0a7/litestar/middleware/rate_limit.py` & `litestar-2.0.0b1/litestar/middleware/rate_limit.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/middleware/session/base.py` & `litestar-2.0.0b1/litestar/middleware/session/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/middleware/session/client_side.py` & `litestar-2.0.0b1/litestar/middleware/session/client_side.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/middleware/session/server_side.py` & `litestar-2.0.0b1/litestar/middleware/session/server_side.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/config.py` & `litestar-2.0.0b1/litestar/openapi/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/controller.py` & `litestar-2.0.0b1/litestar/openapi/controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,60 +1,41 @@
 from __future__ import annotations
 
-from copy import copy
 from functools import cached_property
-from typing import TYPE_CHECKING, Callable, Literal, cast
+from typing import TYPE_CHECKING, Callable, Literal
 
 from yaml import dump as dump_yaml
 
 from litestar.constants import OPENAPI_NOT_INITIALIZED
 from litestar.controller import Controller
 from litestar.enums import MediaType, OpenAPIMediaType
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.handlers import get
-from litestar.response import Response
+from litestar.response.base import ASGIResponse
 from litestar.serialization import encode_json
 from litestar.status_codes import HTTP_404_NOT_FOUND
 
-__all__ = ("OpenAPIController", "OpenAPISchemaResponse")
+__all__ = ("OpenAPIController",)
 
 
 if TYPE_CHECKING:
     from litestar.connection.request import Request
     from litestar.openapi.spec.open_api import OpenAPI
 
 
-class OpenAPISchemaResponse(Response):
-    """Response class for OpenAPI Schemas."""
-
-    def render(self, content: OpenAPI) -> bytes:
-        """Handle rendering of schema into the correct format - either YAML or JSON.
-
-        Args:
-            content: The :class:`OpenAPI <litestar.openapi.spec.open_api.OpenAPI>` instance to render.
-
-        Returns:
-            Rendered bytes.
-        """
-        content_dict = content.to_schema()
-        if self.media_type == OpenAPIMediaType.OPENAPI_YAML:
-            return cast("bytes", dump_yaml(content_dict, default_flow_style=False).encode("utf-8"))
-        return encode_json(content_dict)
-
-
 class OpenAPIController(Controller):
     """Controller for OpenAPI endpoints."""
 
     path: str = "/schema"
     """Base path for the OpenAPI documentation endpoints."""
     style: str = "body { margin: 0; padding: 0 }"
     """Base styling of the html body."""
     redoc_version: str = "next"
     """Redoc version to download from the CDN."""
-    swagger_ui_version: str = "4.15.5"
+    swagger_ui_version: str = "5.0.0"
     """SwaggerUI version to download from the CDN."""
     stoplight_elements_version: str = "7.7.5"
     """StopLight Elements version to download from the CDN."""
     favicon_url: str = ""
     """URL to download a favicon from."""
     redoc_google_fonts: bool = True
     """Download google fonts via CDN.
@@ -140,62 +121,64 @@
 
         Returns:
             A ``<link>`` tag if ``self.favicon_url`` is not empty, otherwise returns a placeholder meta tag.
         """
         return f"<link rel='icon' type='image/x-icon' href='{self.favicon_url}'>" if self.favicon_url else "<meta/>"
 
     @cached_property
-    def render_methods_map(self) -> dict[Literal["redoc", "swagger", "elements"], Callable[[Request], str]]:
+    def render_methods_map(self) -> dict[Literal["redoc", "swagger", "elements"], Callable[[Request], bytes]]:
         """Map render method names to render methods.
 
         Returns:
             A mapping of string keys to render methods.
         """
         return {
             "redoc": self.render_redoc,
             "swagger": self.render_swagger_ui,
             "elements": self.render_stoplight_elements,
         }
 
     @get(path="/openapi.yaml", media_type=OpenAPIMediaType.OPENAPI_YAML, include_in_schema=False, sync_to_thread=False)
-    def retrieve_schema_yaml(self, request: Request) -> Response:
+    def retrieve_schema_yaml(self, request: Request) -> ASGIResponse:
         """Return the OpenAPI schema as YAML with an ``application/vnd.oai.openapi`` Content-Type header.
 
         Args:
             request:
                 A :class:`Request <.connection.Request>` instance.
 
         Returns:
             A Response instance with the YAML object rendered into a string.
         """
         if self.should_serve_endpoint(request):
-            return OpenAPISchemaResponse(
-                content=self.get_schema_from_request(request), media_type=OpenAPIMediaType.OPENAPI_YAML
+            content = dump_yaml(self.get_schema_from_request(request).to_schema(), default_flow_style=False).encode(
+                "utf-8"
             )
-        return Response(content={}, status_code=HTTP_404_NOT_FOUND)
+            return ASGIResponse(body=content, media_type=OpenAPIMediaType.OPENAPI_YAML)
+        return ASGIResponse(body=b"", status_code=HTTP_404_NOT_FOUND, media_type=MediaType.HTML)
 
     @get(path="/openapi.json", media_type=OpenAPIMediaType.OPENAPI_JSON, include_in_schema=False, sync_to_thread=False)
-    def retrieve_schema_json(self, request: Request) -> Response:
+    def retrieve_schema_json(self, request: Request) -> ASGIResponse:
         """Return the OpenAPI schema as JSON with an ``application/vnd.oai.openapi+json`` Content-Type header.
 
         Args:
             request:
                 A :class:`Request <.connection.Request>` instance.
 
         Returns:
             A Response instance with the JSON object rendered into a string.
         """
         if self.should_serve_endpoint(request):
-            return OpenAPISchemaResponse(
-                content=self.get_schema_from_request(request), media_type=OpenAPIMediaType.OPENAPI_JSON
+            return ASGIResponse(
+                body=encode_json(self.get_schema_from_request(request).to_schema()),
+                media_type=OpenAPIMediaType.OPENAPI_JSON,
             )
-        return Response(content={}, status_code=HTTP_404_NOT_FOUND)
+        return ASGIResponse(body=b"", status_code=HTTP_404_NOT_FOUND, media_type=MediaType.HTML)
 
-    @get(path="/", media_type=MediaType.HTML, include_in_schema=False, sync_to_thread=False)
-    def root(self, request: Request) -> Response:
+    @get(path="/", include_in_schema=False, sync_to_thread=False)
+    def root(self, request: Request) -> ASGIResponse:
         """Render a static documentation site.
 
          The site to be rendered is based on the ``root_schema_site`` value set in the application's
          :class:`OpenAPIConfig <.openapi.OpenAPIConfig>`. Defaults to ``redoc``.
 
         Args:
             request:
@@ -210,93 +193,77 @@
         config = request.app.openapi_config
         if not config:  # pragma: no cover
             raise ImproperlyConfiguredException(OPENAPI_NOT_INITIALIZED)
 
         render_method = self.render_methods_map[config.root_schema_site]
 
         if self.should_serve_endpoint(request):
-            return Response(content=render_method(request), media_type=MediaType.HTML)
+            return ASGIResponse(body=render_method(request), media_type=MediaType.HTML)
+        return ASGIResponse(body=self.render_404_page(), status_code=HTTP_404_NOT_FOUND, media_type=MediaType.HTML)
 
-        return Response(
-            content=self.render_404_page(),
-            status_code=HTTP_404_NOT_FOUND,
-            media_type=MediaType.HTML,
-        )
-
-    @get(path="/swagger", media_type=MediaType.HTML, include_in_schema=False, sync_to_thread=False)
-    def swagger_ui(self, request: Request) -> Response:
+    @get(path="/swagger", include_in_schema=False, sync_to_thread=False)
+    def swagger_ui(self, request: Request) -> ASGIResponse:
         """Route handler responsible for rendering Swagger-UI.
 
         Args:
             request:
                 A :class:`Request <.connection.Request>` instance.
 
         Returns:
             A response with a rendered swagger documentation site
         """
         if self.should_serve_endpoint(request):
-            return Response(content=self.render_swagger_ui(request), media_type=MediaType.HTML)
-        return Response(
-            content=self.render_404_page(),
-            status_code=HTTP_404_NOT_FOUND,
-            media_type=MediaType.HTML,
-        )
+            return ASGIResponse(body=self.render_swagger_ui(request), media_type=MediaType.HTML)
+        return ASGIResponse(body=self.render_404_page(), status_code=HTTP_404_NOT_FOUND, media_type=MediaType.HTML)
 
     @get(path="/elements", media_type=MediaType.HTML, include_in_schema=False, sync_to_thread=False)
-    def stoplight_elements(self, request: Request) -> Response:
+    def stoplight_elements(self, request: Request) -> ASGIResponse:
         """Route handler responsible for rendering StopLight Elements.
 
         Args:
             request:
                 A :class:`Request <.connection.Request>` instance.
 
         Returns:
             A response with a rendered stoplight elements documentation site
         """
         if self.should_serve_endpoint(request):
-            return Response(content=self.render_stoplight_elements(request), media_type=MediaType.HTML)
-        return Response(content=self.render_404_page(), status_code=HTTP_404_NOT_FOUND, media_type=MediaType.HTML)
+            return ASGIResponse(body=self.render_stoplight_elements(request), media_type=MediaType.HTML)
+        return ASGIResponse(body=self.render_404_page(), status_code=HTTP_404_NOT_FOUND, media_type=MediaType.HTML)
 
     @get(path="/redoc", media_type=MediaType.HTML, include_in_schema=False, sync_to_thread=False)
-    def redoc(self, request: Request) -> Response:  # pragma: no cover
+    def redoc(self, request: Request) -> ASGIResponse:  # pragma: no cover
         """Route handler responsible for rendering Redoc.
 
         Args:
             request:
                 A :class:`Request <.connection.Request>` instance.
 
         Returns:
             A response with a rendered redoc documentation site
         """
         if self.should_serve_endpoint(request):
-            return Response(content=self.render_redoc(request), media_type=MediaType.HTML)
-        return Response(content=self.render_404_page(), status_code=HTTP_404_NOT_FOUND, media_type=MediaType.HTML)
+            return ASGIResponse(body=self.render_redoc(request), media_type=MediaType.HTML)
+        return ASGIResponse(body=self.render_404_page(), status_code=HTTP_404_NOT_FOUND, media_type=MediaType.HTML)
 
-    def render_swagger_ui(self, request: Request) -> str:
+    def render_swagger_ui(self, request: Request) -> bytes:
         """Render an HTML page for Swagger-UI.
 
         Notes:
             - override this method to customize the template.
 
         Args:
             request:
                 A :class:`Request <.connection.Request>` instance.
 
         Returns:
             A rendered html string.
         """
         schema = self.get_schema_from_request(request)
 
-        # Note: Fix for Swagger rejection OpenAPI >=3.1
-        if not self._dumped_modified_schema:
-            schema_copy = copy(schema)
-            schema_copy.openapi = "3.0.3"
-
-            self._dumped_modified_schema = encode_json(schema_copy.to_schema()).decode("utf-8")
-
         head = f"""
           <head>
             <title>{schema.info.title}</title>
             {self.favicon}
             <meta charset="utf-8"/>
             <meta name="viewport" content="width=device-width, initial-scale=1">
             <link href="{self.swagger_css_url}" rel="stylesheet">
@@ -307,15 +274,15 @@
         """
 
         body = f"""
           <body>
             <div id='swagger-container'/>
             <script type="text/javascript">
             const ui = SwaggerUIBundle({{
-                spec: {self._dumped_modified_schema},
+                spec: {encode_json(schema.to_schema()).decode("utf-8")},
                 dom_id: '#swagger-container',
                 deepLinking: true,
                 showExtensions: true,
                 showCommonExtensions: true,
                 presets: [
                     SwaggerUIBundle.presets.apis,
                     SwaggerUIBundle.SwaggerUIStandalonePreset
@@ -327,17 +294,17 @@
 
         return f"""
         <!DOCTYPE html>
             <html>
                 {head}
                 {body}
             </html>
-        """
+        """.encode()
 
-    def render_stoplight_elements(self, request: Request) -> str:
+    def render_stoplight_elements(self, request: Request) -> bytes:
         """Render an HTML page for StopLight Elements.
 
         Notes:
             - override this method to customize the template.
 
         Args:
             request:
@@ -371,17 +338,17 @@
 
         return f"""
         <!DOCTYPE html>
             <html>
                 {head}
                 {body}
             </html>
-        """
+        """.encode()
 
-    def render_redoc(self, request: Request) -> str:  # pragma: no cover
+    def render_redoc(self, request: Request) -> bytes:  # pragma: no cover
         """Render an HTML page for Redoc.
 
         Notes:
             - override this method to customize the template.
 
         Args:
             request:
@@ -431,17 +398,17 @@
 
         return f"""
         <!DOCTYPE html>
             <html>
                 {head}
                 {body}
             </html>
-        """
+        """.encode()
 
-    def render_404_page(self) -> str:
+    def render_404_page(self) -> bytes:
         """Render an HTML 404 page.
 
         Returns:
             A rendered html string.
         """
 
         return f"""
@@ -456,8 +423,8 @@
                     {self.style}
                 </style>
             </head>
             <body>
                 <h1>Error 404</h1>
             </body>
         </html>
-        """
+        """.encode()
```

### Comparing `litestar-2.0.0a7/litestar/openapi/datastructures.py` & `litestar-2.0.0b1/litestar/openapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/__init__.py` & `litestar-2.0.0b1/litestar/openapi/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/base.py` & `litestar-2.0.0b1/litestar/openapi/spec/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,11 +44,17 @@
         """
         result: dict[str, Any] = {}
 
         for field in fields(self):
             value = _normalize_value(getattr(self, field.name, None))
 
             if value is not None:
-                key = _normalize_key(field.name)
+                if "alias" in field.metadata:
+                    if not isinstance(field.metadata["alias"], str):
+                        raise TypeError('metadata["alias"] must be a str')
+                    key = field.metadata["alias"]
+                else:
+                    key = _normalize_key(field.name)
+
                 result[key] = value
 
         return result
```

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/callback.py` & `litestar-2.0.0b1/litestar/openapi/spec/callback.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/components.py` & `litestar-2.0.0b1/litestar/openapi/spec/components.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/contact.py` & `litestar-2.0.0b1/litestar/openapi/spec/contact.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/discriminator.py` & `litestar-2.0.0b1/litestar/openapi/spec/discriminator.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/encoding.py` & `litestar-2.0.0b1/litestar/openapi/spec/encoding.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/enums.py` & `litestar-2.0.0b1/litestar/openapi/spec/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/example.py` & `litestar-2.0.0b1/litestar/openapi/spec/example.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/external_documentation.py` & `litestar-2.0.0b1/litestar/openapi/spec/external_documentation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/header.py` & `litestar-2.0.0b1/litestar/openapi/spec/header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/info.py` & `litestar-2.0.0b1/litestar/openapi/spec/info.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/license.py` & `litestar-2.0.0b1/litestar/openapi/spec/license.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/link.py` & `litestar-2.0.0b1/litestar/openapi/spec/link.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/media_type.py` & `litestar-2.0.0b1/litestar/openapi/spec/media_type.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/oauth_flow.py` & `litestar-2.0.0b1/litestar/openapi/spec/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/oauth_flows.py` & `litestar-2.0.0b1/litestar/openapi/spec/oauth_flows.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/open_api.py` & `litestar-2.0.0b1/litestar/openapi/spec/open_api.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/operation.py` & `litestar-2.0.0b1/litestar/openapi/spec/operation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/parameter.py` & `litestar-2.0.0b1/litestar/openapi/spec/parameter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/path_item.py` & `litestar-2.0.0b1/litestar/openapi/spec/path_item.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/paths.py` & `litestar-2.0.0b1/litestar/openapi/spec/paths.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/reference.py` & `litestar-2.0.0b1/litestar/openapi/spec/reference.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/request_body.py` & `litestar-2.0.0b1/litestar/openapi/spec/request_body.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/response.py` & `litestar-2.0.0b1/litestar/openapi/spec/response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/responses.py` & `litestar-2.0.0b1/litestar/openapi/spec/responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/schema.py` & `litestar-2.0.0b1/litestar/openapi/spec/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/security_requirement.py` & `litestar-2.0.0b1/litestar/openapi/spec/security_requirement.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/security_scheme.py` & `litestar-2.0.0b1/litestar/openapi/spec/security_scheme.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/server.py` & `litestar-2.0.0b1/litestar/openapi/spec/server.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/server_variable.py` & `litestar-2.0.0b1/litestar/openapi/spec/server_variable.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/tag.py` & `litestar-2.0.0b1/litestar/openapi/spec/tag.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/openapi/spec/xml.py` & `litestar-2.0.0b1/litestar/openapi/spec/xml.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/pagination.py` & `litestar-2.0.0b1/litestar/pagination.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+# ruff: noqa: UP006,UP007
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from typing import Generic, TypeVar
+from typing import Generic, List, Optional, TypeVar
 from uuid import UUID
 
 __all__ = (
     "AbstractAsyncClassicPaginator",
     "AbstractAsyncCursorPaginator",
     "AbstractAsyncOffsetPaginator",
     "AbstractSyncClassicPaginator",
@@ -24,15 +25,15 @@
 
 @dataclass
 class ClassicPagination(Generic[T]):
     """Container for data returned using limit/offset pagination."""
 
     __slots__ = ("items", "page_size", "current_page", "total_pages")
 
-    items: list[T]
+    items: List[T]
     """List of data being sent as part of the response."""
     page_size: int
     """Number of items per page."""
     current_page: int
     """Current page number."""
     total_pages: int
     """Total number of pages."""
@@ -40,15 +41,15 @@
 
 @dataclass
 class OffsetPagination(Generic[T]):
     """Container for data returned using limit/offset pagination."""
 
     __slots__ = ("items", "limit", "offset", "total")
 
-    items: list[T]
+    items: List[T]
     """List of data being sent as part of the response."""
     limit: int
     """Maximal number of items to send."""
     offset: int
     """Offset from the beginning of the query.
 
     Identical to an index.
@@ -59,19 +60,19 @@
 
 @dataclass
 class CursorPagination(Generic[C, T]):
     """Container for data returned using cursor pagination."""
 
     __slots__ = ("items", "results_per_page", "cursor", "next_cursor")
 
-    items: list[T]
+    items: List[T]
     """List of data being sent as part of the response."""
     results_per_page: int
     """Maximal number of items to send."""
-    cursor: C | None
+    cursor: Optional[C]
     """Unique ID, designating the last identifier in the given data set.
 
     This value can be used to request the "next" batch of records.
     """
 
 
 class AbstractSyncClassicPaginator(ABC, Generic[T]):
```

### Comparing `litestar-2.0.0a7/litestar/params.py` & `litestar-2.0.0b1/litestar/params.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,50 +2,44 @@
 
 from dataclasses import asdict, dataclass, field
 from typing import TYPE_CHECKING, Any, Hashable
 
 from litestar.enums import RequestEncodingType
 from litestar.types import Empty
 
-__all__ = ("Body", "BodyKwarg", "Dependency", "DependencyKwarg", "Parameter", "ParameterKwarg")
+__all__ = (
+    "Body",
+    "BodyKwarg",
+    "Dependency",
+    "DependencyKwarg",
+    "KwargDefinition",
+    "Parameter",
+)
 
 
 if TYPE_CHECKING:
     from litestar.openapi.spec.example import Example
     from litestar.openapi.spec.external_documentation import (
         ExternalDocumentation,
     )
 
 
 @dataclass(frozen=True)
-class ParameterKwarg:
-    """Data container representing a parameter."""
+class KwargDefinition:
+    """Data container representing a constrained kwarg."""
 
-    value_type: Any = field(default=Empty)
-    """The field value - `Empty` by default."""
-    header: str | None = field(default=None)
-    """The header parameter key - required for header parameters."""
-    cookie: str | None = field(default=None)
-    """The cookie parameter key - required for cookie parameters."""
-    query: str | None = field(default=None)
-    """The query parameter key for this parameter."""
     examples: list[Example] | None = field(default=None)
     """A list of Example models."""
     external_docs: ExternalDocumentation | None = field(default=None)
     """A url pointing at external documentation for the given parameter."""
     content_encoding: str | None = field(default=None)
     """The content encoding of the value.
 
     Applicable on to string values. See OpenAPI 3.1 for details.
     """
-    required: bool | None = field(default=None)
-    """A boolean flag dictating whether this parameter is required.
-
-    If set to False, None values will be allowed. Defaults to True.
-    """
     default: Any = field(default=Empty)
     """A default value.
 
     If const is true, this value is required.
     """
     title: str | None = field(default=None)
     """String value used in the title section of the OpenAPI schema for the given parameter."""
@@ -98,96 +92,138 @@
     Equivalent to minLength in the OpenAPI specification.
     """
     max_length: int | None = field(default=None)
     """Constrict a string or bytes value to have a maximum length.
 
     Equivalent to maxLength in the OpenAPI specification.
     """
-    regex: str | None = field(default=None)
+    pattern: str | None = field(default=None)
     """A string representing a regex against which the given string will be matched.
 
     Equivalent to pattern in the OpenAPI specification.
     """
+    lower_case: bool | None = field(default=None)
+    """Constrict a string value to be lower case."""
+    upper_case: bool | None = field(default=None)
+    """Constrict a string value to be upper case."""
+
+    @property
+    def is_constrained(self) -> bool:
+        """Return True if any of the constraints are set."""
+        return any(
+            attr if attr and attr is not Empty else False  # type: ignore[comparison-overlap]
+            for attr in (
+                self.gt,
+                self.ge,
+                self.lt,
+                self.le,
+                self.multiple_of,
+                self.min_items,
+                self.max_items,
+                self.min_length,
+                self.max_length,
+                self.pattern,
+                self.const,
+                self.lower_case,
+                self.upper_case,
+            )
+        )
+
+
+@dataclass(frozen=True)
+class ParameterKwarg(KwargDefinition):
+    """Data container representing a parameter."""
+
+    value_type: Any = field(default=Empty)
+    """The field value - `Empty` by default."""
+    header: str | None = field(default=None)
+    """The header parameter key - required for header parameters."""
+    cookie: str | None = field(default=None)
+    """The cookie parameter key - required for cookie parameters."""
+    query: str | None = field(default=None)
+    """The query parameter key for this parameter."""
+    required: bool | None = field(default=None)
+    """A boolean flag dictating whether this parameter is required.
+
+    If set to False, None values will be allowed. Defaults to True.
+    """
 
     def __hash__(self) -> int:  # pragma: no cover
         """Hash the dataclass in a safe way.
 
         Returns:
             A hash
         """
         return sum(hash(v) for v in asdict(self) if isinstance(v, Hashable))
 
 
 def Parameter(
     value_type: Any = Empty,
     *,
-    header: str | None = None,
-    cookie: str | None = None,
-    query: str | None = None,
-    examples: list[Example] | None = None,
-    external_docs: ExternalDocumentation | None = None,
+    const: bool | None = None,
     content_encoding: str | None = None,
-    required: bool | None = None,
+    cookie: str | None = None,
     default: Any = Empty,
-    title: str | None = None,
     description: str | None = None,
-    const: bool | None = None,
-    gt: float | None = None,
+    examples: list[Example] | None = None,
+    external_docs: ExternalDocumentation | None = None,
     ge: float | None = None,
-    lt: float | None = None,
+    gt: float | None = None,
+    header: str | None = None,
     le: float | None = None,
-    multiple_of: float | None = None,
-    min_items: int | None = None,
+    lt: float | None = None,
     max_items: int | None = None,
-    min_length: int | None = None,
     max_length: int | None = None,
-    regex: str | None = None,
+    min_items: int | None = None,
+    min_length: int | None = None,
+    multiple_of: float | None = None,
+    pattern: str | None = None,
+    query: str | None = None,
+    required: bool | None = None,
+    title: str | None = None,
 ) -> Any:
     """Create an extended parameter kwarg definition.
 
     Args:
         value_type: `Empty` by default.
-        header: The header parameter key - required for header parameters.
+        const: A boolean flag dictating whether this parameter is a constant. If True, the value passed to the parameter
+            must equal its default value. This also causes the OpenAPI const field
+            to be populated with the default value.
+        content_encoding: The content encoding of the value.
+            Applicable on to string values. See OpenAPI 3.1 for details.
         cookie: The cookie parameter key - required for cookie parameters.
-        query: The query parameter key for this parameter.
-        examples: A list of Example models.
-        external_docs: A url pointing at external documentation for the given
-            parameter.
-        content_encoding: The content encoding of the value. Applicable on to string values. See
-            OpenAPI 3.1 for details.
-        required: A boolean flag dictating whether this parameter is required. If set to False, None
-            values will be allowed. Defaults to True.
         default: A default value. If const is true, this value is required.
-        title: String value used in the title section of the OpenAPI schema for the given
-            parameter.
-        description: String value used in the description section of the OpenAPI schema for the
-            given parameter.
-        const: A boolean flag dictating whether this parameter is a constant. If True, the value passed
-            to the parameter must equal its default value. This also causes the OpenAPI const field to be populated with
-            the default value.
-        gt: Constrict value to be greater than a given float or int. Equivalent to
-            exclusiveMinimum in the OpenAPI specification.
-        ge: Constrict value to be greater or equal to a given float or int. Equivalent to
-            minimum in the OpenAPI specification.
-        lt: Constrict value to be less than a given float or int. Equivalent to
-            exclusiveMaximum in the OpenAPI specification.
-        le: Constrict value to be less or equal to a given float or int. Equivalent to maximum
-            in the OpenAPI specification.
-        multiple_of: Constrict value to a multiple of a given float or int. Equivalent to
-            multipleOf in the OpenAPI specification.
-        min_items: Constrict a set or a list to have a minimum number of items. Equivalent to
-            minItems in the OpenAPI specification.
-        max_items: Constrict a set or a list to have a maximum number of items. Equivalent to
-            maxItems in the OpenAPI specification.
-        min_length: Constrict a string or bytes value to have a minimum length. Equivalent to
-            minLength in the OpenAPI specification.
-        max_length: Constrict a string or bytes value to have a maximum length. Equivalent to
-            maxLength in the OpenAPI specification.
-        regex: A string representing a regex against which the given string will be matched.
+        description: String value used in the description section of the OpenAPI schema for the given parameter.
+        examples: A list of Example models.
+        external_docs: A url pointing at external documentation for the given parameter.
+        ge: Constrict value to be greater or equal to a given float or int.
+            Equivalent to minimum in the OpenAPI specification.
+        gt: Constrict value to be greater than a given float or int.
+            Equivalent to exclusiveMinimum in the OpenAPI specification.
+        header: The header parameter key - required for header parameters.
+        le: Constrict value to be less or equal to a given float or int.
+            Equivalent to maximum in the OpenAPI specification.
+        lt: Constrict value to be less than a given float or int.
+            Equivalent to exclusiveMaximum in the OpenAPI specification.
+        max_items: Constrict a set or a list to have a maximum number of items.
+            Equivalent to maxItems in the OpenAPI specification.
+        max_length: Constrict a string or bytes value to have a maximum length.
+            Equivalent to maxLength in the OpenAPI specification.
+        min_items: Constrict a set or a list to have a minimum number of items. ֿ
+            Equivalent to minItems in the OpenAPI specification.
+        min_length: Constrict a string or bytes value to have a minimum length.
+            Equivalent to minLength in the OpenAPI specification.
+        multiple_of: Constrict value to a multiple of a given float or int.
+            Equivalent to multipleOf in the OpenAPI specification.
+        pattern: A string representing a regex against which the given string will be matched.
             Equivalent to pattern in the OpenAPI specification.
+        query: The query parameter key for this parameter.
+        required: A boolean flag dictating whether this parameter is required.
+            If set to False, None values will be allowed. Defaults to True.
+        title: String value used in the title section of the OpenAPI schema for the given parameter.
     """
     return ParameterKwarg(
         value_type=value_type,
         header=header,
         cookie=cookie,
         query=query,
         examples=examples,
@@ -203,171 +239,95 @@
         lt=lt,
         le=le,
         multiple_of=multiple_of,
         min_items=min_items,
         max_items=max_items,
         min_length=min_length,
         max_length=max_length,
-        regex=regex,
+        pattern=pattern,
     )
 
 
 @dataclass(frozen=True)
-class BodyKwarg:
+class BodyKwarg(KwargDefinition):
     """Data container representing a request body."""
 
     media_type: str | RequestEncodingType = field(default=RequestEncodingType.JSON)
     """Media-Type of the body."""
-    examples: list[Example] | None = field(default=None)
-    """A list of Example models."""
-    external_docs: ExternalDocumentation | None = field(default=None)
-    """A url pointing at external documentation for the given parameter."""
-    content_encoding: str | None = field(default=None)
-    """The content encoding of the value.
-
-    Applicable on to string values. See OpenAPI 3.1 for details.
-    """
-    default: Any = field(default=Empty)
-    """A default value.
-
-    If const is true, this value is required.
-    """
-    title: str | None = field(default=None)
-    """String value used in the title section of the OpenAPI schema for the given parameter."""
-    description: str | None = field(default=None)
-    """String value used in the description section of the OpenAPI schema for the given parameter."""
-    const: bool | None = field(default=None)
-    """A boolean flag dictating whether this parameter is a constant.
 
-    If True, the value passed to the parameter must equal its default value. This also causes the OpenAPI const field to
-    be populated with the default value.
-    """
-    gt: float | None = field(default=None)
-    """Constrict value to be greater than a given float or int.
-
-    Equivalent to exclusiveMinimum in the OpenAPI specification.
-    """
-    ge: float | None = field(default=None)
-    """Constrict value to be greater or equal to a given float or int.
-
-    Equivalent to minimum in the OpenAPI specification.
-    """
-    lt: float | None = field(default=None)
-    """Constrict value to be less than a given float or int.
-
-    Equivalent to exclusiveMaximum in the OpenAPI specification.
-    """
-    le: float | None = field(default=None)
-    """Constrict value to be less or equal to a given float or int.
-
-    Equivalent to maximum in the OpenAPI specification.
-    """
-    multiple_of: float | None = field(default=None)
-    """Constrict value to a multiple of a given float or int.
-
-    Equivalent to multipleOf in the OpenAPI specification.
-    """
-    min_items: int | None = field(default=None)
-    """Constrict a set or a list to have a minimum number of items.
-
-    Equivalent to minItems in the OpenAPI specification.
-    """
-    max_items: int | None = field(default=None)
-    """Constrict a set or a list to have a maximum number of items.
-
-    Equivalent to maxItems in the OpenAPI specification.
-    """
-    min_length: int | None = field(default=None)
-    """Constrict a string or bytes value to have a minimum length.
-
-    Equivalent to minLength in the OpenAPI specification.
-    """
-    max_length: int | None = field(default=None)
-    """Constrict a string or bytes value to have a maximum length.
-
-    Equivalent to maxLength in the OpenAPI specification.
-    """
-    regex: str | None = field(default=None)
-    """A string representing a regex against which the given string will be matched.
-
-    Equivalent to pattern in the OpenAPI specification.
-    """
     multipart_form_part_limit: int | None = field(default=None)
     """The maximal number of allowed parts in a multipart/formdata request. This limit is intended to protect from DoS attacks."""
 
     def __hash__(self) -> int:  # pragma: no cover
         """Hash the dataclass in a safe way.
 
         Returns:
             A hash
         """
         return sum(hash(v) for v in asdict(self) if isinstance(v, Hashable))
 
 
 def Body(
     *,
-    media_type: str | RequestEncodingType = RequestEncodingType.JSON,
-    examples: list[Example] | None = None,
-    external_docs: ExternalDocumentation | None = None,
+    const: bool | None = None,
     content_encoding: str | None = None,
     default: Any = Empty,
-    title: str | None = None,
     description: str | None = None,
-    const: bool | None = None,
-    gt: float | None = None,
+    examples: list[Example] | None = None,
+    external_docs: ExternalDocumentation | None = None,
     ge: float | None = None,
-    lt: float | None = None,
+    gt: float | None = None,
     le: float | None = None,
-    multiple_of: float | None = None,
-    min_items: int | None = None,
+    lt: float | None = None,
     max_items: int | None = None,
-    min_length: int | None = None,
     max_length: int | None = None,
-    regex: str | None = None,
+    media_type: str | RequestEncodingType = RequestEncodingType.JSON,
+    min_items: int | None = None,
+    min_length: int | None = None,
     multipart_form_part_limit: int | None = None,
+    multiple_of: float | None = None,
+    pattern: str | None = None,
+    title: str | None = None,
 ) -> Any:
     """Create an extended request body kwarg definition.
 
     Args:
-        media_type: Defaults to RequestEncodingType.JSON.
-        examples: A list of Example models.
-        external_docs: A url pointing at external documentation for the given
-            parameter.
-        content_encoding: The content encoding of the value. Applicable on to string values. See
-            OpenAPI 3.1 for details.
+        const: A boolean flag dictating whether this parameter is a constant. If True, the value passed to the parameter
+            must equal its default value. This also causes the OpenAPI const field to be
+            populated with the default value.
+        content_encoding: The content encoding of the value. Applicable on to string values.
+            See OpenAPI 3.1 for details.
         default: A default value. If const is true, this value is required.
-        title: String value used in the title section of the OpenAPI schema for the given
-            parameter.
-        description: String value used in the description section of the OpenAPI schema for the
-            given parameter.
-        const: A boolean flag dictating whether this parameter is a constant. If True, the value passed
-            to the parameter must equal its default value. This also causes the OpenAPI const field to be populated with
-            the default value.
-        gt: Constrict value to be greater than a given float or int. Equivalent to
-            exclusiveMinimum in the OpenAPI specification.
-        ge: Constrict value to be greater or equal to a given float or int. Equivalent to
-            minimum in the OpenAPI specification.
-        lt: Constrict value to be less than a given float or int. Equivalent to
-            exclusiveMaximum in the OpenAPI specification.
-        le: Constrict value to be less or equal to a given float or int. Equivalent to maximum
-            in the OpenAPI specification.
-        multiple_of: Constrict value to a multiple of a given float or int. Equivalent to
-            multipleOf in the OpenAPI specification.
-        min_items: Constrict a set or a list to have a minimum number of items. Equivalent to
-            minItems in the OpenAPI specification.
-        max_items: Constrict a set or a list to have a maximum number of items. Equivalent to
-            maxItems in the OpenAPI specification.
-        min_length: Constrict a string or bytes value to have a minimum length. Equivalent to
-            minLength in the OpenAPI specification.
-        max_length: Constrict a string or bytes value to have a maximum length. Equivalent to
-            maxLength in the OpenAPI specification.
-        regex: A string representing a regex against which the given string will be matched.
-            Equivalent to pattern in the OpenAPI specification.
+        description: String value used in the description section of the OpenAPI schema for the given parameter.
+        examples: A list of Example models.
+        external_docs: A url pointing at external documentation for the given parameter.
+        ge: Constrict value to be greater or equal to a given float or int.
+            Equivalent to minimum in the OpenAPI specification.
+        gt: Constrict value to be greater than a given float or int.
+            Equivalent to exclusiveMinimum in the OpenAPI specification.
+        le: Constrict value to be less or equal to a given float or int.
+            Equivalent to maximum in the OpenAPI specification.
+        lt: Constrict value to be less than a given float or int.
+            Equivalent to exclusiveMaximum in the OpenAPI specification.
+        max_items: Constrict a set or a list to have a maximum number of items.
+            Equivalent to maxItems in the OpenAPI specification.
+        max_length: Constrict a string or bytes value to have a maximum length.
+            Equivalent to maxLength in the OpenAPI specification.
+        media_type: Defaults to RequestEncodingType.JSON.
+        min_items: Constrict a set or a list to have a minimum number of items.
+            Equivalent to minItems in the OpenAPI specification.
+        min_length: Constrict a string or bytes value to have a minimum length.
+            Equivalent to minLength in the OpenAPI specification.
         multipart_form_part_limit: The maximal number of allowed parts in a multipart/formdata request.
             This limit is intended to protect from DoS attacks.
+        multiple_of: Constrict value to a multiple of a given float or int.
+            Equivalent to multipleOf in the OpenAPI specification.
+        pattern: A string representing a regex against which the given string will be matched.
+            Equivalent to pattern in the OpenAPI specification.
+        title: String value used in the title section of the OpenAPI schema for the given parameter.
     """
     return BodyKwarg(
         media_type=media_type,
         examples=examples,
         external_docs=external_docs,
         content_encoding=content_encoding,
         default=default,
@@ -379,15 +339,15 @@
         lt=lt,
         le=le,
         multiple_of=multiple_of,
         min_items=min_items,
         max_items=max_items,
         min_length=min_length,
         max_length=max_length,
-        regex=regex,
+        pattern=pattern,
         multipart_form_part_limit=multipart_form_part_limit,
     )
 
 
 @dataclass(frozen=True)
 class DependencyKwarg:
     """Data container representing a dependency."""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `litestar-2.0.0a7/litestar/partial.py` & `litestar-2.0.0b1/litestar/partial.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/plugins.py` & `litestar-2.0.0b1/litestar/plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 if TYPE_CHECKING:
     from typing_extensions import TypeGuard
 
     from litestar.config.app import AppConfig
     from litestar.dto.interface import DTOInterface
     from litestar.openapi.spec import Schema
-    from litestar.utils.signature import ParsedType
+    from litestar.typing import ParsedType
 
 __all__ = ("SerializationPluginProtocol", "InitPluginProtocol", "OpenAPISchemaPluginProtocol", "PluginProtocol")
 
 ModelT = TypeVar("ModelT")
 DataContainerT = TypeVar("DataContainerT", bound=Union[BaseModel, DataclassProtocol, TypedDict])  # type: ignore[valid-type]
 
 
@@ -61,16 +61,15 @@
 
 @runtime_checkable
 class SerializationPluginProtocol(Protocol):
     """Protocol used to define a serialization plugin for DTOs."""
 
     __slots__ = ()
 
-    @staticmethod
-    def supports_type(parsed_type: ParsedType) -> bool:
+    def supports_type(self, parsed_type: ParsedType) -> bool:
         """Given a value of indeterminate type, determine if this value is supported by the plugin.
 
         Args:
             parsed_type: A parsed type.
 
         Returns:
             Whether the type is supported by the plugin.
```

### Comparing `litestar-2.0.0a7/litestar/response/base.py` & `litestar-2.0.0b1/litestar/response/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,72 +1,215 @@
 from __future__ import annotations
 
-from functools import partial
-from itertools import chain
 from typing import TYPE_CHECKING, Any, Generic, Literal, Mapping, TypeVar, overload
 
 from litestar.datastructures.cookie import Cookie
 from litestar.datastructures.headers import ETag
 from litestar.enums import MediaType, OpenAPIMediaType
 from litestar.exceptions import ImproperlyConfiguredException
-from litestar.serialization import DEFAULT_TYPE_ENCODERS, default_serializer, encode_json, encode_msgpack
+from litestar.serialization import default_serializer, encode_json, encode_msgpack, get_serializer
 from litestar.status_codes import HTTP_200_OK, HTTP_204_NO_CONTENT, HTTP_304_NOT_MODIFIED
-from litestar.utils.helpers import get_enum_string_value
-
-__all__ = ("Response",)
-
+from litestar.utils.helpers import encode_headers, filter_cookies, get_enum_string_value
 
 if TYPE_CHECKING:
+    from typing import Optional
+
+    from litestar.app import Litestar
     from litestar.background_tasks import BackgroundTask, BackgroundTasks
+    from litestar.connection import Request
     from litestar.types import (
         HTTPResponseBodyEvent,
         HTTPResponseStartEvent,
         Receive,
         ResponseCookies,
         ResponseHeaders,
         Scope,
         Send,
         Serializer,
         TypeEncodersMap,
     )
 
+__all__ = ("ASGIResponse", "Response")
+
 T = TypeVar("T")
 
 
+class ASGIResponse:
+    """A low-level ASGI response class."""
+
+    __slots__ = (
+        "background",
+        "body",
+        "content_length",
+        "encoded_headers",
+        "encoding",
+        "is_head_response",
+        "status_code",
+    )
+
+    def __init__(
+        self,
+        *,
+        background: BackgroundTask | BackgroundTasks | None = None,
+        body: bytes | str = b"",
+        content_length: int | None = None,
+        cookies: list[Cookie] | None = None,
+        encoded_headers: list[tuple[bytes, bytes]] | None = None,
+        encoding: str = "utf-8",
+        headers: dict[str, Any] | None = None,
+        is_head_response: bool = False,
+        media_type: MediaType | str | None = None,
+        status_code: int | None = None,
+    ) -> None:
+        """A low-level ASGI response class.
+
+        Args:
+            background: A background task or a list of background tasks to be executed after the response is sent.
+            body: encoded content to send in the response body.
+            content_length: The response content length.
+            cookies: The response cookies.
+            encoded_headers: The response headers.
+            encoding: The response encoding.
+            headers: The response headers.
+            is_head_response: A boolean indicating if the response is a HEAD response.
+            media_type: The response media type.
+            status_code: The response status code.
+        """
+        body = body.encode() if isinstance(body, str) else body
+        status_code = status_code or HTTP_200_OK
+        cookies = cookies or []
+        encoded_headers = encoded_headers or []
+        headers = headers or {}
+        media_type = get_enum_string_value(media_type or MediaType.JSON)
+
+        status_allows_body = not (
+            status_code in {HTTP_204_NO_CONTENT, HTTP_304_NOT_MODIFIED} or status_code < HTTP_200_OK
+        )
+
+        if not status_allows_body or is_head_response:
+            if body and body != b"null":
+                raise ImproperlyConfiguredException(
+                    "response content is not supported for HEAD responses and responses with a status code "
+                    "that does not allow content (304, 204, < 200)"
+                )
+            body = b""
+
+        encoded_headers.append(
+            (
+                b"content-type",
+                (f"{media_type}; charset={encoding}" if media_type.startswith("text/") else media_type).encode(
+                    "latin-1"
+                ),
+            ),
+        )
+
+        if content_length is None:
+            content_length = len(body)
+
+        if "content-length" not in headers and content_length:
+            encoded_headers.append((b"content-length", str(content_length).encode("latin-1")))
+
+        self.background = background
+        self.body = body
+        self.content_length = content_length
+        self.encoded_headers = encode_headers(headers.items(), cookies, encoded_headers)
+        self.encoding = encoding
+        self.is_head_response = is_head_response
+        self.status_code = status_code
+
+    async def after_response(self) -> None:
+        """Execute after the response is sent.
+
+        Returns:
+            None
+        """
+        if self.background is not None:
+            await self.background()
+
+    async def start_response(self, send: Send) -> None:
+        """Emit the start event of the response. This event includes the headers and status codes.
+
+        Args:
+            send: The ASGI send function.
+
+        Returns:
+            None
+        """
+        event: HTTPResponseStartEvent = {
+            "type": "http.response.start",
+            "status": self.status_code,
+            "headers": self.encoded_headers,
+        }
+        await send(event)
+
+    async def send_body(self, send: Send, receive: Receive) -> None:
+        """Emit the response body.
+
+        Args:
+            send: The ASGI send function.
+            receive: The ASGI receive function.
+
+        Notes:
+            - Response subclasses should customize this method if there is a need to customize sending data.
+
+        Returns:
+            None
+        """
+        event: HTTPResponseBodyEvent = {"type": "http.response.body", "body": self.body, "more_body": False}
+        await send(event)
+
+    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
+        """ASGI callable of the ``Response``.
+
+        Args:
+            scope: The ASGI connection scope.
+            receive: The ASGI receive function.
+            send: The ASGI send function.
+
+        Returns:
+            None
+        """
+        await self.start_response(send=send)
+
+        if self.is_head_response:
+            event: HTTPResponseBodyEvent = {"type": "http.response.body", "body": b"", "more_body": False}
+            await send(event)
+        else:
+            await self.send_body(send=send, receive=receive)
+
+        await self.after_response()
+
+
 class Response(Generic[T]):
     """Base Litestar HTTP response class, used as the basis for all other response classes."""
 
     __slots__ = (
         "background",
-        "body",
+        "content",
         "cookies",
         "encoding",
         "headers",
-        "is_head_response",
-        "is_text_response",
         "media_type",
-        "status_allows_body",
         "status_code",
-        "raw_headers",
-        "_enc_hook",
+        "response_type_encoders",
     )
 
-    type_encoders: TypeEncodersMap | None = None
+    content: T
+    type_encoders: Optional[TypeEncodersMap] = None  # noqa: UP007
 
     def __init__(
         self,
         content: T,
         *,
-        status_code: int = HTTP_200_OK,
-        media_type: MediaType | OpenAPIMediaType | str = MediaType.JSON,
         background: BackgroundTask | BackgroundTasks | None = None,
-        headers: ResponseHeaders | None = None,
         cookies: ResponseCookies | None = None,
         encoding: str = "utf-8",
-        is_head_response: bool = False,
+        headers: ResponseHeaders | None = None,
+        media_type: MediaType | OpenAPIMediaType | str | None = None,
+        status_code: int | None = None,
         type_encoders: TypeEncodersMap | None = None,
     ) -> None:
         """Initialize the response.
 
         Args:
             content: A value for the response body that will be rendered into bytes string.
             status_code: An HTTP status code.
@@ -74,60 +217,30 @@
             background: A :class:`BackgroundTask <.background_tasks.BackgroundTask>` instance or
                 :class:`BackgroundTasks <.background_tasks.BackgroundTasks>` to execute after the response is finished.
                 Defaults to ``None``.
             headers: A string keyed dictionary of response headers. Header keys are insensitive.
             cookies: A list of :class:`Cookie <.datastructures.Cookie>` instances to be set under the response
                 ``Set-Cookie`` header.
             encoding: The encoding to be used for the response headers.
-            is_head_response: Whether the response should send only the headers ("head" request) or also the content.
             type_encoders: A mapping of types to callables that transform them into types supported for serialization.
         """
+        self.content = content
         self.background = background
         self.cookies: list[Cookie] = (
             [Cookie(key=key, value=value) for key, value in cookies.items()]
             if isinstance(cookies, Mapping)
             else list(cookies or [])
         )
         self.encoding = encoding
         self.headers: dict[str, Any] = (
             dict(headers) if isinstance(headers, Mapping) else {h.name: h.value for h in headers or {}}
         )
-        self.is_head_response = is_head_response
-        self.media_type = get_enum_string_value(media_type) or MediaType.JSON
-        self.status_allows_body = not (
-            status_code in {HTTP_204_NO_CONTENT, HTTP_304_NOT_MODIFIED} or status_code < HTTP_200_OK
-        )
+        self.media_type = media_type
         self.status_code = status_code
-        self._enc_hook = self.get_serializer(type_encoders)
-
-        if not self.status_allows_body or is_head_response:
-            if content:
-                raise ImproperlyConfiguredException(
-                    "response content is not supported for HEAD responses and responses with a status code "
-                    "that does not allow content (304, 204, < 200)"
-                )
-            self.body = b""
-        else:
-            self.body = content if isinstance(content, bytes) else self.render(content)
-
-        self.headers.setdefault(
-            "content-type",
-            f"{self.media_type}; charset={self.encoding}" if self.media_type.startswith("text/") else self.media_type,
-        )
-        self.raw_headers: list[tuple[bytes, bytes]] = []
-
-    @classmethod
-    def get_serializer(cls, type_encoders: TypeEncodersMap | None = None) -> Serializer:
-        """Get the serializer for this response class."""
-
-        type_encoders = {**(cls.type_encoders or {}), **(type_encoders or {})}
-        if type_encoders:
-            return partial(default_serializer, type_encoders={**DEFAULT_TYPE_ENCODERS, **type_encoders})
-
-        return default_serializer
+        self.response_type_encoders = {**(self.type_encoders or {}), **(type_encoders or {})}
 
     @overload
     def set_cookie(self, /, cookie: Cookie) -> None:
         ...
 
     @overload
     def set_cookie(
@@ -183,15 +296,15 @@
                 path=path,
                 samesite=samesite,
                 secure=secure,
                 value=value,
             )
         self.cookies.append(key)
 
-    def set_header(self, key: str, value: str) -> None:
+    def set_header(self, key: str, value: Any) -> None:
         """Set a header on the response.
 
         Args:
             key: Header key.
             value: Header value.
 
         Returns:
@@ -226,132 +339,87 @@
         Returns:
             None.
         """
         cookie = Cookie(key=key, path=path, domain=domain, expires=0, max_age=0)
         self.cookies = [c for c in self.cookies if c != cookie]
         self.cookies.append(cookie)
 
-    def render(self, content: Any) -> bytes:
+    def render(self, content: Any, media_type: str, enc_hook: Serializer = default_serializer) -> bytes:
         """Handle the rendering of content into a bytes string.
 
-        Args:
-            content: A value for the response body that will be rendered into bytes string.
-
         Returns:
             An encoded bytes string
         """
+        if isinstance(content, bytes):
+            return content
+
         try:
-            if self.media_type.startswith("text/") or isinstance(content, str):
-                if not content:
-                    return b""
+            if media_type.startswith("text/") and not content:
+                return b""
 
-                return content.encode(self.encoding)  # type: ignore
+            if isinstance(content, str):
+                return content.encode(self.encoding)
 
-            if self.media_type == MediaType.MESSAGEPACK:
-                return encode_msgpack(content, self._enc_hook)
+            if media_type == MediaType.MESSAGEPACK:
+                return encode_msgpack(content, enc_hook)
 
-            if self.media_type.startswith("application/json"):
-                return encode_json(content, self._enc_hook)
+            if media_type.startswith("application/json"):
+                return encode_json(content, enc_hook)
 
-            raise ImproperlyConfiguredException(f"unsupported media_type {self.media_type} for content {content!r}")
+            raise ImproperlyConfiguredException(f"unsupported media_type {media_type} for content {content!r}")
         except (AttributeError, ValueError, TypeError) as e:
             raise ImproperlyConfiguredException("Unable to serialize response content") from e
 
-    @property
-    def content_length(self) -> int:
-        """Content length of the response if applicable.
-
-        Returns:
-            The content length of the body (e.g. for use in a ``Content-Length`` header).
-            If the response does not have a body, this value is ``None``
-        """
-        if self.status_allows_body:
-            return len(self.body)
-        return 0
-
-    def encode_headers(self) -> list[tuple[bytes, bytes]]:
-        """Encode the response headers as a list of byte tuples.
-
-        Notes:
-            - A ``Content-Length`` header will be added if appropriate and not provided by the user.
-
-        Returns:
-            A list of tuples containing the headers and cookies of the request in a format ready for ASGI transmission.
-        """
-
-        return list(
-            chain(
-                ((k.lower().encode("latin-1"), str(v).encode("latin-1")) for k, v in self.headers.items()),
-                (cookie.to_encoded_header() for cookie in self.cookies),
-                self.raw_headers,
-            )
-        )
-
-    async def after_response(self) -> None:
-        """Execute after the response is sent.
-
-        Returns:
-            None
-        """
-        if self.background is not None:
-            await self.background()
-
-    async def start_response(self, send: Send) -> None:
-        """Emit the start event of the response. This event includes the headers and status codes.
-
-        Args:
-            send: The ASGI send function.
-
-        Returns:
-            None
-        """
-
-        encoded_headers = self.encode_headers()
-
-        content_length = self.content_length
-        if "content-length" not in self.headers and content_length:
-            encoded_headers.append((b"content-length", str(content_length).encode("latin-1")))
-
-        event: HTTPResponseStartEvent = {
-            "type": "http.response.start",
-            "status": self.status_code,
-            "headers": encoded_headers,
-        }
-
-        await send(event)
-
-    async def send_body(self, send: Send, receive: Receive) -> None:
-        """Emit the response body.
+    def to_asgi_response(
+        self,
+        app: Litestar,
+        request: Request,
+        *,
+        background: BackgroundTask | BackgroundTasks | None = None,
+        cookies: list[Cookie] | None = None,
+        encoded_headers: list[tuple[bytes, bytes]] | None = None,
+        headers: dict[str, str] | None = None,
+        is_head_response: bool = False,
+        media_type: MediaType | str | None = None,
+        status_code: int | None = None,
+        type_encoders: TypeEncodersMap | None = None,
+    ) -> ASGIResponse:
+        """Create an ASGIResponse from a Response instance.
 
         Args:
-            send: The ASGI send function.
-            receive: The ASGI receive function.
-
-        Notes:
-            - Response subclasses should customize this method if there is a need to customize sending data.
+            app: The :class:`Litestar <.app.Litestar>` application instance.
+            background: Background task(s) to be executed after the response is sent.
+            cookies: A list of cookies to be set on the response.
+            encoded_headers: A list of already encoded headers.
+            headers: Additional headers to be merged with the response headers. Response headers take precedence.
+            is_head_response: Whether the response is a HEAD response.
+            media_type: Media type for the response. If ``media_type`` is already set on the response, this is ignored.
+            request: The :class:`Request <.connection.Request>` instance.
+            status_code: Status code for the response. If ``status_code`` is already set on the response, this is
+            type_encoders: A dictionary of type encoders to use for encoding the response content.
 
         Returns:
-            None
+            An ASGIResponse instance.
         """
-        event: HTTPResponseBodyEvent = {"type": "http.response.body", "body": self.body, "more_body": False}
-        await send(event)
 
-    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
-        """ASGI callable of the ``Response``.
+        headers = {**headers, **self.headers} if headers is not None else self.headers
+        cookies = self.cookies if cookies is None else filter_cookies(self.cookies, cookies)
 
-        Args:
-            scope: The ASGI connection scope.
-            receive: The ASGI receive function.
-            send: The ASGI send function.
-
-        Returns:
-            None
-        """
-        await self.start_response(send=send)
-
-        if self.is_head_response:
-            event: HTTPResponseBodyEvent = {"type": "http.response.body", "body": b"", "more_body": False}
-            await send(event)
+        if type_encoders:
+            type_encoders = {**type_encoders, **(self.response_type_encoders or {})}
         else:
-            await self.send_body(send=send, receive=receive)
+            type_encoders = self.response_type_encoders
 
-        await self.after_response()
+        media_type = get_enum_string_value(self.media_type or media_type or MediaType.JSON)
+
+        return ASGIResponse(
+            background=self.background or background,
+            body=self.render(self.content, media_type, get_serializer(type_encoders)),
+            content_length=None,
+            cookies=cookies,
+            encoded_headers=encoded_headers or [],
+            encoding=self.encoding,
+            headers=headers,
+            is_head_response=is_head_response,
+            media_type=media_type,
+            status_code=self.status_code or status_code,
+        )
```

### Comparing `litestar-2.0.0a7/litestar/response/file.py` & `litestar-2.0.0b1/litestar/response/file.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,32 +6,48 @@
 from typing import TYPE_CHECKING, Any, AsyncGenerator, Coroutine, Literal, cast
 from urllib.parse import quote
 from zlib import adler32
 
 from litestar.constants import ONE_MEGABYTE
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.file_system import BaseLocalFileSystem, FileSystemAdapter
-from litestar.response.streaming import StreamingResponse
-from litestar.status_codes import HTTP_200_OK
-
-__all__ = ("FileResponse", "async_file_iterator", "create_etag_for_file")
-
+from litestar.response.base import Response
+from litestar.response.streaming import ASGIStreamingResponse
+from litestar.utils.helpers import filter_cookies, get_enum_string_value
 
 if TYPE_CHECKING:
     from os import PathLike
     from os import stat_result as stat_result_type
 
     from anyio import Path
 
+    from litestar.app import Litestar
     from litestar.background_tasks import BackgroundTask, BackgroundTasks
+    from litestar.connection import Request
+    from litestar.datastructures.cookie import Cookie
     from litestar.datastructures.headers import ETag
     from litestar.enums import MediaType
-    from litestar.types import HTTPResponseBodyEvent, PathType, Receive, ResponseCookies, Send
+    from litestar.types import (
+        HTTPResponseBodyEvent,
+        PathType,
+        Receive,
+        ResponseCookies,
+        ResponseHeaders,
+        Send,
+        TypeEncodersMap,
+    )
     from litestar.types.file_types import FileInfo, FileSystemProtocol
 
+__all__ = (
+    "ASGIFileResponse",
+    "File",
+    "async_file_iterator",
+    "create_etag_for_file",
+)
+
 # brotli not supported in 'mimetypes.encodings_map' until py 3.9.
 encodings_map[".br"] = "br"
 
 
 async def async_file_iterator(
     file_path: PathType, chunk_size: int, adapter: FileSystemAdapter
 ) -> AsyncGenerator[bytes, None]:
@@ -60,134 +76,90 @@
     Returns:
         An etag.
     """
     check = adler32(str(path).encode("utf-8")) & 0xFFFFFFFF
     return f'"{modified_time}-{file_size}-{check}"'
 
 
-class FileResponse(StreamingResponse):
-    """A response, streaming a file as response body."""
-
-    __slots__ = (
-        "chunk_size",
-        "content_disposition_type",
-        "etag",
-        "file_path",
-        "filename",
-        "adapter",
-        "file_info",
-    )
+class ASGIFileResponse(ASGIStreamingResponse):
+    """A low-level ASGI response, streaming a file as response body."""
 
     def __init__(
         self,
-        path: str | PathLike | Path,
         *,
-        background: BackgroundTask | BackgroundTasks | None = None,
         chunk_size: int = ONE_MEGABYTE,
         content_disposition_type: Literal["attachment", "inline"] = "attachment",
-        cookies: ResponseCookies | None = None,
-        encoding: str = "utf-8",
+        encoded_headers: list[tuple[bytes, bytes]] | None = None,
         etag: ETag | None = None,
+        file_info: FileInfo | Coroutine[None, None, FileInfo] | None = None,
+        file_path: str | PathLike | Path,
         file_system: FileSystemProtocol | None = None,
-        filename: str | None = None,
-        file_info: FileInfo | None = None,
-        headers: dict[str, Any] | None = None,
-        is_head_response: bool = False,
-        media_type: Literal[MediaType.TEXT] | str | None = None,
+        filename: str = "",
+        headers: dict[str, str] | None = None,
+        media_type: MediaType | str | None = None,
         stat_result: stat_result_type | None = None,
-        status_code: int = HTTP_200_OK,
+        **kwargs: Any,
     ) -> None:
-        """Initialize ``FileResponse``
-
-        Notes:
-            - This class extends the :class:`StreamingResponse <.response.StreamingResponse>` class.
+        """A low-level ASGI response, streaming a file as response body.
 
         Args:
-            path: A file path in one of the supported formats.
-            status_code: An HTTP status code.
-            media_type: A value for the response ``Content-Type`` header. If not provided, the value will be either
-                derived from the filename if provided and supported by the stdlib, or will default to
-                ``application/octet-stream``.
-            background: A :class:`BackgroundTask <.background_tasks.BackgroundTask>` instance or
-                :class:`BackgroundTasks <.background_tasks.BackgroundTasks>` to execute after the response is finished.
-                Defaults to None.
-            headers: A string keyed dictionary of response headers. Header keys are insensitive.
-            cookies: A list of :class:`Cookie <.datastructures.Cookie>` instances to be set under the response
-                ``Set-Cookie`` header.
-            encoding: The encoding to be used for the response headers.
-            is_head_response: Whether the response should send only the headers ("head" request) or also the content.
-            filename: An optional filename to set in the header.
-            stat_result: An optional result of calling :func:os.stat:. If not provided, this will be done by the
-                response constructor.
-            chunk_size: The chunk sizes to use when streaming the file. Defaults to 1MB.
+            chunk_size: The chunk size to use.
             content_disposition_type: The type of the ``Content-Disposition``. Either ``inline`` or ``attachment``.
-            etag: An optional :class:`ETag <.datastructures.ETag>` instance. If not provided, an etag will be
-                generated.
-            file_system: An implementation of the :class:`FileSystemProtocol <.types.FileSystemProtocol>`. If provided
-                it will be used to load the file.
-            file_info: The output of calling :meth:`file_system.info <types.FileSystemProtocol.info>`, equivalent to
-                providing an :class:`os.stat_result`.
+            encoded_headers: A list of encoded headers.
+            etag: An etag.
+            file_info: A file info.
+            file_path: A path to a file.
+            file_system: A file system adapter.
+            filename: The name of the file.
+            headers: A dictionary of headers.
+            media_type: The media type of the file.
+            stat_result: A stat result.
+            **kwargs: Additional keyword arguments, propagated to :class:`ASGIResponse <.response.base.ASGIResponse>`.
         """
+        encoded_headers = encoded_headers or []
+        headers = headers or {}
+        headers.pop("content-length", None)
+        headers.pop("etag", None)
+        headers.pop("last-modified", None)
+
         if not media_type:
             mimetype, content_encoding = guess_type(filename) if filename else (None, None)
             media_type = mimetype or "application/octet-stream"
             if content_encoding is not None:
-                headers = headers or {}
                 headers.update({"content-encoding": content_encoding})
 
-        self.chunk_size = chunk_size
-        self.content_disposition_type = content_disposition_type
-        self.etag = etag
-        self.file_path = path
-        self.filename = filename or ""
+        quoted_filename = quote(filename)
+        is_utf8 = quoted_filename == filename
+        if is_utf8:
+            content_disposition = f'{content_disposition_type}; filename="{filename}"'
+        else:
+            content_disposition = f"{content_disposition_type}; filename*=utf-8''{quoted_filename}"
+
+        encoded_headers.append((b"content-disposition", content_disposition.encode("ascii")))
+
         self.adapter = FileSystemAdapter(file_system or BaseLocalFileSystem())
 
         super().__init__(
-            content=async_file_iterator(file_path=path, chunk_size=chunk_size, adapter=self.adapter),
-            status_code=status_code,
-            media_type=media_type,
-            background=background,
+            iterator=async_file_iterator(file_path=file_path, chunk_size=chunk_size, adapter=self.adapter),
+            encoded_headers=encoded_headers,
             headers=headers,
-            cookies=cookies,
-            encoding=encoding,
-            is_head_response=is_head_response,
+            media_type=media_type,
+            **kwargs,
         )
+        self.chunk_size = chunk_size
+        self.etag = etag
+        self.file_path = file_path
 
         if file_info:
             self.file_info: FileInfo | Coroutine[Any, Any, FileInfo] = file_info
         elif stat_result:
-            self.file_info = self.adapter.parse_stat_result(result=stat_result, path=path)
+            self.file_info = self.adapter.parse_stat_result(result=stat_result, path=file_path)
         else:
             self.file_info = self.adapter.info(self.file_path)
 
-    @property
-    def content_disposition(self) -> str:
-        """Content disposition.
-
-        Returns:
-            A value for the ``Content-Disposition`` header.
-        """
-        quoted_filename = quote(self.filename)
-        is_utf8 = quoted_filename == self.filename
-        if is_utf8:
-            return f'{self.content_disposition_type}; filename="{self.filename}"'
-        return f"{self.content_disposition_type}; filename*=utf-8''{quoted_filename}"
-
-    @property
-    def content_length(self) -> int:
-        """Content length of the response if applicable.
-
-        Returns:
-            Returns the value of :attr:`stat_result.st_size <os.stat_result.st_size>` to populate the ``Content-Length``
-                header.
-        """
-        if isinstance(self.file_info, dict):
-            return self.file_info["size"]
-        return 0
-
     async def send_body(self, send: Send, receive: Receive) -> None:
         """Emit a stream of events correlating with the response body.
 
         Args:
             send: The ASGI send function.
             receive: The ASGI receive function.
 
@@ -221,15 +193,166 @@
             )
         except FileNotFoundError as e:
             raise ImproperlyConfiguredException(f"{self.file_path} does not exist") from e
 
         if fs_info["type"] != "file":
             raise ImproperlyConfiguredException(f"{self.file_path} is not a file")
 
-        self.set_header("last-modified", formatdate(fs_info["mtime"], usegmt=True))
-        self.set_header("content-disposition", self.content_disposition)
-        self.set_etag(
-            self.etag
-            or create_etag_for_file(path=self.file_path, modified_time=fs_info["mtime"], file_size=fs_info["size"])
-        )
+        self.content_length = fs_info["size"]
+        self.encoded_headers.append((b"content-length", str(self.content_length).encode("ascii")))
+
+        self.encoded_headers.append((b"last-modified", formatdate(fs_info["mtime"], usegmt=True).encode("ascii")))
+
+        if self.etag:
+            self.encoded_headers.append((b"etag", self.etag.to_header().encode("ascii")))
+        else:
+            etag = create_etag_for_file(path=self.file_path, modified_time=fs_info["mtime"], file_size=fs_info["size"])
+            self.encoded_headers.append((b"etag", etag.encode("ascii")))
 
         await super().start_response(send=send)
+
+
+class File(Response):
+    """A response, streaming a file as response body."""
+
+    __slots__ = (
+        "chunk_size",
+        "content_disposition_type",
+        "etag",
+        "file_path",
+        "file_system",
+        "filename",
+        "file_info",
+        "stat_result",
+    )
+
+    def __init__(
+        self,
+        path: str | PathLike | Path,
+        *,
+        background: BackgroundTask | BackgroundTasks | None = None,
+        chunk_size: int = ONE_MEGABYTE,
+        content_disposition_type: Literal["attachment", "inline"] = "attachment",
+        cookies: ResponseCookies | None = None,
+        encoding: str = "utf-8",
+        etag: ETag | None = None,
+        file_info: FileInfo | Coroutine[Any, Any, FileInfo] | None = None,
+        file_system: FileSystemProtocol | None = None,
+        filename: str | None = None,
+        headers: ResponseHeaders | None = None,
+        media_type: Literal[MediaType.TEXT] | str | None = None,
+        stat_result: stat_result_type | None = None,
+        status_code: int | None = None,
+    ) -> None:
+        """Initialize ``File``
+
+        Notes:
+            - This class extends the :class:`Stream <.response.Stream>` class.
+
+        Args:
+            path: A file path in one of the supported formats.
+            background: A :class:`BackgroundTask <.background_tasks.BackgroundTask>` instance or
+                :class:`BackgroundTasks <.background_tasks.BackgroundTasks>` to execute after the response is finished.
+                Defaults to None.
+            chunk_size: The chunk sizes to use when streaming the file. Defaults to 1MB.
+            content_disposition_type: The type of the ``Content-Disposition``. Either ``inline`` or ``attachment``.
+            cookies: A list of :class:`Cookie <.datastructures.Cookie>` instances to be set under the response
+                ``Set-Cookie`` header.
+            encoding: The encoding to be used for the response headers.
+            etag: An optional :class:`ETag <.datastructures.ETag>` instance. If not provided, an etag will be
+                generated.
+            file_info: The output of calling :meth:`file_system.info <types.FileSystemProtocol.info>`, equivalent to
+                providing an :class:`os.stat_result`.
+            file_system: An implementation of the :class:`FileSystemProtocol <.types.FileSystemProtocol>`. If provided
+                it will be used to load the file.
+            filename: An optional filename to set in the header.
+            headers: A string keyed dictionary of response headers. Header keys are insensitive.
+            media_type: A value for the response ``Content-Type`` header. If not provided, the value will be either
+                derived from the filename if provided and supported by the stdlib, or will default to
+                ``application/octet-stream``.
+            stat_result: An optional result of calling :func:os.stat:. If not provided, this will be done by the
+                response constructor.
+            status_code: An HTTP status code.
+        """
+
+        if file_system is not None and not (
+            callable(getattr(file_system, "info", None)) and callable(getattr(file_system, "open", None))
+        ):
+            raise ImproperlyConfiguredException("file_system must adhere to the FileSystemProtocol type")
+
+        self.chunk_size = chunk_size
+        self.content_disposition_type = content_disposition_type
+        self.etag = etag
+        self.file_info = file_info
+        self.file_path = path
+        self.file_system = file_system
+        self.filename = filename or ""
+        self.stat_result = stat_result
+
+        super().__init__(
+            content=None,
+            status_code=status_code,
+            media_type=media_type,
+            background=background,
+            headers=headers,
+            cookies=cookies,
+            encoding=encoding,
+        )
+
+    def to_asgi_response(
+        self,
+        app: Litestar,
+        request: Request,
+        *,
+        background: BackgroundTask | BackgroundTasks | None = None,
+        cookies: list[Cookie] | None = None,
+        encoded_headers: list[tuple[bytes, bytes]] | None = None,
+        headers: dict[str, str] | None = None,
+        is_head_response: bool = False,
+        media_type: MediaType | str | None = None,
+        status_code: int | None = None,
+        type_encoders: TypeEncodersMap | None = None,
+    ) -> ASGIFileResponse:
+        """Create an :class:`ASGIFileResponse <litestar.response.file.ASGIFileResponse>` instance.
+
+        Args:
+            app: The :class:`Litestar <.app.Litestar>` application instance.
+            background: Background task(s) to be executed after the response is sent.
+            cookies: A list of cookies to be set on the response.
+            encoded_headers: A list of already encoded headers.
+            headers: Additional headers to be merged with the response headers. Response headers take precedence.
+            is_head_response: Whether the response is a HEAD response.
+            media_type: Media type for the response. If ``media_type`` is already set on the response, this is ignored.
+            request: The :class:`Request <.connection.Request>` instance.
+            status_code: Status code for the response. If ``status_code`` is already set on the response, this is
+            type_encoders: A dictionary of type encoders to use for encoding the response content.
+
+        Returns:
+            A low-level ASGI file response.
+        """
+        headers = {**headers, **self.headers} if headers is not None else self.headers
+        cookies = self.cookies if cookies is None else filter_cookies(self.cookies, cookies)
+
+        media_type = self.media_type or media_type
+        if media_type is not None:
+            media_type = get_enum_string_value(media_type)
+
+        return ASGIFileResponse(
+            background=self.background or background,
+            body=b"",
+            chunk_size=self.chunk_size,
+            content_disposition_type=self.content_disposition_type,  # pyright: ignore
+            content_length=0,
+            cookies=cookies,
+            encoded_headers=encoded_headers or [],
+            encoding=self.encoding,
+            etag=self.etag,
+            file_info=self.file_info,
+            file_path=self.file_path,
+            file_system=self.file_system,
+            filename=self.filename,
+            headers=headers,
+            is_head_response=is_head_response,
+            media_type=media_type,
+            stat_result=self.stat_result,
+            status_code=self.status_code or status_code,
+        )
```

### Comparing `litestar-2.0.0a7/litestar/response/streaming.py` & `litestar-2.0.0b1/litestar/response/streaming.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,49 @@
 from __future__ import annotations
 
 from functools import partial
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    AsyncGenerator,
-    AsyncIterable,
-    AsyncIterator,
-    Union,
-)
+from typing import TYPE_CHECKING, Any, AsyncGenerator, AsyncIterable, AsyncIterator, Callable, Iterable, Iterator, Union
 
 from anyio import CancelScope, create_task_group
 
 from litestar.enums import MediaType
-from litestar.response.base import Response
-from litestar.status_codes import HTTP_200_OK
+from litestar.response.base import ASGIResponse, Response
 from litestar.types.composite_types import StreamType
+from litestar.utils.helpers import filter_cookies, get_enum_string_value
 from litestar.utils.sync import AsyncIteratorWrapper
 
-__all__ = ("StreamingResponse",)
-
-
 if TYPE_CHECKING:
+    from litestar.app import Litestar
     from litestar.background_tasks import BackgroundTask, BackgroundTasks
+    from litestar.connection import Request
+    from litestar.datastructures.cookie import Cookie
     from litestar.enums import OpenAPIMediaType
-    from litestar.types import HTTPResponseBodyEvent, Receive, ResponseCookies, Send
+    from litestar.types import HTTPResponseBodyEvent, Receive, ResponseCookies, ResponseHeaders, Send, TypeEncodersMap
 
+__all__ = (
+    "ASGIStreamingResponse",
+    "Stream",
+)
 
-class StreamingResponse(Response[StreamType[Union[str, bytes]]]):
-    """An HTTP response that streams the response data as a series of ASGI ``http.response.body`` events."""
+
+class ASGIStreamingResponse(ASGIResponse):
+    """A streaming response."""
 
     __slots__ = ("iterator",)
 
-    def __init__(
-        self,
-        content: StreamType[str | bytes],
-        *,
-        status_code: int = HTTP_200_OK,
-        media_type: MediaType | OpenAPIMediaType | str = MediaType.JSON,
-        background: BackgroundTask | BackgroundTasks | None = None,
-        headers: dict[str, Any] | None = None,
-        cookies: ResponseCookies | None = None,
-        encoding: str = "utf-8",
-        is_head_response: bool = False,
-    ):
-        """Initialize the response.
+    def __init__(self, *, iterator: StreamType, **kwargs: Any):
+        """A low-level ASGI streaming response.
 
         Args:
-            content: A sync or async iterator or iterable.
-            status_code: An HTTP status code.
-            media_type: A value for the response ``Content-Type`` header.
-            background: A :class:`BackgroundTask <.background_tasks.BackgroundTask>` instance or
-                :class:`BackgroundTasks <.background_tasks.BackgroundTasks>` to execute after the response is finished.
-                Defaults to None.
-            headers: A string keyed dictionary of response headers. Header keys are insensitive.
-            cookies: A list of :class:`Cookie <.datastructures.Cookie>` instances to be set under the response
-                ``Set-Cookie`` header.
-            encoding: The encoding to be used for the response headers.
-            is_head_response: Whether the response should send only the headers ("head" request) or also the content.
+            iterator: An async iterator or iterable.
+            **kwargs: Additional keyword arguments propagated to :class:`ASGIResponse <.response.base.ASGIResponse>`.
         """
-        super().__init__(
-            background=background,
-            content=b"",  # type: ignore[arg-type]
-            cookies=cookies,
-            encoding=encoding,
-            headers=headers,
-            media_type=media_type,
-            status_code=status_code,
-            is_head_response=is_head_response,
-        )
+        super().__init__(**kwargs)
         self.iterator: AsyncIterable[str | bytes] | AsyncGenerator[str | bytes, None] = (
-            content if isinstance(content, (AsyncIterable, AsyncIterator)) else AsyncIteratorWrapper(content)
+            iterator if isinstance(iterator, (AsyncIterable, AsyncIterator)) else AsyncIteratorWrapper(iterator)
         )
 
     async def _listen_for_disconnect(self, cancel_scope: CancelScope, receive: Receive) -> None:
         """Listen for a cancellation message, and if received - call cancel on the cancel scope.
 
         Args:
             cancel_scope: A task group cancel scope instance.
@@ -121,7 +90,104 @@
         Returns:
             None
         """
 
         async with create_task_group() as task_group:
             task_group.start_soon(partial(self._stream, send))
             await self._listen_for_disconnect(cancel_scope=task_group.cancel_scope, receive=receive)
+
+
+class Stream(Response[StreamType[Union[str, bytes]]]):
+    """An HTTP response that streams the response data as a series of ASGI ``http.response.body`` events."""
+
+    __slots__ = ("iterator",)
+
+    def __init__(
+        self,
+        content: StreamType[str | bytes] | Callable[[], StreamType[str | bytes]],
+        *,
+        background: BackgroundTask | BackgroundTasks | None = None,
+        cookies: ResponseCookies | None = None,
+        encoding: str = "utf-8",
+        headers: ResponseHeaders | None = None,
+        media_type: MediaType | OpenAPIMediaType | str | None = None,
+        status_code: int | None = None,
+    ):
+        """Initialize the response.
+
+        Args:
+            content: A sync or async iterator or iterable.
+            background: A :class:`BackgroundTask <.background_tasks.BackgroundTask>` instance or
+                :class:`BackgroundTasks <.background_tasks.BackgroundTasks>` to execute after the response is finished.
+                Defaults to None.
+            cookies: A list of :class:`Cookie <.datastructures.Cookie>` instances to be set under the response
+                ``Set-Cookie`` header.
+            encoding: The encoding to be used for the response headers.
+            headers: A string keyed dictionary of response headers. Header keys are insensitive.
+            media_type: A value for the response ``Content-Type`` header.
+            status_code: An HTTP status code.
+        """
+        super().__init__(
+            background=background,
+            content=b"",  # type: ignore[arg-type]
+            cookies=cookies,
+            encoding=encoding,
+            headers=headers,
+            media_type=media_type,
+            status_code=status_code,
+        )
+        self.iterator = content
+
+    def to_asgi_response(
+        self,
+        app: Litestar,
+        request: Request,
+        *,
+        background: BackgroundTask | BackgroundTasks | None = None,
+        cookies: list[Cookie] | None = None,
+        encoded_headers: list[tuple[bytes, bytes]] | None = None,
+        headers: dict[str, str] | None = None,
+        is_head_response: bool = False,
+        media_type: MediaType | str | None = None,
+        status_code: int | None = None,
+        type_encoders: TypeEncodersMap | None = None,
+    ) -> ASGIResponse:
+        """Create an ASGIStreamingResponse from a StremaingResponse instance.
+
+        Args:
+            app: The :class:`Litestar <.app.Litestar>` application instance.
+            background: Background task(s) to be executed after the response is sent.
+            cookies: A list of cookies to be set on the response.
+            encoded_headers: A list of already encoded headers.
+            headers: Additional headers to be merged with the response headers. Response headers take precedence.
+            is_head_response: Whether the response is a HEAD response.
+            media_type: Media type for the response. If ``media_type`` is already set on the response, this is ignored.
+            request: The :class:`Request <.connection.Request>` instance.
+            status_code: Status code for the response. If ``status_code`` is already set on the response, this is
+            type_encoders: A dictionary of type encoders to use for encoding the response content.
+
+        Returns:
+            An ASGIStreamingResponse instance.
+        """
+
+        headers = {**headers, **self.headers} if headers is not None else self.headers
+        cookies = self.cookies if cookies is None else filter_cookies(self.cookies, cookies)
+
+        media_type = get_enum_string_value(media_type or self.media_type or MediaType.JSON)
+
+        iterator = self.iterator
+        if not isinstance(iterator, (Iterable, Iterator, AsyncIterable, AsyncIterator)) and callable(iterator):
+            iterator = iterator()
+
+        return ASGIStreamingResponse(
+            background=self.background or background,
+            body=b"",
+            content_length=0,
+            cookies=cookies,
+            encoded_headers=encoded_headers or [],
+            encoding=self.encoding,
+            headers=headers,
+            is_head_response=is_head_response,
+            iterator=iterator,
+            media_type=media_type,
+            status_code=self.status_code or status_code,
+        )
```

### Comparing `litestar-2.0.0a7/litestar/router.py` & `litestar-2.0.0b1/litestar/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from collections import defaultdict
 from copy import copy
-from typing import TYPE_CHECKING, Any, DefaultDict, Mapping, Sequence, cast
+from typing import TYPE_CHECKING, Any, Mapping, Sequence, cast
 
 from litestar._layers.utils import narrow_response_cookies, narrow_response_headers
 from litestar.controller import Controller
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.handlers.asgi_handlers import ASGIRouteHandler
 from litestar.handlers.http_handlers import HTTPRouteHandler
 from litestar.handlers.websocket_handlers import WebsocketListener, WebsocketRouteHandler
@@ -265,15 +265,15 @@
                 return {path: {http_method: copied_value for http_method in value.http_methods} for path in value.paths}
 
             return {
                 path: {"websocket" if isinstance(value, WebsocketRouteHandler) else "asgi": copied_value}
                 for path in value.paths
             }
 
-        handlers_map: DefaultDict[str, RouteHandlerMapItem] = defaultdict(dict)
+        handlers_map: defaultdict[str, RouteHandlerMapItem] = defaultdict(dict)
         for route_handler in value.get_route_handlers():
             for handler_path in route_handler.paths:
                 path = join_paths([value.path, handler_path]) if handler_path else value.path
                 if isinstance(route_handler, HTTPRouteHandler):
                     for http_method in route_handler.http_methods:
                         handlers_map[path][http_method] = route_handler
                 else:
@@ -286,15 +286,15 @@
     def _validate_registration_value(self, value: ControllerRouterHandler) -> Controller | RouteHandlerType | Router:
         """Ensure values passed to the register method are supported."""
         if is_class_and_subclass(value, Controller):
             return value(owner=self)
 
         # this narrows down to an ABC, but we assume a non-abstract subclass of the ABC superclass
         if is_class_and_subclass(value, WebsocketListener):  # type: ignore[type-abstract]
-            return value()._handler  # pyright: ignore
+            return value(owner=self).to_handler()  # pyright: ignore
 
         if isinstance(value, Router):
             if value.owner:
                 raise ImproperlyConfiguredException(f"Router with path {value.path} has already been registered")
             if value is self:
                 raise ImproperlyConfiguredException("Cannot register a router on itself")
```

### Comparing `litestar-2.0.0a7/litestar/routes/asgi.py` & `litestar-2.0.0b1/litestar/routes/asgi.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         path: str,
         route_handler: ASGIRouteHandler,
     ) -> None:
         """Initialize the route.
 
         Args:
             path: The path for the route.
-            route_handler: An instance of :ref:`ASGIRouteHandler <litestar.handlers.asgi_handlers.ASGIRouteHandler>`.
+            route_handler: An instance of :class:`~.handlers.ASGIRouteHandler`.
         """
         self.route_handler = route_handler
         super().__init__(
             path=path,
             scope_type=ScopeType.ASGI,
             handler_names=[unwrap_partial(route_handler.handler_name)],
         )
```

### Comparing `litestar-2.0.0a7/litestar/routes/base.py` & `litestar-2.0.0b1/litestar/routes/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/routes/http.py` & `litestar-2.0.0b1/litestar/routes/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     from litestar._kwargs import KwargsModel
     from litestar._kwargs.cleanup import DependencyCleanupGroup
     from litestar.connection import Request
     from litestar.types import ASGIApp, HTTPScope, Method, Receive, Scope, Send
 
 
 class HTTPRoute(BaseRoute):
-    """An HTTP route, capable of handling multiple ``HTTPRouteHandler``s."""
+    """An HTTP route, capable of handling multiple ``HTTPRouteHandler``\\ s."""  # noqa: D301
 
     __slots__ = (
         "route_handler_map",
         "route_handlers",
     )
 
     def __init__(
@@ -35,15 +35,15 @@
         path: str,
         route_handlers: list[HTTPRouteHandler],
     ) -> None:
         """Initialize ``HTTPRoute``.
 
         Args:
             path: The path for the route.
-            route_handlers: A list of :class:`HTTPRouteHandler <litestar.handlers.http_handlers.HTTPRouteHandler>`.
+            route_handlers: A list of :class:`~.handlers.HTTPRouteHandler`.
         """
         methods = list(chain.from_iterable([route_handler.http_methods for route_handler in route_handlers]))
         if "OPTIONS" not in methods:
             methods.append("OPTIONS")
             route_handlers.append(self.create_options_handler(path))
 
         self.route_handlers = route_handlers
@@ -210,15 +210,15 @@
 
     @staticmethod
     async def _get_cached_response(request: Request, route_handler: HTTPRouteHandler) -> ASGIApp | None:
         """Retrieve and un-pickle the cached response, if existing.
 
         Args:
             request: The :class:`Request <litestar.connection.Request>` instance
-            route_handler: The :class:`HTTPRouteHandler <litestar.handlers.http_handlers.HTTPRouteHandler>` instance
+            route_handler: The :class:`~.handlers.HTTPRouteHandler` instance
 
         Returns:
             A cached response instance, if existing.
         """
 
         cache_config = request.app.response_cache_config
         cache_key = (route_handler.cache_key_builder or cache_config.key_builder)(request)
```

### Comparing `litestar-2.0.0a7/litestar/routes/websocket.py` & `litestar-2.0.0b1/litestar/routes/websocket.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         path: str,
         route_handler: WebsocketRouteHandler,
     ) -> None:
         """Initialize the route.
 
         Args:
             path: The path for the route.
-            route_handler: An instance of :class:`WebsocketRouteHandler <litestar.handlers.websocket_handlers.WebsocketRouteHandler>`.
+            route_handler: An instance of :class:`~.handlers.WebsocketRouteHandler`.
         """
         self.route_handler = route_handler
         self.handler_parameter_model: KwargsModel | None = None
 
         super().__init__(
             path=path,
             scope_type=ScopeType.WEBSOCKET,
```

### Comparing `litestar-2.0.0a7/litestar/security/base.py` & `litestar-2.0.0b1/litestar/security/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/security/session_auth/auth.py` & `litestar-2.0.0b1/litestar/security/session_auth/auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/security/session_auth/middleware.py` & `litestar-2.0.0b1/litestar/security/session_auth/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/serialization.py` & `litestar-2.0.0b1/litestar/serialization.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from collections import deque
 from decimal import Decimal
+from functools import partial
 from ipaddress import (
     IPv4Address,
     IPv4Interface,
     IPv4Network,
     IPv6Address,
     IPv6Interface,
     IPv6Network,
@@ -25,27 +26,28 @@
     StrictBool,
 )
 from pydantic.color import Color
 from pydantic.json import decimal_encoder
 
 from litestar.enums import MediaType
 from litestar.exceptions import SerializationException
-from litestar.types import Empty
+from litestar.types import Empty, Serializer
 
 if TYPE_CHECKING:
     from litestar.types import TypeEncodersMap
 
 __all__ = (
     "dec_hook",
     "decode_json",
     "decode_media_type",
     "decode_msgpack",
     "default_serializer",
     "encode_json",
     "encode_msgpack",
+    "get_serializer",
 )
 
 T = TypeVar("T")
 
 
 def _enc_base_model(model: BaseModel) -> Any:
     return model.dict()
@@ -267,7 +269,16 @@
     if media_type == MediaType.JSON:
         return decode_json(raw, type_=type_)
 
     if media_type == MediaType.MESSAGEPACK:
         return decode_msgpack(raw, type_=type_)
 
     raise SerializationException(f"Unsupported media type: '{media_type}'")
+
+
+def get_serializer(type_encoders: TypeEncodersMap | None = None) -> Serializer:
+    """Get the serializer for the given type encoders."""
+
+    if type_encoders:
+        return partial(default_serializer, type_encoders={**DEFAULT_TYPE_ENCODERS, **type_encoders})
+
+    return default_serializer
```

### Comparing `litestar-2.0.0a7/litestar/static_files/base.py` & `litestar-2.0.0b1/litestar/static_files/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os.path import commonpath
 from pathlib import Path
 from typing import TYPE_CHECKING, Literal, Sequence
 
 from litestar.enums import ScopeType
 from litestar.exceptions import MethodNotAllowedException, NotFoundException
 from litestar.file_system import FileSystemAdapter
-from litestar.response import FileResponse
+from litestar.response.file import ASGIFileResponse
 from litestar.status_codes import HTTP_404_NOT_FOUND
 
 __all__ = ("StaticFiles",)
 
 
 if TYPE_CHECKING:
     from litestar.types import Receive, Scope, Send
@@ -94,36 +94,36 @@
             filename = "index.html"
             resolved_path, fs_info = await self.get_fs_info(
                 directories=self.directories,
                 file_path=Path(resolved_path or joined_path) / filename,
             )
 
         if fs_info and fs_info["type"] == "file":
-            await FileResponse(
-                path=resolved_path or joined_path,
+            await ASGIFileResponse(
+                file_path=resolved_path or joined_path,
                 file_info=fs_info,
                 file_system=self.adapter.file_system,
                 filename=filename,
-                is_head_response=scope["method"] == "HEAD",
                 content_disposition_type=content_disposition_type,
+                is_head_response=scope["method"] == "HEAD",
             )(scope, receive, send)
             return
 
         if self.is_html_mode:
             filename = "404.html"
             resolved_path, fs_info = await self.get_fs_info(directories=self.directories, file_path=filename)
 
             if fs_info and fs_info["type"] == "file":
-                await FileResponse(
-                    path=resolved_path or joined_path,
+                await ASGIFileResponse(
+                    file_path=resolved_path or joined_path,
                     file_info=fs_info,
                     file_system=self.adapter.file_system,
                     filename=filename,
-                    is_head_response=scope["method"] == "HEAD",
                     status_code=HTTP_404_NOT_FOUND,
                     content_disposition_type=content_disposition_type,
+                    is_head_response=scope["method"] == "HEAD",
                 )(scope, receive, send)
                 return
 
         raise NotFoundException(
             f"no file or directory match the path {resolved_path or joined_path} was found"
         )  # pragma: no cover
```

### Comparing `litestar-2.0.0a7/litestar/static_files/config.py` & `litestar-2.0.0b1/litestar/static_files/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/status_codes.py` & `litestar-2.0.0b1/litestar/status_codes.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/stores/base.py` & `litestar-2.0.0b1/litestar/stores/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/stores/file.py` & `litestar-2.0.0b1/litestar/stores/file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/stores/memory.py` & `litestar-2.0.0b1/litestar/stores/memory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/stores/redis.py` & `litestar-2.0.0b1/litestar/stores/redis.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/stores/registry.py` & `litestar-2.0.0b1/litestar/stores/registry.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/template/base.py` & `litestar-2.0.0b1/litestar/template/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Callable, Protocol, TypeVar, runtime_checkable
-
-from typing_extensions import TypedDict
+from typing import TYPE_CHECKING, Any, Callable, Protocol, TypedDict, TypeVar, runtime_checkable
 
 __all__ = (
     "TemplateContext",
     "TemplateEngineProtocol",
     "TemplateProtocol",
     "csrf_token",
     "url_for",
```

### Comparing `litestar-2.0.0a7/litestar/template/config.py` & `litestar-2.0.0b1/litestar/template/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/testing/__init__.py` & `litestar-2.0.0b1/litestar/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/testing/client/__init__.py` & `litestar-2.0.0b1/litestar/testing/client/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/testing/client/async_client.py` & `litestar-2.0.0b1/litestar/testing/client/async_client.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/testing/client/base.py` & `litestar-2.0.0b1/litestar/testing/client/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/testing/client/sync_client.py` & `litestar-2.0.0b1/litestar/testing/client/sync_client.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/testing/helpers.py` & `litestar-2.0.0b1/litestar/testing/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,16 @@
     on_shutdown: OptionalSequence[LifespanHook] = None,
     on_startup: OptionalSequence[LifespanHook] = None,
     openapi_config: OpenAPIConfig | None = DEFAULT_OPENAPI_CONFIG,
     opt: Mapping[str, Any] | None = None,
     parameters: ParametersMap | None = None,
     plugins: OptionalSequence[PluginProtocol] = None,
     lifespan: list[Callable[[Litestar], AbstractAsyncContextManager] | AbstractAsyncContextManager] | None = None,
-    preferred_validation_backend: Literal["pydantic", "attrs"] | None = None,
     raise_server_exceptions: bool = True,
+    pdb_on_exception: bool | None = None,
     request_class: type[Request] | None = None,
     response_cache_config: ResponseCacheConfig | None = None,
     response_class: ResponseType | None = None,
     response_cookies: ResponseCookies | None = None,
     response_headers: OptionalSequence[ResponseHeader] = None,
     return_dto: type[DTOInterface] | None | EmptyType = Empty,
     root_path: str = "",
@@ -102,14 +102,15 @@
     state: State | None = None,
     static_files_config: OptionalSequence[StaticFilesConfig] = None,
     stores: StoreRegistry | dict[str, Store] | None = None,
     tags: Sequence[str] | None = None,
     template_config: TemplateConfig | None = None,
     type_encoders: TypeEncodersMap | None = None,
     websocket_class: type[WebSocket] | None = None,
+    _preferred_validation_backend: Literal["pydantic", "attrs"] | None = None,
 ) -> TestClient[Litestar]:
     """Create a Litestar app instance and initializes it.
 
     :class:`TestClient <litestar.testing.TestClient>` with it.
 
     Notes:
         - This function should be called as a context manager to ensure async startup and shutdown are
@@ -127,15 +128,14 @@
 
             def test_my_handler() -> None:
                 with create_test_client(my_handler) as client:
                     response == client.get("/some-path")
                     assert response.json() == {"hello": "world"}
 
     Args:
-        preferred_validation_backend:
         route_handlers: A single handler or a sequence of route handlers, which can include instances of
             :class:`Router <litestar.router.Router>`, subclasses of :class:`Controller <.controller.Controller>` or
             any function decorated by the route handler decorators.
         backend: The async backend to use, options are "asyncio" or "trio".
         backend_options: ``anyio`` options.
         base_url: URL scheme and domain for test request paths, e.g. ``http://testserver``.
         raise_server_exceptions: Flag for underlying the test client to raise server exceptions instead of wrapping them
@@ -191,16 +191,16 @@
             application startup.
         openapi_config: Defaults to :attr:`DEFAULT_OPENAPI_CONFIG`
         opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
             wherever you have access to :class:`Request <litestar.connection.request.Request>` or
             :class:`ASGI Scope <.types.Scope>`.
         parameters: A mapping of :class:`Parameter <.params.Parameter>` definitions available to all application
             paths.
+        pdb_on_exception: Drop into the PDB when an exception occurs.
         plugins: Sequence of plugins.
-        preferred_validation_backend: Validation backend to use, if multiple are installed.
         request_class: An optional subclass of :class:`Request <.connection.Request>` to use for http connections.
         response_class: A custom subclass of :class:`Response <.response.Response>` to be used as the app's default
             response.
         response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>`.
         response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
         response_cache_config: Configures caching behavior of the application.
         return_dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for serializing
@@ -257,16 +257,16 @@
         multipart_form_part_limit=multipart_form_part_limit,
         on_app_init=on_app_init,
         on_shutdown=on_shutdown,
         on_startup=on_startup,
         openapi_config=openapi_config,
         opt=opt,
         parameters=parameters,
+        pdb_on_exception=pdb_on_exception,
         plugins=plugins,
-        preferred_validation_backend=preferred_validation_backend,
         request_class=request_class,
         response_cache_config=response_cache_config,
         response_class=response_class,
         response_cookies=response_cookies,
         response_headers=response_headers,
         return_dto=return_dto,
         route_handlers=route_handlers,
@@ -275,14 +275,15 @@
         state=state,
         static_files_config=static_files_config,
         stores=stores,
         tags=tags,
         template_config=template_config,
         type_encoders=type_encoders,
         websocket_class=websocket_class,
+        _preferred_validation_backend=_preferred_validation_backend,
     )
 
     return TestClient[Litestar](
         app=app,
         backend=backend,
         backend_options=backend_options,
         base_url=base_url,
@@ -322,16 +323,16 @@
     multipart_form_part_limit: int = 1000,
     on_app_init: OptionalSequence[OnAppInitHandler] = None,
     on_shutdown: OptionalSequence[LifespanHook] = None,
     on_startup: OptionalSequence[LifespanHook] = None,
     openapi_config: OpenAPIConfig | None = DEFAULT_OPENAPI_CONFIG,
     opt: Mapping[str, Any] | None = None,
     parameters: ParametersMap | None = None,
+    pdb_on_exception: bool | None = None,
     plugins: OptionalSequence[PluginProtocol] = None,
-    preferred_validation_backend: Literal["pydantic", "attrs"] | None = None,
     raise_server_exceptions: bool = True,
     request_class: type[Request] | None = None,
     response_cache_config: ResponseCacheConfig | None = None,
     response_class: ResponseType | None = None,
     response_cookies: ResponseCookies | None = None,
     response_headers: OptionalSequence[ResponseHeader] = None,
     return_dto: type[DTOInterface] | None | EmptyType = Empty,
@@ -342,14 +343,15 @@
     state: State | None = None,
     static_files_config: OptionalSequence[StaticFilesConfig] = None,
     stores: StoreRegistry | dict[str, Store] | None = None,
     tags: Sequence[str] | None = None,
     template_config: TemplateConfig | None = None,
     type_encoders: TypeEncodersMap | None = None,
     websocket_class: type[WebSocket] | None = None,
+    _preferred_validation_backend: Literal["pydantic", "attrs"] | None = None,
 ) -> AsyncTestClient[Litestar]:
     """Create a Litestar app instance and initializes it.
 
     :class:`TestClient <litestar.testing.TestClient>` with it.
 
     Notes:
         - This function should be called as a context manager to ensure async startup and shutdown are
@@ -430,16 +432,16 @@
             application startup.
         openapi_config: Defaults to :attr:`DEFAULT_OPENAPI_CONFIG`
         opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
             wherever you have access to :class:`Request <litestar.connection.request.Request>` or
             :class:`ASGI Scope <.types.Scope>`.
         parameters: A mapping of :class:`Parameter <.params.Parameter>` definitions available to all application
             paths.
+        pdb_on_exception: Drop into the PDB when an exception occurs.
         plugins: Sequence of plugins.
-        preferred_validation_backend: Validation backend to use, if multiple are installed.
         request_class: An optional subclass of :class:`Request <.connection.Request>` to use for http connections.
         response_class: A custom subclass of :class:`Response <.response.Response>` to be used as the app's default
             response.
         response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>`.
         response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
         response_cache_config: Configures caching behavior of the application.
         return_dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for serializing
@@ -496,16 +498,16 @@
         multipart_form_part_limit=multipart_form_part_limit,
         on_app_init=on_app_init,
         on_shutdown=on_shutdown,
         on_startup=on_startup,
         openapi_config=openapi_config,
         opt=opt,
         parameters=parameters,
+        pdb_on_exception=pdb_on_exception,
         plugins=plugins,
-        preferred_validation_backend=preferred_validation_backend,
         request_class=request_class,
         response_cache_config=response_cache_config,
         response_class=response_class,
         response_cookies=response_cookies,
         response_headers=response_headers,
         return_dto=return_dto,
         route_handlers=route_handlers,
@@ -514,14 +516,15 @@
         state=state,
         static_files_config=static_files_config,
         stores=stores,
         tags=tags,
         template_config=template_config,
         type_encoders=type_encoders,
         websocket_class=websocket_class,
+        _preferred_validation_backend=_preferred_validation_backend,
     )
 
     return AsyncTestClient[Litestar](
         app=app,
         backend=backend,
         backend_options=backend_options,
         base_url=base_url,
```

### Comparing `litestar-2.0.0a7/litestar/testing/life_span_handler.py` & `litestar-2.0.0b1/litestar/testing/life_span_handler.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/testing/request_factory.py` & `litestar-2.0.0b1/litestar/testing/request_factory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/testing/transport.py` & `litestar-2.0.0b1/litestar/testing/transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 
 from io import BytesIO
 from types import GeneratorType
-from typing import TYPE_CHECKING, Any, Generic, TypeVar, Union, cast
+from typing import TYPE_CHECKING, Any, Generic, TypedDict, TypeVar, Union, cast
 from urllib.parse import unquote
 
 from anyio import Event
 from httpx import ByteStream, Response
-from typing_extensions import TypedDict
 
 from litestar.status_codes import HTTP_500_INTERNAL_SERVER_ERROR
 from litestar.testing.websocket_test_session import WebSocketTestSession
 
 if TYPE_CHECKING:
     from httpx import Request
```

### Comparing `litestar-2.0.0a7/litestar/testing/websocket_test_session.py` & `litestar-2.0.0b1/litestar/testing/websocket_test_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         portal = self.exit_stack.enter_context(self.client.portal())
 
         try:
             portal.start_task_soon(self.do_asgi_call)
             event: WebSocketConnectEvent = {"type": "websocket.connect"}
             self.receive_queue.put(event)
 
-            message = self.receive()
+            message = self.receive(timeout=self.client.timeout.read)
             self.accepted_subprotocol = cast("str | None", message.get("subprotocol", None))
             self.extra_headers = cast("list[tuple[bytes, bytes]] | None", message.get("headers", None))
             return self
         except Exception:
             self.exit_stack.close()
             raise
```

### Comparing `litestar-2.0.0a7/litestar/types/__init__.py` & `litestar-2.0.0b1/litestar/types/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/types/asgi_types.py` & `litestar-2.0.0b1/litestar/types/asgi_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,19 +36,18 @@
     Callable,
     Dict,
     Iterable,
     List,
     Literal,
     Optional,
     Tuple,
+    TypedDict,
     Union,
 )
 
-from typing_extensions import TypedDict
-
 from litestar.enums import ScopeType
 
 __all__ = (
     "ASGIApp",
     "ASGIVersion",
     "BaseScope",
     "HeaderScope",
```

### Comparing `litestar-2.0.0a7/litestar/types/callable_types.py` & `litestar-2.0.0b1/litestar/types/callable_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,34 +19,35 @@
     from litestar.connection.base import ASGIConnection
     from litestar.connection.request import Request
     from litestar.datastructures.state import State
     from litestar.handlers.base import BaseRouteHandler
     from litestar.handlers.http_handlers import HTTPRouteHandler
     from litestar.response.base import Response
     from litestar.types.protocols import Logger
+
 else:
     AppConfig = Any
     BaseRouteHandler = Any
     Request = Any
     Response = Any
     State = Any
     ASGIConnection = Any
     Logger = Any
     HTTPRouteHandler = Any
 
 ExceptionT = TypeVar("ExceptionT", bound=Exception)
-AfterExceptionHookHandler = Callable[[Exception, Scope, State], SyncOrAsyncUnion[None]]
+AfterExceptionHookHandler = Callable[[Exception, Scope], SyncOrAsyncUnion[None]]
 AfterRequestHookHandler = Union[
     Callable[[ASGIApp], SyncOrAsyncUnion[ASGIApp]], Callable[[Response], SyncOrAsyncUnion[Response]]
 ]
 AfterResponseHookHandler = Callable[[Request], SyncOrAsyncUnion[None]]
 AsyncAnyCallable = Callable[..., Awaitable[Any]]
 AnyCallable = Callable[..., Any]
 AnyGenerator = Union[Generator[Any, Any, Any], AsyncGenerator[Any, Any]]
-BeforeMessageSendHookHandler = Callable[[Message, State, Scope], SyncOrAsyncUnion[None]]
+BeforeMessageSendHookHandler = Callable[[Message, Scope], SyncOrAsyncUnion[None]]
 BeforeRequestHookHandler = Callable[[Request], Union[Any, Awaitable[Any]]]
 CacheKeyBuilder = Callable[[Request], str]
 ExceptionHandler = Callable[[Request, ExceptionT], Response]
 ExceptionLoggingHandler = Callable[[Logger, Scope, List[str]], None]
 GetLogger = Callable[..., Logger]
 Guard = Callable[[ASGIConnection, BaseRouteHandler], SyncOrAsyncUnion[None]]
 LifespanHook = Union[
```

### Comparing `litestar-2.0.0a7/litestar/types/composite_types.py` & `litestar-2.0.0b1/litestar/types/composite_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     AsyncIterator,
     Callable,
     Dict,
     Iterable,
     Iterator,
     Literal,
     Mapping,
+    MutableMapping,
     Sequence,
     Set,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
@@ -41,15 +42,15 @@
     Provide = Any
     ResponseHeader = Any
 
 T = TypeVar("T")
 
 
 Dependencies = Mapping[str, Union[Provide, AnyCallable]]
-ExceptionHandlersMap = Mapping[Union[int, Type[Exception]], ExceptionHandler]
+ExceptionHandlersMap = MutableMapping[Union[int, Type[Exception]], ExceptionHandler]
 MaybePartial = Union[T, partial]
 Middleware = Union[
     Callable[..., ASGIApp], DefineMiddleware, Iterator[Tuple[ASGIApp, Dict[str, Any]]], Type[MiddlewareProtocol]
 ]
 ParametersMap = Mapping[str, ParameterKwarg]
 PathType = Union[Path, PathLike, str]
 ResponseCookies = Union[Sequence[Cookie], Mapping[str, str]]
```

### Comparing `litestar-2.0.0a7/litestar/types/file_types.py` & `litestar-2.0.0b1/litestar/types/file_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,20 @@
     TYPE_CHECKING,
     Any,
     AnyStr,
     Awaitable,
     Literal,
     Optional,
     Protocol,
+    TypedDict,
     Union,
     overload,
 )
 
-from typing_extensions import NotRequired, TypedDict
+from typing_extensions import NotRequired
 
 __all__ = ("FileInfo", "FileSystemProtocol")
 
 
 if TYPE_CHECKING:
     from _typeshed import OpenBinaryMode, OpenTextMode
     from anyio import AsyncFile
```

### Comparing `litestar-2.0.0a7/litestar/types/internal_types.py` & `litestar-2.0.0b1/litestar/types/internal_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/types/serialization.py` & `litestar-2.0.0b1/litestar/types/serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/utils/__init__.py` & `litestar-2.0.0b1/litestar/utils/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from litestar.utils.deprecation import deprecated, warn_deprecation
 
-from .helpers import Ref, get_enum_string_value, get_name
+from .helpers import Ref, encode_headers, get_enum_string_value, get_name, url_quote
 from .path import join_paths, normalize_path
 from .predicates import (
     is_any,
+    is_async_callable,
     is_attrs_class,
     is_class_and_subclass,
     is_class_var,
     is_dataclass_class,
+    is_dataclass_instance,
     is_generic,
     is_mapping,
     is_non_string_iterable,
     is_non_string_sequence,
     is_optional_union,
     is_pydantic_constrained_field,
     is_pydantic_model_class,
@@ -22,45 +24,40 @@
 from .scope import (
     delete_litestar_scope_state,
     get_litestar_scope_state,
     get_serializer_from_scope,
     set_litestar_scope_state,
 )
 from .sequence import compact, find_index, unique
-from .sync import (
-    AsyncCallable,
-    AsyncIteratorWrapper,
-    as_async_callable_list,
-    async_partial,
-    is_async_callable,
-)
+from .sync import AsyncCallable, AsyncIteratorWrapper, async_partial
 from .typing import annotation_is_iterable_of_type, get_origin_or_inner_type, make_non_optional_union
 
 __all__ = (
     "AsyncCallable",
     "AsyncIteratorWrapper",
     "Ref",
     "annotation_is_iterable_of_type",
-    "as_async_callable_list",
     "async_partial",
     "compact",
     "delete_litestar_scope_state",
     "deprecated",
+    "encode_headers",
     "find_index",
     "get_enum_string_value",
     "get_litestar_scope_state",
     "get_name",
     "get_origin_or_inner_type",
     "get_serializer_from_scope",
     "is_any",
     "is_async_callable",
     "is_attrs_class",
     "is_class_and_subclass",
     "is_class_var",
     "is_dataclass_class",
+    "is_dataclass_instance",
     "is_generic",
     "is_mapping",
     "is_non_string_iterable",
     "is_non_string_sequence",
     "is_optional_union",
     "is_pydantic_constrained_field",
     "is_pydantic_model_class",
@@ -68,9 +65,10 @@
     "is_typed_dict",
     "is_union",
     "join_paths",
     "make_non_optional_union",
     "normalize_path",
     "set_litestar_scope_state",
     "unique",
+    "url_quote",
     "warn_deprecation",
 )
```

### Comparing `litestar-2.0.0a7/litestar/utils/compat.py` & `litestar-2.0.0b1/litestar/utils/compat.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/utils/dataclass.py` & `litestar-2.0.0b1/litestar/utils/dataclass.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
 from dataclasses import Field, fields
 from typing import TYPE_CHECKING
 
 from litestar.types import Empty
-from litestar.types.protocols import DataclassProtocol
+from litestar.utils.predicates import is_dataclass_instance
 
 if TYPE_CHECKING:
     from typing import AbstractSet, Any, Iterable
 
+    from litestar.types.protocols import DataclassProtocol
+
 __all__ = (
     "extract_dataclass_fields",
     "extract_dataclass_items",
     "simple_asdict",
 )
 
 
@@ -97,12 +99,12 @@
 
     Returns:
         A dictionary of key/value pairs.
     """
     ret = {}
     for field in extract_dataclass_fields(obj, exclude_none, exclude_empty):
         value = getattr(obj, field.name)
-        if isinstance(value, DataclassProtocol) and convert_nested:
+        if is_dataclass_instance(value) and convert_nested:
             ret[field.name] = simple_asdict(value, exclude_none, exclude_empty)
         else:
             ret[field.name] = getattr(obj, field.name)
     return ret
```

### Comparing `litestar-2.0.0a7/litestar/utils/deprecation.py` & `litestar-2.0.0b1/litestar/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/utils/helpers.py` & `litestar-2.0.0b1/litestar/utils/helpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,33 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from enum import Enum
+from itertools import chain
 from typing import TYPE_CHECKING, Any, Generic, TypeVar, cast
+from urllib.parse import quote
 
-__all__ = ("Ref", "get_enum_string_value", "get_fully_qualified_class_name", "get_name", "unwrap_partial")
+if TYPE_CHECKING:
+    from typing import Iterable
 
+    from litestar.datastructures import Cookie
+    from litestar.types import MaybePartial
 
-T = TypeVar("T")
+__all__ = (
+    "Ref",
+    "encode_headers",
+    "filter_cookies",
+    "get_enum_string_value",
+    "get_fully_qualified_class_name",
+    "get_name",
+    "unwrap_partial",
+    "url_quote",
+)
 
-if TYPE_CHECKING:
-    from litestar.types import MaybePartial
+T = TypeVar("T")
 
 
 def get_name(value: Any) -> str:
     """Get the ``__name__`` of an object.
 
     Args:
         value: An arbitrary object.
@@ -66,7 +79,54 @@
     Returns:
         Callable
     """
     output: Any = value.func if hasattr(value, "func") else value  # pyright: ignore
     while hasattr(output, "func"):
         output = output.func
     return cast("T", output)
+
+
+def encode_headers(
+    headers: Iterable[tuple[str, Any]], cookies: Iterable[Cookie], raw_headers: list[tuple[bytes, bytes]]
+) -> list[tuple[bytes, bytes]]:
+    """Encode the response headers as a list of byte tuples.
+
+    Args:
+        headers: Iterable of header name/value pairs.
+        cookies: A list of cookies.
+        raw_headers: A list of raw headers.
+
+    Returns:
+        A list of byte tuples.
+    """
+    return list(
+        chain(
+            ((k.lower().encode("latin-1"), str(v).encode("latin-1")) for k, v in headers),
+            (cookie.to_encoded_header() for cookie in cookies if not cookie.documentation_only),
+            raw_headers,
+        )
+    )
+
+
+def filter_cookies(local_cookies: Iterable[Cookie], layered_cookies: Iterable[Cookie]) -> list[Cookie]:
+    """Given two sets of cookies, return a unique list of cookies, that are not marked as documentation_only.
+
+    Args:
+        local_cookies: Cookies returned from the local scope.
+        layered_cookies: Cookies returned from the layers.
+
+    Returns:
+        A unified list of cookies
+    """
+    return [cookie for cookie in {*local_cookies, *layered_cookies} if not cookie.documentation_only]
+
+
+def url_quote(value: str | bytes) -> str:
+    """Quote a URL.
+
+    Args:
+        value: A URL.
+
+    Returns:
+        A quoted URL.
+    """
+    return quote(value, safe="/#%[]=:;$&()+,!?*@'~")
```

### Comparing `litestar-2.0.0a7/litestar/utils/path.py` & `litestar-2.0.0b1/litestar/utils/path.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/utils/predicates.py` & `litestar-2.0.0b1/litestar/utils/predicates.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from __future__ import annotations
 
+from asyncio import iscoroutinefunction
 from collections import defaultdict, deque
 from collections.abc import Iterable as CollectionsIterable
 from dataclasses import is_dataclass
-from inspect import isclass
+from functools import partial
+from inspect import isasyncgenfunction, isclass, isgeneratorfunction
 from typing import (
     TYPE_CHECKING,
     Any,
+    Awaitable,
+    Callable,
     ClassVar,
     DefaultDict,
     Deque,
     Dict,
     FrozenSet,
     Generic,
     Iterable,
@@ -27,55 +31,104 @@
 from typing_extensions import (
     ParamSpec,
     TypeGuard,
     get_args,
     is_typeddict,
 )
 
-from litestar.types import DataclassProtocol, Empty
+from litestar.types import Empty
 from litestar.types.builtin_types import UNION_TYPES, NoneType
 from litestar.utils.typing import get_origin_or_inner_type
 
 if TYPE_CHECKING:
-    from litestar.types.builtin_types import (
-        TypedDictClass,
-    )
+    from litestar.types.builtin_types import TypedDictClass
+    from litestar.types.callable_types import AnyGenerator
+    from litestar.types.protocols import DataclassProtocol
+
 
 try:
     import pydantic
 except ImportError:  # pragma: no cover
     pydantic = Empty  # type: ignore
 
 try:
     import attrs
 except ImportError:  # pragma: no cover
     attrs = Empty  # type: ignore
 
 __all__ = (
+    "is_async_callable",
     "is_any",
     "is_attrs_class",
     "is_class_and_subclass",
     "is_class_var",
     "is_dataclass_class",
+    "is_dataclass_instance",
     "is_generic",
     "is_mapping",
     "is_non_string_iterable",
     "is_non_string_sequence",
     "is_optional_union",
     "is_pydantic_constrained_field",
     "is_pydantic_model_class",
     "is_pydantic_model_instance",
+    "is_sync_or_async_generator",
     "is_typed_dict",
     "is_union",
 )
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
+def is_async_callable(value: Callable[P, T]) -> TypeGuard[Callable[P, Awaitable[T]]]:
+    """Extend :func:`asyncio.iscoroutinefunction` to additionally detect async :func:`functools.partial` objects and
+    class instances with ``async def __call__()`` defined.
+
+    Args:
+        value: Any
+
+    Returns:
+        Bool determining if type of ``value`` is an awaitable.
+    """
+    while isinstance(value, partial):
+        value = value.func  # type: ignore[unreachable]
+
+    return iscoroutinefunction(value) or (
+        callable(value) and iscoroutinefunction(value.__call__)  #  type: ignore[operator]
+    )
+
+
+def is_dataclass_instance(obj: Any) -> TypeGuard[DataclassProtocol]:
+    """Check if an object is a dataclass instance.
+
+    Args:
+        obj: An object to check.
+
+    Returns:
+        True if the object is a dataclass instance.
+    """
+    return hasattr(type(obj), "__dataclass_fields__")
+
+
+def is_dataclass_class(annotation: Any) -> TypeGuard[type[DataclassProtocol]]:
+    """Wrap :func:`is_dataclass <dataclasses.is_dataclass>` in a :data:`typing.TypeGuard`.
+
+    Args:
+        annotation: tested to determine if instance or type of :class:`dataclasses.dataclass`.
+
+    Returns:
+        ``True`` if instance or type of ``dataclass``.
+    """
+    try:
+        return isclass(annotation) and is_dataclass(annotation)
+    except TypeError:  # pragma: no cover
+        return False
+
+
 def is_class_and_subclass(annotation: Any, t_type: type[T]) -> TypeGuard[type[T]]:
     """Return ``True`` if ``value`` is a ``class`` and is a subtype of ``t_type``.
 
     See https://github.com/litestar-org/litestar/issues/367
 
     Args:
         annotation: The value to check if is class and subclass of ``t_type``.
@@ -212,29 +265,14 @@
     """
     origin = get_origin_or_inner_type(annotation)
     return origin is Optional or (
         get_origin_or_inner_type(annotation) in UNION_TYPES and NoneType in get_args(annotation)
     )
 
 
-def is_dataclass_class(annotation: Any) -> TypeGuard[type[DataclassProtocol]]:
-    """Wrap :func:`is_dataclass <dataclasses.is_dataclass>` in a :data:`typing.TypeGuard`.
-
-    Args:
-        annotation: tested to determine if instance or type of :class:`dataclasses.dataclass`.
-
-    Returns:
-        ``True`` if instance or type of ``dataclass``.
-    """
-    try:
-        return isclass(annotation) and is_dataclass(annotation)
-    except TypeError:  # pragma: no cover
-        return False
-
-
 def is_typed_dict(annotation: Any) -> TypeGuard[TypedDictClass]:
     """Wrap :func:`typing.is_typeddict` in a :data:`typing.TypeGuard`.
 
     Args:
         annotation: tested to determine if instance or type of :class:`typing.TypedDict`.
 
     Returns:
@@ -283,48 +321,50 @@
     if attrs is not Empty:  # type: ignore[comparison-overlap]
         return attrs.has(annotation)  # pyright: ignore
     return False  # pragma: no cover
 
 
 def is_pydantic_constrained_field(
     annotation: Any,
-) -> TypeGuard[
-    type[pydantic.ConstrainedBytes]  # pyright: ignore
-    | type[pydantic.ConstrainedDate]  # pyright: ignore
-    | type[pydantic.ConstrainedDecimal]  # pyright: ignore
-    | type[pydantic.ConstrainedFloat]  # pyright: ignore
-    | type[pydantic.ConstrainedFrozenSet]  # pyright: ignore
-    | type[pydantic.ConstrainedInt]  # pyright: ignore
-    | type[pydantic.ConstrainedList]  # pyright: ignore
-    | type[pydantic.ConstrainedSet]  # pyright: ignore
-    | type[pydantic.ConstrainedStr]  # pyright: ignore
-]:
+) -> Any:
     """Check if the given annotation is a constrained pydantic type.
 
     Args:
         annotation: A type annotation
 
     Returns:
         True if pydantic is installed and the type is a constrained type, otherwise False.
     """
     try:
-        import pydantic
+        # removed in pydantic v2
+        # so this will raise an ImportError - which is expected.
+        from pydantic import (
+            ConstrainedBytes,
+            ConstrainedDate,
+            ConstrainedDecimal,
+            ConstrainedFloat,
+            ConstrainedFrozenSet,
+            ConstrainedInt,
+            ConstrainedList,
+            ConstrainedSet,
+            ConstrainedStr,
+        )
 
         return any(
             is_class_and_subclass(annotation, constrained_type)
             for constrained_type in (
-                pydantic.ConstrainedBytes,
-                pydantic.ConstrainedDate,
-                pydantic.ConstrainedDecimal,
-                pydantic.ConstrainedFloat,
-                pydantic.ConstrainedFrozenSet,
-                pydantic.ConstrainedInt,
-                pydantic.ConstrainedList,
-                pydantic.ConstrainedSet,
-                pydantic.ConstrainedStr,
+                ConstrainedBytes,
+                ConstrainedDate,
+                ConstrainedDecimal,
+                ConstrainedFloat,
+                ConstrainedFrozenSet,
+                ConstrainedInt,
+                ConstrainedList,
+                ConstrainedSet,
+                ConstrainedStr,
             )
         )
     except ImportError:
         return False
 
 
 def is_struct_class(annotation: Any) -> TypeGuard[type[Struct]]:
@@ -346,7 +386,19 @@
         annotation: A type annotation
 
     Returns:
         A boolean.
     """
     annotation = get_origin_or_inner_type(annotation) or annotation
     return annotation is ClassVar
+
+
+def is_sync_or_async_generator(obj: Any) -> TypeGuard[AnyGenerator]:
+    """Check if the given annotation is a sync or async generator.
+
+    Args:
+        obj: type to be tested for sync or async generator.
+
+    Returns:
+        A boolean.
+    """
+    return isgeneratorfunction(obj) or isasyncgenfunction(obj)
```

### Comparing `litestar-2.0.0a7/litestar/utils/scope.py` & `litestar-2.0.0b1/litestar/utils/scope.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from litestar.constants import SCOPE_STATE_NAMESPACE
+from litestar.serialization import get_serializer
+
+if TYPE_CHECKING:
+    from litestar.types import Scope, Serializer
 
 __all__ = (
     "delete_litestar_scope_state",
     "get_serializer_from_scope",
     "get_litestar_scope_state",
     "set_litestar_scope_state",
 )
 
 
-if TYPE_CHECKING:
-    from litestar.types import Scope, Serializer
-
-
-def get_serializer_from_scope(scope: Scope) -> Serializer | None:
+def get_serializer_from_scope(scope: Scope) -> Serializer:
     """Return a serializer given a scope object.
 
     Args:
         scope: The ASGI connection scope.
 
     Returns:
         A serializer function
     """
     route_handler = scope["route_handler"]
     app = scope["app"]
 
+    if hasattr(route_handler, "resolve_type_encoders"):
+        type_encoders = route_handler.resolve_type_encoders()
+    else:
+        type_encoders = app.type_encoders or {}
+
     if response_class := (
         route_handler.resolve_response_class()  # pyright: ignore
         if hasattr(route_handler, "resolve_response_class")
         else app.response_class
     ):
-        return response_class.get_serializer(
-            route_handler.resolve_type_encoders()  # pyright: ignore
-            if hasattr(route_handler, "resolve_type_encoders")
-            else app.type_encoders
-        )
+        type_encoders = {**type_encoders, **(response_class.type_encoders or {})}
 
-    return None
+    return get_serializer(type_encoders)
 
 
 def get_litestar_scope_state(scope: Scope, key: str, default: Any = None, pop: bool = False) -> Any:
     """Get an internal value from connection scope state.
 
     Note:
         If called with a default value, this method behaves like to `dict.set_default()`, both setting the key in the
```

### Comparing `litestar-2.0.0a7/litestar/utils/sequence.py` & `litestar-2.0.0b1/litestar/utils/sequence.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/utils/sync.py` & `litestar-2.0.0b1/litestar/utils/sync.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-from asyncio import iscoroutinefunction
 from functools import partial
 from inspect import getfullargspec, ismethod
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncGenerator,
     Awaitable,
@@ -13,47 +12,32 @@
     Iterable,
     Iterator,
     TypeVar,
     cast,
 )
 
 from anyio.to_thread import run_sync
-from typing_extensions import ParamSpec, TypeGuard
+from typing_extensions import ParamSpec
 
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.types import Empty
-from litestar.utils.helpers import Ref
+from litestar.utils.helpers import Ref, unwrap_partial
+from litestar.utils.predicates import is_async_callable
 
 if TYPE_CHECKING:
     from litestar.types.empty import EmptyType
     from litestar.utils.signature import ParsedSignature
 
-__all__ = ("AsyncCallable", "AsyncIteratorWrapper", "as_async_callable_list", "async_partial", "is_async_callable")
+__all__ = ("AsyncCallable", "AsyncIteratorWrapper", "async_partial", "is_async_callable")
 
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
-def is_async_callable(value: Callable[P, T]) -> TypeGuard[Callable[P, Awaitable[T]]]:
-    """Extend :func:`asyncio.iscoroutinefunction` to additionally detect async :func:`functools.partial` objects and
-    class instances with ``async def __call__()`` defined.
-
-    Args:
-        value: Any
-
-    Returns:
-        Bool determining if type of ``value`` is an awaitable.
-    """
-    while isinstance(value, partial):
-        value = value.func  # type: ignore[unreachable]
-
-    return iscoroutinefunction(value) or (callable(value) and iscoroutinefunction(value.__call__))  # type: ignore[operator]
-
-
 class AsyncCallable(Generic[P, T]):
     """Wrap a callable into an asynchronous callable."""
 
     __slots__ = ("args", "kwargs", "ref", "is_method", "num_expected_args", "_parsed_signature")
 
     def __init__(self, fn: Callable[P, T]) -> None:
         """Initialize the wrapper from any callable.
@@ -93,29 +77,15 @@
         """Set the parsed signature of the wrapped function.
 
         Args:
             namespace: Namespace for forward ref resolution.
         """
         from litestar.utils.signature import ParsedSignature
 
-        self._parsed_signature = ParsedSignature.from_fn(self.ref.value, namespace)
-
-
-def as_async_callable_list(value: Callable | list[Callable]) -> list[AsyncCallable]:
-    """Wrap callables in ``AsyncCallable`` s.
-
-    Args:
-        value: A callable or list of callables.
-
-    Returns:
-        A list of AsyncCallable instances
-    """
-    if not isinstance(value, list):
-        return [AsyncCallable(value)]
-    return [AsyncCallable(v) for v in value]
+        self._parsed_signature = ParsedSignature.from_fn(unwrap_partial(self.ref.value), namespace)
 
 
 def async_partial(fn: Callable) -> Callable:
     """Wrap a given sync function making it async.
 
     In difference to the :func:`asyncio.run_sync` function, it allows for passing kwargs.
```

### Comparing `litestar-2.0.0a7/litestar/utils/typing.py` & `litestar-2.0.0b1/litestar/utils/typing.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,16 +27,18 @@
 
 from typing_extensions import Annotated, NotRequired, Required, TypeGuard, get_args, get_origin
 
 from litestar.types.builtin_types import UNION_TYPES, NoneType
 
 __all__ = (
     "annotation_is_iterable_of_type",
+    "get_instantiable_origin",
     "get_origin_or_inner_type",
     "get_safe_generic_origin",
+    "instantiable_type_mapping",
     "make_non_optional_union",
     "unwrap_annotation",
 )
 
 
 T = TypeVar("T")
 UnionT = TypeVar("UnionT", bound="Union")
@@ -44,28 +46,41 @@
 tuple_types_regex = re.compile(
     "^"
     + "|".join(
         [*[repr(x) for x in (List, Sequence, Iterable, Iterator, Tuple, Deque)], "tuple", "list", "collections.deque"]
     )
 )
 
-types_mapping = {
+instantiable_type_mapping = {
     AbstractSet: set,
     DefaultDict: defaultdict,
     Deque: deque,
     Dict: dict,
     FrozenSet: frozenset,
     List: list,
     Mapping: dict,
     MutableMapping: dict,
     MutableSequence: list,
     MutableSet: set,
     Sequence: list,
     Set: set,
     Tuple: tuple,
+    abc.Mapping: dict,
+    abc.MutableMapping: dict,
+    abc.MutableSequence: list,
+    abc.MutableSet: set,
+    abc.Sequence: list,
+    abc.Set: set,
+    defaultdict: defaultdict,
+    deque: deque,
+    dict: dict,
+    frozenset: frozenset,
+    list: list,
+    set: set,
+    tuple: tuple,
 }
 
 _safe_generic_origin_map = {
     set: t.AbstractSet,
     defaultdict: t.DefaultDict,
     deque: t.Deque,
     dict: t.Dict,
@@ -101,14 +116,19 @@
 ``collections.abc.Mapping``, are not valid generic types in Python 3.8.
 """
 
 wrapper_type_set = {Annotated, Required, NotRequired}
 """Types that always contain a wrapped type annotation as their first arg."""
 
 
+def normalize_type_annotation(annotation: Any) -> Any:
+    """Normalize a type annotation to a standard form."""
+    return instantiable_type_mapping.get(annotation, annotation)
+
+
 def annotation_is_iterable_of_type(
     annotation: Any,
     type_value: type[T],
 ) -> TypeGuard[Iterable[T]]:
     """Determine if a given annotation is an iterable of the given type_value.
 
     Args:
@@ -196,23 +216,49 @@
 
     Returns:
         Any type.
     """
     origin = get_origin(annotation)
     if origin in wrapper_type_set:
         inner, _, _ = unwrap_annotation(annotation)
-        # we need to recursively call here 'get_origin_or_inner_type' because we might be dealing with a generic type alias
-        # e.g. Annotated[dict[str, list[int]]
+        # we need to recursively call here 'get_origin_or_inner_type' because we might be dealing
+        # with a generic type alias e.g. Annotated[dict[str, list[int]]
         origin = get_origin_or_inner_type(inner)
-    return types_mapping.get(origin, origin)
+    return instantiable_type_mapping.get(origin, origin)
 
 
-def get_safe_generic_origin(origin_type: Any) -> Any:
+def get_safe_generic_origin(origin_type: Any, annotation: Any) -> Any:
     """Get a type that is safe to use as a generic type across all supported Python versions.
 
+    If a builtin collection type is annotated without generic args, e.g, ``a: dict``, then the origin type will be
+    ``None``. In this case, we can use the annotation to determine the correct generic type, if one exists.
+
     Args:
         origin_type: A type - would be the return value of :func:`get_origin()`.
+        annotation: Type annotation associated with the origin type. Should be unwrapped from any wrapper types, such
+            as ``Annotated``.
 
     Returns:
         The ``typing`` module equivalent of the given type, if it exists. Otherwise, the original type is returned.
     """
+    if origin_type is None:
+        return _safe_generic_origin_map.get(annotation)
     return _safe_generic_origin_map.get(origin_type, origin_type)
+
+
+def get_instantiable_origin(origin_type: Any, annotation: Any) -> Any:
+    """Get a type that is safe to instantiate for the given origin type.
+
+    If a builtin collection type is annotated without generic args, e.g, ``a: dict``, then the origin type will be
+    ``None``. In this case, we can use the annotation to determine the correct instantiable type, if one exists.
+
+    Args:
+        origin_type: A type - would be the return value of :func:`get_origin()`.
+        annotation: Type annotation associated with the origin type. Should be unwrapped from any wrapper types, such
+            as ``Annotated``.
+
+    Returns:
+        A builtin type that is safe to instantiate for the given origin type.
+    """
+    if origin_type is None:
+        return instantiable_type_mapping.get(annotation)
+    return instantiable_type_mapping.get(origin_type, origin_type)
```

### Comparing `litestar-2.0.0a7/litestar/utils/version.py` & `litestar-2.0.0b1/litestar/utils/version.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a7/litestar/utils/warnings.py` & `litestar-2.0.0b1/litestar/utils/warnings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import warnings
 
 from litestar.exceptions import LitestarWarning
-from litestar.types import AnyCallable
+from litestar.types import AnyCallable, AnyGenerator
 
 
 def warn_implicit_sync_to_thread(source: AnyCallable, stacklevel: int = 2) -> None:
     if os.getenv("LITESTAR_WARN_IMPLICIT_SYNC_TO_THREAD") == "0":
         return
 
     warnings.warn(
@@ -28,7 +28,24 @@
     warnings.warn(
         f"Use of an asynchronous callable {source} with sync_to_thread; sync_to_thread "
         "has no effect on async callable. You can disable this warning by setting "
         "LITESTAR_WARN_SYNC_TO_THREAD_WITH_ASYNC=0",
         category=LitestarWarning,
         stacklevel=stacklevel,
     )
+
+
+def warn_sync_to_thread_with_generator(source: AnyGenerator, stacklevel: int = 2) -> None:
+    if os.getenv("LITESTAR_WARN_SYNC_TO_THREAD_WITH_GENERATOR") == "0":
+        return
+
+    warnings.warn(
+        f"Use of generator {source} with sync_to_thread; sync_to_thread has no effect "
+        "on generators. You can disable this warning by setting "
+        "LITESTAR_WARN_SYNC_TO_THREAD_WITH_GENERATOR=0",
+        category=LitestarWarning,
+        stacklevel=stacklevel,
+    )
+
+
+def warn_pdb_on_exception(stacklevel: int = 2) -> None:
+    warnings.warn("Python Debugger on exception enabled", category=LitestarWarning, stacklevel=stacklevel)
```

### Comparing `litestar-2.0.0a7/pyproject.toml` & `litestar-2.0.0b1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "litestar"
-version = "2.0.0alpha7"
-description = "Performant, light and flexible ASGI API Framework"
+version = "2.0.0beta1"
+description = "Litestar - A production-ready, highly performant, extensible ASGI API Framework"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
+    "Jacob Coffee <jacob@z7x.org>",
 ]
 maintainers = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
     "Jacob Coffee <jacob@z7x.org>",
 ]
 license = "MIT"
-readme = "README.md"
+readme = "docs/PYPI_README.md"
 homepage = "https://litestar.dev/"
 repository = "https://github.com/litestar-org/litestar"
 documentation = "https://docs.litestar.dev/"
 keywords = [
     "api",
     "rest",
     "http",
@@ -47,14 +48,22 @@
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development",
     "Typing :: Typed",
 ]
 include = ["CHANGELOG.rst"]
 packages = [{ include = "litestar" }]
 
+[tool.poetry.urls]
+"Issue Tracker" = "https://github.com/litestar-org/litestar/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc"
+"Changelog" = "https://github.com/litestar-org/litestar/releases/"
+"Twitter" = "https://twitter.com/LitestarAPI"
+"Reddit" = "https://www.reddit.com/r/litestarapi"
+"Discord" = "https://discord.gg/MmcwxztmQb"
+"Blog" = "https://blog.litestar.dev"
+
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 alembic = { version = "*", optional = true }
 anyio = ">=3"
 attrs = { version = "*", optional = true }
 brotli = { version = "*", optional = true }
 cattrs = { version = "*", optional = true }
@@ -74,25 +83,29 @@
 pydantic = "<2"
 python-dateutil = { version = "*", optional = true }
 python-jose = { version = "*", optional = true }
 pytimeparse = { version = "*", optional = true }
 pyyaml = "*"
 redis = { version = ">=4.4.4,!=4.5.0,!=4.5.1,!=4.5.2,!=4.5.3,!=4.5.5", optional = true, extras = ["hiredis"] }
 rich = { version = ">=13.0.0", optional = true }
+rich-click = { version = "*", optional = true }
 sqlalchemy = { version = ">=2.0.12", optional = true }
 structlog = { version = "*", optional = true }
 typing-extensions = "*"
-uvicorn = {extras = ["standard"], version = "^0.21.1", optional = true}
+uvicorn = {extras = ["standard"], version = "^0.22.0", optional = true}
 importlib-resources = { version="^5.12.0", python = "<3.9" }
 
 [tool.poetry.group.dev.dependencies]
 aiosqlite = "*"
+rich-click = "*"
+alembic = "*"
 asyncmy = "*"
 asyncpg = "*"
 attrs = "*"
+beanie = "*"
 beautifulsoup4 = "*"
 brotli = "*"
 cattrs = "*"
 click = "*"
 cryptography = "*"
 fakeredis = { extras = ["lua"], version = "2.11.0" }
 freezegun = "*"
@@ -110,28 +123,30 @@
 pre-commit = "*"
 psycopg = "*"
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "*"
 pytest-lazy-fixture = "*"
 pytest-mock = "*"
-pytest_docker = "*"
 python-dateutil = "*"
 python-dotenv = "*"
 python-jose = "*"
+oracledb = "*"
 pytimeparse = "*"
 redis = "*"
 rich = "*"
 sqlalchemy = ">=2.0"
 starlette = "*"
 structlog = "*"
 tortoise-orm = ">=0.17.0"
 trio = "*"
 uvicorn = "*"
 pytest-rerunfailures = "^11.1.2"
+duckdb-engine = "*"
+sqlalchemy-spanner = "*"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 auto-pytabs = { extras = ["sphinx"], version = "*" }
 black = "*"
@@ -140,29 +155,48 @@
 sphinx-autobuild = "*"
 sphinx-copybutton = ">=0.5.1"
 sphinx-design = ">=0.3.0,<1"
 sphinxcontrib-mermaid = ">=0.8.1,<1"
 litestar-sphinx-theme = { git = "https://github.com/litestar-org/litestar-sphinx-theme.git" }
 uvicorn = "*"
 
+[tool.poetry.group.lint]
+optional = true
+
+[tool.poetry.group.lint.dependencies]
+asyncpg-stubs = "*"
+black = "*"
+blacken-docs = "*"
+mypy = "*"
+pylint = "*"
+pylint-pydantic = "*"
+pyright = "*"
+ruff = '*'
+slotscheck = "*"
+types-freezegun = "*"
+types-python-jose = "*"
+types-pyyaml = "*"
+types-redis = "*"
+types-beautifulsoup4 = "*"
+types-python-dateutil = "*"
+
 [tool.poetry.extras]
 attrs = ["attrs", "cattrs", "python-dateutil", "pytimeparse"]
 brotli = ["brotli"]
-cli = ["click", "rich", "jsbeautifier", "uvicorn"]
+cli = ["click", "rich", "rich-click", "jsbeautifier", "uvicorn"]
 cryptography = ["cryptography"]
 jinja = ["jinja2"]
 jwt = ["python-jose", "cryptography"]
 opentelemetry = ["opentelemetry-instrumentation-asgi"]
 picologging = ["picologging"]
 redis = ["redis"]
 sqlalchemy = ["sqlalchemy", "alembic"]
-standard = ["click", "jinja2", "jsbeautifier", "rich", "uvicorn"]
+standard = ["click", "jinja2", "jsbeautifier", "rich", "uvicorn", "rich-click"]
 structlog = ["structlog"]
 tortoise-orm = ["tortoise-orm"]
-
 full = [
     "alembic",
     "attrs",
     "brotli",
     "cattrs",
     "click",
     "cryptography",
@@ -176,26 +210,27 @@
     "rich",
     "sqlalchemy",
     "structlog",
     "uvicorn",
 ]
 
 [tool.poetry.scripts]
-litestar = { callable = "litestar:__main__", extras = ["cli"] }
+litestar = { callable = "litestar.__main__:run_cli", extras = ["cli"] }
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 include = '\.pyi?$'
 
 [tool.codespell]
 ignore-words-list = "selectin"
+skip = 'poetry.lock,docs/examples/contrib/sqlalchemy/us_state_lookup.json'
 
 [tool.coverage.run]
 omit = ["*/tests/*", "litestar/contrib/sqlalchemy_1/*"]
 
 [tool.coverage.report]
 exclude_lines = [
     'pragma: no cover',
@@ -203,25 +238,37 @@
     'except ImportError as e:',
     'except ImportError:',
     '\.\.\.',
     'raise NotImplementedError',
 ]
 
 [tool.pytest.ini_options]
-addopts = "--ignore=examples"
+addopts = "--ignore=examples -m='not sqlalchemy_integration'"
 asyncio_mode = "auto"
 filterwarnings = [
     "ignore::trio.TrioDeprecationWarning:anyio._backends._trio*:164",
-    "ignore::DeprecationWarning:pkg_resources:2803",
+    "ignore::DeprecationWarning:pkg_resources.*",
+    "ignore::DeprecationWarning:google.rpc",
+    "ignore::DeprecationWarning:google.gcloud",
+    "ignore::DeprecationWarning:google.iam",
+    "ignore::DeprecationWarning:google",
+    "ignore::DeprecationWarning:sphinxcontrib",
+    "ignore::DeprecationWarning:litestar.*",
 ]
 markers = [
+    "sqlalchemy_integration: SQLAlchemy integration tests",
     "sqlalchemy_asyncmy: SQLAlchemy MySQL (asyncmy) Tests",
     "sqlalchemy_asyncpg: SQLAlchemy Postgres (asyncpg) Tests",
     "sqlalchemy_psycopg_async: SQLAlchemy Postgres (psycopg async) Tests",
-    "sqlalchemy_aiosqlite: SQLAlchemy SQLite (aiosqlite) Tests"
+    "sqlalchemy_aiosqlite: SQLAlchemy SQLite (aiosqlite) Tests",
+    "sqlalchemy_psycopg_sync: SQLAlchemy Postgres (psycopg sync) Tests",
+    "sqlalchemy_sqlite: SQLAlchemy SQLite (sqlite) Tests",
+    "sqlalchemy_oracledb: SQLAlchemy Oracle (oracledb) Tests",
+    "sqlalchemy_spanner: SQLAlchemy Google Cloud Spanner (sqlalchemy-spanner) Tests",
+    "sqlalchemy_duckdb: SQLAlchemy Duckdb (duckdb-engine) Tests",
 ]
 
 [tool.pyright]
 include = ["litestar", "tests", "examples"]
 exclude = [
     "examples/plugins/sqlalchemy_plugin",
     "litestar/contrib/sqlalchemy_1",
@@ -336,14 +383,15 @@
     "S",
     "S101",
     "SIM",
     "TCH",
     "TRY",
 ]
 "docs/examples/application_hooks/before_send_hook.py" = ["UP006"]
+"docs/examples/contrib/sqlalchemy/plugins/**/*.*" = ["UP006"]
 "docs/examples/tests/**/*.*" = [
     "A",
     "ARG",
     "B",
     "BLE",
     "C901",
     "D",
@@ -362,13 +410,32 @@
     "S101",
     "SIM",
     "TCH",
     "TRY",
 ]
 "docs/**/*.*" = ["S", "B", "DTZ", "A", "TCH", "ERA", "D", "RET"]
 "docs/examples/**" = ["T201"]
+"docs/examples/data_transfer_objects**/*.*" = ["UP006"]
 "litestar/exceptions/*.*" = ["N818"]
 "litestar/handlers/**/*.*" = ["N801"]
 "litestar/_openapi/schema_generation/schema.py" = ["C901"]
 "litestar/params.py" = ["N802"]
 "test_apps/**/*.*" = ["D", "TRY", "EM", "S", "PTH"]
 "tools/**/*.*" = ["D", "ARG", "EM", "TRY", "G", "FBT"]
+
+
+[tool.unasyncd]
+add_editors_note = true
+
+
+[tool.unasyncd.files]
+"litestar/contrib/sqlalchemy/repository/_async.py" = "litestar/contrib/sqlalchemy/repository/_sync.py"
+"litestar/contrib/repository/abc/_async.py" = "litestar/contrib/repository/abc/_sync.py"
+
+[tool.unasyncd.per_file_add_replacements."litestar/contrib/repository/abc/_async.py"]
+"AbstractAsyncRepository" = "AbstractSyncRepository"
+"AsyncRepoT" = "SyncRepoT"
+
+[tool.unasyncd.per_file_add_replacements."litestar/contrib/sqlalchemy/repository/_async.py"]
+SQLAlchemyAsyncRepository = "SQLAlchemySyncRepository"
+"sqlalchemy.ext.asyncio.AsyncSession" = "sqlalchemy.orm.Session"
+"litestar.contrib.repository.AbstractAsyncRepository" = "litestar.contrib.repository.AbstractSyncRepository"
```

### Comparing `litestar-2.0.0a7/PKG-INFO` & `litestar-2.0.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: litestar
-Version: 2.0.0a7
-Summary: Performant, light and flexible ASGI API Framework
+Version: 2.0.0b1
+Summary: Litestar - A production-ready, highly performant, extensible ASGI API Framework
 Home-page: https://litestar.dev/
 License: MIT
 Keywords: api,rest,http,asgi,pydantic,litestar,starlite,framework,websocket,litestar
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
 Maintainer: Na'aman Hirschfeld
 Maintainer-email: nhirschfeld@gmail.com
@@ -17,18 +17,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 Provides-Extra: attrs
 Provides-Extra: brotli
 Provides-Extra: cli
@@ -65,26 +61,32 @@
 Requires-Dist: pydantic (<2)
 Requires-Dist: python-dateutil ; extra == "attrs"
 Requires-Dist: python-jose ; extra == "jwt" or extra == "full"
 Requires-Dist: pytimeparse ; extra == "attrs" or extra == "full"
 Requires-Dist: pyyaml
 Requires-Dist: redis[hiredis] (>=4.4.4,!=4.5.0,!=4.5.1,!=4.5.2,!=4.5.3,!=4.5.5) ; extra == "redis" or extra == "full"
 Requires-Dist: rich (>=13.0.0) ; extra == "cli" or extra == "standard" or extra == "full"
+Requires-Dist: rich-click ; extra == "cli" or extra == "standard"
 Requires-Dist: sqlalchemy (>=2.0.12) ; extra == "sqlalchemy" or extra == "full"
 Requires-Dist: structlog ; extra == "structlog" or extra == "full"
 Requires-Dist: typing-extensions
-Requires-Dist: uvicorn[standard] (>=0.21.1,<0.22.0) ; extra == "cli" or extra == "standard" or extra == "full"
+Requires-Dist: uvicorn[standard] (>=0.22.0,<0.23.0) ; extra == "cli" or extra == "standard" or extra == "full"
+Project-URL: Blog, https://blog.litestar.dev
+Project-URL: Changelog, https://github.com/litestar-org/litestar/releases/
 Project-URL: Documentation, https://docs.litestar.dev/
+Project-URL: Discord, https://discord.gg/MmcwxztmQb
+Project-URL: Issue Tracker, https://github.com/litestar-org/litestar/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc
 Project-URL: Repository, https://github.com/litestar-org/litestar
+Project-URL: Reddit, https://www.reddit.com/r/litestarapi
+Project-URL: Twitter, https://twitter.com/LitestarAPI
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable -->
 <p align="center">
-  <img src="artwork/banner-light.svg#gh-light-mode-only" alt="Litestar Logo - Light" width="100%" height="auto" />
-  <img src="artwork/banner-dark.svg#gh-dark-mode-only" alt="Litestar Logo - Dark" width="100%" height="auto" />
+  <img src="artwork/banner-light.svg" alt="Litestar Logo - Light" width="100%" height="auto" />
 </p>
 <!-- markdownlint-restore -->
 
 <div align="center">
 
 [![ci](https://github.com/litestar-org/litestar/actions/workflows/ci.yaml/badge.svg)](https://github.com/litestar-org/litestar/actions/workflows/ci.yaml)
 [![PyPI - Version](https://badge.fury.io/py/litestar.svg)](https://badge.fury.io/py/litestar)
@@ -95,15 +97,15 @@
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 
 <!-- prettier-ignore-start -->
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-101-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-102-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 <!-- prettier-ignore-end -->
 
 [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestarapi?label=r%2FLitestar&logo=reddit)](https://reddit.com/r/litestarapi)
 [![Discord](https://img.shields.io/discord/919193495116337154?color=blue&label=chat%20on%20discord&logo=discord)](https://discord.gg/X3FJqy8d2j)
 [![Matrix](https://img.shields.io/badge/%5Bm%5D%20chat%20on%20Matrix-bridged-blue)](https://matrix.to/#/#litestar:matrix.org)
 [![Medium](https://img.shields.io/badge/Medium-12100E?style=flat&logo=medium&logoColor=white)](https://blog.litestar.dev)
@@ -128,15 +130,15 @@
 pip install litestar
 ```
 
 **Litestar 2.0 is coming out soon**, bringing many new features and improvements.
 You can check out the alpha version by instead running
 
 ```shell
-pip install litestar==2.0.0alpha6
+pip install litestar==2.0.0alpha7
 ```
 
 ## Quick Start
 
 ```python
 from litestar import Litestar, get
 
@@ -489,14 +491,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://sanderwegter.nl"><img src="https://avatars.githubusercontent.com/u/7465799?v=4?s=100" width="100px;" alt="Sander"/><br /><sub><b>Sander</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=SanderWegter" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/erhuabushuo"><img src="https://avatars.githubusercontent.com/u/1642364?v=4?s=100" width="100px;" alt="疯人院主任"/><br /><sub><b>疯人院主任</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=erhuabushuo" title="Documentation">📖</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/aviral-nayya"><img src="https://avatars.githubusercontent.com/u/121891493?v=4?s=100" width="100px;" alt="aviral-nayya"/><br /><sub><b>aviral-nayya</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=aviral-nayya" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/whiskeyriver"><img src="https://avatars.githubusercontent.com/u/162092?v=4?s=100" width="100px;" alt="whiskeyriver"/><br /><sub><b>whiskeyriver</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=whiskeyriver" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://hexcode.tech"><img src="https://avatars.githubusercontent.com/u/419606?v=4?s=100" width="100px;" alt="Phyo Arkar Lwin"/><br /><sub><b>Phyo Arkar Lwin</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=v3ss0n" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/MatthewNewland"><img src="https://avatars.githubusercontent.com/u/9618670?v=4?s=100" width="100px;" alt="MatthewNewland"/><br /><sub><b>MatthewNewland</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3AMatthewNewland" title="Bug reports">🐛</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

