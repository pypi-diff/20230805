# Comparing `tmp/servey-2.8.4.tar.gz` & `tmp/servey-2.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servey-2.8.4.tar", last modified: Tue May  9 21:39:32 2023, max compression
+gzip compressed data, was "servey-2.8.5.tar", last modified: Sat Aug  5 19:42:09 2023, max compression
```

## Comparing `servey-2.8.4.tar` & `servey-2.8.5.tar`

### file list

```diff
@@ -1,193 +1,194 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.574175 servey-2.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-09 21:39:21.000000 servey-2.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17792 2023-05-09 21:39:32.574175 servey-2.8.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.542175 servey-2.8.4/marshy_config_servey/
--rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-05-09 21:39:21.000000 servey-2.8.4/marshy_config_servey/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.542175 servey-2.8.4/servey/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-09 21:39:21.000000 servey-2.8.4/servey/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.546175 servey-2.8.4/servey/action/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-09 21:39:21.000000 servey-2.8.4/servey/action/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-09 21:39:21.000000 servey-2.8.4/servey/action/batch_invoker.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-09 21:39:21.000000 servey-2.8.4/servey/action/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-05-09 21:39:21.000000 servey-2.8.4/servey/action/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.550175 servey-2.8.4/servey/cache_control/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/cache_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-09 21:39:21.000000 servey-2.8.4/servey/cache_control/cache_control_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-09 21:39:21.000000 servey-2.8.4/servey/cache_control/cache_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-09 21:39:21.000000 servey-2.8.4/servey/cache_control/secure_hash_cache_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-09 21:39:21.000000 servey-2.8.4/servey/cache_control/timestamp_cache_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-09 21:39:21.000000 servey-2.8.4/servey/cache_control/ttl_cache_control.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-09 21:39:21.000000 servey-2.8.4/servey/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.550175 servey-2.8.4/servey/finder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/finder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-09 21:39:21.000000 servey-2.8.4/servey/finder/action_finder_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-09 21:39:21.000000 servey-2.8.4/servey/finder/module_action_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-09 21:39:21.000000 servey-2.8.4/servey/finder/module_subscription_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-09 21:39:21.000000 servey-2.8.4/servey/finder/subscription_finder_abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.550175 servey-2.8.4/servey/security/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.550175 servey-2.8.4/servey/security/access_control/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/access_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/access_control/access_control_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/access_control/allow_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/access_control/allow_none.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/access_control/scope_access_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.550175 servey-2.8.4/servey/security/authenticator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/authenticator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/authenticator/password_authenticator_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/authenticator/root_password_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/authorization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.550175 servey-2.8.4/servey/security/authorizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/authorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/authorizer/authorizer_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/authorizer/authorizer_factory_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/authorizer/jwt_authorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/authorizer/jwt_authorizer_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.554175 servey-2.8.4/servey/servey_aws/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.554175 servey-2.8.4/servey/servey_aws/authorizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/authorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/authorizer/kms_authorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/authorizer/kms_authorizer_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.554175 servey-2.8.4/servey/servey_aws/event_handler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/event_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/event_handler/api_gateway_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/event_handler/appsync_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/event_handler/event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/event_handler/event_handler_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/event_handler/sqs_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/lambda_invoker.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/lambda_router.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/lambda_websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.554175 servey-2.8.4/servey/servey_aws/router/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/router/api_gateway_router.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/router/appsync_router.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/router/router.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/router/router_abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.554175 servey-2.8.4/servey/servey_aws/serverless/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.558175 servey-2.8.4/servey/servey_aws/serverless/trigger_handler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/trigger_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/trigger_handler/fixed_rate_trigger_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/trigger_handler/trigger_handler_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/trigger_handler/web_trigger_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.558175 servey-2.8.4/servey/servey_aws/serverless/yml_config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/yml_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/yml_config/action_function_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/yml_config/appsync_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/yml_config/cloudfront_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/yml_config/kms_key_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/yml_config/serverless_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/yml_config/static_site_bucket_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/yml_config/subscription_function_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/yml_config/yml_config_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/sqs_subscription_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/websocket_subscription_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.558175 servey-2.8.4/servey/servey_celery/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_celery/celery_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.558175 servey-2.8.4/servey/servey_celery/celery_config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_celery/celery_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_celery/celery_config/celery_config_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_celery/celery_config/fixed_rate_trigger_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_celery/celery_config/subscription_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_celery/celery_subscription_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.558175 servey-2.8.4/servey/servey_direct/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_direct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_direct/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.562175 servey-2.8.4/servey/servey_starlette/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.562175 servey-2.8.4/servey/servey_starlette/action_endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/action_endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11902 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/action_endpoint/action_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/action_endpoint/action_endpoint_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/action_endpoint/authorizing_action_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/action_endpoint/caching_action_endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.562175 servey-2.8.4/servey/servey_starlette/action_endpoint/factory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/action_endpoint/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/action_endpoint/factory/action_endpoint_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/action_endpoint/factory/action_endpoint_factory_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/action_endpoint/factory/authorizing_action_endpoint_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/action_endpoint/factory/caching_action_endpoint_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/action_endpoint/factory/self_action_endpoint_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/error_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.566175 servey-2.8.4/servey/servey_starlette/route_factory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/route_factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/route_factory/action_route_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/route_factory/asyncapi_route_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/route_factory/authenticator_route_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/route_factory/openapi_route_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/route_factory/route_factory_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/route_factory/static_site_route_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/route_factory/subscription_route_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/starlette_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.566175 servey-2.8.4/servey/servey_starlette/statics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/statics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/statics/index.html
--rw-r--r--   0 runner    (1001) docker     (123)  1079398 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/statics/swagger-ui-bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   192198 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/statics/swagger-ui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.566175 servey-2.8.4/servey/servey_strawberry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.570175 servey-2.8.4/servey/servey_strawberry/entity_factory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/entity_factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/entity_factory/dataclass_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/entity_factory/entity_factory_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/entity_factory/enum_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/entity_factory/forward_ref_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/entity_factory/generic_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/entity_factory/no_op_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.570175 servey-2.8.4/servey/servey_strawberry/handler_filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/handler_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/handler_filter/authorization_handler_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/handler_filter/handler_filter_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/handler_filter/strawberry_type_handler_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/schema_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/schema_factory_lazy_input.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/schema_factory_lazy_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.570175 servey-2.8.4/servey/servey_strawberry/statics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/statics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/statics/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/strawberry_starlette_route_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.570175 servey-2.8.4/servey/servey_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_test/test_servey_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.570175 servey-2.8.4/servey/servey_thread/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_thread/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_thread/asyncio_subscription_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_thread/fixed_rate_trigger_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.574175 servey-2.8.4/servey/servey_web_page/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_web_page/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_web_page/redirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_web_page/web_page_action_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_web_page/web_page_action_endpoint_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_web_page/web_page_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_web_page/web_page_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_web_page/web_page_trigger_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.574175 servey-2.8.4/servey/subscription/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-09 21:39:21.000000 servey-2.8.4/servey/subscription/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-09 21:39:21.000000 servey-2.8.4/servey/subscription/event_filter_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-09 21:39:21.000000 servey-2.8.4/servey/subscription/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-09 21:39:21.000000 servey-2.8.4/servey/subscription/subscription_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-09 21:39:21.000000 servey-2.8.4/servey/subscription/subscription_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.574175 servey-2.8.4/servey/trigger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/trigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-09 21:39:21.000000 servey-2.8.4/servey/trigger/fixed_rate_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-09 21:39:21.000000 servey-2.8.4/servey/trigger/trigger_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-09 21:39:21.000000 servey-2.8.4/servey/trigger/web_trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.574175 servey-2.8.4/servey/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-09 21:39:21.000000 servey-2.8.4/servey/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-09 21:39:21.000000 servey-2.8.4/servey/util/singleton_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-09 21:39:21.000000 servey-2.8.4/servey/util/to_second_datetime_marshaller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.546175 servey-2.8.4/servey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17792 2023-05-09 21:39:32.000000 servey-2.8.4/servey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-05-09 21:39:32.000000 servey-2.8.4/servey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 21:39:32.000000 servey-2.8.4/servey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-09 21:39:32.000000 servey-2.8.4/servey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 21:39:32.000000 servey-2.8.4/servey.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 21:39:32.574175 servey-2.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-09 21:39:21.000000 servey-2.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.843023 servey-2.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-05 19:41:59.000000 servey-2.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17792 2023-08-05 19:42:09.843023 servey-2.8.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.807021 servey-2.8.5/marshy_config_servey/
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-08-05 19:41:59.000000 servey-2.8.5/marshy_config_servey/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.811021 servey-2.8.5/servey/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-08-05 19:41:59.000000 servey-2.8.5/servey/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.815021 servey-2.8.5/servey/action/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-08-05 19:41:59.000000 servey-2.8.5/servey/action/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-05 19:41:59.000000 servey-2.8.5/servey/action/batch_invoker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-05 19:41:59.000000 servey-2.8.5/servey/action/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-08-05 19:41:59.000000 servey-2.8.5/servey/action/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.815021 servey-2.8.5/servey/cache_control/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/cache_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-05 19:41:59.000000 servey-2.8.5/servey/cache_control/cache_control_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-08-05 19:41:59.000000 servey-2.8.5/servey/cache_control/cache_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-05 19:41:59.000000 servey-2.8.5/servey/cache_control/secure_hash_cache_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-08-05 19:41:59.000000 servey-2.8.5/servey/cache_control/timestamp_cache_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-08-05 19:41:59.000000 servey-2.8.5/servey/cache_control/ttl_cache_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-08-05 19:41:59.000000 servey-2.8.5/servey/cors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-05 19:41:59.000000 servey-2.8.5/servey/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.819022 servey-2.8.5/servey/finder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/finder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-05 19:41:59.000000 servey-2.8.5/servey/finder/action_finder_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-08-05 19:41:59.000000 servey-2.8.5/servey/finder/module_action_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-05 19:41:59.000000 servey-2.8.5/servey/finder/module_subscription_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-05 19:41:59.000000 servey-2.8.5/servey/finder/subscription_finder_abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.819022 servey-2.8.5/servey/security/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/security/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.819022 servey-2.8.5/servey/security/access_control/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/security/access_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-05 19:41:59.000000 servey-2.8.5/servey/security/access_control/access_control_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-05 19:41:59.000000 servey-2.8.5/servey/security/access_control/allow_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-05 19:41:59.000000 servey-2.8.5/servey/security/access_control/allow_none.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-05 19:41:59.000000 servey-2.8.5/servey/security/access_control/scope_access_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.819022 servey-2.8.5/servey/security/authenticator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/security/authenticator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-05 19:41:59.000000 servey-2.8.5/servey/security/authenticator/password_authenticator_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-05 19:41:59.000000 servey-2.8.5/servey/security/authenticator/root_password_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-08-05 19:41:59.000000 servey-2.8.5/servey/security/authorization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.823022 servey-2.8.5/servey/security/authorizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/security/authorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-05 19:41:59.000000 servey-2.8.5/servey/security/authorizer/authorizer_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-05 19:41:59.000000 servey-2.8.5/servey/security/authorizer/authorizer_factory_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-08-05 19:41:59.000000 servey-2.8.5/servey/security/authorizer/jwt_authorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-05 19:41:59.000000 servey-2.8.5/servey/security/authorizer/jwt_authorizer_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.823022 servey-2.8.5/servey/servey_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.823022 servey-2.8.5/servey/servey_aws/authorizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/authorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/authorizer/kms_authorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/authorizer/kms_authorizer_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.827022 servey-2.8.5/servey/servey_aws/event_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/event_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/event_handler/api_gateway_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/event_handler/appsync_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/event_handler/event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/event_handler/event_handler_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/event_handler/sqs_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/lambda_invoker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/lambda_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/lambda_websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.827022 servey-2.8.5/servey/servey_aws/router/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/router/api_gateway_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/router/appsync_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/router/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/router/router_abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.827022 servey-2.8.5/servey/servey_aws/serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/serverless/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.827022 servey-2.8.5/servey/servey_aws/serverless/trigger_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/serverless/trigger_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/serverless/trigger_handler/fixed_rate_trigger_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/serverless/trigger_handler/trigger_handler_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/serverless/trigger_handler/web_trigger_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.827022 servey-2.8.5/servey/servey_aws/serverless/yml_config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/serverless/yml_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/serverless/yml_config/action_function_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/serverless/yml_config/appsync_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/serverless/yml_config/cloudfront_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/serverless/yml_config/kms_key_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/serverless/yml_config/serverless_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/serverless/yml_config/static_site_bucket_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/serverless/yml_config/subscription_function_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/serverless/yml_config/yml_config_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/sqs_subscription_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_aws/websocket_subscription_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.831022 servey-2.8.5/servey/servey_celery/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_celery/celery_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.831022 servey-2.8.5/servey/servey_celery/celery_config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_celery/celery_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_celery/celery_config/celery_config_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_celery/celery_config/fixed_rate_trigger_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_celery/celery_config/subscription_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_celery/celery_subscription_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.831022 servey-2.8.5/servey/servey_direct/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_direct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_direct/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.831022 servey-2.8.5/servey/servey_starlette/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.831022 servey-2.8.5/servey/servey_starlette/action_endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/action_endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11902 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/action_endpoint/action_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/action_endpoint/action_endpoint_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/action_endpoint/authorizing_action_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/action_endpoint/caching_action_endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.831022 servey-2.8.5/servey/servey_starlette/action_endpoint/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/action_endpoint/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/action_endpoint/factory/action_endpoint_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/action_endpoint/factory/action_endpoint_factory_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/action_endpoint/factory/authorizing_action_endpoint_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/action_endpoint/factory/caching_action_endpoint_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/action_endpoint/factory/self_action_endpoint_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/error_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.835022 servey-2.8.5/servey/servey_starlette/route_factory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/route_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/route_factory/action_route_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/route_factory/asyncapi_route_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/route_factory/authenticator_route_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/route_factory/openapi_route_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/route_factory/route_factory_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/route_factory/static_site_route_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/route_factory/subscription_route_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/starlette_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.835022 servey-2.8.5/servey/servey_starlette/statics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/statics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/statics/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)  1079398 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/statics/swagger-ui-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   192198 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_starlette/statics/swagger-ui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.835022 servey-2.8.5/servey/servey_strawberry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_strawberry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.839022 servey-2.8.5/servey/servey_strawberry/entity_factory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_strawberry/entity_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_strawberry/entity_factory/dataclass_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_strawberry/entity_factory/entity_factory_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_strawberry/entity_factory/enum_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_strawberry/entity_factory/forward_ref_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_strawberry/entity_factory/generic_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_strawberry/entity_factory/no_op_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.839022 servey-2.8.5/servey/servey_strawberry/handler_filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_strawberry/handler_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_strawberry/handler_filter/authorization_handler_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_strawberry/handler_filter/handler_filter_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_strawberry/handler_filter/strawberry_type_handler_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_strawberry/schema_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_strawberry/schema_factory_lazy_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_strawberry/schema_factory_lazy_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.839022 servey-2.8.5/servey/servey_strawberry/statics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_strawberry/statics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_strawberry/statics/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_strawberry/strawberry_starlette_route_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.839022 servey-2.8.5/servey/servey_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_test/test_servey_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.839022 servey-2.8.5/servey/servey_thread/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_thread/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_thread/asyncio_subscription_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_thread/fixed_rate_trigger_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.843023 servey-2.8.5/servey/servey_web_page/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_web_page/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_web_page/redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_web_page/web_page_action_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_web_page/web_page_action_endpoint_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_web_page/web_page_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_web_page/web_page_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-05 19:41:59.000000 servey-2.8.5/servey/servey_web_page/web_page_trigger_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.843023 servey-2.8.5/servey/subscription/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-05 19:41:59.000000 servey-2.8.5/servey/subscription/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-05 19:41:59.000000 servey-2.8.5/servey/subscription/event_filter_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-08-05 19:41:59.000000 servey-2.8.5/servey/subscription/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-05 19:41:59.000000 servey-2.8.5/servey/subscription/subscription_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-08-05 19:41:59.000000 servey-2.8.5/servey/subscription/subscription_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.843023 servey-2.8.5/servey/trigger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:41:59.000000 servey-2.8.5/servey/trigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-05 19:41:59.000000 servey-2.8.5/servey/trigger/fixed_rate_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-05 19:41:59.000000 servey-2.8.5/servey/trigger/trigger_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-05 19:41:59.000000 servey-2.8.5/servey/trigger/web_trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.843023 servey-2.8.5/servey/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-05 19:41:59.000000 servey-2.8.5/servey/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-08-05 19:41:59.000000 servey-2.8.5/servey/util/singleton_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-05 19:41:59.000000 servey-2.8.5/servey/util/to_second_datetime_marshaller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:42:09.811021 servey-2.8.5/servey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17792 2023-08-05 19:42:09.000000 servey-2.8.5/servey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-08-05 19:42:09.000000 servey-2.8.5/servey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 19:42:09.000000 servey-2.8.5/servey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-05 19:42:09.000000 servey-2.8.5/servey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-05 19:42:09.000000 servey-2.8.5/servey.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 19:42:09.843023 servey-2.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-08-05 19:41:59.000000 servey-2.8.5/setup.py
```

### Comparing `servey-2.8.4/PKG-INFO` & `servey-2.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servey
-Version: 2.8.4
+Version: 2.8.5
 Summary: A better API layer for python
 Home-page: https://github.com/tofarr/servey
 Author: Tim O'Farrell
 Author-email: tofarr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `servey-2.8.4/marshy_config_servey/__init__.py` & `servey-2.8.5/marshy_config_servey/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     register_impl(PasswordAuthenticatorABC, RootPasswordAuthenticator, context)
 
 
 def configure_starlette(context: MarshallerContext):
     try:
         configure_starlette_action_endpoint_factory(context)
         configure_starlette_route_factory(context)
+        configure_starlette_middleware_factory(context)
     except ModuleNotFoundError as e:
         raise_non_ignored(e)
 
 
 def configure_starlette_action_endpoint_factory(context: MarshallerContext):
     from servey.servey_starlette.action_endpoint.factory.action_endpoint_factory_abc import (
         ActionEndpointFactoryABC,
@@ -122,14 +123,25 @@
     register_impl(RouteFactoryABC, OpenapiRouteFactory, context)
     register_impl(RouteFactoryABC, SubscriptionRouteFactory, context)
     register_impl(SubscriptionServiceFactoryABC, SubscriptionRouteFactory, context)
     register_impl(RouteFactoryABC, AsyncapiRouteFactory, context)
     register_impl(RouteFactoryABC, StaticSiteRouteFactory, context)
 
 
+def configure_starlette_middleware_factory(context: MarshallerContext):
+    from servey.servey_starlette.middleware.middleware_factory_abc import (
+        MiddlewareFactoryABC,
+    )
+    from servey.servey_starlette.middleware.cors_middleware_factory import (
+        CORSMiddlewareFactory,
+    )
+
+    register_impl(MiddlewareFactoryABC, CORSMiddlewareFactory, context)
+
+
 def configure_strawberry(context: MarshallerContext):
     try:
         from servey.servey_strawberry.handler_filter.handler_filter_abc import (
             HandlerFilterABC,
         )
         from servey.servey_strawberry.handler_filter.authorization_handler_filter import (
             AuthorizationHandlerFilter,
```

### Comparing `servey-2.8.4/servey/__main__.py` & `servey-2.8.5/servey/__main__.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/action/action.py` & `servey-2.8.5/servey/action/action.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/action/util.py` & `servey-2.8.5/servey/action/util.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/cache_control/cache_header.py` & `servey-2.8.5/servey/cache_control/cache_header.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/cache_control/secure_hash_cache_control.py` & `servey-2.8.5/servey/cache_control/secure_hash_cache_control.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/cache_control/timestamp_cache_control.py` & `servey-2.8.5/servey/cache_control/timestamp_cache_control.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/cache_control/ttl_cache_control.py` & `servey-2.8.5/servey/cache_control/ttl_cache_control.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/finder/action_finder_abc.py` & `servey-2.8.5/servey/finder/action_finder_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/finder/module_action_finder.py` & `servey-2.8.5/servey/finder/module_action_finder.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/finder/module_subscription_finder.py` & `servey-2.8.5/servey/finder/module_subscription_finder.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/finder/subscription_finder_abc.py` & `servey-2.8.5/servey/finder/subscription_finder_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/security/access_control/scope_access_control.py` & `servey-2.8.5/servey/security/access_control/scope_access_control.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/security/authenticator/password_authenticator_abc.py` & `servey-2.8.5/servey/security/authenticator/password_authenticator_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/security/authenticator/root_password_authenticator.py` & `servey-2.8.5/servey/security/authenticator/root_password_authenticator.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/security/authorization.py` & `servey-2.8.5/servey/security/authorization.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/security/authorizer/authorizer_factory_abc.py` & `servey-2.8.5/servey/security/authorizer/authorizer_factory_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/security/authorizer/jwt_authorizer.py` & `servey-2.8.5/servey/security/authorizer/jwt_authorizer.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/security/authorizer/jwt_authorizer_factory.py` & `servey-2.8.5/servey/security/authorizer/jwt_authorizer_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/authorizer/kms_authorizer.py` & `servey-2.8.5/servey/servey_aws/authorizer/kms_authorizer.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/authorizer/kms_authorizer_factory.py` & `servey-2.8.5/servey/servey_aws/authorizer/kms_authorizer_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/event_handler/api_gateway_event_handler.py` & `servey-2.8.5/servey/servey_aws/event_handler/api_gateway_event_handler.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/event_handler/appsync_event_handler.py` & `servey-2.8.5/servey/servey_aws/event_handler/appsync_event_handler.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/event_handler/event_handler.py` & `servey-2.8.5/servey/servey_aws/event_handler/event_handler.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/event_handler/event_handler_abc.py` & `servey-2.8.5/servey/servey_aws/event_handler/event_handler_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/event_handler/sqs_event_handler.py` & `servey-2.8.5/servey/servey_aws/event_handler/sqs_event_handler.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/lambda_invoker.py` & `servey-2.8.5/servey/servey_aws/lambda_invoker.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/lambda_router.py` & `servey-2.8.5/servey/servey_aws/lambda_router.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/lambda_websocket.py` & `servey-2.8.5/servey/servey_aws/lambda_websocket.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/router/api_gateway_router.py` & `servey-2.8.5/servey/servey_aws/router/api_gateway_router.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/router/appsync_router.py` & `servey-2.8.5/servey/servey_aws/router/appsync_router.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/router/router.py` & `servey-2.8.5/servey/servey_aws/router/router.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/router/router_abc.py` & `servey-2.8.5/servey/servey_aws/router/router_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/serverless/__main__.py` & `servey-2.8.5/servey/servey_aws/serverless/__main__.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/serverless/trigger_handler/fixed_rate_trigger_handler.py` & `servey-2.8.5/servey/servey_aws/serverless/trigger_handler/fixed_rate_trigger_handler.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/serverless/trigger_handler/web_trigger_handler.py` & `servey-2.8.5/servey/servey_aws/serverless/trigger_handler/web_trigger_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from marshy.types import ExternalItemType
 
 from servey.action.action import Action
+from servey.cors import get_allowed_origins
+from servey.errors import ServeyError
 from servey.trigger.trigger_abc import TriggerABC
 from servey.trigger.web_trigger import WebTrigger
 from servey.servey_aws.serverless.trigger_handler.trigger_handler_abc import (
     TriggerHandlerABC,
 )
 
 
@@ -25,10 +27,17 @@
             return
         events = lambda_definition.get("events")
         if not events:
             events = lambda_definition["events"] = []
         path = trigger.path or self.path_pattern.format(
             action_name=action.name.replace("_", "-")
         )
-        events.append(
-            {"http": {"path": path, "method": trigger.method.value, "cors": True}}
-        )
+        event = {"http": {"path": path, "method": trigger.method.value}}
+        allowed_origins = get_allowed_origins()
+        if allowed_origins:
+            if len(allowed_origins) > 1:
+                raise ServeyError("multi_origin_unsupported")
+            event["http"]["cors"] = {
+                "origin": allowed_origins[0],
+                "allowCredentials": True,
+            }
+        events.append(event)
```

### Comparing `servey-2.8.4/servey/servey_aws/serverless/yml_config/action_function_config.py` & `servey-2.8.5/servey/servey_aws/serverless/yml_config/action_function_config.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/serverless/yml_config/appsync_config.py` & `servey-2.8.5/servey/servey_aws/serverless/yml_config/appsync_config.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/serverless/yml_config/cloudfront_config.py` & `servey-2.8.5/servey/servey_aws/serverless/yml_config/cloudfront_config.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/serverless/yml_config/kms_key_config.py` & `servey-2.8.5/servey/servey_aws/serverless/yml_config/kms_key_config.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/serverless/yml_config/serverless_template.yml` & `servey-2.8.5/servey/servey_aws/serverless/yml_config/serverless_template.yml`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/serverless/yml_config/static_site_bucket_config.py` & `servey-2.8.5/servey/servey_aws/serverless/yml_config/static_site_bucket_config.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/serverless/yml_config/subscription_function_config.py` & `servey-2.8.5/servey/servey_aws/serverless/yml_config/subscription_function_config.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/serverless/yml_config/yml_config_abc.py` & `servey-2.8.5/servey/servey_aws/serverless/yml_config/yml_config_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/sqs_subscription_service.py` & `servey-2.8.5/servey/servey_aws/sqs_subscription_service.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_aws/websocket_subscription_service.py` & `servey-2.8.5/servey/servey_aws/websocket_subscription_service.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_celery/celery_app.py` & `servey-2.8.5/servey/servey_celery/celery_app.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_celery/celery_config/fixed_rate_trigger_config.py` & `servey-2.8.5/servey/servey_celery/celery_config/fixed_rate_trigger_config.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_celery/celery_config/subscription_config.py` & `servey-2.8.5/servey/servey_celery/celery_config/subscription_config.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_celery/celery_subscription_service.py` & `servey-2.8.5/servey/servey_celery/celery_subscription_service.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_direct/__main__.py` & `servey-2.8.5/servey/servey_direct/__main__.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_starlette/action_endpoint/action_endpoint.py` & `servey-2.8.5/servey/servey_starlette/action_endpoint/action_endpoint.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_starlette/action_endpoint/action_endpoint_abc.py` & `servey-2.8.5/servey/servey_starlette/action_endpoint/action_endpoint_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_starlette/action_endpoint/authorizing_action_endpoint.py` & `servey-2.8.5/servey/servey_starlette/action_endpoint/authorizing_action_endpoint.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_starlette/action_endpoint/caching_action_endpoint.py` & `servey-2.8.5/servey/servey_starlette/action_endpoint/caching_action_endpoint.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_starlette/action_endpoint/factory/action_endpoint_factory.py` & `servey-2.8.5/servey/servey_starlette/action_endpoint/factory/action_endpoint_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_starlette/action_endpoint/factory/action_endpoint_factory_abc.py` & `servey-2.8.5/servey/servey_starlette/action_endpoint/factory/action_endpoint_factory_abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from servey.action.action import Action
 from servey.servey_starlette.action_endpoint.action_endpoint_abc import (
     ActionEndpointABC,
 )
 
 
 class ActionEndpointFactoryABC(ABC):
-    priority: 100
+    priority: int = 100
 
     @abstractmethod
     def create(
         self,
         action: Action,
         skip_args: Set[str],
         factories: List[ActionEndpointFactoryABC],
```

### Comparing `servey-2.8.4/servey/servey_starlette/action_endpoint/factory/authorizing_action_endpoint_factory.py` & `servey-2.8.5/servey/servey_starlette/action_endpoint/factory/authorizing_action_endpoint_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_starlette/action_endpoint/factory/caching_action_endpoint_factory.py` & `servey-2.8.5/servey/servey_starlette/action_endpoint/factory/caching_action_endpoint_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_starlette/action_endpoint/factory/self_action_endpoint_factory.py` & `servey-2.8.5/servey/servey_starlette/action_endpoint/factory/self_action_endpoint_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_starlette/route_factory/action_route_factory.py` & `servey-2.8.5/servey/servey_starlette/route_factory/action_route_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_starlette/route_factory/asyncapi_route_factory.py` & `servey-2.8.5/servey/servey_starlette/route_factory/asyncapi_route_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_starlette/route_factory/authenticator_route_factory.py` & `servey-2.8.5/servey/servey_starlette/route_factory/authenticator_route_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_starlette/route_factory/openapi_route_factory.py` & `servey-2.8.5/servey/servey_starlette/route_factory/openapi_route_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_starlette/route_factory/static_site_route_factory.py` & `servey-2.8.5/servey/servey_starlette/route_factory/static_site_route_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_starlette/route_factory/subscription_route_factory.py` & `servey-2.8.5/servey/servey_starlette/route_factory/subscription_route_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_starlette/starlette_app.py` & `servey-2.8.5/servey/servey_starlette/starlette_app.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,32 @@
 import logging
 
 from marshy.factory.impl_marshaller_factory import get_impls
 from starlette.applications import Starlette
 
+from servey.servey_starlette.middleware.middleware_factory_abc import (
+    MiddlewareFactoryABC,
+)
 from servey.servey_starlette.route_factory.route_factory_abc import RouteFactoryABC
 
 LOGGER = logging.getLogger(__name__)
 routes = []
 for route_factory in sorted(
     list(get_impls(RouteFactoryABC)), key=lambda f: f.priority, reverse=True
 ):
     routes.extend(route_factory().create_routes())
 for route in routes:
     LOGGER.debug("starlette_path:%s", route.path)
 
-app = Starlette(routes=routes)
+middleware = [
+    f
+    for f in (
+        f.create()
+        for f in sorted(
+            [f() for f in get_impls(MiddlewareFactoryABC)],
+            key=lambda f: f.priority,
+            reverse=True,
+        )
+    )
+    if f
+]
+app = Starlette(routes=routes, middleware=middleware)
```

### Comparing `servey-2.8.4/servey/servey_starlette/statics/index.html` & `servey-2.8.5/servey/servey_starlette/statics/index.html`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_starlette/statics/swagger-ui-bundle.js` & `servey-2.8.5/servey/servey_starlette/statics/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_starlette/statics/swagger-ui.css` & `servey-2.8.5/servey/servey_starlette/statics/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_strawberry/entity_factory/dataclass_factory.py` & `servey-2.8.5/servey/servey_strawberry/entity_factory/dataclass_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_strawberry/entity_factory/entity_factory_abc.py` & `servey-2.8.5/servey/servey_strawberry/entity_factory/entity_factory_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_strawberry/entity_factory/enum_factory.py` & `servey-2.8.5/servey/servey_strawberry/entity_factory/enum_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_strawberry/entity_factory/forward_ref_factory.py` & `servey-2.8.5/servey/servey_strawberry/entity_factory/forward_ref_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_strawberry/entity_factory/generic_factory.py` & `servey-2.8.5/servey/servey_strawberry/entity_factory/generic_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_strawberry/entity_factory/no_op_factory.py` & `servey-2.8.5/servey/servey_strawberry/entity_factory/no_op_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_strawberry/handler_filter/authorization_handler_filter.py` & `servey-2.8.5/servey/servey_strawberry/handler_filter/authorization_handler_filter.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_strawberry/handler_filter/handler_filter_abc.py` & `servey-2.8.5/servey/servey_strawberry/handler_filter/handler_filter_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_strawberry/handler_filter/strawberry_type_handler_filter.py` & `servey-2.8.5/servey/servey_strawberry/handler_filter/strawberry_type_handler_filter.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_strawberry/schema_factory.py` & `servey-2.8.5/servey/servey_strawberry/schema_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             self.query[f.name] = f
 
     # pylint: disable=R0911
     def _resolve_type_futures(self, type_, resolved: Set):
         if isinstance(type_, str):
             type_ = self.types[type_]
         if isinstance(type_, StrawberryAnnotation):
-            type_.type = self._resolve_type_futures(type_.annotation, resolved)
+            type_.annotation = self._resolve_type_futures(type_.annotation, resolved)
             return type_
         if isinstance(type_, StrawberryContainer):
             type_.of_type = self._resolve_type_futures(type_.of_type, resolved)
             return type_
         name = typing_inspect.get_forward_arg(type_)
         if name:
             type_ = self.types[name]
```

### Comparing `servey-2.8.4/servey/servey_strawberry/schema_factory_lazy_input.py` & `servey-2.8.5/servey/servey_strawberry/schema_factory_lazy_input.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_strawberry/schema_factory_lazy_type.py` & `servey-2.8.5/servey/servey_strawberry/schema_factory_lazy_type.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_strawberry/statics/index.html` & `servey-2.8.5/servey/servey_strawberry/statics/index.html`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_strawberry/strawberry_starlette_route_factory.py` & `servey-2.8.5/servey/servey_strawberry/strawberry_starlette_route_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_test/test_servey_actions.py` & `servey-2.8.5/servey/servey_test/test_servey_actions.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_thread/__main__.py` & `servey-2.8.5/servey/servey_thread/__main__.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_thread/asyncio_subscription_service.py` & `servey-2.8.5/servey/servey_thread/asyncio_subscription_service.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_thread/fixed_rate_trigger_thread.py` & `servey-2.8.5/servey/servey_thread/fixed_rate_trigger_thread.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_web_page/web_page_action_endpoint.py` & `servey-2.8.5/servey/servey_web_page/web_page_action_endpoint.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_web_page/web_page_action_endpoint_factory.py` & `servey-2.8.5/servey/servey_web_page/web_page_action_endpoint_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_web_page/web_page_event_handler.py` & `servey-2.8.5/servey/servey_web_page/web_page_event_handler.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_web_page/web_page_trigger.py` & `servey-2.8.5/servey/servey_web_page/web_page_trigger.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/servey_web_page/web_page_trigger_handler.py` & `servey-2.8.5/servey/servey_web_page/web_page_trigger_handler.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/subscription/__init__.py` & `servey-2.8.5/servey/subscription/__init__.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/subscription/subscription.py` & `servey-2.8.5/servey/subscription/subscription.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/subscription/subscription_event.py` & `servey-2.8.5/servey/subscription/subscription_event.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/subscription/subscription_service.py` & `servey-2.8.5/servey/subscription/subscription_service.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/trigger/web_trigger.py` & `servey-2.8.5/servey/trigger/web_trigger.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/util/__init__.py` & `servey-2.8.5/servey/util/__init__.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey/util/singleton_abc.py` & `servey-2.8.5/servey/util/singleton_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.4/servey.egg-info/PKG-INFO` & `servey-2.8.5/servey.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servey
-Version: 2.8.4
+Version: 2.8.5
 Summary: A better API layer for python
 Home-page: https://github.com/tofarr/servey
 Author: Tim O'Farrell
 Author-email: tofarr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `servey-2.8.4/servey.egg-info/SOURCES.txt` & `servey-2.8.5/servey.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 MANIFEST.in
 setup.py
 marshy_config_servey/__init__.py
 servey/__init__.py
 servey/__main__.py
+servey/cors.py
 servey/errors.py
 servey.egg-info/PKG-INFO
 servey.egg-info/SOURCES.txt
 servey.egg-info/dependency_links.txt
 servey.egg-info/requires.txt
 servey.egg-info/top_level.txt
 servey/action/__init__.py
```

### Comparing `servey-2.8.4/servey.egg-info/requires.txt` & `servey-2.8.5/servey.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,30 +2,31 @@
 json-urley~=1.0
 marshy~=4.0
 pyjwt~=2.4
 python-dateutil~=2.8
 schemey~=6.0
 
 [all]
-pytest-xdist~=3.2
-celery~=5.2
 ruamel.yaml~=0.17
-pytest-cov~=4.0
+pytest-xdist~=3.2
 pygments~=2.13
-starlette~=0.19
-pytest~=7.2
 requests~=2.28
+uvicorn[standard]~=0.18
+pytest-cov~=4.0
+Jinja2~=3.1
+starlette~=0.19
+strawberry-graphql~=0.151
 black~=23.3
+celery~=5.2
 boto3~=1.26
-Jinja2~=3.1
-python-multipart~=0.0
+pytest~=7.2
 pyyaml~=6.0
-uvicorn[standard]~=0.18
+strawberry-graphql~=0.177
 pylint~=2.17
-strawberry-graphql~=0.151
+python-multipart~=0.0
 
 [dev]
 black~=23.3
 boto3~=1.26
 pytest~=7.2
 pytest-cov~=4.0
 pytest-xdist~=3.2
@@ -41,11 +42,11 @@
 pygments~=2.13
 requests~=2.28
 python-multipart~=0.0
 
 [serverless]
 pyyaml~=6.0
 ruamel.yaml~=0.17
-strawberry-graphql~=0.151
+strawberry-graphql~=0.177
 
 [web_page]
 Jinja2~=3.1
```

### Comparing `servey-2.8.4/setup.py` & `servey-2.8.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         "requests~=2.28",
         "python-multipart~=0.0",
     ],
     "scheduler": ["celery~=5.2"],
     "serverless": [
         "pyyaml~=6.0",
         "ruamel.yaml~=0.17",
-        "strawberry-graphql~=0.151",  # We need this to generate the graphql schema - or do we?
+        "strawberry-graphql~=0.177",  # We need this to generate the graphql schema - or do we?
     ],
     "web_page": [
         "Jinja2~=3.1",
     ],
 }
 extras_require["all"] = list(
     {
```

