# Comparing `tmp/syft-0.8.2b6.tar.gz` & `tmp/syft-0.8.2b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.2b6.tar", last modified: Mon Jul 17 15:39:19 2023, max compression
+gzip compressed data, was "syft-0.8.2b7.tar", last modified: Sat Aug  5 12:23:10 2023, max compression
```

## Comparing `syft-0.8.2b6.tar` & `syft-0.8.2b7.tar`

### file list

```diff
@@ -1,214 +1,228 @@
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.509721 syft-0.8.2b6/
--rw-r--r--   0 om        (1001) users      (100)    11843 2023-07-17 15:37:23.000000 syft-0.8.2b6/LICENSE
--rw-r--r--   0 om        (1001) users      (100)       98 2023-07-17 15:37:23.000000 syft-0.8.2b6/MANIFEST.in
--rw-r--r--   0 om        (1001) users      (100)    16852 2023-07-17 15:39:19.509721 syft-0.8.2b6/PKG-INFO
--rw-r--r--   0 om        (1001) users      (100)    16170 2023-07-17 15:37:23.000000 syft-0.8.2b6/README.md
--rw-r--r--   0 om        (1001) users      (100)      272 2023-07-17 15:37:23.000000 syft-0.8.2b6/pyproject.toml
--rw-r--r--   0 om        (1001) users      (100)     3210 2023-07-17 15:39:19.513721 syft-0.8.2b6/setup.cfg
--rw-r--r--   0 om        (1001) users      (100)      107 2023-07-17 15:37:23.000000 syft-0.8.2b6/setup.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.493721 syft-0.8.2b6/src/
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.493721 syft-0.8.2b6/src/syft/
--rw-r--r--   0 om        (1001) users      (100)      580 2023-07-17 15:37:26.000000 syft-0.8.2b6/src/syft/VERSION
--rw-r--r--   0 om        (1001) users      (100)     5750 2023-07-17 15:37:26.000000 syft-0.8.2b6/src/syft/__init__.py
--rw-r--r--   0 om        (1001) users      (100)       93 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/__main__.py
--rw-r--r--   0 om        (1001) users      (100)      790 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/abstract_node.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.497721 syft-0.8.2b6/src/syft/capnp/
--rw-r--r--   0 om        (1001) users      (100)      270 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/capnp/__init__.py
--rw-r--r--   0 om        (1001) users      (100)       75 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/capnp/iterable.capnp
--rw-r--r--   0 om        (1001) users      (100)      102 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 om        (1001) users      (100)      186 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.497721 syft-0.8.2b6/src/syft/client/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/client/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    26545 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/client/api.py
--rw-r--r--   0 om        (1001) users      (100)    28762 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/client/client.py
--rw-r--r--   0 om        (1001) users      (100)      568 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/client/connection.py
--rw-r--r--   0 om        (1001) users      (100)      650 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/client/deploy.py
--rw-r--r--   0 om        (1001) users      (100)     9211 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/client/domain_client.py
--rw-r--r--   0 om        (1001) users      (100)     6924 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/client/enclave_client.py
--rw-r--r--   0 om        (1001) users      (100)     6404 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/client/gateway_client.py
--rw-r--r--   0 om        (1001) users      (100)    15257 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/client/registry.py
--rw-r--r--   0 om        (1001) users      (100)     2623 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/client/search.py
--rw-r--r--   0 om        (1001) users      (100)      549 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/client/user_settings.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.497721 syft-0.8.2b6/src/syft/external/
--rw-r--r--   0 om        (1001) users      (100)     1735 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/external/__init__.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.497721 syft-0.8.2b6/src/syft/external/oblv/
--rw-r--r--   0 om        (1001) users      (100)      860 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/external/oblv/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      284 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/external/oblv/auth.py
--rw-r--r--   0 om        (1001) users      (100)      212 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/external/oblv/constants.py
--rw-r--r--   0 om        (1001) users      (100)     4835 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/external/oblv/deployment.py
--rw-r--r--   0 om        (1001) users      (100)    12380 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/external/oblv/deployment_client.py
--rw-r--r--   0 om        (1001) users      (100)     1800 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/external/oblv/exceptions.py
--rw-r--r--   0 om        (1001) users      (100)      489 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/external/oblv/oblv_keys.py
--rw-r--r--   0 om        (1001) users      (100)     2280 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/external/oblv/oblv_keys_stash.py
--rw-r--r--   0 om        (1001) users      (100)     7462 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/external/oblv/oblv_proxy.py
--rw-r--r--   0 om        (1001) users      (100)    13948 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/external/oblv/oblv_service.py
--rw-r--r--   0 om        (1001) users      (100)     1146 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/gevent_patch.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.497721 syft-0.8.2b6/src/syft/img/
--rw-r--r--   0 om        (1001) users      (100)      297 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/img/base64.py
--rw-r--r--   0 om        (1001) users      (100)    25535 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/img/logo.png
--rw-r--r--   0 om        (1001) users      (100)    41764 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/img/small-grid-symbol-logo.png
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.497721 syft-0.8.2b6/src/syft/node/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/node/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     2631 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/node/credentials.py
--rw-r--r--   0 om        (1001) users      (100)      152 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/node/domain.py
--rw-r--r--   0 om        (1001) users      (100)      259 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/node/enclave.py
--rw-r--r--   0 om        (1001) users      (100)      819 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/node/gateway.py
--rw-r--r--   0 om        (1001) users      (100)    33437 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/node/node.py
--rw-r--r--   0 om        (1001) users      (100)     6960 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/node/routes.py
--rw-r--r--   0 om        (1001) users      (100)     2064 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/node/run.py
--rw-r--r--   0 om        (1001) users      (100)     7737 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/node/server.py
--rw-r--r--   0 om        (1001) users      (100)      127 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/node/worker.py
--rw-r--r--   0 om        (1001) users      (100)     1228 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/node/worker_settings.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.501721 syft-0.8.2b6/src/syft/serde/
--rw-r--r--   0 om        (1001) users      (100)      159 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     3597 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/array.py
--rw-r--r--   0 om        (1001) users      (100)     4099 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/arrow.py
--rw-r--r--   0 om        (1001) users      (100)      298 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/capnp.py
--rw-r--r--   0 om        (1001) users      (100)      722 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/deserialize.py
--rw-r--r--   0 om        (1001) users      (100)     1230 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/lib_permissions.py
--rw-r--r--   0 om        (1001) users      (100)    11663 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/lib_service_registry.py
--rw-r--r--   0 om        (1001) users      (100)      875 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/mock.py
--rw-r--r--   0 om        (1001) users      (100)    11639 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/recursive.py
--rw-r--r--   0 om        (1001) users      (100)    10253 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/recursive_primitives.py
--rw-r--r--   0 om        (1001) users      (100)     1822 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/serializable.py
--rw-r--r--   0 om        (1001) users      (100)      369 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/serialize.py
--rw-r--r--   0 om        (1001) users      (100)     4959 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/signature.py
--rw-r--r--   0 om        (1001) users      (100)     4885 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/third_party.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.501721 syft-0.8.2b6/src/syft/service/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/__init__.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.501721 syft-0.8.2b6/src/syft/service/action/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      703 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/action_data_empty.py
--rw-r--r--   0 om        (1001) users      (100)    16706 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/action_graph.py
--rw-r--r--   0 om        (1001) users      (100)     6874 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/action_graph_service.py
--rw-r--r--   0 om        (1001) users      (100)    48803 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/action_object.py
--rw-r--r--   0 om        (1001) users      (100)     2502 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/action_permissions.py
--rw-r--r--   0 om        (1001) users      (100)    27128 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/action_service.py
--rw-r--r--   0 om        (1001) users      (100)    10264 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/action_store.py
--rw-r--r--   0 om        (1001) users      (100)     1165 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/action_types.py
--rw-r--r--   0 om        (1001) users      (100)     3889 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/numpy.py
--rw-r--r--   0 om        (1001) users      (100)     2233 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/pandas.py
--rw-r--r--   0 om        (1001) users      (100)     2920 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/plan.py
--rw-r--r--   0 om        (1001) users      (100)     4951 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/verification.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.501721 syft-0.8.2b6/src/syft/service/code/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/code/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      236 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/code/code_parse.py
--rw-r--r--   0 om        (1001) users      (100)      102 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/code/unparse.py
--rw-r--r--   0 om        (1001) users      (100)    27413 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/code/user_code.py
--rw-r--r--   0 om        (1001) users      (100)     1756 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/code/user_code_parse.py
--rw-r--r--   0 om        (1001) users      (100)    10340 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/code/user_code_service.py
--rw-r--r--   0 om        (1001) users      (100)     1446 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/code/user_code_stash.py
--rw-r--r--   0 om        (1001) users      (100)     1782 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/context.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.501721 syft-0.8.2b6/src/syft/service/data_subject/
--rw-r--r--   0 om        (1001) users      (100)       69 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/data_subject/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     4076 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/data_subject/data_subject.py
--rw-r--r--   0 om        (1001) users      (100)      870 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/data_subject/data_subject_member.py
--rw-r--r--   0 om        (1001) users      (100)     3215 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/data_subject/data_subject_member_service.py
--rw-r--r--   0 om        (1001) users      (100)     5006 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/data_subject/data_subject_service.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.505721 syft-0.8.2b6/src/syft/service/dataset/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/dataset/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    23590 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/dataset/dataset.py
--rw-r--r--   0 om        (1001) users      (100)     6603 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/dataset/dataset_service.py
--rw-r--r--   0 om        (1001) users      (100)     1911 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/dataset/dataset_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.505721 syft-0.8.2b6/src/syft/service/enclave/
--rw-r--r--   0 om        (1001) users      (100)     6038 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/enclave/enclave_service.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.505721 syft-0.8.2b6/src/syft/service/metadata/
--rw-r--r--   0 om        (1001) users      (100)     1170 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/metadata/metadata_service.py
--rw-r--r--   0 om        (1001) users      (100)     3774 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/metadata/node_metadata.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.505721 syft-0.8.2b6/src/syft/service/network/
--rw-r--r--   0 om        (1001) users      (100)    18260 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/network/network_service.py
--rw-r--r--   0 om        (1001) users      (100)     3100 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/network/node_peer.py
--rw-r--r--   0 om        (1001) users      (100)     4657 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/network/routes.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.505721 syft-0.8.2b6/src/syft/service/notification/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/notification/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     7961 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/notification/notification_service.py
--rw-r--r--   0 om        (1001) users      (100)     4566 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/notification/notification_stash.py
--rw-r--r--   0 om        (1001) users      (100)     3259 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/notification/notifications.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.505721 syft-0.8.2b6/src/syft/service/policy/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/policy/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    22437 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/policy/policy.py
--rw-r--r--   0 om        (1001) users      (100)     2081 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/policy/policy_service.py
--rw-r--r--   0 om        (1001) users      (100)     1077 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/policy/user_policy_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.505721 syft-0.8.2b6/src/syft/service/project/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/project/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    48433 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/project/project.py
--rw-r--r--   0 om        (1001) users      (100)    15374 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/project/project_service.py
--rw-r--r--   0 om        (1001) users      (100)     1908 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/project/project_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.505721 syft-0.8.2b6/src/syft/service/queue/
--rw-r--r--   0 om        (1001) users      (100)     2044 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/queue/base_queue.py
--rw-r--r--   0 om        (1001) users      (100)     3008 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/queue/queue.py
--rw-r--r--   0 om        (1001) users      (100)     4845 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/queue/queue_stash.py
--rw-r--r--   0 om        (1001) users      (100)     7929 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/queue/zmq_queue.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.505721 syft-0.8.2b6/src/syft/service/request/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/request/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    28165 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/request/request.py
--rw-r--r--   0 om        (1001) users      (100)    10135 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/request/request_service.py
--rw-r--r--   0 om        (1001) users      (100)     1410 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/request/request_stash.py
--rw-r--r--   0 om        (1001) users      (100)     3100 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/response.py
--rw-r--r--   0 om        (1001) users      (100)    13815 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/service.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.505721 syft-0.8.2b6/src/syft/service/settings/
--rw-r--r--   0 om        (1001) users      (100)     1109 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/settings/settings.py
--rw-r--r--   0 om        (1001) users      (100)     3608 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/settings/settings_service.py
--rw-r--r--   0 om        (1001) users      (100)     1711 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/settings/settings_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.505721 syft-0.8.2b6/src/syft/service/user/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/user/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      201 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/user/roles.py
--rw-r--r--   0 om        (1001) users      (100)     6115 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/user/user.py
--rw-r--r--   0 om        (1001) users      (100)     3427 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/user/user_roles.py
--rw-r--r--   0 om        (1001) users      (100)    16878 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/user/user_service.py
--rw-r--r--   0 om        (1001) users      (100)     4510 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/user/user_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.505721 syft-0.8.2b6/src/syft/service/vpn/
--rw-r--r--   0 om        (1001) users      (100)     1809 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/vpn/headscale_client.py
--rw-r--r--   0 om        (1001) users      (100)     6789 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/vpn/tailscale_client.py
--rw-r--r--   0 om        (1001) users      (100)     5414 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/vpn/vpn.py
--rw-r--r--   0 om        (1001) users      (100)     5171 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/warnings.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.509721 syft-0.8.2b6/src/syft/store/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/store/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     3235 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/store/dict_document_store.py
--rw-r--r--   0 om        (1001) users      (100)    22993 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/store/document_store.py
--rw-r--r--   0 om        (1001) users      (100)    22010 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/store/kv_document_store.py
--rw-r--r--   0 om        (1001) users      (100)     4326 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/store/linked_obj.py
--rw-r--r--   0 om        (1001) users      (100)    11840 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/store/locks.py
--rw-r--r--   0 om        (1001) users      (100)     8768 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/store/mongo_client.py
--rw-r--r--   0 om        (1001) users      (100)      846 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/store/mongo_codecs.py
--rw-r--r--   0 om        (1001) users      (100)    13836 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/store/mongo_document_store.py
--rw-r--r--   0 om        (1001) users      (100)    13136 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/store/sqlite_document_store.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.509721 syft-0.8.2b6/src/syft/types/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/types/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      136 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/types/base.py
--rw-r--r--   0 om        (1001) users      (100)     1091 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/types/datetime.py
--rw-r--r--   0 om        (1001) users      (100)     5167 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/types/grid_url.py
--rw-r--r--   0 om        (1001) users      (100)     4807 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/types/syft_metaclass.py
--rw-r--r--   0 om        (1001) users      (100)    25848 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/types/syft_object.py
--rw-r--r--   0 om        (1001) users      (100)     8113 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/types/transforms.py
--rw-r--r--   0 om        (1001) users      (100)     2098 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/types/twin_object.py
--rw-r--r--   0 om        (1001) users      (100)     8038 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/types/uid.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.509721 syft-0.8.2b6/src/syft/util/
--rw-r--r--   0 om        (1001) users      (100)       67 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      852 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/autoreload.py
--rw-r--r--   0 om        (1001) users      (100)      271 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/colors.py
--rw-r--r--   0 om        (1001) users      (100)       34 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/constants.py
--rw-r--r--   0 om        (1001) users      (100)     1514 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/decorators.py
--rw-r--r--   0 om        (1001) users      (100)      445 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/env.py
--rw-r--r--   0 om        (1001) users      (100)     1607 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/experimental_flags.py
--rw-r--r--   0 om        (1001) users      (100)     1327 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/filterwarnings.py
--rw-r--r--   0 om        (1001) users      (100)     2940 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/fonts.py
--rw-r--r--   0 om        (1001) users      (100)      153 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/jax_settings.py
--rw-r--r--   0 om        (1001) users      (100)     3779 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/logger.py
--rw-r--r--   0 om        (1001) users      (100)      752 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/markdown.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.509721 syft-0.8.2b6/src/syft/util/notebook_ui/
--rw-r--r--   0 om        (1001) users      (100)    27090 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/notebook_ui/notebook_addons.py
--rw-r--r--   0 om        (1001) users      (100)       42 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/options.py
--rw-r--r--   0 om        (1001) users      (100)     5297 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/schema.py
--rw-r--r--   0 om        (1001) users      (100)     2771 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/telemetry.py
--rw-r--r--   0 om        (1001) users      (100)     6728 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/trace_decorator.py
--rw-r--r--   0 om        (1001) users      (100)    23185 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/util.py
--rw-r--r--   0 om        (1001) users      (100)     3123 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/version_compare.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.497721 syft-0.8.2b6/src/syft.egg-info/
--rw-r--r--   0 om        (1001) users      (100)    16852 2023-07-17 15:39:19.000000 syft-0.8.2b6/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 om        (1001) users      (100)     5975 2023-07-17 15:39:19.000000 syft-0.8.2b6/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 om        (1001) users      (100)        1 2023-07-17 15:39:19.000000 syft-0.8.2b6/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 om        (1001) users      (100)       43 2023-07-17 15:39:19.000000 syft-0.8.2b6/src/syft.egg-info/entry_points.txt
--rw-r--r--   0 om        (1001) users      (100)        1 2023-07-17 15:39:19.000000 syft-0.8.2b6/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 om        (1001) users      (100)     1555 2023-07-17 15:39:19.000000 syft-0.8.2b6/src/syft.egg-info/requires.txt
--rw-r--r--   0 om        (1001) users      (100)        5 2023-07-17 15:39:19.000000 syft-0.8.2b6/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.118659 syft-0.8.2b7/
+-rw-r--r--   0 om        (1001) users      (100)    11843 2023-08-05 12:21:46.000000 syft-0.8.2b7/LICENSE
+-rw-r--r--   0 om        (1001) users      (100)       98 2023-08-05 12:21:46.000000 syft-0.8.2b7/MANIFEST.in
+-rw-r--r--   0 om        (1001) users      (100)    16852 2023-08-05 12:23:10.118659 syft-0.8.2b7/PKG-INFO
+-rw-r--r--   0 om        (1001) users      (100)    16170 2023-08-05 12:21:46.000000 syft-0.8.2b7/README.md
+-rw-r--r--   0 om        (1001) users      (100)      272 2023-08-05 12:21:46.000000 syft-0.8.2b7/pyproject.toml
+-rw-r--r--   0 om        (1001) users      (100)     3210 2023-08-05 12:23:10.118659 syft-0.8.2b7/setup.cfg
+-rw-r--r--   0 om        (1001) users      (100)      107 2023-08-05 12:21:46.000000 syft-0.8.2b7/setup.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.098659 syft-0.8.2b7/src/
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.102659 syft-0.8.2b7/src/syft/
+-rw-r--r--   0 om        (1001) users      (100)      580 2023-08-05 12:21:49.000000 syft-0.8.2b7/src/syft/VERSION
+-rw-r--r--   0 om        (1001) users      (100)     5750 2023-08-05 12:21:49.000000 syft-0.8.2b7/src/syft/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)       93 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/__main__.py
+-rw-r--r--   0 om        (1001) users      (100)      790 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/abstract_node.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.102659 syft-0.8.2b7/src/syft/capnp/
+-rw-r--r--   0 om        (1001) users      (100)      270 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/capnp/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)       75 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 om        (1001) users      (100)      102 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 om        (1001) users      (100)      186 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.102659 syft-0.8.2b7/src/syft/client/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/client/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    27127 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/client/api.py
+-rw-r--r--   0 om        (1001) users      (100)    28998 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/client/client.py
+-rw-r--r--   0 om        (1001) users      (100)      568 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/client/connection.py
+-rw-r--r--   0 om        (1001) users      (100)      650 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/client/deploy.py
+-rw-r--r--   0 om        (1001) users      (100)     9925 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/client/domain_client.py
+-rw-r--r--   0 om        (1001) users      (100)     7000 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/client/enclave_client.py
+-rw-r--r--   0 om        (1001) users      (100)     6404 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/client/gateway_client.py
+-rw-r--r--   0 om        (1001) users      (100)    15257 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/client/registry.py
+-rw-r--r--   0 om        (1001) users      (100)     2623 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/client/search.py
+-rw-r--r--   0 om        (1001) users      (100)      549 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/client/user_settings.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.102659 syft-0.8.2b7/src/syft/external/
+-rw-r--r--   0 om        (1001) users      (100)     1735 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/external/__init__.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.106659 syft-0.8.2b7/src/syft/external/oblv/
+-rw-r--r--   0 om        (1001) users      (100)      860 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/external/oblv/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      284 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/external/oblv/auth.py
+-rw-r--r--   0 om        (1001) users      (100)      212 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/external/oblv/constants.py
+-rw-r--r--   0 om        (1001) users      (100)     4835 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/external/oblv/deployment.py
+-rw-r--r--   0 om        (1001) users      (100)    12380 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/external/oblv/deployment_client.py
+-rw-r--r--   0 om        (1001) users      (100)     1800 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/external/oblv/exceptions.py
+-rw-r--r--   0 om        (1001) users      (100)      489 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/external/oblv/oblv_keys.py
+-rw-r--r--   0 om        (1001) users      (100)     2280 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/external/oblv/oblv_keys_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     7462 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/external/oblv/oblv_proxy.py
+-rw-r--r--   0 om        (1001) users      (100)    13949 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/external/oblv/oblv_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1146 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/gevent_patch.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.106659 syft-0.8.2b7/src/syft/img/
+-rw-r--r--   0 om        (1001) users      (100)      297 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/img/base64.py
+-rw-r--r--   0 om        (1001) users      (100)    25535 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/img/logo.png
+-rw-r--r--   0 om        (1001) users      (100)    41764 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/img/small-grid-symbol-logo.png
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.106659 syft-0.8.2b7/src/syft/node/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/node/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     2631 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/node/credentials.py
+-rw-r--r--   0 om        (1001) users      (100)      152 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/node/domain.py
+-rw-r--r--   0 om        (1001) users      (100)      259 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/node/enclave.py
+-rw-r--r--   0 om        (1001) users      (100)      819 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/node/gateway.py
+-rw-r--r--   0 om        (1001) users      (100)    34306 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/node/node.py
+-rw-r--r--   0 om        (1001) users      (100)     6960 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/node/routes.py
+-rw-r--r--   0 om        (1001) users      (100)     2064 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/node/run.py
+-rw-r--r--   0 om        (1001) users      (100)     7737 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/node/server.py
+-rw-r--r--   0 om        (1001) users      (100)      127 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/node/worker.py
+-rw-r--r--   0 om        (1001) users      (100)     1228 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/node/worker_settings.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.106659 syft-0.8.2b7/src/syft/serde/
+-rw-r--r--   0 om        (1001) users      (100)      159 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     3597 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/array.py
+-rw-r--r--   0 om        (1001) users      (100)     4099 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/arrow.py
+-rw-r--r--   0 om        (1001) users      (100)      298 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/capnp.py
+-rw-r--r--   0 om        (1001) users      (100)      722 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/deserialize.py
+-rw-r--r--   0 om        (1001) users      (100)     1230 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/lib_permissions.py
+-rw-r--r--   0 om        (1001) users      (100)    11663 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/lib_service_registry.py
+-rw-r--r--   0 om        (1001) users      (100)      875 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/mock.py
+-rw-r--r--   0 om        (1001) users      (100)    11639 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/recursive.py
+-rw-r--r--   0 om        (1001) users      (100)    11054 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/recursive_primitives.py
+-rw-r--r--   0 om        (1001) users      (100)     1822 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/serializable.py
+-rw-r--r--   0 om        (1001) users      (100)      369 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/serialize.py
+-rw-r--r--   0 om        (1001) users      (100)     4959 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/signature.py
+-rw-r--r--   0 om        (1001) users      (100)     4885 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/third_party.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.106659 syft-0.8.2b7/src/syft/service/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/__init__.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.110659 syft-0.8.2b7/src/syft/service/action/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      703 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/action_data_empty.py
+-rw-r--r--   0 om        (1001) users      (100)    16706 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/action_graph.py
+-rw-r--r--   0 om        (1001) users      (100)     6874 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/action_graph_service.py
+-rw-r--r--   0 om        (1001) users      (100)    49572 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/action_object.py
+-rw-r--r--   0 om        (1001) users      (100)     2502 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/action_permissions.py
+-rw-r--r--   0 om        (1001) users      (100)    27533 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/action_service.py
+-rw-r--r--   0 om        (1001) users      (100)    10264 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/action_store.py
+-rw-r--r--   0 om        (1001) users      (100)     1165 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/action_types.py
+-rw-r--r--   0 om        (1001) users      (100)     3889 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/numpy.py
+-rw-r--r--   0 om        (1001) users      (100)     2233 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/pandas.py
+-rw-r--r--   0 om        (1001) users      (100)     2920 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/plan.py
+-rw-r--r--   0 om        (1001) users      (100)     4951 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/verification.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.110659 syft-0.8.2b7/src/syft/service/blob_storage/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/blob_storage/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     3437 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/blob_storage/service.py
+-rw-r--r--   0 om        (1001) users      (100)      594 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/blob_storage/stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.110659 syft-0.8.2b7/src/syft/service/code/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/code/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      236 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/code/code_parse.py
+-rw-r--r--   0 om        (1001) users      (100)      102 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/code/unparse.py
+-rw-r--r--   0 om        (1001) users      (100)    30430 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/code/user_code.py
+-rw-r--r--   0 om        (1001) users      (100)     1756 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/code/user_code_parse.py
+-rw-r--r--   0 om        (1001) users      (100)    12538 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/code/user_code_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1446 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/code/user_code_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.110659 syft-0.8.2b7/src/syft/service/code_history/
+-rw-r--r--   0 om        (1001) users      (100)     4297 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/code_history/code_history.py
+-rw-r--r--   0 om        (1001) users      (100)     8729 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/code_history/code_history_service.py
+-rw-r--r--   0 om        (1001) users      (100)     2348 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/code_history/code_history_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     1782 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/context.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.110659 syft-0.8.2b7/src/syft/service/data_subject/
+-rw-r--r--   0 om        (1001) users      (100)       69 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/data_subject/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     4076 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/data_subject/data_subject.py
+-rw-r--r--   0 om        (1001) users      (100)      870 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/data_subject/data_subject_member.py
+-rw-r--r--   0 om        (1001) users      (100)     3215 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/data_subject/data_subject_member_service.py
+-rw-r--r--   0 om        (1001) users      (100)     5006 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/data_subject/data_subject_service.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.110659 syft-0.8.2b7/src/syft/service/dataset/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/dataset/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    23590 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/dataset/dataset.py
+-rw-r--r--   0 om        (1001) users      (100)     6603 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/dataset/dataset_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1911 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/dataset/dataset_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.110659 syft-0.8.2b7/src/syft/service/enclave/
+-rw-r--r--   0 om        (1001) users      (100)     6039 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/enclave/enclave_service.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.110659 syft-0.8.2b7/src/syft/service/metadata/
+-rw-r--r--   0 om        (1001) users      (100)     1170 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/metadata/metadata_service.py
+-rw-r--r--   0 om        (1001) users      (100)     3774 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/metadata/node_metadata.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.110659 syft-0.8.2b7/src/syft/service/network/
+-rw-r--r--   0 om        (1001) users      (100)    18260 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/network/network_service.py
+-rw-r--r--   0 om        (1001) users      (100)     3100 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/network/node_peer.py
+-rw-r--r--   0 om        (1001) users      (100)     4657 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/network/routes.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.110659 syft-0.8.2b7/src/syft/service/notification/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/notification/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     7961 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/notification/notification_service.py
+-rw-r--r--   0 om        (1001) users      (100)     4566 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/notification/notification_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     3259 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/notification/notifications.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.110659 syft-0.8.2b7/src/syft/service/policy/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/policy/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    22636 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/policy/policy.py
+-rw-r--r--   0 om        (1001) users      (100)     2081 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/policy/policy_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1077 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/policy/user_policy_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.110659 syft-0.8.2b7/src/syft/service/project/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/project/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    47645 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/project/project.py
+-rw-r--r--   0 om        (1001) users      (100)    15374 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/project/project_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1908 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/project/project_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.114659 syft-0.8.2b7/src/syft/service/queue/
+-rw-r--r--   0 om        (1001) users      (100)     2038 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/queue/base_queue.py
+-rw-r--r--   0 om        (1001) users      (100)     3006 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/queue/queue.py
+-rw-r--r--   0 om        (1001) users      (100)     4845 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/queue/queue_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     7754 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/queue/zmq_queue.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.114659 syft-0.8.2b7/src/syft/service/request/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/request/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    29652 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/request/request.py
+-rw-r--r--   0 om        (1001) users      (100)    10135 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/request/request_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1410 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/request/request_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     3125 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/response.py
+-rw-r--r--   0 om        (1001) users      (100)    13815 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/service.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.114659 syft-0.8.2b7/src/syft/service/settings/
+-rw-r--r--   0 om        (1001) users      (100)     1109 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/settings/settings.py
+-rw-r--r--   0 om        (1001) users      (100)     3608 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/settings/settings_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1711 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/settings/settings_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.114659 syft-0.8.2b7/src/syft/service/user/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/user/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      201 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/user/roles.py
+-rw-r--r--   0 om        (1001) users      (100)     9666 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/user/user.py
+-rw-r--r--   0 om        (1001) users      (100)     3427 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/user/user_roles.py
+-rw-r--r--   0 om        (1001) users      (100)    17595 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/user/user_service.py
+-rw-r--r--   0 om        (1001) users      (100)     4510 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/user/user_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.114659 syft-0.8.2b7/src/syft/service/vpn/
+-rw-r--r--   0 om        (1001) users      (100)     1830 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/vpn/headscale_client.py
+-rw-r--r--   0 om        (1001) users      (100)     6789 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/vpn/tailscale_client.py
+-rw-r--r--   0 om        (1001) users      (100)     5414 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/vpn/vpn.py
+-rw-r--r--   0 om        (1001) users      (100)     5171 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/warnings.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.114659 syft-0.8.2b7/src/syft/store/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/__init__.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.114659 syft-0.8.2b7/src/syft/store/blob_storage/
+-rw-r--r--   0 om        (1001) users      (100)     3961 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/blob_storage/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     2790 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/blob_storage/on_disk.py
+-rw-r--r--   0 om        (1001) users      (100)     1036 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/blob_storage/seaweedfs.py
+-rw-r--r--   0 om        (1001) users      (100)     3235 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/dict_document_store.py
+-rw-r--r--   0 om        (1001) users      (100)    23280 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/document_store.py
+-rw-r--r--   0 om        (1001) users      (100)    22188 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/kv_document_store.py
+-rw-r--r--   0 om        (1001) users      (100)     4326 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/linked_obj.py
+-rw-r--r--   0 om        (1001) users      (100)    11840 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/locks.py
+-rw-r--r--   0 om        (1001) users      (100)     8768 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/mongo_client.py
+-rw-r--r--   0 om        (1001) users      (100)      846 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/mongo_codecs.py
+-rw-r--r--   0 om        (1001) users      (100)    14031 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/mongo_document_store.py
+-rw-r--r--   0 om        (1001) users      (100)    13136 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/sqlite_document_store.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.114659 syft-0.8.2b7/src/syft/types/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/types/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      136 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/types/base.py
+-rw-r--r--   0 om        (1001) users      (100)     2151 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/types/blob_storage.py
+-rw-r--r--   0 om        (1001) users      (100)     1091 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/types/datetime.py
+-rw-r--r--   0 om        (1001) users      (100)     5167 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/types/grid_url.py
+-rw-r--r--   0 om        (1001) users      (100)      919 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/types/identity.py
+-rw-r--r--   0 om        (1001) users      (100)     4807 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/types/syft_metaclass.py
+-rw-r--r--   0 om        (1001) users      (100)    25449 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/types/syft_object.py
+-rw-r--r--   0 om        (1001) users      (100)     8113 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/types/transforms.py
+-rw-r--r--   0 om        (1001) users      (100)     2098 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/types/twin_object.py
+-rw-r--r--   0 om        (1001) users      (100)     8038 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/types/uid.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.118659 syft-0.8.2b7/src/syft/util/
+-rw-r--r--   0 om        (1001) users      (100)       67 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      852 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/autoreload.py
+-rw-r--r--   0 om        (1001) users      (100)      271 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/colors.py
+-rw-r--r--   0 om        (1001) users      (100)       34 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/constants.py
+-rw-r--r--   0 om        (1001) users      (100)     1514 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/decorators.py
+-rw-r--r--   0 om        (1001) users      (100)      445 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/env.py
+-rw-r--r--   0 om        (1001) users      (100)     1607 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/experimental_flags.py
+-rw-r--r--   0 om        (1001) users      (100)     1327 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/filterwarnings.py
+-rw-r--r--   0 om        (1001) users      (100)     2940 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/fonts.py
+-rw-r--r--   0 om        (1001) users      (100)      153 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/jax_settings.py
+-rw-r--r--   0 om        (1001) users      (100)     3779 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/logger.py
+-rw-r--r--   0 om        (1001) users      (100)      752 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/markdown.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.118659 syft-0.8.2b7/src/syft/util/notebook_ui/
+-rw-r--r--   0 om        (1001) users      (100)    27090 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/notebook_ui/notebook_addons.py
+-rw-r--r--   0 om        (1001) users      (100)       42 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/options.py
+-rw-r--r--   0 om        (1001) users      (100)     5297 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/schema.py
+-rw-r--r--   0 om        (1001) users      (100)     2771 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/telemetry.py
+-rw-r--r--   0 om        (1001) users      (100)     6728 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/trace_decorator.py
+-rw-r--r--   0 om        (1001) users      (100)    23185 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/util.py
+-rw-r--r--   0 om        (1001) users      (100)     3123 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/version_compare.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.102659 syft-0.8.2b7/src/syft.egg-info/
+-rw-r--r--   0 om        (1001) users      (100)    16852 2023-08-05 12:23:10.000000 syft-0.8.2b7/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 om        (1001) users      (100)     6427 2023-08-05 12:23:10.000000 syft-0.8.2b7/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 om        (1001) users      (100)        1 2023-08-05 12:23:10.000000 syft-0.8.2b7/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 om        (1001) users      (100)       43 2023-08-05 12:23:10.000000 syft-0.8.2b7/src/syft.egg-info/entry_points.txt
+-rw-r--r--   0 om        (1001) users      (100)        1 2023-08-05 12:23:09.000000 syft-0.8.2b7/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 om        (1001) users      (100)     1555 2023-08-05 12:23:10.000000 syft-0.8.2b7/src/syft.egg-info/requires.txt
+-rw-r--r--   0 om        (1001) users      (100)        5 2023-08-05 12:23:10.000000 syft-0.8.2b7/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.2b6/LICENSE` & `syft-0.8.2b7/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/PKG-INFO` & `syft-0.8.2b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.2b6
+Version: 0.8.2b7
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.2b6 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.2b7 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: telemetry
```

### Comparing `syft-0.8.2b6/README.md` & `syft-0.8.2b7/README.md`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/setup.cfg` & `syft-0.8.2b7/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.2-beta.6"
+version = attr: "0.8.2-beta.7"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
```

### Comparing `syft-0.8.2b6/src/syft/VERSION` & `syft-0.8.2b7/src/syft/VERSION`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.2-beta.6"
+__version__ = "0.8.2-beta.7"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.2b6/src/syft/__init__.py` & `syft-0.8.2b7/src/syft/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.2-beta.6"
+__version__ = "0.8.2-beta.7"
 
 # stdlib
 import pathlib
 from pathlib import Path
 import sys
 from typing import Any
 from typing import Callable
```

### Comparing `syft-0.8.2b6/src/syft/abstract_node.py` & `syft-0.8.2b7/src/syft/abstract_node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/client/api.py` & `syft-0.8.2b7/src/syft/client/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from typing import Optional
 from typing import Tuple
 from typing import Union
 from typing import _GenericAlias
 
 # third party
 from nacl.exceptions import BadSignatureError
-from pydantic import BaseModel
 from pydantic import EmailStr
 from result import OkErr
 from result import Result
 from typeguard import check_type
 
 # relative
 from ..abstract_node import AbstractNode
@@ -37,16 +36,18 @@
 from ..service.context import AuthedServiceContext
 from ..service.context import ChangeContext
 from ..service.response import SyftAttributeError
 from ..service.response import SyftError
 from ..service.response import SyftSuccess
 from ..service.service import UserLibConfigRegistry
 from ..service.service import UserServiceConfigRegistry
+from ..service.user.user_roles import ServiceRole
 from ..service.warnings import APIEndpointWarning
 from ..service.warnings import WarningContext
+from ..types.identity import Identity
 from ..types.syft_object import SYFT_OBJECT_VERSION_1
 from ..types.syft_object import SyftBaseObject
 from ..types.syft_object import SyftObject
 from ..types.uid import LineageID
 from ..types.uid import UID
 from ..util.autoreload import autoreload_enabled
 from ..util.telemetry import instrument
@@ -389,14 +390,15 @@
     endpoints: Dict[str, APIEndpoint]
     lib_endpoints: Optional[Dict[str, LibEndpoint]] = None
     api_module: Optional[APIModule] = None
     libs: Optional[APIModule] = None
     signing_key: Optional[SyftSigningKey] = None
     # serde / storage rules
     refresh_api_callback: Optional[Callable] = None
+    __user_role: ServiceRole = ServiceRole.NONE
 
     # def __post_init__(self) -> None:
     #     pass
 
     @staticmethod
     def for_user(
         node: AbstractNode, user_verify_key: Optional[SyftVerifyKey] = None
@@ -473,16 +475,21 @@
             endpoints[unique_path] = endpoint
 
         return SyftAPI(
             node_name=node.name,
             node_uid=node.id,
             endpoints=endpoints,
             lib_endpoints=lib_endpoints,
+            __user_role=role,
         )
 
+    @property
+    def user_role(self) -> ServiceRole:
+        return self.__user_role
+
     def make_call(self, api_call: SyftAPICall) -> Result:
         signed_call = api_call.sign(credentials=self.signing_key)
         signed_result = self.connection.make_call(signed_call)
 
         result = debox_signed_syftapicall_response(signed_result=signed_result)
 
         if isinstance(result, OkErr):
@@ -667,52 +674,50 @@
         Inspector._getdef = types.MethodType(monkey_patch_getdef, Inspector)
 except Exception:
     # print("Failed to monkeypatch IPython Signature Override")
     pass  # nosec
 
 
 @serializable()
-class NodeView(BaseModel):
-    class Config:
-        arbitrary_types_allowed = True
-
+class NodeIdentity(Identity):
     node_name: str
-    node_id: UID
-    verify_key: SyftVerifyKey
 
     @staticmethod
     def from_api(api: SyftAPI):
         # stores the name root verify key of the domain node
         node_metadata = api.connection.get_node_metadata(api.signing_key)
-        return NodeView(
+        return NodeIdentity(
             node_name=node_metadata.name,
             node_id=api.node_uid,
             verify_key=SyftVerifyKey.from_string(node_metadata.verify_key),
         )
 
     @classmethod
     def from_change_context(cls, context: ChangeContext):
         return cls(
             node_name=context.node.name,
             node_id=context.node.id,
             verify_key=context.node.signing_key.verify_key,
         )
 
     def __eq__(self, other: Any) -> bool:
-        if not isinstance(other, NodeView):
+        if not isinstance(other, NodeIdentity):
             return False
         return (
             self.node_name == other.node_name
             and self.verify_key == other.verify_key
             and self.node_id == other.node_id
         )
 
     def __hash__(self) -> int:
         return hash((self.node_name, self.verify_key))
 
+    def __repr__(self) -> str:
+        return f"NodeIdentity <name={self.node_name}, id={self.node_id.short()}, 🔑={str(self.verify_key)[0:8]}>"
+
 
 def validate_callable_args_and_kwargs(args, kwargs, signature: Signature):
     _valid_kwargs = {}
     if "kwargs" in signature.parameters:
         _valid_kwargs = kwargs
     else:
         for key, value in kwargs.items():
@@ -727,19 +732,26 @@
                 t = index_syft_by_module_name(param.annotation)
             else:
                 t = param.annotation
             msg = None
             try:
                 if t is not inspect.Parameter.empty:
                     if isinstance(t, _GenericAlias) and type(None) in t.__args__:
+                        success = False
                         for v in t.__args__:
                             if issubclass(v, EmailStr):
                                 v = str
-                            check_type(key, value, v)  # raises Exception
-                            break  # only need one to match
+                            try:
+                                check_type(key, value, v)  # raises Exception
+                                success = True
+                                break  # only need one to match
+                            except Exception:  # nosec
+                                pass
+                        if not success:
+                            raise TypeError()
                     else:
                         check_type(key, value, t)  # raises Exception
             except TypeError:
                 _type_str = getattr(t, "__name__", str(t))
                 msg = f"`{key}` must be of type `{_type_str}` not `{type(value).__name__}`"
 
             if msg:
```

### Comparing `syft-0.8.2b6/src/syft/client/client.py` & `syft-0.8.2b7/src/syft/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 from ..service.context import NodeServiceContext
 from ..service.metadata.node_metadata import NodeMetadata
 from ..service.metadata.node_metadata import NodeMetadataJSON
 from ..service.response import SyftError
 from ..service.response import SyftSuccess
 from ..service.user.user import UserCreate
 from ..service.user.user import UserPrivateKey
+from ..service.user.user import UserView
 from ..service.user.user_roles import ServiceRole
 from ..service.user.user_service import UserService
 from ..types.grid_url import GridURL
 from ..types.syft_object import SYFT_OBJECT_VERSION_1
 from ..types.uid import UID
 from ..util.logger import debug
 from ..util.telemetry import instrument
@@ -565,14 +566,20 @@
 
     @property
     def peers(self) -> Optional[Union[List[NodePeer], SyftError]]:
         if self.api.has_service("network"):
             return self.api.services.network.get_all_peers()
         return None
 
+    @property
+    def me(self) -> Optional[Union[UserView, SyftError]]:
+        if self.api.has_service("user"):
+            return self.api.services.user.get_current_user()
+        return None
+
     def login(
         self, email: str, password: str, cache: bool = True, register=False, **kwargs
     ) -> Self:
         if register:
             self.register(email=email, password=password, **kwargs)
         user_private_key = self.connection.login(email=email, password=password)
         if isinstance(user_private_key, SyftError):
```

### Comparing `syft-0.8.2b6/src/syft/client/connection.py` & `syft-0.8.2b7/src/syft/client/connection.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/client/deploy.py` & `syft-0.8.2b7/src/syft/client/deploy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/client/domain_client.py` & `syft-0.8.2b7/src/syft/client/domain_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 # third party
 from tqdm import tqdm
 
 # relative
 from ..abstract_node import NodeSideType
 from ..img.base64 import base64read
 from ..serde.serializable import serializable
+from ..service.code_history.code_history import CodeHistoriesDict
+from ..service.code_history.code_history import UsersCodeHistoriesDict
 from ..service.dataset.dataset import Contributor
 from ..service.dataset.dataset import CreateAsset
 from ..service.dataset.dataset import CreateDataset
 from ..service.response import SyftError
 from ..service.response import SyftSuccess
 from ..service.user.roles import Roles
 from ..service.user.user_roles import ServiceRole
@@ -120,14 +122,16 @@
     def data_subject_registry(self) -> Optional[APIModule]:
         if self.api.has_service("data_subject"):
             return self.api.services.data_subject
         return None
 
     @property
     def code(self) -> Optional[APIModule]:
+        # if self.api.refresh_api_callback is not None:
+        #     self.api.refresh_api_callback()
         if self.api.has_service("code"):
             return self.api.services.code
         return None
 
     @property
     def requests(self) -> Optional[APIModule]:
         if self.api.has_service("request"):
@@ -142,14 +146,28 @@
 
     @property
     def projects(self) -> Optional[APIModule]:
         if self.api.has_service("project"):
             return self.api.services.project
         return None
 
+    @property
+    def code_history_service(self) -> Optional[APIModule]:
+        if self.api is not None and self.api.has_service("code_history"):
+            return self.api.services.code_history
+        return None
+
+    @property
+    def code_history(self) -> CodeHistoriesDict:
+        return self.api.services.code_history.get_history()
+
+    @property
+    def code_histories(self) -> UsersCodeHistoriesDict:
+        return self.api.services.code_history.get_histories()
+
     def get_project(
         self,
         name: str = None,
         uid: UID = None,
     ) -> Optional[Project]:
         """Get project by name or UID"""
```

### Comparing `syft-0.8.2b6/src/syft/client/enclave_client.py` & `syft-0.8.2b7/src/syft/client/enclave_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,17 @@
             api = APIRegistry.get_by_recent_node_uid(k.node_id)
             if api is None:
                 raise ValueError(f"could not find client for input {v}")
             else:
                 apis += [api]
 
         for api in apis:
-            api.services.code.request_code_execution(code=code)
+            res = api.services.code.request_code_execution(code=code)
+            if isinstance(res, SyftError):
+                return res
 
         # we are using the real method here, see the .code property getter
         _ = self.code
         res = self._request_code_execution(code=code)
 
         return res
```

### Comparing `syft-0.8.2b6/src/syft/client/gateway_client.py` & `syft-0.8.2b7/src/syft/client/gateway_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/client/registry.py` & `syft-0.8.2b7/src/syft/client/registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/client/search.py` & `syft-0.8.2b7/src/syft/client/search.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/client/user_settings.py` & `syft-0.8.2b7/src/syft/client/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/external/__init__.py` & `syft-0.8.2b7/src/syft/external/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/external/oblv/__init__.py` & `syft-0.8.2b7/src/syft/external/oblv/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/external/oblv/deployment.py` & `syft-0.8.2b7/src/syft/external/oblv/deployment.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/external/oblv/deployment_client.py` & `syft-0.8.2b7/src/syft/external/oblv/deployment_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/external/oblv/exceptions.py` & `syft-0.8.2b7/src/syft/external/oblv/exceptions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/external/oblv/oblv_keys_stash.py` & `syft-0.8.2b7/src/syft/external/oblv/oblv_keys_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/external/oblv/oblv_proxy.py` & `syft-0.8.2b7/src/syft/external/oblv/oblv_proxy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/external/oblv/oblv_service.py` & `syft-0.8.2b7/src/syft/external/oblv/oblv_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,15 +374,15 @@
         if user_code.is_err():
             return SyftError(
                 message=f"Unable to find {user_code_id} in {type(user_code_service)}"
             )
         user_code = user_code.ok()
 
         res = user_code.status.mutate(
-            value=UserCodeStatus.EXECUTE,
+            value=UserCodeStatus.APPROVED,
             node_name=node_name,
             verify_key=context.credentials,
         )
         if res.is_err():
             return res
         user_code.status = res.ok()
         user_code_service.update_code_state(context=context, code_item=user_code)
```

### Comparing `syft-0.8.2b6/src/syft/gevent_patch.py` & `syft-0.8.2b7/src/syft/gevent_patch.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/img/logo.png` & `syft-0.8.2b7/src/syft/img/logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/img/small-grid-symbol-logo.png` & `syft-0.8.2b7/src/syft/img/small-grid-symbol-logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/node/credentials.py` & `syft-0.8.2b7/src/syft/node/credentials.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/node/gateway.py` & `syft-0.8.2b7/src/syft/node/gateway.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/node/node.py` & `syft-0.8.2b7/src/syft/node/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,17 @@
 from ..client.api import debox_signed_syftapicall_response
 from ..external import OBLV
 from ..serde.deserialize import _deserialize
 from ..serde.serialize import _serialize
 from ..service.action.action_service import ActionService
 from ..service.action.action_store import DictActionStore
 from ..service.action.action_store import SQLiteActionStore
+from ..service.blob_storage.service import BlobStorageService
 from ..service.code.user_code_service import UserCodeService
+from ..service.code_history.code_history_service import CodeHistoryService
 from ..service.context import AuthedServiceContext
 from ..service.context import NodeServiceContext
 from ..service.context import UnauthedServiceContext
 from ..service.context import UserLoginCredentials
 from ..service.data_subject.data_subject_member_service import DataSubjectMemberService
 from ..service.data_subject.data_subject_service import DataSubjectService
 from ..service.dataset.dataset_service import DatasetService
@@ -75,14 +77,16 @@
 from ..service.settings.settings_service import SettingsService
 from ..service.settings.settings_stash import SettingsStash
 from ..service.user.user import User
 from ..service.user.user import UserCreate
 from ..service.user.user_roles import ServiceRole
 from ..service.user.user_service import UserService
 from ..service.user.user_stash import UserStash
+from ..store.blob_storage import BlobStorageConfig
+from ..store.blob_storage.on_disk import OnDiskBlobStorageConfig
 from ..store.dict_document_store import DictStoreConfig
 from ..store.document_store import StoreConfig
 from ..store.sqlite_document_store import SQLiteStoreClientConfig
 from ..store.sqlite_document_store import SQLiteStoreConfig
 from ..types.syft_object import HIGHEST_SYFT_OBJECT_VERSION
 from ..types.syft_object import LOWEST_SYFT_OBJECT_VERSION
 from ..types.syft_object import SyftObject
@@ -193,15 +197,16 @@
         root_email: str = default_root_email,
         root_password: str = default_root_password,
         processes: int = 0,
         is_subprocess: bool = False,
         node_type: Union[str, NodeType] = NodeType.DOMAIN,
         local_db: bool = False,
         sqlite_path: Optional[str] = None,
-        queue_config: QueueConfig = ZMQQueueConfig,
+        blob_storage_config: Optional[BlobStorageConfig] = None,
+        queue_config: Optional[QueueConfig] = None,
         node_side_type: Union[str, NodeSideType] = NodeSideType.HIGH_SIDE,
         enable_warnings: bool = False,
     ):
         # 🟡 TODO 22: change our ENV variable format and default init args to make this
         # less horrible or add some convenience functions
         if node_uid_env is not None:
             self.id = UID.from_string(node_uid_env)
@@ -236,15 +241,17 @@
                 DataSubjectService,
                 NetworkService,
                 PolicyService,
                 NotificationService,
                 DataSubjectMemberService,
                 ProjectService,
                 EnclaveService,
+                CodeHistoryService,
                 MetadataService,
+                BlobStorageService,
             ]
             if services is None
             else services
         )
 
         self.service_config = ServiceConfigRegistry.get_registered_configs()
         self.local_db = local_db
@@ -283,20 +290,28 @@
         self.node_side_type = node_side_type
 
         self.post_init()
         self.create_initial_settings(admin_email=root_email)
         if not (self.is_subprocess or self.processes == 0):
             self.init_queue_manager(queue_config=queue_config)
 
+        self.init_blob_storage(config=blob_storage_config)
+
         NodeRegistry.set_node_for(self.id, self)
 
-    def init_queue_manager(self, queue_config: QueueConfig):
+    def init_blob_storage(self, config: Optional[BlobStorageConfig] = None) -> None:
+        config_ = OnDiskBlobStorageConfig() if config is None else config
+        self.blob_storage_client = config_.client_type(config=config_.client_config)
+
+    def init_queue_manager(self, queue_config: Optional[QueueConfig]):
+        queue_config_ = ZMQQueueConfig() if queue_config is None else queue_config
+
         MessageHandlers = [APICallMessageHandler]
 
-        self.queue_manager = QueueManager(queue_config)
+        self.queue_manager = QueueManager(config=queue_config_)
         for message_handler in MessageHandlers:
             queue_name = message_handler.queue_name
             producer = self.queue_manager.create_producer(
                 queue_name=queue_name,
             )
             consumer = self.queue_manager.create_consumer(
                 message_handler, producer.address
@@ -495,15 +510,17 @@
                 DataSubjectService,
                 NetworkService,
                 PolicyService,
                 NotificationService,
                 DataSubjectMemberService,
                 ProjectService,
                 EnclaveService,
+                CodeHistoryService,
                 MetadataService,
+                BlobStorageService,
             ]
 
             if OBLV:
                 # relative
                 from ..external.oblv.oblv_service import OblvService
 
                 store_services += [OblvService]
```

### Comparing `syft-0.8.2b6/src/syft/node/routes.py` & `syft-0.8.2b7/src/syft/node/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/node/run.py` & `syft-0.8.2b7/src/syft/node/run.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/node/server.py` & `syft-0.8.2b7/src/syft/node/server.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/node/worker_settings.py` & `syft-0.8.2b7/src/syft/node/worker_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/serde/array.py` & `syft-0.8.2b7/src/syft/serde/array.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/serde/arrow.py` & `syft-0.8.2b7/src/syft/serde/arrow.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/serde/deserialize.py` & `syft-0.8.2b7/src/syft/serde/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/serde/lib_permissions.py` & `syft-0.8.2b7/src/syft/serde/lib_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/serde/lib_service_registry.py` & `syft-0.8.2b7/src/syft/serde/lib_service_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/serde/mock.py` & `syft-0.8.2b7/src/syft/serde/mock.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/serde/recursive.py` & `syft-0.8.2b7/src/syft/serde/recursive.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/serde/recursive_primitives.py` & `syft-0.8.2b7/src/syft/serde/recursive_primitives.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # stdlib
 from collections import OrderedDict
 from collections import defaultdict
 from enum import Enum
 from enum import EnumMeta
 import functools
+import pathlib
+from pathlib import PurePath
 import sys
 from types import MappingProxyType
 from typing import Any
 from typing import Collection
 from typing import Dict
 from typing import List
 from typing import Mapping
 from typing import Optional
+from typing import Type
 from typing import TypeVar
 from typing import Union
 from typing import _GenericAlias
 from typing import _SpecialForm
 from typing import cast
 import weakref
 
@@ -162,14 +165,32 @@
     module_parts = deserialized_type.split(".")
     klass = module_parts.pop()
     klass = "None" if klass == "NoneType" else klass
     exception_type = getattr(sys.modules[".".join(module_parts)], klass)
     return exception_type
 
 
+TPath = TypeVar("TPath", bound=PurePath)
+
+
+def serialize_path(path: PurePath) -> bytes:
+    # relative
+    from .serialize import _serialize
+
+    return cast(bytes, _serialize(str(path), to_bytes=True))
+
+
+def deserialize_path(path_type: Type[TPath], buf: bytes) -> TPath:
+    # relative
+    from .deserialize import _deserialize
+
+    path: str = _deserialize(buf, from_bytes=True)
+    return path_type(path)
+
+
 # bit_length + 1 for signed
 recursive_serde_register(
     int,
     serialize=lambda x: x.to_bytes((x.bit_length() + 7) // 8 + 1, "big", signed=True),
     deserialize=lambda x_bytes: int.from_bytes(x_bytes, "big", signed=True),
 )
 
@@ -270,14 +291,29 @@
 recursive_serde_register(
     MappingProxyType,
     serialize=serialize_kv,
     deserialize=functools.partial(deserialize_kv, MappingProxyType),
 )
 
 
+for __path_type in (
+    PurePath,
+    pathlib.PurePosixPath,
+    pathlib.PureWindowsPath,
+    pathlib.Path,
+    pathlib.PosixPath,
+    pathlib.WindowsPath,
+):
+    recursive_serde_register(
+        __path_type,
+        serialize=serialize_path,
+        deserialize=functools.partial(deserialize_path, __path_type),
+    )
+
+
 def serialize_generic_alias(serialized_type: _GenericAlias) -> bytes:
     # relative
     from ..util.util import full_name_with_name
     from .serialize import _serialize
 
     fqn = full_name_with_name(klass=serialized_type)
     module_parts = fqn.split(".")
```

### Comparing `syft-0.8.2b6/src/syft/serde/serializable.py` & `syft-0.8.2b7/src/syft/serde/serializable.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/serde/signature.py` & `syft-0.8.2b7/src/syft/serde/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/serde/third_party.py` & `syft-0.8.2b7/src/syft/serde/third_party.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/action/action_data_empty.py` & `syft-0.8.2b7/src/syft/service/action/action_data_empty.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/action/action_graph.py` & `syft-0.8.2b7/src/syft/service/action/action_graph.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/action/action_graph_service.py` & `syft-0.8.2b7/src/syft/service/action/action_graph_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/action/action_object.py` & `syft-0.8.2b7/src/syft/service/action/action_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -417,14 +417,15 @@
     """Action object for remote execution."""
 
     __canonical_name__ = "ActionObject"
     __version__ = SYFT_OBJECT_VERSION_1
 
     __attr_searchable__: List[str] = []
     syft_action_data: Optional[Any] = None
+    # syft_action_proxy_reference: Optional[LinkedObject] = None
     syft_pointer_type: ClassVar[Type[ActionObjectPointer]]
 
     # Help with calculating history hash for code verification
     syft_parent_hashes: Optional[Union[int, List[int]]]
     syft_parent_op: Optional[str]
     syft_parent_args: Optional[Any]
     syft_parent_kwargs: Optional[Any]
@@ -433,14 +434,36 @@
     syft_node_uid: Optional[UID]
     _syft_pre_hooks__: Dict[str, List] = {}
     _syft_post_hooks__: Dict[str, List] = {}
     syft_twin_type: TwinMode = TwinMode.NONE
     syft_passthrough_attrs = BASE_PASSTHROUGH_ATTRS
     # syft_dont_wrap_attrs = ["shape"]
 
+    # @property
+    # def syft_action_proxy(self) -> Optional[BlobStorageEntry]:
+    #     return (
+    #         self.syft_action_proxy_reference.resolve
+    #         if self.syft_action_proxy_reference is not None
+    #         else None
+    #     )
+
+    # @property
+    # def syft_action_data(self) -> Any:
+    #     # relative
+    #     from ...client.api import APIRegistry
+
+    #     api = APIRegistry.api_for(
+    #         node_uid=self.node_uid,
+    #         user_verify_key=self.syft_client_verify_key,
+    #     )
+    #     syft_object_resource = api.services.blob_storage.read(
+    #         uid=self.syft_action_proxy_reference.id
+    #     )
+    #     return syft_object_resource.read()
+
     @property
     def is_pointer(self) -> bool:
         return self.syft_node_uid is not None
 
     @property
     def syft_lineage_id(self) -> LineageID:
         """Compute the LineageID of the ActionObject, using the `id` and the `syft_history_hash` memebers"""
```

### Comparing `syft-0.8.2b6/src/syft/service/action/action_permissions.py` & `syft-0.8.2b7/src/syft/service/action/action_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/action/action_service.py` & `syft-0.8.2b7/src/syft/service/action/action_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,17 @@
 from ..warnings import HighSideCRUDWarning
 from .action_object import Action
 from .action_object import ActionObject
 from .action_object import ActionObjectPointer
 from .action_object import ActionType
 from .action_object import AnyActionObject
 from .action_object import TwinMode
+from .action_permissions import ActionObjectPermission
 from .action_permissions import ActionObjectREAD
+from .action_permissions import ActionPermission
 from .action_store import ActionStore
 from .action_types import action_type_for_type
 from .numpy import NumpyArrayObject
 from .pandas import PandasDataFrameObject  # noqa: F401
 from .pandas import PandasSeriesObject  # noqa: F401
 
 
@@ -207,16 +209,26 @@
 
         set_result = self.store.set(
             uid=result_id,
             credentials=context.credentials,
             syft_object=result_action_object,
             has_result_read_permission=True,
         )
+
         if set_result.is_err():
             return set_result.err()
+
+        if len(code_item.output_policy.output_readers) > 0:
+            self.store.add_permissions(
+                [
+                    ActionObjectPermission(result_id, ActionPermission.READ, x)
+                    for x in code_item.output_policy.output_readers
+                ]
+            )
+
         return Ok(result_action_object)
 
     def execute_plan(
         self, plan, context: AuthedServiceContext, plan_kwargs: Dict[str, ActionObject]
     ):
         id2inpkey = {v.id: k for k, v in plan.inputs.items()}
```

### Comparing `syft-0.8.2b6/src/syft/service/action/action_store.py` & `syft-0.8.2b7/src/syft/service/action/action_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/action/action_types.py` & `syft-0.8.2b7/src/syft/service/action/action_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/action/numpy.py` & `syft-0.8.2b7/src/syft/service/action/numpy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/action/pandas.py` & `syft-0.8.2b7/src/syft/service/action/pandas.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/action/plan.py` & `syft-0.8.2b7/src/syft/service/action/plan.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/action/verification.py` & `syft-0.8.2b7/src/syft/service/action/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/code/user_code.py` & `syft-0.8.2b7/src/syft/service/code/user_code.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,34 +5,36 @@
 import ast
 from enum import Enum
 import hashlib
 import inspect
 from io import StringIO
 import itertools
 import sys
+import time
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Type
 from typing import Union
 
 # third party
 from typing_extensions import Self
 
 # relative
 from ...abstract_node import NodeType
-from ...client.api import NodeView
+from ...client.api import NodeIdentity
 from ...client.enclave_client import EnclaveMetadata
 from ...node.credentials import SyftVerifyKey
 from ...serde.deserialize import _deserialize
 from ...serde.serializable import serializable
 from ...serde.serialize import _serialize
 from ...store.document_store import PartitionKey
+from ...types.datetime import DateTime
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftHashableObject
 from ...types.syft_object import SyftObject
 from ...types.transforms import TransformContext
 from ...types.transforms import add_node_uid_for_key
 from ...types.transforms import generate_id
 from ...types.transforms import transform
@@ -52,14 +54,16 @@
 from ..policy.policy import SingleExecutionExactOutput
 from ..policy.policy import SubmitUserPolicy
 from ..policy.policy import UserPolicy
 from ..policy.policy import init_policy
 from ..policy.policy import load_policy_code
 from ..policy.policy_service import PolicyService
 from ..response import SyftError
+from ..response import SyftNotReady
+from ..response import SyftSuccess
 from .code_parse import GlobalsVisitor
 from .unparse import unparse
 
 UserVerifyKeyPartitionKey = PartitionKey(key="user_verify_key", type_=SyftVerifyKey)
 CodeHashPartitionKey = PartitionKey(key="code_hash", type_=int)
 
 PyCodeObject = Any
@@ -85,109 +89,123 @@
 
         uid_kwargs[k] = uid
     return uid_kwargs
 
 
 @serializable()
 class UserCodeStatus(Enum):
-    SUBMITTED = "submitted"
+    PENDING = "pending"
     DENIED = "denied"
-    EXECUTE = "execute"
+    APPROVED = "approved"
 
     def __hash__(self) -> int:
         return hash(self.value)
 
 
 # User Code status context for multiple approvals
 # To make nested dicts hashable for mongodb
 # as status is in attr_searchable
-@serializable(attrs=["base_dict"])
-class UserCodeStatusContext(SyftHashableObject):
-    base_dict: Dict = {}
+@serializable(attrs=["status_dict"])
+class UserCodeStatusCollection(SyftHashableObject):
+    status_dict: Dict[NodeIdentity, UserCodeStatus] = {}
 
-    def __init__(self, base_dict: Dict):
-        self.base_dict = base_dict
+    def __init__(self, status_dict: Dict):
+        self.status_dict = status_dict
 
     def __repr__(self):
-        return str(self.base_dict)
+        return str(self.status_dict)
 
     def _repr_html_(self):
         string = f"""
             <style>
                 .syft-user_code {{color: {SURFACE[options.color_theme]};}}
                 </style>
                 <div class='syft-user_code'>
                     <h3 style="line-height: 25%; margin-top: 25px;">User Code Status</h3>
                     <p style="margin-left: 3px;">
             """
-        for node_view, status in self.base_dict.items():
-            node_name_str = f"{node_view.node_name}"
-            uid_str = f"{node_view.node_id}"
+        for node_identity, status in self.status_dict.items():
+            node_name_str = f"{node_identity.node_name}"
+            uid_str = f"{node_identity.node_id}"
             status_str = f"{status.value}"
-
             string += f"""
                     &#x2022; <strong>UID: </strong>{uid_str}&nbsp;
                     <strong>Node name: </strong>{node_name_str}&nbsp;
                     <strong>Status: </strong>{status_str}
                     <br>
                 """
         string += "</p></div>"
         return string
 
     def __repr_syft_nested__(self):
         string = ""
-        for node_view, status in self.base_dict.items():
-            string += f"{node_view.node_name}: {status}<br>"
+        for node_identity, status in self.status_dict.items():
+            string += f"{node_identity.node_name}: {status}<br>"
         return string
 
+    def get_status_message(self):
+        if self.approved:
+            return SyftSuccess(message=f"{type(self)} approved")
+        string = ""
+        for node_identity, status in self.status_dict.items():
+            string += f"Code status on node '{node_identity.node_name}' is '{status}'. "
+        if self.denied:
+            return SyftError(message=f"{type(self)} Your code cannot be run: {string}")
+        else:
+            return SyftNotReady(
+                message=f"{type(self)} Your code is waiting for approval. {string}"
+            )
+
     @property
     def approved(self) -> bool:
-        # approved for this node only
-        statuses = set(self.base_dict.values())
-        return len(statuses) == 1 and UserCodeStatus.EXECUTE in statuses
+        return all([x == UserCodeStatus.APPROVED for x in self.status_dict.values()])
+
+    @property
+    def denied(self) -> bool:
+        return UserCodeStatus.DENIED in self.status_dict.values()
 
-    def for_context(self, context: AuthedServiceContext) -> UserCodeStatus:
+    def for_user_context(self, context: AuthedServiceContext) -> UserCodeStatus:
         if context.node.node_type == NodeType.ENCLAVE:
-            keys = set(self.base_dict.values())
-            if len(keys) == 1 and UserCodeStatus.EXECUTE in keys:
-                return UserCodeStatus.EXECUTE
-            elif UserCodeStatus.SUBMITTED in keys and UserCodeStatus.DENIED not in keys:
-                return UserCodeStatus.SUBMITTED
+            keys = set(self.status_dict.values())
+            if len(keys) == 1 and UserCodeStatus.APPROVED in keys:
+                return UserCodeStatus.APPROVED
+            elif UserCodeStatus.PENDING in keys and UserCodeStatus.DENIED not in keys:
+                return UserCodeStatus.PENDING
             elif UserCodeStatus.DENIED in keys:
                 return UserCodeStatus.DENIED
             else:
                 return Exception(f"Invalid types in {keys} for Code Submission")
 
         elif context.node.node_type == NodeType.DOMAIN:
-            node_view = NodeView(
+            node_identity = NodeIdentity(
                 node_name=context.node.name,
                 node_id=context.node.id,
                 verify_key=context.node.signing_key.verify_key,
             )
-            if node_view in self.base_dict:
-                return self.base_dict[node_view]
+            if node_identity in self.status_dict:
+                return self.status_dict[node_identity]
             else:
                 raise Exception(
                     f"Code Object does not contain {context.node.name} Domain's data"
                 )
         else:
             raise Exception(
                 f"Invalid Node Type for Code Submission:{context.node.node_type}"
             )
 
     def mutate(
         self, value: UserCodeStatus, node_name: str, node_id, verify_key: SyftVerifyKey
     ) -> Union[SyftError, Self]:
-        node_view = NodeView(
+        node_identity = NodeIdentity(
             node_name=node_name, node_id=node_id, verify_key=verify_key
         )
-        base_dict = self.base_dict
-        if node_view in base_dict:
-            base_dict[node_view] = value
-            self.base_dict = base_dict
+        status_dict = self.status_dict
+        if node_identity in status_dict:
+            status_dict[node_identity] = value
+            self.status_dict = status_dict
             return self
         else:
             return SyftError(
                 message="Cannot Modify Status as the Domain's data is not included in the request"
             )
 
 
@@ -209,71 +227,96 @@
     output_policy_state: bytes = b""
     parsed_code: str
     service_func_name: str
     unique_func_name: str
     user_unique_func_name: str
     code_hash: str
     signature: inspect.Signature
-    status: UserCodeStatusContext
+    status: UserCodeStatusCollection
     input_kwargs: List[str]
     enclave_metadata: Optional[EnclaveMetadata] = None
+    submit_time: Optional[DateTime]
 
     __attr_searchable__ = ["user_verify_key", "status", "service_func_name"]
-    __attr_unique__ = ["code_hash", "user_unique_func_name"]
-    __repr_attrs__ = ["status.approved", "service_func_name", "shareholders"]
+    __attr_unique__ = []
+    __repr_attrs__ = ["service_func_name", "input_owners", "code_status"]
 
     def __setattr__(self, key: str, value: Any) -> None:
         attr = getattr(type(self), key, None)
         if inspect.isdatadescriptor(attr):
             attr.fset(self, value)
         else:
             return super().__setattr__(key, value)
 
     def _coll_repr_(self) -> Dict[str, Any]:
-        status = list(self.status.base_dict.values())[0].value
-        if status == UserCodeStatus.SUBMITTED.value:
+        status = list(self.status.status_dict.values())[0].value
+        if status == UserCodeStatus.PENDING.value:
             badge_color = "badge-purple"
-        elif status == UserCodeStatus.EXECUTE.value:
+        elif status == UserCodeStatus.APPROVED.value:
             badge_color = "badge-green"
         else:
             badge_color = "badge-red"
         status_badge = {"value": status, "type": badge_color}
         return {
             "Input Policy": self.input_policy_type.__canonical_name__,
             "Output Policy": self.output_policy_type.__canonical_name__,
             "Function name": self.service_func_name,
             "User verify key": {
                 "value": str(self.user_verify_key),
                 "type": "clipboard",
             },
             "Status": status_badge,
+            "Submit time": str(self.submit_time),
         }
 
     @property
-    def shareholders(self) -> List[str]:
-        node_names_list = []
-        nodes = self.input_policy_init_kwargs.keys()
-        for node_view in nodes:
-            node_names_list.append(str(node_view.node_name))
-        return node_names_list
+    def is_enclave_code(self) -> bool:
+        return self.enclave_metadata is not None
+
+    @property
+    def input_owners(self) -> List[str]:
+        return [str(x.node_name) for x in self.input_policy_init_kwargs.keys()]
+
+    @property
+    def input_owner_verify_keys(self) -> List[SyftVerifyKey]:
+        return [x.verify_key for x in self.input_policy_init_kwargs.keys()]
+
+    @property
+    def output_reader_names(self) -> List[SyftVerifyKey]:
+        keys = self.output_policy_init_kwargs.get("output_readers", [])
+        inpkey2name = {x.verify_key: x.node_name for x in self.input_policy_init_kwargs}
+        return [inpkey2name[k] for k in keys if k in inpkey2name]
+
+    @property
+    def output_readers(self) -> List[SyftVerifyKey]:
+        return self.output_policy_init_kwargs.get("output_readers", [])
+
+    @property
+    def code_status(self) -> list:
+        status_list = []
+        for node_view, status in self.status.status_dict.items():
+            status_list.append(
+                f"Node: {node_view.node_name}, Status: {status.value}",
+            )
+        return status_list
 
     @property
     def input_policy(self) -> Optional[InputPolicy]:
         if not self.status.approved:
             return None
 
         if len(self.input_policy_state) == 0:
             input_policy = None
             if isinstance(self.input_policy_type, type) and issubclass(
                 self.input_policy_type, InputPolicy
             ):
                 # TODO: Tech Debt here
                 node_view_workaround = False
                 for k, _ in self.input_policy_init_kwargs.items():
-                    if isinstance(k, NodeView):
+                    if isinstance(k, NodeIdentity):
                         node_view_workaround = True
 
                 if node_view_workaround:
                     input_policy = self.input_policy_type(
                         init_kwargs=self.input_policy_init_kwargs
                     )
                 else:
@@ -352,27 +395,34 @@
         else:
             raise Exception(f"You can't set {type(value)} as output_policy_state")
 
     @property
     def byte_code(self) -> Optional[PyCodeObject]:
         return compile_byte_code(self.parsed_code)
 
+    def get_results(self) -> Any:
+        # relative
+        from ...client.api import APIRegistry
+
+        api = APIRegistry.api_for(self.node_uid, self.syft_client_verify_key)
+        return api.services.code.get_results(self)
+
     @property
     def assets(self) -> List[Asset]:
         # relative
         from ...client.api import APIRegistry
 
         api = APIRegistry.api_for(self.node_uid, self.syft_client_verify_key)
         if api is None:
             return SyftError(message=f"You must login to {self.node_uid}")
 
         inputs = (
             uids
-            for node_view, uids in self.input_policy_init_kwargs.items()
-            if node_view.node_name == api.node_name
+            for node_identity, uids in self.input_policy_init_kwargs.items()
+            if node_identity.node_name == api.node_name
         )
         all_assets = []
         for uid in itertools.chain.from_iterable(x.values() for x in inputs):
             if isinstance(uid, UID):
                 assets = api.services.dataset.get_assets_by_action_id(uid)
                 if not isinstance(assets, list):
                     return assets
@@ -414,19 +464,28 @@
                 return result
             except Exception as e:
                 print(f"Failed to run unsafe_function. {e}")
 
         return wrapper
 
     def _repr_markdown_(self):
+        shared_with_line = ""
+        if len(self.output_readers) > 0:
+            owners_string = " and ".join([f"*{x}*" for x in self.output_reader_names])
+            shared_with_line += (
+                f"Custom Policy: "
+                f"outputs are *shared* with the owners of {owners_string} once computed"
+            )
+
         md = f"""class UserCode
     id: UID = {self.id}
-    status.approved: bool = {self.status.approved}
     service_func_name: str = {self.service_func_name}
-    shareholders: list = {self.shareholders}
+    shareholders: list = {self.input_owners}
+    status: list = {self.code_status}
+    {shared_with_line}
     code:
 
 {self.raw_code}"""
         return as_markdown_code(md)
 
     @property
     def show_code(self) -> CodeMarkdown:
@@ -483,14 +542,18 @@
                 print("Warning: The result you see is computed on PRIVATE data.")
             elif on_mock_data:
                 print("Warning: The result you see is computed on MOCK data.")
             return self.local_function(**filtered_kwargs)
         else:
             raise NotImplementedError
 
+    @property
+    def input_owner_verify_keys(self) -> List[str]:
+        return [x.verify_key for x in self.input_policy_init_kwargs.keys()]
+
 
 class ArgumentType(Enum):
     REAL = 1
     MOCK = 2
     PRIVATE = 4
 
 
@@ -503,24 +566,28 @@
         else:
             return asset.mock, ArgumentType.MOCK
     if hasattr(deboxed_arg, "syft_action_data"):
         deboxed_arg = deboxed_arg.syft_action_data
     return deboxed_arg, ArgumentType.REAL
 
 
-def syft_function_single_use(*args: Any, **kwargs: Any):
+def syft_function_single_use(
+    *args: Any, share_results_with_owners=False, **kwargs: Any
+):
     return syft_function(
         input_policy=ExactMatch(*args, **kwargs),
         output_policy=SingleExecutionExactOutput(),
+        share_results_with_owners=share_results_with_owners,
     )
 
 
 def syft_function(
     input_policy: Union[InputPolicy, UID],
     output_policy: Optional[Union[OutputPolicy, UID]] = None,
+    share_results_with_owners=False,
 ) -> SubmitUserCode:
     if isinstance(input_policy, CustomInputPolicy):
         input_policy_type = SubmitUserPolicy.from_obj(input_policy)
     else:
         input_policy_type = type(input_policy)
 
     if output_policy is None:
@@ -533,35 +600,43 @@
 
     def decorator(f):
         print(
             f"Syft function '{f.__name__}' successfully created. "
             f"To add a code request, please create a project using `project = syft.Project(...)`, "
             f"then use command `project.create_code_request`."
         )
-        return SubmitUserCode(
+        res = SubmitUserCode(
             code=inspect.getsource(f),
             func_name=f.__name__,
             signature=inspect.signature(f),
             input_policy_type=input_policy_type,
             input_policy_init_kwargs=input_policy.init_kwargs,
             output_policy_type=output_policy_type,
             output_policy_init_kwargs=output_policy.init_kwargs,
             local_function=f,
             input_kwargs=f.__code__.co_varnames[: f.__code__.co_argcount],
         )
 
+        if share_results_with_owners:
+            res.output_policy_init_kwargs[
+                "output_readers"
+            ] = res.input_owner_verify_keys
+        return res
+
     return decorator
 
 
 def generate_unique_func_name(context: TransformContext) -> TransformContext:
     code_hash = context.output["code_hash"]
     service_func_name = context.output["func_name"]
     context.output["service_func_name"] = service_func_name
     func_name = f"user_func_{service_func_name}_{context.credentials}_{code_hash}"
-    user_unique_func_name = f"user_func_{service_func_name}_{context.credentials}"
+    user_unique_func_name = (
+        f"user_func_{service_func_name}_{context.credentials}_{time.time()}"
+    )
     context.output["unique_func_name"] = func_name
     context.output["user_unique_func_name"] = user_unique_func_name
     return context
 
 
 def process_code(
     raw_code: str,
@@ -603,15 +678,15 @@
 
 
 def new_check_code(context: TransformContext) -> TransformContext:
     # TODO remove this tech debt hack
     input_kwargs = context.output["input_policy_init_kwargs"]
     node_view_workaround = False
     for k in input_kwargs.keys():
-        if isinstance(k, NodeView):
+        if isinstance(k, NodeIdentity):
             node_view_workaround = True
 
     if not node_view_workaround:
         input_keys = list(input_kwargs.keys())
     else:
         input_keys = []
         for d in input_kwargs.values():
@@ -688,50 +763,56 @@
     context.output["output_policy_type"] = op
     return context
 
 
 def add_custom_status(context: TransformContext) -> TransformContext:
     input_keys = list(context.output["input_policy_init_kwargs"].keys())
     if context.node.node_type == NodeType.DOMAIN:
-        node_view = NodeView(
+        node_identity = NodeIdentity(
             node_name=context.node.name,
             node_id=context.node.id,
             verify_key=context.node.signing_key.verify_key,
         )
-        context.output["status"] = UserCodeStatusContext(
-            base_dict={node_view: UserCodeStatus.SUBMITTED}
+        context.output["status"] = UserCodeStatusCollection(
+            status_dict={node_identity: UserCodeStatus.PENDING}
         )
-        # if node_view in input_keys or len(input_keys) == 0:
+        # if node_identity in input_keys or len(input_keys) == 0:
         #     context.output["status"] = UserCodeStatusContext(
-        #         base_dict={node_view: UserCodeStatus.SUBMITTED}
+        #         base_dict={node_identity: UserCodeStatus.SUBMITTED}
         #     )
         # else:
-        #     raise ValueError(f"Invalid input keys: {input_keys} for {node_view}")
+        #     raise ValueError(f"Invalid input keys: {input_keys} for {node_identity}")
     elif context.node.node_type == NodeType.ENCLAVE:
-        base_dict = {key: UserCodeStatus.SUBMITTED for key in input_keys}
-        context.output["status"] = UserCodeStatusContext(base_dict=base_dict)
+        status_dict = {key: UserCodeStatus.PENDING for key in input_keys}
+        context.output["status"] = UserCodeStatusCollection(status_dict=status_dict)
     else:
         raise NotImplementedError(
             f"Invalid node type:{context.node.node_type} for code submission"
         )
     return context
 
 
+def add_submit_time(context: TransformContext) -> TransformContext:
+    context.output["submit_time"] = DateTime.now()
+    return context
+
+
 @transform(SubmitUserCode, UserCode)
 def submit_user_code_to_user_code() -> List[Callable]:
     return [
         generate_id,
         hash_code,
         generate_unique_func_name,
         check_input_policy,
         check_output_policy,
         new_check_code,
         add_credentials_for_key("user_verify_key"),
         add_custom_status,
         add_node_uid_for_key("node_uid"),
+        add_submit_time,
     ]
 
 
 @serializable()
 class UserCodeExecutionResult(SyftObject):
     # version
     __canonical_name__ = "UserCodeExecutionResult"
```

### Comparing `syft-0.8.2b6/src/syft/service/code/user_code_parse.py` & `syft-0.8.2b7/src/syft/service/code/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/code/user_code_service.py` & `syft-0.8.2b7/src/syft/service/code/user_code_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,28 +6,31 @@
 from typing import Union
 
 # third party
 from result import OkErr
 from result import Result
 
 # relative
+from ...abstract_node import NodeType
+from ...client.enclave_client import EnclaveClient
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
 from ...store.linked_obj import LinkedObject
 from ...types.twin_object import TwinObject
 from ...types.uid import UID
 from ...util.telemetry import instrument
 from ..action.action_object import ActionObject
+from ..action.action_permissions import ActionObjectPermission
+from ..action.action_permissions import ActionPermission
 from ..context import AuthedServiceContext
-from ..policy.policy import OutputHistory
+from ..network.routes import route_to_connection
 from ..request.request import SubmitRequest
 from ..request.request import UserCodeStatusChange
 from ..request.request_service import RequestService
 from ..response import SyftError
-from ..response import SyftNotReady
 from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import SERVICE_TO_TYPES
 from ..service import TYPE_TO_SERVICE
 from ..service import service_method
 from ..user.user_roles import GUEST_ROLE_LEVEL
 from .user_code import SubmitUserCode
@@ -48,34 +51,56 @@
         self.stash = UserCodeStash(store=store)
 
     @service_method(path="code.submit", name="submit", roles=GUEST_ROLE_LEVEL)
     def submit(
         self, context: AuthedServiceContext, code: SubmitUserCode
     ) -> Union[UserCode, SyftError]:
         """Add User Code"""
-        result = self.stash.set(context.credentials, code.to(UserCode, context=context))
+        result = self._submit(context=context, code=code)
         if result.is_err():
             return SyftError(message=str(result.err()))
         return SyftSuccess(message="User Code Submitted")
 
+    def _submit(self, context: AuthedServiceContext, code: SubmitUserCode) -> Result:
+        result = self.stash.set(context.credentials, code.to(UserCode, context=context))
+        return result
+
     def _request_code_execution(
         self,
         context: AuthedServiceContext,
         code: SubmitUserCode,
         reason: Optional[str] = "",
     ):
-        user_code = code.to(UserCode, context=context)
+        user_code: UserCode = code.to(UserCode, context=context)
+        if not all(
+            [x in user_code.input_owner_verify_keys for x in user_code.output_readers]
+        ):
+            raise ValueError("outputs can only be distributed to input owners")
         result = self.stash.set(context.credentials, user_code)
         if result.is_err():
             return SyftError(message=str(result.err()))
 
+        # Create a code history
+        code_history_service = context.node.get_service("codehistoryservice")
+        result = code_history_service.submit_version(context=context, code=user_code)
+        if isinstance(result, SyftError):
+            return result
+
+        # Users that have access to the output also have access to the code item
+        self.stash.add_permissions(
+            [
+                ActionObjectPermission(user_code.id, ActionPermission.READ, x)
+                for x in user_code.output_readers
+            ]
+        )
+
         linked_obj = LinkedObject.from_obj(user_code, node_uid=context.node.id)
 
         CODE_EXECUTE = UserCodeStatusChange(
-            value=UserCodeStatus.EXECUTE, linked_obj=linked_obj
+            value=UserCodeStatus.APPROVED, linked_obj=linked_obj
         )
         changes = [CODE_EXECUTE]
 
         request = SubmitRequest(changes=changes)
         method = context.node.get_service_method(RequestService.submit)
         result = method(context=context, request=request, reason=reason)
 
@@ -141,117 +166,152 @@
 
     def load_user_code(self, context: AuthedServiceContext) -> None:
         result = self.stash.get_all(credentials=context.credentials)
         if result.is_ok():
             user_code_items = result.ok()
             load_approved_policy_code(user_code_items=user_code_items)
 
+    @service_method(path="code.get_results", name="get_results", roles=GUEST_ROLE_LEVEL)
+    def get_results(
+        self, context: AuthedServiceContext, inp: Union[UID, UserCode]
+    ) -> Union[List[UserCode], SyftError]:
+        uid = inp.id if isinstance(inp, UserCode) else inp
+        code_result = self.stash.get_by_uid(context.credentials, uid=uid)
+
+        if code_result.is_err():
+            return SyftError(message=code_result.err())
+        code = code_result.ok()
+
+        if code.is_enclave_code:
+            # if the current node is not the enclave
+            if not context.node.node_type == NodeType.ENCLAVE:
+                connection = route_to_connection(code.enclave_metadata.route)
+                enclave_client = EnclaveClient(
+                    connection=connection,
+                    credentials=context.node.signing_key,
+                )
+                return enclave_client.code.get_results(code.id)
+
+            # if the current node is the enclave
+            else:
+                if not code.status.approved:
+                    return code.status.get_status_message()
+
+                if (output_policy := code.output_policy) is None:
+                    return SyftError(message=f"Output policy not approved {code}")
+
+                if len(output_policy.output_history) > 0:
+                    return resolve_outputs(
+                        context=context, output_ids=output_policy.last_output_ids
+                    )
+                else:
+                    return SyftError(message="No results available")
+        else:
+            return SyftError(message="Endpoint only supported for enclave code")
+
     @service_method(path="code.call", name="call", roles=GUEST_ROLE_LEVEL)
     def call(
         self, context: AuthedServiceContext, uid: UID, **kwargs: Any
     ) -> Union[SyftSuccess, SyftError]:
         """Call a User Code Function"""
         try:
-            filtered_kwargs = filter_kwargs(kwargs)
-            result = self.stash.get_by_uid(context.credentials, uid=uid)
-            if not result.is_ok():
-                return SyftError(message=result.err())
-
             # Unroll variables
-            code_item = result.ok()
-            code_status = code_item.status
+            kwarg2id = map_kwargs_to_id(kwargs)
 
-            # Check if the user has permission to execute the code
-            # They can execute if they are root user or if they are the user who submitted the code
-            if not (
-                context.credentials == context.node.verify_key
-                or context.credentials == code_item.user_verify_key
-            ):
-                return SyftError(
-                    message=f"Code Execution Permission: {context.credentials} denied"
-                )
-
-            # Check if the code is approved
-            if code_status.for_context(context) != UserCodeStatus.EXECUTE:
-                if code_status.for_context(context) == UserCodeStatus.SUBMITTED:
-                    string = ""
-                    for node_view, status in code_status.base_dict.items():
-                        string += f"Code status on node '{node_view.node_name}' is '{status.value}'. "
-                    return SyftNotReady(
-                        message=f"{type(code_item)} Your code is waiting for approval. {string}"
-                    )
-                return SyftError(
-                    message=f"{type(code_item)} Your code cannot be run: {code_status.for_context(context)}"
-                )
+            # get code item
+            code_result = self.stash.get_by_uid(context.credentials, uid=uid)
+            if code_result.is_err():
+                return SyftError(message=code_result.err())
+            code: UserCode = code_result.ok()
+
+            if not code.status.approved:
+                return code.status.get_status_message()
+
+            # Check if the user has permission to execute the code.
+            if not (has_code_permission := self.has_code_permission(code, context)):
+                return has_code_permission
 
-            output_policy = code_item.output_policy
-            if output_policy is None:
-                raise Exception("Output policy not approved", code_item)
+            if (output_policy := code.output_policy) is None:
+                return SyftError("Output policy not approved", code)
 
             # Check if the OutputPolicy is valid
-            is_valid = output_policy.valid
-
-            if not is_valid:
+            if not (is_valid := output_policy.valid):
                 if len(output_policy.output_history) > 0:
-                    result = get_outputs(
-                        context=context,
-                        output_history=output_policy.output_history[-1],
+                    result = resolve_outputs(
+                        context=context, output_ids=output_policy.last_output_ids
                     )
                     return result.as_empty()
                 return is_valid
 
             # Execute the code item
             action_service = context.node.get_service("actionservice")
-            result: Result = action_service._user_code_execute(
-                context, code_item, filtered_kwargs
-            )
-            if isinstance(result, str):
-                return SyftError(message=result)
+
+            output_result: Result[
+                Union[ActionObject, TwinObject], str
+            ] = action_service._user_code_execute(context, code, kwarg2id)
+
+            if output_result.is_err():
+                return SyftError(message=output_result.err())
+            result = output_result.ok()
 
             # Apply Output Policy to the results and update the OutputPolicyState
-            result: Union[ActionObject, TwinObject] = result.ok()
             output_policy.apply_output(context=context, outputs=result)
-            code_item.output_policy = output_policy
-            update_success = self.update_code_state(
-                context=context, code_item=code_item
-            )
-            if not update_success:
+            code.output_policy = output_policy
+            if not (
+                update_success := self.update_code_state(
+                    context=context, code_item=code
+                )
+            ):
                 return update_success
+
             if isinstance(result, TwinObject):
                 return result.mock
             else:
                 return result.as_empty()
         except Exception as e:
             return SyftError(message=f"Failed to run. {e}")
 
+    def has_code_permission(self, code_item, context):
+        if not (
+            context.credentials == context.node.verify_key
+            or context.credentials == code_item.user_verify_key
+        ):
+            return SyftError(
+                message=f"Code Execution Permission: {context.credentials} denied"
+            )
+        return SyftSuccess(message="you have permission")
+
 
-def get_outputs(context: AuthedServiceContext, output_history: OutputHistory) -> Any:
+def resolve_outputs(
+    context: AuthedServiceContext,
+    output_ids: Optional[Union[List[UID], Dict[str, UID]]],
+) -> Any:
     # relative
     from ...service.action.action_object import TwinMode
 
-    if isinstance(output_history.outputs, list):
-        if len(output_history.outputs) == 0:
+    if isinstance(output_ids, list):
+        if len(output_ids) == 0:
             return None
         outputs = []
-        for output_id in output_history.outputs:
+        for output_id in output_ids:
             action_service = context.node.get_service("actionservice")
             result = action_service.get(
                 context, uid=output_id, twin_mode=TwinMode.PRIVATE
             )
             if isinstance(result, OkErr):
                 result = result.value
             outputs.append(result)
         if len(outputs) == 1:
             return outputs[0]
         return outputs
     else:
         raise NotImplementedError
 
 
-def filter_kwargs(kwargs: Dict[str, Any]) -> Dict[str, Any]:
+def map_kwargs_to_id(kwargs: Dict[str, Any]) -> Dict[str, Any]:
     # relative
     from ...types.twin_object import TwinObject
     from ..action.action_object import ActionObject
     from ..dataset.dataset import Asset
 
     filtered_kwargs = {}
     for k, v in kwargs.items():
```

### Comparing `syft-0.8.2b6/src/syft/service/code/user_code_stash.py` & `syft-0.8.2b7/src/syft/service/code/user_code_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/context.py` & `syft-0.8.2b7/src/syft/service/context.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/data_subject/data_subject.py` & `syft-0.8.2b7/src/syft/service/data_subject/data_subject.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/data_subject/data_subject_member.py` & `syft-0.8.2b7/src/syft/service/data_subject/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/data_subject/data_subject_member_service.py` & `syft-0.8.2b7/src/syft/service/data_subject/data_subject_member_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/data_subject/data_subject_service.py` & `syft-0.8.2b7/src/syft/service/data_subject/data_subject_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/dataset/dataset.py` & `syft-0.8.2b7/src/syft/service/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/dataset/dataset_service.py` & `syft-0.8.2b7/src/syft/service/dataset/dataset_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/dataset/dataset_stash.py` & `syft-0.8.2b7/src/syft/service/dataset/dataset_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/enclave/enclave_service.py` & `syft-0.8.2b7/src/syft/service/enclave/enclave_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         user_code_service = context.node.get_service("usercodeservice")
         action_service = context.node.get_service("actionservice")
         user_code = user_code_service.get_by_uid(context=root_context, uid=user_code_id)
         if isinstance(user_code, SyftError):
             return user_code
 
         status_update = user_code.status.mutate(
-            value=UserCodeStatus.EXECUTE,
+            value=UserCodeStatus.APPROVED,
             node_name=node_name,
             node_id=node_id,
             verify_key=context.credentials,
         )
         if isinstance(status_update, SyftError):
             return status_update
```

### Comparing `syft-0.8.2b6/src/syft/service/metadata/metadata_service.py` & `syft-0.8.2b7/src/syft/service/metadata/metadata_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/metadata/node_metadata.py` & `syft-0.8.2b7/src/syft/service/metadata/node_metadata.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/network/network_service.py` & `syft-0.8.2b7/src/syft/service/network/network_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/network/node_peer.py` & `syft-0.8.2b7/src/syft/service/network/node_peer.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/network/routes.py` & `syft-0.8.2b7/src/syft/service/network/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/notification/notification_service.py` & `syft-0.8.2b7/src/syft/service/notification/notification_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/notification/notification_stash.py` & `syft-0.8.2b7/src/syft/service/notification/notification_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/notification/notifications.py` & `syft-0.8.2b7/src/syft/service/notification/notifications.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/policy/policy.py` & `syft-0.8.2b7/src/syft/service/policy/policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # third party
 from RestrictedPython import compile_restricted
 from result import Ok
 
 # relative
 from ...abstract_node import NodeType
-from ...client.api import NodeView
+from ...client.api import NodeIdentity
 from ...node.credentials import SyftVerifyKey
 from ...serde.recursive_primitives import recursive_serde_register_type
 from ...serde.serializable import serializable
 from ...store.document_store import PartitionKey
 from ...types.datetime import DateTime
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftObject
@@ -127,15 +127,15 @@
     DENIED = "denied"
     APPROVED = "approved"
 
 
 def partition_by_node(kwargs: Dict[str, Any]) -> Dict[str, UID]:
     # relative
     from ...client.api import APIRegistry
-    from ...client.api import NodeView
+    from ...client.api import NodeIdentity
     from ...types.twin_object import TwinObject
     from ..action.action_object import ActionObject
 
     # fetches the all the current api's connected
     api_list = APIRegistry.get_all_api()
     output_kwargs = {}
     for k, v in kwargs.items():
@@ -149,19 +149,19 @@
 
         if not isinstance(uid, UID):
             raise Exception(f"Input {k} must have a UID not {type(v)}")
 
         _obj_exists = False
         for api in api_list:
             if api.services.action.exists(uid):
-                node_view = NodeView.from_api(api)
-                if node_view not in output_kwargs:
-                    output_kwargs[node_view] = {k: uid}
+                node_identity = NodeIdentity.from_api(api)
+                if node_identity not in output_kwargs:
+                    output_kwargs[node_identity] = {k: uid}
                 else:
-                    output_kwargs[node_view].update({k: uid})
+                    output_kwargs[node_identity].update({k: uid})
 
                 _obj_exists = True
                 break
 
         if not _obj_exists:
             raise Exception(f"Input data {k}:{uid} does not belong to any Domain")
 
@@ -183,19 +183,19 @@
 
     def filter_kwargs(
         self, kwargs: Dict[Any, Any], context: AuthedServiceContext, code_item_id: UID
     ) -> Dict[Any, Any]:
         raise NotImplementedError
 
     @property
-    def inputs(self) -> Dict[NodeView, Any]:
+    def inputs(self) -> Dict[NodeIdentity, Any]:
         return self.init_kwargs
 
     def _inputs_for_context(self, context: ChangeContext):
-        user_node_view = NodeView.from_change_context(context)
+        user_node_view = NodeIdentity.from_change_context(context)
         inputs = self.inputs[user_node_view]
 
         action_service = context.node.get_service("actionservice")
         for var_name, uid in inputs.items():
             action_object = action_service.store.get(
                 uid=uid, credentials=user_node_view.verify_key
             )
@@ -247,20 +247,20 @@
 
 def allowed_ids_only(
     allowed_inputs: Dict[str, UID],
     kwargs: Dict[str, Any],
     context: AuthedServiceContext,
 ) -> Dict[str, UID]:
     if context.node.node_type == NodeType.DOMAIN:
-        node_view = NodeView(
+        node_identity = NodeIdentity(
             node_name=context.node.name,
             node_id=context.node.id,
             verify_key=context.node.signing_key.verify_key,
         )
-        allowed_inputs = allowed_inputs[node_view]
+        allowed_inputs = allowed_inputs[node_identity]
     elif context.node.node_type == NodeType.ENCLAVE:
         base_dict = {}
         for key in allowed_inputs.values():
             base_dict.update(key)
         allowed_inputs = base_dict
     else:
         raise Exception(
@@ -315,14 +315,15 @@
     # version
     __canonical_name__ = "OutputPolicy"
     __version__ = SYFT_OBJECT_VERSION_1
 
     output_history: List[OutputHistory] = []
     output_kwargs: List[str] = []
     node_uid: Optional[UID]
+    output_readers: List[SyftVerifyKey] = []
 
     def apply_output(
         self,
         context: NodeServiceContext,
         outputs: Any,
     ) -> Any:
         output_uids = filter_only_uids(outputs)
@@ -336,14 +337,18 @@
         self.output_history.append(history)
         return outputs
 
     @property
     def outputs(self) -> List[str]:
         return self.output_kwargs
 
+    @property
+    def last_output_ids(self) -> List[str]:
+        return self.output_history[-1].outputs
+
 
 @serializable()
 class OutputPolicyExecuteCount(OutputPolicy):
     __canonical_name__ = "OutputPolicyExecuteCount"
     __version__ = SYFT_OBJECT_VERSION_1
 
     count: int = 0
```

### Comparing `syft-0.8.2b6/src/syft/service/policy/policy_service.py` & `syft-0.8.2b7/src/syft/service/policy/policy_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/policy/user_policy_stash.py` & `syft-0.8.2b7/src/syft/service/policy/user_policy_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/project/project.py` & `syft-0.8.2b7/src/syft/service/project/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,28 +20,31 @@
 # third party
 import pydantic
 from pydantic import validator
 from rich.progress import Progress
 from typing_extensions import Self
 
 # relative
+from ...client.api import NodeIdentity
 from ...client.client import SyftClient
 from ...client.client import SyftClientSessionCache
 from ...node.credentials import SyftSigningKey
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
 from ...serde.serialize import _serialize
 from ...service.metadata.node_metadata import NodeMetadata
 from ...store.linked_obj import LinkedObject
 from ...types.datetime import DateTime
+from ...types.identity import Identity
+from ...types.identity import UserIdentity
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftObject
 from ...types.syft_object import short_qual_name
 from ...types.transforms import TransformContext
-from ...types.transforms import keep
+from ...types.transforms import rename
 from ...types.transforms import transform
 from ...types.uid import UID
 from ...util import options
 from ...util.colors import SURFACE
 from ...util.markdown import markdown_as_class_with_fields
 from ...util.util import full_name_with_qualname
 from ..code.user_code import SubmitUserCode
@@ -56,52 +59,17 @@
 
 
 @serializable()
 class EventAlreadyAddedException(SyftException):
     pass
 
 
-class Identity(SyftObject):
-    __canonical_name__ = "Identity"
-    __version__ = SYFT_OBJECT_VERSION_1
-
-    id: UID
-    verify_key: SyftVerifyKey
-
-    __repr_attrs__ = ["id", "verify_key"]
-
-    def __repr__(self) -> str:
-        verify_key_str = f"{self.verify_key}"
-        return f"<🔑 {verify_key_str[0:8]} @ 🟢 {self.id.short()}>"
-
-    @classmethod
-    def from_client(cls, client: SyftClient) -> Identity:
-        return cls(id=client.id, verify_key=client.credentials.verify_key)
-
-
-@serializable()
-class NodeIdentity(Identity):
-    """This class is used to identify the node owner"""
-
-    __canonical_name__ = "NodeIdentity"
-    __version__ = SYFT_OBJECT_VERSION_1
-
-
-# Used to Identity data scientist users of the node
-@serializable()
-class UserIdentity(Identity):
-    """This class is used to identify the data scientist users of the node"""
-
-    __canonical_name__ = "UserIdentity"
-    __version__ = SYFT_OBJECT_VERSION_1
-
-
 @transform(NodeMetadata, NodeIdentity)
 def metadata_to_node_identity() -> List[Callable]:
-    return [keep(["id", "verify_key"])]
+    return [rename("id", "node_id"), rename("name", "node_name")]
 
 
 class ProjectEvent(SyftObject):
     __canonical_name__ = "ProjectEvent"
     __version__ = SYFT_OBJECT_VERSION_1
 
     __hash_exclude_attrs__ = ["event_hash", "signature"]
```

### Comparing `syft-0.8.2b6/src/syft/service/project/project_service.py` & `syft-0.8.2b7/src/syft/service/project/project_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/project/project_stash.py` & `syft-0.8.2b7/src/syft/service/project/project_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/queue/base_queue.py` & `syft-0.8.2b7/src/syft/service/queue/base_queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,16 @@
     pass
 
 
 @serializable()
 class QueueConfig:
     """Base Queue configuration"""
 
-    client_config: Type[QueueClientConfig]
     client_type: Type[QueueClient]
+    client_config: QueueClientConfig
 
 
 @serializable()
 class BaseQueueManager:
     config: QueueConfig
 
     def __init__(self, config: QueueConfig):
```

### Comparing `syft-0.8.2b6/src/syft/service/queue/queue.py` & `syft-0.8.2b7/src/syft/service/queue/queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 @serializable()
 class QueueManager(BaseQueueManager):
     config: QueueConfig
 
     def post_init(self):
-        self.client_config = self.config.client_config()
+        self.client_config = self.config.client_config
         self._client = self.config.client_type(self.client_config)
 
     def close(self):
         return self._client.close()
 
     def create_consumer(
         self,
```

### Comparing `syft-0.8.2b6/src/syft/service/queue/queue_stash.py` & `syft-0.8.2b7/src/syft/service/queue/queue_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/queue/zmq_queue.py` & `syft-0.8.2b7/src/syft/service/queue/zmq_queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from typing import DefaultDict
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 # third party
 import gevent
-from pydantic import validator
 import zmq.green as zmq
 
 # relative
 from ...serde.serializable import serializable
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftObject
 from ...types.uid import UID
@@ -110,19 +109,15 @@
 
 @serializable()
 class ZMQClientConfig(SyftObject, QueueClientConfig):
     __canonical_name__ = "ZMQClientConfig"
     __version__ = SYFT_OBJECT_VERSION_1
 
     id: Optional[UID]
-    hostname: Optional[str]
-
-    @validator("hostname", pre=True, always=True)
-    def get_hostname(cls, v: Optional[str]) -> str:
-        return "127.0.0.1" if v is None else v
+    hostname: str = "127.0.0.1"
 
 
 @serializable(attrs=["host"])
 class ZMQClient(QueueClient):
     """ZMQ Client for creating producers and consumers."""
 
     producers: Dict[str, ZMQProducer]
@@ -252,9 +247,9 @@
             self.purge_queue(queue_name=queue_name)
 
         return SyftSuccess(message="Successfully purged all queues.")
 
 
 @serializable()
 class ZMQQueueConfig(QueueConfig):
-    client_config = ZMQClientConfig
     client_type = ZMQClient
+    client_config = ZMQClientConfig()
```

### Comparing `syft-0.8.2b6/src/syft/service/request/request.py` & `syft-0.8.2b7/src/syft/service/request/request.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,14 +145,16 @@
 @serializable()
 class Request(SyftObject):
     __canonical_name__ = "Request"
     __version__ = SYFT_OBJECT_VERSION_1
 
     requesting_user_verify_key: SyftVerifyKey
     requesting_user_name: str = ""
+    requesting_user_email: Optional[str] = ""
+    requesting_user_institution: Optional[str] = ""
     approving_user_verify_key: Optional[SyftVerifyKey]
     request_time: DateTime
     updated_at: Optional[DateTime]
     node_uid: UID
     request_hash: str
     changes: List[Change]
     history: List[ChangeStatus] = []
@@ -187,31 +189,55 @@
             str_change = f"{str_change}. "
             str_changes.append(str_change)
         str_changes = "\n".join(str_changes)
         api = APIRegistry.api_for(
             self.node_uid,
             self.syft_client_verify_key,
         )
+        shared_with_line = ""
+        if self.code and len(self.code.output_readers) > 0:
+            # owner_names = ["canada", "US"]
+            owners_string = " and ".join(
+                [f"<strong>{x}</strong>" for x in self.code.output_reader_names]
+            )
+            shared_with_line += (
+                f"<p><strong>Custom Policy: </strong> "
+                f"outputs are <strong>shared</strong> with the owners of {owners_string} once computed"
+            )
+
         metadata = api.services.metadata.get_metadata()
         admin_email = metadata.admin_email
         node_name = api.node_name.capitalize() if api.node_name is not None else ""
+
+        email_str = (
+            f"({self.requesting_user_email})" if self.requesting_user_email else ""
+        )
+        institution_str = (
+            f"<strong>Institution:</strong> {self.requesting_user_institution}"
+            if self.requesting_user_institution
+            else ""
+        )
+
         return f"""
             <style>
             .syft-request {{color: {SURFACE[options.color_theme]};}}
             </style>
             <div class='syft-request'>
                 <h3>Request</h3>
                 <p><strong>Id: </strong>{self.id}</p>
                 <p><strong>Request time: </strong>{self.request_time}</p>
                 {updated_at_line}
+                {shared_with_line}
                 <p><strong>Changes: </strong> {str_changes}</p>
                 <p><strong>Status: </strong>{self.status}</p>
                 <p><strong>Requested on: </strong> {node_name} of type <strong> \
                     {metadata.node_type.value.capitalize()}</strong> owned by {admin_email}</p>
+                <p><strong>Requested by:</strong> {self.requesting_user_name} {email_str} {institution_str}</p>
             </div>
+
             """
 
     def _coll_repr_(self):
         if self.status == RequestStatus.APPROVED:
             badge_color = "badge-green"
         elif self.status == RequestStatus.PENDING:
             badge_color = "badge-gray"
@@ -219,14 +245,17 @@
             badge_color = "badge-red"
 
         status_badge = {"value": self.status.name.capitalize(), "type": badge_color}
         return {
             "changes": " ".join([x.__repr_syft_nested__() for x in self.changes]),
             "request time": str(self.request_time),
             "status": status_badge,
+            "user_name": self.requesting_user_name,
+            "user_email": self.requesting_user_email,
+            "user_institution": self.requesting_user_institution,
             "requesting user": {
                 "value": str(self.requesting_user_verify_key),
                 "type": "clipboard",
             },
             "reviewed_at": str(self.updated_at),
         }
 
@@ -236,14 +265,17 @@
             if isinstance(change, UserCodeStatusChange):
                 return change.link
 
         return SyftError(
             message="This type of request does not have code associated with it."
         )
 
+    def get_results(self) -> Any:
+        return self.code.get_results()
+
     @property
     def current_change_state(self) -> Dict[UID, bool]:
         change_applied_map = {}
         for change_status in self.history:
             # only store the last change
             change_applied_map[change_status.change_id] = change_status.applied
 
@@ -506,33 +538,37 @@
             "requesting_user_verify_key"
         ] = context.obj.requesting_user_verify_key
     else:
         context.output["requesting_user_verify_key"] = context.credentials
     return context
 
 
-def add_requesting_user_name(context: TransformContext) -> TransformContext:
+def add_requesting_user_info(context: TransformContext) -> TransformContext:
     try:
         user_key = context.output["requesting_user_verify_key"]
         user_service = context.node.get_service("UserService")
         user = user_service.get_by_verify_key(user_key)
         context.output["requesting_user_name"] = user.name
+        context.output["requesting_user_email"] = user.email
+        context.output["requesting_user_institution"] = (
+            user.institution if user.institution else ""
+        )
     except Exception:
         context.output["requesting_user_name"] = "guest_user"
     return context
 
 
 @transform(SubmitRequest, Request)
 def submit_request_to_request() -> List[Callable]:
     return [
         generate_id,
         add_node_uid_for_key("node_uid"),
         add_request_time,
         check_requesting_user_verify_key,
-        add_requesting_user_name,
+        add_requesting_user_info,
         hash_changes,
     ]
 
 
 @serializable()
 class ObjectMutation(Change):
     __canonical_name__ = "ObjectMutation"
@@ -738,16 +774,19 @@
                 verify_key=context.node.signing_key.verify_key,
             )
         if not isinstance(res, SyftError):
             obj.status = res
             return obj
         return res
 
-    def is_enclave_request(self, req_enclave_metadata):
-        return req_enclave_metadata is not None and self.value == UserCodeStatus.EXECUTE
+    def is_enclave_request(self, user_code: UserCode):
+        return (
+            user_code.is_enclave_code is not None
+            and self.value == UserCodeStatus.APPROVED
+        )
 
     def _run(
         self, context: ChangeContext, apply: bool
     ) -> Result[SyftSuccess, SyftError]:
         try:
             valid = self.valid
             if not valid:
@@ -762,15 +801,15 @@
                 if isinstance(res, SyftError):
                     return Err(res.message)
 
                 # relative
                 from ..enclave.enclave_service import propagate_inputs_to_enclave
 
                 user_code = res
-                if self.is_enclave_request(user_code.enclave_metadata):
+                if self.is_enclave_request(user_code):
                     enclave_res = propagate_inputs_to_enclave(
                         user_code=res, context=context
                     )
                     if isinstance(enclave_res, SyftError):
                         return enclave_res
                 self.linked_obj.update_with_context(context, user_code)
             else:
```

### Comparing `syft-0.8.2b6/src/syft/service/request/request_service.py` & `syft-0.8.2b7/src/syft/service/request/request_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/request/request_stash.py` & `syft-0.8.2b7/src/syft/service/request/request_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/response.py` & `syft-0.8.2b7/src/syft/service/response.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,16 @@
     @property
     def _repr_html_class_(self) -> str:
         return "alert-success"
 
 
 @serializable()
 class SyftNotReady(SyftResponseMessage):
+    _bool: bool = False
+
     @property
     def _repr_html_class_(self) -> str:
         return "alert-info"
 
 
 @serializable()
 class SyftWarning(SyftResponseMessage):
```

### Comparing `syft-0.8.2b6/src/syft/service/service.py` & `syft-0.8.2b7/src/syft/service/service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/settings/settings.py` & `syft-0.8.2b7/src/syft/service/settings/settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/settings/settings_service.py` & `syft-0.8.2b7/src/syft/service/settings/settings_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/settings/settings_stash.py` & `syft-0.8.2b7/src/syft/service/settings/settings_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/user/user_roles.py` & `syft-0.8.2b7/src/syft/service/user/user_roles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/user/user_service.py` & `syft-0.8.2b7/src/syft/service/user/user_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,18 @@
     )
     def get_all(
         self,
         context: AuthedServiceContext,
         page_size: Optional[int] = 0,
         page_index: Optional[int] = 0,
     ) -> Union[Optional[UserViewPage], Optional[UserView], SyftError]:
-        result = self.stash.get_all(context.credentials)
+        if context.role in [ServiceRole.DATA_OWNER, ServiceRole.ADMIN]:
+            result = self.stash.get_all(context.credentials, has_permission=True)
+        else:
+            result = self.stash.get_all(context.credentials)
         if result.is_ok():
             results = [user.to(UserView) for user in result.ok()]
 
             # If chunk size is defined, then split list into evenly sized chunks
             if page_size:
                 total = len(results)
                 results = [
@@ -188,23 +191,27 @@
     #         if user:
     #             return user
     #     return SyftError(message=str(result.err()))
 
     @service_method(
         path="user.get_current_user", name="get_current_user", roles=GUEST_ROLE_LEVEL
     )
-    def get_current_user(self, context: AuthedServiceContext) -> UserView:
+    def get_current_user(
+        self, context: AuthedServiceContext
+    ) -> Union[UserView, SyftError]:
         result = self.stash.get_by_verify_key(
             credentials=context.credentials, verify_key=context.credentials
         )
         if result.is_ok():
             # this seems weird that we get back None as Ok(None)
             user = result.ok()
             if user:
-                return user
+                return user.to(UserView)
+            else:
+                SyftError(message="User not found!")
         return SyftError(message=str(result.err()))
 
     @service_method(path="user.update", name="update", roles=GUEST_ROLE_LEVEL)
     def update(
         self, context: AuthedServiceContext, uid: UID, user_update: UserUpdate
     ) -> Union[UserView, SyftError]:
         updates_role = user_update.role is not Empty
@@ -215,14 +222,24 @@
         ):
             return SyftError(message=f"{context.role} is not allowed to edit roles")
 
         # Get user to be updated by its UID
         result = self.stash.get_by_uid(credentials=context.credentials, uid=uid)
 
         # TODO: ADD Email Validation
+        # check if the email already exists
+        if user_update.email is not Empty:
+            user_with_email = self.stash.get_by_email(
+                credentials=context.credentials, email=user_update.email
+            )
+            if user_with_email.ok() is not None:
+                return SyftError(
+                    message=f"A user with the email {user_update.email} already exists."
+                )
+
         if result.is_err():
             error_msg = (
                 f"Failed to find user with UID: {uid}. Error: {str(result.err())}"
             )
             return SyftError(message=error_msg)
 
         user = result.ok()
@@ -431,15 +448,15 @@
         msg = SyftSuccess(message=success_message)
         return tuple([msg, user.to(UserPrivateKey)])
 
     def user_verify_key(self, email: str) -> Union[SyftVerifyKey, SyftError]:
         # we are bypassing permissions here, so dont use to return a result directly to the user
         credentials = self.admin_verify_key()
         result = self.stash.get_by_email(credentials=credentials, email=email)
-        if result.is_ok():
+        if result.ok() is not None:
             return result.ok().verify_key
         return SyftError(message=f"No user with email: {email}")
 
     def get_by_verify_key(
         self, verify_key: SyftVerifyKey
     ) -> Union[UserView, SyftError]:
         # we are bypassing permissions here, so dont use to return a result directly to the user
```

### Comparing `syft-0.8.2b6/src/syft/service/user/user_stash.py` & `syft-0.8.2b7/src/syft/service/user/user_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/vpn/headscale_client.py` & `syft-0.8.2b7/src/syft/service/vpn/headscale_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 @serializable()
 class HeadscaleAuthToken(SyftObject):
     __canonical_name__ = "HeadscaleAuthToken"
     __version__ = SYFT_OBJECT_VERSION_1
 
     id: Optional[UID]
-    namespace: str
+    user: str
     key: str
 
 
 class HeadscaleRoutes(VPNRoutes):
     GENERATE_KEY = "/commands/generate_key"
     LIST_NODES = "/commands/list_nodes"
 
@@ -60,11 +60,12 @@
 
         command_result = result.ok()
 
         if command_result.error:
             return SyftError(message=result.error)
 
         result = json.loads(command_result.report)
+        print("got result", result)
         return HeadscaleAuthToken(
             key=result["key"],
-            namespace=result["namespace"],
+            user=result["user"],
         )
```

### Comparing `syft-0.8.2b6/src/syft/service/vpn/tailscale_client.py` & `syft-0.8.2b7/src/syft/service/vpn/tailscale_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,18 +153,17 @@
 
         return TailscaleStatus(**status_info)
 
     def connect(
         self, headscale_host: str, headscale_auth_token: str
     ) -> Union[SyftSuccess, SyftError]:
         CONNECT_TIMEOUT = 60
-
         command_args = {
             "args": [
-                "-login-server",
+                "--login-server",
                 f"{headscale_host}",
                 "--reset",
                 "--force-reauth",
                 "--authkey",
                 f"{headscale_auth_token}",
                 "--accept-dns=false",
             ],
```

### Comparing `syft-0.8.2b6/src/syft/service/vpn/vpn.py` & `syft-0.8.2b7/src/syft/service/vpn/vpn.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/service/warnings.py` & `syft-0.8.2b7/src/syft/service/warnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/store/dict_document_store.py` & `syft-0.8.2b7/src/syft/store/dict_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/store/document_store.py` & `syft-0.8.2b7/src/syft/store/document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -445,17 +445,20 @@
         self, credentials: SyftVerifyKey, qk: QueryKey, has_permission=False
     ) -> Result[SyftSuccess, Err]:
         return self._thread_safe_cbk(
             self._delete, credentials, qk, has_permission=has_permission
         )
 
     def all(
-        self, credentials: SyftVerifyKey, order_by: Optional[PartitionKey] = None
+        self,
+        credentials: SyftVerifyKey,
+        order_by: Optional[PartitionKey] = None,
+        has_permission: Optional[bool] = False,
     ) -> Result[List[BaseStash.object_type], str]:
-        return self._thread_safe_cbk(self._all, credentials, order_by)
+        return self._thread_safe_cbk(self._all, credentials, order_by, has_permission)
 
     # Potentially thread-unsafe methods.
     # CAUTION:
     #       * Don't use self.lock here.
     #       * Do not call the public thread-safe methods here(with locking).
     # These methods are called from the public thread-safe API, and will hang the process.
     def _set(
@@ -529,17 +532,20 @@
         return (
             Ok(obj)
             if isinstance(obj, type_)
             else Err(f"{type(obj)} does not match required type: {type_}")
         )
 
     def get_all(
-        self, credentials: SyftVerifyKey, order_by: Optional[PartitionKey] = None
+        self,
+        credentials: SyftVerifyKey,
+        order_by: Optional[PartitionKey] = None,
+        has_permission: bool = False,
     ) -> Result[List[BaseStash.object_type], str]:
-        return self.partition.all(credentials, order_by)
+        return self.partition.all(credentials, order_by, has_permission)
 
     def __len__(self) -> int:
         return len(self.partition)
 
     def set(
         self,
         credentials: SyftVerifyKey,
@@ -669,14 +675,17 @@
 
     def get_by_uid(
         self, credentials: SyftVerifyKey, uid: UID
     ) -> Result[Optional[BaseUIDStoreStash.object_type], str]:
         qks = QueryKeys(qks=[UIDPartitionKey.with_obj(uid)])
         return self.query_one(credentials=credentials, qks=qks)
 
+    def add_permissions(self, permissions: List[ActionObjectPermission]) -> None:
+        self.partition.add_permissions(permissions)
+
     def set(
         self,
         credentials: SyftVerifyKey,
         obj: BaseUIDStoreStash.object_type,
         add_permissions: Optional[List[ActionObjectPermission]] = None,
         ignore_duplicates: bool = False,
     ) -> Result[BaseUIDStoreStash.object_type, str]:
```

### Comparing `syft-0.8.2b6/src/syft/store/kv_document_store.py` & `syft-0.8.2b7/src/syft/store/kv_document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,22 +139,27 @@
             return Err(str(e))
 
         return Ok()
 
     def __len__(self) -> int:
         return len(self.data)
 
-    def _get(self, uid: UID, credentials: SyftVerifyKey) -> Result[SyftObject, str]:
+    def _get(
+        self,
+        uid: UID,
+        credentials: SyftVerifyKey,
+        has_permission: Optional[bool] = False,
+    ) -> Result[SyftObject, str]:
         # relative
         from ..service.action.action_store import ActionObjectREAD
 
         # if you get something you need READ permission
         read_permission = ActionObjectREAD(uid=uid, credentials=credentials)
 
-        if self.has_permission(read_permission):
+        if self.has_permission(read_permission) or has_permission:
             syft_object = self.data[uid]
             return Ok(syft_object)
         return Err(f"Permission: {read_permission} denied")
 
     # Potentially thread-unsafe methods.
     # CAUTION:
     #       * Don't use self.lock here.
@@ -282,18 +287,21 @@
             pass
         elif permission.permission == ActionPermission.EXECUTE:
             pass
 
         return False
 
     def _all(
-        self, credentials: SyftVerifyKey, order_by: Optional[PartitionKey] = None
+        self,
+        credentials: SyftVerifyKey,
+        order_by: Optional[PartitionKey] = None,
+        has_permission: Optional[bool] = False,
     ) -> Result[List[BaseStash.object_type], str]:
         # this checks permissions
-        res = [self._get(uid, credentials) for uid in self.data.keys()]
+        res = [self._get(uid, credentials, has_permission) for uid in self.data.keys()]
         result = [x.ok() for x in res if x.is_ok()]
         if order_by is not None:
             result = sorted(result, key=lambda x: getattr(x, order_by.key, ""))
         return Ok(result)
 
     def _remove_keys(
         self,
```

### Comparing `syft-0.8.2b6/src/syft/store/linked_obj.py` & `syft-0.8.2b7/src/syft/store/linked_obj.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/store/locks.py` & `syft-0.8.2b7/src/syft/store/locks.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/store/mongo_client.py` & `syft-0.8.2b7/src/syft/store/mongo_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/store/mongo_codecs.py` & `syft-0.8.2b7/src/syft/store/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/store/mongo_document_store.py` & `syft-0.8.2b7/src/syft/store/mongo_document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,14 +296,15 @@
         )
 
     def _get_all_from_store(
         self,
         credentials: SyftVerifyKey,
         qks: QueryKeys,
         order_by: Optional[PartitionKey] = None,
+        has_permission: Optional[bool] = False,
     ) -> Result[List[SyftObject], str]:
         collection_status = self.collection
         if collection_status.is_err():
             return collection_status
         collection = collection_status.ok()
 
         if order_by is not None:
@@ -343,18 +344,26 @@
 
         return Err(f"Failed to delete object with qk: {qk}")
 
     def has_permission(self, permission: ActionObjectPermission) -> bool:
         # TODO: implement
         return True
 
-    def _all(self, credentials: SyftVerifyKey, order_by: Optional[PartitionKey] = None):
+    def _all(
+        self,
+        credentials: SyftVerifyKey,
+        order_by: Optional[PartitionKey] = None,
+        has_permission: Optional[bool] = False,
+    ):
         qks = QueryKeys(qks=())
         return self._get_all_from_store(
-            credentials=credentials, qks=qks, order_by=order_by
+            credentials=credentials,
+            qks=qks,
+            order_by=order_by,
+            has_permission=has_permission,
         )
 
     def __len__(self):
         collection_status = self.collection
         if collection_status.is_err():
             return 0
         collection = collection_status.ok()
```

### Comparing `syft-0.8.2b6/src/syft/store/sqlite_document_store.py` & `syft-0.8.2b7/src/syft/store/sqlite_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/types/datetime.py` & `syft-0.8.2b7/src/syft/types/datetime.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/types/grid_url.py` & `syft-0.8.2b7/src/syft/types/grid_url.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/types/syft_metaclass.py` & `syft-0.8.2b7/src/syft/types/syft_metaclass.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/types/syft_object.py` & `syft-0.8.2b7/src/syft/types/syft_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -461,29 +461,114 @@
 def short_uid(uid: UID) -> str:
     if uid is None:
         return uid
     else:
         return str(uid)[:6] + "..."
 
 
+def get_repr_values_table(_self, is_homogenous, extra_fields=None):
+    if extra_fields is None:
+        extra_fields = []
+
+    cols = defaultdict(list)
+    for item in iter(_self):
+        # unpack dict
+        if isinstance(_self, dict):
+            cols["key"].append(item)
+            item = _self.__getitem__(item)
+
+        # get id
+        id_ = getattr(item, "id", None)
+        if id_ is not None:
+            cols["id"].append({"value": str(id_), "type": "clipboard"})
+
+        if type(item) == type:
+            t = full_name_with_qualname(item)
+        else:
+            try:
+                t = item.__class__.__name__
+            except Exception:
+                t = item.__repr__()
+
+        if not is_homogenous:
+            cols["type"].append(t)
+
+        # if has _coll_repr_
+        if hasattr(item, "_coll_repr_"):
+            ret_val = item._coll_repr_()
+            if "id" in ret_val:
+                del ret_val["id"]
+            for key in ret_val.keys():
+                cols[key].append(ret_val[key])
+        else:
+            for field in extra_fields:
+                value = item
+                try:
+                    attrs = field.split(".")
+                    for i, attr in enumerate(attrs):
+                        # find indexing like abc[1]
+                        res = re.search("\[[+-]?\d+\]", attr)
+                        has_index = False
+                        if res:
+                            has_index = True
+                            index_str = res.group()
+                            index = int(index_str.replace("[", "").replace("]", ""))
+                            attr = attr.replace(index_str, "")
+
+                        value = getattr(value, attr, None)
+                        if isinstance(value, list) and has_index:
+                            value = value[index]
+                        # If the object has a special representation when nested we will use that instead
+                        if (
+                            hasattr(value, "__repr_syft_nested__")
+                            and i == len(attrs) - 1
+                        ):
+                            value = value.__repr_syft_nested__()
+                        if (
+                            isinstance(value, list)
+                            and i == len(attrs) - 1
+                            and len(value) > 0
+                            and hasattr(value[0], "__repr_syft_nested__")
+                        ):
+                            value = [
+                                x.__repr_syft_nested__()
+                                if hasattr(x, "__repr_syft_nested__")
+                                else x
+                                for x in value
+                            ]
+                    if value is None:
+                        value = "n/a"
+
+                except Exception as e:
+                    print(e)
+                    value = None
+                cols[field].append(str(value))
+
+    df = pd.DataFrame(cols)
+
+    if "created_at" in df.columns:
+        df.sort_values(by="created_at", ascending=False, inplace=True)
+
+    return df.to_dict("records")
+
+
 def list_dict_repr_html(self) -> str:
     try:
         max_check = 1
         items_checked = 0
         has_syft = False
         extra_fields = []
         if isinstance(self, dict):
             values = list(self.values())
         else:
             values = self
 
         if len(values) == 0:
             return self.__repr__()
 
-        is_homogenous = len(set([type(x) for x in values])) == 1
         for item in iter(self):
             items_checked += 1
             if items_checked > max_check:
                 break
             if isinstance(self, dict):
                 item = self.__getitem__(item)
 
@@ -494,110 +579,32 @@
             else:
                 mro = str(self)
 
             if "syft" in str(mro).lower():
                 has_syft = True
                 extra_fields = getattr(item, "__repr_attrs__", [])
                 break
+
         if has_syft:
+            # if custom_repr:
+            table_icon = None
+            if hasattr(values[0], "icon"):
+                table_icon = values[0].icon
+            # this is a list of dicts
+            is_homogenous = len(set([type(x) for x in values])) == 1
             # third party
             first_value = values[0]
             if is_homogenous:
                 cls_name = first_value.__class__.__name__
             else:
                 cls_name = ""
+            vals = get_repr_values_table(self, is_homogenous, extra_fields=extra_fields)
 
-            cols = defaultdict(list)
-            for item in iter(self):
-                # unpack dict
-                if isinstance(self, dict):
-                    cols["key"].append(item)
-                    item = self.__getitem__(item)
-
-                # get id
-                id_ = getattr(item, "id", None)
-                if id_ is not None:
-                    cols["id"].append({"value": str(id_), "type": "clipboard"})
-
-                if type(item) == type:
-                    t = full_name_with_qualname(item)
-                else:
-                    try:
-                        t = item.__class__.__name__
-                    except Exception:
-                        t = item.__repr__()
-
-                if not is_homogenous:
-                    cols["type"].append(t)
-
-                # if has _coll_repr_
-                if hasattr(item, "_coll_repr_"):
-                    ret_val = item._coll_repr_()
-                    if "id" in ret_val:
-                        del ret_val["id"]
-                    for key in ret_val.keys():
-                        cols[key].append(ret_val[key])
-                else:
-                    for field in extra_fields:
-                        value = item
-                        try:
-                            attrs = field.split(".")
-                            for i, attr in enumerate(attrs):
-                                # find indexing like abc[1]
-                                res = re.search("\[[+-]?\d+\]", attr)
-                                has_index = False
-                                if res:
-                                    has_index = True
-                                    index_str = res.group()
-                                    index = int(
-                                        index_str.replace("[", "").replace("]", "")
-                                    )
-                                    attr = attr.replace(index_str, "")
-
-                                value = getattr(value, attr, None)
-                                if isinstance(value, list) and has_index:
-                                    value = value[index]
-                                # If the object has a special representation when nested we will use that instead
-                                if (
-                                    hasattr(value, "__repr_syft_nested__")
-                                    and i == len(attrs) - 1
-                                ):
-                                    value = value.__repr_syft_nested__()
-                                if (
-                                    isinstance(value, list)
-                                    and i == len(attrs) - 1
-                                    and len(value) > 0
-                                    and hasattr(value[0], "__repr_syft_nested__")
-                                ):
-                                    value = [
-                                        x.__repr_syft_nested__()
-                                        if hasattr(x, "__repr_syft_nested__")
-                                        else x
-                                        for x in value
-                                    ]
-                            if value is None:
-                                value = "n/a"
-
-                        except Exception as e:
-                            print(e)
-                            value = None
-                        cols[field].append(str(value))
-
-            df = pd.DataFrame(cols)
-
-            if "created_at" in df.columns:
-                df.sort_values(by="created_at", ascending=False, inplace=True)
-
-            # if custom_repr:
-            table_icon = None
-            if hasattr(values[0], "icon"):
-                table_icon = values[0].icon
-            # this is a list of dicts
             return create_table_template(
-                df.to_dict("records"),
+                vals,
                 f"{cls_name} {self.__class__.__name__.capitalize()}",
                 table_icon=table_icon,
             )
 
     except Exception as e:
         print(f"error representing {type(self)} of objects. {e}")
         pass
```

### Comparing `syft-0.8.2b6/src/syft/types/transforms.py` & `syft-0.8.2b7/src/syft/types/transforms.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/types/twin_object.py` & `syft-0.8.2b7/src/syft/types/twin_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/types/uid.py` & `syft-0.8.2b7/src/syft/types/uid.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/util/autoreload.py` & `syft-0.8.2b7/src/syft/util/autoreload.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/util/decorators.py` & `syft-0.8.2b7/src/syft/util/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/util/experimental_flags.py` & `syft-0.8.2b7/src/syft/util/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/util/filterwarnings.py` & `syft-0.8.2b7/src/syft/util/filterwarnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/util/fonts.py` & `syft-0.8.2b7/src/syft/util/fonts.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/util/logger.py` & `syft-0.8.2b7/src/syft/util/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/util/markdown.py` & `syft-0.8.2b7/src/syft/util/markdown.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/util/notebook_ui/notebook_addons.py` & `syft-0.8.2b7/src/syft/util/notebook_ui/notebook_addons.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/util/schema.py` & `syft-0.8.2b7/src/syft/util/schema.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/util/telemetry.py` & `syft-0.8.2b7/src/syft/util/telemetry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/util/trace_decorator.py` & `syft-0.8.2b7/src/syft/util/trace_decorator.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/util/util.py` & `syft-0.8.2b7/src/syft/util/util.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft/util/version_compare.py` & `syft-0.8.2b7/src/syft/util/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b6/src/syft.egg-info/PKG-INFO` & `syft-0.8.2b7/src/syft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.2b6
+Version: 0.8.2b7
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.2b6 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.2b7 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: telemetry
```

### Comparing `syft-0.8.2b6/src/syft.egg-info/SOURCES.txt` & `syft-0.8.2b7/src/syft.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -84,21 +84,27 @@
 src/syft/service/action/action_service.py
 src/syft/service/action/action_store.py
 src/syft/service/action/action_types.py
 src/syft/service/action/numpy.py
 src/syft/service/action/pandas.py
 src/syft/service/action/plan.py
 src/syft/service/action/verification.py
+src/syft/service/blob_storage/__init__.py
+src/syft/service/blob_storage/service.py
+src/syft/service/blob_storage/stash.py
 src/syft/service/code/__init__.py
 src/syft/service/code/code_parse.py
 src/syft/service/code/unparse.py
 src/syft/service/code/user_code.py
 src/syft/service/code/user_code_parse.py
 src/syft/service/code/user_code_service.py
 src/syft/service/code/user_code_stash.py
+src/syft/service/code_history/code_history.py
+src/syft/service/code_history/code_history_service.py
+src/syft/service/code_history/code_history_stash.py
 src/syft/service/data_subject/__init__.py
 src/syft/service/data_subject/data_subject.py
 src/syft/service/data_subject/data_subject_member.py
 src/syft/service/data_subject/data_subject_member_service.py
 src/syft/service/data_subject/data_subject_service.py
 src/syft/service/dataset/__init__.py
 src/syft/service/dataset/dataset.py
@@ -148,18 +154,23 @@
 src/syft/store/kv_document_store.py
 src/syft/store/linked_obj.py
 src/syft/store/locks.py
 src/syft/store/mongo_client.py
 src/syft/store/mongo_codecs.py
 src/syft/store/mongo_document_store.py
 src/syft/store/sqlite_document_store.py
+src/syft/store/blob_storage/__init__.py
+src/syft/store/blob_storage/on_disk.py
+src/syft/store/blob_storage/seaweedfs.py
 src/syft/types/__init__.py
 src/syft/types/base.py
+src/syft/types/blob_storage.py
 src/syft/types/datetime.py
 src/syft/types/grid_url.py
+src/syft/types/identity.py
 src/syft/types/syft_metaclass.py
 src/syft/types/syft_object.py
 src/syft/types/transforms.py
 src/syft/types/twin_object.py
 src/syft/types/uid.py
 src/syft/util/__init__.py
 src/syft/util/autoreload.py
```

### Comparing `syft-0.8.2b6/src/syft.egg-info/requires.txt` & `syft-0.8.2b7/src/syft.egg-info/requires.txt`

 * *Files identical despite different names*

