# Comparing `tmp/jj-2.7.3.tar.gz` & `tmp/jj-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jj-2.7.3.tar", last modified: Sun Jun  4 08:42:24 2023, max compression
+gzip compressed data, was "jj-2.8.0.tar", last modified: Sat Aug  5 11:36:20 2023, max compression
```

## Comparing `jj-2.7.3.tar` & `jj-2.8.0.tar`

### file list

```diff
@@ -1,118 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.052106 jj-2.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-04 08:42:14.000000 jj-2.7.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-06-04 08:42:24.052106 jj-2.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-06-04 08:42:14.000000 jj-2.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.040105 jj-2.7.3/jj/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-04 08:42:14.000000 jj-2.7.3/jj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-04 08:42:14.000000 jj-2.7.3/jj/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-04 08:42:14.000000 jj-2.7.3/jj/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.044106 jj-2.7.3/jj/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-04 08:42:14.000000 jj-2.7.3/jj/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-04 08:42:14.000000 jj-2.7.3/jj/apps/_abstract_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-04 08:42:14.000000 jj-2.7.3/jj/apps/_base_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-04 08:42:14.000000 jj-2.7.3/jj/apps/_default_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.044106 jj-2.7.3/jj/expiration_policy/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-04 08:42:14.000000 jj-2.7.3/jj/expiration_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-04 08:42:14.000000 jj-2.7.3/jj/expiration_policy/_expiration_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-04 08:42:14.000000 jj-2.7.3/jj/expiration_policy/_expire_after_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-04 08:42:14.000000 jj-2.7.3/jj/expiration_policy/_expire_never.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.044106 jj-2.7.3/jj/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-04 08:42:14.000000 jj-2.7.3/jj/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-04 08:42:14.000000 jj-2.7.3/jj/handlers/_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-04 08:42:14.000000 jj-2.7.3/jj/handlers/_handler_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.044106 jj-2.7.3/jj/http/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-04 08:42:14.000000 jj-2.7.3/jj/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.044106 jj-2.7.3/jj/http/codes/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-04 08:42:14.000000 jj-2.7.3/jj/http/codes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.044106 jj-2.7.3/jj/http/headers/
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-04 08:42:14.000000 jj-2.7.3/jj/http/headers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.044106 jj-2.7.3/jj/http/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-04 08:42:14.000000 jj-2.7.3/jj/http/methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.044106 jj-2.7.3/jj/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-04 08:42:14.000000 jj-2.7.3/jj/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-04 08:42:14.000000 jj-2.7.3/jj/logs/_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-04 08:42:14.000000 jj-2.7.3/jj/logs/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.044106 jj-2.7.3/jj/logs/formatters/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-04 08:42:14.000000 jj-2.7.3/jj/logs/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-04 08:42:14.000000 jj-2.7.3/jj/logs/formatters/_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-04 08:42:14.000000 jj-2.7.3/jj/logs/formatters/_simple_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.044106 jj-2.7.3/jj/matchers/
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/_resolvable_matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.048106 jj-2.7.3/jj/matchers/attribute_matchers/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/attribute_matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/attribute_matchers/_attribute_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/attribute_matchers/_contain_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/attribute_matchers/_equal_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/attribute_matchers/_exist_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/attribute_matchers/_multi_dict_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/attribute_matchers/_regex_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/attribute_matchers/_route_matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.048106 jj-2.7.3/jj/matchers/logical_matchers/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/logical_matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/logical_matchers/_all_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/logical_matchers/_any_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/logical_matchers/_logical_matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.048106 jj-2.7.3/jj/matchers/request_matchers/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/request_matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/request_matchers/_header_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/request_matchers/_method_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/request_matchers/_param_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/request_matchers/_path_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/request_matchers/_request_matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.048106 jj-2.7.3/jj/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-04 08:42:14.000000 jj-2.7.3/jj/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-04 08:42:14.000000 jj-2.7.3/jj/middlewares/_abstract_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-04 08:42:14.000000 jj-2.7.3/jj/middlewares/_base_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-04 08:42:14.000000 jj-2.7.3/jj/middlewares/_logger_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-04 08:42:14.000000 jj-2.7.3/jj/middlewares/_middleware_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-04 08:42:14.000000 jj-2.7.3/jj/middlewares/_root_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-04 08:42:14.000000 jj-2.7.3/jj/middlewares/_self_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.048106 jj-2.7.3/jj/mock/
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.052106 jj-2.7.3/jj/mock/_history/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_history/_body_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_history/_history_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_history/_history_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_history/_history_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_history/_history_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_history/_history_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_mocked.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_remote_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_remote_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_stacked.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_system_log_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:14.000000 jj-2.7.3/jj/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.052106 jj-2.7.3/jj/requests/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-04 08:42:14.000000 jj-2.7.3/jj/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-04 08:42:14.000000 jj-2.7.3/jj/requests/_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.052106 jj-2.7.3/jj/resolvers/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-04 08:42:14.000000 jj-2.7.3/jj/resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-04 08:42:14.000000 jj-2.7.3/jj/resolvers/_matcher_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-04 08:42:14.000000 jj-2.7.3/jj/resolvers/_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-04 08:42:14.000000 jj-2.7.3/jj/resolvers/_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-04 08:42:14.000000 jj-2.7.3/jj/resolvers/_reversed_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.052106 jj-2.7.3/jj/responses/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-04 08:42:14.000000 jj-2.7.3/jj/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-04 08:42:14.000000 jj-2.7.3/jj/responses/_relay_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-06-04 08:42:14.000000 jj-2.7.3/jj/responses/_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-04 08:42:14.000000 jj-2.7.3/jj/responses/_static_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-04 08:42:14.000000 jj-2.7.3/jj/responses/_stream_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.052106 jj-2.7.3/jj/runners/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-04 08:42:14.000000 jj-2.7.3/jj/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-04 08:42:14.000000 jj-2.7.3/jj/runners/_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.052106 jj-2.7.3/jj/servers/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-04 08:42:14.000000 jj-2.7.3/jj/servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-04 08:42:14.000000 jj-2.7.3/jj/servers/_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.040105 jj-2.7.3/jj.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-06-04 08:42:24.000000 jj-2.7.3/jj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-04 08:42:24.000000 jj-2.7.3/jj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 08:42:24.000000 jj-2.7.3/jj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-04 08:42:24.000000 jj-2.7.3/jj.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-04 08:42:24.000000 jj-2.7.3/jj.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-04 08:42:24.052106 jj-2.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-04 08:42:14.000000 jj-2.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.483361 jj-2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-05 11:36:05.000000 jj-2.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-08-05 11:36:20.483361 jj-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-08-05 11:36:05.000000 jj-2.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.463361 jj-2.8.0/jj/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-05 11:36:05.000000 jj-2.8.0/jj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-05 11:36:05.000000 jj-2.8.0/jj/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-08-05 11:36:05.000000 jj-2.8.0/jj/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-05 11:36:05.000000 jj-2.8.0/jj/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.467361 jj-2.8.0/jj/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-05 11:36:05.000000 jj-2.8.0/jj/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-05 11:36:05.000000 jj-2.8.0/jj/apps/_abstract_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-08-05 11:36:05.000000 jj-2.8.0/jj/apps/_base_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-05 11:36:05.000000 jj-2.8.0/jj/apps/_default_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.467361 jj-2.8.0/jj/expiration_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-05 11:36:05.000000 jj-2.8.0/jj/expiration_policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-05 11:36:05.000000 jj-2.8.0/jj/expiration_policy/_expiration_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-05 11:36:05.000000 jj-2.8.0/jj/expiration_policy/_expire_after_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-05 11:36:05.000000 jj-2.8.0/jj/expiration_policy/_expire_never.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.467361 jj-2.8.0/jj/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-05 11:36:05.000000 jj-2.8.0/jj/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-05 11:36:05.000000 jj-2.8.0/jj/handlers/_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-05 11:36:05.000000 jj-2.8.0/jj/handlers/_handler_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.467361 jj-2.8.0/jj/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-05 11:36:05.000000 jj-2.8.0/jj/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.467361 jj-2.8.0/jj/http/codes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-05 11:36:05.000000 jj-2.8.0/jj/http/codes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.467361 jj-2.8.0/jj/http/headers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-08-05 11:36:05.000000 jj-2.8.0/jj/http/headers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.467361 jj-2.8.0/jj/http/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-05 11:36:05.000000 jj-2.8.0/jj/http/methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.467361 jj-2.8.0/jj/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-08-05 11:36:05.000000 jj-2.8.0/jj/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-05 11:36:05.000000 jj-2.8.0/jj/logs/_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-05 11:36:05.000000 jj-2.8.0/jj/logs/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-08-05 11:36:05.000000 jj-2.8.0/jj/logs/_request_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.471361 jj-2.8.0/jj/logs/formatters/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-05 11:36:05.000000 jj-2.8.0/jj/logs/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-05 11:36:05.000000 jj-2.8.0/jj/logs/formatters/_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-05 11:36:05.000000 jj-2.8.0/jj/logs/formatters/_simple_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.471361 jj-2.8.0/jj/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-05 11:36:05.000000 jj-2.8.0/jj/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-05 11:36:05.000000 jj-2.8.0/jj/matchers/_resolvable_matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.471361 jj-2.8.0/jj/matchers/attribute_matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-05 11:36:05.000000 jj-2.8.0/jj/matchers/attribute_matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-05 11:36:05.000000 jj-2.8.0/jj/matchers/attribute_matchers/_attribute_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-05 11:36:05.000000 jj-2.8.0/jj/matchers/attribute_matchers/_contain_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-08-05 11:36:05.000000 jj-2.8.0/jj/matchers/attribute_matchers/_equal_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-05 11:36:05.000000 jj-2.8.0/jj/matchers/attribute_matchers/_exist_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-08-05 11:36:05.000000 jj-2.8.0/jj/matchers/attribute_matchers/_multi_dict_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-05 11:36:05.000000 jj-2.8.0/jj/matchers/attribute_matchers/_regex_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-05 11:36:05.000000 jj-2.8.0/jj/matchers/attribute_matchers/_route_matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.471361 jj-2.8.0/jj/matchers/logical_matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-05 11:36:05.000000 jj-2.8.0/jj/matchers/logical_matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-08-05 11:36:05.000000 jj-2.8.0/jj/matchers/logical_matchers/_all_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-05 11:36:05.000000 jj-2.8.0/jj/matchers/logical_matchers/_any_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-05 11:36:05.000000 jj-2.8.0/jj/matchers/logical_matchers/_logical_matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.475361 jj-2.8.0/jj/matchers/request_matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-05 11:36:05.000000 jj-2.8.0/jj/matchers/request_matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-05 11:36:05.000000 jj-2.8.0/jj/matchers/request_matchers/_header_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-05 11:36:05.000000 jj-2.8.0/jj/matchers/request_matchers/_method_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-08-05 11:36:05.000000 jj-2.8.0/jj/matchers/request_matchers/_param_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-05 11:36:05.000000 jj-2.8.0/jj/matchers/request_matchers/_path_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-05 11:36:05.000000 jj-2.8.0/jj/matchers/request_matchers/_request_matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.475361 jj-2.8.0/jj/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-05 11:36:05.000000 jj-2.8.0/jj/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-05 11:36:05.000000 jj-2.8.0/jj/middlewares/_abstract_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-08-05 11:36:05.000000 jj-2.8.0/jj/middlewares/_base_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-08-05 11:36:05.000000 jj-2.8.0/jj/middlewares/_logger_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-08-05 11:36:05.000000 jj-2.8.0/jj/middlewares/_middleware_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-05 11:36:05.000000 jj-2.8.0/jj/middlewares/_root_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-05 11:36:05.000000 jj-2.8.0/jj/middlewares/_self_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.479361 jj-2.8.0/jj/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-08-05 11:36:05.000000 jj-2.8.0/jj/mock/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.479361 jj-2.8.0/jj/mock/_history/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-05 11:36:05.000000 jj-2.8.0/jj/mock/_history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-05 11:36:05.000000 jj-2.8.0/jj/mock/_history/_body_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-05 11:36:05.000000 jj-2.8.0/jj/mock/_history/_history_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.479361 jj-2.8.0/jj/mock/_history/_history_formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-05 11:36:05.000000 jj-2.8.0/jj/mock/_history/_history_formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-05 11:36:05.000000 jj-2.8.0/jj/mock/_history/_history_formatter/_history_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-05 11:36:05.000000 jj-2.8.0/jj/mock/_history/_history_formatter/_pretty_history_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-05 11:36:05.000000 jj-2.8.0/jj/mock/_history/_history_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-08-05 11:36:05.000000 jj-2.8.0/jj/mock/_history/_history_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-08-05 11:36:05.000000 jj-2.8.0/jj/mock/_history/_history_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-08-05 11:36:05.000000 jj-2.8.0/jj/mock/_history/_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-08-05 11:36:05.000000 jj-2.8.0/jj/mock/_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-08-05 11:36:05.000000 jj-2.8.0/jj/mock/_mocked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-08-05 11:36:05.000000 jj-2.8.0/jj/mock/_remote_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-08-05 11:36:05.000000 jj-2.8.0/jj/mock/_remote_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-05 11:36:05.000000 jj-2.8.0/jj/mock/_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-05 11:36:05.000000 jj-2.8.0/jj/mock/_stacked.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-05 11:36:05.000000 jj-2.8.0/jj/mock/_system_log_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-05 11:36:05.000000 jj-2.8.0/jj/mock/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:05.000000 jj-2.8.0/jj/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.479361 jj-2.8.0/jj/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-05 11:36:05.000000 jj-2.8.0/jj/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-08-05 11:36:05.000000 jj-2.8.0/jj/requests/_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.483361 jj-2.8.0/jj/resolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-05 11:36:05.000000 jj-2.8.0/jj/resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-05 11:36:05.000000 jj-2.8.0/jj/resolvers/_matcher_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-08-05 11:36:05.000000 jj-2.8.0/jj/resolvers/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-08-05 11:36:05.000000 jj-2.8.0/jj/resolvers/_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-05 11:36:05.000000 jj-2.8.0/jj/resolvers/_reversed_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.483361 jj-2.8.0/jj/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-05 11:36:05.000000 jj-2.8.0/jj/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-08-05 11:36:05.000000 jj-2.8.0/jj/responses/_relay_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-08-05 11:36:05.000000 jj-2.8.0/jj/responses/_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-05 11:36:05.000000 jj-2.8.0/jj/responses/_static_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-05 11:36:05.000000 jj-2.8.0/jj/responses/_stream_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.483361 jj-2.8.0/jj/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-05 11:36:05.000000 jj-2.8.0/jj/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-08-05 11:36:05.000000 jj-2.8.0/jj/runners/_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.483361 jj-2.8.0/jj/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-05 11:36:05.000000 jj-2.8.0/jj/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-08-05 11:36:05.000000 jj-2.8.0/jj/servers/_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:36:20.463361 jj-2.8.0/jj.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-08-05 11:36:20.000000 jj-2.8.0/jj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-08-05 11:36:20.000000 jj-2.8.0/jj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 11:36:20.000000 jj-2.8.0/jj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-05 11:36:20.000000 jj-2.8.0/jj.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-05 11:36:20.000000 jj-2.8.0/jj.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-05 11:36:20.487361 jj-2.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-05 11:36:05.000000 jj-2.8.0/setup.py
```

### Comparing `jj-2.7.3/LICENSE.txt` & `jj-2.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/PKG-INFO` & `jj-2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jj
-Version: 2.7.3
+Version: 2.8.0
 Summary: Remote HTTP Mock
 Home-page: https://github.com/tsv1/jj
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `jj-2.7.3/README.md` & `jj-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/__init__.py` & `jj-2.8.0/jj/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/_core.py` & `jj-2.8.0/jj/_core.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/apps/_base_app.py` & `jj-2.8.0/jj/apps/_base_app.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/expiration_policy/_expire_after_requests.py` & `jj-2.8.0/jj/expiration_policy/_expire_after_requests.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/expiration_policy/_expire_never.py` & `jj-2.8.0/jj/expiration_policy/_expire_never.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/http/codes/__init__.py` & `jj-2.8.0/jj/http/codes/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/http/headers/__init__.py` & `jj-2.8.0/jj/http/headers/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/logs/__init__.py` & `jj-2.8.0/jj/logs/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 
 from ._filter import Filter
 from ._logger import Logger
+from ._request_filter import RequestFilter
 from .formatters import Formatter, SimpleFormatter
 
 __all__ = ("Logger", "Filter", "Formatter", "SimpleFormatter")
 
 
 # Set custom Logger class
 
@@ -17,15 +18,17 @@
 logger: Logger = logging.getLogger("jj.access_logger")  # type: ignore
 logger.setLevel(logging.INFO)
 logger.propagate = False
 
 # Register Filter
 
 filter_ = Filter()
+request_filter_ = RequestFilter()
 logger.addFilter(filter_)
+logger.addFilter(request_filter_)
 
 # Register Handler
 
 handler = logging.StreamHandler()
 logger.addHandler(handler)
 
 # Register Formatter
```

### Comparing `jj-2.7.3/jj/logs/_filter.py` & `jj-2.8.0/jj/logs/_filter.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/logs/formatters/_formatter.py` & `jj-2.8.0/jj/logs/formatters/_formatter.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/matchers/__init__.py` & `jj-2.8.0/jj/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/matchers/_resolvable_matcher.py` & `jj-2.8.0/jj/matchers/_resolvable_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/matchers/attribute_matchers/__init__.py` & `jj-2.8.0/jj/matchers/attribute_matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/matchers/attribute_matchers/_contain_matcher.py` & `jj-2.8.0/jj/matchers/attribute_matchers/_contain_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/matchers/attribute_matchers/_equal_matcher.py` & `jj-2.8.0/jj/matchers/attribute_matchers/_equal_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/matchers/attribute_matchers/_multi_dict_matcher.py` & `jj-2.8.0/jj/matchers/attribute_matchers/_multi_dict_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/matchers/attribute_matchers/_regex_matcher.py` & `jj-2.8.0/jj/matchers/attribute_matchers/_regex_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/matchers/attribute_matchers/_route_matcher.py` & `jj-2.8.0/jj/matchers/attribute_matchers/_route_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/matchers/logical_matchers/_all_matcher.py` & `jj-2.8.0/jj/matchers/logical_matchers/_all_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/matchers/logical_matchers/_any_matcher.py` & `jj-2.8.0/jj/matchers/logical_matchers/_any_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/matchers/request_matchers/_header_matcher.py` & `jj-2.8.0/jj/matchers/request_matchers/_header_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/matchers/request_matchers/_method_matcher.py` & `jj-2.8.0/jj/matchers/request_matchers/_method_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/matchers/request_matchers/_param_matcher.py` & `jj-2.8.0/jj/matchers/request_matchers/_param_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/matchers/request_matchers/_path_matcher.py` & `jj-2.8.0/jj/matchers/request_matchers/_path_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/middlewares/_abstract_middleware.py` & `jj-2.8.0/jj/middlewares/_abstract_middleware.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/middlewares/_base_middleware.py` & `jj-2.8.0/jj/middlewares/_base_middleware.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/middlewares/_logger_middleware.py` & `jj-2.8.0/jj/middlewares/_logger_middleware.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/middlewares/_self_middleware.py` & `jj-2.8.0/jj/middlewares/_self_middleware.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/mock/_history/_body_parser.py` & `jj-2.8.0/jj/mock/_history/_body_parser.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/mock/_history/_history_repository.py` & `jj-2.8.0/jj/mock/_history/_history_repository.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,7 +26,10 @@
         })
 
     async def delete_by_tag(self, tag: str) -> None:
         self._storage = [x for x in self._storage if tag not in x["tags"]]
 
     async def get_by_tag(self, tag: str) -> List[HistoryItem]:
         return [x for x in self._storage if tag in x["tags"]]
+
+    async def clear(self) -> None:
+        self._storage.clear()
```

### Comparing `jj-2.7.3/jj/mock/_history/_history_request.py` & `jj-2.8.0/jj/mock/_history/_history_request.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/mock/_history/_history_response.py` & `jj-2.8.0/jj/mock/_history/_history_response.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/mock/_mock.py` & `jj-2.8.0/jj/mock/_mock.py`

 * *Files 20% similar despite different names*

```diff
@@ -62,34 +62,74 @@
             errors.append(f"Decode Error: invalid expiration policy ({expiration_policy!r})")
 
         if len(errors) > 0:
             raise _DecodeError("\n".join(errors))
 
         return handler_id, matcher, response, expiration_policy
 
+    def _register_handler(self, handler_id: str,
+                          matcher: MatcherType,
+                          response: RemoteResponseType,
+                          expiration_policy: Optional[ExpirationPolicy]) -> None:
+        async def handler(req: Request) -> RemoteResponseType:
+            res = response.copy()
+            await res._prepare_hook(req)
+            return res
+
+        self._resolver.register_attribute("handler_id", handler_id, handler)
+        self._resolver.register_attribute("expiration_policy", expiration_policy, handler)
+        setattr(self._app.__class__, handler_id, matcher(handler))
+
+    def _deregister_handler(self, handler_id: str) -> None:
+        handler = getattr(self._app.__class__, handler_id, None)
+        if handler is None:
+            return
+
+        try:
+            delattr(self._app.__class__, handler_id)
+        except AttributeError:
+            pass
+
+        matchers = self._resolver.get_matchers(handler)
+        for matcher in matchers:
+            self._resolver.deregister_matcher(matcher, handler)
+
+        attributes = self._resolver.get_attributes(handler)
+        for attribute in attributes:
+            self._resolver.deregister_attribute(attribute, handler)
+
+        self._resolver._registry.remove_container(handler)
+
+    @jj.match(POST, "/__jj__/reset", headers={"x-jj-remote-mock": exists})
+    async def reset(self, request: Request) -> Response:
+        await request.read()
+
+        handlers = self._resolver.get_handlers(self._app.__class__)
+        for handler in handlers:
+            handler_id = self._resolver.get_attribute("handler_id", handler, None)
+            if handler_id:
+                self._deregister_handler(handler_id)
+
+        await self._repo.clear()
+
+        return Response(status=OK, json={"status": OK})
+
     @jj.match_any([
         jj.match(POST, "/__jj__/register", headers={"x-jj-remote-mock": exists}),
         # backward compatibility
         jj.match(POST, headers={"x-jj-remote-mock": exists})
     ])
     async def register(self, request: Request) -> Response:
         payload = await request.read()
         try:
             handler_id, matcher, response, expiration_policy = self._decode(payload)
         except Exception as e:
             return Response(status=BAD_REQUEST, json={"status": BAD_REQUEST, "error": str(e)})
 
-        async def handler(request: Request) -> RemoteResponseType:
-            res = response.copy()
-            await res._prepare_hook(request)
-            return res
-
-        self._resolver.register_attribute("handler_id", handler_id, handler)
-        self._resolver.register_attribute("expiration_policy", expiration_policy, handler)
-        setattr(self._app.__class__, handler_id, matcher(handler))
+        self._register_handler(handler_id, matcher, response, expiration_policy)
 
         return Response(status=OK, json={"status": OK})
 
     @jj.match_any([
         jj.match(DELETE, "/__jj__/deregister", headers={"x-jj-remote-mock": exists}),
         # backward compatibility
         jj.match(DELETE, headers={"x-jj-remote-mock": exists})
@@ -97,20 +137,16 @@
     async def deregister(self, request: Request) -> Response:
         payload = await request.read()
         try:
             handler_id, *_ = self._decode(payload)
         except Exception as e:
             return Response(status=BAD_REQUEST, json={"status": BAD_REQUEST, "error": str(e)})
 
-        try:
-            delattr(self._app.__class__, handler_id)
-        except AttributeError:
-            pass
-
-        await self._repo.delete_by_tag(handler_id)
+        self._deregister_handler(handler_id)
+        await self._repo.delete_by_tag(handler_id)  # delete history
 
         return Response(status=OK, json={"status": OK})
 
     @jj.match_any([
         jj.match(GET, "/__jj__/history", headers={"x-jj-remote-mock": exists}),
         # backward compatibility
         jj.match(GET, headers={"x-jj-remote-mock": exists})
```

### Comparing `jj-2.7.3/jj/mock/_mocked.py` & `jj-2.8.0/jj/mock/_mocked.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from types import TracebackType
 from typing import List, Optional, Type, Union
 
 from rtry import CancelledError, retry
 from rtry.types import AttemptValue, DelayCallable, DelayValue, LoggerCallable, TimeoutValue
 
-from ._history import HistoryItem
+from ._history import HistoryFormatter, HistoryItem
 from ._remote_handler import RemoteHandler
 from ._utils import run_async
 
 __all__ = ("Mocked",)
 
 
 class Mocked:
     def __init__(self, handler: RemoteHandler, *,
                  disposable: bool = True,
-                 prefetch_history: bool = True) -> None:
+                 prefetch_history: bool = True,
+                 history_formatter: Optional[HistoryFormatter] = None
+                 ) -> None:
         self._handler = handler
         self._disposable = disposable
         self._prefetch_history = prefetch_history
         self._history: Union[List[HistoryItem], None] = None
+        self._history_formatter = history_formatter
 
     @property
     def handler(self) -> RemoteHandler:
         return self._handler
 
     @property
     def disposable(self) -> bool:
@@ -75,10 +78,17 @@
     def __exit__(self,
                  exc_type: Optional[Type[BaseException]],
                  exc_val: Optional[BaseException],
                  exc_tb: Optional[TracebackType]) -> None:
         return run_async(self.__aexit__, exc_type, exc_val, exc_tb)
 
     def __repr__(self) -> str:
-        return (f"Mocked<{self._handler}, "
-                f"disposable={self._disposable}, "
-                f"prefetch_history={self._prefetch_history}>")
+        if self._history_formatter:
+            formatted = None
+            if self._history is not None:
+                formatted = self._history_formatter.format_history(self._history)
+            return (f"Mocked<disposable={self._disposable}, "
+                    f"prefetch_history={self._prefetch_history} "
+                    f"history={formatted}>")
+        else:
+            return (f"Mocked<disposable={self._disposable}, "
+                    f"prefetch_history={self._prefetch_history}>")
```

### Comparing `jj-2.7.3/jj/mock/_remote_handler.py` & `jj-2.8.0/jj/mock/_remote_handler.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/mock/_remote_mock.py` & `jj-2.8.0/jj/mock/_remote_mock.py`

 * *Files 13% similar despite different names*

```diff
@@ -35,15 +35,16 @@
             self,
             matcher,
             response,
             expiration_policy=expiration_policy,
             history_adapter=history_adapter,
         )
 
-    async def _do_request(self, method: str, url: str, data: bytes) -> Tuple[int, bytes]:
+    async def _do_request(self, method: str, url: str,
+                          data: Optional[bytes] = None) -> Tuple[int, bytes]:
         headers = {"x-jj-remote-mock": f"v{version}"}
         async with ClientSession() as session:
             async with session.request(method, url, data=data, headers=headers) as response:
                 body = await response.read()
                 return response.status, body
 
     def _pack_payload(self, handler: RemoteHandler) -> bytes:
@@ -71,7 +72,14 @@
 
     async def fetch_history(self, handler: RemoteHandler) -> List[HistoryItem]:
         url = f"{self._url}/__jj__/history"
         status, body = await self._do_request(GET, url, self._pack_payload(handler))
         if status != OK:
             raise _RemoteMockError(f"Can't retrieve mock history ({body!r})")
         return cast(List[HistoryItem], unpack(body))
+
+    async def reset(self) -> "RemoteMock":
+        url = f"{self._url}/__jj__/reset"
+        status, body = await self._do_request(POST, url)
+        if status != OK:
+            raise _RemoteMockError(f"Can't reset mock ({body!r})")
+        return self
```

### Comparing `jj-2.7.3/jj/mock/_stacked.py` & `jj-2.8.0/jj/mock/_stacked.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/mock/_utils.py` & `jj-2.8.0/jj/mock/_utils.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/requests/_request.py` & `jj-2.8.0/jj/requests/_request.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/resolvers/_registry.py` & `jj-2.8.0/jj/resolvers/_registry.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,9 +19,20 @@
 
     def get(self, container: Any, name: str) -> Any:
         if (container not in self._registry) or (name not in self._registry[container]):
             return self._factory()
         return self._registry[container][name]
 
     def remove(self, container: Any, name: str, key: Any) -> None:
+        # backward compatibility
+        return self.remove_key(container, name, key)
+
+    def remove_key(self, container: Any, name: str, key: Any) -> None:
         if (container in self._registry) and (name in self._registry[container]):
             self._registry[container][name].pop(key, None)
+
+    def remove_name(self, container: Any, name: str) -> None:
+        if container in self._registry:
+            self._registry[container].pop(name, None)
+
+    def remove_container(self, container: Any) -> None:
+        self._registry.pop(container, None)
```

### Comparing `jj-2.7.3/jj/resolvers/_resolver.py` & `jj-2.8.0/jj/resolvers/_resolver.py`

 * *Files 11% similar despite different names*

```diff
@@ -70,14 +70,18 @@
         self.register_handler(unwrapped, type(self._default_app))
         self._registry.add(unwrapped, "matchers", matcher)
 
     def deregister_matcher(self, matcher: MatcherFunction, handler: HandlerFunction) -> None:
         unwrapped = self.unwrap(handler)
         self._registry.remove(unwrapped, "matchers", matcher)
 
+        matchers = self._registry.get(unwrapped, "matchers")
+        if len(matchers) == 0:
+            self._registry.remove_name(unwrapped, "matchers")
+
     def get_matchers(self, handler: HandlerFunction) -> List[MatcherFunction]:
         unwrapped = self.unwrap(handler)
         matchers = self._registry.get(unwrapped, "matchers")
         return list(matchers.keys())
 
     # Attributes
 
@@ -85,21 +89,30 @@
         unwrapped = self.unwrap(handler)
         self._registry.add(unwrapped, "attributes", name, value)
 
     def deregister_attribute(self, attribute_name: Any, handler: AppOrHandler) -> None:
         unwrapped = self.unwrap(handler)
         self._registry.remove(unwrapped, "attributes", attribute_name)
 
+        attributes = self._registry.get(unwrapped, "attributes")
+        if len(attributes) == 0:
+            self._registry.remove_name(unwrapped, "attributes")
+
     def get_attribute(self, attribute_name: Any,
                       handler: AppOrHandler,
                       default: Any = nil) -> Any:
         unwrapped = self.unwrap(handler)
         attributes = self._registry.get(unwrapped, "attributes")
         return attributes.get(attribute_name, default)
 
+    def get_attributes(self, handler: AppOrHandler) -> List[Any]:
+        unwrapped = self.unwrap(handler)
+        attributes = self._registry.get(unwrapped, "attributes")
+        return list(attributes.keys())
+
     # Resolve
 
     async def _match_request(self, request: Request, matchers: List[MatcherFunction]) -> bool:
         if len(matchers) == 0:
             return False
         for matcher in matchers:
             if not await matcher(request):
```

### Comparing `jj-2.7.3/jj/responses/_relay_response.py` & `jj-2.8.0/jj/responses/_relay_response.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/responses/_response.py` & `jj-2.8.0/jj/responses/_response.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/responses/_static_response.py` & `jj-2.8.0/jj/responses/_static_response.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/responses/_stream_response.py` & `jj-2.8.0/jj/responses/_stream_response.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/runners/_runner.py` & `jj-2.8.0/jj/runners/_runner.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj/servers/_server.py` & `jj-2.8.0/jj/servers/_server.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.3/jj.egg-info/PKG-INFO` & `jj-2.8.0/jj.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jj
-Version: 2.7.3
+Version: 2.8.0
 Summary: Remote HTTP Mock
 Home-page: https://github.com/tsv1/jj
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `jj-2.7.3/jj.egg-info/SOURCES.txt` & `jj-2.8.0/jj.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE.txt
 README.md
 setup.cfg
 setup.py
 jj/__init__.py
+jj/__main__.py
 jj/_core.py
 jj/_version.py
 jj/py.typed
 jj.egg-info/PKG-INFO
 jj.egg-info/SOURCES.txt
 jj.egg-info/dependency_links.txt
 jj.egg-info/requires.txt
@@ -25,14 +26,15 @@
 jj/http/__init__.py
 jj/http/codes/__init__.py
 jj/http/headers/__init__.py
 jj/http/methods/__init__.py
 jj/logs/__init__.py
 jj/logs/_filter.py
 jj/logs/_logger.py
+jj/logs/_request_filter.py
 jj/logs/formatters/__init__.py
 jj/logs/formatters/_formatter.py
 jj/logs/formatters/_simple_formatter.py
 jj/matchers/__init__.py
 jj/matchers/_resolvable_matcher.py
 jj/matchers/attribute_matchers/__init__.py
 jj/matchers/attribute_matchers/_attribute_matcher.py
@@ -71,14 +73,17 @@
 jj/mock/_history/__init__.py
 jj/mock/_history/_body_parser.py
 jj/mock/_history/_history_adapter.py
 jj/mock/_history/_history_item.py
 jj/mock/_history/_history_repository.py
 jj/mock/_history/_history_request.py
 jj/mock/_history/_history_response.py
+jj/mock/_history/_history_formatter/__init__.py
+jj/mock/_history/_history_formatter/_history_formatter.py
+jj/mock/_history/_history_formatter/_pretty_history_formatter.py
 jj/requests/__init__.py
 jj/requests/_request.py
 jj/resolvers/__init__.py
 jj/resolvers/_matcher_function.py
 jj/resolvers/_registry.py
 jj/resolvers/_resolver.py
 jj/resolvers/_reversed_resolver.py
```

### Comparing `jj-2.7.3/setup.cfg` & `jj-2.8.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.7.3
+current_version = 2.8.0
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `jj-2.7.3/setup.py` & `jj-2.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="jj",
-    version="2.7.3",
+    version="2.8.0",
     description="Remote HTTP Mock",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
     author_email="tsv1@fastmail.com",
     python_requires=">=3.7.0",
     url="https://github.com/tsv1/jj",
```

