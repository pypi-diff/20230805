# Comparing `tmp/litestar-2.0.0b4.tar.gz` & `tmp/litestar-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litestar-2.0.0b4.tar", max compression
+gzip compressed data, was "litestar-2.0.0rc1.tar", max compression
```

## Comparing `litestar-2.0.0b4.tar` & `litestar-2.0.0rc1.tar`

### file list

```diff
@@ -1,312 +1,307 @@
--rw-r--r--   0        0        0     1092 2023-07-21 15:49:23.812703 litestar-2.0.0b4/LICENSE
--rw-r--r--   0        0        0    16790 2023-07-21 15:49:23.816703 litestar-2.0.0b4/docs/PYPI_README.md
--rw-r--r--   0        0        0      744 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/__init__.py
--rw-r--r--   0        0        0      228 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/__main__.py
--rw-r--r--   0        0        0       77 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_asgi/__init__.py
--rw-r--r--   0        0        0     6395 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_asgi/asgi_router.py
--rw-r--r--   0        0        0      349 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_asgi/routing_trie/__init__.py
--rw-r--r--   0        0        0     7780 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_asgi/routing_trie/mapping.py
--rw-r--r--   0        0        0     5932 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_asgi/routing_trie/traversal.py
--rw-r--r--   0        0        0     2598 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_asgi/routing_trie/types.py
--rw-r--r--   0        0        0     1244 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_asgi/routing_trie/validate.py
--rw-r--r--   0        0        0     1528 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_asgi/utils.py
--rw-r--r--   0        0        0       66 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_kwargs/__init__.py
--rw-r--r--   0        0        0     3842 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_kwargs/cleanup.py
--rw-r--r--   0        0        0     4234 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_kwargs/dependencies.py
--rw-r--r--   0        0        0    14983 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_kwargs/extractors.py
--rw-r--r--   0        0        0    20484 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_kwargs/kwargs_model.py
--rw-r--r--   0        0        0     2808 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_kwargs/parameter_definition.py
--rw-r--r--   0        0        0        0 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_layers/__init__.py
--rw-r--r--   0        0        0     1288 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_layers/utils.py
--rw-r--r--   0        0        0     6165 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_multipart.py
--rw-r--r--   0        0        0        0 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/__init__.py
--rw-r--r--   0        0        0     9202 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/parameters.py
--rw-r--r--   0        0        0     5536 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/path_item.py
--rw-r--r--   0        0        0     1231 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/request_body.py
--rw-r--r--   0        0        0     9743 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/responses.py
--rw-r--r--   0        0        0       64 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/schema_generation/__init__.py
--rw-r--r--   0        0        0     3250 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/schema_generation/constrained_fields.py
--rw-r--r--   0        0        0     2250 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/schema_generation/examples.py
--rw-r--r--   0        0        0    24613 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/schema_generation/schema.py
--rw-r--r--   0        0        0      524 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/schema_generation/utils.py
--rw-r--r--   0        0        0        0 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/typescript_converter/__init__.py
--rw-r--r--   0        0        0    10909 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/typescript_converter/converter.py
--rw-r--r--   0        0        0     5220 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/typescript_converter/schema_parsing.py
--rw-r--r--   0        0        0     7664 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/typescript_converter/types.py
--rw-r--r--   0        0        0     1460 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/utils.py
--rw-r--r--   0        0        0     2396 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_parsers.py
--rw-r--r--   0        0        0      126 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_signature/__init__.py
--rw-r--r--   0        0        0    10095 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_signature/model.py
--rw-r--r--   0        0        0     2718 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_signature/utils.py
--rw-r--r--   0        0        0    36944 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/app.py
--rw-r--r--   0        0        0     2200 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/background_tasks.py
--rw-r--r--   0        0        0      176 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/channels/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/channels/backends/__init__.py
--rw-r--r--   0        0        0      346 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/channels/backends/_redis_flushall_streams.lua
--rw-r--r--   0        0        0      101 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/channels/backends/_redis_pubsub_publish.lua
--rw-r--r--   0        0        0      401 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/channels/backends/_redis_xadd_expire.lua
--rw-r--r--   0        0        0     1300 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/channels/backends/base.py
--rw-r--r--   0        0        0     2750 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/channels/backends/memory.py
--rw-r--r--   0        0        0     9395 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/channels/backends/redis.py
--rw-r--r--   0        0        0    15702 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/channels/plugin.py
--rw-r--r--   0        0        0     4647 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/channels/subscriber.py
--rw-r--r--   0        0        0      119 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/cli/__init__.py
--rw-r--r--   0        0        0    12672 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/cli/_utils.py
--rw-r--r--   0        0        0        0 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/cli/commands/__init__.py
--rw-r--r--   0        0        0     6631 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/cli/commands/core.py
--rw-r--r--   0        0        0     2314 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/cli/commands/schema.py
--rw-r--r--   0        0        0     2413 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/cli/commands/sessions.py
--rw-r--r--   0        0        0     2183 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/cli/main.py
--rw-r--r--   0        0        0        0 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/config/__init__.py
--rw-r--r--   0        0        0     1747 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/config/allowed_hosts.py
--rw-r--r--   0        0        0    11706 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/config/app.py
--rw-r--r--   0        0        0     2742 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/config/compression.py
--rw-r--r--   0        0        0     5178 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/config/cors.py
--rw-r--r--   0        0        0     1771 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/config/csrf.py
--rw-r--r--   0        0        0     2005 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/config/response_cache.py
--rw-r--r--   0        0        0     1922 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/connection/__init__.py
--rw-r--r--   0        0        0    10791 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/connection/base.py
--rw-r--r--   0        0        0     7756 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/connection/request.py
--rw-r--r--   0        0        0    11530 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/connection/websocket.py
--rw-r--r--   0        0        0     1622 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/constants.py
--rw-r--r--   0        0        0        0 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/__init__.py
--rw-r--r--   0        0        0       85 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/attrs/__init__.py
--rw-r--r--   0        0        0     2096 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/attrs/attrs_schema_plugin.py
--rw-r--r--   0        0        0        0 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/htmx/__init__.py
--rw-r--r--   0        0        0     4800 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/htmx/_utils.py
--rw-r--r--   0        0        0     4167 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/htmx/request.py
--rw-r--r--   0        0        0     6408 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/htmx/response.py
--rw-r--r--   0        0        0     1261 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/htmx/types.py
--rw-r--r--   0        0        0     2557 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/jinja.py
--rw-r--r--   0        0        0      521 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/jwt/__init__.py
--rw-r--r--   0        0        0    28722 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/jwt/jwt_auth.py
--rw-r--r--   0        0        0     4373 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/jwt/jwt_token.py
--rw-r--r--   0        0        0     6953 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/jwt/middleware.py
--rw-r--r--   0        0        0     3983 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/mako.py
--rw-r--r--   0        0        0      683 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/msgspec.py
--rw-r--r--   0        0        0      180 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/opentelemetry/__init__.py
--rw-r--r--   0        0        0      845 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/opentelemetry/_utils.py
--rw-r--r--   0        0        0     4235 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/opentelemetry/config.py
--rw-r--r--   0        0        0     2214 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/opentelemetry/middleware.py
--rw-r--r--   0        0        0     3168 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/piccolo.py
--rw-r--r--   0        0        0      207 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/prometheus/__init__.py
--rw-r--r--   0        0        0     2733 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/prometheus/config.py
--rw-r--r--   0        0        0     1646 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/prometheus/controller.py
--rw-r--r--   0        0        0     6873 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/prometheus/middleware.py
--rw-r--r--   0        0        0      808 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/pydantic/__init__.py
--rw-r--r--   0        0        0     3011 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/pydantic/pydantic_dto_factory.py
--rw-r--r--   0        0        0     4571 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/pydantic/pydantic_init_plugin.py
--rw-r--r--   0        0        0     8802 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/pydantic/pydantic_schema_plugin.py
--rw-r--r--   0        0        0      364 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/repository/__init__.py
--rw-r--r--   0        0        0      162 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/repository/abc/__init__.py
--rw-r--r--   0        0        0     8889 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/repository/abc/_async.py
--rw-r--r--   0        0        0     8907 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/repository/abc/_sync.py
--rw-r--r--   0        0        0      328 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/repository/exceptions.py
--rw-r--r--   0        0        0     2064 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/repository/filters.py
--rw-r--r--   0        0        0      641 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/repository/handlers.py
--rw-r--r--   0        0        0        0 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/repository/testing/__init__.py
--rw-r--r--   0        0        0    25918 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/repository/testing/generic_mock_repository.py
--rw-r--r--   0        0        0        0 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5668 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/base.py
--rw-r--r--   0        0        0    11308 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/dto.py
--rw-r--r--   0        0        0      941 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/__init__.py
--rw-r--r--   0        0        0      319 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/_slots_base.py
--rw-r--r--   0        0        0      504 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/init/__init__.py
--rw-r--r--   0        0        0      458 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/init/config/__init__.py
--rw-r--r--   0        0        0     4541 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py
--rw-r--r--   0        0        0    11418 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/init/config/common.py
--rw-r--r--   0        0        0    11483 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/init/config/engine.py
--rw-r--r--   0        0        0     3753 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/init/config/sync.py
--rw-r--r--   0        0        0     1647 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/init/plugin.py
--rw-r--r--   0        0        0     1505 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/serialization.py
--rw-r--r--   0        0        0      288 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/repository/__init__.py
--rw-r--r--   0        0        0    28708 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/repository/_async.py
--rw-r--r--   0        0        0    28402 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/repository/_sync.py
--rw-r--r--   0        0        0     1033 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/repository/_util.py
--rw-r--r--   0        0        0      754 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/repository/types.py
--rw-r--r--   0        0        0     6327 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/types.py
--rw-r--r--   0        0        0     9762 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/controller.py
--rw-r--r--   0        0        0    16456 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/data_extractors.py
--rw-r--r--   0        0        0      883 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/datastructures/__init__.py
--rw-r--r--   0        0        0     3770 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/datastructures/cookie.py
--rw-r--r--   0        0        0    18809 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/datastructures/headers.py
--rw-r--r--   0        0        0     2977 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/datastructures/multi_dicts.py
--rw-r--r--   0        0        0     5027 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/datastructures/response_header.py
--rw-r--r--   0        0        0     9646 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/datastructures/state.py
--rw-r--r--   0        0        0     2695 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/datastructures/upload_file.py
--rw-r--r--   0        0        0     7285 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/datastructures/url.py
--rw-r--r--   0        0        0     3117 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/di.py
--rw-r--r--   0        0        0      645 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/__init__.py
--rw-r--r--   0        0        0    21671 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/_backend.py
--rw-r--r--   0        0        0     4261 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/_types.py
--rw-r--r--   0        0        0    20517 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/_utils.py
--rw-r--r--   0        0        0     7288 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/base_factory.py
--rw-r--r--   0        0        0     2501 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/config.py
--rw-r--r--   0        0        0     4858 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/data_structures.py
--rw-r--r--   0        0        0     2507 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/dataclass_dto_factory.py
--rw-r--r--   0        0        0     1325 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/factory/__init__.py
--rw-r--r--   0        0        0      701 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/factory/stdlib/dataclass.py
--rw-r--r--   0        0        0     1388 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/field.py
--rw-r--r--   0        0        0     4948 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/interface.py
--rw-r--r--   0        0        0     2113 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/msgspec_dto_factory.py
--rw-r--r--   0        0        0      516 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/types.py
--rw-r--r--   0        0        0     1728 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/enums.py
--rw-r--r--   0        0        0      201 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/events/__init__.py
--rw-r--r--   0        0        0     4371 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/events/emitter.py
--rw-r--r--   0        0        0     1313 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/events/listener.py
--rw-r--r--   0        0        0     1302 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/exceptions/__init__.py
--rw-r--r--   0        0        0     1721 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/exceptions/base_exceptions.py
--rw-r--r--   0        0        0      331 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/exceptions/dto_exceptions.py
--rw-r--r--   0        0        0     4629 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/exceptions/http_exceptions.py
--rw-r--r--   0        0        0     1351 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/exceptions/websocket_exceptions.py
--rw-r--r--   0        0        0     5344 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/file_system.py
--rw-r--r--   0        0        0      559 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/handlers/__init__.py
--rw-r--r--   0        0        0     3868 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/handlers/asgi_handlers.py
--rw-r--r--   0        0        0    21575 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/handlers/base.py
--rw-r--r--   0        0        0      263 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/handlers/http_handlers/__init__.py
--rw-r--r--   0        0        0     6450 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/handlers/http_handlers/_utils.py
--rw-r--r--   0        0        0    26309 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/handlers/http_handlers/base.py
--rw-r--r--   0        0        0    62224 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/handlers/http_handlers/decorators.py
--rw-r--r--   0        0        0      340 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/handlers/websocket_handlers/__init__.py
--rw-r--r--   0        0        0     7217 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/handlers/websocket_handlers/_utils.py
--rw-r--r--   0        0        0    19092 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/handlers/websocket_handlers/listener.py
--rw-r--r--   0        0        0     3605 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/handlers/websocket_handlers/route_handler.py
--rw-r--r--   0        0        0      147 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/logging/__init__.py
--rw-r--r--   0        0        0      569 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/logging/_utils.py
--rw-r--r--   0        0        0    12215 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/logging/config.py
--rw-r--r--   0        0        0     1129 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/logging/picologging.py
--rw-r--r--   0        0        0      860 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/logging/standard.py
--rw-r--r--   0        0        0      385 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/__init__.py
--rw-r--r--   0        0        0     2079 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/_utils.py
--rw-r--r--   0        0        0     3021 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/allowed_hosts.py
--rw-r--r--   0        0        0     3430 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/authentication.py
--rw-r--r--   0        0        0     5284 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/base.py
--rw-r--r--   0        0        0     8454 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/compression.py
--rw-r--r--   0        0        0     2554 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/cors.py
--rw-r--r--   0        0        0     6438 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/csrf.py
--rw-r--r--   0        0        0      124 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/exceptions/__init__.py
--rw-r--r--   0        0        0     7141 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/exceptions/_debug_response.py
--rw-r--r--   0        0        0     9435 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/exceptions/middleware.py
--rw-r--r--   0        0        0      398 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/exceptions/templates/body.html
--rw-r--r--   0        0        0      344 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/exceptions/templates/frame.html
--rw-r--r--   0        0        0      920 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/exceptions/templates/scripts.js
--rw-r--r--   0        0        0     1830 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/exceptions/templates/styles.css
--rw-r--r--   0        0        0    13307 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/logging.py
--rw-r--r--   0        0        0    10817 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/rate_limit.py
--rw-r--r--   0        0        0       70 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/session/__init__.py
--rw-r--r--   0        0        0     7941 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/session/base.py
--rw-r--r--   0        0        0    10352 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/session/client_side.py
--rw-r--r--   0        0        0     8540 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/middleware/session/server_side.py
--rw-r--r--   0        0        0      183 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/__init__.py
--rw-r--r--   0        0        0     5600 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/config.py
--rw-r--r--   0        0        0    15653 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/controller.py
--rw-r--r--   0        0        0      724 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/datastructures.py
--rw-r--r--   0        0        0     1691 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/__init__.py
--rw-r--r--   0        0        0     1885 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/base.py
--rw-r--r--   0        0        0      961 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/callback.py
--rw-r--r--   0        0        0     2936 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/components.py
--rw-r--r--   0        0        0      592 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/contact.py
--rw-r--r--   0        0        0      950 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/discriminator.py
--rw-r--r--   0        0        0     3290 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/encoding.py
--rw-r--r--   0        0        0      974 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/enums.py
--rw-r--r--   0        0        0     1168 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/example.py
--rw-r--r--   0        0        0      614 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/external_documentation.py
--rw-r--r--   0        0        0     5669 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/header.py
--rw-r--r--   0        0        0     1413 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/info.py
--rw-r--r--   0        0        0      752 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/license.py
--rw-r--r--   0        0        0     2876 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/link.py
--rw-r--r--   0        0        0     1882 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/media_type.py
--rw-r--r--   0        0        0     1195 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/oauth_flow.py
--rw-r--r--   0        0        0      897 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/oauth_flows.py
--rw-r--r--   0        0        0     4028 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/open_api.py
--rw-r--r--   0        0        0     4842 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/operation.py
--rw-r--r--   0        0        0     6242 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/parameter.py
--rw-r--r--   0        0        0     3245 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/path_item.py
--rw-r--r--   0        0        0     1255 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/paths.py
--rw-r--r--   0        0        0     1351 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/reference.py
--rw-r--r--   0        0        0     1095 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/request_body.py
--rw-r--r--   0        0        0     1854 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/response.py
--rw-r--r--   0        0        0     2367 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/responses.py
--rw-r--r--   0        0        0    34581 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/schema.py
--rw-r--r--   0        0        0     1686 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/security_requirement.py
--rw-r--r--   0        0        0     2690 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/security_scheme.py
--rw-r--r--   0        0        0     1077 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/server.py
--rw-r--r--   0        0        0     1171 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/server_variable.py
--rw-r--r--   0        0        0      923 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/tag.py
--rw-r--r--   0        0        0     1702 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/xml.py
--rw-r--r--   0        0        0    11029 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/pagination.py
--rw-r--r--   0        0        0    15113 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/params.py
--rw-r--r--   0        0        0     7433 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/partial.py
--rw-r--r--   0        0        0     3923 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/plugins.py
--rw-r--r--   0        0        0        0 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/py.typed
--rw-r--r--   0        0        0      208 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/response/__init__.py
--rw-r--r--   0        0        0    15238 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/response/base.py
--rw-r--r--   0        0        0    14298 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/response/file.py
--rw-r--r--   0        0        0     5440 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/response/redirect.py
--rw-r--r--   0        0        0     7956 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/response/streaming.py
--rw-r--r--   0        0        0     5229 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/response/template.py
--rw-r--r--   0        0        0    15308 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/router.py
--rw-r--r--   0        0        0      191 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/routes/__init__.py
--rw-r--r--   0        0        0     1719 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/routes/asgi.py
--rw-r--r--   0        0        0     6788 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/routes/base.py
--rw-r--r--   0        0        0    13224 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/routes/http.py
--rw-r--r--   0        0        0     3002 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/routes/websocket.py
--rw-r--r--   0        0        0       97 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/security/__init__.py
--rw-r--r--   0        0        0     7165 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/security/base.py
--rw-r--r--   0        0        0      188 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/security/session_auth/__init__.py
--rw-r--r--   0        0        0     5602 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/security/session_auth/auth.py
--rw-r--r--   0        0        0     4956 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/security/session_auth/middleware.py
--rw-r--r--   0        0        0      348 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/serialization/__init__.py
--rw-r--r--   0        0        0      277 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/serialization/_msgspec_utils.py
--rw-r--r--   0        0        0     7755 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/serialization/msgspec_hooks.py
--rw-r--r--   0        0        0      158 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/static_files/__init__.py
--rw-r--r--   0        0        0     5046 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/static_files/base.py
--rw-r--r--   0        0        0     3598 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/static_files/config.py
--rw-r--r--   0        0        0     9536 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/status_codes.py
--rw-r--r--   0        0        0        0 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/stores/__init__.py
--rw-r--r--   0        0        0     4396 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/stores/base.py
--rw-r--r--   0        0        0     5430 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/stores/file.py
--rw-r--r--   0        0        0     3625 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/stores/memory.py
--rw-r--r--   0        0        0     6208 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/stores/redis.py
--rw-r--r--   0        0        0     2216 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/stores/registry.py
--rw-r--r--   0        0        0      204 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/template/__init__.py
--rw-r--r--   0        0        0     4083 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/template/base.py
--rw-r--r--   0        0        0     1894 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/template/config.py
--rw-r--r--   0        0        0      581 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/testing/__init__.py
--rw-r--r--   0        0        0     1816 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/testing/client/__init__.py
--rw-r--r--   0        0        0    17562 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/testing/client/async_client.py
--rw-r--r--   0        0        0     5145 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/testing/client/base.py
--rw-r--r--   0        0        0    19671 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/testing/client/sync_client.py
--rw-r--r--   0        0        0    29713 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/testing/helpers.py
--rw-r--r--   0        0        0     2540 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/testing/life_span_handler.py
--rw-r--r--   0        0        0    22456 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/testing/request_factory.py
--rw-r--r--   0        0        0     8056 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/testing/transport.py
--rw-r--r--   0        0        0     8564 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/testing/websocket_test_session.py
--rw-r--r--   0        0        0     4171 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/types/__init__.py
--rw-r--r--   0        0        0     8937 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/types/asgi_types.py
--rw-r--r--   0        0        0      566 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/types/builtin_types.py
--rw-r--r--   0        0        0     2962 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/types/callable_types.py
--rw-r--r--   0        0        0     1782 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/types/composite_types.py
--rw-r--r--   0        0        0      286 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/types/empty.py
--rw-r--r--   0        0        0     2635 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/types/file_types.py
--rw-r--r--   0        0        0      918 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/types/helper_types.py
--rw-r--r--   0        0        0     1751 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/types/internal_types.py
--rw-r--r--   0        0        0     2984 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/types/protocols.py
--rw-r--r--   0        0        0     2039 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/types/serialization.py
--rw-r--r--   0        0        0    20917 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/typing.py
--rw-r--r--   0        0        0     2167 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/__init__.py
--rw-r--r--   0        0        0      729 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/compat.py
--rw-r--r--   0        0        0     3763 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/dataclass.py
--rw-r--r--   0        0        0     3553 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/deprecation.py
--rw-r--r--   0        0        0     3334 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/helpers.py
--rw-r--r--   0        0        0      723 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/path.py
--rw-r--r--   0        0        0    12498 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/predicates.py
--rw-r--r--   0        0        0     2789 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/scope.py
--rw-r--r--   0        0        0      983 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/sequence.py
--rw-r--r--   0        0        0     5521 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/signature.py
--rw-r--r--   0        0        0     4374 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/sync.py
--rw-r--r--   0        0        0     8299 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/typing.py
--rw-r--r--   0        0        0     1921 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/version.py
--rw-r--r--   0        0        0     1992 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/warnings.py
--rw-r--r--   0        0        0    13677 2023-07-21 15:49:23.856704 litestar-2.0.0b4/pyproject.toml
--rw-r--r--   0        0        0    21540 1970-01-01 00:00:00.000000 litestar-2.0.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-08-05 15:12:52.511124 litestar-2.0.0rc1/LICENSE
+-rw-r--r--   0        0        0    16810 2023-08-05 15:12:52.511124 litestar-2.0.0rc1/docs/PYPI_README.md
+-rw-r--r--   0        0        0      744 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/__init__.py
+-rw-r--r--   0        0        0      228 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/__main__.py
+-rw-r--r--   0        0        0       77 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_asgi/__init__.py
+-rw-r--r--   0        0        0     6395 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_asgi/asgi_router.py
+-rw-r--r--   0        0        0      349 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_asgi/routing_trie/__init__.py
+-rw-r--r--   0        0        0     7780 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_asgi/routing_trie/mapping.py
+-rw-r--r--   0        0        0     5932 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_asgi/routing_trie/traversal.py
+-rw-r--r--   0        0        0     2598 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_asgi/routing_trie/types.py
+-rw-r--r--   0        0        0     1244 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_asgi/routing_trie/validate.py
+-rw-r--r--   0        0        0     1528 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_asgi/utils.py
+-rw-r--r--   0        0        0       66 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_kwargs/__init__.py
+-rw-r--r--   0        0        0     3842 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_kwargs/cleanup.py
+-rw-r--r--   0        0        0     4177 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_kwargs/dependencies.py
+-rw-r--r--   0        0        0    14706 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_kwargs/extractors.py
+-rw-r--r--   0        0        0    20211 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_kwargs/kwargs_model.py
+-rw-r--r--   0        0        0     2808 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_kwargs/parameter_definition.py
+-rw-r--r--   0        0        0        0 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_layers/__init__.py
+-rw-r--r--   0        0        0     1288 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_layers/utils.py
+-rw-r--r--   0        0        0     6241 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_multipart.py
+-rw-r--r--   0        0        0        0 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_openapi/__init__.py
+-rw-r--r--   0        0        0     9202 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_openapi/parameters.py
+-rw-r--r--   0        0        0     5847 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_openapi/path_item.py
+-rw-r--r--   0        0        0     1372 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_openapi/request_body.py
+-rw-r--r--   0        0        0     9872 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_openapi/responses.py
+-rw-r--r--   0        0        0       64 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_openapi/schema_generation/__init__.py
+-rw-r--r--   0        0        0     3249 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_openapi/schema_generation/constrained_fields.py
+-rw-r--r--   0        0        0     2249 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_openapi/schema_generation/examples.py
+-rw-r--r--   0        0        0    23915 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_openapi/schema_generation/schema.py
+-rw-r--r--   0        0        0      524 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_openapi/schema_generation/utils.py
+-rw-r--r--   0        0        0        0 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_openapi/typescript_converter/__init__.py
+-rw-r--r--   0        0        0    10909 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_openapi/typescript_converter/converter.py
+-rw-r--r--   0        0        0     5220 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_openapi/typescript_converter/schema_parsing.py
+-rw-r--r--   0        0        0     7664 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_openapi/typescript_converter/types.py
+-rw-r--r--   0        0        0     1489 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_openapi/utils.py
+-rw-r--r--   0        0        0     2396 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_parsers.py
+-rw-r--r--   0        0        0       65 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_signature/__init__.py
+-rw-r--r--   0        0        0    11376 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_signature/model.py
+-rw-r--r--   0        0        0      277 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_signature/types.py
+-rw-r--r--   0        0        0     2102 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/_signature/utils.py
+-rw-r--r--   0        0        0    37288 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/app.py
+-rw-r--r--   0        0        0     2200 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/background_tasks.py
+-rw-r--r--   0        0        0      176 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/channels/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/channels/backends/__init__.py
+-rw-r--r--   0        0        0      346 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/channels/backends/_redis_flushall_streams.lua
+-rw-r--r--   0        0        0      101 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/channels/backends/_redis_pubsub_publish.lua
+-rw-r--r--   0        0        0      401 2023-08-05 15:12:52.543127 litestar-2.0.0rc1/litestar/channels/backends/_redis_xadd_expire.lua
+-rw-r--r--   0        0        0     1300 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/channels/backends/base.py
+-rw-r--r--   0        0        0     2750 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/channels/backends/memory.py
+-rw-r--r--   0        0        0     9395 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/channels/backends/redis.py
+-rw-r--r--   0        0        0    15776 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/channels/plugin.py
+-rw-r--r--   0        0        0     4647 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/channels/subscriber.py
+-rw-r--r--   0        0        0      119 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/cli/__init__.py
+-rw-r--r--   0        0        0    13649 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/cli/_utils.py
+-rw-r--r--   0        0        0        0 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/cli/commands/__init__.py
+-rw-r--r--   0        0        0     6795 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/cli/commands/core.py
+-rw-r--r--   0        0        0     2334 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/cli/commands/schema.py
+-rw-r--r--   0        0        0     2433 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/cli/commands/sessions.py
+-rw-r--r--   0        0        0     2287 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/cli/main.py
+-rw-r--r--   0        0        0        0 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/config/__init__.py
+-rw-r--r--   0        0        0     1747 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/config/allowed_hosts.py
+-rw-r--r--   0        0        0    11687 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/config/app.py
+-rw-r--r--   0        0        0     2742 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/config/compression.py
+-rw-r--r--   0        0        0     5178 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/config/cors.py
+-rw-r--r--   0        0        0     1771 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/config/csrf.py
+-rw-r--r--   0        0        0     2005 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/config/response_cache.py
+-rw-r--r--   0        0        0     1922 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/connection/__init__.py
+-rw-r--r--   0        0        0    10791 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/connection/base.py
+-rw-r--r--   0        0        0     7756 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/connection/request.py
+-rw-r--r--   0        0        0    11530 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/connection/websocket.py
+-rw-r--r--   0        0        0     1622 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/constants.py
+-rw-r--r--   0        0        0        0 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/__init__.py
+-rw-r--r--   0        0        0       85 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/attrs/__init__.py
+-rw-r--r--   0        0        0     2052 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/attrs/attrs_schema_plugin.py
+-rw-r--r--   0        0        0        0 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/htmx/__init__.py
+-rw-r--r--   0        0        0     4800 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/htmx/_utils.py
+-rw-r--r--   0        0        0     4167 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/htmx/request.py
+-rw-r--r--   0        0        0     6408 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/htmx/response.py
+-rw-r--r--   0        0        0     1261 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/htmx/types.py
+-rw-r--r--   0        0        0     2557 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/jinja.py
+-rw-r--r--   0        0        0      521 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/jwt/__init__.py
+-rw-r--r--   0        0        0    28722 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/jwt/jwt_auth.py
+-rw-r--r--   0        0        0     4373 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/jwt/jwt_token.py
+-rw-r--r--   0        0        0     6953 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/jwt/middleware.py
+-rw-r--r--   0        0        0     3983 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/mako.py
+-rw-r--r--   0        0        0      180 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      845 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/opentelemetry/_utils.py
+-rw-r--r--   0        0        0     4235 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/opentelemetry/config.py
+-rw-r--r--   0        0        0     2214 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/opentelemetry/middleware.py
+-rw-r--r--   0        0        0     2982 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/piccolo.py
+-rw-r--r--   0        0        0      207 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/prometheus/__init__.py
+-rw-r--r--   0        0        0     2733 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/prometheus/config.py
+-rw-r--r--   0        0        0     1646 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/prometheus/controller.py
+-rw-r--r--   0        0        0     6873 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/prometheus/middleware.py
+-rw-r--r--   0        0        0      808 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/pydantic/__init__.py
+-rw-r--r--   0        0        0     2732 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/pydantic/pydantic_dto_factory.py
+-rw-r--r--   0        0        0     4559 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/pydantic/pydantic_init_plugin.py
+-rw-r--r--   0        0        0     8673 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/pydantic/pydantic_schema_plugin.py
+-rw-r--r--   0        0        0      364 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/repository/__init__.py
+-rw-r--r--   0        0        0      162 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/repository/abc/__init__.py
+-rw-r--r--   0        0        0    10158 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/repository/abc/_async.py
+-rw-r--r--   0        0        0    10170 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/repository/abc/_sync.py
+-rw-r--r--   0        0        0      328 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/repository/exceptions.py
+-rw-r--r--   0        0        0     3194 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/repository/filters.py
+-rw-r--r--   0        0        0      916 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/repository/handlers.py
+-rw-r--r--   0        0        0        0 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/repository/testing/__init__.py
+-rw-r--r--   0        0        0    28118 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/repository/testing/generic_mock_repository.py
+-rw-r--r--   0        0        0        0 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5668 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/sqlalchemy/base.py
+-rw-r--r--   0        0        0    11524 2023-08-05 15:12:52.547127 litestar-2.0.0rc1/litestar/contrib/sqlalchemy/dto.py
+-rw-r--r--   0        0        0      941 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/contrib/sqlalchemy/plugins/__init__.py
+-rw-r--r--   0        0        0      319 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/contrib/sqlalchemy/plugins/_slots_base.py
+-rw-r--r--   0        0        0      504 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/contrib/sqlalchemy/plugins/init/__init__.py
+-rw-r--r--   0        0        0      458 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/contrib/sqlalchemy/plugins/init/config/__init__.py
+-rw-r--r--   0        0        0     4541 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py
+-rw-r--r--   0        0        0    11418 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/contrib/sqlalchemy/plugins/init/config/common.py
+-rw-r--r--   0        0        0    11483 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/contrib/sqlalchemy/plugins/init/config/engine.py
+-rw-r--r--   0        0        0     3753 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/contrib/sqlalchemy/plugins/init/config/sync.py
+-rw-r--r--   0        0        0     1627 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/contrib/sqlalchemy/plugins/init/plugin.py
+-rw-r--r--   0        0        0     1485 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/contrib/sqlalchemy/plugins/serialization.py
+-rw-r--r--   0        0        0      288 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/contrib/sqlalchemy/repository/__init__.py
+-rw-r--r--   0        0        0    41588 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/contrib/sqlalchemy/repository/_async.py
+-rw-r--r--   0        0        0    41223 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/contrib/sqlalchemy/repository/_sync.py
+-rw-r--r--   0        0        0     1416 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/contrib/sqlalchemy/repository/_util.py
+-rw-r--r--   0        0        0      754 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/contrib/sqlalchemy/repository/types.py
+-rw-r--r--   0        0        0     6327 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/contrib/sqlalchemy/types.py
+-rw-r--r--   0        0        0     9510 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/controller.py
+-rw-r--r--   0        0        0    16456 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/data_extractors.py
+-rw-r--r--   0        0        0      883 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/datastructures/__init__.py
+-rw-r--r--   0        0        0     3770 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/datastructures/cookie.py
+-rw-r--r--   0        0        0    18812 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/datastructures/headers.py
+-rw-r--r--   0        0        0     2977 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/datastructures/multi_dicts.py
+-rw-r--r--   0        0        0     5027 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/datastructures/response_header.py
+-rw-r--r--   0        0        0     9646 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/datastructures/state.py
+-rw-r--r--   0        0        0     2695 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/datastructures/upload_file.py
+-rw-r--r--   0        0        0     7285 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/datastructures/url.py
+-rw-r--r--   0        0        0     3372 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/di.py
+-rw-r--r--   0        0        0      473 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/dto/__init__.py
+-rw-r--r--   0        0        0    32042 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/dto/_backend.py
+-rw-r--r--   0        0        0     4155 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/dto/_types.py
+-rw-r--r--   0        0        0    12489 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/dto/base_dto.py
+-rw-r--r--   0        0        0     2501 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/dto/config.py
+-rw-r--r--   0        0        0     3905 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/dto/data_structures.py
+-rw-r--r--   0        0        0     2229 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/dto/dataclass_dto.py
+-rw-r--r--   0        0        0     1388 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/dto/field.py
+-rw-r--r--   0        0        0     1846 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/dto/msgspec_dto.py
+-rw-r--r--   0        0        0      386 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/dto/types.py
+-rw-r--r--   0        0        0     1728 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/enums.py
+-rw-r--r--   0        0        0      201 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/events/__init__.py
+-rw-r--r--   0        0        0     4488 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/events/emitter.py
+-rw-r--r--   0        0        0     1313 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/events/listener.py
+-rw-r--r--   0        0        0     1302 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/exceptions/__init__.py
+-rw-r--r--   0        0        0     1721 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/exceptions/base_exceptions.py
+-rw-r--r--   0        0        0      331 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/exceptions/dto_exceptions.py
+-rw-r--r--   0        0        0     4629 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/exceptions/http_exceptions.py
+-rw-r--r--   0        0        0     1351 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/exceptions/websocket_exceptions.py
+-rw-r--r--   0        0        0     5344 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/file_system.py
+-rw-r--r--   0        0        0      652 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/handlers/__init__.py
+-rw-r--r--   0        0        0     3868 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/handlers/asgi_handlers.py
+-rw-r--r--   0        0        0    21425 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/handlers/base.py
+-rw-r--r--   0        0        0      263 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/handlers/http_handlers/__init__.py
+-rw-r--r--   0        0        0     6450 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/handlers/http_handlers/_utils.py
+-rw-r--r--   0        0        0    26124 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/handlers/http_handlers/base.py
+-rw-r--r--   0        0        0    62332 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/handlers/http_handlers/decorators.py
+-rw-r--r--   0        0        0      425 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/handlers/websocket_handlers/__init__.py
+-rw-r--r--   0        0        0     6166 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/handlers/websocket_handlers/_utils.py
+-rw-r--r--   0        0        0    17515 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/handlers/websocket_handlers/listener.py
+-rw-r--r--   0        0        0     3588 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/handlers/websocket_handlers/route_handler.py
+-rw-r--r--   0        0        0      147 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/logging/__init__.py
+-rw-r--r--   0        0        0      569 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/logging/_utils.py
+-rw-r--r--   0        0        0    12215 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/logging/config.py
+-rw-r--r--   0        0        0     1129 2023-08-05 15:12:52.551128 litestar-2.0.0rc1/litestar/logging/picologging.py
+-rw-r--r--   0        0        0      860 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/logging/standard.py
+-rw-r--r--   0        0        0      385 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/middleware/__init__.py
+-rw-r--r--   0        0        0     2079 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/middleware/_utils.py
+-rw-r--r--   0        0        0     3021 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/middleware/allowed_hosts.py
+-rw-r--r--   0        0        0     3430 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/middleware/authentication.py
+-rw-r--r--   0        0        0     5284 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/middleware/base.py
+-rw-r--r--   0        0        0     8454 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/middleware/compression.py
+-rw-r--r--   0        0        0     2554 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/middleware/cors.py
+-rw-r--r--   0        0        0     6438 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/middleware/csrf.py
+-rw-r--r--   0        0        0      124 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/middleware/exceptions/__init__.py
+-rw-r--r--   0        0        0     7370 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/middleware/exceptions/_debug_response.py
+-rw-r--r--   0        0        0     9438 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/middleware/exceptions/middleware.py
+-rw-r--r--   0        0        0      398 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/middleware/exceptions/templates/body.html
+-rw-r--r--   0        0        0      344 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/middleware/exceptions/templates/frame.html
+-rw-r--r--   0        0        0      920 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/middleware/exceptions/templates/scripts.js
+-rw-r--r--   0        0        0     1830 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/middleware/exceptions/templates/styles.css
+-rw-r--r--   0        0        0    13307 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/middleware/logging.py
+-rw-r--r--   0        0        0    10817 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/middleware/rate_limit.py
+-rw-r--r--   0        0        0       70 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/middleware/session/__init__.py
+-rw-r--r--   0        0        0     7941 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/middleware/session/base.py
+-rw-r--r--   0        0        0    10352 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/middleware/session/client_side.py
+-rw-r--r--   0        0        0     8573 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/middleware/session/server_side.py
+-rw-r--r--   0        0        0      183 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/__init__.py
+-rw-r--r--   0        0        0     5600 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/config.py
+-rw-r--r--   0        0        0    15653 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/controller.py
+-rw-r--r--   0        0        0      724 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/datastructures.py
+-rw-r--r--   0        0        0     1691 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/__init__.py
+-rw-r--r--   0        0        0     1885 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/base.py
+-rw-r--r--   0        0        0      961 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/callback.py
+-rw-r--r--   0        0        0     2936 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/components.py
+-rw-r--r--   0        0        0      592 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/contact.py
+-rw-r--r--   0        0        0      950 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/discriminator.py
+-rw-r--r--   0        0        0     3290 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/encoding.py
+-rw-r--r--   0        0        0      974 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/enums.py
+-rw-r--r--   0        0        0     1168 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/example.py
+-rw-r--r--   0        0        0      614 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/external_documentation.py
+-rw-r--r--   0        0        0     5669 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/header.py
+-rw-r--r--   0        0        0     1413 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/info.py
+-rw-r--r--   0        0        0      752 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/license.py
+-rw-r--r--   0        0        0     2876 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/link.py
+-rw-r--r--   0        0        0     1882 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/media_type.py
+-rw-r--r--   0        0        0     1195 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/oauth_flow.py
+-rw-r--r--   0        0        0      897 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/oauth_flows.py
+-rw-r--r--   0        0        0     4028 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/open_api.py
+-rw-r--r--   0        0        0     4842 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/operation.py
+-rw-r--r--   0        0        0     6242 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/parameter.py
+-rw-r--r--   0        0        0     3245 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/path_item.py
+-rw-r--r--   0        0        0     1255 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/paths.py
+-rw-r--r--   0        0        0     1351 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/reference.py
+-rw-r--r--   0        0        0     1095 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/request_body.py
+-rw-r--r--   0        0        0     1854 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/response.py
+-rw-r--r--   0        0        0     2367 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/responses.py
+-rw-r--r--   0        0        0    34581 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/schema.py
+-rw-r--r--   0        0        0     1686 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/security_requirement.py
+-rw-r--r--   0        0        0     2690 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/security_scheme.py
+-rw-r--r--   0        0        0     1077 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/server.py
+-rw-r--r--   0        0        0     1171 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/server_variable.py
+-rw-r--r--   0        0        0      923 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/tag.py
+-rw-r--r--   0        0        0     1702 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/openapi/spec/xml.py
+-rw-r--r--   0        0        0    11029 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/pagination.py
+-rw-r--r--   0        0        0    15113 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/params.py
+-rw-r--r--   0        0        0     6475 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/plugins.py
+-rw-r--r--   0        0        0        0 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/py.typed
+-rw-r--r--   0        0        0      287 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/response/__init__.py
+-rw-r--r--   0        0        0    15205 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/response/base.py
+-rw-r--r--   0        0        0    14298 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/response/file.py
+-rw-r--r--   0        0        0     5440 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/response/redirect.py
+-rw-r--r--   0        0        0     5272 2023-08-05 15:12:52.555128 litestar-2.0.0rc1/litestar/response/sse.py
+-rw-r--r--   0        0        0     7956 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/response/streaming.py
+-rw-r--r--   0        0        0     5229 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/response/template.py
+-rw-r--r--   0        0        0    15289 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/router.py
+-rw-r--r--   0        0        0      191 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/routes/__init__.py
+-rw-r--r--   0        0        0     1719 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/routes/asgi.py
+-rw-r--r--   0        0        0     6681 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/routes/base.py
+-rw-r--r--   0        0        0    13330 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/routes/http.py
+-rw-r--r--   0        0        0     3002 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/routes/websocket.py
+-rw-r--r--   0        0        0       97 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/security/__init__.py
+-rw-r--r--   0        0        0     7165 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/security/base.py
+-rw-r--r--   0        0        0      188 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/security/session_auth/__init__.py
+-rw-r--r--   0        0        0     5602 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/security/session_auth/auth.py
+-rw-r--r--   0        0        0     4956 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/security/session_auth/middleware.py
+-rw-r--r--   0        0        0      348 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/serialization/__init__.py
+-rw-r--r--   0        0        0     7755 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/serialization/msgspec_hooks.py
+-rw-r--r--   0        0        0      158 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/static_files/__init__.py
+-rw-r--r--   0        0        0     5185 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/static_files/base.py
+-rw-r--r--   0        0        0     3598 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/static_files/config.py
+-rw-r--r--   0        0        0     9536 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/status_codes.py
+-rw-r--r--   0        0        0        0 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/stores/__init__.py
+-rw-r--r--   0        0        0     4396 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/stores/base.py
+-rw-r--r--   0        0        0     5430 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/stores/file.py
+-rw-r--r--   0        0        0     3625 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/stores/memory.py
+-rw-r--r--   0        0        0     6208 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/stores/redis.py
+-rw-r--r--   0        0        0     2216 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/stores/registry.py
+-rw-r--r--   0        0        0      204 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/template/__init__.py
+-rw-r--r--   0        0        0     4083 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/template/base.py
+-rw-r--r--   0        0        0     1894 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/template/config.py
+-rw-r--r--   0        0        0      581 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/testing/__init__.py
+-rw-r--r--   0        0        0     1816 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/testing/client/__init__.py
+-rw-r--r--   0        0        0    17562 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/testing/client/async_client.py
+-rw-r--r--   0        0        0     5145 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/testing/client/base.py
+-rw-r--r--   0        0        0    19670 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/testing/client/sync_client.py
+-rw-r--r--   0        0        0    29684 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/testing/helpers.py
+-rw-r--r--   0        0        0     2918 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/testing/life_span_handler.py
+-rw-r--r--   0        0        0    22456 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/testing/request_factory.py
+-rw-r--r--   0        0        0     8056 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/testing/transport.py
+-rw-r--r--   0        0        0     8564 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/testing/websocket_test_session.py
+-rw-r--r--   0        0        0     4171 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/types/__init__.py
+-rw-r--r--   0        0        0     8937 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/types/asgi_types.py
+-rw-r--r--   0        0        0      566 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/types/builtin_types.py
+-rw-r--r--   0        0        0     2962 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/types/callable_types.py
+-rw-r--r--   0        0        0     1783 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/types/composite_types.py
+-rw-r--r--   0        0        0      286 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/types/empty.py
+-rw-r--r--   0        0        0     2635 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/types/file_types.py
+-rw-r--r--   0        0        0      918 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/types/helper_types.py
+-rw-r--r--   0        0        0     1751 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/types/internal_types.py
+-rw-r--r--   0        0        0     2984 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/types/protocols.py
+-rw-r--r--   0        0        0     2039 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/types/serialization.py
+-rw-r--r--   0        0        0    22757 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/typing.py
+-rw-r--r--   0        0        0     2143 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/utils/__init__.py
+-rw-r--r--   0        0        0      729 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/utils/compat.py
+-rw-r--r--   0        0        0     3763 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/utils/dataclass.py
+-rw-r--r--   0        0        0     3553 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/utils/deprecation.py
+-rw-r--r--   0        0        0     3081 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/utils/helpers.py
+-rw-r--r--   0        0        0      723 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/utils/path.py
+-rw-r--r--   0        0        0    12498 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/utils/predicates.py
+-rw-r--r--   0        0        0     2789 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/utils/scope.py
+-rw-r--r--   0        0        0      745 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/utils/sequence.py
+-rw-r--r--   0        0        0     5381 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/utils/signature.py
+-rw-r--r--   0        0        0     4374 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/utils/sync.py
+-rw-r--r--   0        0        0     8462 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/utils/typing.py
+-rw-r--r--   0        0        0     1921 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/utils/version.py
+-rw-r--r--   0        0        0     1992 2023-08-05 15:12:52.559128 litestar-2.0.0rc1/litestar/utils/warnings.py
+-rw-r--r--   0        0        0    14075 2023-08-05 15:12:52.563129 litestar-2.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    21518 1970-01-01 00:00:00.000000 litestar-2.0.0rc1/PKG-INFO
```

### Comparing `litestar-2.0.0b4/LICENSE` & `litestar-2.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/docs/PYPI_README.md` & `litestar-2.0.0rc1/docs/PYPI_README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 | Meta      |     | [![Litestar Project](https://img.shields.io/badge/Litestar%20Org-%E2%AD%90%20Litestar-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/litestar-org/litestar) [![types - Mypy](https://img.shields.io/badge/types-Mypy-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/python/mypy) [![License - MIT](https://img.shields.io/badge/license-MIT-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://spdx.org/licenses/) [![Litestar Sponsors](https://img.shields.io/badge/Sponsor-%E2%9D%A4-%23edb641.svg?&logo=github&logoColor=edb641&labelColor=202235)](https://github.com/sponsors/litestar-org) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json&labelColor=202235)](https://github.com/astral-sh/ruff) [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=python&labelColor=202235&logoColor=edb641)](https://github.com/psf/black) [![All Contributors](https://img.shields.io/github/all-contributors/litestar-org/litestar?labelColor=202235&color=edb641&logoColor=edb641)](#contributors-)  |
 
 <!-- prettier-ignore-end -->
 </div>
 
 # Starlite → Litestar
 
-**[Starlite has been renamed to Litestar](https://litestar.dev/about/organization.html#litestar-and-starlite)**
+> [!IMPORTANT]\
+> [**_Starlite has been renamed to Litestar_**](https://litestar.dev/about/organization.html#litestar-and-starlite)
 
 <hr>
 
 Litestar is a powerful, performant, flexible and opinionated ASGI framework,
 offering first class typing support.
 
 Check out the [documentation 📚](https://docs.litestar.dev/).
@@ -36,15 +37,15 @@
 pip install litestar
 ```
 
 **Litestar 2.0 is coming out soon**, bringing many new features and improvements.
 You can check out the latest pre-release version by instead running
 
 ```shell
-pip install litestar==2.0.0beta3
+pip install litestar==2.0.0beta4
 ```
 
 ## Quick Start
 
 ```python
 from litestar import Litestar, get
```

### Comparing `litestar-2.0.0b4/litestar/__init__.py` & `litestar-2.0.0rc1/litestar/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 
 __version__ = get_version()
 
 
 __all__ = (
     "Controller",
     "HttpMethod",
+    "Litestar",
     "MediaType",
     "Request",
     "Response",
     "Router",
-    "Litestar",
     "WebSocket",
+    "__version__",
     "asgi",
     "delete",
     "get",
     "head",
     "patch",
     "post",
     "put",
     "route",
     "websocket",
     "websocket_listener",
-    "__version__",
 )
```

### Comparing `litestar-2.0.0b4/litestar/_asgi/asgi_router.py` & `litestar-2.0.0rc1/litestar/_asgi/asgi_router.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/_asgi/routing_trie/mapping.py` & `litestar-2.0.0rc1/litestar/_asgi/routing_trie/mapping.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/_asgi/routing_trie/traversal.py` & `litestar-2.0.0rc1/litestar/_asgi/routing_trie/traversal.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/_asgi/routing_trie/types.py` & `litestar-2.0.0rc1/litestar/_asgi/routing_trie/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/_asgi/routing_trie/validate.py` & `litestar-2.0.0rc1/litestar/_asgi/routing_trie/validate.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/_asgi/utils.py` & `litestar-2.0.0rc1/litestar/_asgi/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/_kwargs/cleanup.py` & `litestar-2.0.0rc1/litestar/_kwargs/cleanup.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/_kwargs/dependencies.py` & `litestar-2.0.0rc1/litestar/_kwargs/dependencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 from inspect import isasyncgen, isgenerator
 from typing import TYPE_CHECKING, Any
 
-from litestar._signature import get_signature_model
 from litestar.utils.compat import async_next
 
 __all__ = ("Dependency", "create_dependency_batches", "map_dependencies_recursively", "resolve_dependency")
 
 
 if TYPE_CHECKING:
     from litestar._kwargs.cleanup import DependencyCleanupGroup
@@ -54,15 +53,15 @@
     Args:
         dependency: An instance of :class:`Dependency <litestar._kwargs.Dependency>`
         connection: An instance of :class:`Request <litestar.connection.Request>` or
             :class:`WebSocket <litestar.connection.WebSocket>`.
         kwargs: Any kwargs to pass to the dependency, the result will be stored here as well.
         cleanup_group: DependencyCleanupGroup to which generators returned by ``dependency`` will be added
     """
-    signature_model = get_signature_model(dependency.provide)
+    signature_model = dependency.provide.signature_model
     dependency_kwargs = (
         signature_model.parse_values_from_connection_kwargs(connection=connection, **kwargs)
         if signature_model._fields
         else {}
     )
     value = await dependency.provide(**dependency_kwargs)
```

### Comparing `litestar-2.0.0b4/litestar/_kwargs/extractors.py` & `litestar-2.0.0rc1/litestar/_kwargs/extractors.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,25 +7,24 @@
 from litestar._multipart import parse_multipart_form
 from litestar._parsers import (
     parse_headers,
     parse_query_string,
     parse_url_encoded_form_data,
 )
 from litestar.datastructures.upload_file import UploadFile
-from litestar.dto.interface import ConnectionContext
 from litestar.enums import ParamType, RequestEncodingType
 from litestar.exceptions import ValidationException
 from litestar.params import BodyKwarg
 from litestar.types import Empty
 
 if TYPE_CHECKING:
     from litestar._kwargs import KwargsModel
     from litestar._kwargs.parameter_definition import ParameterDefinition
     from litestar.connection import ASGIConnection, Request
-    from litestar.dto.interface import DTOInterface
+    from litestar.dto import AbstractDTO
     from litestar.typing import FieldDefinition
 
 
 __all__ = (
     "body_extractor",
     "cookies_extractor",
     "create_connection_value_extractor",
@@ -285,22 +284,22 @@
     Returns:
         The MessagePack value.
     """
     return await connection.msgpack()
 
 
 def create_multipart_extractor(
-    field_definition: FieldDefinition, is_data_optional: bool, dto_type: type[DTOInterface] | None
+    field_definition: FieldDefinition, is_data_optional: bool, data_dto: type[AbstractDTO] | None
 ) -> Callable[[ASGIConnection[Any, Any, Any, Any]], Coroutine[Any, Any, Any]]:
     """Create a multipart form-data extractor.
 
     Args:
         field_definition: A FieldDefinition instance.
         is_data_optional: Boolean dictating whether the field is optional.
-        dto_type: The DTO type, if configured for handler.
+        data_dto: A data DTO type, if configured for handler.
 
     Returns:
         An extractor function.
     """
     body_kwarg_multipart_form_part_limit: int | None = None
     if field_definition.kwarg_definition and isinstance(field_definition.kwarg_definition, BodyKwarg):
         body_kwarg_multipart_form_part_limit = field_definition.kwarg_definition.multipart_form_part_limit
@@ -328,52 +327,45 @@
             return list(form_values.values())
         if field_definition.is_simple_type and field_definition.annotation is UploadFile and form_values:
             return next(v for v in form_values.values() if isinstance(v, UploadFile))
 
         if not form_values and is_data_optional:
             return None
 
-        if dto_type:
-            ctx = ConnectionContext.from_connection(connection)
-            return dto_type(ctx).builtins_to_data_type(form_values)
-
-        return form_values
+        return data_dto(connection).decode_builtins(form_values) if data_dto else form_values
 
     return cast("Callable[[ASGIConnection[Any, Any, Any, Any]], Coroutine[Any, Any, Any]]", extract_multipart)
 
 
 def create_url_encoded_data_extractor(
-    is_data_optional: bool, dto_type: type[DTOInterface] | None
+    is_data_optional: bool, data_dto: type[AbstractDTO] | None
 ) -> Callable[[ASGIConnection[Any, Any, Any, Any]], Coroutine[Any, Any, Any]]:
     """Create extractor for url encoded form-data.
 
     Args:
         is_data_optional: Boolean dictating whether the field is optional.
-        dto_type: The DTO type, if configured for handler.
+        data_dto: A data DTO type, if configured for handler.
 
     Returns:
         An extractor function.
     """
 
     async def extract_url_encoded_extractor(
         connection: Request[Any, Any, Any],
     ) -> Any:
         connection.scope["_form"] = form_values = (  # type: ignore[typeddict-unknown-key]
             connection.scope["_form"]  # type: ignore[typeddict-item]
             if "_form" in connection.scope
             else parse_url_encoded_form_data(await connection.body())
         )
+
         if not form_values and is_data_optional:
             return None
 
-        if dto_type:
-            ctx = ConnectionContext.from_connection(connection)
-            return dto_type(ctx).builtins_to_data_type(form_values)
-
-        return form_values
+        return data_dto(connection).decode_builtins(form_values) if data_dto else form_values
 
     return cast(
         "Callable[[ASGIConnection[Any, Any, Any, Any]], Coroutine[Any, Any, Any]]", extract_url_encoded_extractor
     )
 
 
 def create_data_extractor(kwargs_model: KwargsModel) -> Callable[[dict[str, Any], ASGIConnection], None]:
@@ -383,32 +375,33 @@
         kwargs_model: The KwargsModel instance.
 
     Returns:
         An extractor for the request's body.
     """
 
     if kwargs_model.expected_form_data:
-        media_type, field_definition, dto_type = kwargs_model.expected_form_data
+        media_type, field_definition = kwargs_model.expected_form_data
 
         if media_type == RequestEncodingType.MULTI_PART:
             data_extractor = create_multipart_extractor(
                 field_definition=field_definition,
                 is_data_optional=kwargs_model.is_data_optional,
-                dto_type=dto_type,
+                data_dto=kwargs_model.expected_data_dto,
             )
         else:
             data_extractor = create_url_encoded_data_extractor(
-                is_data_optional=kwargs_model.is_data_optional, dto_type=dto_type
+                is_data_optional=kwargs_model.is_data_optional,
+                data_dto=kwargs_model.expected_data_dto,
             )
     elif kwargs_model.expected_msgpack_data:
         data_extractor = cast(
             "Callable[[ASGIConnection[Any, Any, Any, Any]], Coroutine[Any, Any, Any]]", msgpack_extractor
         )
-    elif kwargs_model.expected_dto_data:
-        data_extractor = create_dto_extractor(kwargs_model.expected_dto_data)
+    elif kwargs_model.expected_data_dto:
+        data_extractor = create_dto_extractor(data_dto=kwargs_model.expected_data_dto)
     else:
         data_extractor = cast(
             "Callable[[ASGIConnection[Any, Any, Any, Any]], Coroutine[Any, Any, Any]]", json_extractor
         )
 
     def extractor(
         values: dict[str, Any],
@@ -416,23 +409,21 @@
     ) -> None:
         values["data"] = data_extractor(connection)
 
     return extractor
 
 
 def create_dto_extractor(
-    dto_type: type[DTOInterface],
+    data_dto: type[AbstractDTO],
 ) -> Callable[[ASGIConnection[Any, Any, Any, Any]], Coroutine[Any, Any, Any]]:
     """Create a DTO data extractor.
 
-    Args:
-        dto_type: The :class:`DTOInterface` subclass.
 
     Returns:
         An extractor function.
     """
 
     async def dto_extractor(connection: Request[Any, Any, Any]) -> Any:
-        ctx = ConnectionContext.from_connection(connection)
-        return dto_type(ctx).bytes_to_data_type(await connection.body())
+        body = await connection.body()
+        return data_dto(connection).decode_bytes(body)
 
     return dto_extractor  # type:ignore[return-value]
```

### Comparing `litestar-2.0.0b4/litestar/_kwargs/kwargs_model.py` & `litestar-2.0.0rc1/litestar/_kwargs/kwargs_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,103 +25,103 @@
     state_extractor,
 )
 from litestar._kwargs.parameter_definition import (
     ParameterDefinition,
     create_parameter_definition,
     merge_parameter_sets,
 )
-from litestar._signature import SignatureModel, get_signature_model
 from litestar.constants import RESERVED_KWARGS
 from litestar.enums import ParamType, RequestEncodingType
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.params import BodyKwarg, ParameterKwarg
 from litestar.typing import FieldDefinition
 
 __all__ = ("KwargsModel",)
 
 
 if TYPE_CHECKING:
+    from litestar._signature import SignatureModel
     from litestar.connection import ASGIConnection
     from litestar.di import Provide
-    from litestar.dto.interface import DTOInterface
+    from litestar.dto import AbstractDTO
     from litestar.utils.signature import ParsedSignature
 
 
 class KwargsModel:
     """Model required kwargs for a given RouteHandler and its dependencies.
 
     This is done once and is memoized during application bootstrap, ensuring minimal runtime overhead.
     """
 
     __slots__ = (
         "dependency_batches",
         "expected_cookie_params",
-        "expected_dto_data",
+        "expected_data_dto",
         "expected_form_data",
-        "expected_msgpack_data",
         "expected_header_params",
+        "expected_msgpack_data",
         "expected_path_params",
         "expected_query_params",
         "expected_reserved_kwargs",
         "extractors",
         "has_kwargs",
         "is_data_optional",
         "sequence_query_parameter_names",
     )
 
     def __init__(
         self,
         *,
         expected_cookie_params: set[ParameterDefinition],
-        expected_dto_data: type[DTOInterface] | None,
+        expected_data_dto: type[AbstractDTO] | None,
         expected_dependencies: set[Dependency],
-        expected_form_data: tuple[RequestEncodingType | str, FieldDefinition, type[DTOInterface] | None] | None,
-        expected_msgpack_data: FieldDefinition | None,
+        expected_form_data: tuple[RequestEncodingType | str, FieldDefinition] | None,
         expected_header_params: set[ParameterDefinition],
+        expected_msgpack_data: FieldDefinition | None,
         expected_path_params: set[ParameterDefinition],
         expected_query_params: set[ParameterDefinition],
         expected_reserved_kwargs: set[str],
-        sequence_query_parameter_names: set[str],
         is_data_optional: bool,
+        sequence_query_parameter_names: set[str],
     ) -> None:
         """Initialize ``KwargsModel``.
 
         Args:
             expected_cookie_params: Any expected cookie parameter kwargs
             expected_dependencies: Any expected dependency kwargs
-            expected_dto_data: Any expected DTO data kwargs
             expected_form_data: Any expected form data kwargs
-            expected_msgpack_data: Any expected MessagePack data kwargs
             expected_header_params: Any expected header parameter kwargs
+            expected_msgpack_data: Any expected MessagePack data kwargs
             expected_path_params: Any expected path parameter kwargs
             expected_query_params: Any expected query parameter kwargs
             expected_reserved_kwargs: Any expected reserved kwargs, e.g. 'state'
-            sequence_query_parameter_names: Any query parameters that are sequences
+            expected_data_dto: A data DTO, if defined
             is_data_optional: Treat data as optional
+            sequence_query_parameter_names: Any query parameters that are sequences
         """
         self.expected_cookie_params = expected_cookie_params
-        self.expected_dto_data = expected_dto_data
         self.expected_form_data = expected_form_data
-        self.expected_msgpack_data = expected_msgpack_data
         self.expected_header_params = expected_header_params
+        self.expected_msgpack_data = expected_msgpack_data
         self.expected_path_params = expected_path_params
         self.expected_query_params = expected_query_params
         self.expected_reserved_kwargs = expected_reserved_kwargs
+        self.expected_data_dto = expected_data_dto
         self.sequence_query_parameter_names = tuple(sequence_query_parameter_names)
 
         self.has_kwargs = (
             expected_cookie_params
             or expected_dependencies
             or expected_form_data
             or expected_msgpack_data
             or expected_header_params
             or expected_path_params
             or expected_query_params
             or expected_reserved_kwargs
-            or expected_dto_data
+            or expected_data_dto
         )
 
         self.is_data_optional = is_data_optional
         self.extractors = self._create_extractors()
         self.dependency_batches = create_dependency_batches(expected_dependencies)
 
     def _create_extractors(self) -> list[Callable[[dict[str, Any], ASGIConnection], None]]:
@@ -255,27 +255,24 @@
     def create_for_signature_model(
         cls,
         signature_model: type[SignatureModel],
         parsed_signature: ParsedSignature,
         dependencies: dict[str, Provide],
         path_parameters: set[str],
         layered_parameters: dict[str, FieldDefinition],
-        data_dto: type[DTOInterface] | None,
     ) -> KwargsModel:
         """Pre-determine what parameters are required for a given combination of route + route handler. It is executed
         during the application bootstrap process.
 
         Args:
             signature_model: A :class:`SignatureModel <litestar._signature.SignatureModel>` subclass.
             parsed_signature: A :class:`ParsedSignature <litestar._signature.ParsedSignature>` instance.
             dependencies: A string keyed dictionary mapping dependency providers.
             path_parameters: Any expected path parameters.
             layered_parameters: A string keyed dictionary of layered parameters.
-            data_dto: A :class:`DTOInterface <litestar._dto.DTOInterface>` subclass if one is declared
-                for the route handler, or ``None``.
 
         Returns:
             An instance of KwargsModel
         """
 
         field_definitions = signature_model._fields
 
@@ -296,40 +293,39 @@
         expected_reserved_kwargs = {field_name for field_name in field_definitions if field_name in RESERVED_KWARGS}
         expected_path_parameters = {p for p in param_definitions if p.param_type == ParamType.PATH}
         expected_header_parameters = {p for p in param_definitions if p.param_type == ParamType.HEADER}
         expected_cookie_parameters = {p for p in param_definitions if p.param_type == ParamType.COOKIE}
         expected_query_parameters = {p for p in param_definitions if p.param_type == ParamType.QUERY}
         sequence_query_parameter_names = {p.field_alias for p in expected_query_parameters if p.is_sequence}
 
-        expected_form_data: tuple[RequestEncodingType | str, FieldDefinition, type[DTOInterface] | None] | None = None
+        expected_form_data: tuple[RequestEncodingType | str, FieldDefinition] | None = None
         expected_msgpack_data: FieldDefinition | None = None
-        expected_dto_data: type[DTOInterface] | None = None
-
+        expected_data_dto: type[AbstractDTO] | None = None
         data_field_definition = field_definitions.get("data")
 
         media_type: RequestEncodingType | str | None = None
         if data_field_definition:
             if isinstance(data_field_definition.kwarg_definition, BodyKwarg):
                 media_type = data_field_definition.kwarg_definition.media_type
 
             if media_type in (RequestEncodingType.MULTI_PART, RequestEncodingType.URL_ENCODED):
-                expected_form_data = (media_type, data_field_definition, data_dto)
-            elif data_dto:
-                expected_dto_data = data_dto
+                expected_form_data = (media_type, data_field_definition)
+                expected_data_dto = signature_model._data_dto
+            elif signature_model._data_dto:
+                expected_data_dto = signature_model._data_dto
             elif media_type == RequestEncodingType.MESSAGEPACK:
                 expected_msgpack_data = data_field_definition
 
         for dependency in expected_dependencies:
             dependency_kwargs_model = cls.create_for_signature_model(
-                signature_model=get_signature_model(dependency.provide),
+                signature_model=dependency.provide.signature_model,
                 parsed_signature=parsed_signature,
                 dependencies=dependencies,
                 path_parameters=path_parameters,
                 layered_parameters=layered_parameters,
-                data_dto=None,
             )
             expected_path_parameters = merge_parameter_sets(
                 expected_path_parameters, dependency_kwargs_model.expected_path_params
             )
             expected_query_parameters = merge_parameter_sets(
                 expected_query_parameters, dependency_kwargs_model.expected_query_params
             )
@@ -348,15 +344,15 @@
 
             expected_reserved_kwargs.update(dependency_kwargs_model.expected_reserved_kwargs)
             sequence_query_parameter_names.update(dependency_kwargs_model.sequence_query_parameter_names)
 
         return KwargsModel(
             expected_cookie_params=expected_cookie_parameters,
             expected_dependencies=expected_dependencies,
-            expected_dto_data=expected_dto_data,
+            expected_data_dto=expected_data_dto,
             expected_form_data=expected_form_data,
             expected_header_params=expected_header_parameters,
             expected_msgpack_data=expected_msgpack_data,
             expected_path_params=expected_path_parameters,
             expected_query_params=expected_query_parameters,
             expected_reserved_kwargs=expected_reserved_kwargs,
             is_data_optional=field_definitions["data"].is_optional if "data" in expected_reserved_kwargs else False,
@@ -401,25 +397,25 @@
 
     @classmethod
     def _create_dependency_graph(cls, key: str, dependencies: dict[str, Provide]) -> Dependency:
         """Create a graph like structure of dependencies, with each dependency including its own dependencies as a
         list.
         """
         provide = dependencies[key]
-        sub_dependency_keys = [k for k in get_signature_model(provide)._fields if k in dependencies]
+        sub_dependency_keys = [k for k in provide.signature_model._fields if k in dependencies]
         return Dependency(
             key=key,
             provide=provide,
             dependencies=[cls._create_dependency_graph(key=k, dependencies=dependencies) for k in sub_dependency_keys],
         )
 
     @classmethod
     def _validate_dependency_data(
         cls,
-        expected_form_data: tuple[RequestEncodingType | str, FieldDefinition, type[DTOInterface] | None] | None,
+        expected_form_data: tuple[RequestEncodingType | str, FieldDefinition] | None,
         dependency_kwargs_model: KwargsModel,
     ) -> None:
         """Validate that the 'data' kwarg is compatible across dependencies."""
         if bool(expected_form_data) != bool(dependency_kwargs_model.expected_form_data):
             raise ImproperlyConfiguredException(
                 "Dependencies have incompatible 'data' kwarg types: one expects JSON and the other expects form-data"
             )
```

### Comparing `litestar-2.0.0b4/litestar/_kwargs/parameter_definition.py` & `litestar-2.0.0rc1/litestar/_kwargs/parameter_definition.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/_layers/utils.py` & `litestar-2.0.0rc1/litestar/_layers/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/_multipart.py` & `litestar-2.0.0rc1/litestar/_multipart.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,16 @@
         if field_name:
             post_data = form_part[line_index:-4].lstrip(b"\r\n")
             if file_name:
                 form_file = UploadFile(
                     content_type=content_type, filename=file_name, file_data=post_data, headers=dict(headers)
                 )
                 fields[field_name].append(form_file)
-            else:
+            elif post_data:
                 try:
                     fields[field_name].append(decode_json(post_data, type_decoders=type_decoders))
                 except SerializationException:
                     fields[field_name].append(post_data.decode(content_charset))
+            else:
+                fields[field_name].append(None)
 
     return {k: v if len(v) > 1 else v[0] for k, v in fields.items()}
```

### Comparing `litestar-2.0.0b4/litestar/_openapi/parameters.py` & `litestar-2.0.0rc1/litestar/_openapi/parameters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/_openapi/path_item.py` & `litestar-2.0.0rc1/litestar/_openapi/path_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from __future__ import annotations
 
 from inspect import cleandoc
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Iterable
 
 from litestar._openapi.parameters import create_parameter_for_handler
 from litestar._openapi.request_body import create_request_body
 from litestar._openapi.responses import create_responses
 from litestar._openapi.schema_generation import SchemaCreator
 from litestar._openapi.utils import SEPARATORS_CLEANUP_PATTERN
 from litestar.openapi.spec.path_item import PathItem
 from litestar.utils.helpers import unwrap_partial
 
 __all__ = ("create_path_item", "extract_layered_values", "get_description_for_handler")
 
-
 if TYPE_CHECKING:
     from litestar.handlers.http_handlers import HTTPRouteHandler
     from litestar.openapi.spec import Schema, SecurityRequirement
     from litestar.plugins import OpenAPISchemaPluginProtocol
     from litestar.routes import HTTPRoute
     from litestar.types.callable_types import OperationIDCreator
 
@@ -62,15 +61,15 @@
             security.extend(layer.security)
     return sorted(set(tags)) if tags else None, security or None
 
 
 def create_path_item(
     create_examples: bool,
     operation_id_creator: OperationIDCreator,
-    plugins: list[OpenAPISchemaPluginProtocol],
+    plugins: Iterable[OpenAPISchemaPluginProtocol],
     route: HTTPRoute,
     schemas: dict[str, Schema],
     use_handler_docstrings: bool,
 ) -> tuple[PathItem, list[str]]:
     """Create a PathItem for the given route parsing all http_methods into Operation Models.
 
     Args:
@@ -104,19 +103,26 @@
                 or None
             )
             raises_validation_error = bool("data" in handler_fields or path_item.parameters or parameters)
 
             request_body = None
             if "data" in handler_fields:
                 request_body = create_request_body(
-                    route_handler=route_handler, field=handler_fields["data"], schema_creator=request_schema_creator
+                    route_handler=route_handler,
+                    field_definition=handler_fields["data"],
+                    schema_creator=request_schema_creator,
                 )
-            operation_id = route_handler.operation_id or operation_id_creator(
-                route_handler, http_method, route.path_components
-            )
+
+            if isinstance(route_handler.operation_id, str):
+                operation_id = route_handler.operation_id
+            elif callable(route_handler.operation_id):
+                operation_id = route_handler.operation_id(route_handler, http_method, route.path_components)
+            else:
+                operation_id = operation_id_creator(route_handler, http_method, route.path_components)
+
             tags, security = extract_layered_values(route_handler)
             operation = route_handler.operation_class(
                 operation_id=operation_id,
                 tags=tags,
                 summary=route_handler.summary or SEPARATORS_CLEANUP_PATTERN.sub("", route_handler.handler_name.title()),
                 description=get_description_for_handler(route_handler, use_handler_docstrings),
                 deprecated=route_handler.deprecated,
```

### Comparing `litestar-2.0.0b4/litestar/_openapi/request_body.py` & `litestar-2.0.0rc1/litestar/_openapi/request_body.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,20 +13,22 @@
 if TYPE_CHECKING:
     from litestar._openapi.schema_generation import SchemaCreator
     from litestar.handlers import BaseRouteHandler
     from litestar.typing import FieldDefinition
 
 
 def create_request_body(
-    route_handler: BaseRouteHandler, field: FieldDefinition, schema_creator: SchemaCreator
+    route_handler: BaseRouteHandler, field_definition: FieldDefinition, schema_creator: SchemaCreator
 ) -> RequestBody | None:
     """Create a RequestBody model for the given RouteHandler or return None."""
     media_type: RequestEncodingType | str = RequestEncodingType.JSON
-    if isinstance(field.kwarg_definition, BodyKwarg) and field.kwarg_definition.media_type:
-        media_type = field.kwarg_definition.media_type
+    if isinstance(field_definition.kwarg_definition, BodyKwarg) and field_definition.kwarg_definition.media_type:
+        media_type = field_definition.kwarg_definition.media_type
 
-    if dto := route_handler.resolve_dto():
-        schema = dto.create_openapi_schema("data", str(route_handler), schema_creator)
+    if dto := route_handler.resolve_data_dto():
+        schema = dto.create_openapi_schema(
+            field_definition=field_definition, handler_id=route_handler.handler_id, schema_creator=schema_creator
+        )
     else:
-        schema = schema_creator.for_field_definition(field)
+        schema = schema_creator.for_field_definition(field_definition)
 
     return RequestBody(required=True, content={media_type: OpenAPIMediaType(schema=schema)})
```

### Comparing `litestar-2.0.0b4/litestar/_openapi/responses.py` & `litestar-2.0.0rc1/litestar/_openapi/responses.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,64 +67,68 @@
     return Schema(description=cookie.description or "", example=value)
 
 
 def create_success_response(  # noqa: C901
     route_handler: HTTPRouteHandler, schema_creator: SchemaCreator
 ) -> OpenAPIResponse:
     """Create the schema for a success response."""
-    return_type = route_handler.parsed_fn_signature.return_type
-    return_annotation = return_type.annotation
+    field_definition = route_handler.parsed_fn_signature.return_type
+    return_annotation = field_definition.annotation
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
 
-    if return_annotation is not Signature.empty and not return_type.is_subclass_of(
+    if return_annotation is not Signature.empty and not field_definition.is_subclass_of(
         (NoneType, File, Redirect, Stream, ASGIResponse)
     ):
         media_type = route_handler.media_type
+
         if return_annotation is Template:
             return_annotation = str
             media_type = media_type or MediaType.HTML
-        elif return_type.is_subclass_of(LitestarResponse):
-            return_annotation = return_type.inner_types[0].annotation if return_type.inner_types else Any
+
+        elif field_definition.is_subclass_of(LitestarResponse):
+            return_annotation = field_definition.inner_types[0].annotation if field_definition.inner_types else Any
             media_type = media_type or MediaType.JSON
 
         if dto := route_handler.resolve_return_dto():
-            result = dto.create_openapi_schema("return", str(route_handler), schema_creator)
+            result = dto.create_openapi_schema(
+                field_definition=field_definition, handler_id=route_handler.handler_id, schema_creator=schema_creator
+            )
         else:
             result = schema_creator.for_field_definition(FieldDefinition.from_annotation(return_annotation))
 
         schema = result if isinstance(result, Schema) else schema_creator.schemas[result.value]
 
         schema.content_encoding = route_handler.content_encoding
         schema.content_media_type = route_handler.content_media_type
 
         response = OpenAPIResponse(
             content={get_enum_string_value(media_type): OpenAPIMediaType(schema=result)}, description=description
         )
 
-    elif return_type.is_subclass_of(Redirect):
+    elif field_definition.is_subclass_of(Redirect):
         response = OpenAPIResponse(
             content=None,
             description=description,
             headers={
                 "location": OpenAPIHeader(
                     schema=Schema(type=OpenAPIType.STRING), description="target path for the redirect"
                 )
             },
         )
 
-    elif return_type.is_subclass_of((File, Stream)):
+    elif field_definition.is_subclass_of((File, Stream)):
         response = OpenAPIResponse(
             content={
                 route_handler.media_type: OpenAPIMediaType(
                     schema=Schema(
                         type=OpenAPIType.STRING,
                         content_encoding=route_handler.content_encoding or "application/octet-stream",
                         content_media_type=route_handler.content_media_type,
```

### Comparing `litestar-2.0.0b4/litestar/_openapi/schema_generation/constrained_fields.py` & `litestar-2.0.0rc1/litestar/_openapi/schema_generation/constrained_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from re import Pattern
 from typing import TYPE_CHECKING
 
 from litestar.openapi.spec.enums import OpenAPIFormat, OpenAPIType
 from litestar.openapi.spec.schema import Schema
 
 if TYPE_CHECKING:
-    from _decimal import Decimal
+    from decimal import Decimal
 
     from litestar.params import KwargDefinition
 
 __all__ = (
     "create_date_constrained_field_schema",
     "create_numerical_constrained_field_schema",
     "create_string_constrained_field_schema",
```

### Comparing `litestar-2.0.0b4/litestar/_openapi/schema_generation/examples.py` & `litestar-2.0.0rc1/litestar/_openapi/schema_generation/examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from dataclasses import replace
+from decimal import Decimal
 from enum import Enum
 from typing import TYPE_CHECKING, Any
 
-from _decimal import Decimal
 from polyfactory.exceptions import ParameterException
 from polyfactory.field_meta import FieldMeta, Null
 from polyfactory.utils.helpers import unwrap_annotation
 
 from litestar.openapi.spec import Example
 from litestar.types import Empty
 from litestar.utils import is_pydantic_model_instance
```

### Comparing `litestar-2.0.0b4/litestar/_openapi/schema_generation/schema.py` & `litestar-2.0.0rc1/litestar/_openapi/schema_generation/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from collections import deque
 from copy import copy
 from dataclasses import MISSING, fields
 from datetime import date, datetime, time, timedelta
-from enum import EnumMeta
+from decimal import Decimal
+from enum import Enum, EnumMeta
 from ipaddress import IPv4Address, IPv4Interface, IPv4Network, IPv6Address, IPv6Interface, IPv6Network
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     DefaultDict,
     Deque,
@@ -28,15 +29,14 @@
     Tuple,
     Union,
     cast,
     get_origin,
 )
 from uuid import UUID
 
-from _decimal import Decimal
 from msgspec.structs import FieldInfo
 from msgspec.structs import fields as msgspec_struct_fields
 from typing_extensions import NotRequired, Required, get_args, get_type_hints
 
 from litestar._openapi.schema_generation.constrained_fields import (
     create_date_constrained_field_schema,
     create_numerical_constrained_field_schema,
@@ -64,15 +64,14 @@
     is_undefined_sentinel,
 )
 from litestar.utils.typing import get_origin_or_inner_type, make_non_optional_union
 
 if TYPE_CHECKING:
     from msgspec import Struct
 
-    from litestar.dto.types import ForType
     from litestar.plugins import OpenAPISchemaPluginProtocol
 
 
 KWARG_DEFINITION_ATTRIBUTE_TO_OPENAPI_PROPERTY_MAP: dict[str, str] = {
     "content_encoding": "contentEncoding",
     "default": "default",
     "description": "description",
@@ -137,28 +136,24 @@
     UploadFile: Schema(
         type=OpenAPIType.STRING,
         content_media_type="application/octet-stream",
     ),
 }
 
 
-def _get_type_schema_name(value: Any, dto_for: ForType | None) -> str:
+def _get_type_schema_name(value: Any) -> str:
     """Extract the schema name from a data container.
 
     Args:
         value: A data container
-        dto_for: The type of DTO to create the schema for.
 
     Returns:
         A string
     """
-    name = cast("str", getattr(value, "__schema_name__", value.__name__))
-    if dto_for == "data":
-        return f"{name}RequestBody"
-    return f"{name}ResponseBody" if dto_for == "return" else name
+    return cast("str", getattr(value, "__schema_name__", value.__name__))
 
 
 def create_enum_schema(annotation: EnumMeta) -> Schema:
     """Create a schema instance for an enum.
 
     Args:
         annotation: An enum.
@@ -180,15 +175,15 @@
     Yields:
         The flattened arguments of the Literal.
     """
     for arg in get_args(annotation):
         if get_origin_or_inner_type(arg) is Literal:
             yield from _iter_flat_literal_args(arg)
         else:
-            yield arg
+            yield arg.value if isinstance(arg, Enum) else arg
 
 
 def create_literal_schema(annotation: Any) -> Schema:
     """Create a schema instance for a Literal.
 
     Args:
         annotation: An Literal annotation.
@@ -226,15 +221,15 @@
 
 class SchemaCreator:
     __slots__ = ("generate_examples", "plugins", "schemas", "prefer_alias", "dto_for")
 
     def __init__(
         self,
         generate_examples: bool = False,
-        plugins: list[OpenAPISchemaPluginProtocol] | None = None,
+        plugins: Iterable[OpenAPISchemaPluginProtocol] | None = None,
         schemas: dict[str, Schema] | None = None,
         prefer_alias: bool = True,
     ) -> None:
         """Instantiate a SchemaCreator.
 
         Args:
             generate_examples: Whether to generate examples if none are given.
@@ -252,41 +247,38 @@
         """Return a SchemaCreator with generate_examples set to False."""
         if not self.generate_examples:
             return self
         new = copy(self)
         new.generate_examples = False
         return new
 
-    def for_field_definition(
-        self, field_definition: FieldDefinition, dto_for: ForType | None = None
-    ) -> Schema | Reference:
+    def for_field_definition(self, field_definition: FieldDefinition) -> Schema | Reference:
         """Create a Schema for a given FieldDefinition.
 
         Args:
             field_definition: A signature field instance.
-            dto_for: The type of DTO to create the schema for.
 
         Returns:
             A schema instance.
         """
         result: Schema | Reference
         if field_definition.is_optional:
             result = self.for_optional_field(field_definition)
         elif field_definition.is_union:
             result = self.for_union_field(field_definition)
         elif is_struct_class(field_definition.annotation):
-            result = self.for_struct_class(field_definition.annotation, dto_for)
+            result = self.for_struct_class(field_definition.annotation)
         elif is_dataclass_class(field_definition.annotation):
-            result = self.for_dataclass(field_definition.annotation, dto_for)
+            result = self.for_dataclass(field_definition.annotation)
         elif is_typed_dict(field_definition.annotation):
-            result = self.for_typed_dict(field_definition.annotation, dto_for)
+            result = self.for_typed_dict(field_definition.annotation)
         elif plugins_for_annotation := [
             plugin for plugin in self.plugins if plugin.is_plugin_supported_type(field_definition.annotation)
         ]:
-            result = self.for_plugin(field_definition, plugins_for_annotation[0], dto_for)
+            result = self.for_plugin(field_definition, plugins_for_annotation[0])
         elif is_pydantic_constrained_field(field_definition.annotation) or (
             isinstance(field_definition.kwarg_definition, (ParameterKwarg, BodyKwarg))
             and field_definition.kwarg_definition.is_constrained
         ):
             result = self.for_constrained_field(field_definition)
         elif field_definition.inner_types and not field_definition.is_generic:
             result = self.for_object_type(field_definition)
@@ -421,46 +413,42 @@
                     items=self.for_field_definition(field_definition=field_definition.inner_types[1]),
                 ),
                 "cursor": cursor_schema,
                 "results_per_page": Schema(type=OpenAPIType.INTEGER, description="Maximal number of items to send."),
             },
         )
 
-    def for_plugin(
-        self, field_definition: FieldDefinition, plugin: OpenAPISchemaPluginProtocol, dto_for: ForType | None = None
-    ) -> Schema | Reference:
+    def for_plugin(self, field_definition: FieldDefinition, plugin: OpenAPISchemaPluginProtocol) -> Schema | Reference:
         """Create a schema using a plugin.
 
         Args:
             field_definition: A signature field instance.
             plugin: A plugin for the field type.
-            dto_for: The type of DTO to generate a schema for if any.
 
         Returns:
             A schema instance.
         """
-        schema = plugin.to_openapi_schema(annotation=field_definition.annotation, schema_creator=self, dto_for=dto_for)
+        schema = plugin.to_openapi_schema(field_definition=field_definition, schema_creator=self)
         if isinstance(schema, SchemaDataContainer):
             return self.for_field_definition(
                 FieldDefinition.from_kwarg(
                     annotation=schema.data_container,
                     name=field_definition.name,
                     default=field_definition.default,
                     extra=field_definition.extra,
                     kwarg_definition=field_definition.kwarg_definition,
                 )
             )
         return schema  # pragma: no cover
 
-    def for_struct_class(self, annotation: type[Struct], dto_for: ForType | None) -> Schema:
+    def for_struct_class(self, annotation: type[Struct]) -> Schema:
         """Create a schema object for a given msgspec.Struct class.
 
         Args:
             annotation: A msgspec.Struct class.
-            dto_for: The type of DTO to generate a schema for.
 
         Returns:
             A schema instance.
         """
 
         def _is_field_required(field: FieldInfo) -> bool:
             return field.required or field.default_factory is Empty
@@ -474,23 +462,23 @@
                 ]
             ),
             properties={
                 field.encode_name: self.for_field_definition(FieldDefinition.from_kwarg(field.type, field.encode_name))
                 for field in msgspec_struct_fields(annotation)
             },
             type=OpenAPIType.OBJECT,
-            title=_get_type_schema_name(annotation, dto_for),
+            title=_get_type_schema_name(annotation),
         )
 
-    def for_dataclass(self, annotation: type[DataclassProtocol], dto_for: ForType | None) -> Schema:
+    # noinspection PyDataclass
+    def for_dataclass(self, annotation: type[DataclassProtocol]) -> Schema:
         """Create a schema object for a given dataclass class.
 
         Args:
             annotation: A dataclass class.
-            dto_for: The type of DTO to generate a schema for.
 
         Returns:
             A schema instance.
         """
         annotation_hints = get_type_hints(annotation, include_extras=True)
         return Schema(
             required=sorted(
@@ -504,36 +492,38 @@
                     )
                 ]
             ),
             properties={
                 k: self.for_field_definition(FieldDefinition.from_kwarg(v, k)) for k, v in annotation_hints.items()
             },
             type=OpenAPIType.OBJECT,
-            title=_get_type_schema_name(annotation, dto_for),
+            title=_get_type_schema_name(annotation),
         )
 
-    def for_typed_dict(self, annotation: TypedDictClass, dto_for: ForType | None) -> Schema:
+    # noinspection PyTypedDict
+    def for_typed_dict(self, annotation: TypedDictClass) -> Schema:
         """Create a schema object for a given typed dict.
 
         Args:
             annotation: A typed-dict class.
-            dto_for: The type of DTO to generate a schema for.
 
         Returns:
             A schema instance.
         """
-        annotations: dict[str, Any] = {
-            k: get_args(v)[0] if get_origin(v) in (Required, NotRequired) else v
-            for k, v in get_type_hints(annotation, include_extras=True).items()
-        }
         return Schema(
             required=sorted(getattr(annotation, "__required_keys__", [])),
-            properties={k: self.for_field_definition(FieldDefinition.from_kwarg(v, k)) for k, v in annotations.items()},
+            properties={
+                k: self.for_field_definition(FieldDefinition.from_kwarg(v, k))
+                for k, v in {
+                    k: get_args(v)[0] if get_origin(v) in (Required, NotRequired) else v
+                    for k, v in get_type_hints(annotation, include_extras=True).items()
+                }.items()
+            },
             type=OpenAPIType.OBJECT,
-            title=_get_type_schema_name(annotation, dto_for),
+            title=_get_type_schema_name(annotation),
         )
 
     def for_constrained_field(self, field: FieldDefinition) -> Schema:
         """Create Schema for Pydantic Constrained fields (created using constr(), conint() and so forth, or by subclassing
         Constrained*)
 
         Args:
```

### Comparing `litestar-2.0.0b4/litestar/_openapi/schema_generation/utils.py` & `litestar-2.0.0rc1/litestar/_openapi/schema_generation/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/_openapi/typescript_converter/converter.py` & `litestar-2.0.0rc1/litestar/_openapi/typescript_converter/converter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/_openapi/typescript_converter/schema_parsing.py` & `litestar-2.0.0rc1/litestar/_openapi/typescript_converter/schema_parsing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/_openapi/typescript_converter/types.py` & `litestar-2.0.0rc1/litestar/_openapi/typescript_converter/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/_openapi/utils.py` & `litestar-2.0.0rc1/litestar/_openapi/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from litestar.types.internal_types import PathParameterDefinition
 
 if TYPE_CHECKING:
     from litestar.handlers.http_handlers import HTTPRouteHandler
     from litestar.types import Method
 
 
-__all__ = ("default_operation_id_creator",)
+__all__ = ("default_operation_id_creator", "SEPARATORS_CLEANUP_PATTERN")
 
 SEPARATORS_CLEANUP_PATTERN = re.compile(r"[!#$%&'*+\-.^_`|~:]+")
 
 
 def default_operation_id_creator(
     route_handler: HTTPRouteHandler,
     http_method: Method,
```

### Comparing `litestar-2.0.0b4/litestar/_parsers.py` & `litestar-2.0.0rc1/litestar/_parsers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/_signature/model.py` & `litestar-2.0.0rc1/litestar/_signature/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,56 @@
-# ruff: noqa: UP006
+# ruff: noqa: UP006, UP007
 from __future__ import annotations
 
 import re
+from functools import partial
+from pathlib import Path, PurePath
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     ClassVar,
     Dict,
     Literal,
     Optional,
     Sequence,
     Set,
+    Type,
     TypedDict,
     Union,
     cast,
 )
+from uuid import UUID
 
 from msgspec import NODEFAULT, Meta, Struct, ValidationError, convert, defstruct
 from msgspec.structs import asdict
 from typing_extensions import Annotated
 
-from litestar._signature.utils import create_type_overrides, validate_signature_dependencies
+from litestar._signature.types import ExtendedMsgSpecValidationError
+from litestar._signature.utils import (
+    _get_decoder_for_type,
+    _normalize_annotation,
+    _validate_signature_dependencies,
+)
+from litestar.datastructures import ImmutableState
+from litestar.dto import AbstractDTO, DTOData
 from litestar.enums import ParamType, ScopeType
 from litestar.exceptions import InternalServerException, ValidationException
-from litestar.params import DependencyKwarg, KwargDefinition, ParameterKwarg
-from litestar.serialization._msgspec_utils import ExtendedMsgSpecValidationError
+from litestar.params import KwargDefinition, ParameterKwarg
 from litestar.typing import FieldDefinition  # noqa
-from litestar.utils import make_non_optional_union
+from litestar.utils import is_class_and_subclass
 from litestar.utils.dataclass import simple_asdict
-from litestar.utils.typing import unwrap_union
 
 if TYPE_CHECKING:
     from typing_extensions import NotRequired
 
     from litestar.connection import ASGIConnection
-    from litestar.types import AnyCallable
+    from litestar.types import AnyCallable, TypeDecodersSequence
     from litestar.utils.signature import ParsedSignature
 
-
 __all__ = (
     "ErrorMessage",
     "SignatureModel",
 )
 
 
 class ErrorMessage(TypedDict):
@@ -63,20 +71,38 @@
     "pattern",
     "min_length",
     "max_length",
 )
 
 ERR_RE = re.compile(r"`\$\.(.+)`$")
 
+DEFAULT_TYPE_DECODERS = [
+    (lambda x: is_class_and_subclass(x, (Path, PurePath, ImmutableState, UUID)), lambda t, v: t(v)),
+]
+
+
+def _deserializer(target_type: Any, value: Any, default_deserializer: Callable[[Any, Any], Any]) -> Any:
+    if isinstance(value, DTOData):
+        return value
+
+    if isinstance(value, target_type):
+        return value
+
+    if decoder := getattr(target_type, "_decoder", None):
+        return decoder(target_type, value)
+
+    return default_deserializer(target_type, value)
+
 
 class SignatureModel(Struct):
     """Model that represents a function signature that uses a msgspec specific type or types."""
 
-    # NOTE: we have to use Set and Dict here because python 3.8 goes haywire if we use 'set' and 'dict'
+    _data_dto: ClassVar[Optional[Type[AbstractDTO]]]
     _dependency_name_set: ClassVar[Set[str]]
+    # NOTE: we have to use Set and Dict here because python 3.8 goes haywire if we use 'set' and 'dict'
     _fields: ClassVar[Dict[str, FieldDefinition]]
     _return_annotation: ClassVar[Any]
 
     @classmethod
     def _create_exception(cls, connection: ASGIConnection, messages: list[ErrorMessage]) -> Exception:
         """Create an exception class - either a ValidationException or an InternalServerException, depending on whether
             the failure is in client provided values or injected dependencies.
@@ -127,23 +153,21 @@
                     message["source"] = ParamType.HEADER
                 else:
                     message["source"] = ParamType.QUERY
 
         return message
 
     @classmethod
-    def _collect_errors(
-        cls, default_deserializer: Callable[[Any, Any], Any], **kwargs: Any
-    ) -> list[tuple[str, Exception]]:
+    def _collect_errors(cls, deserializer: Callable[[Any, Any], Any], **kwargs: Any) -> list[tuple[str, Exception]]:
         exceptions: list[tuple[str, Exception]] = []
         for field_name in cls._fields:
             try:
                 raw_value = kwargs[field_name]
                 annotation = cls.__annotations__[field_name]
-                convert(raw_value, type=annotation, strict=False, dec_hook=default_deserializer, str_keys=True)
+                convert(raw_value, type=annotation, strict=False, dec_hook=deserializer, str_keys=True)
             except Exception as e:  # noqa: BLE001
                 exceptions.append((field_name, e))
 
         return exceptions
 
     @classmethod
     def parse_values_from_connection_kwargs(cls, connection: ASGIConnection, **kwargs: Any) -> dict[str, Any]:
@@ -157,24 +181,25 @@
             ValidationException: If validation failed.
             InternalServerException: If another exception has been raised.
 
         Returns:
             A dictionary of parsed values
         """
         messages: list[ErrorMessage] = []
+        deserializer = partial(_deserializer, default_deserializer=connection.route_handler.default_deserializer)
         try:
-            return convert(kwargs, cls, strict=False, dec_hook=connection.route_handler.default_deserializer).to_dict()
+            return convert(kwargs, cls, strict=False, dec_hook=deserializer, str_keys=True).to_dict()
         except ExtendedMsgSpecValidationError as e:
             for exc in e.errors:
                 keys = [str(loc) for loc in exc["loc"]]
                 message = cls._build_error_message(keys=keys, exc_msg=exc["msg"], connection=connection)
                 messages.append(message)
             raise cls._create_exception(messages=messages, connection=connection) from e
         except ValidationError as e:
-            for field_name, exc in cls._collect_errors(default_deserializer=connection.route_handler.default_deserializer, **kwargs):  # type: ignore[assignment]
+            for field_name, exc in cls._collect_errors(deserializer=deserializer, **kwargs):  # type: ignore[assignment]
                 match = ERR_RE.search(str(exc))
                 keys = [field_name, str(match.group(1))] if match else [field_name]
                 message = cls._build_error_message(keys=keys, exc_msg=str(e), connection=connection)
                 messages.append(message)
             raise cls._create_exception(messages=messages, connection=connection) from e
 
     def to_dict(self) -> dict[str, Any]:
@@ -187,29 +212,29 @@
 
     @classmethod
     def create(
         cls,
         dependency_name_set: set[str],
         fn: AnyCallable,
         parsed_signature: ParsedSignature,
-        has_data_dto: bool = False,
+        type_decoders: TypeDecodersSequence,
+        data_dto: type[AbstractDTO] | None = None,
     ) -> type[SignatureModel]:
         fn_name = (
             fn_name if (fn_name := getattr(fn, "__name__", "anonymous")) and fn_name != "<lambda>" else "anonymous"
         )
 
-        dependency_names = validate_signature_dependencies(
+        dependency_names = _validate_signature_dependencies(
             dependency_name_set=dependency_name_set, fn_name=fn_name, parsed_signature=parsed_signature
         )
-        type_overrides = create_type_overrides(parsed_signature, has_data_dto)
 
         struct_fields: list[tuple[str, Any, Any]] = []
 
         for field_definition in parsed_signature.parameters.values():
-            annotation = type_overrides.get(field_definition.name, field_definition.annotation)
+            meta_data: Meta | None = None
 
             if isinstance(field_definition.kwarg_definition, KwargDefinition):
                 meta_kwargs: dict[str, Any] = {"extra": {}}
 
                 kwarg_definition = simple_asdict(field_definition.kwarg_definition, exclude_empty=True)
                 if min_items := kwarg_definition.pop("min_items", None):
                     meta_kwargs["min_length"] = min_items
@@ -218,40 +243,63 @@
 
                 for k, v in kwarg_definition.items():
                     if hasattr(Meta, k) and v is not None:
                         meta_kwargs[k] = v
                     else:
                         meta_kwargs["extra"][k] = v
 
-                meta = Meta(**meta_kwargs)
-                if field_definition.is_optional:
-                    annotation = Optional[Annotated[make_non_optional_union(annotation), meta]]
-                elif field_definition.is_union and meta_kwargs.keys() & MSGSPEC_CONSTRAINT_FIELDS:
-                    # unwrap inner types of a union and apply constraints to each individual type
-                    # see https://github.com/jcrist/msgspec/issues/447
-                    annotation = Union[
-                        tuple(Annotated[inner_type, meta] for inner_type in unwrap_union(annotation))  # pyright: ignore
-                    ]
-                else:
-                    annotation = Annotated[annotation, meta]
+                meta_data = Meta(**meta_kwargs)
 
-            elif (
-                isinstance(field_definition.kwarg_definition, DependencyKwarg)
-                and field_definition.kwarg_definition.skip_validation
-            ):
-                annotation = Any
+            annotation = cls._create_annotation(
+                field_definition=field_definition,
+                type_decoders=[*(type_decoders or []), *DEFAULT_TYPE_DECODERS],
+                meta_data=meta_data,
+            )
 
             default = field_definition.default if field_definition.has_default else NODEFAULT
             struct_fields.append((field_definition.name, annotation, default))
 
         return defstruct(  # type:ignore[return-value]
             f"{fn_name}_signature_model",
             struct_fields,
             bases=(cls,),
             module=getattr(fn, "__module__", None),
             namespace={
                 "_return_annotation": parsed_signature.return_type.annotation,
                 "_dependency_name_set": dependency_names,
                 "_fields": parsed_signature.parameters,
+                "_data_dto": data_dto,
             },
             kw_only=True,
         )
+
+    @classmethod
+    def _create_annotation(
+        cls,
+        field_definition: FieldDefinition,
+        type_decoders: TypeDecodersSequence,
+        meta_data: Meta | None = None,
+    ) -> Any:
+        annotation = _normalize_annotation(field_definition=field_definition)
+
+        if annotation is Any:
+            return annotation
+
+        if field_definition.is_union:
+            types = [
+                cls._create_annotation(
+                    field_definition=inner_type,
+                    type_decoders=type_decoders,
+                    meta_data=meta_data,
+                )
+                for inner_type in (t for t in field_definition.inner_types if t.annotation is not type(None))
+            ]
+            return Optional[types[0]] if field_definition.is_optional else Union[tuple(types)]  # pyright: ignore
+
+        if decoder := _get_decoder_for_type(annotation, type_decoders=type_decoders):
+            # FIXME: temporary (hopefully) hack, see: https://github.com/jcrist/msgspec/issues/497
+            setattr(annotation, "_decoder", decoder)
+
+        if meta_data:
+            annotation = Annotated[annotation, meta_data]  # pyright: ignore
+
+        return annotation
```

### Comparing `litestar-2.0.0b4/litestar/_signature/utils.py` & `litestar-2.0.0rc1/litestar/_signature/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,25 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, cast
+from typing import TYPE_CHECKING, Any, Callable
 
 from litestar.constants import SKIP_VALIDATION_NAMES
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.params import DependencyKwarg
-from litestar.types import Empty
+from litestar.types import Empty, TypeDecodersSequence
 
 if TYPE_CHECKING:
+    from litestar.typing import FieldDefinition
     from litestar.utils.signature import ParsedSignature
 
-    from .model import SignatureModel
 
-__all__ = ("create_type_overrides", "validate_signature_dependencies", "get_signature_model")
+__all__ = ("_validate_signature_dependencies", "_normalize_annotation", "_get_decoder_for_type")
 
 
-def get_signature_model(value: Any) -> type[SignatureModel]:
-    """Retrieve and validate the signature model from a provider or handler."""
-    try:
-        return cast("type[SignatureModel]", value.signature_model)
-    except AttributeError as e:  # pragma: no cover
-        raise ImproperlyConfiguredException(f"The 'signature_model' attribute for {value} is not set") from e
-
-
-def create_type_overrides(parsed_signature: ParsedSignature, has_data_dto: bool) -> dict[str, Any]:
-    """Create typing overrides for field definitions.
-
-    Args:
-        parsed_signature: A parsed function signature.
-        has_data_dto: Whether the signature contains a data DTO.
-
-    Returns:
-        A dictionary of typing overrides
-    """
-    type_overrides = {}
-    for field_definition in parsed_signature.parameters.values():
-        if field_definition.name in SKIP_VALIDATION_NAMES or (
-            isinstance(field_definition.kwarg_definition, DependencyKwarg)
-            and field_definition.kwarg_definition.skip_validation
-        ):
-            type_overrides[field_definition.name] = Any
-
-        if has_data_dto and "data" in parsed_signature.parameters:
-            type_overrides["data"] = Any
-
-    return type_overrides
-
-
-def validate_signature_dependencies(
+def _validate_signature_dependencies(
     dependency_name_set: set[str], fn_name: str, parsed_signature: ParsedSignature
 ) -> set[str]:
     """Validate dependencies of ``parsed_signature``.
 
     Args:
         dependency_name_set: A set of dependency names
         fn_name: A callable's name.
@@ -67,7 +35,24 @@
             if not parameter.is_optional and parameter.default is Empty:
                 raise ImproperlyConfiguredException(
                     f"Explicit dependency '{parameter.name}' for '{fn_name}' has no default value, "
                     f"or provided dependency."
                 )
             dependency_names.add(parameter.name)
     return dependency_names
+
+
+def _normalize_annotation(field_definition: FieldDefinition) -> Any:
+    if field_definition.name in SKIP_VALIDATION_NAMES or (
+        isinstance(field_definition.kwarg_definition, DependencyKwarg)
+        and field_definition.kwarg_definition.skip_validation
+    ):
+        return Any
+
+    return field_definition.annotation
+
+
+def _get_decoder_for_type(target_type: Any, type_decoders: TypeDecodersSequence) -> Callable[[type, Any], Any] | None:
+    return next(
+        (decoder for predicate, decoder in type_decoders if predicate(target_type)),
+        None,
+    )
```

### Comparing `litestar-2.0.0b4/litestar/app.py` & `litestar-2.0.0rc1/litestar/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,42 +26,44 @@
     NoRouteMatchFoundException,
 )
 from litestar.logging.config import LoggingConfig, get_logger_placeholder
 from litestar.middleware.cors import CORSMiddleware
 from litestar.openapi.config import OpenAPIConfig
 from litestar.openapi.spec.components import Components
 from litestar.plugins import (
+    CLIPluginProtocol,
     InitPluginProtocol,
     OpenAPISchemaPluginProtocol,
+    PluginProtocol,
+    PluginRegistry,
     SerializationPluginProtocol,
 )
 from litestar.router import Router
 from litestar.routes import ASGIRoute, HTTPRoute, WebSocketRoute
 from litestar.static_files.base import StaticFiles
 from litestar.stores.registry import StoreRegistry
 from litestar.types import Empty, TypeDecodersSequence
 from litestar.types.internal_types import PathParameterDefinition
-from litestar.utils import AsyncCallable, join_paths, unique
+from litestar.utils import AsyncCallable, deprecated, join_paths, unique
 from litestar.utils.dataclass import extract_dataclass_items
 from litestar.utils.predicates import is_async_callable
 from litestar.utils.warnings import warn_pdb_on_exception
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
     from litestar.config.compression import CompressionConfig
     from litestar.config.cors import CORSConfig
     from litestar.config.csrf import CSRFConfig
     from litestar.datastructures import CacheControlHeader, ETag, ResponseHeader
-    from litestar.dto.interface import DTOInterface
+    from litestar.dto import AbstractDTO
     from litestar.events.listener import EventListener
     from litestar.logging.config import BaseLoggingConfig
     from litestar.openapi.spec import SecurityRequirement
     from litestar.openapi.spec.open_api import OpenAPI
-    from litestar.plugins import PluginProtocol
     from litestar.static_files.config import StaticFilesConfig
     from litestar.stores.base import Store
     from litestar.template.config import TemplateConfig
     from litestar.types import (
         AfterExceptionHookHandler,
         AfterRequestHookHandler,
         AfterResponseHookHandler,
@@ -90,14 +92,15 @@
         RouteHandlerType,
         Scope,
         Send,
         TypeEncodersMap,
     )
     from litestar.types.callable_types import LifespanHook
 
+
 __all__ = ("HandlerIndex", "Litestar", "DEFAULT_OPENAPI_CONFIG")
 
 DEFAULT_OPENAPI_CONFIG = OpenAPIConfig(title="Litestar API", version="1.0.0")
 """The default OpenAPI config used if not configuration is explicitly passed to the
 :class:`Litestar <.app.Litestar>` instance constructor.
 """
 
@@ -126,14 +129,15 @@
     and Route Handlers should be registered on it.
     """
 
     __slots__ = (
         "_lifespan_managers",
         "_debug",
         "_openapi_schema",
+        "plugins",
         "after_exception",
         "allowed_hosts",
         "asgi_handler",
         "asgi_router",
         "before_send",
         "compression_config",
         "cors_config",
@@ -142,19 +146,17 @@
         "get_logger",
         "logger",
         "logging_config",
         "multipart_form_part_limit",
         "on_shutdown",
         "on_startup",
         "openapi_config",
-        "openapi_schema_plugins",
         "request_class",
         "response_cache_config",
         "route_map",
-        "serialization_plugins",
         "signature_namespace",
         "state",
         "static_files_config",
         "stores",
         "template_engine",
         "websocket_class",
         "pdb_on_exception",
@@ -170,15 +172,15 @@
         allowed_hosts: Sequence[str] | AllowedHostsConfig | None = None,
         before_request: BeforeRequestHookHandler | None = None,
         before_send: OptionalSequence[BeforeMessageSendHookHandler] | None = None,
         cache_control: CacheControlHeader | None = None,
         compression_config: CompressionConfig | None = None,
         cors_config: CORSConfig | None = None,
         csrf_config: CSRFConfig | None = None,
-        dto: type[DTOInterface] | None | EmptyType = Empty,
+        dto: type[AbstractDTO] | None | EmptyType = Empty,
         debug: bool | None = None,
         dependencies: Dependencies | None = None,
         etag: ETag | None = None,
         event_emitter_backend: type[BaseEventEmitterBackend] = SimpleEventEmitter,
         exception_handlers: ExceptionHandlersMap | None = None,
         guards: OptionalSequence[Guard] | None = None,
         listeners: OptionalSequence[EventListener] | None = None,
@@ -193,15 +195,15 @@
         parameters: ParametersMap | None = None,
         plugins: OptionalSequence[PluginProtocol] | None = None,
         request_class: type[Request] | None = None,
         response_cache_config: ResponseCacheConfig | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: OptionalSequence[ResponseHeader] | None = None,
-        return_dto: type[DTOInterface] | None | EmptyType = Empty,
+        return_dto: type[AbstractDTO] | None | EmptyType = Empty,
         security: OptionalSequence[SecurityRequirement] | None = None,
         signature_namespace: Mapping[str, Any] | None = None,
         state: State | None = None,
         static_files_config: OptionalSequence[StaticFilesConfig] | None = None,
         stores: StoreRegistry | dict[str, Store] | None = None,
         tags: Sequence[str] | None = None,
         template_config: TemplateConfig | None = None,
@@ -234,15 +236,15 @@
                 this app. Can be overridden by route handlers.
             compression_config: Configures compression behaviour of the application, this enabled a builtin or user
                 defined Compression middleware.
             cors_config: If set, configures :class:`CORSMiddleware <.middleware.cors.CORSMiddleware>`.
             csrf_config: If set, configures :class:`CSRFMiddleware <.middleware.csrf.CSRFMiddleware>`.
             debug: If ``True``, app errors rendered as HTML with a stack trace.
             dependencies: A string keyed mapping of dependency :class:`Providers <.di.Provide>`.
-            dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for (de)serializing and
+            dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for (de)serializing and
                 validation of request data.
             etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` to add to route handlers of this app.
                 Can be overridden by route handlers.
             event_emitter_backend: A subclass of
                 :class:`BaseEventEmitterBackend <.events.emitter.BaseEventEmitterBackend>`.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
             guards: A sequence of :class:`Guard <.types.Guard>` callables.
@@ -270,15 +272,15 @@
             plugins: Sequence of plugins.
             request_class: An optional subclass of :class:`Request <.connection.Request>` to use for http connections.
             response_class: A custom subclass of :class:`Response <.response.Response>` to be used as the app's default
                 response.
             response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>`.
             response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
             response_cache_config: Configures caching behavior of the application.
-            return_dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for serializing
+            return_dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for serializing
                 outbound response data.
             route_handlers: A sequence of route handlers, which can include instances of
                 :class:`Router <.router.Router>`, subclasses of :class:`Controller <.controller.Controller>` or any
                 callable decorated by the route handler decorators.
             security: A sequence of dicts that will be added to the schema of all route handlers in the application.
                 See
                 :data:`SecurityRequirement <.openapi.spec.SecurityRequirement>` for details.
@@ -331,20 +333,15 @@
             multipart_form_part_limit=multipart_form_part_limit,
             on_shutdown=list(on_shutdown or []),
             on_startup=list(on_startup or []),
             openapi_config=openapi_config,
             opt=dict(opt or {}),
             parameters=parameters or {},
             pdb_on_exception=pdb_on_exception,
-            plugins=list(
-                chain(
-                    plugins or [],
-                    self.default_plugins,
-                )
-            ),
+            plugins=[*(plugins or []), *self._get_default_plugins()],
             request_class=request_class,
             response_cache_config=response_cache_config or ResponseCacheConfig(),
             response_class=response_class,
             response_cookies=response_cookies or [],
             response_headers=response_headers or [],
             return_dto=return_dto,
             route_handlers=list(route_handlers) if route_handlers is not None else [],
@@ -361,14 +358,16 @@
         )
         for handler in chain(
             on_app_init or [],
             (p.on_app_init for p in config.plugins if isinstance(p, InitPluginProtocol)),
         ):
             config = handler(config)  # pyright: ignore
 
+        self.plugins = PluginRegistry(config.plugins)
+
         self._openapi_schema: OpenAPI | None = None
         self._debug: bool = True
         self._lifespan_managers = config.lifespan
 
         self.get_logger: GetLogger = get_logger_placeholder
         self.logger: Logger | None = None
         self.routes: list[HTTPRoute | ASGIRoute | WebSocketRoute] = []
@@ -383,18 +382,16 @@
         self.csrf_config = config.csrf_config
         self.event_emitter = config.event_emitter_backend(listeners=config.listeners)
         self.logging_config = config.logging_config
         self.multipart_form_part_limit = config.multipart_form_part_limit
         self.on_shutdown = config.on_shutdown
         self.on_startup = config.on_startup
         self.openapi_config = config.openapi_config
-        self.openapi_schema_plugins = [p for p in config.plugins if isinstance(p, OpenAPISchemaPluginProtocol)]
         self.request_class = config.request_class or Request
         self.response_cache_config = config.response_cache_config
-        self.serialization_plugins = [p for p in config.plugins if isinstance(p, SerializationPluginProtocol)]
         self.state = config.state
         self.static_files_config = config.static_files_config
         self.template_engine = config.template_config.engine_instance if config.template_config else None
         self.websocket_class = config.websocket_class or WebSocket
         self.debug = config.debug
         self.pdb_on_exception: bool = config.pdb_on_exception
 
@@ -444,15 +441,30 @@
         self.asgi_handler = self._create_asgi_handler()
 
         self.stores: StoreRegistry = (
             config.stores if isinstance(config.stores, StoreRegistry) else StoreRegistry(config.stores)
         )
 
     @property
-    def default_plugins(self) -> list[PluginProtocol]:
+    @deprecated(version="2.0", alternative="Litestar.plugins.cli", kind="property")
+    def cli_plugins(self) -> list[CLIPluginProtocol]:
+        return list(self.plugins.cli)
+
+    @property
+    @deprecated(version="2.0", alternative="Litestar.plugins.openapi", kind="property")
+    def openapi_schema_plugins(self) -> list[OpenAPISchemaPluginProtocol]:
+        return list(self.plugins.openapi)
+
+    @property
+    @deprecated(version="2.0", alternative="Litestar.plugins.serialization", kind="property")
+    def serialization_plugins(self) -> list[SerializationPluginProtocol]:
+        return list(self.plugins.serialization)
+
+    @staticmethod
+    def _get_default_plugins() -> list[PluginProtocol]:
         default_plugins: list[PluginProtocol] = []
         with suppress(MissingDependencyException):
             from litestar.contrib.pydantic import PydanticInitPlugin, PydanticSchemaPlugin
 
             default_plugins.extend((PydanticInitPlugin(), PydanticSchemaPlugin()))
 
         with suppress(MissingDependencyException):
@@ -802,15 +814,15 @@
                 isinstance(route, HTTPRoute)
                 and any(route_handler.include_in_schema for route_handler, _ in route.route_handler_map.values())
                 and (route.path_format or "/") not in self._openapi_schema.paths
             ):
                 path_item, created_operation_ids = create_path_item(
                     route=route,
                     create_examples=self.openapi_config.create_examples,
-                    plugins=self.openapi_schema_plugins,
+                    plugins=self.plugins.openapi,
                     use_handler_docstrings=self.openapi_config.use_handler_docstrings,
                     operation_id_creator=self.openapi_config.operation_id_creator,
                     schemas=schemas,
                 )
                 self._openapi_schema.paths[route.path_format or "/"] = path_item
 
                 for operation_id in created_operation_ids:
```

### Comparing `litestar-2.0.0b4/litestar/background_tasks.py` & `litestar-2.0.0rc1/litestar/background_tasks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/channels/backends/base.py` & `litestar-2.0.0rc1/litestar/channels/backends/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/channels/backends/memory.py` & `litestar-2.0.0rc1/litestar/channels/backends/memory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/channels/backends/redis.py` & `litestar-2.0.0rc1/litestar/channels/backends/redis.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/channels/plugin.py` & `litestar-2.0.0rc1/litestar/channels/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import asyncio
 from asyncio import CancelledError, Queue, Task, create_task
 from contextlib import AbstractAsyncContextManager, asynccontextmanager, suppress
 from functools import partial
-from os.path import join as join_path
 from typing import TYPE_CHECKING, AsyncGenerator, Awaitable, Callable, Iterable
 
 import msgspec.json
 
 from litestar.di import Provide
 from litestar.exceptions import ImproperlyConfiguredException, LitestarException
 from litestar.handlers import WebsocketRouteHandler
@@ -78,14 +77,18 @@
         self._pub_queue: Queue[tuple[bytes, list[str]]] | None = None
         self._pub_task: Task | None = None
         self._sub_task: Task | None = None
 
         if not (channels or arbitrary_channels_allowed):
             raise ImproperlyConfiguredException("Must define either channels or set arbitrary_channels_allowed=True")
 
+        # make the path absolute, so we can simply concatenate it later
+        if not ws_handler_base_path.endswith("/"):
+            ws_handler_base_path += "/"
+
         self._arbitrary_channels_allowed = arbitrary_channels_allowed
         self._create_route_handlers = create_ws_route_handlers
         self._handler_root_path = ws_handler_base_path
         self._socket_send_mode: WebSocketMode = ws_send_mode
         self._encode_json = msgspec.json.Encoder(
             enc_hook=partial(default_serializer, type_encoders=type_encoders)
         ).encode
@@ -108,19 +111,19 @@
         """Plugin hook. Set up a ``channels`` dependency, add route handlers and register application hooks"""
         app_config.dependencies["channels"] = Provide(lambda: self, use_cache=True, sync_to_thread=False)
         app_config.lifespan.append(self)
         app_config.signature_namespace.update(ChannelsPlugin=ChannelsPlugin)
 
         if self._create_route_handlers:
             if self._arbitrary_channels_allowed:
-                path = join_path(self._handler_root_path, "{channel_name:str}")  # noqa: PTH118
+                path = self._handler_root_path + "{channel_name:str}"
                 route_handlers = [WebsocketRouteHandler(path)(self._ws_handler_func)]
             else:
                 route_handlers = [
-                    WebsocketRouteHandler(join_path(self._handler_root_path, channel_name))(  # noqa: PTH118
+                    WebsocketRouteHandler(self._handler_root_path + channel_name)(
                         self._create_ws_handler_func(channel_name)
                     )
                     for channel_name in self._channels
                 ]
             app_config.route_handlers.extend(route_handlers)
 
         return app_config
```

### Comparing `litestar-2.0.0b4/litestar/channels/subscriber.py` & `litestar-2.0.0rc1/litestar/channels/subscriber.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/cli/_utils.py` & `litestar-2.0.0rc1/litestar/cli/_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 try:
     import rich_click  # noqa: F401
 
     RICH_CLICK_INSTALLED = True
 except ImportError:
     pass
 
-if TYPE_CHECKING or not RICH_CLICK_INSTALLED:
+if TYPE_CHECKING or not RICH_CLICK_INSTALLED:  # pragma: no cover
     from click import ClickException, Command, Context, Group, pass_context
 else:
     from rich_click import ClickException, Context, pass_context
     from rich_click.rich_command import RichCommand as Command  # noqa: TCH002
     from rich_click.rich_group import RichGroup as Group
 
 
@@ -193,20 +193,54 @@
         self,
         name: str | None = None,
         commands: dict[str, Command] | Sequence[Command] | None = None,
         **attrs: Any,
     ) -> None:
         """Init ``LitestarExtensionGroup``"""
         super().__init__(name=name, commands=commands, **attrs)
+        self._prepare_done = False
 
         for entry_point in entry_points(group="litestar.commands"):
             command = entry_point.load()
             _wrap_commands([command])
             self.add_command(command, entry_point.name)
 
+    def _prepare(self, ctx: Context) -> None:
+        if self._prepare_done:
+            return
+
+        if isinstance(ctx.obj, LitestarEnv):
+            env: LitestarEnv | None = ctx.obj
+        else:
+            try:
+                env = ctx.obj = LitestarEnv.from_env(ctx.params.get("app_path"))
+            except LitestarCLIException:
+                env = None
+
+        if env:
+            for plugin in env.app.plugins.cli:
+                plugin.on_cli_init(self)
+
+        self._prepare_done = True
+
+    def make_context(
+        self,
+        info_name: str | None,
+        args: list[str],
+        parent: Context | None = None,
+        **extra: Any,
+    ) -> Context:
+        ctx = super().make_context(info_name, args, parent, **extra)
+        self._prepare(ctx)
+        return ctx
+
+    def list_commands(self, ctx: Context) -> list[str]:
+        self._prepare(ctx)
+        return super().list_commands(ctx)
+
 
 def _inject_args(func: Callable[P, T]) -> Callable[Concatenate[Context, P], T]:
     """Inject the app instance into a ``Command``"""
     params = inspect.signature(func).parameters
 
     @wraps(func)
     def wrapped(ctx: Context, /, *args: P.args, **kwargs: P.kwargs) -> T:
```

### Comparing `litestar-2.0.0b4/litestar/cli/commands/core.py` & `litestar-2.0.0rc1/litestar/cli/commands/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 
 import inspect
 import multiprocessing
 import os
 import subprocess
 import sys
-from typing import TYPE_CHECKING, Any, cast
+from typing import TYPE_CHECKING, Any
 
 import uvicorn
 from rich.tree import Tree
 
-from litestar.cli._utils import RICH_CLICK_INSTALLED, LitestarEnv, console, show_app_info
+from litestar.cli._utils import RICH_CLICK_INSTALLED, console, show_app_info
 from litestar.routes import HTTPRoute, WebSocketRoute
 from litestar.utils.helpers import unwrap_partial
 
-if TYPE_CHECKING or not RICH_CLICK_INSTALLED:
+if TYPE_CHECKING or not RICH_CLICK_INSTALLED:  # pragma: no cover
     import click
     from click import Context, command, option
 else:
     import rich_click as click
     from rich_click import Context, command, option
 
 __all__ = ("info_command", "routes_command", "run_command")
@@ -106,15 +106,23 @@
 
     if debug:
         os.environ["LITESTAR_DEBUG"] = "1"
 
     if pdb:
         os.environ["LITESTAR_PDB"] = "1"
 
-    env = cast(LitestarEnv, ctx.obj())
+    if callable(ctx.obj):
+        ctx.obj = ctx.obj()
+    else:
+        if debug:
+            ctx.obj.app.debug = True
+        if pdb:
+            ctx.obj.app.pdb_on_exception = True
+
+    env = ctx.obj
     app = env.app
 
     reload_dirs = env.reload_dirs or reload_dir
 
     host = env.host or host
     port = env.port if env.port is not None else port
     fd = env.fd if env.fd is not None else fd
```

### Comparing `litestar-2.0.0b4/litestar/cli/commands/schema.py` & `litestar-2.0.0rc1/litestar/cli/commands/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from litestar import Litestar
 from litestar._openapi.typescript_converter.converter import (
     convert_openapi_to_typescript,
 )
 from litestar.cli._utils import RICH_CLICK_INSTALLED, LitestarCLIException, LitestarGroup
 
-if TYPE_CHECKING or not RICH_CLICK_INSTALLED:
+if TYPE_CHECKING or not RICH_CLICK_INSTALLED:  # pragma: no cover
     from click import Path as ClickPath
     from click import group, option
 else:
     from rich_click import Path as ClickPath
     from rich_click import group, option
```

### Comparing `litestar-2.0.0b4/litestar/cli/commands/sessions.py` & `litestar-2.0.0rc1/litestar/cli/commands/sessions.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from litestar import Litestar
 from litestar.cli._utils import RICH_CLICK_INSTALLED, LitestarCLIException, LitestarGroup, console
 from litestar.middleware import DefineMiddleware
 from litestar.middleware.session import SessionMiddleware
 from litestar.middleware.session.server_side import ServerSideSessionBackend
 from litestar.utils import is_class_and_subclass
 
-if TYPE_CHECKING or not RICH_CLICK_INSTALLED:
+if TYPE_CHECKING or not RICH_CLICK_INSTALLED:  # pragma: no cover
     from click import argument, group
 else:
     from rich_click import argument, group
 
 
 __all__ = ("clear_sessions_command", "delete_session_command", "get_session_backend", "sessions_group")
```

### Comparing `litestar-2.0.0b4/litestar/cli/main.py` & `litestar-2.0.0rc1/litestar/cli/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 from ._utils import RICH_CLICK_INSTALLED, LitestarEnv, LitestarExtensionGroup
 from .commands import core, schema, sessions
 
-if TYPE_CHECKING or not RICH_CLICK_INSTALLED:
+if TYPE_CHECKING or not RICH_CLICK_INSTALLED:  # pragma: no cover
     import click
     from click import Context, group, option, pass_context
     from click import Path as ClickPath
 else:
     import rich_click as click
     from rich_click import Context, group, option, pass_context
     from rich_click import Path as ClickPath
@@ -44,15 +44,17 @@
     type=ClickPath(dir_okay=True, file_okay=False, path_type=Path),
     show_default=False,
 )
 @pass_context
 def litestar_group(ctx: Context, app_path: str | None, app_dir: Path | None = None) -> None:
     """Litestar CLI."""
     sys.path.append(str(app_dir))
-    ctx.obj = lambda: LitestarEnv.from_env(app_path)
+
+    if ctx.obj is None:  # env has not been loaded yet, so we can lazy load it
+        ctx.obj = lambda: LitestarEnv.from_env(app_path)
 
 
 # add sub commands here
 
 litestar_group.add_command(core.info_command)
 litestar_group.add_command(core.run_command)
 litestar_group.add_command(core.routes_command)
```

### Comparing `litestar-2.0.0b4/litestar/config/allowed_hosts.py` & `litestar-2.0.0rc1/litestar/config/allowed_hosts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/config/app.py` & `litestar-2.0.0rc1/litestar/config/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     from litestar import Litestar
     from litestar.config.compression import CompressionConfig
     from litestar.config.cors import CORSConfig
     from litestar.config.csrf import CSRFConfig
     from litestar.connection import Request, WebSocket
     from litestar.datastructures import CacheControlHeader, ETag, ResponseHeader
     from litestar.di import Provide
-    from litestar.dto.interface import DTOInterface
+    from litestar.dto import AbstractDTO
     from litestar.events.emitter import BaseEventEmitterBackend
     from litestar.events.listener import EventListener
     from litestar.logging.config import BaseLoggingConfig
     from litestar.openapi.config import OpenAPIConfig
     from litestar.openapi.spec import SecurityRequirement
     from litestar.plugins import PluginProtocol
     from litestar.static_files.config import StaticFilesConfig
@@ -104,16 +104,16 @@
     """If set this enables the builtin CORS middleware."""
     csrf_config: CSRFConfig | None = field(default=None)
     """If set this enables the builtin CSRF middleware."""
     debug: bool = field(default=False)
     """If ``True``, app errors rendered as HTML with a stack trace."""
     dependencies: dict[str, Provide | AnyCallable] = field(default_factory=dict)
     """A string keyed dictionary of dependency :class:`Provider <.di.Provide>` instances."""
-    dto: type[DTOInterface] | None | EmptyType = field(default=Empty)
-    """:class:`DTOInterface <.dto.interface.DTOInterface>` to use for (de)serializing and validation of request data."""
+    dto: type[AbstractDTO] | None | EmptyType = field(default=Empty)
+    """:class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for (de)serializing and validation of request data."""
     etag: ETag | None = field(default=None)
     """An ``etag`` header of type :class:`ETag <.datastructures.ETag>` to add to route handlers of this app.
 
     Can be overridden by route handlers.
     """
     event_emitter_backend: type[BaseEventEmitterBackend] = field(default=SimpleEventEmitter)
     """A subclass of :class:`BaseEventEmitterBackend <.events.emitter.BaseEventEmitterBackend>`."""
@@ -155,16 +155,16 @@
     """A custom subclass of :class:`Response <.response.Response>` to be used as the app's default response."""
     response_cookies: ResponseCookies = field(default_factory=list)  # type: ignore
     """A list of :class:`Cookie <.datastructures.Cookie>`."""
     response_headers: Sequence[ResponseHeader] = field(default_factory=list)
     """A string keyed dictionary mapping :class:`ResponseHeader <.datastructures.ResponseHeader>`."""
     response_cache_config: ResponseCacheConfig = field(default_factory=ResponseCacheConfig)
     """Configures caching behavior of the application."""
-    return_dto: type[DTOInterface] | None | EmptyType = field(default=Empty)
-    """:class:`DTOInterface <.dto.interface.DTOInterface>` to use for serializing outbound response
+    return_dto: type[AbstractDTO] | None | EmptyType = field(default=Empty)
+    """:class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for serializing outbound response
     data.
     """
     route_handlers: list[ControllerRouterHandler] = field(default_factory=list)
     """A required list of route handlers, which can include instances of :class:`Router <.router.Router>`,
     subclasses of :class:`Controller <.controller.Controller>` or any function decorated by the route handler
     decorators.
     """
```

### Comparing `litestar-2.0.0b4/litestar/config/compression.py` & `litestar-2.0.0rc1/litestar/config/compression.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/config/cors.py` & `litestar-2.0.0rc1/litestar/config/cors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/config/csrf.py` & `litestar-2.0.0rc1/litestar/config/csrf.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/config/response_cache.py` & `litestar-2.0.0rc1/litestar/config/response_cache.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/connection/__init__.py` & `litestar-2.0.0rc1/litestar/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/connection/base.py` & `litestar-2.0.0rc1/litestar/connection/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/connection/request.py` & `litestar-2.0.0rc1/litestar/connection/request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/connection/websocket.py` & `litestar-2.0.0rc1/litestar/connection/websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/constants.py` & `litestar-2.0.0rc1/litestar/constants.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/htmx/_utils.py` & `litestar-2.0.0rc1/litestar/contrib/htmx/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/htmx/request.py` & `litestar-2.0.0rc1/litestar/contrib/htmx/request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/htmx/response.py` & `litestar-2.0.0rc1/litestar/contrib/htmx/response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/htmx/types.py` & `litestar-2.0.0rc1/litestar/contrib/htmx/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/jinja.py` & `litestar-2.0.0rc1/litestar/contrib/jinja.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/jwt/__init__.py` & `litestar-2.0.0rc1/litestar/contrib/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/jwt/jwt_auth.py` & `litestar-2.0.0rc1/litestar/contrib/jwt/jwt_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/jwt/jwt_token.py` & `litestar-2.0.0rc1/litestar/contrib/jwt/jwt_token.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/jwt/middleware.py` & `litestar-2.0.0rc1/litestar/contrib/jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/mako.py` & `litestar-2.0.0rc1/litestar/contrib/mako.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/opentelemetry/_utils.py` & `litestar-2.0.0rc1/litestar/contrib/opentelemetry/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/opentelemetry/config.py` & `litestar-2.0.0rc1/litestar/contrib/opentelemetry/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/opentelemetry/middleware.py` & `litestar-2.0.0rc1/litestar/contrib/opentelemetry/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/piccolo.py` & `litestar-2.0.0rc1/litestar/contrib/piccolo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from __future__ import annotations
 
 from dataclasses import replace
-from typing import Any, Generator, Generic, Optional, TypeVar
+from decimal import Decimal
+from typing import Any, Generator, Generic, List, Optional, TypeVar
 
-from _decimal import Decimal
 from msgspec import Meta
 from typing_extensions import Annotated
 
-from litestar.dto import AbstractDTOFactory, DTOField, Mark
+from litestar.dto import AbstractDTO, DTOField, Mark
 from litestar.dto.data_structures import DTOFieldDefinition
 from litestar.exceptions import MissingDependencyException
 from litestar.types import Empty
-from litestar.utils.helpers import get_fully_qualified_class_name
 
 try:
     import piccolo  # noqa: F401
 except ImportError as e:
     raise MissingDependencyException("piccolo") from e
 
 from piccolo.columns import Column, column_types
@@ -32,15 +31,15 @@
     if isinstance(column, (column_types.Decimal, column_types.Numeric)):
         column_type: Any = Decimal
         meta = Meta(extra=extra)
     elif isinstance(column, (column_types.Email, column_types.Varchar)):
         column_type = str
         meta = Meta(max_length=column.length, extra=extra)
     elif isinstance(column, column_types.Array):
-        column_type = list[column.base_column.value_type]  # type: ignore
+        column_type = List[column.base_column.value_type]  # type: ignore
         meta = Meta(extra=extra)
     elif isinstance(column, (column_types.JSON, column_types.JSONB)):
         column_type = str
         meta = Meta(extra={**extra, "format": "json"})
     elif isinstance(column, column_types.Text):
         column_type = str
         meta = Meta(extra={**extra, "format": "text-area"})
@@ -62,27 +61,24 @@
 
     if column._meta.get_choices_dict():
         extra["enum"] = column._meta.get_choices_dict()
 
     return extra
 
 
-class PiccoloDTO(AbstractDTOFactory[T], Generic[T]):
+class PiccoloDTO(AbstractDTO[T], Generic[T]):
     @classmethod
     def generate_field_definitions(cls, model_type: type[Table]) -> Generator[DTOFieldDefinition, None, None]:
-        unique_model_name = get_fully_qualified_class_name(model_type)
-
         for column in model_type._meta.columns:
             yield replace(
                 DTOFieldDefinition.from_field_definition(
                     field_definition=_parse_piccolo_type(column, _create_column_extra(column)),
                     dto_field=DTOField(mark=Mark.READ_ONLY if column._meta.primary_key else None),
-                    unique_model_name=unique_model_name,
+                    model_name=model_type.__name__,
                     default_factory=Empty,
-                    dto_for=None,
                 ),
                 default=Empty if column._meta.required else None,
                 name=column._meta.name,
             )
 
     @classmethod
     def detect_nested_field(cls, field_definition: FieldDefinition) -> bool:
```

### Comparing `litestar-2.0.0b4/litestar/contrib/prometheus/config.py` & `litestar-2.0.0rc1/litestar/contrib/prometheus/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/prometheus/controller.py` & `litestar-2.0.0rc1/litestar/contrib/prometheus/controller.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/prometheus/middleware.py` & `litestar-2.0.0rc1/litestar/contrib/prometheus/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/pydantic/__init__.py` & `litestar-2.0.0rc1/litestar/contrib/pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/pydantic/pydantic_dto_factory.py` & `litestar-2.0.0rc1/litestar/contrib/pydantic/pydantic_dto_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from __future__ import annotations
 
 from dataclasses import replace
 from typing import TYPE_CHECKING, Collection, Generic, TypeVar
 
-from litestar.dto._utils import get_model_type_hints
-from litestar.dto.base_factory import AbstractDTOFactory
+from litestar.dto.base_dto import AbstractDTO
 from litestar.dto.data_structures import DTOFieldDefinition
 from litestar.dto.field import DTO_FIELD_META_KEY, DTOField
 from litestar.exceptions import MissingDependencyException
 from litestar.types.empty import Empty
-from litestar.utils.helpers import get_fully_qualified_class_name
 
 if TYPE_CHECKING:
-    from typing import ClassVar, Generator
+    from typing import Generator
 
     from litestar.typing import FieldDefinition
 
 
 try:
     import pydantic
 
@@ -28,26 +26,22 @@
     raise MissingDependencyException("pydantic") from e
 
 __all__ = ("PydanticDTO",)
 
 T = TypeVar("T", bound="pydantic.BaseModel | Collection[pydantic.BaseModel]")
 
 
-class PydanticDTO(AbstractDTOFactory[T], Generic[T]):
+class PydanticDTO(AbstractDTO[T], Generic[T]):
     """Support for domain modelling with Pydantic."""
 
-    __slots__ = ()
-
-    model_type: ClassVar[type[pydantic.BaseModel]]
-
     @classmethod
     def generate_field_definitions(
         cls, model_type: type[pydantic.BaseModel]
     ) -> Generator[DTOFieldDefinition, None, None]:
-        model_field_definitions = get_model_type_hints(model_type)
+        model_field_definitions = cls.get_model_type_hints(model_type)
 
         if pydantic.VERSION.startswith("1"):  # pragma: no cover
             model_fields: dict[str, pydantic.fields.FieldInfo] = {k: model_field.field_info for k, model_field in model_type.__fields__.items()}  # type: ignore
         else:
             model_fields = dict(model_type.model_fields)
 
         for field_name, field_info in model_fields.items():
@@ -61,19 +55,18 @@
             else:
                 default = Empty
 
             yield replace(
                 DTOFieldDefinition.from_field_definition(
                     field_definition=field_definition,
                     dto_field=dto_field,
-                    unique_model_name=get_fully_qualified_class_name(model_type),
+                    model_name=model_type.__name__,
                     default_factory=field_info.default_factory
                     if field_info.default_factory and field_info.default_factory is not PydanticUndefined  # type: ignore[comparison-overlap]
                     else Empty,
-                    dto_for=None,
                 ),
                 default=default,
                 name=field_name,
             )
 
     @classmethod
     def detect_nested_field(cls, field_definition: FieldDefinition) -> bool:
```

### Comparing `litestar-2.0.0b4/litestar/contrib/pydantic/pydantic_init_plugin.py` & `litestar-2.0.0rc1/litestar/contrib/pydantic/pydantic_init_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 from contextlib import suppress
 from typing import TYPE_CHECKING, Any, Callable, TypeVar, cast
 from uuid import UUID
 
 from msgspec import ValidationError
 
+from litestar._signature.types import ExtendedMsgSpecValidationError
 from litestar.exceptions import MissingDependencyException
 from litestar.plugins import InitPluginProtocol
-from litestar.serialization._msgspec_utils import ExtendedMsgSpecValidationError
 from litestar.utils import is_class_and_subclass, is_pydantic_model_class
 
 if TYPE_CHECKING:
     from litestar.config.app import AppConfig
 
 try:
     import pydantic
```

### Comparing `litestar-2.0.0b4/litestar/contrib/pydantic/pydantic_schema_plugin.py` & `litestar-2.0.0rc1/litestar/contrib/pydantic/pydantic_schema_plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any
+from typing import Any
 
 from typing_extensions import Annotated, get_type_hints
 
 from litestar._openapi.schema_generation.schema import SchemaCreator, _get_type_schema_name
 from litestar.exceptions import MissingDependencyException
 from litestar.openapi.spec import Example, OpenAPIFormat, OpenAPIType, Schema
 from litestar.plugins import OpenAPISchemaPluginProtocol
 from litestar.types import Empty
 from litestar.typing import FieldDefinition
 from litestar.utils import is_class_and_subclass, is_pydantic_model_class, is_undefined_sentinel
 
-if TYPE_CHECKING:
-    from litestar.dto.types import ForType
-
 try:
     import pydantic
 except ImportError as e:
     raise MissingDependencyException("pydantic") from e
 
 PYDANTIC_TYPE_MAP: dict[type[Any] | None | Any, Schema] = {
     pydantic.ByteSize: Schema(type=OpenAPIType.INTEGER),
@@ -135,39 +132,37 @@
 
 
 class PydanticSchemaPlugin(OpenAPISchemaPluginProtocol):
     @staticmethod
     def is_plugin_supported_type(value: Any) -> bool:
         return isinstance(value, _supported_types) or is_class_and_subclass(value, _supported_types)  # type: ignore
 
-    def to_openapi_schema(self, annotation: Any, schema_creator: SchemaCreator, dto_for: ForType | None) -> Schema:
+    def to_openapi_schema(self, field_definition: FieldDefinition, schema_creator: SchemaCreator) -> Schema:
         """Given a type annotation, transform it into an OpenAPI schema class.
 
         Args:
-            annotation: A type annotation.
+            field_definition: FieldDefinition instance.
             schema_creator: An instance of the schema creator class
-            dto_for: The type of the DTO if any.
 
         Returns:
             An :class:`OpenAPI <litestar.openapi.spec.schema.Schema>` instance.
         """
-        if is_pydantic_model_class(annotation):
-            return self.for_pydantic_model(annotation=annotation, schema_creator=schema_creator, dto_for=dto_for)
-        return PYDANTIC_TYPE_MAP[annotation]
+        if is_pydantic_model_class(field_definition.annotation):
+            return self.for_pydantic_model(annotation=field_definition.annotation, schema_creator=schema_creator)
+        return PYDANTIC_TYPE_MAP[field_definition.annotation]  # pragma: no cover
 
     @classmethod
     def for_pydantic_model(
-        cls, annotation: type[pydantic.BaseModel], schema_creator: SchemaCreator, dto_for: ForType | None
+        cls, annotation: type[pydantic.BaseModel], schema_creator: SchemaCreator
     ) -> Schema:  # pyright: ignore
         """Create a schema object for a given pydantic model class.
 
         Args:
             annotation: A pydantic model class.
             schema_creator: An instance of the schema creator class
-            dto_for: The type of the DTO if any.
 
         Returns:
             A schema instance.
         """
 
         annotation_hints = get_type_hints(annotation, include_extras=True)
         model_config = getattr(annotation, "__config__", getattr(annotation, "model_config", Empty))
@@ -176,15 +171,15 @@
             for k, f in getattr(annotation, "__fields__", getattr(annotation, "model_fields", {})).items()
         }
 
         # pydantic v2 logic
         if isinstance(model_config, dict):
             title = model_config.get("title")
             example = model_config.get("example")
-        else:
+        else:  # pragma: no cover
             title = getattr(model_config, "title", None)
             example = getattr(model_config, "example", None)
 
         field_definitions = {
             f.alias
             if f.alias and schema_creator.prefer_alias
             else k: FieldDefinition.from_kwarg(
@@ -197,10 +192,10 @@
             for k, f in model_fields.items()
         }
 
         return Schema(
             required=sorted(f.name for f in field_definitions.values() if f.is_required),
             properties={k: schema_creator.for_field_definition(f) for k, f in field_definitions.items()},
             type=OpenAPIType.OBJECT,
-            title=title or _get_type_schema_name(annotation, dto_for),
+            title=title or _get_type_schema_name(annotation),
             examples=[Example(example)] if example else None,
         )
```

### Comparing `litestar-2.0.0b4/litestar/contrib/repository/abc/_async.py` & `litestar-2.0.0rc1/litestar/contrib/repository/abc/_async.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class AbstractAsyncRepository(Generic[T], metaclass=ABCMeta):
     """Interface for persistent data interaction."""
 
     model_type: type[T]
     """Type of object represented by the repository."""
-    id_attribute = "id"
+    id_attribute: Any = "id"
     """Name of the primary identifying attribute on :attr:`model_type`."""
 
     def __init__(self, **kwargs: Any) -> None:
         """Repository constructors accept arbitrary kwargs."""
         super().__init__(**kwargs)
 
     @abstractmethod
@@ -192,14 +192,33 @@
             The updated or created instance.
 
         Raises:
             NotFoundError: If no instance found with same identifier as ``data``.
         """
 
     @abstractmethod
+    async def upsert_many(self, data: list[T]) -> list[T]:
+        """Update or create multiple instances.
+
+        Update instances with the attribute values present on ``data``, or create a new instance if
+        one doesn't exist.
+
+        Args:
+            data: Instances to update or created. Identifier used to determine if an
+                existing instance exists is the value of an attribute on ``data`` named as value of
+                :attr:`id_attribute <AbstractAsyncRepository.id_attribute>`.
+
+        Returns:
+            The updated or created instances.
+
+        Raises:
+            NotFoundError: If no instance found with same identifier as ``data``.
+        """
+
+    @abstractmethod
     async def list_and_count(self, *filters: FilterTypes, **kwargs: Any) -> tuple[list[T], int]:
         """List records with total count.
 
         Args:
             *filters: Types for specific filtering operations.
             **kwargs: Instance attribute value filters.
 
@@ -249,31 +268,35 @@
             The item, if it exists.
         """
         if item_or_none is None:
             raise NotFoundError("No item found when one was expected")
         return item_or_none
 
     @classmethod
-    def get_id_attribute_value(cls, item: T | type[T]) -> Any:
+    def get_id_attribute_value(cls, item: T | type[T], id_attribute: str | None = None) -> Any:
         """Get value of attribute named as :attr:`id_attribute <AbstractAsyncRepository.id_attribute>` on ``item``.
 
         Args:
             item: Anything that should have an attribute named as :attr:`id_attribute <AbstractAsyncRepository.id_attribute>` value.
+            id_attribute: Allows customization of the unique identifier to use for model fetching.
+                Defaults to `None`, but can reference any surrogate or candidate key for the table.
 
         Returns:
             The value of attribute on ``item`` named as :attr:`id_attribute <AbstractAsyncRepository.id_attribute>`.
         """
-        return getattr(item, cls.id_attribute)
+        return getattr(item, id_attribute if id_attribute is not None else cls.id_attribute)
 
     @classmethod
-    def set_id_attribute_value(cls, item_id: Any, item: T) -> T:
+    def set_id_attribute_value(cls, item_id: Any, item: T, id_attribute: str | None = None) -> T:
         """Return the ``item`` after the ID is set to the appropriate attribute.
 
         Args:
             item_id: Value of ID to be set on instance
             item: Anything that should have an attribute named as :attr:`id_attribute <AbstractAsyncRepository.id_attribute>` value.
+            id_attribute: Allows customization of the unique identifier to use for model fetching.
+                Defaults to `None`, but can reference any surrogate or candidate key for the table.
 
         Returns:
             Item with ``item_id`` set to :attr:`id_attribute <AbstractAsyncRepository.id_attribute>`
         """
-        setattr(item, cls.id_attribute, item_id)
+        setattr(item, id_attribute if id_attribute is not None else cls.id_attribute, item_id)
         return item
```

### Comparing `litestar-2.0.0b4/litestar/contrib/repository/abc/_sync.py` & `litestar-2.0.0rc1/litestar/contrib/repository/abc/_sync.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 class AbstractSyncRepository(Generic[T], metaclass=ABCMeta):
     """Interface for persistent data interaction."""
 
     model_type: type[T]
     """Type of object represented by the repository."""
-    id_attribute = "id"
+    id_attribute: Any = "id"
     """Name of the primary identifying attribute on :attr:`model_type`."""
 
     def __init__(self, **kwargs: Any) -> None:
         """Repository constructors accept arbitrary kwargs."""
         super().__init__(**kwargs)
 
     @abstractmethod
@@ -194,14 +194,33 @@
             The updated or created instance.
 
         Raises:
             NotFoundError: If no instance found with same identifier as ``data``.
         """
 
     @abstractmethod
+    def upsert_many(self, data: list[T]) -> list[T]:
+        """Update or create multiple instances.
+
+        Update instances with the attribute values present on ``data``, or create a new instance if
+        one doesn't exist.
+
+        Args:
+            data: Instances to update or created. Identifier used to determine if an
+                existing instance exists is the value of an attribute on ``data`` named as value of
+                :attr:`id_attribute <AbstractAsyncRepository.id_attribute>`.
+
+        Returns:
+            The updated or created instances.
+
+        Raises:
+            NotFoundError: If no instance found with same identifier as ``data``.
+        """
+
+    @abstractmethod
     def list_and_count(self, *filters: FilterTypes, **kwargs: Any) -> tuple[list[T], int]:
         """List records with total count.
 
         Args:
             *filters: Types for specific filtering operations.
             **kwargs: Instance attribute value filters.
 
@@ -251,31 +270,35 @@
             The item, if it exists.
         """
         if item_or_none is None:
             raise NotFoundError("No item found when one was expected")
         return item_or_none
 
     @classmethod
-    def get_id_attribute_value(cls, item: T | type[T]) -> Any:
+    def get_id_attribute_value(cls, item: T | type[T], id_attribute: str | None = None) -> Any:
         """Get value of attribute named as :attr:`id_attribute <AbstractAsyncRepository.id_attribute>` on ``item``.
 
         Args:
             item: Anything that should have an attribute named as :attr:`id_attribute <AbstractAsyncRepository.id_attribute>` value.
+            id_attribute: Allows customization of the unique identifier to use for model fetching.
+                Defaults to `None`, but can reference any surrogate or candidate key for the table.
 
         Returns:
             The value of attribute on ``item`` named as :attr:`id_attribute <AbstractAsyncRepository.id_attribute>`.
         """
-        return getattr(item, cls.id_attribute)
+        return getattr(item, id_attribute if id_attribute is not None else cls.id_attribute)
 
     @classmethod
-    def set_id_attribute_value(cls, item_id: Any, item: T) -> T:
+    def set_id_attribute_value(cls, item_id: Any, item: T, id_attribute: str | None = None) -> T:
         """Return the ``item`` after the ID is set to the appropriate attribute.
 
         Args:
             item_id: Value of ID to be set on instance
             item: Anything that should have an attribute named as :attr:`id_attribute <AbstractAsyncRepository.id_attribute>` value.
+            id_attribute: Allows customization of the unique identifier to use for model fetching.
+                Defaults to `None`, but can reference any surrogate or candidate key for the table.
 
         Returns:
             Item with ``item_id`` set to :attr:`id_attribute <AbstractAsyncRepository.id_attribute>`
         """
-        setattr(item, cls.id_attribute, item_id)
+        setattr(item, id_attribute if id_attribute is not None else cls.id_attribute, item_id)
         return item
```

### Comparing `litestar-2.0.0b4/litestar/contrib/repository/filters.py` & `litestar-2.0.0rc1/litestar/contrib/repository/filters.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,18 +14,21 @@
 __all__ = (
     "BeforeAfter",
     "CollectionFilter",
     "FilterTypes",
     "LimitOffset",
     "OrderBy",
     "SearchFilter",
+    "NotInCollectionFilter",
+    "OnBeforeAfter",
+    "NotInSearchFilter",
 )
 
 
-FilterTypes: TypeAlias = "BeforeAfter | CollectionFilter[Any] | LimitOffset | OrderBy | SearchFilter"
+FilterTypes: TypeAlias = "BeforeAfter | OnBeforeAfter | CollectionFilter[Any] | LimitOffset | OrderBy | SearchFilter | NotInCollectionFilter[Any] | NotInSearchFilter"
 """Aggregate type alias of the types supported for collection filtering."""
 
 
 @dataclass
 class BeforeAfter:
     """Data required to filter a query on a ``datetime`` column."""
 
@@ -34,24 +37,46 @@
     before: datetime | None
     """Filter results where field earlier than this."""
     after: datetime | None
     """Filter results where field later than this."""
 
 
 @dataclass
+class OnBeforeAfter:
+    """Data required to filter a query on a ``datetime`` column."""
+
+    field_name: str
+    """Name of the model attribute to filter on."""
+    on_or_before: datetime | None
+    """Filter results where field is on or earlier than this."""
+    on_or_after: datetime | None
+    """Filter results where field on or later than this."""
+
+
+@dataclass
 class CollectionFilter(Generic[T]):
     """Data required to construct a ``WHERE ... IN (...)`` clause."""
 
     field_name: str
     """Name of the model attribute to filter on."""
     values: abc.Collection[T]
     """Values for ``IN`` clause."""
 
 
 @dataclass
+class NotInCollectionFilter(Generic[T]):
+    """Data required to construct a ``WHERE ... NOT IN (...)`` clause."""
+
+    field_name: str
+    """Name of the model attribute to filter on."""
+    values: abc.Collection[T]
+    """Values for ``NOT IN`` clause."""
+
+
+@dataclass
 class LimitOffset:
     """Data required to add limit/offset filtering to a query."""
 
     limit: int
     """Value for ``LIMIT`` clause of query."""
     offset: int
     """Value for ``OFFSET`` clause of query."""
@@ -73,7 +98,19 @@
 
     field_name: str
     """Name of the model attribute to sort on."""
     value: str
     """Values for ``LIKE`` clause."""
     ignore_case: bool | None = False
     """Should the search be case insensitive."""
+
+
+@dataclass
+class NotInSearchFilter:
+    """Data required to construct a ``WHERE field_name NOT LIKE '%' || :value || '%'`` clause."""
+
+    field_name: str
+    """Name of the model attribute to search on."""
+    value: str
+    """Values for ``NOT LIKE`` clause."""
+    ignore_case: bool | None = False
+    """Should the search be case insensitive."""
```

### Comparing `litestar-2.0.0b4/litestar/contrib/repository/testing/generic_mock_repository.py` & `litestar-2.0.0rc1/litestar/contrib/repository/testing/generic_mock_repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,17 @@
                 "_model_has_updated_at": hasattr(item, "updated_at"),
             },
         )
 
     def _find_or_raise_not_found(self, item_id: Any) -> ModelT:
         return self.check_not_found(self.collection.get(item_id))
 
+    def _find_or_none(self, item_id: Any) -> ModelT | None:
+        return self.collection.get(item_id)
+
     def _now(self) -> datetime:
         return datetime.now(tz=self.tz).replace(tzinfo=None)
 
     def _update_audit_attributes(self, data: ModelT, now: datetime | None = None, do_created: bool = False) -> ModelT:
         now = now or self._now()
         if self._model_has_updated_at:
             data.updated_at = now  # type:ignore[attr-defined]
@@ -309,14 +312,35 @@
             NotFoundError: If no instance found with same identifier as ``data``.
         """
         item_id = self.get_id_attribute_value(data)
         if item_id in self.collection:
             return await self.update(data)
         return await self.add(data)
 
+    async def upsert_many(self, data: list[ModelT]) -> list[ModelT]:
+        """Update or create multiple instance.
+
+        Update instance with the attribute values present on ``data``, or create a new instance if
+        one doesn't exist.
+
+        Args:
+            data: List of instances to update existing, or be created. Identifier used to determine if an
+                existing instance exists is the value of an attribute on `data` named as value of
+                :attr:`id_attribute <AsyncGenericMockRepository.id_attribute>`.
+
+        Returns:
+            The updated or created instances.
+        """
+        data_to_update = [row for row in data if self._find_or_none(self.get_id_attribute_value(row)) is not None]
+        data_to_add = [row for row in data if self._find_or_none(self.get_id_attribute_value(row)) is None]
+
+        updated_items = await self.update_many(data_to_update)
+        added_items = await self.add_many(data_to_add)
+        return updated_items + added_items
+
     async def list_and_count(
         self,
         *filters: FilterTypes,
         **kwargs: Any,
     ) -> tuple[list[ModelT], int]:
         """Get a list of instances, optionally filtered with a total row count.
 
@@ -418,14 +442,17 @@
                 "_model_has_updated_at": hasattr(item, "updated_at"),
             },
         )
 
     def _find_or_raise_not_found(self, item_id: Any) -> ModelT:
         return self.check_not_found(self.collection.get(item_id))
 
+    def _find_or_none(self, item_id: Any) -> ModelT | None:
+        return self.collection.get(item_id)
+
     def _now(self) -> datetime:
         return datetime.now(tz=self.tz).replace(tzinfo=None)
 
     def _update_audit_attributes(self, data: ModelT, now: datetime | None = None, do_created: bool = False) -> ModelT:
         now = now or self._now()
         if self._model_has_updated_at:
             data.updated_at = now  # type:ignore[attr-defined]
@@ -660,14 +687,35 @@
 
         Raises:
             NotFoundError: If no instance found with same identifier as ``data``.
         """
         item_id = self.get_id_attribute_value(data)
         return self.update(data) if item_id in self.collection else self.add(data)
 
+    def upsert_many(self, data: list[ModelT]) -> list[ModelT]:
+        """Update or create multiple instance.
+
+        Update instance with the attribute values present on ``data``, or create a new instance if
+        one doesn't exist.
+
+        Args:
+            data: List of instances to update existing, or be created. Identifier used to determine if an
+                existing instance exists is the value of an attribute on `data` named as value of
+                :attr:`id_attribute <AsyncGenericMockRepository.id_attribute>`.
+
+        Returns:
+            The updated or created instances.
+        """
+        data_to_update = [row for row in data if self._find_or_none(self.get_id_attribute_value(row)) is not None]
+        data_to_add = [row for row in data if self._find_or_none(self.get_id_attribute_value(row)) is None]
+
+        updated_items = self.update_many(data_to_update)
+        added_items = self.add_many(data_to_add)
+        return updated_items + added_items
+
     def list_and_count(
         self,
         *filters: FilterTypes,
         **kwargs: Any,
     ) -> tuple[list[ModelT], int]:
         """Get a list of instances, optionally filtered with a total row count.
```

### Comparing `litestar-2.0.0b4/litestar/contrib/sqlalchemy/base.py` & `litestar-2.0.0rc1/litestar/contrib/sqlalchemy/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/sqlalchemy/dto.py` & `litestar-2.0.0rc1/litestar/contrib/sqlalchemy/dto.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,53 +5,49 @@
 from typing import TYPE_CHECKING, Collection, Generic, Optional, TypeVar
 
 from sqlalchemy import Column, inspect, orm, sql
 from sqlalchemy.ext.associationproxy import AssociationProxy, AssociationProxyExtensionType
 from sqlalchemy.ext.hybrid import HybridExtensionType, hybrid_property
 from sqlalchemy.orm import (
     ColumnProperty,
+    CompositeProperty,
     DeclarativeBase,
     InspectionAttr,
     Mapped,
+    MappedColumn,
     NotExtension,
     QueryableAttribute,
     RelationshipDirection,
     RelationshipProperty,
 )
 
-from litestar.dto._utils import get_model_type_hints
-from litestar.dto.base_factory import AbstractDTOFactory
+from litestar.dto.base_dto import AbstractDTO
 from litestar.dto.data_structures import DTOFieldDefinition
 from litestar.dto.field import DTO_FIELD_META_KEY, DTOField, Mark
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.types.empty import Empty
 from litestar.typing import FieldDefinition
-from litestar.utils.helpers import get_fully_qualified_class_name
 from litestar.utils.signature import ParsedSignature
 
 if TYPE_CHECKING:
-    from typing import Any, ClassVar, Generator
+    from typing import Any, Generator
 
     from typing_extensions import TypeAlias
 
 __all__ = ("SQLAlchemyDTO",)
 
 T = TypeVar("T", bound="DeclarativeBase | Collection[DeclarativeBase]")
 
-ElementType: TypeAlias = "Column | RelationshipProperty"
+ElementType: TypeAlias = "Column | RelationshipProperty | CompositeProperty"
 SQLA_NS = {**vars(orm), **vars(sql)}
 
 
-class SQLAlchemyDTO(AbstractDTOFactory[T], Generic[T]):
+class SQLAlchemyDTO(AbstractDTO[T], Generic[T]):
     """Support for domain modelling with SQLAlchemy."""
 
-    __slots__ = ()
-
-    model_type: ClassVar[type[DeclarativeBase]]
-
     @singledispatchmethod
     @classmethod
     def handle_orm_descriptor(
         cls,
         extension_type: NotExtension | AssociationProxyExtensionType | HybridExtensionType,
         orm_descriptor: InspectionAttr,
         key: str,
@@ -74,15 +70,15 @@
             raise NotImplementedError(f"Unexpected descriptor type for '{extension_type}': '{orm_descriptor}'")
 
         elem: ElementType
         if isinstance(orm_descriptor.property, ColumnProperty):
             if not isinstance(orm_descriptor.property.expression, Column):
                 raise NotImplementedError(f"Expected 'Column', got: '{orm_descriptor.property.expression}'")
             elem = orm_descriptor.property.expression
-        elif isinstance(orm_descriptor.property, RelationshipProperty):
+        elif isinstance(orm_descriptor.property, (RelationshipProperty, CompositeProperty)):
             elem = orm_descriptor.property
         else:
             raise NotImplementedError(f"Unhandled property type: '{orm_descriptor.property}'")
 
         default, default_factory = _detect_defaults(elem)
 
         try:
@@ -98,16 +94,15 @@
                 field_definition=replace(
                     field_definition,
                     name=key,
                     default=default,
                 ),
                 default_factory=default_factory,
                 dto_field=elem.info.get(DTO_FIELD_META_KEY, DTOField()),
-                dto_for=None,
-                unique_model_name=model_name,
+                model_name=model_name,
             )
         ]
 
     @handle_orm_descriptor.register(AssociationProxyExtensionType)
     @classmethod
     def _(
         cls,
@@ -130,16 +125,15 @@
                 field_definition=replace(
                     field_definition,
                     name=key,
                     default=Empty,
                 ),
                 default_factory=None,
                 dto_field=orm_descriptor.info.get(DTO_FIELD_META_KEY, DTOField(mark=Mark.READ_ONLY)),
-                unique_model_name=model_name,
-                dto_for=None,
+                model_name=model_name,
             )
         ]
 
     @handle_orm_descriptor.register(HybridExtensionType)
     @classmethod
     def _(
         cls,
@@ -159,56 +153,65 @@
                 field_definition=replace(
                     getter_sig.return_type,
                     name=orm_descriptor.__name__,
                     default=Empty,
                 ),
                 default_factory=None,
                 dto_field=orm_descriptor.info.get(DTO_FIELD_META_KEY, DTOField(mark=Mark.READ_ONLY)),
-                unique_model_name=model_name,
-                dto_for="return",
+                model_name=model_name,
             )
         ]
 
         if orm_descriptor.fset is not None:
             setter_sig = ParsedSignature.from_fn(orm_descriptor.fset, {})
             field_defs.append(
                 DTOFieldDefinition.from_field_definition(
                     field_definition=replace(
                         next(iter(setter_sig.parameters.values())),
                         name=orm_descriptor.__name__,
                         default=Empty,
                     ),
                     default_factory=None,
                     dto_field=orm_descriptor.info.get(DTO_FIELD_META_KEY, DTOField(mark=Mark.WRITE_ONLY)),
-                    unique_model_name=model_name,
-                    dto_for="data",
+                    model_name=model_name,
                 )
             )
 
         return field_defs
 
     @classmethod
     def generate_field_definitions(cls, model_type: type[DeclarativeBase]) -> Generator[DTOFieldDefinition, None, None]:
         if (mapper := inspect(model_type)) is None:  # pragma: no cover
             raise RuntimeError("Unexpected `None` value for mapper.")
 
         # includes SQLAlchemy names and other mapped class names in the forward reference resolution namespace
         namespace = {**SQLA_NS, **{m.class_.__name__: m.class_ for m in mapper.registry.mappers if m is not mapper}}
-        model_type_hints = get_model_type_hints(model_type, namespace=namespace)
-        model_name = get_fully_qualified_class_name(model_type)
+        model_type_hints = cls.get_model_type_hints(model_type, namespace=namespace)
+        model_name = model_type.__name__
 
         # the same hybrid property descriptor can be included in `all_orm_descriptors` multiple times, once
         # for each method name it is bound to. We only need to see it once, so track views of it here.
         seen_hybrid_descriptors: set[hybrid_property] = set()
+        skipped_columns: set[str] = set()
+        for composite_property in mapper.composites:
+            for attr in composite_property.attrs:
+                if isinstance(attr, (MappedColumn, Column)):
+                    skipped_columns.add(attr.name)
+                elif isinstance(attr, str):
+                    skipped_columns.add(attr)
         for key, orm_descriptor in mapper.all_orm_descriptors.items():
             if isinstance(orm_descriptor, hybrid_property):
                 if orm_descriptor in seen_hybrid_descriptors:
                     continue
+
                 seen_hybrid_descriptors.add(orm_descriptor)
 
+            if key in skipped_columns:
+                continue
+
             yield from cls.handle_orm_descriptor(
                 orm_descriptor.extension_type, key, orm_descriptor, model_type_hints, model_name
             )
 
     @classmethod
     def detect_nested_field(cls, field_definition: FieldDefinition) -> bool:
         return field_definition.is_subclass_of(DeclarativeBase)
@@ -267,14 +270,17 @@
             return FieldDefinition.from_annotation(collection_type.safe_generic_origin[elem.mapper.class_])
 
         if detect_nullable_relationship(elem):
             return FieldDefinition.from_annotation(Optional[elem.mapper.class_])
 
         return FieldDefinition.from_annotation(elem.mapper.class_)
 
+    if isinstance(elem, CompositeProperty):
+        return FieldDefinition.from_annotation(elem.composite_class)
+
     raise ImproperlyConfiguredException(
         f"Unable to parse type from element '{elem}'. Consider adding a type hint.",
     )
 
 
 def detect_nullable_relationship(elem: RelationshipProperty) -> bool:
     """Detects if a relationship is nullable.
```

### Comparing `litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/__init__.py` & `litestar-2.0.0rc1/litestar/contrib/sqlalchemy/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py` & `litestar-2.0.0rc1/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/init/config/common.py` & `litestar-2.0.0rc1/litestar/contrib/sqlalchemy/plugins/init/config/common.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/init/config/engine.py` & `litestar-2.0.0rc1/litestar/contrib/sqlalchemy/plugins/init/config/engine.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/init/config/sync.py` & `litestar-2.0.0rc1/litestar/contrib/sqlalchemy/plugins/init/config/sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/init/plugin.py` & `litestar-2.0.0rc1/litestar/contrib/sqlalchemy/plugins/init/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 
 __all__ = ("SQLAlchemyInitPlugin",)
 
 
 class SQLAlchemyInitPlugin(InitPluginProtocol, _slots_base.SlotsBase):
     """SQLAlchemy application lifecycle configuration."""
 
-    __slots__ = ()
-
     def __init__(self, config: SQLAlchemyAsyncConfig | SQLAlchemySyncConfig) -> None:
         """Initialize ``SQLAlchemyPlugin``.
 
         Args:
             config: configure DB connection and hook handlers and dependencies.
         """
         self._config = config
```

### Comparing `litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/serialization.py` & `litestar-2.0.0rc1/litestar/contrib/sqlalchemy/plugins/serialization.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 from . import _slots_base
 
 if TYPE_CHECKING:
     from litestar.typing import FieldDefinition
 
 
 class SQLAlchemySerializationPlugin(SerializationPluginProtocol, _slots_base.SlotsBase):
-    __slots__ = ()
-
     def __init__(self) -> None:
         self._type_dto_map: dict[type[DeclarativeBase], type[SQLAlchemyDTO[Any]]] = {}
 
     def supports_type(self, field_definition: FieldDefinition) -> bool:
         return (
             field_definition.is_collection and field_definition.has_inner_subclass_of(DeclarativeBase)
         ) or field_definition.is_subclass_of(DeclarativeBase)
```

### Comparing `litestar-2.0.0b4/litestar/contrib/sqlalchemy/repository/_util.py` & `litestar-2.0.0rc1/litestar/contrib/sqlalchemy/repository/_util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from __future__ import annotations
 
 from contextlib import contextmanager
-from typing import Any
+from typing import TYPE_CHECKING, Any, cast
 
 from sqlalchemy.exc import IntegrityError, SQLAlchemyError
 
 from litestar.contrib.repository import ConflictError, RepositoryError
 
+if TYPE_CHECKING:
+    from sqlalchemy.orm import InstrumentedAttribute
+
+    from litestar.contrib.sqlalchemy.base import ModelProtocol
+
 
 @contextmanager
 def wrap_sqlalchemy_exception() -> Any:
     """Do something within context to raise a `RepositoryError` chained
     from an original `SQLAlchemyError`.
 
         >>> try:
@@ -25,7 +30,13 @@
         yield
     except IntegrityError as exc:
         raise ConflictError from exc
     except SQLAlchemyError as exc:
         raise RepositoryError(f"An exception occurred: {exc}") from exc
     except AttributeError as exc:
         raise RepositoryError from exc
+
+
+def get_instrumented_attr(model: type[ModelProtocol], key: str | InstrumentedAttribute) -> InstrumentedAttribute:
+    if isinstance(key, str):
+        return cast("InstrumentedAttribute", getattr(model, key))
+    return key
```

### Comparing `litestar-2.0.0b4/litestar/contrib/sqlalchemy/repository/types.py` & `litestar-2.0.0rc1/litestar/contrib/sqlalchemy/repository/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/contrib/sqlalchemy/types.py` & `litestar-2.0.0rc1/litestar/contrib/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/controller.py` & `litestar-2.0.0rc1/litestar/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from collections import defaultdict
-from copy import copy, deepcopy
+from copy import deepcopy
 from functools import partial
 from typing import TYPE_CHECKING, Any, Mapping, cast
 
 from litestar._layers.utils import narrow_response_cookies, narrow_response_headers
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.handlers.base import BaseRouteHandler
 from litestar.handlers.http_handlers import HTTPRouteHandler
@@ -14,15 +14,15 @@
 from litestar.utils import AsyncCallable, normalize_path
 
 __all__ = ("Controller",)
 
 
 if TYPE_CHECKING:
     from litestar.datastructures import CacheControlHeader, ETag
-    from litestar.dto.interface import DTOInterface
+    from litestar.dto import AbstractDTO
     from litestar.openapi.spec import SecurityRequirement
     from litestar.response import Response
     from litestar.router import Router
     from litestar.types import (
         AfterRequestHookHandler,
         AfterResponseHookHandler,
         BeforeRequestHookHandler,
@@ -90,16 +90,16 @@
     """A :class:`CacheControlHeader <.datastructures.CacheControlHeader>` header to add to route handlers of this
     controller.
 
     Can be overridden by route handlers.
     """
     dependencies: Dependencies | None
     """A string keyed dictionary of dependency :class:`Provider <.di.Provide>` instances."""
-    dto: type[DTOInterface] | None | EmptyType
-    """:class:`DTOInterface <.dto.interface.DTOInterface>` to use for (de)serializing and validation of request data."""
+    dto: type[AbstractDTO] | None | EmptyType
+    """:class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for (de)serializing and validation of request data."""
     etag: ETag | None
     """An ``etag`` header of type :class:`ETag <.datastructures.ETag>` to add to route handlers of this controller.
 
     Can be overridden by route handlers.
     """
     exception_handlers: ExceptionHandlersMap | None
     """A map of handler functions to status codes and/or exception types."""
@@ -127,16 +127,16 @@
     """A custom subclass of :class:`Response <.response.Response>` to be used as the default response for all route
     handlers under the controller.
     """
     response_cookies: ResponseCookies | None
     """A list of :class:`Cookie <.datastructures.Cookie>` instances."""
     response_headers: ResponseHeaders | None
     """A string keyed dictionary mapping :class:`ResponseHeader <.datastructures.ResponseHeader>` instances."""
-    return_dto: type[DTOInterface] | None | EmptyType
-    """:class:`DTOInterface <.dto.interface.DTOInterface>` to use for serializing outbound response
+    return_dto: type[AbstractDTO] | None | EmptyType
+    """:class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for serializing outbound response
     data.
     """
     tags: OptionalSequence[str]
     """A sequence of string tags that will be appended to the schema of all route handlers under the controller."""
     security: OptionalSequence[SecurityRequirement]
     """A sequence of dictionaries that to the schema of all route handlers under the controller."""
     signature_namespace: dict[str, Any]
@@ -180,22 +180,20 @@
 
     def get_route_handlers(self) -> list[BaseRouteHandler]:
         """Get a controller's route handlers and set the controller as the handlers' owner.
 
         Returns:
             A list containing a copy of the route handlers defined on the controller
         """
-        from litestar import websocket_listener
 
         route_handlers: list[BaseRouteHandler] = []
 
         for field_name in set(dir(self)) - set(dir(Controller)):
             if (attr := getattr(self, field_name, None)) and isinstance(attr, BaseRouteHandler):
-                # we are special casing here because the websocket_listener context cannot be deep copied without breaking
-                route_handler = copy(attr) if isinstance(attr, websocket_listener) else deepcopy(attr)
+                route_handler = deepcopy(attr)
                 route_handler.fn.value = partial(route_handler.fn.value, self)
                 route_handler.owner = self
                 route_handlers.append(route_handler)
 
         self.validate_route_handlers(route_handlers=route_handlers)
 
         return route_handlers
```

### Comparing `litestar-2.0.0b4/litestar/data_extractors.py` & `litestar-2.0.0rc1/litestar/data_extractors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/datastructures/__init__.py` & `litestar-2.0.0rc1/litestar/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/datastructures/cookie.py` & `litestar-2.0.0rc1/litestar/datastructures/cookie.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/datastructures/headers.py` & `litestar-2.0.0rc1/litestar/datastructures/headers.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from multidict import CIMultiDict, CIMultiDictProxy, MultiMapping
 from typing_extensions import get_type_hints
 
 from litestar._multipart import parse_content_header
 from litestar._parsers import parse_headers
 from litestar.datastructures.multi_dicts import MultiMixin
-from litestar.dto._utils import resolve_model_type
+from litestar.dto.base_dto import AbstractDTO
 from litestar.exceptions import ImproperlyConfiguredException, ValidationException
 
 __all__ = ("Accept", "CacheControlHeader", "ETag", "Header", "Headers", "MutableScopeHeaders")
 
 from litestar.typing import FieldDefinition
 from litestar.utils.dataclass import simple_asdict
 
@@ -66,15 +66,15 @@
                     headers_ = headers  # pyright: ignore
                 else:
                     headers_ = [(key.decode("latin-1"), value.decode("latin-1")) for key, value in headers]
 
             super().__init__(CIMultiDict(headers_))
         else:
             super().__init__(headers)
-        self._header_list: Optional["RawHeadersList"] = None
+        self._header_list: Optional[RawHeadersList] = None
 
     @classmethod
     def from_scope(cls, scope: "HeaderScope") -> "Headers":
         """Create headers from a send-message.
 
         Args:
             scope: The ASGI connection scope.
@@ -108,15 +108,15 @@
 
     def __init__(self, scope: Optional["HeaderScope"] = None) -> None:
         """Initialize ``MutableScopeHeaders`` from a ``HeaderScope``.
 
         Args:
             scope: The ASGI connection scope.
         """
-        self.headers: "RawHeadersList"
+        self.headers: RawHeadersList
         if scope is not None:
             if not isinstance(scope["headers"], list):
                 scope["headers"] = list(scope["headers"])
 
             self.headers = cast("RawHeadersList", scope["headers"])
         else:
             self.headers = []
@@ -365,15 +365,15 @@
         """
 
         if cls._field_definitions is None:
             cls._field_definitions = {}
             for key, value in get_type_hints(cls, include_extras=True).items():
                 definition = FieldDefinition.from_kwarg(annotation=value, name=key)
                 # resolve_model_type so that field_definition.raw has the real raw type e.g. <class 'bool'>
-                cls._field_definitions[key] = resolve_model_type(definition)
+                cls._field_definitions[key] = AbstractDTO.resolve_model_type(definition)
         return cls._field_definitions
 
     @classmethod
     def _convert_to_type(cls, value: str, field_definition: FieldDefinition) -> Any:
         """Convert the value to the expected type.
 
         Args:
```

### Comparing `litestar-2.0.0b4/litestar/datastructures/multi_dicts.py` & `litestar-2.0.0rc1/litestar/datastructures/multi_dicts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/datastructures/response_header.py` & `litestar-2.0.0rc1/litestar/datastructures/response_header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/datastructures/state.py` & `litestar-2.0.0rc1/litestar/datastructures/state.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/datastructures/upload_file.py` & `litestar-2.0.0rc1/litestar/datastructures/upload_file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/datastructures/url.py` & `litestar-2.0.0rc1/litestar/datastructures/url.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/di.py` & `litestar-2.0.0rc1/litestar/di.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from inspect import isclass
 from typing import TYPE_CHECKING, Any
 
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.types import Empty
-from litestar.utils import Ref
+from litestar.utils import Ref, async_partial
 from litestar.utils.predicates import is_async_callable, is_sync_or_async_generator
 from litestar.utils.warnings import (
     warn_implicit_sync_to_thread,
     warn_sync_to_thread_with_async_callable,
     warn_sync_to_thread_with_generator,
 )
 
@@ -49,24 +49,30 @@
             dependency: Callable to call or class to instantiate. The result is then injected as a dependency.
             use_cache: Cache the dependency return value. Defaults to False.
             sync_to_thread: Run sync code in an async thread. Defaults to False.
         """
         if not callable(dependency):
             raise ImproperlyConfiguredException("Provider dependency must a callable value")
 
-        self.dependency = Ref["AnyCallable"](dependency)
-        self.has_sync_callable = isclass(dependency) or not is_async_callable(dependency)
-        if self.has_sync_callable and sync_to_thread is None and not is_sync_or_async_generator(dependency):
-            warn_implicit_sync_to_thread(dependency, stacklevel=3)
+        has_sync_callable = isclass(dependency) or not is_async_callable(dependency)
 
         if sync_to_thread is not None:
             if is_sync_or_async_generator(dependency):
                 warn_sync_to_thread_with_generator(dependency, stacklevel=3)
-            elif not self.has_sync_callable:
+            elif not has_sync_callable:
                 warn_sync_to_thread_with_async_callable(dependency, stacklevel=3)  # pyright: ignore
+        elif has_sync_callable and not is_sync_or_async_generator(dependency):
+            warn_implicit_sync_to_thread(dependency, stacklevel=3)
+
+        if sync_to_thread and has_sync_callable:
+            self.dependency = Ref["AnyCallable"](async_partial(dependency))  # pyright: ignore
+            self.has_sync_callable = False
+        else:
+            self.dependency = Ref["AnyCallable"](dependency)  # pyright: ignore
+            self.has_sync_callable = has_sync_callable
 
         self.sync_to_thread = bool(sync_to_thread)
         self.use_cache = use_cache
         self.value: Any = Empty
 
     async def __call__(self, **kwargs: Any) -> Any:
         """Call the provider's dependency."""
```

### Comparing `litestar-2.0.0b4/litestar/dto/_backend.py` & `litestar-2.0.0rc1/litestar/typing.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,559 +1,570 @@
-"""DTO backends do the heavy lifting of decoding and validating raw bytes into domain models, and
-back again, to bytes.
-"""
 from __future__ import annotations
 
-import secrets
-from typing import TYPE_CHECKING, Any, Final, cast
-
-from msgspec import Struct, convert
-
-from litestar.dto._types import (
-    CollectionType,
-    CompositeType,
-    MappingType,
-    NestedFieldInfo,
-    SimpleType,
-    TransferDTOFieldDefinition,
-    TupleType,
-    UnionType,
+from collections import abc, deque
+from copy import deepcopy
+from dataclasses import dataclass, replace
+from inspect import Parameter, Signature
+from typing import Any, AnyStr, Callable, Collection, ForwardRef, Literal, Mapping, Sequence, TypeVar, cast
+
+from msgspec import UnsetType
+from typing_extensions import Annotated, NotRequired, Required, Self, get_args, get_origin
+
+from litestar.exceptions import ImproperlyConfiguredException
+from litestar.openapi.spec import Example
+from litestar.params import BodyKwarg, DependencyKwarg, KwargDefinition, ParameterKwarg
+from litestar.types import Empty
+from litestar.types.builtin_types import NoneType, UnionTypes
+from litestar.utils.predicates import (
+    is_annotated_type,
+    is_any,
+    is_class_and_subclass,
+    is_generic,
+    is_non_string_iterable,
+    is_non_string_sequence,
+    is_pydantic_constrained_field,
 )
-from litestar.dto._utils import (
-    RenameStrategies,
-    build_annotation_for_backend,
-    create_struct_for_field_definitions,
-    should_exclude_field,
-    should_ignore_field,
-    should_mark_private,
-    transfer_data,
+from litestar.utils.typing import (
+    get_instantiable_origin,
+    get_safe_generic_origin,
+    make_non_optional_union,
+    unwrap_annotation,
 )
-from litestar.dto.data_structures import DTOData
-from litestar.dto.field import Mark
-from litestar.enums import RequestEncodingType
-from litestar.exceptions import SerializationException
-from litestar.serialization import decode_json, decode_msgpack
-from litestar.typing import FieldDefinition
-from litestar.utils.helpers import get_fully_qualified_class_name
-
-if TYPE_CHECKING:
-    from typing import AbstractSet, Callable, Collection, Generator
-
-    from litestar._openapi.schema_generation import SchemaCreator
-    from litestar.dto import DTOConfig
-    from litestar.dto._types import FieldDefinitionsType
-    from litestar.dto.data_structures import DTOFieldDefinition
-    from litestar.dto.interface import ConnectionContext
-    from litestar.dto.types import ForType
-    from litestar.openapi.spec import Reference, Schema
-    from litestar.types.serialization import LitestarEncodableType
 
-__all__ = ("DTOBackend", "BackendContext")
+try:
+    from pydantic.fields import FieldInfo
+except ImportError:
+    FieldInfo = Empty  # type: ignore
 
+__all__ = ("FieldDefinition",)
 
-class BackendContext:
-    """Context required by DTO backends to perform their work."""
+T = TypeVar("T", bound=KwargDefinition)
 
-    __slots__ = (
-        "config",
-        "dto_for",
-        "field_definition_generator",
-        "is_nested_field_predicate",
-        "model_type",
-        "field_definition",
-        "wrapper_attribute_name",
-    )
 
-    def __init__(
-        self,
-        dto_config: DTOConfig,
-        dto_for: ForType,
-        field_definition: FieldDefinition,
-        field_definition_generator: Callable[[Any], Generator[DTOFieldDefinition, None, None]],
-        is_nested_field_predicate: Callable[[FieldDefinition], bool],
-        model_type: type[Any],
-        wrapper_attribute_name: str | None,
-    ) -> None:
-        """Create a backend context.
+def _unpack_predicate(value: Any) -> dict[str, Any]:
+    try:
+        from annotated_types import Predicate
 
-        Args:
-            dto_config: DTO config.
-            dto_for: "data" or "return"
-            field_definition: Parsed type.
-            field_definition_generator: Generator that produces
-                :class:`FieldDefinition <.dto.factory.types.FieldDefinition>` instances given ``model_type``.
-            is_nested_field_predicate: Function that detects if a field is nested.
-            model_type: Model type.
-            wrapper_attribute_name: If the data that DTO should operate upon is wrapped in a generic datastructure, this is the
-                name of the attribute that the data is stored in.
-        """
-        self.config: Final[DTOConfig] = dto_config
-        self.dto_for: Final[ForType] = dto_for
-        self.field_definition: Final[FieldDefinition] = field_definition
-        self.field_definition_generator: Final[
-            Callable[[Any], Generator[DTOFieldDefinition, None, None]]
-        ] = field_definition_generator
-        self.is_nested_field_predicate: Final[Callable[[FieldDefinition], bool]] = is_nested_field_predicate
-        self.model_type: Final[type[Any]] = model_type
-        self.wrapper_attribute_name = wrapper_attribute_name
+        if isinstance(value, Predicate):
+            if value.func == str.islower:
+                return {"lower_case": True}
+            if value.func == str.isupper:
+                return {"upper_case": True}
+            if value.func == str.isascii:
+                return {"pattern": "[[:ascii:]]"}
+            if value.func == str.isdigit:
+                return {"pattern": "[[:digit:]]"}
+    except ImportError:
+        pass
 
+    return {}
 
-class NestedDepthExceededError(Exception):
-    """Raised when a nested type exceeds the maximum allowed depth.
-
-    Not an exception that is intended to be raised into userland, rather a signal to the process that is iterating over
-    the field definitions that the current field should be skipped.
-    """
 
+def _parse_metadata(value: Any, is_sequence_container: bool, extra: dict[str, Any] | None) -> dict[str, Any]:
+    """Parse metadata from a value.
 
-class DTOBackend:
-    __slots__ = (
-        "annotation",
-        "context",
-        "dto_data_type",
-        "parsed_field_definitions",
-        "reverse_name_map",
-        "transfer_model_type",
-    )
+    Args:
+        value: A metadata value from annotation, namely anything stored under Annotated[x, metadata...]
+        is_sequence_container: Whether the type is a sequence container (list, tuple etc...)
+        extra: Extra key values to parse.
 
-    def __init__(self, context: BackendContext) -> None:
-        """Create dto backend instance.
+    Returns:
+        A dictionary of constraints, which fulfill the kwargs of a KwargDefinition class.
+    """
+    extra = {
+        **cast("dict[str, Any]", extra or getattr(value, "extra", None) or {}),
+        **(getattr(value, "json_schema_extra", None) or {}),
+    }
+    if example := extra.pop("example", None):
+        example_list = [Example(value=example)]
+    elif examples := getattr(value, "examples", None):
+        example_list = [Example(value=example) for example in cast("list[str]", examples)]
+    else:
+        example_list = None
+
+    return {
+        k: v
+        for k, v in {
+            "gt": getattr(value, "gt", None),
+            "ge": getattr(value, "ge", None),
+            "lt": getattr(value, "lt", None),
+            "le": getattr(value, "le", None),
+            "multiple_of": getattr(value, "multiple_of", None),
+            "min_length": None if is_sequence_container else getattr(value, "min_length", None),
+            "max_length": None if is_sequence_container else getattr(value, "max_length", None),
+            "description": getattr(value, "description", None),
+            "examples": example_list,
+            "title": getattr(value, "title", None),
+            "lower_case": getattr(value, "to_lower", None),
+            "upper_case": getattr(value, "to_upper", None),
+            "pattern": getattr(value, "regex", getattr(value, "pattern", None)),
+            "min_items": getattr(value, "min_items", getattr(value, "min_length", None))
+            if is_sequence_container
+            else None,
+            "max_items": getattr(value, "max_items", getattr(value, "max_length", None))
+            if is_sequence_container
+            else None,
+            "const": getattr(value, "const", None) is not None,
+            **extra,
+        }.items()
+        if v is not None
+    }
+
+
+def _traverse_metadata(
+    metadata: Sequence[Any], is_sequence_container: bool, extra: dict[str, Any] | None
+) -> dict[str, Any]:
+    """Recursively traverse metadata from a value.
+
+    Args:
+        metadata: A list of metadata values from annotation, namely anything stored under Annotated[x, metadata...]
+        is_sequence_container: Whether or not the container is a sequence container (list, tuple etc...)
+        extra: Extra key values to parse.
 
-        Args:
-            context: context of the type represented by this backend.
-        """
-        self.context = context
-        self.parsed_field_definitions = self.parse_model(
-            model_type=context.model_type, exclude=context.config.exclude, include=context.config.include
-        )
-        self.transfer_model_type = self.create_transfer_model_type(
-            get_fully_qualified_class_name(context.model_type), self.parsed_field_definitions
-        )
-        self.dto_data_type: type[DTOData] | None = None
-        if context.field_definition.is_subclass_of(DTOData):
-            self.dto_data_type = context.field_definition.annotation
-            annotation = self.context.field_definition.inner_types[0].annotation
+    Returns:
+        A dictionary of constraints, which fulfill the kwargs of a KwargDefinition class.
+    """
+    constraints: dict[str, Any] = {}
+    for value in metadata:
+        if isinstance(value, (list, set, frozenset, deque)):
+            constraints.update(
+                _traverse_metadata(
+                    metadata=cast("Sequence[Any]", value), is_sequence_container=is_sequence_container, extra=extra
+                )
+            )
+        elif is_annotated_type(value) and (type_args := [v for v in get_args(value) if v is not None]):
+            # annotated values can be nested inside other annotated values
+            # this behaviour is buggy in python 3.8, hence we need to guard here.
+            if len(type_args) > 1:
+                constraints.update(
+                    _traverse_metadata(metadata=type_args[1:], is_sequence_container=is_sequence_container, extra=extra)
+                )
+        elif unpacked_predicate := _unpack_predicate(value):
+            constraints.update(unpacked_predicate)
         else:
-            annotation = context.field_definition.annotation
-        self.annotation = build_annotation_for_backend(annotation, self.transfer_model_type)
-
-    def parse_model(
-        self, model_type: Any, exclude: AbstractSet[str], include: AbstractSet[str], nested_depth: int = 0
-    ) -> FieldDefinitionsType:
-        """Reduce :attr:`model_type` to :class:`FieldDefinitionsType`.
-
-        .. important::
-            Implementations must respect the :attr:`config` object. For example:
-                - fields marked private must never be included in the field definitions.
-                - if a ``purpose`` is declared, then read-only fields must be taken into account.
-                - field renaming must be implemented.
-                - additional fields must be included, subject to ``purpose``.
-                - nested depth and nested recursion depth must be adhered to.
-
-        Returns:
-            Fields for data transfer.
+            constraints.update(_parse_metadata(value=value, is_sequence_container=is_sequence_container, extra=extra))
+    return constraints
 
-            Key is the name of the new field, and value is a tuple of type and default value pairs.
 
-            Add a new field called "new_field", that is a string, and required:
-            {"new_field": (str, ...)}
+def _create_metadata_from_type(
+    metadata: Sequence[Any], model: type[T], annotation: Any, extra: dict[str, Any] | None
+) -> tuple[T | None, dict[str, Any]]:
+    is_sequence_container = is_non_string_sequence(annotation)
+    result = _traverse_metadata(metadata=metadata, is_sequence_container=is_sequence_container, extra=extra)
 
-            Add a new field called "new_field", that is a string, and not-required:
-            {"new_field": (str, "default")}
+    constraints = {k: v for k, v in result.items() if k in dir(model)}
+    extra = {k: v for k, v in result.items() if k not in constraints}
+    return model(**constraints) if constraints else None, extra
 
-            Add a new field called "new_field", that may be `None`:
-            {"new_field": (str | None, None)}
-        """
-        defined_fields = []
-        for field_definition in self.context.field_definition_generator(model_type):
-            if should_ignore_field(field_definition, self.context.dto_for):
-                continue
-
-            if should_mark_private(field_definition, self.context.config.underscore_fields_private):
-                field_definition.dto_field.mark = Mark.PRIVATE
-
-            try:
-                transfer_type = self._create_transfer_type(
-                    field_definition=field_definition,
-                    exclude=exclude,
-                    include=include,
-                    field_name=field_definition.name,
-                    unique_name=field_definition.unique_name(),
-                    nested_depth=nested_depth,
-                )
-            except NestedDepthExceededError:
-                continue
 
-            if rename := self.context.config.rename_fields.get(field_definition.name):
-                serialization_name = rename
-            elif self.context.config.rename_strategy:
-                serialization_name = RenameStrategies(self.context.config.rename_strategy)(field_definition.name)
-            else:
-                serialization_name = field_definition.name
+@dataclass(frozen=True)
+class FieldDefinition:
+    """Represents a function parameter or type annotation."""
 
-            transfer_field_definition = TransferDTOFieldDefinition.from_dto_field_definition(
-                field_definition=field_definition,
-                serialization_name=serialization_name,
-                transfer_type=transfer_type,
-                is_partial=self.context.config.partial,
-                is_excluded=should_exclude_field(
-                    field_definition=field_definition, exclude=exclude, include=include, dto_for=self.context.dto_for
-                ),
-            )
-            defined_fields.append(transfer_field_definition)
-        return tuple(defined_fields)
+    __slots__ = (
+        "annotation",
+        "args",
+        "default",
+        "extra",
+        "inner_types",
+        "instantiable_origin",
+        "kwarg_definition",
+        "metadata",
+        "name",
+        "origin",
+        "raw",
+        "safe_generic_origin",
+        "type_wrappers",
+    )
 
-    def create_transfer_model_type(self, unique_name: str, field_definitions: FieldDefinitionsType) -> type[Struct]:
-        """Create a model for data transfer.
+    raw: Any
+    """The annotation exactly as received."""
+    annotation: Any
+    """The annotation with any "wrapper" types removed, e.g. Annotated."""
+    type_wrappers: tuple[type, ...]
+    """A set of all "wrapper" types, e.g. Annotated."""
+    origin: Any
+    """The result of calling ``get_origin(annotation)`` after unwrapping Annotated, e.g. list."""
+    args: tuple[Any, ...]
+    """The result of calling ``get_args(annotation)`` after unwrapping Annotated, e.g. (int,)."""
+    metadata: tuple[Any, ...]
+    """Any metadata associated with the annotation via ``Annotated``."""
+    instantiable_origin: Any
+    """An equivalent type to ``origin`` that can be safely instantiated. E.g., ``Sequence`` -> ``list``."""
+    safe_generic_origin: Any
+    """An equivalent type to ``origin`` that can be safely used as a generic type across all supported Python versions.
 
-        Args:
-            unique_name: name for the type that should be unique across all transfer types.
-            field_definitions: field definitions for the container type.
+    This is to serve safely rebuilding a generic outer type with different args at runtime.
+    """
+    inner_types: tuple[FieldDefinition, ...]
+    """The type's generic args parsed as ``FieldDefinition``, if applicable."""
+    default: Any
+    """Default value of the field."""
+    extra: dict[str, Any]
+    """A mapping of extra values."""
+    kwarg_definition: KwargDefinition | DependencyKwarg | None
+    """Kwarg Parameter."""
+    name: str
+    """Field name."""
+
+    def __deepcopy__(self, memo: dict[str, Any]) -> Self:
+        return type(self)(**{attr: deepcopy(getattr(self, attr)) for attr in self.__slots__})
+
+    def __eq__(self, other: Any) -> bool:
+        if not isinstance(other, FieldDefinition):
+            return False
+
+        if self.origin:
+            return self.origin == other.origin and self.inner_types == other.inner_types
+
+        return self.annotation == other.annotation  # type: ignore[no-any-return]
+
+    def __hash__(self) -> int:
+        return hash((self.name, self.raw, self.annotation, self.origin, self.inner_types))
+
+    @classmethod
+    def _extract_metadata(
+        cls, annotation: Any, name: str | None, default: Any, metadata: tuple[Any, ...], extra: dict[str, Any] | None
+    ) -> tuple[KwargDefinition | None, dict[str, Any]]:
+        from litestar.dto.base_dto import AbstractDTO
+
+        model = BodyKwarg if name == "data" else ParameterKwarg
+        if isinstance(default, FieldInfo):
+            return _create_metadata_from_type(metadata=[default], model=model, annotation=annotation, extra=extra)
+
+        if is_pydantic_constrained_field(annotation) or isinstance(annotation, AbstractDTO):
+            return _create_metadata_from_type(metadata=[annotation], model=model, annotation=annotation, extra=extra)
+
+        if any(isinstance(arg, KwargDefinition) for arg in get_args(annotation)):
+            return next(arg for arg in get_args(annotation) if isinstance(arg, KwargDefinition)), extra or {}
+
+        if metadata:
+            return _create_metadata_from_type(metadata=metadata, model=model, annotation=annotation, extra=extra)
+
+        return None, {}
+
+    @property
+    def has_default(self) -> bool:
+        """Check if the field has a default value.
 
         Returns:
-            A ``BackendT`` class.
+            True if the default is not Empty or Ellipsis otherwise False.
         """
-        fqn_uid: str = self._gen_unique_name_id(unique_name)
-        struct = create_struct_for_field_definitions(fqn_uid, field_definitions)
-        setattr(struct, "__schema_name__", unique_name)
-        return struct
+        return self.default is not Empty and self.default is not Ellipsis
 
-    def parse_raw(self, raw: bytes, connection_context: ConnectionContext) -> Struct | Collection[Struct]:
-        """Parse raw bytes into transfer model type.
+    @property
+    def is_non_string_iterable(self) -> bool:
+        """Check if the field type is an Iterable.
 
-        Args:
-            raw: bytes
-            connection_context: Information about the active connection.
+        If ``self.annotation`` is an optional union, only the non-optional members of the union are evaluated.
 
-        Returns:
-            The raw bytes parsed into transfer model type.
+        See: https://github.com/litestar-org/litestar/issues/1106
         """
+        annotation = self.annotation
+        if self.is_optional:
+            annotation = make_non_optional_union(annotation)
+        return is_non_string_iterable(annotation)
+
+    @property
+    def is_non_string_sequence(self) -> bool:
+        """Check if the field type is a non-string Sequence.
 
-        if connection_context.request_encoding_type not in [RequestEncodingType.JSON, RequestEncodingType.MESSAGEPACK]:
-            raise SerializationException(
-                f"Unsupported request encoding type: '{connection_context.request_encoding_type}'"
-            )
-
-        if connection_context.request_encoding_type == RequestEncodingType.JSON:
-            result = decode_json(value=raw, target_type=self.annotation, type_decoders=connection_context.type_decoders)
-        else:
-            result = decode_msgpack(
-                value=raw, target_type=self.annotation, type_decoders=connection_context.type_decoders
-            )
-
-        return cast("Struct | Collection[Struct]", result)
+        If ``self.annotation`` is an optional union, only the non-optional members of the union are evaluated.
 
-    def parse_builtins(self, builtins: Any, connection_context: ConnectionContext) -> Any:
-        """Parse builtin types into transfer model type.
-
-        Args:
-            builtins: Builtin type.
-            connection_context: Information about the active connection.
-
-        Returns:
-            The builtin type parsed into transfer model type.
+        See: https://github.com/litestar-org/litestar/issues/1106
         """
-        return convert(
-            obj=builtins, type=self.annotation, dec_hook=connection_context.default_deserializer, strict=False
-        )
+        annotation = self.annotation
+        if self.is_optional:
+            annotation = make_non_optional_union(annotation)
+        return is_non_string_sequence(annotation)
+
+    @property
+    def is_any(self) -> bool:
+        """Check if the field type is Any."""
+        return is_any(self.annotation)
+
+    @property
+    def is_generic(self) -> bool:
+        """Check if the field type is a custom class extending Generic."""
+        return is_generic(self.annotation)
+
+    @property
+    def is_simple_type(self) -> bool:
+        """Check if the field type is a singleton value (e.g. int, str etc.)."""
+        return not (
+            self.is_generic or self.is_optional or self.is_union or self.is_mapping or self.is_non_string_iterable
+        )
+
+    @property
+    def is_parameter_field(self) -> bool:
+        """Check if the field type is a parameter kwarg value."""
+        return isinstance(self.kwarg_definition, ParameterKwarg)
+
+    @property
+    def is_const(self) -> bool:
+        """Check if the field is defined as constant value."""
+        return bool(self.kwarg_definition and getattr(self.kwarg_definition, "const", False))
+
+    @property
+    def is_required(self) -> bool:
+        """Check if the field should be marked as a required parameter."""
+        if Required in self.type_wrappers:  # type: ignore[comparison-overlap]
+            return True
+
+        if NotRequired in self.type_wrappers or UnsetType in self.args:  # type: ignore[comparison-overlap]
+            return False
+
+        if isinstance(self.kwarg_definition, ParameterKwarg) and self.kwarg_definition.required is not None:
+            return self.kwarg_definition.required
+
+        return not self.is_optional and not self.is_any and (not self.has_default or self.default is None)
+
+    @property
+    def is_annotated(self) -> bool:
+        """Check if the field type is Annotated."""
+        return Annotated in self.type_wrappers  # type: ignore[comparison-overlap]
+
+    @property
+    def is_literal(self) -> bool:
+        """Check if the field type is Literal."""
+        return get_origin(self.annotation) is Literal
+
+    @property
+    def is_forward_ref(self) -> bool:
+        """Whether the annotation is a forward reference or not."""
+        return isinstance(self.annotation, (str, ForwardRef))
+
+    @property
+    def is_mapping(self) -> bool:
+        """Whether the annotation is a mapping or not."""
+        return self.is_subclass_of(Mapping)
+
+    @property
+    def is_tuple(self) -> bool:
+        """Whether the annotation is a ``tuple`` or not."""
+        return self.is_subclass_of(tuple)
+
+    @property
+    def is_type_var(self) -> bool:
+        """Whether the annotation is a TypeVar or not."""
+        return isinstance(self.annotation, TypeVar)
+
+    @property
+    def is_union(self) -> bool:
+        """Whether the annotation is a union type or not."""
+        return self.origin in UnionTypes
+
+    @property
+    def is_optional(self) -> bool:
+        """Whether the annotation is Optional or not."""
+        return bool(self.is_union and NoneType in self.args)
+
+    @property
+    def is_collection(self) -> bool:
+        """Whether the annotation is a collection type or not."""
+        return self.is_subclass_of(Collection)
+
+    @property
+    def is_non_string_collection(self) -> bool:
+        """Whether the annotation is a non-string collection type or not."""
+        return self.is_collection and not self.is_subclass_of((str, bytes))
+
+    @property
+    def bound_types(self) -> tuple[FieldDefinition, ...] | None:
+        """A tuple of bound types - if the annotation is a TypeVar with bound types, otherwise None."""
+        if self.is_type_var and (bound := getattr(self.annotation, "__bound__", None)):
+            if is_non_string_sequence(bound):
+                return tuple(FieldDefinition.from_annotation(t) for t in bound)
+            return (FieldDefinition.from_annotation(bound),)
+        return None
+
+    @property
+    def generic_types(self) -> tuple[FieldDefinition, ...] | None:
+        """A tuple of generic types passed into the annotation - if its generic."""
+        if not (bases := getattr(self.annotation, "__orig_bases__", None)):
+            return None
+        args: list[FieldDefinition] = []
+        for base_args in [getattr(base, "__args__", ()) for base in bases]:
+            for arg in base_args:
+                field_definition = FieldDefinition.from_annotation(arg)
+                if field_definition.generic_types:
+                    args.extend(field_definition.generic_types)
+                else:
+                    args.append(field_definition)
+        return tuple(args)
 
-    def populate_data_from_builtins(self, builtins: Any, connection_context: ConnectionContext) -> Any:
-        """Populate model instance from builtin types.
+    def is_subclass_of(self, cl: type[Any] | tuple[type[Any], ...]) -> bool:
+        """Whether the annotation is a subclass of the given type.
+
+        Where ``self.annotation`` is a union type, this method will return ``True`` when all members of the union are
+        a subtype of ``cl``, otherwise, ``False``.
 
         Args:
-            builtins: Builtin type.
-            connection_context: Information about the active connection.
+            cl: The type to check, or tuple of types. Passed as 2nd argument to ``issubclass()``.
 
         Returns:
-            Instance or collection of ``model_type`` instances.
+            Whether the annotation is a subtype of the given type(s).
         """
-        if self.dto_data_type:
-            return self.dto_data_type(
-                backend=self,
-                data_as_builtins=transfer_data(
-                    destination_type=dict,
-                    source_data=self.parse_builtins(builtins, connection_context),
-                    field_definitions=self.parsed_field_definitions,
-                    dto_for="data",
-                    field_definition=self.context.field_definition,
-                ),
-            )
-        return self.transfer_data_from_builtins(self.parse_builtins(builtins, connection_context))
+        if self.origin:
+            if self.origin in UnionTypes:
+                return all(t.is_subclass_of(cl) for t in self.inner_types)
 
-    def transfer_data_from_builtins(self, builtins: Any) -> Any:
-        """Populate model instance from builtin types.
+            return self.origin not in UnionTypes and is_class_and_subclass(self.origin, cl)
 
-        Args:
-            builtins: Builtin type.
+        if self.annotation is AnyStr:
+            return is_class_and_subclass(str, cl) or is_class_and_subclass(bytes, cl)
 
-        Returns:
-            Instance or collection of ``model_type`` instances.
-        """
-        return transfer_data(
-            self.context.model_type, builtins, self.parsed_field_definitions, "data", self.context.field_definition
-        )
+        return self.annotation is not Any and not self.is_type_var and is_class_and_subclass(self.annotation, cl)
 
-    def populate_data_from_raw(self, raw: bytes, connection_context: ConnectionContext) -> Any:
-        """Parse raw bytes into instance of `model_type`.
+    def has_inner_subclass_of(self, cl: type[Any] | tuple[type[Any], ...]) -> bool:
+        """Whether any generic args are a subclass of the given type.
 
         Args:
-            raw: bytes
-            connection_context: Information about the active connection.
+            cl: The type to check, or tuple of types. Passed as 2nd argument to ``issubclass()``.
 
         Returns:
-            Instance or collection of ``model_type`` instances.
+            Whether any of the type's generic args are a subclass of the given type.
         """
-        if self.dto_data_type:
-            return self.dto_data_type(
-                backend=self,
-                data_as_builtins=transfer_data(
-                    dict,
-                    self.parse_raw(raw, connection_context),
-                    self.parsed_field_definitions,
-                    "data",
-                    self.context.field_definition,
-                ),
-            )
-        return transfer_data(
-            self.context.model_type,
-            self.parse_raw(raw, connection_context),
-            self.parsed_field_definitions,
-            "data",
-            self.context.field_definition,
-        )
+        return any(t.is_subclass_of(cl) for t in self.inner_types)
 
-    def encode_data(self, data: Any, connection_context: ConnectionContext) -> LitestarEncodableType:
-        """Encode data into a ``LitestarEncodableType``.
+    @classmethod
+    def from_annotation(cls, annotation: Any, **kwargs: Any) -> FieldDefinition:
+        """Initialize FieldDefinition.
 
         Args:
-            data: Data to encode.
-            connection_context: Information about the active connection.
+            annotation: The type annotation. This should be extracted from the return of
+                ``get_type_hints(..., include_extras=True)`` so that forward references are resolved and recursive
+                ``Annotated`` types are flattened.
+            **kwargs: Additional keyword arguments to pass to the ``FieldDefinition`` constructor.
 
         Returns:
-            Encoded data.
+            FieldDefinition
         """
-        if self.context.wrapper_attribute_name:
-            setattr(
-                data,
-                self.context.wrapper_attribute_name,
-                transfer_data(
-                    destination_type=self.transfer_model_type,
-                    source_data=getattr(data, self.context.wrapper_attribute_name),
-                    field_definitions=self.parsed_field_definitions,
-                    dto_for="return",
-                    field_definition=self.context.field_definition,
-                ),
-            )
-            # cast() here because we take for granted that whatever ``data`` is, it must be something
-            # that litestar can natively encode.
-            return cast("LitestarEncodableType", data)
-
-        return transfer_data(
-            destination_type=self.transfer_model_type,
-            source_data=data,
-            field_definitions=self.parsed_field_definitions,
-            dto_for="return",
-            field_definition=self.context.field_definition,
-        )
 
-    def create_openapi_schema(self, schema_creator: SchemaCreator) -> Reference | Schema:
-        """Create an openAPI schema for the given DTO."""
-        return schema_creator.for_field_definition(
-            FieldDefinition.from_annotation(self.annotation), dto_for=self.context.dto_for
-        )
+        unwrapped, metadata, wrappers = unwrap_annotation(annotation if annotation is not Empty else Any)
+        origin = get_origin(unwrapped)
 
-    def _create_transfer_type(
-        self,
-        field_definition: FieldDefinition,
-        exclude: AbstractSet[str],
-        include: AbstractSet[str],
-        field_name: str,
-        unique_name: str,
-        nested_depth: int,
-    ) -> CompositeType | SimpleType:
-        exclude = _filter_nested_field(exclude, field_name)
-        include = _filter_nested_field(include, field_name)
-
-        if field_definition.is_union:
-            return self._create_union_type(
-                field_definition=field_definition,
-                exclude=exclude,
-                include=include,
-                unique_name=unique_name,
-                nested_depth=nested_depth,
-            )
+        args = () if origin is abc.Callable else get_args(unwrapped)
 
-        if field_definition.is_tuple:
-            if len(field_definition.inner_types) == 2 and field_definition.inner_types[1].annotation is Ellipsis:
-                return self._create_collection_type(
-                    field_definition=field_definition,
-                    exclude=exclude,
-                    include=include,
-                    unique_name=unique_name,
-                    nested_depth=nested_depth,
+        if not kwargs.get("kwarg_definition"):
+            if isinstance(kwargs.get("default"), (KwargDefinition, DependencyKwarg)):
+                kwargs["kwarg_definition"] = kwargs.pop("default")
+            elif any(isinstance(v, (KwargDefinition, DependencyKwarg)) for v in metadata):
+                kwargs["kwarg_definition"] = next(
+                    v for v in metadata if isinstance(v, (KwargDefinition, DependencyKwarg))
+                )
+                metadata = tuple(v for v in metadata if not isinstance(v, (KwargDefinition, DependencyKwarg)))
+            elif (extra := kwargs.get("extra", {})) and "kwarg_definition" in extra:
+                kwargs["kwarg_definition"] = extra.pop("kwarg_definition")
+            else:
+                kwargs["kwarg_definition"], kwargs["extra"] = cls._extract_metadata(
+                    annotation=annotation,
+                    name=kwargs.get("name", ""),
+                    default=kwargs.get("default", Empty),
+                    metadata=metadata,
+                    extra=kwargs.get("extra", {}),
                 )
-            return self._create_tuple_type(
-                field_definition=field_definition,
-                exclude=exclude,
-                include=include,
-                unique_name=unique_name,
-                nested_depth=nested_depth,
-            )
 
-        if field_definition.is_mapping:
-            return self._create_mapping_type(
-                field_definition=field_definition,
-                exclude=exclude,
-                include=include,
-                unique_name=unique_name,
-                nested_depth=nested_depth,
-            )
+        kwargs.setdefault("annotation", unwrapped)
+        kwargs.setdefault("args", args)
+        kwargs.setdefault("default", Empty)
+        kwargs.setdefault("extra", {})
+        kwargs.setdefault("inner_types", tuple(FieldDefinition.from_annotation(arg) for arg in args))
+        kwargs.setdefault("instantiable_origin", get_instantiable_origin(origin, unwrapped))
+        kwargs.setdefault("kwarg_definition", None)
+        kwargs.setdefault("metadata", metadata)
+        kwargs.setdefault("name", "")
+        kwargs.setdefault("origin", origin)
+        kwargs.setdefault("raw", annotation)
+        kwargs.setdefault("safe_generic_origin", get_safe_generic_origin(origin, unwrapped))
+        kwargs.setdefault("type_wrappers", wrappers)
+
+        instance = FieldDefinition(**kwargs)
+        if not instance.has_default and instance.kwarg_definition:
+            return replace(instance, default=instance.kwarg_definition.default)
+
+        return instance
+
+    @classmethod
+    def from_kwarg(
+        cls,
+        annotation: Any,
+        name: str,
+        default: Any = Empty,
+        inner_types: tuple[FieldDefinition, ...] | None = None,
+        kwarg_definition: KwargDefinition | DependencyKwarg | None = None,
+        extra: dict[str, Any] | None = None,
+    ) -> FieldDefinition:
+        """Create a new FieldDefinition instance.
 
-        if field_definition.is_non_string_collection:
-            return self._create_collection_type(
-                field_definition=field_definition,
-                exclude=exclude,
-                include=include,
-                unique_name=unique_name,
-                nested_depth=nested_depth,
-            )
-
-        transfer_model: NestedFieldInfo | None = None
-        if self.context.is_nested_field_predicate(field_definition):
-            if nested_depth == self.context.config.max_nested_depth:
-                raise NestedDepthExceededError()
+        Args:
+            annotation: The type of the kwarg.
+            name: Field name.
+            default: A default value.
+            inner_types: A tuple of FieldDefinition instances representing the inner types, if any.
+            kwarg_definition: Kwarg Parameter.
+            extra: A mapping of extra values.
 
-            nested_field_definitions = self.parse_model(
-                model_type=field_definition.annotation, exclude=exclude, include=include, nested_depth=nested_depth + 1
-            )
-            transfer_model = NestedFieldInfo(
-                model=self.create_transfer_model_type(unique_name, nested_field_definitions),
-                field_definitions=nested_field_definitions,
-            )
+        Returns:
+            FieldDefinition instance.
+        """
 
-        return SimpleType(field_definition, nested_field_info=transfer_model)
+        return cls.from_annotation(
+            annotation,
+            name=name,
+            **{
+                k: v
+                for k, v in {
+                    "inner_types": inner_types,
+                    "kwarg_definition": kwarg_definition,
+                    "extra": extra,
+                    "default": default,
+                }.items()
+                if v is not None
+            },
+        )
+
+    @classmethod
+    def from_parameter(cls, parameter: Parameter, fn_type_hints: dict[str, Any]) -> FieldDefinition:
+        """Initialize ParsedSignatureParameter.
 
-    def _create_collection_type(
-        self,
-        field_definition: FieldDefinition,
-        exclude: AbstractSet[str],
-        include: AbstractSet[str],
-        unique_name: str,
-        nested_depth: int,
-    ) -> CollectionType:
-        inner_types = field_definition.inner_types
-        inner_type = self._create_transfer_type(
-            field_definition=inner_types[0] if inner_types else FieldDefinition.from_annotation(Any),
-            exclude=exclude,
-            include=include,
-            field_name="0",
-            unique_name=_enumerate_name(unique_name, 0),
-            nested_depth=nested_depth,
-        )
-        return CollectionType(
-            field_definition=field_definition, inner_type=inner_type, has_nested=_determine_has_nested(inner_type)
-        )
+        Args:
+            parameter: inspect.Parameter
+            fn_type_hints: mapping of names to types. Should be result of ``get_type_hints()``, preferably via the
+                :attr:``get_fn_type_hints() <.utils.signature_parsing.get_fn_type_hints>`` helper.
 
-    def _create_mapping_type(
-        self,
-        field_definition: FieldDefinition,
-        exclude: AbstractSet[str],
-        include: AbstractSet[str],
-        unique_name: str,
-        nested_depth: int,
-    ) -> MappingType:
-        inner_types = field_definition.inner_types
-        key_type = self._create_transfer_type(
-            field_definition=inner_types[0] if inner_types else FieldDefinition.from_annotation(Any),
-            exclude=exclude,
-            include=include,
-            field_name="0",
-            unique_name=_enumerate_name(unique_name, 0),
-            nested_depth=nested_depth,
-        )
-        value_type = self._create_transfer_type(
-            field_definition=inner_types[1] if inner_types else FieldDefinition.from_annotation(Any),
-            exclude=exclude,
-            include=include,
-            field_name="1",
-            unique_name=_enumerate_name(unique_name, 1),
-            nested_depth=nested_depth,
-        )
-        return MappingType(
-            field_definition=field_definition,
-            key_type=key_type,
-            value_type=value_type,
-            has_nested=_determine_has_nested(key_type) or _determine_has_nested(value_type),
-        )
+        Returns:
+            ParsedSignatureParameter.
 
-    def _create_tuple_type(
-        self,
-        field_definition: FieldDefinition,
-        exclude: AbstractSet[str],
-        include: AbstractSet[str],
-        unique_name: str,
-        nested_depth: int,
-    ) -> TupleType:
-        inner_types = tuple(
-            self._create_transfer_type(
-                field_definition=inner_type,
-                exclude=exclude,
-                include=include,
-                field_name=str(i),
-                unique_name=_enumerate_name(unique_name, i),
-                nested_depth=nested_depth,
-            )
-            for i, inner_type in enumerate(field_definition.inner_types)
-        )
-        return TupleType(
-            field_definition=field_definition,
-            inner_types=inner_types,
-            has_nested=any(_determine_has_nested(t) for t in inner_types),
-        )
+        """
+        from litestar.datastructures import ImmutableState
 
-    def _create_union_type(
-        self,
-        field_definition: FieldDefinition,
-        exclude: AbstractSet[str],
-        include: AbstractSet[str],
-        unique_name: str,
-        nested_depth: int,
-    ) -> UnionType:
-        inner_types = tuple(
-            self._create_transfer_type(
-                field_definition=inner_type,
-                exclude=exclude,
-                include=include,
-                field_name=str(i),
-                unique_name=_enumerate_name(unique_name, i),
-                nested_depth=nested_depth,
-            )
-            for i, inner_type in enumerate(field_definition.inner_types)
-        )
-        return UnionType(
-            field_definition=field_definition,
-            inner_types=inner_types,
-            has_nested=any(_determine_has_nested(t) for t in inner_types),
+        try:
+            annotation = fn_type_hints[parameter.name]
+        except KeyError as e:
+            raise ImproperlyConfiguredException(
+                f"'{parameter.name}' does not have a type annotation. If it should receive any value, use 'Any'."
+            ) from e
+
+        if parameter.name == "state" and not issubclass(annotation, ImmutableState):
+            raise ImproperlyConfiguredException(
+                f"The type annotation `{annotation}` is an invalid type for the 'state' reserved kwarg. "
+                "It must be typed to a subclass of `litestar.datastructures.ImmutableState` or "
+                "`litestar.datastructures.State`."
+            )
+
+        return FieldDefinition.from_kwarg(
+            annotation=annotation,
+            name=parameter.name,
+            default=Empty if parameter.default is Signature.empty else parameter.default,
         )
 
-    @staticmethod
-    def _gen_unique_name_id(unique_name: str) -> str:
-        # Generate a unique ID
-        # Convert the ID to a short alphanumeric string
-        return f"{unique_name}-{secrets.token_hex(8)}"
-
-
-def _filter_nested_field(field_name_set: AbstractSet[str], field_name: str) -> AbstractSet[str]:
-    """Filter a nested field name."""
-    return {split[1] for s in field_name_set if (split := s.split(".", 1))[0] == field_name and len(split) > 1}
-
-
-def _enumerate_name(name: str, index: int) -> str:
-    """Enumerate ``name`` with ``index``."""
-    return f"{name}_{index}"
+    def match_predicate_recursively(self, predicate: Callable[[FieldDefinition], bool]) -> bool:
+        """Recursively test the passed in predicate against the field and any of its inner fields.
 
+        Args:
+            predicate: A callable that receives a field definition instance as an arg and returns a boolean.
 
-def _determine_has_nested(transfer_type: SimpleType | CompositeType) -> bool:
-    """Determine if a transfer type has nested types."""
-    if isinstance(transfer_type, SimpleType):
-        return bool(transfer_type.nested_field_info)
-    return transfer_type.has_nested
+        Returns:
+            A boolean.
+        """
+        return predicate(self) or any(t.match_predicate_recursively(predicate) for t in self.inner_types)
```

### Comparing `litestar-2.0.0b4/litestar/dto/_types.py` & `litestar-2.0.0rc1/litestar/dto/_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 from typing import TYPE_CHECKING
 
 from litestar.dto.data_structures import DTOFieldDefinition
 
 if TYPE_CHECKING:
     from typing import Any
 
-    from typing_extensions import Self, TypeAlias
+    from typing_extensions import Self
 
     from litestar.typing import FieldDefinition
 
 
 @dataclass(frozen=True)
 class NestedFieldInfo:
     """Type for representing fields and model type of nested model type."""
 
     __slots__ = ("model", "field_definitions")
 
     model: type[Any]
-    field_definitions: FieldDefinitionsType
+    field_definitions: tuple[TransferDTOFieldDefinition, ...]
 
 
 @dataclass(frozen=True)
 class TransferType:
     """Type for representing model types for data transfer."""
 
     __slots__ = ("field_definition",)
@@ -37,14 +37,18 @@
     """Represents indivisible, non-composite types."""
 
     __slots__ = ("nested_field_info",)
 
     nested_field_info: NestedFieldInfo | None
     """If the type is a 'nested' type, this is the model generated for transfer to/from it."""
 
+    @property
+    def has_nested(self) -> bool:
+        return self.nested_field_info is not None
+
 
 @dataclass(frozen=True)
 class CompositeType(TransferType):
     """A type that is made up of other types."""
 
     __slots__ = ("has_nested",)
 
@@ -90,16 +94,15 @@
 
 
 @dataclass(frozen=True)
 class TransferDTOFieldDefinition(DTOFieldDefinition):
     __slots__ = (
         "default_factory",
         "dto_field",
-        "dto_for",
-        "unique_model_name",
+        "model_name",
         "is_excluded",
         "is_partial",
         "serialization_name",
         "transfer_type",
         "unique_name",
     )
 
@@ -123,28 +126,23 @@
     ) -> Self:
         return cls(
             annotation=field_definition.annotation,
             args=field_definition.args,
             default=field_definition.default,
             default_factory=field_definition.default_factory,
             dto_field=field_definition.dto_field,
-            dto_for=field_definition.dto_for,
             extra=field_definition.extra,
             inner_types=field_definition.inner_types,
             instantiable_origin=field_definition.instantiable_origin,
             is_excluded=is_excluded,
             is_partial=is_partial,
             kwarg_definition=field_definition.kwarg_definition,
             metadata=field_definition.metadata,
             name=field_definition.name,
             origin=field_definition.origin,
             raw=field_definition.raw,
             safe_generic_origin=field_definition.safe_generic_origin,
             serialization_name=serialization_name,
             transfer_type=transfer_type,
             type_wrappers=field_definition.type_wrappers,
-            unique_model_name=field_definition.unique_model_name,
+            model_name=field_definition.model_name,
         )
-
-
-FieldDefinitionsType: TypeAlias = "tuple[TransferDTOFieldDefinition, ...]"
-"""Generic representation of names and types."""
```

### Comparing `litestar-2.0.0b4/litestar/dto/config.py` & `litestar-2.0.0rc1/litestar/dto/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/dto/data_structures.py` & `litestar-2.0.0rc1/litestar/dto/data_structures.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from litestar.typing import FieldDefinition
 
 if TYPE_CHECKING:
     from typing import Any, Callable
 
     from litestar.dto import DTOField
     from litestar.dto._backend import DTOBackend
-    from litestar.dto.types import ForType
 
 T = TypeVar("T")
 
 
 class DTOData(Generic[T]):
     """DTO validated data and utility methods."""
 
@@ -64,74 +63,54 @@
 @dataclass(frozen=True)
 class DTOFieldDefinition(FieldDefinition):
     """A model field representation for purposes of generating a DTO backend model type."""
 
     __slots__ = (
         "default_factory",
         "dto_field",
-        "dto_for",
-        "unique_model_name",
+        "model_name",
     )
 
-    unique_model_name: str
-    """Unique identifier of model that owns the field."""
+    model_name: str
+    """The name of the model for which the field is generated."""
     default_factory: Callable[[], Any] | None
     """Default factory of the field."""
     dto_field: DTOField
     """DTO field configuration."""
-    dto_for: ForType | None
-    """Direction of transfer for field.
-
-    Specify if the field definition should only be added to models for only the request (``"data"``) or response
-    (``"return"``). If there should be no such distinction, set to ``None``.
-
-    This is to support special cases where the type to set an attribute may be different to the type received when
-    retrieving its value. For example, a :class:`sqlalchemy.ext.hybrid.hybrid_property` may be set with a ``str`` but
-    retrieved as some other type.
-
-    The difference between this, and marking a field as read-only or private, is that it cannot be overridden by the end
-    user.
-    """
-
-    def unique_name(self) -> str:
-        return f"{self.unique_model_name}.{self.name}"
 
     @classmethod
     def from_field_definition(
         cls,
         field_definition: FieldDefinition,
-        unique_model_name: str,
+        model_name: str,
         default_factory: Callable[[], Any] | None,
         dto_field: DTOField,
-        dto_for: ForType | None,
     ) -> DTOFieldDefinition:
         """Create a :class:`FieldDefinition` from a :class:`FieldDefinition`.
 
         Args:
             field_definition: A :class:`FieldDefinition` to create a :class:`FieldDefinition` from.
-            unique_model_name: The unique name of the model.
+            model_name: The name of the model.
             default_factory: Default factory function, if any.
             dto_field: DTOField instance.
-            dto_for: DTO type.
 
         Returns:
             A :class:`FieldDefinition` instance.
         """
         return DTOFieldDefinition(
             annotation=field_definition.annotation,
             args=field_definition.args,
             default=field_definition.default,
+            default_factory=default_factory,
+            dto_field=dto_field,
             extra=field_definition.extra,
             inner_types=field_definition.inner_types,
             instantiable_origin=field_definition.instantiable_origin,
             kwarg_definition=field_definition.kwarg_definition,
             metadata=field_definition.metadata,
+            model_name=model_name,
             name=field_definition.name,
             origin=field_definition.origin,
             raw=field_definition.raw,
             safe_generic_origin=field_definition.safe_generic_origin,
             type_wrappers=field_definition.type_wrappers,
-            unique_model_name=unique_model_name,
-            default_factory=default_factory,
-            dto_field=dto_field,
-            dto_for=dto_for,
         )
```

### Comparing `litestar-2.0.0b4/litestar/dto/dataclass_dto_factory.py` & `litestar-2.0.0rc1/litestar/dto/dataclass_dto.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,51 @@
 from __future__ import annotations
 
 from dataclasses import MISSING, fields, replace
 from typing import TYPE_CHECKING, Generic, TypeVar
 
-from litestar.dto._utils import get_model_type_hints
-from litestar.dto.base_factory import AbstractDTOFactory
+from litestar.dto.base_dto import AbstractDTO
 from litestar.dto.data_structures import DTOFieldDefinition
 from litestar.dto.field import DTO_FIELD_META_KEY, DTOField
 from litestar.params import DependencyKwarg, KwargDefinition
 from litestar.types.empty import Empty
-from litestar.utils.helpers import get_fully_qualified_class_name
 
 if TYPE_CHECKING:
-    from typing import ClassVar, Collection, Generator
+    from typing import Collection, Generator
 
     from litestar.types.protocols import DataclassProtocol
     from litestar.typing import FieldDefinition
 
 
 __all__ = ("DataclassDTO", "T")
 
 T = TypeVar("T", bound="DataclassProtocol | Collection[DataclassProtocol]")
 AnyDataclass = TypeVar("AnyDataclass", bound="DataclassProtocol")
 
 
-class DataclassDTO(AbstractDTOFactory[T], Generic[T]):
+class DataclassDTO(AbstractDTO[T], Generic[T]):
     """Support for domain modelling with dataclasses."""
 
-    __slots__ = ()
-
-    model_type: ClassVar[type[DataclassProtocol]]
-
     @classmethod
     def generate_field_definitions(
         cls, model_type: type[DataclassProtocol]
     ) -> Generator[DTOFieldDefinition, None, None]:
         dc_fields = {f.name: f for f in fields(model_type)}
-        for key, field_definition in get_model_type_hints(model_type).items():
+        for key, field_definition in cls.get_model_type_hints(model_type).items():
             if not (dc_field := dc_fields.get(key)):
                 continue
 
             default = dc_field.default if dc_field.default is not MISSING else Empty
             default_factory = dc_field.default_factory if dc_field.default_factory is not MISSING else None
             field_defintion = replace(
                 DTOFieldDefinition.from_field_definition(
                     field_definition=field_definition,
                     default_factory=default_factory,
                     dto_field=dc_field.metadata.get(DTO_FIELD_META_KEY, DTOField()),
-                    unique_model_name=get_fully_qualified_class_name(model_type),
-                    dto_for=None,
+                    model_name=model_type.__name__,
                 ),
                 name=key,
                 default=default,
             )
 
             yield replace(field_defintion, default=Empty, kwarg_definition=default) if isinstance(
                 default, (KwargDefinition, DependencyKwarg)
```

### Comparing `litestar-2.0.0b4/litestar/dto/field.py` & `litestar-2.0.0rc1/litestar/dto/field.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/dto/msgspec_dto_factory.py` & `litestar-2.0.0rc1/litestar/dto/msgspec_dto.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,50 @@
 from __future__ import annotations
 
 from dataclasses import replace
 from typing import TYPE_CHECKING, Collection, Generic, TypeVar, cast
 
 from msgspec import NODEFAULT, Struct, inspect
 
-from litestar.dto._utils import get_model_type_hints
-from litestar.dto.base_factory import AbstractDTOFactory
+from litestar.dto.base_dto import AbstractDTO
 from litestar.dto.data_structures import DTOFieldDefinition
 from litestar.dto.field import DTO_FIELD_META_KEY, DTOField
 from litestar.types.empty import Empty
-from litestar.utils.helpers import get_fully_qualified_class_name
 
 if TYPE_CHECKING:
-    from typing import Any, ClassVar, Generator
+    from typing import Any, Generator
 
     from litestar.typing import FieldDefinition
 
 
 __all__ = ("MsgspecDTO",)
 
 T = TypeVar("T", bound="Struct | Collection[Struct]")
 
 
-class MsgspecDTO(AbstractDTOFactory[T], Generic[T]):
+class MsgspecDTO(AbstractDTO[T], Generic[T]):
     """Support for domain modelling with Msgspec."""
 
-    __slots__ = ()
-
-    model_type: ClassVar[type[Struct]]
-
     @classmethod
     def generate_field_definitions(cls, model_type: type[Struct]) -> Generator[DTOFieldDefinition, None, None]:
         msgspec_fields = {f.name: f for f in cast("inspect.StructType", inspect.type_info(model_type)).fields}
 
         def default_or_empty(value: Any) -> Any:
             return Empty if value is NODEFAULT else value
 
-        for key, field_definition in get_model_type_hints(model_type).items():
+        for key, field_definition in cls.get_model_type_hints(model_type).items():
             msgspec_field = msgspec_fields[key]
             dto_field = (field_definition.extra or {}).pop(DTO_FIELD_META_KEY, DTOField())
 
             yield replace(
                 DTOFieldDefinition.from_field_definition(
                     field_definition=field_definition,
                     dto_field=dto_field,
-                    unique_model_name=get_fully_qualified_class_name(model_type),
+                    model_name=model_type.__name__,
                     default_factory=default_or_empty(msgspec_field.default_factory),
-                    dto_for=None,
                 ),
                 default=default_or_empty(msgspec_field.default),
                 name=key,
             )
 
     @classmethod
     def detect_nested_field(cls, field_definition: FieldDefinition) -> bool:
```

### Comparing `litestar-2.0.0b4/litestar/enums.py` & `litestar-2.0.0rc1/litestar/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/events/emitter.py` & `litestar-2.0.0rc1/litestar/events/emitter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import math
 import sys
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from contextlib import AsyncExitStack
+from functools import partial
 from typing import TYPE_CHECKING, Any, Sequence
 
 if sys.version_info < (3, 9):
     from typing import AsyncContextManager
 else:
     from contextlib import AbstractAsyncContextManager as AsyncContextManager
 
@@ -74,23 +75,25 @@
         super().__init__(listeners=listeners)
         self._receive_stream: MemoryObjectReceiveStream | None = None
         self._send_stream: MemoryObjectSendStream | None = None
         self._exit_stack: AsyncExitStack | None = None
 
     @staticmethod
     async def _worker(receive_stream: MemoryObjectReceiveStream) -> None:
-        """Worker that runs in a separate task and continuously pulls events from asyncio queue.
+        """Run items from ``receive_stream`` in a task group.
 
         Returns:
             None
         """
-        async with receive_stream:
+        async with receive_stream, anyio.create_task_group() as task_group:
             async for item in receive_stream:
                 fn, args, kwargs = item
-                await fn(*args, **kwargs)
+                if kwargs:
+                    fn = partial(fn, **kwargs)
+                task_group.start_soon(fn, *args)
 
     async def __aenter__(self) -> SimpleEventEmitter:
         self._exit_stack = AsyncExitStack()
         send_stream, receive_stream = anyio.create_memory_object_stream(math.inf)
         self._send_stream = send_stream
         task_group = anyio.create_task_group()
```

### Comparing `litestar-2.0.0b4/litestar/events/listener.py` & `litestar-2.0.0rc1/litestar/events/listener.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/exceptions/__init__.py` & `litestar-2.0.0rc1/litestar/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/exceptions/base_exceptions.py` & `litestar-2.0.0rc1/litestar/exceptions/base_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/exceptions/http_exceptions.py` & `litestar-2.0.0rc1/litestar/exceptions/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/exceptions/websocket_exceptions.py` & `litestar-2.0.0rc1/litestar/exceptions/websocket_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/file_system.py` & `litestar-2.0.0rc1/litestar/file_system.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/handlers/__init__.py` & `litestar-2.0.0rc1/litestar/handlers/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 from .asgi_handlers import ASGIRouteHandler, asgi
 from .base import BaseRouteHandler
 from .http_handlers import HTTPRouteHandler, delete, get, head, patch, post, put, route
-from .websocket_handlers import WebsocketListener, WebsocketRouteHandler, websocket, websocket_listener
+from .websocket_handlers import (
+    WebsocketListener,
+    WebsocketListenerRouteHandler,
+    WebsocketRouteHandler,
+    websocket,
+    websocket_listener,
+)
 
 __all__ = (
     "ASGIRouteHandler",
     "BaseRouteHandler",
     "HTTPRouteHandler",
     "WebsocketListener",
     "WebsocketRouteHandler",
+    "WebsocketListenerRouteHandler",
     "asgi",
     "delete",
     "get",
     "head",
     "patch",
     "post",
     "put",
```

### Comparing `litestar-2.0.0b4/litestar/handlers/asgi_handlers.py` & `litestar-2.0.0rc1/litestar/handlers/asgi_handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/handlers/base.py` & `litestar-2.0.0rc1/litestar/handlers/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,42 +2,39 @@
 
 from copy import copy
 from functools import partial
 from typing import TYPE_CHECKING, Any, Callable, Mapping, Sequence, cast
 
 from litestar._signature import SignatureModel
 from litestar.di import Provide
-from litestar.dto.interface import HandlerContext
 from litestar.exceptions import ImproperlyConfiguredException
-from litestar.serialization import default_deserializer
+from litestar.serialization import default_deserializer, default_serializer
 from litestar.types import (
     Dependencies,
     Empty,
     ExceptionHandlersMap,
     Guard,
     MaybePartial,
     Middleware,
     TypeDecodersSequence,
     TypeEncodersMap,
 )
 from litestar.typing import FieldDefinition
-from litestar.utils import AsyncCallable, Ref, async_partial, get_name, normalize_path
+from litestar.utils import AsyncCallable, Ref, get_name, normalize_path
 from litestar.utils.helpers import unwrap_partial
-from litestar.utils.predicates import is_async_callable
-from litestar.utils.signature import ParsedSignature, infer_request_encoding_from_field_definition
+from litestar.utils.signature import ParsedSignature
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
-    from litestar import Litestar
+    from litestar.app import Litestar
     from litestar.connection import ASGIConnection
     from litestar.controller import Controller
-    from litestar.dto.interface import DTOInterface
+    from litestar.dto import AbstractDTO
     from litestar.params import ParameterKwarg
-    from litestar.plugins import SerializationPluginProtocol
     from litestar.router import Router
     from litestar.types import AnyCallable, AsyncAnyCallable, ExceptionHandler
     from litestar.types.empty import EmptyType
 
 __all__ = ("BaseRouteHandler",)
 
 
@@ -45,136 +42,174 @@
     """Base route handler.
 
     Serves as a subclass for all route handlers
     """
 
     __slots__ = (
         "_fn",
+        "_parsed_data_field",
         "_parsed_fn_signature",
+        "_parsed_return_field",
+        "_resolved_data_dto",
         "_resolved_dependencies",
-        "_resolved_dto",
         "_resolved_guards",
         "_resolved_layered_parameters",
         "_resolved_return_dto",
         "_resolved_signature_namespace",
         "_resolved_type_decoders",
         "_resolved_type_encoders",
+        "_signature_model",
         "dependencies",
         "dto",
         "exception_handlers",
         "guards",
         "middleware",
         "name",
         "opt",
         "owner",
         "paths",
         "return_dto",
-        "signature_model",
         "signature_namespace",
         "type_decoders",
         "type_encoders",
     )
 
     def __init__(
         self,
         path: str | Sequence[str] | None = None,
         *,
         dependencies: Dependencies | None = None,
-        dto: type[DTOInterface] | None | EmptyType = Empty,
+        dto: type[AbstractDTO] | None | EmptyType = Empty,
         exception_handlers: ExceptionHandlersMap | None = None,
         guards: Sequence[Guard] | None = None,
         middleware: Sequence[Middleware] | None = None,
         name: str | None = None,
         opt: Mapping[str, Any] | None = None,
-        return_dto: type[DTOInterface] | None | EmptyType = Empty,
+        return_dto: type[AbstractDTO] | None | EmptyType = Empty,
         signature_namespace: Mapping[str, Any] | None = None,
         type_encoders: TypeEncodersMap | None = None,
         type_decoders: TypeDecodersSequence | None = None,
         **kwargs: Any,
     ) -> None:
         """Initialize ``HTTPRouteHandler``.
 
         Args:
             path: A path fragment for the route handler function or a sequence of path fragments. If not given defaults
                 to ``/``
             dependencies: A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances.
-            dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for (de)serializing and
+            dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for (de)serializing and
                 validation of request data.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
             guards: A sequence of :class:`Guard <.types.Guard>` callables.
             middleware: A sequence of :class:`Middleware <.types.Middleware>`.
             name: A string identifying the route handler.
             opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
                 wherever you have access to :class:`Request <.connection.Request>` or
                 :class:`ASGI Scope <.types.Scope>`.
-            return_dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for serializing
+            return_dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for serializing
                 outbound response data.
             signature_namespace: A mapping of names to types for use in forward reference resolution during signature
                 modelling.
             type_encoders: A mapping of types to callables that transform them into types supported for serialization.
             type_decoders: A sequence of tuples, each composed of a predicate testing for type identity and a msgspec hook for deserialization.
             **kwargs: Any additional kwarg - will be set in the opt dictionary.
         """
         self._parsed_fn_signature: ParsedSignature | EmptyType = Empty
+        self._parsed_return_field: FieldDefinition | EmptyType = Empty
+        self._parsed_data_field: FieldDefinition | None | EmptyType = Empty
+        self._resolved_data_dto: type[AbstractDTO] | None | EmptyType = Empty
         self._resolved_dependencies: dict[str, Provide] | EmptyType = Empty
-        self._resolved_dto: type[DTOInterface] | None | EmptyType = Empty
         self._resolved_guards: list[Guard] | EmptyType = Empty
         self._resolved_layered_parameters: dict[str, FieldDefinition] | EmptyType = Empty
-        self._resolved_return_dto: type[DTOInterface] | None | EmptyType = Empty
+        self._resolved_return_dto: type[AbstractDTO] | None | EmptyType = Empty
         self._resolved_signature_namespace: dict[str, Any] | EmptyType = Empty
-        self._resolved_type_encoders: TypeEncodersMap | EmptyType = Empty
         self._resolved_type_decoders: TypeDecodersSequence | EmptyType = Empty
+        self._resolved_type_encoders: TypeEncodersMap | EmptyType = Empty
+        self._signature_model: type[SignatureModel] | EmptyType = Empty
 
         self.dependencies = dependencies
         self.dto = dto
         self.exception_handlers = exception_handlers
         self.guards = guards
         self.middleware = middleware
         self.name = name
         self.opt = dict(opt or {})
+        self.opt.update(**kwargs)
         self.owner: Controller | Router | None = None
         self.return_dto = return_dto
-        self.signature_model: type[SignatureModel] | None = None
         self.signature_namespace = signature_namespace or {}
+        self.type_decoders = type_decoders
+        self.type_encoders = type_encoders
+
         self.paths = (
             {normalize_path(p) for p in path}
             if path and isinstance(path, list)
             else {normalize_path(path or "/")}  # type: ignore
         )
-        self.opt.update(**kwargs)
-        self.type_encoders = type_encoders
-        self.type_decoders = type_decoders
 
     def __call__(self, fn: AsyncAnyCallable) -> Self:
         """Replace a function with itself."""
         self._fn = Ref["MaybePartial[AsyncAnyCallable]"](fn)
         return self
 
     @property
+    def handler_id(self) -> str:
+        """A unique identifier used for generation of DTOs."""
+        return f"{self!s}::{sum(id(layer) for layer in self.ownership_layers)}"
+
+    @property
     def default_deserializer(self) -> Callable[[Any, Any], Any]:
+        """Get a default deserializer for the route handler.
+
+        Returns:
+            A default deserializer for the route handler.
+
+        """
+        return partial(default_deserializer, type_decoders=self.resolve_type_decoders())
+
+    @property
+    def default_serializer(self) -> Callable[[Any], Any]:
         """Get a default serializer for the route handler.
 
         Returns:
             A default serializer for the route handler.
 
         """
-        return partial(default_deserializer, type_decoders=self.resolve_type_decoders())
+        return partial(default_serializer, type_encoders=self.resolve_type_encoders())
+
+    @property
+    def signature_model(self) -> type[SignatureModel]:
+        """Get the signature model for the route handler.
+
+        Returns:
+            A signature model for the route handler.
+
+        """
+        if self._signature_model is Empty:
+            self._signature_model = SignatureModel.create(
+                dependency_name_set=self.dependency_name_set,
+                fn=cast("AnyCallable", self.fn.value),
+                parsed_signature=self.parsed_fn_signature,
+                data_dto=self.resolve_data_dto(),
+                type_decoders=self.resolve_type_decoders(),
+            )
+        return cast("type[SignatureModel]", self._signature_model)
 
     @property
     def fn(self) -> Ref[MaybePartial[AsyncAnyCallable]]:
         """Get the handler function.
 
         Raises:
             ImproperlyConfiguredException: if handler fn is not set.
 
         Returns:
             Handler function
         """
         if not hasattr(self, "_fn"):
-            raise ImproperlyConfiguredException("Handler has not decorated a function")
+            raise ImproperlyConfiguredException("No callable has been registered for this handler")
         return self._fn
 
     @property
     def parsed_fn_signature(self) -> ParsedSignature:
         """Return the parsed signature of the handler function.
 
         This method is memoized so the computation occurs only once.
@@ -186,14 +221,26 @@
             self._parsed_fn_signature = ParsedSignature.from_fn(
                 unwrap_partial(self.fn.value), self.resolve_signature_namespace()
             )
 
         return cast("ParsedSignature", self._parsed_fn_signature)
 
     @property
+    def parsed_return_field(self) -> FieldDefinition:
+        if self._parsed_return_field is Empty:
+            self._parsed_return_field = self.parsed_fn_signature.return_type
+        return cast("FieldDefinition", self._parsed_return_field)
+
+    @property
+    def parsed_data_field(self) -> FieldDefinition | None:
+        if self._parsed_data_field is Empty:
+            self._parsed_data_field = self.parsed_fn_signature.parameters.get("data")
+        return cast("FieldDefinition | None", self._parsed_data_field)
+
+    @property
     def handler_name(self) -> str:
         """Get the name of the handler function.
 
         Raises:
             ImproperlyConfiguredException: if handler fn is not set.
 
         Returns:
@@ -218,14 +265,18 @@
         cur: Any = self
         while cur:
             layers.append(cur)
             cur = cur.owner
 
         return list(reversed(layers))
 
+    @property
+    def app(self) -> Litestar:
+        return cast("Litestar", self.ownership_layers[0])
+
     def resolve_type_encoders(self) -> TypeEncodersMap:
         """Return a merged type_encoders mapping.
 
         This method is memoized so the computation occurs only once.
 
         Returns:
             A dict of type encoders
@@ -283,22 +334,34 @@
 
     def resolve_dependencies(self) -> dict[str, Provide]:
         """Return all dependencies correlating to handler function's kwargs that exist in the handler's scope."""
         if self._resolved_dependencies is Empty:
             self._resolved_dependencies = {}
 
             for layer in self.ownership_layers:
-                for key, value in (layer.dependencies or {}).items():
-                    if not isinstance(value, Provide):
-                        value = Provide(value)
+                for key, provider in (layer.dependencies or {}).items():
+                    if not isinstance(provider, Provide):
+                        provider = Provide(provider)
+
                     self._validate_dependency_is_unique(
-                        dependencies=self._resolved_dependencies, key=key, provider=value
+                        dependencies=self._resolved_dependencies, key=key, provider=provider
                     )
-                    self._resolved_dependencies[key] = value
 
+                    if not getattr(provider, "signature_model", None):
+                        provider.signature_model = SignatureModel.create(
+                            dependency_name_set=self.dependency_name_set,
+                            fn=provider.dependency.value,
+                            parsed_signature=ParsedSignature.from_fn(
+                                unwrap_partial(provider.dependency.value), self.resolve_signature_namespace()
+                            ),
+                            data_dto=self.resolve_data_dto(),
+                            type_decoders=self.resolve_type_decoders(),
+                        )
+
+                    self._resolved_dependencies[key] = provider
         return cast("dict[str, Provide]", self._resolved_dependencies)
 
     def resolve_middleware(self) -> list[Middleware]:
         """Build the middleware stack for the RouteHandler and return it.
 
         The middlewares are added from top to bottom (``app -> router -> controller -> route handler``) and then
         reversed.
@@ -341,84 +404,80 @@
             ns: dict[str, Any] = {}
             for layer in self.ownership_layers:
                 ns.update(layer.signature_namespace)
 
             self._resolved_signature_namespace = ns
         return cast("dict[str, Any]", self._resolved_signature_namespace)
 
-    def resolve_dto(self) -> type[DTOInterface] | None:
+    def resolve_data_dto(self) -> type[AbstractDTO] | None:
         """Resolve the data_dto by starting from the route handler and moving up.
         If a handler is found it is returned, otherwise None is set.
         This method is memoized so the computation occurs only once.
 
         Returns:
-            An optional :class:`DTO type <.dto.interface.DTOInterface>`
+            An optional :class:`DTO type <.dto.base_dto.AbstractDTO>`
         """
-        if self._resolved_dto is Empty:
-            dtos: list[type[DTOInterface] | None] = [
-                layer_dto  # type:ignore[misc]
-                for layer in self.ownership_layers
-                if (layer_dto := layer.dto) is not Empty
-            ]
-            self._resolved_dto = dtos[-1] if dtos else None
+        if self._resolved_data_dto is Empty:
+            if data_dtos := cast(
+                "list[type[AbstractDTO] | None]",
+                [layer.dto for layer in self.ownership_layers if layer.dto is not Empty],
+            ):
+                data_dto: type[AbstractDTO] | None = data_dtos[-1]
+            elif self.parsed_data_field and (
+                plugins_for_data_type := [
+                    plugin
+                    for plugin in self.app.plugins.serialization
+                    if self.parsed_data_field.match_predicate_recursively(plugin.supports_type)
+                ]
+            ):
+                data_dto = plugins_for_data_type[0].create_dto_for_type(self.parsed_data_field)
+            else:
+                data_dto = None
+
+            if self.parsed_data_field and data_dto:
+                data_dto.create_for_field_definition(
+                    field_definition=self.parsed_data_field, handler_id=self.handler_id
+                )
+
+            self._resolved_data_dto = data_dto
 
-        return cast("type[DTOInterface] | None", self._resolved_dto)
+        return cast("type[AbstractDTO] | None", self._resolved_data_dto)
 
-    def resolve_return_dto(self) -> type[DTOInterface] | None:
+    def resolve_return_dto(self) -> type[AbstractDTO] | None:
         """Resolve the return_dto by starting from the route handler and moving up.
         If a handler is found it is returned, otherwise None is set.
         This method is memoized so the computation occurs only once.
 
         Returns:
-            An optional :class:`DTO type <.dto.interface.DTOInterface>`
+            An optional :class:`DTO type <.dto.base_dto.AbstractDTO>`
         """
         if self._resolved_return_dto is Empty:
-            return_dtos: list[type[DTOInterface] | None] = [
-                layer_dto_type  # type:ignore[misc]
-                for layer in self.ownership_layers
-                if (layer_dto_type := layer.return_dto) is not Empty
-            ]
-            self._resolved_return_dto = return_dtos[-1] if return_dtos else self.resolve_dto()
-
-        return cast("type[DTOInterface] | None", self._resolved_return_dto)
-
-    def _set_dto(self, dto: type[DTOInterface]) -> None:
-        """Set the dto for the handler.
-
-        Args:
-            dto: The :class:`DTO type <.dto.interface.DTOInterface>` to set.
-        """
-        self._resolved_dto = dto
-
-    def _set_return_dto(self, dto: type[DTOInterface]) -> None:
-        """Set the return_dto for the handler.
-
-        Args:
-            dto: The :class:`DTO type <.dto.interface.DTOInterface>` to set.
-        """
-        self._resolved_return_dto = dto
-
-    def _init_handler_dtos(self) -> None:
-        """Initialize the data and return DTOs for the handler."""
-        if (dto := self.resolve_dto()) and (data_parameter := self.parsed_fn_signature.parameters.get("data")):
-            dto.on_registration(
-                HandlerContext(
-                    dto_for="data",
-                    handler_id=str(self),
-                    field_definition=data_parameter,
-                    request_encoding_type=infer_request_encoding_from_field_definition(data_parameter),
+            if return_dtos := cast(
+                "list[type[AbstractDTO] | None]",
+                [layer.return_dto for layer in self.ownership_layers if layer.return_dto is not Empty],
+            ):
+                return_dto: type[AbstractDTO] | None = return_dtos[-1]
+            elif plugins_for_return_type := [
+                plugin
+                for plugin in self.app.plugins.serialization
+                if self.parsed_return_field.match_predicate_recursively(plugin.supports_type)
+            ]:
+                return_dto = plugins_for_return_type[0].create_dto_for_type(self.parsed_return_field)
+            else:
+                return_dto = self.resolve_data_dto()
+
+            if return_dto and return_dto.is_supported_model_type_field(self.parsed_return_field):
+                return_dto.create_for_field_definition(
+                    field_definition=self.parsed_return_field, handler_id=self.handler_id
                 )
-            )
+                self._resolved_return_dto = return_dto
+            else:
+                self._resolved_return_dto = None
 
-        if return_dto := self.resolve_return_dto():
-            return_dto.on_registration(
-                HandlerContext(
-                    dto_for="return", handler_id=str(self), field_definition=self.parsed_fn_signature.return_type
-                )
-            )
+        return cast("type[AbstractDTO] | None", self._resolved_return_dto)
 
     async def authorize_connection(self, connection: ASGIConnection) -> None:
         """Ensure the connection is authorized by running all the route guards in scope."""
         for guard in self.resolve_guards():
             await guard(connection, copy(self))  # type: ignore
 
     @staticmethod
@@ -428,85 +487,37 @@
             if provider == value:
                 raise ImproperlyConfiguredException(
                     f"Provider for key {key} is already defined under the different key {dependency_key}. "
                     f"If you wish to override a provider, it must have the same key."
                 )
 
     def on_registration(self, app: Litestar) -> None:
-        """Called once per handler when the app object is instantiated."""
+        """Called once per handler when the app object is instantiated.
+
+        Args:
+            app: The :class:`Litestar<.app.Litestar>` app object.
+
+        Returns:
+            None
+        """
         self._validate_handler_function()
-        self._handle_serialization_plugins(app.serialization_plugins)
-        self._init_handler_dtos()
-        self._set_runtime_callables()
-        self._create_signature_model(app)
-        self._create_provider_signature_models(app)
+        self.resolve_dependencies()
         self.resolve_guards()
         self.resolve_middleware()
         self.resolve_opts()
+        self.resolve_data_dto()
+        self.resolve_return_dto()
 
     def _validate_handler_function(self) -> None:
         """Validate the route handler function once set by inspecting its return annotations."""
 
-    def _set_runtime_callables(self) -> None:
-        """Optimize the ``route_handler.fn`` and any ``provider.dependency`` callables for runtime by doing the following:
-
-        1. ensure that the ``self`` argument is preserved by binding it using partial.
-        2. ensure sync functions are wrapped in AsyncCallable for sync_to_thread handlers.
-        """
-        for provider in self.resolve_dependencies().values():
-            if not is_async_callable(provider.dependency.value):
-                provider.has_sync_callable = False
-                if provider.sync_to_thread:
-                    provider.dependency.value = async_partial(provider.dependency.value)
-                else:
-                    provider.has_sync_callable = True
-
-    def _create_signature_model(self, app: Litestar) -> None:
-        """Create signature model for handler function."""
-        if not self.signature_model:
-            self.signature_model = SignatureModel.create(
-                dependency_name_set=self.dependency_name_set,
-                fn=cast("AnyCallable", self.fn.value),
-                parsed_signature=self.parsed_fn_signature,
-                has_data_dto=bool(self.resolve_dto()),
-            )
-
-    def _create_provider_signature_models(self, app: Litestar) -> None:
-        """Create signature models for dependency providers."""
-        for provider in self.resolve_dependencies().values():
-            if not getattr(provider, "signature_model", None):
-                provider.signature_model = SignatureModel.create(
-                    dependency_name_set=self.dependency_name_set,
-                    fn=provider.dependency.value,
-                    parsed_signature=ParsedSignature.from_fn(
-                        unwrap_partial(provider.dependency.value), self.resolve_signature_namespace()
-                    ),
-                    has_data_dto=bool(self.resolve_dto()),
-                )
-
-    def _handle_serialization_plugins(self, plugins: list[SerializationPluginProtocol]) -> None:
-        """Handle the serialization plugins for the handler."""
-        # must do the return dto first, otherwise it will resolve to the same as the data dto
-        if self.resolve_return_dto() is None:
-            return_type = self.parsed_fn_signature.return_type
-            for plugin in plugins:
-                if plugin.supports_type(return_type):
-                    self._set_return_dto(plugin.create_dto_for_type(return_type))
-                    break
-
-        if (data_param := self.parsed_fn_signature.parameters.get("data")) and self.resolve_dto() is None:
-            for plugin in plugins:
-                if plugin.supports_type(data_param):
-                    self._set_dto(plugin.create_dto_for_type(data_param))
-                    break
-
     def __str__(self) -> str:
         """Return a unique identifier for the route handler.
 
         Returns:
             A string
         """
-        target: type[AsyncAnyCallable] | AsyncAnyCallable
+        target: type[AsyncAnyCallable] | AsyncAnyCallable  # pyright: ignore
         target = unwrap_partial(self.fn.value)
         if not hasattr(target, "__qualname__"):
             target = type(target)
         return f"{target.__module__}.{target.__qualname__}"
```

### Comparing `litestar-2.0.0b4/litestar/handlers/http_handlers/_utils.py` & `litestar-2.0.0rc1/litestar/handlers/http_handlers/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/handlers/http_handlers/base.py` & `litestar-2.0.0rc1/litestar/handlers/http_handlers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from enum import Enum
 from typing import TYPE_CHECKING, AnyStr, Mapping, TypedDict, cast
 
 from litestar._layers.utils import narrow_response_cookies, narrow_response_headers
 from litestar.datastructures.cookie import Cookie
 from litestar.datastructures.response_header import ResponseHeader
-from litestar.dto.interface import ConnectionContext
 from litestar.enums import HttpMethod, MediaType
 from litestar.exceptions import (
     HTTPException,
     ImproperlyConfiguredException,
 )
 from litestar.handlers.base import BaseRouteHandler
 from litestar.handlers.http_handlers._utils import (
@@ -51,17 +50,18 @@
     from typing import Any, Awaitable, Callable, Sequence
 
     from litestar.app import Litestar
     from litestar.background_tasks import BackgroundTask, BackgroundTasks
     from litestar.config.response_cache import CACHE_FOREVER
     from litestar.connection import Request
     from litestar.datastructures import CacheControlHeader, ETag
-    from litestar.dto.interface import DTOInterface
+    from litestar.dto import AbstractDTO
     from litestar.openapi.datastructures import ResponseSpec
     from litestar.openapi.spec import SecurityRequirement
+    from litestar.types.callable_types import OperationIDCreator
 
 __all__ = ("HTTPRouteHandler", "route")
 
 
 class ResponseHandlerMap(TypedDict):
     default_handler: Callable[[Any], Awaitable[ASGIApp]] | EmptyType
     response_type_handler: Callable[[Any], Awaitable[ASGIApp]] | EmptyType
@@ -119,37 +119,37 @@
         after_response: AfterResponseHookHandler | None = None,
         background: BackgroundTask | BackgroundTasks | None = None,
         before_request: BeforeRequestHookHandler | None = None,
         cache: bool | int | type[CACHE_FOREVER] = False,
         cache_control: CacheControlHeader | None = None,
         cache_key_builder: CacheKeyBuilder | None = None,
         dependencies: Dependencies | None = None,
-        dto: type[DTOInterface] | None | EmptyType = Empty,
+        dto: type[AbstractDTO] | None | EmptyType = Empty,
         etag: ETag | None = None,
         exception_handlers: ExceptionHandlersMap | None = None,
         guards: Sequence[Guard] | None = None,
         http_method: HttpMethod | Method | Sequence[HttpMethod | Method],
         media_type: MediaType | str | None = None,
         middleware: Sequence[Middleware] | None = None,
         name: str | None = None,
         opt: Mapping[str, Any] | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: ResponseHeaders | None = None,
-        return_dto: type[DTOInterface] | None | EmptyType = Empty,
+        return_dto: type[AbstractDTO] | None | EmptyType = Empty,
         status_code: int | None = None,
         sync_to_thread: bool | None = None,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
         include_in_schema: bool = True,
         operation_class: type[Operation] = Operation,
-        operation_id: str | None = None,
+        operation_id: str | OperationIDCreator | None = None,
         raises: Sequence[type[HTTPException]] | None = None,
         response_description: str | None = None,
         responses: Mapping[int, ResponseSpec] | None = None,
         signature_namespace: Mapping[str, Any] | None = None,
         security: Sequence[SecurityRequirement] | None = None,
         summary: str | None = None,
         tags: Sequence[str] | None = None,
@@ -175,15 +175,15 @@
             cache: Enables response caching if configured on the application level. Valid values are ``True`` or a
                 number of seconds (e.g. ``120``) to cache the response.
             cache_control: A ``cache-control`` header of type
                 :class:`CacheControlHeader <.datastructures.CacheControlHeader>` that will be added to the response.
             cache_key_builder: A :class:`cache-key builder function <.types.CacheKeyBuilder>`. Allows for customization
                 of the cache key if caching is configured on the application level.
             dependencies: A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances.
-            dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for (de)serializing and
+            dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for (de)serializing and
                 validation of request data.
             etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` that will be added to the response.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
             guards: A sequence of :class:`Guard <.types.Guard>` callables.
             http_method: An :class:`http method string <.types.Method>`, a member of the enum
                 :class:`HttpMethod <.enums.HttpMethod>` or a list of these that correlates to the methods the route
                 handler function should handle.
@@ -197,28 +197,28 @@
             response_class: A custom subclass of :class:`Response <.response.Response>` to be used as route handler's
                 default response.
             response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>` instances.
             response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
                 instances.
             responses: A mapping of additional status codes and a description of their expected content.
                 This information will be included in the OpenAPI schema
-            return_dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for serializing
+            return_dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for serializing
                 outbound response data.
             signature_namespace: A mapping of names to types for use in forward reference resolution during signature modelling.
             status_code: An http status code for the response. Defaults to ``200`` for mixed method or ``GET``, ``PUT`` and
                 ``PATCH``, ``201`` for ``POST`` and ``204`` for ``DELETE``.
             sync_to_thread: A boolean dictating whether the handler function will be executed in a worker thread or the
                 main event loop. This has an effect only for sync handler functions. See using sync handler functions.
             content_encoding: A string describing the encoding of the content, e.g. ``"base64"``.
             content_media_type: A string designating the media-type of the content, e.g. ``"image/png"``.
             deprecated:  A boolean dictating whether this route should be marked as deprecated in the OpenAPI schema.
             description: Text used for the route's schema description section.
             include_in_schema: A boolean flag dictating whether  the route handler should be documented in the OpenAPI schema.
             operation_class: :class:`Operation <.openapi.spec.operation.Operation>` to be used with the route's OpenAPI schema.
-            operation_id: An identifier used for the route's schema operationId. Defaults to the ``__name__`` of the wrapped function.
+            operation_id: Either a string or a callable returning a string. An identifier used for the route's schema operationId.
             raises:  A list of exception classes extending from litestar.HttpException that is used for the OpenAPI documentation.
                 This list should describe all exceptions raised within the route handler's function/method. The Litestar
                 ValidationException will be added automatically for the schema if any validation is involved.
             response_description: Text used for the route's response schema description section.
             security: A sequence of dictionaries that contain information about which security scheme can be used on the endpoint.
             summary: Text used for the route's schema summary section.
             tags: A sequence of string tags that will be appended to the OpenAPI schema.
@@ -465,27 +465,32 @@
                 a Response instance or an arbitrary value.
             request: A :class:`Request <.connection.Request>` instance
 
         Returns:
             A Response instance
         """
         if return_dto_type := self.resolve_return_dto():
-            ctx = ConnectionContext.from_connection(request)
-            data = return_dto_type(ctx).data_to_encodable_type(data)
+            data = return_dto_type(request).data_to_encodable_type(data)
 
         response_handler = self.get_response_handler(is_response_type_data=isinstance(data, Response))
         return await response_handler(app=app, data=data, request=request)  # type: ignore
 
     def on_registration(self, app: Litestar) -> None:
         if before_request := self.resolve_before_request():
             before_request.set_parsed_signature(self.resolve_signature_namespace())
 
         super().on_registration(app)
         self.resolve_after_response()
 
+        if self.sync_to_thread and not is_async_callable(self.fn.value):
+            self.fn.value = async_partial(self.fn.value)
+            self.has_sync_callable = False
+        else:
+            self.has_sync_callable = not is_async_callable(self.fn.value)
+
     def _validate_handler_function(self) -> None:
         """Validate the route handler function once it is set by inspecting its return annotations."""
         super()._validate_handler_function()
 
         return_type = self.parsed_fn_signature.return_type
 
         if return_type.annotation is Empty:
@@ -517,19 +522,9 @@
 
         if "socket" in self.parsed_fn_signature.parameters:
             raise ImproperlyConfiguredException("The 'socket' kwarg is not supported with http handlers")
 
         if "data" in self.parsed_fn_signature.parameters and "GET" in self.http_methods:
             raise ImproperlyConfiguredException("'data' kwarg is unsupported for 'GET' request handlers")
 
-    def _set_runtime_callables(self) -> None:
-        """Set the runtime callables for the route handler."""
-        super()._set_runtime_callables()
-        self.has_sync_callable = False
-        if not is_async_callable(self.fn.value):
-            if self.sync_to_thread:
-                self.fn.value = async_partial(self.fn.value)
-            else:
-                self.has_sync_callable = True
-
 
 route = HTTPRouteHandler
```

### Comparing `litestar-2.0.0b4/litestar/handlers/http_handlers/decorators.py` & `litestar-2.0.0rc1/litestar/handlers/http_handlers/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 if TYPE_CHECKING:
     from typing import Any, Mapping
 
     from litestar.background_tasks import BackgroundTask, BackgroundTasks
     from litestar.config.response_cache import CACHE_FOREVER
     from litestar.datastructures import CacheControlHeader, ETag
-    from litestar.dto.interface import DTOInterface
+    from litestar.dto import AbstractDTO
     from litestar.openapi.datastructures import ResponseSpec
     from litestar.openapi.spec import SecurityRequirement
     from litestar.types import (
         AfterRequestHookHandler,
         AfterResponseHookHandler,
         BeforeRequestHookHandler,
         CacheKeyBuilder,
@@ -32,14 +32,15 @@
         Guard,
         Middleware,
         ResponseCookies,
         ResponseHeaders,
         ResponseType,
         TypeEncodersMap,
     )
+    from litestar.types.callable_types import OperationIDCreator
 
 
 __all__ = ("get", "head", "post", "put", "patch", "delete")
 
 MSG_SEMANTIC_ROUTE_HANDLER_WITH_HTTP = "semantic route handlers cannot define http_method"
 
 
@@ -57,37 +58,37 @@
         after_response: AfterResponseHookHandler | None = None,
         background: BackgroundTask | BackgroundTasks | None = None,
         before_request: BeforeRequestHookHandler | None = None,
         cache: bool | int | type[CACHE_FOREVER] = False,
         cache_control: CacheControlHeader | None = None,
         cache_key_builder: CacheKeyBuilder | None = None,
         dependencies: Dependencies | None = None,
-        dto: type[DTOInterface] | None | EmptyType = Empty,
+        dto: type[AbstractDTO] | None | EmptyType = Empty,
         etag: ETag | None = None,
         exception_handlers: ExceptionHandlersMap | None = None,
         guards: list[Guard] | None = None,
         media_type: MediaType | str | None = None,
         middleware: list[Middleware] | None = None,
         name: str | None = None,
         opt: dict[str, Any] | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: ResponseHeaders | None = None,
-        return_dto: type[DTOInterface] | None | EmptyType = Empty,
+        return_dto: type[AbstractDTO] | None | EmptyType = Empty,
         signature_namespace: Mapping[str, Any] | None = None,
         status_code: int | None = None,
         sync_to_thread: bool | None = None,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
         include_in_schema: bool = True,
         operation_class: type[Operation] = Operation,
-        operation_id: str | None = None,
+        operation_id: str | OperationIDCreator | None = None,
         raises: list[type[HTTPException]] | None = None,
         response_description: str | None = None,
         responses: dict[int, ResponseSpec] | None = None,
         security: list[SecurityRequirement] | None = None,
         summary: str | None = None,
         tags: list[str] | None = None,
         type_encoders: TypeEncodersMap | None = None,
@@ -111,15 +112,15 @@
                 bypassing the route handler.
             cache: Enables response caching if configured on the application level. Valid values are ``True`` or a number
                 of seconds (e.g. ``120``) to cache the response.
             cache_control: A ``cache-control`` header of type
                 :class:`CacheControlHeader <.datastructures.CacheControlHeader>` that will be added to the response.
             cache_key_builder: A :class:`cache-key builder function <.types.CacheKeyBuilder>`. Allows for customization
                 of the cache key if caching is configured on the application level.
-            dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for (de)serializing and
+            dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for (de)serializing and
                 validation of request data.
             dependencies: A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances.
             etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` that will be added to the response.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
             guards: A sequence of :class:`Guard <.types.Guard>` callables.
             http_method: An :class:`http method string <.types.Method>`, a member of the enum
                 :class:`HttpMethod <litestar.enums.HttpMethod>` or a list of these that correlates to the methods the
@@ -133,28 +134,28 @@
             response_class: A custom subclass of :class:`Response <.response.Response>` to be used as route handler's
                 default response.
             response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>` instances.
             response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
                 instances.
             responses: A mapping of additional status codes and a description of their expected content.
                 This information will be included in the OpenAPI schema
-            return_dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for serializing
+            return_dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for serializing
                 outbound response data.
             signature_namespace: A mapping of names to types for use in forward reference resolution during signature modelling.
             status_code: An http status code for the response. Defaults to ``200`` for mixed method or ``GET``, ``PUT``
                 and ``PATCH``, ``201`` for ``POST`` and ``204`` for ``DELETE``.
             sync_to_thread: A boolean dictating whether the handler function will be executed in a worker thread or the
                 main event loop. This has an effect only for sync handler functions. See using sync handler functions.
             content_encoding: A string describing the encoding of the content, e.g. ``base64``.
             content_media_type: A string designating the media-type of the content, e.g. ``image/png``.
             deprecated:  A boolean dictating whether this route should be marked as deprecated in the OpenAPI schema.
             description: Text used for the route's schema description section.
             include_in_schema: A boolean flag dictating whether  the route handler should be documented in the OpenAPI schema.
             operation_class: :class:`Operation <.openapi.spec.operation.Operation>` to be used with the route's OpenAPI schema.
-            operation_id: An identifier used for the route's schema operationId. Defaults to the ``__name__`` of the wrapped function.
+            operation_id: Either a string or a callable returning a string. An identifier used for the route's schema operationId.
             raises:  A list of exception classes extending from litestar.HttpException that is used for the OpenAPI documentation.
                 This list should describe all exceptions raised within the route handler's function/method. The Litestar
                 ValidationException will be added automatically for the schema if any validation is involved.
             response_description: Text used for the route's response schema description section.
             security: A sequence of dictionaries that contain information about which security scheme can be used on the endpoint.
             summary: Text used for the route's schema summary section.
             tags: A sequence of string tags that will be appended to the OpenAPI schema.
@@ -221,37 +222,37 @@
         after_response: AfterResponseHookHandler | None = None,
         background: BackgroundTask | BackgroundTasks | None = None,
         before_request: BeforeRequestHookHandler | None = None,
         cache: bool | int | type[CACHE_FOREVER] = False,
         cache_control: CacheControlHeader | None = None,
         cache_key_builder: CacheKeyBuilder | None = None,
         dependencies: Dependencies | None = None,
-        dto: type[DTOInterface] | None | EmptyType = Empty,
+        dto: type[AbstractDTO] | None | EmptyType = Empty,
         etag: ETag | None = None,
         exception_handlers: ExceptionHandlersMap | None = None,
         guards: list[Guard] | None = None,
         media_type: MediaType | str | None = None,
         middleware: list[Middleware] | None = None,
         name: str | None = None,
         opt: dict[str, Any] | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: ResponseHeaders | None = None,
-        return_dto: type[DTOInterface] | None | EmptyType = Empty,
+        return_dto: type[AbstractDTO] | None | EmptyType = Empty,
         signature_namespace: Mapping[str, Any] | None = None,
         status_code: int | None = None,
         sync_to_thread: bool | None = None,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
         include_in_schema: bool = True,
         operation_class: type[Operation] = Operation,
-        operation_id: str | None = None,
+        operation_id: str | OperationIDCreator | None = None,
         raises: list[type[HTTPException]] | None = None,
         response_description: str | None = None,
         responses: dict[int, ResponseSpec] | None = None,
         security: list[SecurityRequirement] | None = None,
         summary: str | None = None,
         tags: list[str] | None = None,
         type_encoders: TypeEncodersMap | None = None,
@@ -276,15 +277,15 @@
             cache: Enables response caching if configured on the application level. Valid values are ``True`` or a number
                 of seconds (e.g. ``120``) to cache the response.
             cache_control: A ``cache-control`` header of type
                 :class:`CacheControlHeader <.datastructures.CacheControlHeader>` that will be added to the response.
             cache_key_builder: A :class:`cache-key builder function <.types.CacheKeyBuilder>`. Allows for customization
                 of the cache key if caching is configured on the application level.
             dependencies: A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances.
-            dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for (de)serializing and
+            dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for (de)serializing and
                 validation of request data.
             etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` that will be added to the response.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
             guards: A sequence of :class:`Guard <.types.Guard>` callables.
             http_method: An :class:`http method string <.types.Method>`, a member of the enum
                 :class:`HttpMethod <litestar.enums.HttpMethod>` or a list of these that correlates to the methods the
                 route handler function should handle.
@@ -297,28 +298,28 @@
             response_class: A custom subclass of :class:`Response <.response.Response>` to be used as route handler's
                 default response.
             response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>` instances.
             response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
                 instances.
             responses: A mapping of additional status codes and a description of their expected content.
                 This information will be included in the OpenAPI schema
-            return_dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for serializing
+            return_dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for serializing
                 outbound response data.
             signature_namespace: A mapping of names to types for use in forward reference resolution during signature modelling.
             status_code: An http status code for the response. Defaults to ``200`` for mixed method or ``GET``, ``PUT`` and
                 ``PATCH``, ``201`` for ``POST`` and ``204`` for ``DELETE``.
             sync_to_thread: A boolean dictating whether the handler function will be executed in a worker thread or the
                 main event loop. This has an effect only for sync handler functions. See using sync handler functions.
             content_encoding: A string describing the encoding of the content, e.g. ``base64``.
             content_media_type: A string designating the media-type of the content, e.g. ``image/png``.
             deprecated:  A boolean dictating whether this route should be marked as deprecated in the OpenAPI schema.
             description: Text used for the route's schema description section.
             include_in_schema: A boolean flag dictating whether  the route handler should be documented in the OpenAPI schema.
             operation_class: :class:`Operation <.openapi.spec.operation.Operation>` to be used with the route's OpenAPI schema.
-            operation_id: An identifier used for the route's schema operationId. Defaults to the ``__name__`` of the wrapped function.
+            operation_id: Either a string or a callable returning a string. An identifier used for the route's schema operationId.
             raises:  A list of exception classes extending from litestar.HttpException that is used for the OpenAPI documentation.
                 This list should describe all exceptions raised within the route handler's function/method. The Litestar
                 ValidationException will be added automatically for the schema if any validation is involved.
             response_description: Text used for the route's response schema description section.
             security: A sequence of dictionaries that contain information about which security scheme can be used on the endpoint.
             summary: Text used for the route's schema summary section.
             tags: A sequence of string tags that will be appended to the OpenAPI schema.
@@ -386,15 +387,15 @@
         after_response: AfterResponseHookHandler | None = None,
         background: BackgroundTask | BackgroundTasks | None = None,
         before_request: BeforeRequestHookHandler | None = None,
         cache: bool | int | type[CACHE_FOREVER] = False,
         cache_control: CacheControlHeader | None = None,
         cache_key_builder: CacheKeyBuilder | None = None,
         dependencies: Dependencies | None = None,
-        dto: type[DTOInterface] | None | EmptyType = Empty,
+        dto: type[AbstractDTO] | None | EmptyType = Empty,
         etag: ETag | None = None,
         exception_handlers: ExceptionHandlersMap | None = None,
         guards: list[Guard] | None = None,
         media_type: MediaType | str | None = None,
         middleware: list[Middleware] | None = None,
         name: str | None = None,
         opt: dict[str, Any] | None = None,
@@ -407,19 +408,19 @@
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
         include_in_schema: bool = True,
         operation_class: type[Operation] = Operation,
-        operation_id: str | None = None,
+        operation_id: str | OperationIDCreator | None = None,
         raises: list[type[HTTPException]] | None = None,
         response_description: str | None = None,
         responses: dict[int, ResponseSpec] | None = None,
-        return_dto: type[DTOInterface] | None | EmptyType = Empty,
+        return_dto: type[AbstractDTO] | None | EmptyType = Empty,
         security: list[SecurityRequirement] | None = None,
         summary: str | None = None,
         tags: list[str] | None = None,
         type_encoders: TypeEncodersMap | None = None,
         **kwargs: Any,
     ) -> None:
         """Initialize ``head``.
@@ -445,15 +446,15 @@
             cache: Enables response caching if configured on the application level. Valid values are ``True`` or a number
                 of seconds (e.g. ``120``) to cache the response.
             cache_control: A ``cache-control`` header of type
                 :class:`CacheControlHeader <.datastructures.CacheControlHeader>` that will be added to the response.
             cache_key_builder: A :class:`cache-key builder function <.types.CacheKeyBuilder>`. Allows for customization
                 of the cache key if caching is configured on the application level.
             dependencies: A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances.
-            dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for (de)serializing and
+            dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for (de)serializing and
                 validation of request data.
             etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` that will be added to the response.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
             guards: A sequence of :class:`Guard <.types.Guard>` callables.
             http_method: An :class:`http method string <.types.Method>`, a member of the enum
                 :class:`HttpMethod <litestar.enums.HttpMethod>` or a list of these that correlates to the methods the
                 route handler function should handle.
@@ -466,28 +467,28 @@
             response_class: A custom subclass of :class:`Response <.response.Response>` to be used as route handler's
                 default response.
             response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>` instances.
             response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
                 instances.
             responses: A mapping of additional status codes and a description of their expected content.
                 This information will be included in the OpenAPI schema
-            return_dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for serializing
+            return_dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for serializing
                 outbound response data.
             signature_namespace: A mapping of names to types for use in forward reference resolution during signature modelling.
             status_code: An http status code for the response. Defaults to ``200`` for mixed method or ``GET``, ``PUT`` and
                 ``PATCH``, ``201`` for ``POST`` and ``204`` for ``DELETE``.
             sync_to_thread: A boolean dictating whether the handler function will be executed in a worker thread or the
                 main event loop. This has an effect only for sync handler functions. See using sync handler functions.
             content_encoding: A string describing the encoding of the content, e.g. ``base64``.
             content_media_type: A string designating the media-type of the content, e.g. ``image/png``.
             deprecated:  A boolean dictating whether this route should be marked as deprecated in the OpenAPI schema.
             description: Text used for the route's schema description section.
             include_in_schema: A boolean flag dictating whether  the route handler should be documented in the OpenAPI schema.
             operation_class: :class:`Operation <.openapi.spec.operation.Operation>` to be used with the route's OpenAPI schema.
-            operation_id: An identifier used for the route's schema operationId. Defaults to the ``__name__`` of the wrapped function.
+            operation_id: Either a string or a callable returning a string. An identifier used for the route's schema operationId.
             raises:  A list of exception classes extending from litestar.HttpException that is used for the OpenAPI documentation.
                 This list should describe all exceptions raised within the route handler's function/method. The Litestar
                 ValidationException will be added automatically for the schema if any validation is involved.
             response_description: Text used for the route's response schema description section.
             security: A sequence of dictionaries that contain information about which security scheme can be used on the endpoint.
             summary: Text used for the route's schema summary section.
             tags: A sequence of string tags that will be appended to the OpenAPI schema.
@@ -568,37 +569,37 @@
         after_response: AfterResponseHookHandler | None = None,
         background: BackgroundTask | BackgroundTasks | None = None,
         before_request: BeforeRequestHookHandler | None = None,
         cache: bool | int | type[CACHE_FOREVER] = False,
         cache_control: CacheControlHeader | None = None,
         cache_key_builder: CacheKeyBuilder | None = None,
         dependencies: Dependencies | None = None,
-        dto: type[DTOInterface] | None | EmptyType = Empty,
+        dto: type[AbstractDTO] | None | EmptyType = Empty,
         etag: ETag | None = None,
         exception_handlers: ExceptionHandlersMap | None = None,
         guards: list[Guard] | None = None,
         media_type: MediaType | str | None = None,
         middleware: list[Middleware] | None = None,
         name: str | None = None,
         opt: dict[str, Any] | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: ResponseHeaders | None = None,
-        return_dto: type[DTOInterface] | None | EmptyType = Empty,
+        return_dto: type[AbstractDTO] | None | EmptyType = Empty,
         signature_namespace: Mapping[str, Any] | None = None,
         status_code: int | None = None,
         sync_to_thread: bool | None = None,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
         include_in_schema: bool = True,
         operation_class: type[Operation] = Operation,
-        operation_id: str | None = None,
+        operation_id: str | OperationIDCreator | None = None,
         raises: list[type[HTTPException]] | None = None,
         response_description: str | None = None,
         responses: dict[int, ResponseSpec] | None = None,
         security: list[SecurityRequirement] | None = None,
         summary: str | None = None,
         tags: list[str] | None = None,
         type_encoders: TypeEncodersMap | None = None,
@@ -623,15 +624,15 @@
             cache: Enables response caching if configured on the application level. Valid values are ``True`` or a number
                 of seconds (e.g. ``120``) to cache the response.
             cache_control: A ``cache-control`` header of type
                 :class:`CacheControlHeader <.datastructures.CacheControlHeader>` that will be added to the response.
             cache_key_builder: A :class:`cache-key builder function <.types.CacheKeyBuilder>`. Allows for customization
                 of the cache key if caching is configured on the application level.
             dependencies: A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances.
-            dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for (de)serializing and
+            dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for (de)serializing and
                 validation of request data.
             etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` that will be added to the response.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
             guards: A sequence of :class:`Guard <.types.Guard>` callables.
             http_method: An :class:`http method string <.types.Method>`, a member of the enum
                 :class:`HttpMethod <litestar.enums.HttpMethod>` or a list of these that correlates to the methods the
                 route handler function should handle.
@@ -644,28 +645,28 @@
             response_class: A custom subclass of :class:`Response <.response.Response>` to be used as route handler's
                 default response.
             response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>` instances.
             response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
                 instances.
             responses: A mapping of additional status codes and a description of their expected content.
                 This information will be included in the OpenAPI schema
-            return_dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for serializing
+            return_dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for serializing
                 outbound response data.
             signature_namespace: A mapping of names to types for use in forward reference resolution during signature modelling.
             status_code: An http status code for the response. Defaults to ``200`` for mixed method or ``GET``, ``PUT`` and
                 ``PATCH``, ``201`` for ``POST`` and ``204`` for ``DELETE``.
             sync_to_thread: A boolean dictating whether the handler function will be executed in a worker thread or the
                 main event loop. This has an effect only for sync handler functions. See using sync handler functions.
             content_encoding: A string describing the encoding of the content, e.g. ``base64``.
             content_media_type: A string designating the media-type of the content, e.g. ``image/png``.
             deprecated:  A boolean dictating whether this route should be marked as deprecated in the OpenAPI schema.
             description: Text used for the route's schema description section.
             include_in_schema: A boolean flag dictating whether  the route handler should be documented in the OpenAPI schema.
             operation_class: :class:`Operation <.openapi.spec.operation.Operation>` to be used with the route's OpenAPI schema.
-            operation_id: An identifier used for the route's schema operationId. Defaults to the ``__name__`` of the wrapped function.
+            operation_id: Either a string or a callable returning a string. An identifier used for the route's schema operationId.
             raises:  A list of exception classes extending from litestar.HttpException that is used for the OpenAPI documentation.
                 This list should describe all exceptions raised within the route handler's function/method. The Litestar
                 ValidationException will be added automatically for the schema if any validation is involved.
             response_description: Text used for the route's response schema description section.
             security: A sequence of dictionaries that contain information about which security scheme can be used on the endpoint.
             summary: Text used for the route's schema summary section.
             tags: A sequence of string tags that will be appended to the OpenAPI schema.
@@ -732,37 +733,37 @@
         after_response: AfterResponseHookHandler | None = None,
         background: BackgroundTask | BackgroundTasks | None = None,
         before_request: BeforeRequestHookHandler | None = None,
         cache: bool | int | type[CACHE_FOREVER] = False,
         cache_control: CacheControlHeader | None = None,
         cache_key_builder: CacheKeyBuilder | None = None,
         dependencies: Dependencies | None = None,
-        dto: type[DTOInterface] | None | EmptyType = Empty,
+        dto: type[AbstractDTO] | None | EmptyType = Empty,
         etag: ETag | None = None,
         exception_handlers: ExceptionHandlersMap | None = None,
         guards: list[Guard] | None = None,
         media_type: MediaType | str | None = None,
         middleware: list[Middleware] | None = None,
         name: str | None = None,
         opt: dict[str, Any] | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: ResponseHeaders | None = None,
-        return_dto: type[DTOInterface] | None | EmptyType = Empty,
+        return_dto: type[AbstractDTO] | None | EmptyType = Empty,
         signature_namespace: Mapping[str, Any] | None = None,
         status_code: int | None = None,
         sync_to_thread: bool | None = None,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
         include_in_schema: bool = True,
         operation_class: type[Operation] = Operation,
-        operation_id: str | None = None,
+        operation_id: str | OperationIDCreator | None = None,
         raises: list[type[HTTPException]] | None = None,
         response_description: str | None = None,
         responses: dict[int, ResponseSpec] | None = None,
         security: list[SecurityRequirement] | None = None,
         summary: str | None = None,
         tags: list[str] | None = None,
         type_encoders: TypeEncodersMap | None = None,
@@ -787,15 +788,15 @@
             cache: Enables response caching if configured on the application level. Valid values are ``True`` or a number
                 of seconds (e.g. ``120``) to cache the response.
             cache_control: A ``cache-control`` header of type
                 :class:`CacheControlHeader <.datastructures.CacheControlHeader>` that will be added to the response.
             cache_key_builder: A :class:`cache-key builder function <.types.CacheKeyBuilder>`. Allows for customization
                 of the cache key if caching is configured on the application level.
             dependencies: A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances.
-            dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for (de)serializing and
+            dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for (de)serializing and
                 validation of request data.
             etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` that will be added to the response.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
             guards: A sequence of :class:`Guard <.types.Guard>` callables.
             http_method: An :class:`http method string <.types.Method>`, a member of the enum
                 :class:`HttpMethod <litestar.enums.HttpMethod>` or a list of these that correlates to the methods the
                 route handler function should handle.
@@ -808,28 +809,28 @@
             response_class: A custom subclass of :class:`Response <.response.Response>` to be used as route handler's
                 default response.
             response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>` instances.
             response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
                 instances.
             responses: A mapping of additional status codes and a description of their expected content.
                 This information will be included in the OpenAPI schema
-            return_dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for serializing
+            return_dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for serializing
                 outbound response data.
             signature_namespace: A mapping of names to types for use in forward reference resolution during signature modelling.
             status_code: An http status code for the response. Defaults to ``200`` for mixed method or ``GET``, ``PUT`` and
                 ``PATCH``, ``201`` for ``POST`` and ``204`` for ``DELETE``.
             sync_to_thread: A boolean dictating whether the handler function will be executed in a worker thread or the
                 main event loop. This has an effect only for sync handler functions. See using sync handler functions.
             content_encoding: A string describing the encoding of the content, e.g. ``base64``.
             content_media_type: A string designating the media-type of the content, e.g. ``image/png``.
             deprecated:  A boolean dictating whether this route should be marked as deprecated in the OpenAPI schema.
             description: Text used for the route's schema description section.
             include_in_schema: A boolean flag dictating whether  the route handler should be documented in the OpenAPI schema.
             operation_class: :class:`Operation <.openapi.spec.operation.Operation>` to be used with the route's OpenAPI schema.
-            operation_id: An identifier used for the route's schema operationId. Defaults to the ``__name__`` of the wrapped function.
+            operation_id: Either a string or a callable returning a string. An identifier used for the route's schema operationId.
             raises:  A list of exception classes extending from litestar.HttpException that is used for the OpenAPI documentation.
                 This list should describe all exceptions raised within the route handler's function/method. The Litestar
                 ValidationException will be added automatically for the schema if any validation is involved.
             response_description: Text used for the route's response schema description section.
             security: A sequence of dictionaries that contain information about which security scheme can be used on the endpoint.
             summary: Text used for the route's schema summary section.
             tags: A sequence of string tags that will be appended to the OpenAPI schema.
@@ -896,37 +897,37 @@
         after_response: AfterResponseHookHandler | None = None,
         background: BackgroundTask | BackgroundTasks | None = None,
         before_request: BeforeRequestHookHandler | None = None,
         cache: bool | int | type[CACHE_FOREVER] = False,
         cache_control: CacheControlHeader | None = None,
         cache_key_builder: CacheKeyBuilder | None = None,
         dependencies: Dependencies | None = None,
-        dto: type[DTOInterface] | None | EmptyType = Empty,
+        dto: type[AbstractDTO] | None | EmptyType = Empty,
         etag: ETag | None = None,
         exception_handlers: ExceptionHandlersMap | None = None,
         guards: list[Guard] | None = None,
         media_type: MediaType | str | None = None,
         middleware: list[Middleware] | None = None,
         name: str | None = None,
         opt: dict[str, Any] | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: ResponseHeaders | None = None,
-        return_dto: type[DTOInterface] | None | EmptyType = Empty,
+        return_dto: type[AbstractDTO] | None | EmptyType = Empty,
         signature_namespace: Mapping[str, Any] | None = None,
         status_code: int | None = None,
         sync_to_thread: bool | None = None,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
         include_in_schema: bool = True,
         operation_class: type[Operation] = Operation,
-        operation_id: str | None = None,
+        operation_id: str | OperationIDCreator | None = None,
         raises: list[type[HTTPException]] | None = None,
         response_description: str | None = None,
         responses: dict[int, ResponseSpec] | None = None,
         security: list[SecurityRequirement] | None = None,
         summary: str | None = None,
         tags: list[str] | None = None,
         type_encoders: TypeEncodersMap | None = None,
@@ -951,15 +952,15 @@
             cache: Enables response caching if configured on the application level. Valid values are ``True`` or a number
                 of seconds (e.g. ``120``) to cache the response.
             cache_control: A ``cache-control`` header of type
                 :class:`CacheControlHeader <.datastructures.CacheControlHeader>` that will be added to the response.
             cache_key_builder: A :class:`cache-key builder function <.types.CacheKeyBuilder>`. Allows for customization
                 of the cache key if caching is configured on the application level.
             dependencies: A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances.
-            dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for (de)serializing and
+            dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for (de)serializing and
                 validation of request data.
             etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` that will be added to the response.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
             guards: A sequence of :class:`Guard <.types.Guard>` callables.
             http_method: An :class:`http method string <.types.Method>`, a member of the enum
                 :class:`HttpMethod <litestar.enums.HttpMethod>` or a list of these that correlates to the methods the
                 route handler function should handle.
@@ -972,28 +973,28 @@
             response_class: A custom subclass of :class:`Response <.response.Response>` to be used as route handler's
                 default response.
             response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>` instances.
             response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
                 instances.
             responses: A mapping of additional status codes and a description of their expected content.
                 This information will be included in the OpenAPI schema
-            return_dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for serializing
+            return_dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for serializing
                 outbound response data.
             signature_namespace: A mapping of names to types for use in forward reference resolution during signature modelling.
             status_code: An http status code for the response. Defaults to ``200`` for mixed method or ``GET``, ``PUT`` and
                 ``PATCH``, ``201`` for ``POST`` and ``204`` for ``DELETE``.
             sync_to_thread: A boolean dictating whether the handler function will be executed in a worker thread or the
                 main event loop. This has an effect only for sync handler functions. See using sync handler functions.
             content_encoding: A string describing the encoding of the content, e.g. ``base64``.
             content_media_type: A string designating the media-type of the content, e.g. ``image/png``.
             deprecated:  A boolean dictating whether this route should be marked as deprecated in the OpenAPI schema.
             description: Text used for the route's schema description section.
             include_in_schema: A boolean flag dictating whether  the route handler should be documented in the OpenAPI schema.
             operation_class: :class:`Operation <.openapi.spec.operation.Operation>` to be used with the route's OpenAPI schema.
-            operation_id: An identifier used for the route's schema operationId. Defaults to the ``__name__`` of the wrapped function.
+            operation_id: Either a string or a callable returning a string. An identifier used for the route's schema operationId.
             raises:  A list of exception classes extending from litestar.HttpException that is used for the OpenAPI documentation.
                 This list should describe all exceptions raised within the route handler's function/method. The Litestar
                 ValidationException will be added automatically for the schema if any validation is involved.
             response_description: Text used for the route's response schema description section.
             security: A sequence of dictionaries that contain information about which security scheme can be used on the endpoint.
             summary: Text used for the route's schema summary section.
             tags: A sequence of string tags that will be appended to the OpenAPI schema.
```

### Comparing `litestar-2.0.0b4/litestar/handlers/websocket_handlers/_utils.py` & `litestar-2.0.0rc1/litestar/handlers/websocket_handlers/_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,174 +1,145 @@
 from __future__ import annotations
 
-import inspect
 from functools import wraps
-from typing import TYPE_CHECKING, Any, Callable, Coroutine, Dict, cast
+from inspect import Parameter, Signature
+from typing import TYPE_CHECKING, Any, Callable, Coroutine, Dict
+
+from msgspec.json import Encoder as JsonEncoder
 
 from litestar.di import Provide
-from litestar.dto.interface import ConnectionContext
 from litestar.serialization import decode_json
+from litestar.types.builtin_types import NoneType
 from litestar.utils import AsyncCallable
 from litestar.utils.helpers import unwrap_partial
 
 if TYPE_CHECKING:
-    from contextlib import AbstractAsyncContextManager
-
-    from msgspec.json import Encoder as JsonEncoder
-
     from litestar import WebSocket
-    from litestar.dto.interface import DTOInterface
-    from litestar.types import AnyCallable, TypeEncodersMap
-    from litestar.types.asgi_types import WebSocketMode
+    from litestar.handlers.websocket_handlers.listener import WebsocketListenerRouteHandler
+    from litestar.types import AnyCallable
     from litestar.utils.signature import ParsedSignature
 
 
-class ListenerContext:
-    __slots__ = (
-        "can_send_data",
-        "handler_function",
-        "handle_receive",
-        "handle_send",
-        "json_encoder",
-        "listener_callback",
-        "listener_callback_signature",
-        "pass_socket",
-        "resolved_data_dto",
-        "resolved_return_dto",
-    )
+def create_handle_receive(listener: WebsocketListenerRouteHandler) -> Callable[[WebSocket], Coroutine[Any, None, None]]:
+    if data_dto := listener.resolve_data_dto():
 
-    can_send_data: bool
-    handler_function: AnyCallable
-    handle_receive: Callable[[WebSocket, DTOInterface | None], Any]
-    handle_send: Callable[[WebSocket, Any, DTOInterface | None], Coroutine[None, None, None]]
-    json_encoder: JsonEncoder
-    listener_callback: AnyCallable
-    listener_callback_signature: ParsedSignature
-    pass_socket: bool
-    resolved_data_dto: type[DTOInterface] | None
-    resolved_return_dto: type[DTOInterface] | None
-    resolved_type_encoders: TypeEncodersMap
-
-
-def create_handle_receive(
-    resolved_data_dto: type[DTOInterface] | None,
-    receive_mode: WebSocketMode,
-    wants_receive_type: type,
-) -> Callable[[WebSocket, DTOInterface | None], Coroutine[Any, None, None]]:
-    if resolved_data_dto:
-
-        async def handle_receive(socket: WebSocket, dto: DTOInterface | None) -> Any:
-            received_data = await socket.receive_data(mode=receive_mode)
-            if isinstance(received_data, str):
-                received_data = received_data.encode("utf-8")
-            return cast("DTOInterface", dto).bytes_to_data_type(received_data)
-
-    elif wants_receive_type is str:
-
-        async def handle_receive(socket: WebSocket, dto: DTOInterface | None) -> Any:
-            received_data = await socket.receive_data(mode=receive_mode)
-            if isinstance(received_data, bytes):
-                return received_data.decode("utf-8")
-            return received_data
-
-    elif wants_receive_type is bytes:
-
-        async def handle_receive(socket: WebSocket, dto: DTOInterface | None) -> Any:
-            received_data = await socket.receive_data(mode=receive_mode)
-            if isinstance(received_data, str):
-                return received_data.encode("utf-8")
-            return received_data
+        async def handle_receive(socket: WebSocket) -> Any:
+            received_data = await socket.receive_data(mode=listener._receive_mode)
+            return data_dto(socket).decode_bytes(
+                received_data.encode("utf-8") if isinstance(received_data, str) else received_data
+            )
+
+    elif listener.parsed_data_field and listener.parsed_data_field.annotation is str:
+
+        async def handle_receive(socket: WebSocket) -> Any:
+            received_data = await socket.receive_data(mode=listener._receive_mode)
+            return received_data.decode("utf-8") if isinstance(received_data, bytes) else received_data
+
+    elif listener.parsed_data_field and listener.parsed_data_field.annotation is bytes:
+
+        async def handle_receive(socket: WebSocket) -> Any:
+            received_data = await socket.receive_data(mode=listener._receive_mode)
+            return received_data.encode("utf-8") if isinstance(received_data, str) else received_data
 
     else:
 
-        async def handle_receive(socket: WebSocket, dto: DTOInterface | None) -> Any:
-            received_data = await socket.receive_data(mode=receive_mode)
+        async def handle_receive(socket: WebSocket) -> Any:
+            received_data = await socket.receive_data(mode=listener._receive_mode)
             return decode_json(value=received_data, type_decoders=socket.route_handler.resolve_type_decoders())
 
     return handle_receive
 
 
 def create_handle_send(
-    resolved_return_dto: type[DTOInterface] | None,
-    json_encoder: JsonEncoder,
-    should_encode_to_json: bool,
-    send_mode: WebSocketMode,
-) -> Callable[[WebSocket, Any, DTOInterface | None], Coroutine[None, None, None]]:
-    if resolved_return_dto:
-
-        async def handle_send(socket: WebSocket, data_to_send: Any, dto: DTOInterface | None) -> None:
-            data_to_send = json_encoder.encode(cast("DTOInterface", dto).data_to_encodable_type(data_to_send))
-            await socket.send_data(data_to_send, send_mode)  # pyright: ignore
-
-    elif should_encode_to_json:
-
-        async def handle_send(socket: WebSocket, data_to_send: Any, dto: DTOInterface | None) -> None:
-            data_to_send = json_encoder.encode(data_to_send)
-            await socket.send_data(data_to_send, send_mode)  # pyright: ignore
+    listener: WebsocketListenerRouteHandler,
+) -> Callable[[WebSocket, Any], Coroutine[None, None, None]]:
+    json_encoder = JsonEncoder(enc_hook=listener.default_serializer)
+
+    if return_dto := listener.resolve_return_dto():
+
+        async def handle_send(socket: WebSocket, data: Any) -> None:
+            encoded_data = return_dto(socket).data_to_encodable_type(data)
+            data = json_encoder.encode(encoded_data)
+            await socket.send_data(data=data, mode=listener._send_mode)
+
+    elif listener.parsed_return_field.is_subclass_of((str, bytes)) or (
+        listener.parsed_return_field.is_optional and listener.parsed_return_field.has_inner_subclass_of((str, bytes))
+    ):
+
+        async def handle_send(socket: WebSocket, data: Any) -> None:
+            await socket.send_data(data=data, mode=listener._send_mode)
 
     else:
 
-        async def handle_send(socket: WebSocket, data_to_send: Any, dto: DTOInterface | None) -> None:
-            await socket.send_data(data_to_send, send_mode)  # pyright: ignore
+        async def handle_send(socket: WebSocket, data: Any) -> None:
+            data = json_encoder.encode(data)
+            await socket.send_data(data=data, mode=listener._send_mode)
 
     return handle_send
 
 
-def create_handler_function(
-    listener_context: ListenerContext,
-    lifespan_manager: Callable[..., AbstractAsyncContextManager],
-) -> Callable[..., Coroutine[None, None, None]]:
-    listener_callback = AsyncCallable(listener_context.listener_callback)
+class ListenerHandler:
+    __slots__ = ("_can_send_data", "_fn", "_listener", "_pass_socket")
 
-    async def handler_fn(
-        *args: Any, socket: WebSocket, connection_lifespan_dependencies: Dict[str, Any], **kwargs: Any  # noqa: UP006
+    def __init__(
+        self,
+        listener: WebsocketListenerRouteHandler,
+        fn: AnyCallable,
+        parsed_signature: ParsedSignature,
+        namespace: dict[str, Any],
+    ) -> None:
+        self._can_send_data = not parsed_signature.return_type.is_subclass_of(NoneType)
+        self._fn = AsyncCallable(fn)
+        self._listener = listener
+        self._pass_socket = "socket" in parsed_signature.parameters
+
+    async def __call__(
+        self,
+        *args: Any,
+        socket: WebSocket,
+        connection_lifespan_dependencies: Dict[str, Any],  # noqa: UP006
+        **kwargs: Any,
     ) -> None:
-        ctx = ConnectionContext.from_connection(socket)
-        data_dto = listener_context.resolved_data_dto(ctx) if listener_context.resolved_data_dto else None
-        return_dto = listener_context.resolved_return_dto(ctx) if listener_context.resolved_return_dto else None
-        handle_receive = listener_context.handle_receive
-        handle_send = listener_context.handle_send if listener_context.can_send_data else None
+        lifespan_mananger = self._listener._connection_lifespan or self._listener.default_connection_lifespan
+        handle_send = self._listener.resolve_send_handler() if self._can_send_data else None
+        handle_receive = self._listener.resolve_receive_handler()
 
-        if listener_context.pass_socket:
+        if self._pass_socket:
             kwargs["socket"] = socket
 
-        async with lifespan_manager(**connection_lifespan_dependencies):
+        async with lifespan_mananger(**connection_lifespan_dependencies):
             while True:
-                received_data = await handle_receive(socket, data_dto)
-                data_to_send = await listener_callback(*args, data=received_data, **kwargs)
+                received_data = await handle_receive(socket)
+                data = await self._fn(*args, data=received_data, **kwargs)
                 if handle_send:
-                    await handle_send(socket, data_to_send, return_dto)
-
-    return handler_fn
+                    await handle_send(socket, data)
 
 
-def create_handler_signature(callback_signature: inspect.Signature) -> inspect.Signature:
-    """Creates a :class:`inspect.Signature` for the handler function for signature modelling.
+def create_handler_signature(callback_signature: Signature) -> Signature:
+    """Creates a :class:`Signature` for the handler function for signature modelling.
 
     This is required for two reasons:
 
         1. the :class:`.handlers.WebsocketHandler` signature model cannot contain the ``data`` parameter, which is
             required for :class:`.handlers.websocket_listener` handlers.
         2. the :class;`.handlers.WebsocketHandler` signature model must include the ``socket`` parameter, which is
             optional for :class:`.handlers.websocket_listener` handlers.
 
     Args:
-        callback_signature: The :class:`inspect.Signature` of the listener callback.
+        callback_signature: The :class:`Signature` of the listener callback.
 
     Returns:
-        The :class:`inspect.Signature` for the listener callback as required for signature modelling.
+        The :class:`Signature` for the listener callback as required for signature modelling.
     """
-    new_params = [p for p in callback_signature.parameters.values() if p.name not in {"data"}]
+    new_params = [p for p in callback_signature.parameters.values() if p.name != "data"]
     if "socket" not in callback_signature.parameters:
-        new_params.append(inspect.Parameter(name="socket", kind=inspect.Parameter.KEYWORD_ONLY, annotation="WebSocket"))
+        new_params.append(Parameter(name="socket", kind=Parameter.KEYWORD_ONLY, annotation="WebSocket"))
 
     new_params.append(
-        inspect.Parameter(
-            name="connection_lifespan_dependencies", kind=inspect.Parameter.KEYWORD_ONLY, annotation="Dict[str, Any]"
-        )
+        Parameter(name="connection_lifespan_dependencies", kind=Parameter.KEYWORD_ONLY, annotation="Dict[str, Any]")
     )
 
     return callback_signature.replace(parameters=new_params)
 
 
 def create_stub_dependency(src: AnyCallable) -> Provide:
     """Create a stub dependency, accepting any kwargs defined in ``src``, and
```

### Comparing `litestar-2.0.0b4/litestar/handlers/websocket_handlers/listener.py` & `litestar-2.0.0rc1/litestar/handlers/websocket_handlers/listener.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,149 +1,141 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from contextlib import AbstractAsyncContextManager, asynccontextmanager
-from functools import partial
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncGenerator,
     Callable,
     Dict,
     Mapping,
     Optional,
     cast,
     overload,
 )
 
-from msgspec.json import Encoder as JsonEncoder
-
 from litestar._signature import SignatureModel
 from litestar.connection import WebSocket
-from litestar.dto.interface import HandlerContext
 from litestar.exceptions import ImproperlyConfiguredException, WebSocketDisconnect
-from litestar.serialization import default_serializer
 from litestar.types import (
     AnyCallable,
     Dependencies,
     Empty,
     EmptyType,
     ExceptionHandler,
     Guard,
     Middleware,
     TypeEncodersMap,
 )
-from litestar.types.builtin_types import NoneType
 from litestar.utils import AsyncCallable
-from litestar.utils.signature import ParsedSignature
+from litestar.utils.signature import ParsedSignature, get_fn_type_hints
 
 from ._utils import (
-    ListenerContext,
+    ListenerHandler,
     create_handle_receive,
     create_handle_send,
-    create_handler_function,
     create_handler_signature,
     create_stub_dependency,
 )
 from .route_handler import WebsocketRouteHandler
 
 if TYPE_CHECKING:
     from typing import Coroutine
 
-    from litestar import Litestar, Router
-    from litestar.dto.interface import DTOInterface
-    from litestar.types.asgi_types import WebSocketMode
+    from typing_extensions import Self
 
+    from litestar import Router
+    from litestar.dto import AbstractDTO
+    from litestar.types.asgi_types import WebSocketMode
 
-__all__ = ("WebsocketListener", "websocket_listener")
+__all__ = ("WebsocketListener", "WebsocketListenerRouteHandler", "websocket_listener")
 
 
-class websocket_listener(WebsocketRouteHandler):
+class WebsocketListenerRouteHandler(WebsocketRouteHandler):
     """A websocket listener that automatically accepts a connection, handles disconnects,
     invokes a callback function every time new data is received and sends any data
     returned
     """
 
     __slots__ = {
         "connection_accept_handler": "Callback to accept a WebSocket connection. By default, calls WebSocket.accept",
         "on_accept": "Callback invoked after a WebSocket connection has been accepted",
         "on_disconnect": "Callback invoked after a WebSocket connection has been closed",
-        "_initialized": None,
-        "_pass_socket": None,
+        "_connection_lifespan": None,
+        "_handle_receive": None,
+        "_handle_send": None,
         "_receive_mode": None,
         "_send_mode": None,
-        "_listener_context": None,
-        "_connection_lifespan": None,
-        "_dependency_stubs": None,
     }
 
     @overload
     def __init__(
         self,
         path: str | None | list[str] | None = None,
         *,
         connection_lifespan: Callable[..., AbstractAsyncContextManager[Any]] | None = None,
         dependencies: Dependencies | None = None,
-        dto: type[DTOInterface] | None | EmptyType = Empty,
+        dto: type[AbstractDTO] | None | EmptyType = Empty,
         exception_handlers: dict[int | type[Exception], ExceptionHandler] | None = None,
         guards: list[Guard] | None = None,
         middleware: list[Middleware] | None = None,
         receive_mode: WebSocketMode = "text",
         send_mode: WebSocketMode = "text",
         name: str | None = None,
         opt: dict[str, Any] | None = None,
-        return_dto: type[DTOInterface] | None | EmptyType = Empty,
+        return_dto: type[AbstractDTO] | None | EmptyType = Empty,
         signature_namespace: Mapping[str, Any] | None = None,
         type_encoders: TypeEncodersMap | None = None,
         **kwargs: Any,
     ) -> None:
         ...
 
     @overload
     def __init__(
         self,
         path: str | None | list[str] | None = None,
         *,
         connection_accept_handler: Callable[[WebSocket], Coroutine[Any, Any, None]] = WebSocket.accept,
         dependencies: Dependencies | None = None,
-        dto: type[DTOInterface] | None | EmptyType = Empty,
+        dto: type[AbstractDTO] | None | EmptyType = Empty,
         exception_handlers: dict[int | type[Exception], ExceptionHandler] | None = None,
         guards: list[Guard] | None = None,
         middleware: list[Middleware] | None = None,
         receive_mode: WebSocketMode = "text",
         send_mode: WebSocketMode = "text",
         name: str | None = None,
         on_accept: AnyCallable | None = None,
         on_disconnect: AnyCallable | None = None,
         opt: dict[str, Any] | None = None,
-        return_dto: type[DTOInterface] | None | EmptyType = Empty,
+        return_dto: type[AbstractDTO] | None | EmptyType = Empty,
         signature_namespace: Mapping[str, Any] | None = None,
         type_encoders: TypeEncodersMap | None = None,
         **kwargs: Any,
     ) -> None:
         ...
 
     def __init__(
         self,
         path: str | None | list[str] | None = None,
         *,
         connection_accept_handler: Callable[[WebSocket], Coroutine[Any, Any, None]] = WebSocket.accept,
         connection_lifespan: Callable[..., AbstractAsyncContextManager[Any]] | None = None,
         dependencies: Dependencies | None = None,
-        dto: type[DTOInterface] | None | EmptyType = Empty,
+        dto: type[AbstractDTO] | None | EmptyType = Empty,
         exception_handlers: dict[int | type[Exception], ExceptionHandler] | None = None,
         guards: list[Guard] | None = None,
         middleware: list[Middleware] | None = None,
         receive_mode: WebSocketMode = "text",
         send_mode: WebSocketMode = "text",
         name: str | None = None,
         on_accept: AnyCallable | None = None,
         on_disconnect: AnyCallable | None = None,
         opt: dict[str, Any] | None = None,
-        return_dto: type[DTOInterface] | None | EmptyType = Empty,
+        return_dto: type[AbstractDTO] | None | EmptyType = Empty,
         signature_namespace: Mapping[str, Any] | None = None,
         type_encoders: TypeEncodersMap | None = None,
         **kwargs: Any,
     ) -> None:
         """Initialize ``WebsocketRouteHandler``
 
         Args:
@@ -151,87 +143,134 @@
                 to ``/``
             connection_accept_handler: A callable that accepts a :class:`WebSocket <.connection.WebSocket>` instance
                 and returns a coroutine that when awaited, will accept the connection. Defaults to ``WebSocket.accept``.
             connection_lifespan: An asynchronous context manager, handling the lifespan of the connection. By default,
                 it calls the ``connection_accept_handler``, ``on_connect`` and ``on_disconnect``. Can request any
                 dependencies, for example the :class:`WebSocket <.connection.WebSocket>` connection
             dependencies: A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances.
-            dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for (de)serializing and
+            dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for (de)serializing and
                 validation of request data.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
             guards: A sequence of :class:`Guard <.types.Guard>` callables.
             middleware: A sequence of :class:`Middleware <.types.Middleware>`.
             receive_mode: Websocket mode to receive data in, either `text` or `binary`.
             send_mode: Websocket mode to receive data in, either `text` or `binary`.
             name: A string identifying the route handler.
             on_accept: Callback invoked after a connection has been accepted. Can request any dependencies, for example
                 the :class:`WebSocket <.connection.WebSocket>` connection
             on_disconnect: Callback invoked after a connection has been closed. Can request any dependencies, for
                 example the :class:`WebSocket <.connection.WebSocket>` connection
             opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
                 wherever you have access to :class:`Request <.connection.Request>` or
                 :class:`ASGI Scope <.types.Scope>`.
-            return_dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for serializing
+            return_dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for serializing
                 outbound response data.
             signature_namespace: A mapping of names to types for use in forward reference resolution during signature
                 modelling.
             type_encoders: A mapping of types to callables that transform them into types supported for serialization.
             **kwargs: Any additional kwarg - will be set in the opt dictionary.
         """
         if connection_lifespan and any([on_accept, on_disconnect, connection_accept_handler is not WebSocket.accept]):
             raise ImproperlyConfiguredException(
                 "connection_lifespan can not be used with connection hooks "
                 "(on_accept, on_disconnect, connection_accept_handler)",
             )
-        self._listener_context = ListenerContext()
+
         self._receive_mode: WebSocketMode = receive_mode
         self._send_mode: WebSocketMode = send_mode
         self._connection_lifespan = connection_lifespan
+        self._send_handler: Callable[[WebSocket, Any], Coroutine[None, None, None]] | EmptyType = Empty
+        self._receive_handler: Callable[[WebSocket], Any] | EmptyType = Empty
 
         self.connection_accept_handler = connection_accept_handler
         self.on_accept = AsyncCallable(on_accept) if on_accept else None
         self.on_disconnect = AsyncCallable(on_disconnect) if on_disconnect else None
         self.type_encoders = type_encoders
 
+        listener_dependencies = dict(dependencies or {})
+
+        listener_dependencies["connection_lifespan_dependencies"] = create_stub_dependency(
+            connection_lifespan or self.default_connection_lifespan
+        )
+
+        if self.on_accept:
+            listener_dependencies["on_accept_dependencies"] = create_stub_dependency(self.on_accept.ref.value)
+
+        if self.on_disconnect:
+            listener_dependencies["on_disconnect_dependencies"] = create_stub_dependency(self.on_disconnect.ref.value)
+
         super().__init__(
             path=path,
-            dependencies=dependencies,
+            dependencies=listener_dependencies,
             exception_handlers=exception_handlers,
             guards=guards,
             middleware=middleware,
             name=name,
             opt=opt,
             signature_namespace=signature_namespace,
+            dto=dto,
+            return_dto=return_dto,
             **kwargs,
         )
 
-        # its important that this is assigned after the super() call
-        self.dto = dto
-        self.return_dto = return_dto
-
-        if not self.dependencies:
-            self.dependencies = {}
-
-        self.dependencies = dict(self.dependencies)
-        self.dependencies["connection_lifespan_dependencies"] = create_stub_dependency(
-            self._connection_lifespan or self.default_connection_lifespan
+    def __call__(self, fn: AnyCallable) -> Self:
+        parsed_signature = ParsedSignature.from_fn(fn, self.resolve_signature_namespace())
+
+        if "data" not in parsed_signature.parameters:
+            raise ImproperlyConfiguredException("Websocket listeners must accept a 'data' parameter")
+
+        for param in ("request", "body"):
+            if param in parsed_signature.parameters:
+                raise ImproperlyConfiguredException(f"The {param} kwarg is not supported with websocket listeners")
+
+        # we are manipulating the signature of the decorated function below, so we must store the original values for
+        # use elsewhere.
+        self._parsed_return_field = parsed_signature.return_type
+        self._parsed_data_field = parsed_signature.parameters.get("data")
+        self._parsed_fn_signature = ParsedSignature.from_signature(
+            create_handler_signature(parsed_signature.original_signature),
+            fn_type_hints={
+                **get_fn_type_hints(fn, namespace=self.resolve_signature_namespace()),
+                **get_fn_type_hints(ListenerHandler.__call__, namespace=self.resolve_signature_namespace()),
+            },
+        )
+
+        return super().__call__(
+            ListenerHandler(
+                listener=self, fn=fn, parsed_signature=parsed_signature, namespace=self.resolve_signature_namespace()
+            )
         )
 
-        if self.on_accept:
-            self.dependencies["on_accept_dependencies"] = create_stub_dependency(self.on_accept.ref.value)
+    def _validate_handler_function(self) -> None:
+        """Validate the route handler function once it's set by inspecting its return annotations."""
+        # validation occurs in the call method
 
-        if self.on_disconnect:
-            self.dependencies["on_disconnect_dependencies"] = create_stub_dependency(self.on_disconnect.ref.value)
+    @property
+    def signature_model(self) -> type[SignatureModel]:
+        """Get the signature model for the route handler.
+
+        Returns:
+            A signature model for the route handler.
+
+        """
+        if self._signature_model is Empty:
+            self._signature_model = SignatureModel.create(
+                dependency_name_set=self.dependency_name_set,
+                fn=cast("AnyCallable", self.fn.value),
+                parsed_signature=self.parsed_fn_signature,
+                type_decoders=self.resolve_type_decoders(),
+            )
+        return cast("type[SignatureModel]", self._signature_model)
 
     @asynccontextmanager
     async def default_connection_lifespan(
         self,
         socket: WebSocket,
-        on_accept_dependencies: Optional[Dict[str, Any]] = None,  # noqa: UP007, UP006
-        on_disconnect_dependencies: Optional[Dict[str, Any]] = None,  # noqa: UP007, UP006
+        on_accept_dependencies: Optional[Dict[str, Any]] = None,  # noqa: UP006, UP007
+        on_disconnect_dependencies: Optional[Dict[str, Any]] = None,  # noqa: UP006, UP007
     ) -> AsyncGenerator[None, None]:
         """Handle the connection lifespan of a :class:`WebSocket <.connection.WebSocket>`.
 
         Args:
             socket: The :class:`WebSocket <.connection.WebSocket>` connection
             on_accept_dependencies: Dependencies requested by the :attr:`on_accept` hook
             on_disconnect_dependencies: Dependencies requested by the :attr:`on_disconnect` hook
@@ -251,99 +290,35 @@
             yield
         except WebSocketDisconnect:
             pass
         finally:
             if self.on_disconnect:
                 await self.on_disconnect(**(on_disconnect_dependencies or {}))
 
-    def _validate_handler_function(self) -> None:
-        """Validate the route handler function once it's set by inspecting its return annotations."""
-        # since none of the validation rules of WebsocketRouteHandler apply here, this is let empty. Validation of the
-        # user supplied method happens at init time of this handler instead in __call__
-
-    def _init_handler_dtos(self) -> None:
-        """Initialize the data and return DTOs for the handler."""
-        if dto := self.resolve_dto():
-            data_parameter = self._listener_context.listener_callback_signature.parameters["data"]
-            dto.on_registration(HandlerContext(dto_for="data", handler_id=str(self), field_definition=data_parameter))
-
-        if return_dto := self.resolve_return_dto():
-            return_type = self._listener_context.listener_callback_signature.return_type
-            return_dto.on_registration(
-                HandlerContext(dto_for="return", handler_id=str(self), field_definition=return_type)
-            )
-
-    def __call__(self, listener_callback: AnyCallable) -> websocket_listener:
-        self._listener_context.listener_callback = listener_callback
-        self._listener_context.handler_function = handler_function = create_handler_function(
-            listener_context=self._listener_context,
-            lifespan_manager=self._connection_lifespan or self.default_connection_lifespan,
-        )
-        return super().__call__(handler_function)
+    def resolve_receive_handler(self) -> Callable[[WebSocket], Any]:
+        if self._receive_handler is Empty:
+            self._receive_handler = create_handle_receive(self)
+        return cast("Callable[[WebSocket], Any]", self._receive_handler)
+
+    def resolve_send_handler(self) -> Callable[[WebSocket, Any], Coroutine[None, None, None]]:
+        if self._send_handler is Empty:
+            self._send_handler = create_handle_send(self)
+        return cast("Callable[[WebSocket, Any], Coroutine[None, None, None]]", self._send_handler)
 
-    def on_registration(self, app: Litestar) -> None:
-        self._set_listener_context()
-        super().on_registration(app)
-
-    def _create_signature_model(self, app: Litestar) -> None:
-        """Create signature model for handler function."""
-        if not self.signature_model:
-            new_signature = create_handler_signature(
-                self._listener_context.listener_callback_signature.original_signature
-            )
-            self.signature_model = SignatureModel.create(
-                dependency_name_set=self.dependency_name_set,
-                fn=cast("AnyCallable", self.fn.value),
-                parsed_signature=ParsedSignature.from_signature(new_signature, self.resolve_signature_namespace()),
-            )
 
-    def _set_listener_context(self) -> None:
-        listener_callback_signature = ParsedSignature.from_fn(
-            self._listener_context.listener_callback, self.resolve_signature_namespace()
-        )
-
-        if "data" not in listener_callback_signature.parameters:
-            raise ImproperlyConfiguredException("Websocket listeners must accept a 'data' parameter")
-
-        for param in ("request", "body"):
-            if param in listener_callback_signature.parameters:
-                raise ImproperlyConfiguredException(f"The {param} kwarg is not supported with websocket listeners")
-
-        resolved_data_dto = self.resolve_dto()
-        resolved_return_dto = self.resolve_return_dto()
-
-        self._listener_context.listener_callback_signature = listener_callback_signature
-        self._listener_context.can_send_data = not listener_callback_signature.return_type.is_subclass_of(NoneType)
-        self._listener_context.pass_socket = "socket" in listener_callback_signature.parameters
-        self._listener_context.resolved_data_dto = resolved_data_dto
-        self._listener_context.resolved_return_dto = resolved_return_dto
-        self._listener_context.handle_receive = create_handle_receive(
-            resolved_data_dto, self._receive_mode, listener_callback_signature.parameters["data"].annotation
-        )
-        should_encode_to_json = not (
-            listener_callback_signature.return_type.is_subclass_of((str, bytes))
-            or (
-                listener_callback_signature.return_type.is_optional
-                and listener_callback_signature.return_type.has_inner_subclass_of((str, bytes))
-            )
-        )
-        json_encoder = JsonEncoder(enc_hook=partial(default_serializer, type_encoders=self.resolve_type_encoders()))
-
-        self._listener_context.handle_send = create_handle_send(
-            resolved_return_dto, json_encoder, should_encode_to_json, self._send_mode
-        )
+websocket_listener = WebsocketListenerRouteHandler
 
 
 class WebsocketListener(ABC):
     path: str | None | list[str] | None = None
     """A path fragment for the route handler function or a sequence of path fragments. If not given defaults to ``/``"""
     dependencies: Dependencies | None = None
     """A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances."""
-    dto: type[DTOInterface] | None | EmptyType = Empty
-    """:class:`DTOInterface <.dto.interface.DTOInterface>` to use for (de)serializing and validation of request data"""
+    dto: type[AbstractDTO] | None | EmptyType = Empty
+    """:class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for (de)serializing and validation of request data"""
     exception_handlers: dict[int | type[Exception], ExceptionHandler] | None = None
     """A mapping of status codes and/or exception types to handler functions."""
     guards: list[Guard] | None = None
     """A sequence of :class:`Guard <.types.Guard>` callables."""
     middleware: list[Middleware] | None = None
     """A sequence of :class:`Middleware <.types.Middleware>`."""
     on_accept: AnyCallable | None = None
@@ -357,16 +332,16 @@
     name: str | None = None
     """A string identifying the route handler."""
     opt: dict[str, Any] | None = None
     """
     A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or wherever you
     have access to :class:`Request <.connection.Request>` or :class:`ASGI Scope <.types.Scope>`.
     """
-    return_dto: type[DTOInterface] | None | EmptyType = Empty
-    """:class:`DTOInterface <.dto.interface.DTOInterface>` to use for serializing outbound response data."""
+    return_dto: type[AbstractDTO] | None | EmptyType = Empty
+    """:class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for serializing outbound response data."""
     signature_namespace: Mapping[str, Any] | None = None
     """
     A mapping of names to types for use in forward reference resolution during signature modelling.
     """
     type_encoders: TypeEncodersMap | None = None
     """
     type_encoders: A mapping of types to callables that transform them into types supported for serialization.
@@ -376,16 +351,16 @@
         """Initialize a WebsocketListener instance.
 
         Args:
             owner: The :class:`Router <.router.Router>` instance that owns this listener.
         """
         self._owner = owner
 
-    def to_handler(self) -> websocket_listener:
-        handler = websocket_listener(
+    def to_handler(self) -> WebsocketListenerRouteHandler:
+        handler = WebsocketListenerRouteHandler(
             dependencies=self.dependencies,
             dto=self.dto,
             exception_handlers=self.exception_handlers,
             guards=self.guards,
             middleware=self.middleware,
             send_mode=self.send_mode,
             receive_mode=self.receive_mode,
```

### Comparing `litestar-2.0.0b4/litestar/handlers/websocket_handlers/route_handler.py` & `litestar-2.0.0rc1/litestar/handlers/websocket_handlers/route_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 
 class WebsocketRouteHandler(BaseRouteHandler):
     """Websocket route handler decorator.
 
     Use this decorator to decorate websocket handler functions.
     """
 
-    __slots__ = ()
-
     def __init__(
         self,
         path: str | None | list[str] | None = None,
         *,
         dependencies: Dependencies | None = None,
         exception_handlers: dict[int | type[Exception], ExceptionHandler] | None = None,
         guards: list[Guard] | None = None,
@@ -64,17 +62,20 @@
 
     def _validate_handler_function(self) -> None:
         """Validate the route handler function once it's set by inspecting its return annotations."""
         super()._validate_handler_function()
 
         if not self.parsed_fn_signature.return_type.is_subclass_of(NoneType):
             raise ImproperlyConfiguredException("Websocket handler functions should return 'None'")
+
         if "socket" not in self.parsed_fn_signature.parameters:
             raise ImproperlyConfiguredException("Websocket handlers must set a 'socket' kwarg")
+
         for param in ("request", "body", "data"):
             if param in self.parsed_fn_signature.parameters:
                 raise ImproperlyConfiguredException(f"The {param} kwarg is not supported with websocket handlers")
+
         if not is_async_callable(self.fn.value):
             raise ImproperlyConfiguredException("Functions decorated with 'websocket' must be async functions")
 
 
 websocket = WebsocketRouteHandler
```

### Comparing `litestar-2.0.0b4/litestar/logging/_utils.py` & `litestar-2.0.0rc1/litestar/logging/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/logging/config.py` & `litestar-2.0.0rc1/litestar/logging/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/logging/picologging.py` & `litestar-2.0.0rc1/litestar/logging/picologging.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/logging/standard.py` & `litestar-2.0.0rc1/litestar/logging/standard.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/middleware/_utils.py` & `litestar-2.0.0rc1/litestar/middleware/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/middleware/allowed_hosts.py` & `litestar-2.0.0rc1/litestar/middleware/allowed_hosts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/middleware/authentication.py` & `litestar-2.0.0rc1/litestar/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/middleware/base.py` & `litestar-2.0.0rc1/litestar/middleware/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/middleware/compression.py` & `litestar-2.0.0rc1/litestar/middleware/compression.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/middleware/cors.py` & `litestar-2.0.0rc1/litestar/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/middleware/csrf.py` & `litestar-2.0.0rc1/litestar/middleware/csrf.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/middleware/exceptions/_debug_response.py` & `litestar-2.0.0rc1/litestar/middleware/exceptions/_debug_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from html import escape
 from inspect import getinnerframes
 from pathlib import Path
 from traceback import format_exception
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 from litestar.enums import MediaType
 from litestar.response import Response
 from litestar.status_codes import HTTP_500_INTERNAL_SERVER_ERROR
 from litestar.utils import get_name
 
 __all__ = (
@@ -176,15 +176,18 @@
     Args:
         request: A :class:`Request <litestar.connection.Request>` instance.
         exc: An Exception instance to render debug response from.
 
     Returns:
         A response with a rendered exception traceback.
     """
-    if "text/html" in request.headers.get("accept", ""):
-        content = create_html_response_content(exc=exc, request=request)
+    if MediaType.HTML in request.headers.get("accept", ""):
+        content: Any = create_html_response_content(exc=exc, request=request)
         media_type = MediaType.HTML
+    elif MediaType.JSON in request.headers.get("accept", ""):
+        content = {"details": create_plain_text_response_content(exc), "status_code": HTTP_500_INTERNAL_SERVER_ERROR}
+        media_type = MediaType.JSON
     else:
         content = create_plain_text_response_content(exc)
         media_type = MediaType.TEXT
 
     return Response(content=content, media_type=media_type, status_code=HTTP_500_INTERNAL_SERVER_ERROR)
```

### Comparing `litestar-2.0.0b4/litestar/middleware/exceptions/middleware.py` & `litestar-2.0.0rc1/litestar/middleware/exceptions/middleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,17 +51,19 @@
         exc: Exception Instance to be resolved to a handler.
 
     Returns:
         Optional exception handler callable.
     """
     if not exception_handlers:
         return None
+
     status_code: int | None = getattr(exc, "status_code", None)
     if status_code and (exception_handler := exception_handlers.get(status_code)):
         return exception_handler
+
     return next(
         (exception_handlers[cast("Type[Exception]", cls)] for cls in getmro(type(exc)) if cls in exception_handlers),
         exception_handlers[HTTP_500_INTERNAL_SERVER_ERROR]
         if not hasattr(exc, "status_code") and HTTP_500_INTERNAL_SERVER_ERROR in exception_handlers
         else None,
     )
 
@@ -213,14 +215,15 @@
         """
         if isinstance(exc, WebSocketException):
             code = exc.code
             reason = exc.detail
         else:
             code = 4000 + getattr(exc, "status_code", HTTP_500_INTERNAL_SERVER_ERROR)
             reason = getattr(exc, "detail", repr(exc))
+
         event: WebSocketCloseEvent = {"type": "websocket.close", "code": code, "reason": reason}
         await send(event)
 
     def default_http_exception_handler(self, request: Request, exc: Exception) -> Response[Any]:
         """Handle an HTTP exception by returning the appropriate response.
 
         Args:
```

### Comparing `litestar-2.0.0b4/litestar/middleware/exceptions/templates/scripts.js` & `litestar-2.0.0rc1/litestar/middleware/exceptions/templates/scripts.js`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/middleware/exceptions/templates/styles.css` & `litestar-2.0.0rc1/litestar/middleware/exceptions/templates/styles.css`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/middleware/logging.py` & `litestar-2.0.0rc1/litestar/middleware/logging.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/middleware/rate_limit.py` & `litestar-2.0.0rc1/litestar/middleware/rate_limit.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/middleware/session/base.py` & `litestar-2.0.0rc1/litestar/middleware/session/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/middleware/session/client_side.py` & `litestar-2.0.0rc1/litestar/middleware/session/client_side.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/middleware/session/server_side.py` & `litestar-2.0.0rc1/litestar/middleware/session/server_side.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,17 @@
             headers.add(
                 "Set-Cookie",
                 Cookie(value="null", key=self.config.key, expires=0, **cookie_params).to_header(header=""),
             )
         else:
             serialised_data = self.serialize_data(scope_session, scope)
             await self.set(session_id=session_id, data=serialised_data, store=store)
-            headers["Set-Cookie"] = Cookie(value=session_id, key=self.config.key, **cookie_params).to_header(header="")
+            headers.add(
+                "Set-Cookie", Cookie(value=session_id, key=self.config.key, **cookie_params).to_header(header="")
+            )
 
     async def load_from_connection(self, connection: ASGIConnection) -> dict[str, Any]:
         """Load session data from a connection and return it as a dictionary to be used in the current application
         scope.
 
         The session-ID will be gathered from a cookie with the key set in
         :attr:`BaseBackendConfig.key`. If a cookie is found, its value will be used as the session-ID and data associated
```

### Comparing `litestar-2.0.0b4/litestar/openapi/config.py` & `litestar-2.0.0rc1/litestar/openapi/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/controller.py` & `litestar-2.0.0rc1/litestar/openapi/controller.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/datastructures.py` & `litestar-2.0.0rc1/litestar/openapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/__init__.py` & `litestar-2.0.0rc1/litestar/openapi/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/base.py` & `litestar-2.0.0rc1/litestar/openapi/spec/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/callback.py` & `litestar-2.0.0rc1/litestar/openapi/spec/callback.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/components.py` & `litestar-2.0.0rc1/litestar/openapi/spec/components.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/contact.py` & `litestar-2.0.0rc1/litestar/openapi/spec/contact.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/discriminator.py` & `litestar-2.0.0rc1/litestar/openapi/spec/discriminator.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/encoding.py` & `litestar-2.0.0rc1/litestar/openapi/spec/encoding.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/enums.py` & `litestar-2.0.0rc1/litestar/openapi/spec/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/example.py` & `litestar-2.0.0rc1/litestar/openapi/spec/example.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/external_documentation.py` & `litestar-2.0.0rc1/litestar/openapi/spec/external_documentation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/header.py` & `litestar-2.0.0rc1/litestar/openapi/spec/header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/info.py` & `litestar-2.0.0rc1/litestar/openapi/spec/info.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/license.py` & `litestar-2.0.0rc1/litestar/openapi/spec/license.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/link.py` & `litestar-2.0.0rc1/litestar/openapi/spec/link.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/media_type.py` & `litestar-2.0.0rc1/litestar/openapi/spec/media_type.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/oauth_flow.py` & `litestar-2.0.0rc1/litestar/openapi/spec/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/oauth_flows.py` & `litestar-2.0.0rc1/litestar/openapi/spec/oauth_flows.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/open_api.py` & `litestar-2.0.0rc1/litestar/openapi/spec/open_api.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/operation.py` & `litestar-2.0.0rc1/litestar/openapi/spec/operation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/parameter.py` & `litestar-2.0.0rc1/litestar/openapi/spec/parameter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/path_item.py` & `litestar-2.0.0rc1/litestar/openapi/spec/path_item.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/paths.py` & `litestar-2.0.0rc1/litestar/openapi/spec/paths.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/reference.py` & `litestar-2.0.0rc1/litestar/openapi/spec/reference.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/request_body.py` & `litestar-2.0.0rc1/litestar/openapi/spec/request_body.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/response.py` & `litestar-2.0.0rc1/litestar/openapi/spec/response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/responses.py` & `litestar-2.0.0rc1/litestar/openapi/spec/responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/schema.py` & `litestar-2.0.0rc1/litestar/openapi/spec/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/security_requirement.py` & `litestar-2.0.0rc1/litestar/openapi/spec/security_requirement.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/security_scheme.py` & `litestar-2.0.0rc1/litestar/openapi/spec/security_scheme.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/server.py` & `litestar-2.0.0rc1/litestar/openapi/spec/server.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/server_variable.py` & `litestar-2.0.0rc1/litestar/openapi/spec/server_variable.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/tag.py` & `litestar-2.0.0rc1/litestar/openapi/spec/tag.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/openapi/spec/xml.py` & `litestar-2.0.0rc1/litestar/openapi/spec/xml.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/pagination.py` & `litestar-2.0.0rc1/litestar/pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/params.py` & `litestar-2.0.0rc1/litestar/params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/response/base.py` & `litestar-2.0.0rc1/litestar/response/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,15 +410,14 @@
             type_encoders = self.response_type_encoders
 
         media_type = get_enum_string_value(self.media_type or media_type or MediaType.JSON)
 
         return ASGIResponse(
             background=self.background or background,
             body=self.render(self.content, media_type, get_serializer(type_encoders)),
-            content_length=None,
             cookies=cookies,
             encoded_headers=encoded_headers or [],
             encoding=self.encoding,
             headers=headers,
             is_head_response=is_head_response,
             media_type=media_type,
             status_code=self.status_code or status_code,
```

### Comparing `litestar-2.0.0b4/litestar/response/file.py` & `litestar-2.0.0rc1/litestar/response/file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/response/redirect.py` & `litestar-2.0.0rc1/litestar/response/redirect.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/response/streaming.py` & `litestar-2.0.0rc1/litestar/response/streaming.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/response/template.py` & `litestar-2.0.0rc1/litestar/response/template.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/router.py` & `litestar-2.0.0rc1/litestar/router.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from litestar.utils.sync import AsyncCallable
 
 __all__ = ("Router",)
 
 
 if TYPE_CHECKING:
     from litestar.datastructures import CacheControlHeader, ETag
-    from litestar.dto.interface import DTOInterface
+    from litestar.dto import AbstractDTO
     from litestar.openapi.spec import SecurityRequirement
     from litestar.routes import BaseRoute
     from litestar.types import (
         AfterRequestHookHandler,
         AfterResponseHookHandler,
         BeforeRequestHookHandler,
         ControllerRouterHandler,
@@ -81,25 +81,25 @@
         path: str,
         *,
         after_request: AfterRequestHookHandler | None = None,
         after_response: AfterResponseHookHandler | None = None,
         before_request: BeforeRequestHookHandler | None = None,
         cache_control: CacheControlHeader | None = None,
         dependencies: Dependencies | None = None,
-        dto: type[DTOInterface] | None | EmptyType = Empty,
+        dto: type[AbstractDTO] | None | EmptyType = Empty,
         etag: ETag | None = None,
         exception_handlers: ExceptionHandlersMap | None = None,
         guards: Sequence[Guard] | None = None,
         middleware: Sequence[Middleware] | None = None,
         opt: Mapping[str, Any] | None = None,
         parameters: ParametersMap | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: ResponseHeaders | None = None,
-        return_dto: type[DTOInterface] | None | EmptyType = Empty,
+        return_dto: type[AbstractDTO] | None | EmptyType = Empty,
         route_handlers: Sequence[ControllerRouterHandler],
         security: Sequence[SecurityRequirement] | None = None,
         signature_namespace: Mapping[str, Any] | None = None,
         tags: Sequence[str] | None = None,
         type_encoders: TypeEncodersMap | None = None,
         type_decoders: TypeDecodersSequence | None = None,
     ) -> None:
@@ -114,15 +114,15 @@
             before_request: A sync or async function called immediately before calling the route handler. Receives
                 the :class:`litestar.connection.Request` instance and any non-``None`` return value is used for the
                 response, bypassing the route handler.
             cache_control: A ``cache-control`` header of type
                 :class:`CacheControlHeader <.datastructures.CacheControlHeader>` to add to route handlers of
                 this router. Can be overridden by route handlers.
             dependencies: A string keyed mapping of dependency :class:`Provide <.di.Provide>` instances.
-            dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for (de)serializing and
+            dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for (de)serializing and
                 validation of request data.
             etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` to add to route handlers of this app.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
             guards: A sequence of :data:`Guard <.types.Guard>` callables.
             middleware: A sequence of :data:`Middleware <.types.Middleware>`.
             opt: A string keyed mapping of arbitrary values that can be accessed in :data:`Guards <.types.Guard>` or
                 wherever you have access to :class:`Request <.connection.Request>` or
@@ -132,15 +132,15 @@
             path: A path fragment that is prefixed to all route handlers, controllers and other routers associated
                 with the router instance.
             response_class: A custom subclass of :class:`Response <.response.Response>` to be used as the default for
                 all route handlers, controllers and other routers associated with the router instance.
             response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>` instances.
             response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
                 instances.
-            return_dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for serializing
+            return_dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for serializing
                 outbound response data.
             route_handlers: A required sequence of route handlers, which can include instances of
                 :class:`Router <.router.Router>`, subclasses of :class:`Controller <.controller.Controller>` or any
                 function decorated by the route handler decorators.
             security: A sequence of dicts that will be added to the schema of all route handlers in the application.
                 See :data:`SecurityRequirement <.openapi.spec.SecurityRequirement>`
                 for details.
```

### Comparing `litestar-2.0.0b4/litestar/routes/asgi.py` & `litestar-2.0.0rc1/litestar/routes/asgi.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/routes/base.py` & `litestar-2.0.0rc1/litestar/routes/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable
 from uuid import UUID
 
 import msgspec
 
 from litestar._kwargs import KwargsModel
-from litestar._signature import get_signature_model
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.types.internal_types import PathParameterDefinition
 from litestar.utils import join_paths, normalize_path
 
 if TYPE_CHECKING:
     from litestar.enums import ScopeType
     from litestar.handlers.base import BaseRouteHandler
@@ -130,20 +129,19 @@
         path_parameters = set()
         for param in self.path_parameters:
             if param.name in path_parameters:
                 raise ImproperlyConfiguredException(f"Duplicate parameter '{param.name}' detected in '{self.path}'.")
             path_parameters.add(param.name)
 
         return KwargsModel.create_for_signature_model(
-            signature_model=get_signature_model(route_handler),
+            signature_model=route_handler.signature_model,
             parsed_signature=route_handler.parsed_fn_signature,
             dependencies=route_handler.resolve_dependencies(),
             path_parameters=path_parameters,
             layered_parameters=route_handler.resolve_layered_parameters(),
-            data_dto=route_handler.resolve_dto(),
         )
 
     @staticmethod
     def _validate_path_parameter(param: str, path: str) -> None:
         """Validate that a path parameter adheres to the required format and datatypes.
 
         Raises:
```

### Comparing `litestar-2.0.0b4/litestar/routes/http.py` & `litestar-2.0.0rc1/litestar/routes/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,17 @@
         Args:
             path: The path for the route.
             route_handlers: A list of :class:`~.handlers.HTTPRouteHandler`.
         """
         methods = list(chain.from_iterable([route_handler.http_methods for route_handler in route_handlers]))
         if "OPTIONS" not in methods:
             methods.append("OPTIONS")
-            route_handlers.append(self.create_options_handler(path))
+            options_handler = self.create_options_handler(path)
+            options_handler.owner = route_handlers[0].owner
+            route_handlers.append(options_handler)
 
         self.route_handlers = route_handlers
         self.route_handler_map: dict[Method, tuple[HTTPRouteHandler, KwargsModel]] = {}
 
         super().__init__(
             methods=methods,
             path=path,
```

### Comparing `litestar-2.0.0b4/litestar/routes/websocket.py` & `litestar-2.0.0rc1/litestar/routes/websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/security/base.py` & `litestar-2.0.0rc1/litestar/security/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/security/session_auth/auth.py` & `litestar-2.0.0rc1/litestar/security/session_auth/auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/security/session_auth/middleware.py` & `litestar-2.0.0rc1/litestar/security/session_auth/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/serialization/msgspec_hooks.py` & `litestar-2.0.0rc1/litestar/serialization/msgspec_hooks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/static_files/base.py` & `litestar-2.0.0rc1/litestar/static_files/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -105,16 +105,19 @@
                 filename=filename,
                 content_disposition_type=content_disposition_type,
                 is_head_response=scope["method"] == "HEAD",
             )(scope, receive, send)
             return
 
         if self.is_html_mode:
-            filename = "404.html"
-            resolved_path, fs_info = await self.get_fs_info(directories=self.directories, file_path=filename)
+            # for some reason coverage doesn't catch these two lines
+            filename = "404.html"  # pragma: no cover
+            resolved_path, fs_info = await self.get_fs_info(  # pragma: no cover
+                directories=self.directories, file_path=filename
+            )
 
             if fs_info and fs_info["type"] == "file":
                 await ASGIFileResponse(
                     file_path=resolved_path or joined_path,
                     file_info=fs_info,
                     file_system=self.adapter.file_system,
                     filename=filename,
```

### Comparing `litestar-2.0.0b4/litestar/static_files/config.py` & `litestar-2.0.0rc1/litestar/static_files/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/status_codes.py` & `litestar-2.0.0rc1/litestar/status_codes.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/stores/base.py` & `litestar-2.0.0rc1/litestar/stores/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/stores/file.py` & `litestar-2.0.0rc1/litestar/stores/file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/stores/memory.py` & `litestar-2.0.0rc1/litestar/stores/memory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/stores/redis.py` & `litestar-2.0.0rc1/litestar/stores/redis.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/stores/registry.py` & `litestar-2.0.0rc1/litestar/stores/registry.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/template/base.py` & `litestar-2.0.0rc1/litestar/template/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/template/config.py` & `litestar-2.0.0rc1/litestar/template/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/testing/__init__.py` & `litestar-2.0.0rc1/litestar/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/testing/client/__init__.py` & `litestar-2.0.0rc1/litestar/testing/client/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/testing/client/async_client.py` & `litestar-2.0.0rc1/litestar/testing/client/async_client.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/testing/client/base.py` & `litestar-2.0.0rc1/litestar/testing/client/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/testing/client/sync_client.py` & `litestar-2.0.0rc1/litestar/testing/client/sync_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         Client.__init__(
             self,
             app=self.app,
             base_url=base_url,
             headers={"user-agent": "testclient"},
             follow_redirects=True,
             cookies=cookies,
-            transport=TestClientTransport(  # type: ignore [arg-type]
+            transport=TestClientTransport(  # type: ignore[arg-type]
                 client=self,
                 raise_server_exceptions=raise_server_exceptions,
                 root_path=root_path,
             ),
             timeout=timeout,
         )
```

### Comparing `litestar-2.0.0b4/litestar/testing/helpers.py` & `litestar-2.0.0rc1/litestar/testing/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     from litestar import Request, WebSocket
     from litestar.config.allowed_hosts import AllowedHostsConfig
     from litestar.config.compression import CompressionConfig
     from litestar.config.cors import CORSConfig
     from litestar.config.csrf import CSRFConfig
     from litestar.config.response_cache import ResponseCacheConfig
     from litestar.datastructures import CacheControlHeader, ETag, ResponseHeader, State
-    from litestar.dto.interface import DTOInterface
+    from litestar.dto import AbstractDTO
     from litestar.events import BaseEventEmitterBackend, EventListener
     from litestar.logging.config import BaseLoggingConfig
     from litestar.middleware.session.base import BaseBackendConfig
     from litestar.openapi.config import OpenAPIConfig
     from litestar.openapi.spec import SecurityRequirement
     from litestar.plugins import PluginProtocol
     from litestar.static_files.config import StaticFilesConfig
@@ -64,17 +64,17 @@
     base_url: str = "http://testserver.local",
     before_request: BeforeRequestHookHandler | None = None,
     before_send: OptionalSequence[BeforeMessageSendHookHandler] | None = None,
     cache_control: CacheControlHeader | None = None,
     compression_config: CompressionConfig | None = None,
     cors_config: CORSConfig | None = None,
     csrf_config: CSRFConfig | None = None,
-    debug: bool = False,
+    debug: bool = True,
     dependencies: Dependencies | None = None,
-    dto: type[DTOInterface] | None | EmptyType = Empty,
+    dto: type[AbstractDTO] | None | EmptyType = Empty,
     etag: ETag | None = None,
     event_emitter_backend: type[BaseEventEmitterBackend] = SimpleEventEmitter,
     exception_handlers: ExceptionHandlersMap | None = None,
     guards: OptionalSequence[Guard] | None = None,
     listeners: OptionalSequence[EventListener] | None = None,
     logging_config: BaseLoggingConfig | EmptyType | None = Empty,
     middleware: OptionalSequence[Middleware] | None = None,
@@ -90,15 +90,15 @@
     raise_server_exceptions: bool = True,
     pdb_on_exception: bool | None = None,
     request_class: type[Request] | None = None,
     response_cache_config: ResponseCacheConfig | None = None,
     response_class: ResponseType | None = None,
     response_cookies: ResponseCookies | None = None,
     response_headers: OptionalSequence[ResponseHeader] | None = None,
-    return_dto: type[DTOInterface] | None | EmptyType = Empty,
+    return_dto: type[AbstractDTO] | None | EmptyType = Empty,
     root_path: str = "",
     security: OptionalSequence[SecurityRequirement] | None = None,
     session_config: BaseBackendConfig | None = None,
     signature_namespace: Mapping[str, Any] | None = None,
     state: State | None = None,
     static_files_config: OptionalSequence[StaticFilesConfig] | None = None,
     stores: StoreRegistry | dict[str, Store] | None = None,
@@ -163,15 +163,15 @@
             this app. Can be overridden by route handlers.
         compression_config: Configures compression behaviour of the application, this enabled a builtin or user
             defined Compression middleware.
         cors_config: If set, configures :class:`CORSMiddleware <.middleware.cors.CORSMiddleware>`.
         csrf_config: If set, configures :class:`CSRFMiddleware <.middleware.csrf.CSRFMiddleware>`.
         debug: If ``True``, app errors rendered as HTML with a stack trace.
         dependencies: A string keyed mapping of dependency :class:`Providers <.di.Provide>`.
-        dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for (de)serializing and
+        dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for (de)serializing and
             validation of request data.
         etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` to add to route handlers of this app.
             Can be overridden by route handlers.
         event_emitter_backend: A subclass of
             :class:`BaseEventEmitterBackend <.events.emitter.BaseEventEmitterBackend>`.
         exception_handlers: A mapping of status codes and/or exception types to handler functions.
         guards: A sequence of :class:`Guard <.types.Guard>` callables.
@@ -199,15 +199,15 @@
         plugins: Sequence of plugins.
         request_class: An optional subclass of :class:`Request <.connection.Request>` to use for http connections.
         response_class: A custom subclass of :class:`Response <.response.Response>` to be used as the app's default
             response.
         response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>`.
         response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
         response_cache_config: Configures caching behavior of the application.
-        return_dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for serializing
+        return_dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for serializing
             outbound response data.
         route_handlers: A sequence of route handlers, which can include instances of
             :class:`Router <.router.Router>`, subclasses of :class:`Controller <.controller.Controller>` or any
             callable decorated by the route handler decorators.
         security: A sequence of dicts that will be added to the schema of all route handlers in the application.
             See
             :data:`SecurityRequirement <.openapi.spec.SecurityRequirement>` for details.
@@ -306,17 +306,17 @@
     base_url: str = "http://testserver.local",
     before_request: BeforeRequestHookHandler | None = None,
     before_send: OptionalSequence[BeforeMessageSendHookHandler] | None = None,
     cache_control: CacheControlHeader | None = None,
     compression_config: CompressionConfig | None = None,
     cors_config: CORSConfig | None = None,
     csrf_config: CSRFConfig | None = None,
-    debug: bool = False,
+    debug: bool = True,
     dependencies: Dependencies | None = None,
-    dto: type[DTOInterface] | None | EmptyType = Empty,
+    dto: type[AbstractDTO] | None | EmptyType = Empty,
     etag: ETag | None = None,
     event_emitter_backend: type[BaseEventEmitterBackend] = SimpleEventEmitter,
     exception_handlers: ExceptionHandlersMap | None = None,
     guards: OptionalSequence[Guard] | None = None,
     lifespan: list[Callable[[Litestar], AbstractAsyncContextManager] | AbstractAsyncContextManager] | None = None,
     listeners: OptionalSequence[EventListener] | None = None,
     logging_config: BaseLoggingConfig | EmptyType | None = Empty,
@@ -332,15 +332,15 @@
     plugins: OptionalSequence[PluginProtocol] | None = None,
     raise_server_exceptions: bool = True,
     request_class: type[Request] | None = None,
     response_cache_config: ResponseCacheConfig | None = None,
     response_class: ResponseType | None = None,
     response_cookies: ResponseCookies | None = None,
     response_headers: OptionalSequence[ResponseHeader] | None = None,
-    return_dto: type[DTOInterface] | None | EmptyType = Empty,
+    return_dto: type[AbstractDTO] | None | EmptyType = Empty,
     root_path: str = "",
     security: OptionalSequence[SecurityRequirement] | None = None,
     session_config: BaseBackendConfig | None = None,
     signature_namespace: Mapping[str, Any] | None = None,
     state: State | None = None,
     static_files_config: OptionalSequence[StaticFilesConfig] | None = None,
     stores: StoreRegistry | dict[str, Store] | None = None,
@@ -405,15 +405,15 @@
             this app. Can be overridden by route handlers.
         compression_config: Configures compression behaviour of the application, this enabled a builtin or user
             defined Compression middleware.
         cors_config: If set, configures :class:`CORSMiddleware <.middleware.cors.CORSMiddleware>`.
         csrf_config: If set, configures :class:`CSRFMiddleware <.middleware.csrf.CSRFMiddleware>`.
         debug: If ``True``, app errors rendered as HTML with a stack trace.
         dependencies: A string keyed mapping of dependency :class:`Providers <.di.Provide>`.
-        dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for (de)serializing and
+        dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for (de)serializing and
             validation of request data.
         etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` to add to route handlers of this app.
             Can be overridden by route handlers.
         event_emitter_backend: A subclass of
             :class:`BaseEventEmitterBackend <.events.emitter.BaseEventEmitterBackend>`.
         exception_handlers: A mapping of status codes and/or exception types to handler functions.
         guards: A sequence of :class:`Guard <.types.Guard>` callables.
@@ -441,15 +441,15 @@
         plugins: Sequence of plugins.
         request_class: An optional subclass of :class:`Request <.connection.Request>` to use for http connections.
         response_class: A custom subclass of :class:`Response <.response.Response>` to be used as the app's default
             response.
         response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>`.
         response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
         response_cache_config: Configures caching behavior of the application.
-        return_dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for serializing
+        return_dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for serializing
             outbound response data.
         route_handlers: A sequence of route handlers, which can include instances of
             :class:`Router <.router.Router>`, subclasses of :class:`Controller <.controller.Controller>` or any
             callable decorated by the route handler decorators.
         security: A sequence of dicts that will be added to the schema of all route handlers in the application.
             See
             :data:`SecurityRequirement <.openapi.spec.SecurityRequirement>` for details.
```

### Comparing `litestar-2.0.0b4/litestar/testing/life_span_handler.py` & `litestar-2.0.0rc1/litestar/testing/life_span_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,29 +42,35 @@
         await self.stream_receive.send(event)
 
         message = await self.receive()
         if message["type"] not in (
             "lifespan.startup.complete",
             "lifespan.startup.failed",
         ):
-            raise AssertionError
+            raise RuntimeError(
+                "Received unexpected ASGI message type. Expected 'lifespan.startup.complete' or "
+                f"'lifespan.startup.failed'. Got {message['type']!r}",
+            )
         if message["type"] == "lifespan.startup.failed":
             await self.receive()
 
     async def wait_shutdown(self) -> None:
         async with self.stream_send:
             lifespan_shutdown_event: LifeSpanShutdownEvent = {"type": "lifespan.shutdown"}
             await self.stream_receive.send(lifespan_shutdown_event)
 
             message = await self.receive()
             if message["type"] not in (
                 "lifespan.shutdown.complete",
                 "lifespan.shutdown.failed",
             ):
-                raise AssertionError
+                raise RuntimeError(
+                    "Received unexpected ASGI message type. Expected 'lifespan.shutdown.complete' or "
+                    f"'lifespan.shutdown.failed'. Got {message['type']!r}",
+                )
             if message["type"] == "lifespan.shutdown.failed":
                 await self.receive()
 
     async def lifespan(self) -> None:
         scope = {"type": "lifespan"}
         try:
             await self.client.app(scope, self.stream_receive.receive, self.stream_send.send)
```

### Comparing `litestar-2.0.0b4/litestar/testing/request_factory.py` & `litestar-2.0.0rc1/litestar/testing/request_factory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/testing/transport.py` & `litestar-2.0.0rc1/litestar/testing/transport.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/testing/websocket_test_session.py` & `litestar-2.0.0rc1/litestar/testing/websocket_test_session.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/types/__init__.py` & `litestar-2.0.0rc1/litestar/types/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/types/asgi_types.py` & `litestar-2.0.0rc1/litestar/types/asgi_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/types/builtin_types.py` & `litestar-2.0.0rc1/litestar/types/builtin_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/types/callable_types.py` & `litestar-2.0.0rc1/litestar/types/callable_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/types/composite_types.py` & `litestar-2.0.0rc1/litestar/types/composite_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     "PathType",
     "ResponseCookies",
     "ResponseHeaders",
     "Scopes",
     "TypeEncodersMap",
 )
 
+
 if TYPE_CHECKING:
     from os import PathLike
     from pathlib import Path
 
     from typing_extensions import TypeAlias
 
     from litestar.datastructures.cookie import Cookie
```

### Comparing `litestar-2.0.0b4/litestar/types/file_types.py` & `litestar-2.0.0rc1/litestar/types/file_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/types/helper_types.py` & `litestar-2.0.0rc1/litestar/types/helper_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/types/internal_types.py` & `litestar-2.0.0rc1/litestar/types/internal_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/types/protocols.py` & `litestar-2.0.0rc1/litestar/types/protocols.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/types/serialization.py` & `litestar-2.0.0rc1/litestar/types/serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/utils/__init__.py` & `litestar-2.0.0rc1/litestar/utils/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,25 +27,24 @@
 )
 from .scope import (
     delete_litestar_scope_state,
     get_litestar_scope_state,
     get_serializer_from_scope,
     set_litestar_scope_state,
 )
-from .sequence import compact, find_index, unique
+from .sequence import find_index, unique
 from .sync import AsyncCallable, AsyncIteratorWrapper, async_partial
 from .typing import annotation_is_iterable_of_type, get_origin_or_inner_type, make_non_optional_union
 
 __all__ = (
     "AsyncCallable",
     "AsyncIteratorWrapper",
     "Ref",
     "annotation_is_iterable_of_type",
     "async_partial",
-    "compact",
     "delete_litestar_scope_state",
     "deprecated",
     "encode_headers",
     "find_index",
     "get_enum_string_value",
     "get_litestar_scope_state",
     "get_name",
```

### Comparing `litestar-2.0.0b4/litestar/utils/compat.py` & `litestar-2.0.0rc1/litestar/utils/compat.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/utils/dataclass.py` & `litestar-2.0.0rc1/litestar/utils/dataclass.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/utils/deprecation.py` & `litestar-2.0.0rc1/litestar/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/utils/helpers.py` & `litestar-2.0.0rc1/litestar/utils/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     from litestar.types import MaybePartial
 
 __all__ = (
     "Ref",
     "encode_headers",
     "filter_cookies",
     "get_enum_string_value",
-    "get_fully_qualified_class_name",
     "get_name",
     "unwrap_partial",
     "url_quote",
 )
 
 T = TypeVar("T")
 
@@ -36,20 +35,14 @@
         A name string.
     """
     if hasattr(value, "__name__"):
         return cast("str", value.__name__)
     return type(value).__name__
 
 
-def get_fully_qualified_class_name(value: type[Any]) -> str:
-    """Construct the full path name for a type."""
-    module = getattr(value, "__module__", "<no module>")
-    return f"{module}.{value.__qualname__}"
-
-
 def get_enum_string_value(value: Enum | str) -> str:
     """Return the string value of a string enum.
 
     See: https://github.com/litestar-org/litestar/pull/633#issuecomment-1286519267
 
     Args:
         value: An enum or string.
```

### Comparing `litestar-2.0.0b4/litestar/utils/path.py` & `litestar-2.0.0rc1/litestar/utils/path.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/utils/predicates.py` & `litestar-2.0.0rc1/litestar/utils/predicates.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/utils/scope.py` & `litestar-2.0.0rc1/litestar/utils/scope.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/utils/signature.py` & `litestar-2.0.0rc1/litestar/utils/signature.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import sys
 import typing
+from copy import deepcopy
 from dataclasses import dataclass, replace
 from inspect import Signature, getmembers, isclass, ismethod
 from itertools import chain
 from typing import Any
 
 from typing_extensions import Self, get_type_hints
 
@@ -88,64 +89,63 @@
     parameters: dict[str, FieldDefinition]
     """A mapping of parameter names to ParsedSignatureParameter instances."""
     return_type: FieldDefinition
     """The return annotation of the callable."""
     original_signature: Signature
     """The raw signature as returned by :func:`inspect.signature`"""
 
+    def __deepcopy__(self, memo: dict[str, Any]) -> Self:
+        return type(self)(
+            parameters={k: deepcopy(v) for k, v in self.parameters.items()},
+            return_type=deepcopy(self.return_type),
+            original_signature=deepcopy(self.original_signature),
+        )
+
     @classmethod
     def from_fn(cls, fn: AnyCallable, signature_namespace: dict[str, Any]) -> Self:
         """Parse a function signature.
 
         Args:
             fn: Any callable.
             signature_namespace: mapping of names to types for forward reference resolution
 
         Returns:
             ParsedSignature
         """
         signature = Signature.from_callable(fn)
         fn_type_hints = get_fn_type_hints(fn, namespace=signature_namespace)
 
+        return cls.from_signature(signature, fn_type_hints)
+
+    @classmethod
+    def from_signature(cls, signature: Signature, fn_type_hints: dict[str, type]) -> Self:
+        """Parse an :class:`inspect.Signature` instance.
+
+        Args:
+            signature: An :class:`inspect.Signature` instance.
+            fn_type_hints: mapping of types
+
+        Returns:
+            ParsedSignature
+        """
+
         parameters = tuple(
             FieldDefinition.from_parameter(parameter=parameter, fn_type_hints=fn_type_hints)
             for name, parameter in signature.parameters.items()
             if name not in ("self", "cls")
         )
 
         return_type = FieldDefinition.from_annotation(fn_type_hints.get("return", Any))
 
         return cls(
             parameters={p.name: p for p in parameters},
             return_type=return_type if "return" in fn_type_hints else replace(return_type, annotation=Empty),
             original_signature=signature,
         )
 
-    @classmethod
-    def from_signature(cls, signature: Signature, signature_namespace: dict[str, Any]) -> Self:
-        """Parse an :class:`inspect.Signature` instance.
-
-        Python's `get_type_hints()` function does not support parsing signatures directly, so we need to create a dummy
-        function to pass to it. Maybe there's a better way to do this, but this does work.
-
-        Args:
-            signature: An :class:`inspect.Signature` instance.
-            signature_namespace: mapping of names to types for forward reference resolution
-
-        Returns:
-            ParsedSignature
-        """
-
-        def fn() -> None:
-            ...
-
-        fn.__signature__ = signature  # type:ignore[attr-defined]
-        fn.__annotations__ = {p.name: p.annotation for p in signature.parameters.values()}
-        return cls.from_fn(fn, signature_namespace)
-
 
 def infer_request_encoding_from_field_definition(field_definition: FieldDefinition) -> RequestEncodingType | str:
     """Infer the request encoding type from a parsed type.
 
     Args:
         field_definition: The parsed parameter to infer the request encoding type from.
```

### Comparing `litestar-2.0.0b4/litestar/utils/sync.py` & `litestar-2.0.0rc1/litestar/utils/sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/utils/typing.py` & `litestar-2.0.0rc1/litestar/utils/typing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,58 @@
 from __future__ import annotations
 
 import re
-import typing as t
 from collections import abc, defaultdict, deque
 from typing import (
     AbstractSet,
     Any,
+    AsyncGenerator,
+    AsyncIterable,
+    AsyncIterator,
+    Awaitable,
+    Collection,
+    Container,
+    Coroutine,
     DefaultDict,
     Deque,
     Dict,
     FrozenSet,
+    Generator,
+    ItemsView,
     Iterable,
     Iterator,
+    KeysView,
     List,
     Mapping,
+    MappingView,
     MutableMapping,
     MutableSequence,
     MutableSet,
+    Reversible,
     Sequence,
     Set,
     Tuple,
     TypeVar,
     Union,
+    ValuesView,
     cast,
 )
 
 from typing_extensions import Annotated, NotRequired, Required, TypeGuard, get_args, get_origin
 
 from litestar.types.builtin_types import NoneType, UnionTypes
 
 __all__ = (
     "annotation_is_iterable_of_type",
     "get_instantiable_origin",
     "get_origin_or_inner_type",
     "get_safe_generic_origin",
     "instantiable_type_mapping",
     "make_non_optional_union",
+    "safe_generic_origin_map",
     "unwrap_annotation",
     "unwrap_union",
 )
 
 
 T = TypeVar("T")
 UnionT = TypeVar("UnionT", bound="Union")
@@ -76,44 +89,44 @@
     dict: dict,
     frozenset: frozenset,
     list: list,
     set: set,
     tuple: tuple,
 }
 
-_safe_generic_origin_map = {
-    set: t.AbstractSet,
-    defaultdict: t.DefaultDict,
-    deque: t.Deque,
-    dict: t.Dict,
-    frozenset: t.FrozenSet,
-    list: t.List,
-    tuple: t.Tuple,
-    abc.Mapping: t.Mapping,
-    abc.MutableMapping: t.MutableMapping,
-    abc.MutableSequence: t.MutableSequence,
-    abc.MutableSet: t.MutableSet,
-    abc.Sequence: t.Sequence,
-    abc.Set: t.AbstractSet,
-    abc.Collection: t.Collection,
-    abc.Container: t.Container,
-    abc.ItemsView: t.ItemsView,
-    abc.KeysView: t.KeysView,
-    abc.MappingView: t.MappingView,
-    abc.ValuesView: t.ValuesView,
-    abc.Iterable: t.Iterable,
-    abc.Iterator: t.Iterator,
-    abc.Generator: t.Generator,
-    abc.Reversible: t.Reversible,
-    abc.Coroutine: t.Coroutine,
-    abc.AsyncGenerator: t.AsyncGenerator,
-    abc.AsyncIterable: t.AsyncIterable,
-    abc.AsyncIterator: t.AsyncIterator,
-    abc.Awaitable: t.Awaitable,
-    **{union_t: t.Union for union_t in UnionTypes},
+safe_generic_origin_map = {
+    set: AbstractSet,
+    defaultdict: DefaultDict,
+    deque: Deque,
+    dict: Dict,
+    frozenset: FrozenSet,
+    list: List,
+    tuple: Tuple,
+    abc.Mapping: Mapping,
+    abc.MutableMapping: MutableMapping,
+    abc.MutableSequence: MutableSequence,
+    abc.MutableSet: MutableSet,
+    abc.Sequence: Sequence,
+    abc.Set: AbstractSet,
+    abc.Collection: Collection,
+    abc.Container: Container,
+    abc.ItemsView: ItemsView,
+    abc.KeysView: KeysView,
+    abc.MappingView: MappingView,
+    abc.ValuesView: ValuesView,
+    abc.Iterable: Iterable,
+    abc.Iterator: Iterator,
+    abc.Generator: Generator,
+    abc.Reversible: Reversible,
+    abc.Coroutine: Coroutine,
+    abc.AsyncGenerator: AsyncGenerator,
+    abc.AsyncIterable: AsyncIterable,
+    abc.AsyncIterator: AsyncIterator,
+    abc.Awaitable: Awaitable,
+    **{union_t: Union for union_t in UnionTypes},
 }
 """A mapping of types to equivalent types that are safe to be used as generics across all Python versions.
 
 This is necessary because occasionally we want to rebuild a generic outer type with different args, and types such as
 ``collections.abc.Mapping``, are not valid generic types in Python 3.8.
 """
 
@@ -238,16 +251,16 @@
         annotation: Type annotation associated with the origin type. Should be unwrapped from any wrapper types, such
             as ``Annotated``.
 
     Returns:
         The ``typing`` module equivalent of the given type, if it exists. Otherwise, the original type is returned.
     """
     if origin_type is None:
-        return _safe_generic_origin_map.get(annotation)
-    return _safe_generic_origin_map.get(origin_type, origin_type)
+        return safe_generic_origin_map.get(annotation)
+    return safe_generic_origin_map.get(origin_type, origin_type)
 
 
 def get_instantiable_origin(origin_type: Any, annotation: Any) -> Any:
     """Get a type that is safe to instantiate for the given origin type.
 
     If a builtin collection type is annotated without generic args, e.g, ``a: dict``, then the origin type will be
     ``None``. In this case, we can use the annotation to determine the correct instantiable type, if one exists.
```

### Comparing `litestar-2.0.0b4/litestar/utils/version.py` & `litestar-2.0.0rc1/litestar/utils/version.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/litestar/utils/warnings.py` & `litestar-2.0.0rc1/litestar/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b4/pyproject.toml` & `litestar-2.0.0rc1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "litestar"
-version = "2.0.0beta4"
+version = "2.0.0rc1"
 description = "Litestar - A production-ready, highly performant, extensible ASGI API Framework"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
     "Jacob Coffee <jacob@z7x.org>",
@@ -19,22 +19,17 @@
 readme = "docs/PYPI_README.md"
 homepage = "https://litestar.dev/"
 repository = "https://github.com/litestar-org/litestar"
 documentation = "https://docs.litestar.dev/"
 keywords = [
     "api",
     "rest",
-    "http",
     "asgi",
-    "pydantic",
     "litestar",
     "starlite",
-    "framework",
-    "websocket",
-    "litestar",
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
@@ -109,32 +104,34 @@
 
 [tool.poetry.group.dev.dependencies]
 aiosqlite = "*"
 asyncmy = "*"
 asyncpg = "*"
 beautifulsoup4 = "*"
 duckdb-engine = "*"
-fakeredis = { extras = ["lua"], version = "<2.17.0" }
-freezegun = "*"
 fsspec = "*"
 greenlet = "*"
+httpx-sse = "*"
 hypothesis = "*"
 opentelemetry-sdk = "*"
 oracledb = "*"
 psycopg = "*"
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "*"
 pytest-lazy-fixture = "*"
 pytest-mock = "*"
 pytest-rerunfailures = "*"
+pytest-timeout = "^2.1.0"
 python-dotenv = "*"
 sqlalchemy-spanner = "*"
 starlette = "*"
+time-machine = "^2.11.0"
 trio = "*"
+pytest-xdist = "^3.3.1"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 auto-pytabs = { extras = ["sphinx"], version = "*" }
 black = "*"
@@ -156,15 +153,14 @@
 mypy = "*"
 pre-commit = "*"
 pyright = "*"
 ruff = '*'
 slotscheck = "*"
 sourcery = "*"
 types-beautifulsoup4 = "*"
-types-freezegun = "*"
 types-python-jose = "*"
 types-pyyaml = "*"
 types-redis = "*"
 
 [tool.poetry.extras]
 annotated-types = ["annotated-types"]
 attrs = ["attrs"]
@@ -221,40 +217,48 @@
 include = '\.pyi?$'
 
 [tool.codespell]
 ignore-words-list = "selectin"
 skip = 'poetry.lock,docs/examples/contrib/sqlalchemy/us_state_lookup.json'
 
 [tool.coverage.run]
-omit = ["*/tests/*", "litestar/contrib/sqlalchemy_1/*"]
+omit = ["*/tests/*"]
+parallel = true
+concurrency = ["multiprocessing", "thread"]
 
 [tool.coverage.report]
 exclude_lines = [
     'pragma: no cover',
     'if TYPE_CHECKING:',
     'except ImportError as e:',
     'except ImportError:',
     '\.\.\.',
     'raise NotImplementedError',
     'if VERSION.startswith("1"):',
     'if pydantic.VERSION.startswith("1"):',
 ]
 
 [tool.pytest.ini_options]
-addopts = "--ignore=examples -m='not sqlalchemy_integration'"
+addopts = "-m='not sqlalchemy_integration' --dist=loadgroup"
 asyncio_mode = "auto"
 filterwarnings = [
-    "ignore::trio.TrioDeprecationWarning:anyio._backends._trio*:164",
+    "ignore::trio.TrioDeprecationWarning:anyio._backends._trio*:",
     "ignore::DeprecationWarning:pkg_resources.*",
     "ignore::DeprecationWarning:google.rpc",
     "ignore::DeprecationWarning:google.gcloud",
     "ignore::DeprecationWarning:google.iam",
     "ignore::DeprecationWarning:google",
     "ignore::DeprecationWarning:sphinxcontrib",
     "ignore::DeprecationWarning:litestar.*",
+    "ignore:The `__fields__` attribute is deprecated:DeprecationWarning:pydantic*",
+    "ignore:Support for class-based `config` is deprecated:DeprecationWarning:pydantic*",
+    "ignore:The `dict` method is deprecated:DeprecationWarning:",
+    "ignore:The `parse_obj` method is deprecated:DeprecationWarning:",
+    "ignore:The `json` method is deprecated:DeprecationWarning:",
+    "ignore:Extra keyword arguments on `Field` is deprecated:DeprecationWarning:pydantic*",
 ]
 markers = [
     "sqlalchemy_integration: SQLAlchemy integration tests",
     "sqlalchemy_asyncmy: SQLAlchemy MySQL (asyncmy) Tests",
     "sqlalchemy_asyncpg: SQLAlchemy Postgres (asyncpg) Tests",
     "sqlalchemy_psycopg_async: SQLAlchemy Postgres (psycopg async) Tests",
     "sqlalchemy_aiosqlite: SQLAlchemy SQLite (aiosqlite) Tests",
@@ -276,15 +280,15 @@
 strict = true
 disallow_untyped_decorators = true
 disallow_any_generics = false
 implicit_reexport = false
 show_error_codes = true
 
 [[tool.mypy.overrides]]
-module = ["tests.*.test_sqlalchemy_sync", "tests.*.test_sqlalchemy_async"]
+module = ["tests.*.test_sqlalchemy", "tests.*.test_sqlalchemy"]
 disable_error_code = "attr-defined"
 
 [[tool.mypy.overrides]]
 module = "tests.unit.test_contrib.test_sqlalchemy.test_dto"
 disable_error_code = ["arg-type", "misc", "valid-type", "var-annotated"]
 
 [[tool.mypy.overrides]]
```

### Comparing `litestar-2.0.0b4/PKG-INFO` & `litestar-2.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: litestar
-Version: 2.0.0b4
+Version: 2.0.0rc1
 Summary: Litestar - A production-ready, highly performant, extensible ASGI API Framework
 Home-page: https://litestar.dev/
 License: MIT
-Keywords: api,rest,http,asgi,pydantic,litestar,starlite,framework,websocket,litestar
+Keywords: api,rest,asgi,litestar,starlite
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
 Maintainer: Na'aman Hirschfeld
 Maintainer-email: nhirschfeld@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -114,15 +114,16 @@
 | Meta      |     | [![Litestar Project](https://img.shields.io/badge/Litestar%20Org-%E2%AD%90%20Litestar-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/litestar-org/litestar) [![types - Mypy](https://img.shields.io/badge/types-Mypy-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/python/mypy) [![License - MIT](https://img.shields.io/badge/license-MIT-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://spdx.org/licenses/) [![Litestar Sponsors](https://img.shields.io/badge/Sponsor-%E2%9D%A4-%23edb641.svg?&logo=github&logoColor=edb641&labelColor=202235)](https://github.com/sponsors/litestar-org) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json&labelColor=202235)](https://github.com/astral-sh/ruff) [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=python&labelColor=202235&logoColor=edb641)](https://github.com/psf/black) [![All Contributors](https://img.shields.io/github/all-contributors/litestar-org/litestar?labelColor=202235&color=edb641&logoColor=edb641)](#contributors-)  |
 
 <!-- prettier-ignore-end -->
 </div>
 
 # Starlite → Litestar
 
-**[Starlite has been renamed to Litestar](https://litestar.dev/about/organization.html#litestar-and-starlite)**
+> [!IMPORTANT]\
+> [**_Starlite has been renamed to Litestar_**](https://litestar.dev/about/organization.html#litestar-and-starlite)
 
 <hr>
 
 Litestar is a powerful, performant, flexible and opinionated ASGI framework,
 offering first class typing support.
 
 Check out the [documentation 📚](https://docs.litestar.dev/).
@@ -133,15 +134,15 @@
 pip install litestar
 ```
 
 **Litestar 2.0 is coming out soon**, bringing many new features and improvements.
 You can check out the latest pre-release version by instead running
 
 ```shell
-pip install litestar==2.0.0beta3
+pip install litestar==2.0.0beta4
 ```
 
 ## Quick Start
 
 ```python
 from litestar import Litestar, get
```

