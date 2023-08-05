# Comparing `tmp/summa_embed-0.17.7.tar.gz` & `tmp/summa_embed-0.17.8.tar.gz`

## Comparing `summa_embed-0.17.7.tar` & `summa_embed-0.17.8.tar`

### file list

```diff
@@ -1,125 +1,125 @@
--rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.17.7/local_dependencies/summa-proto/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-07-05 08:54:48.000000 summa_embed-0.17.7/local_dependencies/summa-proto/LICENSE
--rw-r--r--   0      501       20     2381 2023-07-05 08:54:48.000000 summa_embed-0.17.7/local_dependencies/summa-proto/build.rs
--rwxr-xr-x   0      501       20      244 2023-07-05 08:54:48.000000 summa_embed-0.17.7/local_dependencies/summa-proto/gen-docs.sh
--rw-r--r--   0      501       20     2561 2023-07-05 08:54:48.000000 summa_embed-0.17.7/local_dependencies/summa-proto/markdown.tmpl
--rw-r--r--   0      501       20        0 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/proto/__init__.py
--rw-r--r--   0      501       20     1556 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/proto/consumer_service.proto
--rw-r--r--   0      501       20      393 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/proto/dag_pb.proto
--rw-r--r--   0      501       20    10598 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/proto/index_service.proto
--rw-r--r--   0      501       20     7741 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/proto/query.proto
--rw-r--r--   0      501       20      499 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/proto/reflection_service.proto
--rw-r--r--   0      501       20      867 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/proto/search_service.proto
--rw-r--r--   0      501       20      407 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/proto/unixfs.proto
--rw-r--r--   0      501       20       96 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/proto/utils.proto
--rw-r--r--   0      501       20     2523 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/src/lib.rs
--rw-r--r--   0      501       20     2683 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/src/proto_traits/collector.rs
--rw-r--r--   0      501       20      212 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      394 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/src/proto_traits/query.rs
--rw-r--r--   0      501       20      613 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-proto/src/proto_traits/score.rs
--rw-r--r--   0        0        0     2113 1970-01-01 00:00:00.000000 summa_embed-0.17.7/local_dependencies/summa-core/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-07-05 08:54:45.000000 summa_embed-0.17.7/local_dependencies/summa-core/LICENSE
--rw-r--r--   0      501       20   370551 2023-07-05 08:54:45.000000 summa_embed-0.17.7/local_dependencies/summa-core/dictionaries/drugs.csv
--rw-r--r--   0      501       20       92 2023-07-05 08:54:45.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/collectors/mod.rs
--rw-r--r--   0      501       20     7233 2023-07-05 08:54:45.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
--rw-r--r--   0      501       20     2107 2023-07-05 08:54:45.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/custom_serializer.rs
--rw-r--r--   0      501       20     5492 2023-07-05 08:54:45.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/default_tokenizers.rs
--rw-r--r--   0      501       20    13820 2023-07-05 08:54:45.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/fruit_extractors.rs
--rw-r--r--   0      501       20    31266 2023-07-05 08:54:45.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/index_holder.rs
--rw-r--r--   0      501       20    13903 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/index_registry.rs
--rw-r--r--   0      501       20    20309 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/index_writer_holder.rs
--rw-r--r--   0      501       20     1694 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
--rw-r--r--   0      501       20      144 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/merge_policies/mod.rs
--rw-r--r--   0      501       20     2045 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
--rw-r--r--   0      501       20     5962 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/mod.rs
--rw-r--r--   0      501       20     6539 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/queries/exists_query.rs
--rw-r--r--   0      501       20       54 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/queries/mod.rs
--rw-r--r--   0      501       20      250 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/mod.rs
--rw-r--r--   0      501       20     1193 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs
--rw-r--r--   0      501       20      693 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs
--rw-r--r--   0      501       20     2092 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs
--rw-r--r--   0      501       20    13740 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
--rw-r--r--   0      501       20     1899 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
--rw-r--r--   0      501       20    63781 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
--rw-r--r--   0      501       20     5812 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs
--rw-r--r--   0      501       20     2498 2023-07-05 08:54:46.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/utils.rs
--rw-r--r--   0      501       20     2216 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/segment_attributes.rs
--rw-r--r--   0      501       20     1901 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/snippet_generator.rs
--rw-r--r--   0      501       20    11998 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/summa_document.rs
--rw-r--r--   0      501       20     7462 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/components/summa_tokenizer.rs
--rw-r--r--   0      501       20     2162 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/configs/config_proxy.rs
--rw-r--r--   0      501       20     4526 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/configs/core.rs
--rw-r--r--   0      501       20     3512 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/configs/file_proxy.rs
--rw-r--r--   0      501       20      383 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/configs/mod.rs
--rw-r--r--   0      501       20     3335 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/configs/partial_proxy.rs
--rw-r--r--   0      501       20     8009 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/directories/byte_range_cache.rs
--rw-r--r--   0      501       20     8015 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/directories/caching_directory.rs
--rw-r--r--   0      501       20     7015 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
--rw-r--r--   0      501       20     5258 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/directories/external_requests.rs
--rw-r--r--   0      501       20    17667 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
--rw-r--r--   0      501       20     2255 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/directories/mod.rs
--rw-r--r--   0      501       20     6756 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/directories/network_directory.rs
--rw-r--r--   0      501       20     5192 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/errors.rs
--rw-r--r--   0      501       20     2421 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/hyper_external_request.rs
--rw-r--r--   0      501       20      742 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/lib.rs
--rw-r--r--   0      501       20     1471 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/metrics/cache_metrics.rs
--rw-r--r--   0      501       20      960 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/metrics/label.rs
--rw-r--r--   0      501       20       92 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/metrics/mod.rs
--rw-r--r--   0      501       20      583 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/page_rank.rs
--rw-r--r--   0      501       20     5474 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/proto_traits/aggregation.rs
--rw-r--r--   0      501       20     2294 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/proto_traits/compression.rs
--rw-r--r--   0      501       20     1068 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
--rw-r--r--   0      501       20      323 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      662 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/proto_traits/order.rs
--rw-r--r--   0      501       20      582 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/proto_traits/snippet.rs
--rw-r--r--   0      501       20      411 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
--rw-r--r--   0      501       20     2048 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/scorers/eval_scorer.rs
--rw-r--r--   0      501       20     1538 2023-07-05 08:54:47.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
--rw-r--r--   0      501       20      826 2023-07-05 08:54:48.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
--rw-r--r--   0      501       20      218 2023-07-05 08:54:48.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/scorers/mod.rs
--rw-r--r--   0      501       20      480 2023-07-05 08:54:48.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
--rw-r--r--   0      501       20     7908 2023-07-05 08:54:48.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
--rw-r--r--   0      501       20      415 2023-07-05 08:54:48.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/utils/mod.rs
--rw-r--r--   0      501       20      309 2023-07-05 08:54:48.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/utils/random.rs
--rw-r--r--   0      501       20     3165 2023-07-05 08:54:48.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/utils/sync.rs
--rw-r--r--   0      501       20      559 2023-07-05 08:54:48.000000 summa_embed-0.17.7/local_dependencies/summa-core/src/validators.rs
--rw-r--r--   0        0        0     2767 1970-01-01 00:00:00.000000 summa_embed-0.17.7/local_dependencies/summa-server/Cargo.toml
--rw-r--r--   0      501       20       43 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-server/.cargo/config.toml
--rw-r--r--   0      501       20     1050 2023-07-05 08:54:49.000000 summa_embed-0.17.7/local_dependencies/summa-server/LICENSE
--rw-r--r--   0      501       20     2832 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/apis/consumer.rs
--rw-r--r--   0      501       20    13268 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/apis/index.rs
--rw-r--r--   0      501       20      105 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/apis/mod.rs
--rw-r--r--   0      501       20     2909 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/apis/reflection.rs
--rw-r--r--   0      501       20     1278 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/apis/search.rs
--rw-r--r--   0      501       20      783 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/bin/main.rs
--rw-r--r--   0      501       20     5305 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/components/consumer_manager.rs
--rw-r--r--   0      501       20      813 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs
--rw-r--r--   0      501       20     1082 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/components/consumers/dummy.rs
--rw-r--r--   0      501       20    11633 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs
--rw-r--r--   0      501       20      270 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/components/consumers/kafka/mod.rs
--rw-r--r--   0      501       20      532 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/components/consumers/kafka/status.rs
--rw-r--r--   0      501       20      155 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/components/consumers/mod.rs
--rw-r--r--   0      501       20     3811 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/components/index_meter.rs
--rw-r--r--   0      501       20      258 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/components/mod.rs
--rw-r--r--   0      501       20      943 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/configs/api.rs
--rw-r--r--   0      501       20      919 2023-07-05 08:54:50.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/configs/consumer.rs
--rw-r--r--   0      501       20      434 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/configs/metrics.rs
--rw-r--r--   0      501       20      116 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/configs/mod.rs
--rw-r--r--   0      501       20     4268 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/configs/server.rs
--rw-r--r--   0      501       20      991 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/configs/store.rs
--rw-r--r--   0      501       20     3459 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/errors.rs
--rw-r--r--   0      501       20     1427 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/lib.rs
--rw-r--r--   0      501       20     3681 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/logging.rs
--rw-r--r--   0      501       20    15704 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/server.rs
--rw-r--r--   0      501       20     8110 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/services/api.rs
--rw-r--r--   0      501       20    40154 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/services/index.rs
--rw-r--r--   0      501       20     5174 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/services/metrics.rs
--rw-r--r--   0      501       20      287 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/services/mod.rs
--rw-r--r--   0      501       20     2108 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/utils/mod.rs
--rw-r--r--   0      501       20      923 2023-07-05 08:54:51.000000 summa_embed-0.17.7/local_dependencies/summa-server/src/utils/thread_handler.rs
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 summa_embed-0.17.7/Cargo.toml
--rw-r--r--   0      501       20      685 2023-07-05 08:54:48.000000 summa_embed-0.17.7/.gitignore
--rw-r--r--   0      501       20      400 2023-07-05 08:54:48.000000 summa_embed-0.17.7/pyproject.toml
--rw-r--r--   0      501       20     2199 2023-07-05 08:54:48.000000 summa_embed-0.17.7/src/lib.rs
--rw-r--r--   0      501       20   101390 2023-07-05 08:55:23.000000 summa_embed-0.17.7/Cargo.lock
--rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.17.7/PKG-INFO
+-rw-r--r--   0        0        0     2113 1970-01-01 00:00:00.000000 summa_embed-0.17.8/local_dependencies/summa-core/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/LICENSE
+-rw-r--r--   0      501       20   370551 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/dictionaries/drugs.csv
+-rw-r--r--   0      501       20       92 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/collectors/mod.rs
+-rw-r--r--   0      501       20     7233 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
+-rw-r--r--   0      501       20     2107 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/custom_serializer.rs
+-rw-r--r--   0      501       20     5492 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/default_tokenizers.rs
+-rw-r--r--   0      501       20    13859 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/fruit_extractors.rs
+-rw-r--r--   0      501       20    31266 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/index_holder.rs
+-rw-r--r--   0      501       20    13903 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/index_registry.rs
+-rw-r--r--   0      501       20    20595 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/index_writer_holder.rs
+-rw-r--r--   0      501       20     1694 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
+-rw-r--r--   0      501       20      144 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/merge_policies/mod.rs
+-rw-r--r--   0      501       20     2045 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
+-rw-r--r--   0      501       20     5962 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/mod.rs
+-rw-r--r--   0      501       20     6539 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/queries/exists_query.rs
+-rw-r--r--   0      501       20       54 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/queries/mod.rs
+-rw-r--r--   0      501       20      250 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/query_parser/mod.rs
+-rw-r--r--   0      501       20     1193 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs
+-rw-r--r--   0      501       20      693 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs
+-rw-r--r--   0      501       20     2092 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs
+-rw-r--r--   0      501       20    13740 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
+-rw-r--r--   0      501       20     1899 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
+-rw-r--r--   0      501       20    63781 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
+-rw-r--r--   0      501       20     5812 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs
+-rw-r--r--   0      501       20     2498 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/query_parser/utils.rs
+-rw-r--r--   0      501       20     2216 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/segment_attributes.rs
+-rw-r--r--   0      501       20     1901 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/snippet_generator.rs
+-rw-r--r--   0      501       20    11998 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/summa_document.rs
+-rw-r--r--   0      501       20     7462 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/components/summa_tokenizer.rs
+-rw-r--r--   0      501       20     2162 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/configs/config_proxy.rs
+-rw-r--r--   0      501       20     4526 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/configs/core.rs
+-rw-r--r--   0      501       20     3512 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/configs/file_proxy.rs
+-rw-r--r--   0      501       20      383 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/configs/mod.rs
+-rw-r--r--   0      501       20     3335 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/configs/partial_proxy.rs
+-rw-r--r--   0      501       20     8009 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/directories/byte_range_cache.rs
+-rw-r--r--   0      501       20     8015 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/directories/caching_directory.rs
+-rw-r--r--   0      501       20     7015 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
+-rw-r--r--   0      501       20     5258 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/directories/external_requests.rs
+-rw-r--r--   0      501       20    17667 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
+-rw-r--r--   0      501       20     2255 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/directories/mod.rs
+-rw-r--r--   0      501       20     6756 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/directories/network_directory.rs
+-rw-r--r--   0      501       20     5192 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/errors.rs
+-rw-r--r--   0      501       20     2421 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/hyper_external_request.rs
+-rw-r--r--   0      501       20      742 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/lib.rs
+-rw-r--r--   0      501       20     1471 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/metrics/cache_metrics.rs
+-rw-r--r--   0      501       20      960 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/metrics/label.rs
+-rw-r--r--   0      501       20       92 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/metrics/mod.rs
+-rw-r--r--   0      501       20      583 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/page_rank.rs
+-rw-r--r--   0      501       20     5474 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/proto_traits/aggregation.rs
+-rw-r--r--   0      501       20     2294 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/proto_traits/compression.rs
+-rw-r--r--   0      501       20     1068 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
+-rw-r--r--   0      501       20      323 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      662 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/proto_traits/order.rs
+-rw-r--r--   0      501       20      582 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/proto_traits/snippet.rs
+-rw-r--r--   0      501       20      411 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
+-rw-r--r--   0      501       20     2048 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/scorers/eval_scorer.rs
+-rw-r--r--   0      501       20     1538 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
+-rw-r--r--   0      501       20      826 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
+-rw-r--r--   0      501       20      218 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/scorers/mod.rs
+-rw-r--r--   0      501       20      480 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
+-rw-r--r--   0      501       20     7908 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
+-rw-r--r--   0      501       20      415 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/utils/mod.rs
+-rw-r--r--   0      501       20      309 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/utils/random.rs
+-rw-r--r--   0      501       20     3165 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/utils/sync.rs
+-rw-r--r--   0      501       20      559 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-core/src/validators.rs
+-rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.17.8/local_dependencies/summa-proto/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-proto/LICENSE
+-rw-r--r--   0      501       20     2381 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-proto/build.rs
+-rwxr-xr-x   0      501       20      244 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-proto/gen-docs.sh
+-rw-r--r--   0      501       20     2561 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-proto/markdown.tmpl
+-rw-r--r--   0      501       20        0 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-proto/proto/__init__.py
+-rw-r--r--   0      501       20     1556 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-proto/proto/consumer_service.proto
+-rw-r--r--   0      501       20      393 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-proto/proto/dag_pb.proto
+-rw-r--r--   0      501       20    10598 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-proto/proto/index_service.proto
+-rw-r--r--   0      501       20     7741 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-proto/proto/query.proto
+-rw-r--r--   0      501       20      499 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-proto/proto/reflection_service.proto
+-rw-r--r--   0      501       20      867 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-proto/proto/search_service.proto
+-rw-r--r--   0      501       20      407 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-proto/proto/unixfs.proto
+-rw-r--r--   0      501       20       96 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-proto/proto/utils.proto
+-rw-r--r--   0      501       20     2523 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-proto/src/lib.rs
+-rw-r--r--   0      501       20     2683 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-proto/src/proto_traits/collector.rs
+-rw-r--r--   0      501       20      212 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-proto/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      394 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-proto/src/proto_traits/query.rs
+-rw-r--r--   0      501       20      613 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-proto/src/proto_traits/score.rs
+-rw-r--r--   0        0        0     2767 1970-01-01 00:00:00.000000 summa_embed-0.17.8/local_dependencies/summa-server/Cargo.toml
+-rw-r--r--   0      501       20       43 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/.cargo/config.toml
+-rw-r--r--   0      501       20     1050 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/LICENSE
+-rw-r--r--   0      501       20     2832 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/apis/consumer.rs
+-rw-r--r--   0      501       20    13268 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/apis/index.rs
+-rw-r--r--   0      501       20      105 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/apis/mod.rs
+-rw-r--r--   0      501       20     2909 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/apis/reflection.rs
+-rw-r--r--   0      501       20     1278 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/apis/search.rs
+-rw-r--r--   0      501       20      783 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/bin/main.rs
+-rw-r--r--   0      501       20     5305 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/components/consumer_manager.rs
+-rw-r--r--   0      501       20      813 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs
+-rw-r--r--   0      501       20     1082 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/components/consumers/dummy.rs
+-rw-r--r--   0      501       20    11633 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs
+-rw-r--r--   0      501       20      270 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/components/consumers/kafka/mod.rs
+-rw-r--r--   0      501       20      532 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/components/consumers/kafka/status.rs
+-rw-r--r--   0      501       20      155 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/components/consumers/mod.rs
+-rw-r--r--   0      501       20     3811 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/components/index_meter.rs
+-rw-r--r--   0      501       20      258 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/components/mod.rs
+-rw-r--r--   0      501       20      943 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/configs/api.rs
+-rw-r--r--   0      501       20      919 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/configs/consumer.rs
+-rw-r--r--   0      501       20      434 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/configs/metrics.rs
+-rw-r--r--   0      501       20      116 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/configs/mod.rs
+-rw-r--r--   0      501       20     4268 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/configs/server.rs
+-rw-r--r--   0      501       20      991 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/configs/store.rs
+-rw-r--r--   0      501       20     3459 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/errors.rs
+-rw-r--r--   0      501       20     1427 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/lib.rs
+-rw-r--r--   0      501       20     3681 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/logging.rs
+-rw-r--r--   0      501       20    15704 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/server.rs
+-rw-r--r--   0      501       20     8110 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/services/api.rs
+-rw-r--r--   0      501       20    40154 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/services/index.rs
+-rw-r--r--   0      501       20     5174 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/services/metrics.rs
+-rw-r--r--   0      501       20      287 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/services/mod.rs
+-rw-r--r--   0      501       20     2108 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/utils/mod.rs
+-rw-r--r--   0      501       20      923 2023-07-11 15:09:13.000000 summa_embed-0.17.8/local_dependencies/summa-server/src/utils/thread_handler.rs
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 summa_embed-0.17.8/Cargo.toml
+-rw-r--r--   0      501       20      685 2023-07-11 15:09:13.000000 summa_embed-0.17.8/.gitignore
+-rw-r--r--   0      501       20      400 2023-07-11 15:09:13.000000 summa_embed-0.17.8/pyproject.toml
+-rw-r--r--   0      501       20     2199 2023-07-11 15:09:13.000000 summa_embed-0.17.8/src/lib.rs
+-rw-r--r--   0      501       20   102369 2023-07-11 15:09:29.000000 summa_embed-0.17.8/Cargo.lock
+-rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.17.8/PKG-INFO
```

### Comparing `summa_embed-0.17.7/local_dependencies/summa-proto/Cargo.toml` & `summa_embed-0.17.8/local_dependencies/summa-proto/Cargo.toml`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-proto/LICENSE` & `summa_embed-0.17.8/local_dependencies/summa-core/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-proto/build.rs` & `summa_embed-0.17.8/local_dependencies/summa-proto/build.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-proto/markdown.tmpl` & `summa_embed-0.17.8/local_dependencies/summa-proto/markdown.tmpl`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-proto/proto/consumer_service.proto` & `summa_embed-0.17.8/local_dependencies/summa-proto/proto/consumer_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-proto/proto/index_service.proto` & `summa_embed-0.17.8/local_dependencies/summa-proto/proto/index_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-proto/proto/query.proto` & `summa_embed-0.17.8/local_dependencies/summa-proto/proto/query.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-proto/proto/search_service.proto` & `summa_embed-0.17.8/local_dependencies/summa-proto/proto/search_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-proto/src/lib.rs` & `summa_embed-0.17.8/local_dependencies/summa-proto/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-proto/src/proto_traits/collector.rs` & `summa_embed-0.17.8/local_dependencies/summa-proto/src/proto_traits/collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-proto/src/proto_traits/score.rs` & `summa_embed-0.17.8/local_dependencies/summa-proto/src/proto_traits/score.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/Cargo.toml` & `summa_embed-0.17.8/local_dependencies/summa-core/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-core"
-version = "0.17.7"
+version = "0.17.8"
 authors = ["Pasha Podolsky <ppodolsky@me.com>"]
 edition = "2021"
 license-file = "LICENSE"
 description = "Summa Core library"
 
 [lib]
 name = "summa_core"
```

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/LICENSE` & `summa_embed-0.17.8/local_dependencies/summa-proto/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/dictionaries/drugs.csv` & `summa_embed-0.17.8/local_dependencies/summa-core/dictionaries/drugs.csv`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/components/custom_serializer.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/components/custom_serializer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/components/default_tokenizers.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/components/default_tokenizers.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/components/fruit_extractors.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/components/fruit_extractors.rs`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 use rustc_hash::FxHashMap;
 use summa_proto::proto;
 use tantivy::aggregation::agg_result::AggregationResults;
 use tantivy::collector::{FacetCounts, FruitHandle, MultiCollector, MultiFruit};
 use tantivy::query::Query;
 use tantivy::schema::Field;
-use tantivy::Searcher;
+use tantivy::{Order, Searcher};
 
 use crate::components::snippet_generator::SnippetGeneratorConfig;
 use crate::components::IndexHolder;
 use crate::errors::{BuilderError, Error, SummaResult};
 use crate::proto_traits::Wrapper;
 use crate::scorers::eval_scorer_tweaker::EvalScorerTweaker;
 use crate::scorers::EvalScorer;
@@ -155,16 +155,16 @@
                     ) as Box<dyn FruitExtractor>
                 }
                 Some(proto::Scorer {
                     scorer: Some(proto::scorer::Scorer::OrderBy(field_name)),
                 }) => {
                     let top_docs_collector =
                         tantivy::collector::TopDocs::with_limit((top_docs_collector_proto.offset + top_docs_collector_proto.limit + 1) as usize)
-                            .order_by_u64_field(field_name);
-                    Box::new(
+                            .order_by_fast_field(field_name, Order::Desc);
+                    Box::<TopDocs<u64>>::new(
                         TopDocsBuilder::default()
                             .handle(multi_collector.add_collector(top_docs_collector))
                             .index_alias(index_alias.to_string())
                             .searcher(searcher)
                             .query(query.box_clone())
                             .limit(top_docs_collector_proto.limit)
                             .offset(top_docs_collector_proto.offset)
```

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/components/index_holder.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/components/index_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/components/index_registry.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/components/index_registry.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/components/index_writer_holder.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/components/index_writer_holder.rs`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,32 @@
                 _ => extract_flatten(v, &parts[i..], buffer),
             },
             None => break,
         }
     }
 }
 
+fn cast_to_term(unique_field: &Field, full_path: &str, value: &serde_json::Value) -> Vec<Term> {
+    let mut term = Term::with_capacity(128);
+    let mut json_term_writer = JsonTermWriter::from_field_and_json_path(*unique_field, full_path, true, &mut term);
+    match value {
+        serde_json::Value::Number(n) => {
+            vec![convert_to_fast_value_and_get_term(&mut json_term_writer, &n.to_string()).expect("incorrect json type")]
+        }
+        serde_json::Value::String(s) => {
+            let mut term = Term::with_capacity(128);
+            let mut json_term_writer = JsonTermWriter::from_field_and_json_path(*unique_field, full_path, true, &mut term);
+            json_term_writer.set_str(s);
+            vec![json_term_writer.term().clone()]
+        }
+        serde_json::Value::Array(v) => v.iter().flat_map(|e| cast_to_term(unique_field, full_path, e)).collect(),
+        _ => unreachable!(),
+    }
+}
+
 /// Wrap `tantivy::SingleSegmentIndexWriter` and allows to recreate it
 pub struct SingleIndexWriter {
     pub index_writer: RwLock<SingleSegmentIndexWriter>,
     pub index: Index,
     pub writer_heap_size_bytes: usize,
 }
 
@@ -255,45 +273,35 @@
 
     /// Delete index by its unique fields
     pub(super) fn resolve_conflicts(&self, document: &mut Document, conflict_strategy: proto::ConflictStrategy) -> SummaResult<Option<u64>> {
         if self.unique_fields.is_empty() || matches!(conflict_strategy, proto::ConflictStrategy::DoNothing) {
             return Ok(None);
         }
 
-        let unique_terms = self
+        let unique_terms: Vec<Term> = self
             .unique_fields
             .iter()
             .filter_map(|(unique_field, full_path)| {
                 document.get_first(*unique_field).and_then(|value| match value {
-                    Value::Str(s) => Some(Ok(Term::from_field_text(*unique_field, s))),
-                    Value::JsonObject(i) => i.get(full_path).map(|value| {
-                        let mut term = Term::with_capacity(128);
-                        let mut json_term_writer = JsonTermWriter::from_field_and_json_path(*unique_field, full_path, true, &mut term);
-                        match value {
-                            serde_json::Value::Number(n) => {
-                                Ok(convert_to_fast_value_and_get_term(&mut json_term_writer, &n.to_string()).expect("incorrect json type"))
-                            }
-                            serde_json::Value::String(s) => {
-                                json_term_writer.set_str(s);
-                                Ok(json_term_writer.term().clone())
-                            }
-                            _ => unreachable!(),
-                        }
-                    }),
-                    Value::I64(i) => Some(Ok(Term::from_field_i64(*unique_field, *i))),
-                    Value::U64(i) => Some(Ok(Term::from_field_u64(*unique_field, *i))),
-                    Value::F64(i) => Some(Ok(Term::from_field_f64(*unique_field, *i))),
+                    Value::Str(s) => Some(Ok(vec![Term::from_field_text(*unique_field, s)])),
+                    Value::JsonObject(i) => i.get(full_path).map(|value| Ok(cast_to_term(unique_field, full_path, value))),
+                    Value::I64(i) => Some(Ok(vec![Term::from_field_i64(*unique_field, *i)])),
+                    Value::U64(i) => Some(Ok(vec![Term::from_field_u64(*unique_field, *i)])),
+                    Value::F64(i) => Some(Ok(vec![Term::from_field_f64(*unique_field, *i)])),
                     _ => {
                         let schema = self.index_writer.index().schema();
                         let field_type = schema.get_field_entry(*unique_field).field_type();
                         Some(Err(Error::Validation(Box::new(ValidationError::InvalidUniqueFieldType(field_type.clone())))))
                     }
                 })
             })
-            .collect::<SummaResult<Vec<_>>>()?;
+            .collect::<SummaResult<Vec<_>>>()?
+            .into_iter()
+            .flatten()
+            .collect();
 
         if unique_terms.is_empty() {
             Err(ValidationError::MissingUniqueField(format!(
                 "{:?}",
                 self.index_writer.index().schema().to_named_doc(document)
             )))?
         }
```

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/components/mod.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/components/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/components/queries/exists_query.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/components/queries/exists_query.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest` & `summa_embed-0.17.8/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/components/query_parser/utils.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/components/query_parser/utils.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/components/segment_attributes.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/components/segment_attributes.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/components/snippet_generator.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/components/snippet_generator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/components/summa_document.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/components/summa_document.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/components/summa_tokenizer.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/components/summa_tokenizer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/configs/config_proxy.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/configs/config_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/configs/core.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/configs/core.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/configs/file_proxy.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/configs/file_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/configs/partial_proxy.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/configs/partial_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/directories/byte_range_cache.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/directories/byte_range_cache.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/directories/caching_directory.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/directories/caching_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/directories/external_requests.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/directories/external_requests.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/directories/hot_cache_directory.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/directories/hot_cache_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/directories/mod.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/directories/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/directories/network_directory.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/directories/network_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/errors.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/errors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/hyper_external_request.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/hyper_external_request.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/lib.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/metrics/cache_metrics.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/metrics/cache_metrics.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/metrics/label.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/metrics/label.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/page_rank.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/page_rank.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/proto_traits/aggregation.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/proto_traits/aggregation.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/proto_traits/compression.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/proto_traits/compression.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/proto_traits/merge_policy.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/proto_traits/merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/proto_traits/order.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/proto_traits/order.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/proto_traits/snippet.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/proto_traits/snippet.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/scorers/eval_scorer.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/scorers/eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/utils/sync.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/utils/sync.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-core/src/validators.rs` & `summa_embed-0.17.8/local_dependencies/summa-core/src/validators.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/Cargo.toml` & `summa_embed-0.17.8/local_dependencies/summa-server/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 edition = "2021"
 name = "summa-server"
-version = "0.17.7"
+version = "0.17.8"
 license-file = "LICENSE"
 description = "Fast full-text search server"
 homepage = "https://github.com/izihawa/summa"
 repository = "https://github.com/izihawa/summa"
 keywords = ["async", "search", "server", "grpc"]
 
 [lib]
@@ -51,15 +51,15 @@
 rand = { version = "0.8", features = ["small_rng"] }
 rdkafka = { version = "0.29", optional = true }
 rlimit = "0.9"
 serde = { version = "1.0", default_features = false, features = ["derive", "std"] }
 serde_derive = "1.0"
 serde_json = { version = "1.0" }
 serde_yaml = { version = "0.8" }
-summa-core = { version = "0.17.7", path = "../summa-core", features = ["fs", "hyper-external-request", "tokio-rt"] }
+summa-core = { version = "0.17.8", path = "../summa-core", features = ["fs", "hyper-external-request", "tokio-rt"] }
 summa-proto = { features = ["grpc"] , path = "../summa-proto" }
 take_mut = "0.2"
 tantivy = { git = "https://github.com/izihawa/tantivy", branch = "feature/summa", default_features = false, features = ["quickwit", "zstd-compression"] }
 tantivy-fst = "0.4.0"
 time = { version = "0.3", features = ["serde-well-known", "wasm-bindgen"] }
 thiserror = "1.0"
 tokio = { version = "1.25", default_features = false , features = ["full", "time"] }
```

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/LICENSE` & `summa_embed-0.17.8/local_dependencies/summa-server/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/src/apis/consumer.rs` & `summa_embed-0.17.8/local_dependencies/summa-server/src/apis/consumer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/src/apis/index.rs` & `summa_embed-0.17.8/local_dependencies/summa-server/src/apis/index.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/src/apis/reflection.rs` & `summa_embed-0.17.8/local_dependencies/summa-server/src/apis/reflection.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/src/apis/search.rs` & `summa_embed-0.17.8/local_dependencies/summa-server/src/apis/search.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/src/bin/main.rs` & `summa_embed-0.17.8/local_dependencies/summa-server/src/bin/main.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/src/components/consumer_manager.rs` & `summa_embed-0.17.8/local_dependencies/summa-server/src/components/consumer_manager.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs` & `summa_embed-0.17.8/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/src/components/consumers/dummy.rs` & `summa_embed-0.17.8/local_dependencies/summa-server/src/components/consumers/dummy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs` & `summa_embed-0.17.8/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/src/components/consumers/kafka/status.rs` & `summa_embed-0.17.8/local_dependencies/summa-server/src/components/consumers/kafka/status.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/src/components/index_meter.rs` & `summa_embed-0.17.8/local_dependencies/summa-server/src/components/index_meter.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/src/configs/api.rs` & `summa_embed-0.17.8/local_dependencies/summa-server/src/configs/api.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/src/configs/consumer.rs` & `summa_embed-0.17.8/local_dependencies/summa-server/src/configs/consumer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/src/configs/server.rs` & `summa_embed-0.17.8/local_dependencies/summa-server/src/configs/server.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/src/configs/store.rs` & `summa_embed-0.17.8/local_dependencies/summa-server/src/configs/store.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/src/errors.rs` & `summa_embed-0.17.8/local_dependencies/summa-server/src/errors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/src/lib.rs` & `summa_embed-0.17.8/local_dependencies/summa-server/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/src/logging.rs` & `summa_embed-0.17.8/local_dependencies/summa-server/src/logging.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/src/server.rs` & `summa_embed-0.17.8/local_dependencies/summa-server/src/server.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/src/services/api.rs` & `summa_embed-0.17.8/local_dependencies/summa-server/src/services/api.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/src/services/index.rs` & `summa_embed-0.17.8/local_dependencies/summa-server/src/services/index.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/src/services/metrics.rs` & `summa_embed-0.17.8/local_dependencies/summa-server/src/services/metrics.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/src/utils/mod.rs` & `summa_embed-0.17.8/local_dependencies/summa-server/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/local_dependencies/summa-server/src/utils/thread_handler.rs` & `summa_embed-0.17.8/local_dependencies/summa-server/src/utils/thread_handler.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/Cargo.toml` & `summa_embed-0.17.8/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-embed-py"
-version = "0.17.7"
+version = "0.17.8"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "summa_embed"
 crate-type = ["cdylib"]
 
@@ -13,12 +13,12 @@
 futures = "0.3"
 prost = "0.11"
 pyo3 = { version = "0.18", features = ["serde"] }
 pyo3-asyncio = { version =  "0.18", features = ["attributes", "tokio-runtime"] }
 pyo3-log = "0.8"
 pythonize = "0.18"
 serde_json = "1.0"
-summa-core = { version = "0.17.7", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
-summa-server = { version = "0.17.7", path = "local_dependencies/summa-server", default_features = false }
+summa-core = { version = "0.17.8", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
+summa-server = { version = "0.17.8", path = "local_dependencies/summa-server", default_features = false }
 summa-proto = { path = "local_dependencies/summa-proto" }
 tantivy = { git = "https://github.com/izihawa/tantivy", branch = "feature/summa", default_features = false, features = ["quickwit", "zstd-compression"] }
 tokio = { version = "1.25", default_features = false }
```

### Comparing `summa_embed-0.17.7/.gitignore` & `summa_embed-0.17.8/.gitignore`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/src/lib.rs` & `summa_embed-0.17.8/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.7/Cargo.lock` & `summa_embed-0.17.8/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -144,21 +144,21 @@
 dependencies = [
  "event-listener",
  "futures-core",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.70"
+version = "0.1.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "79fa67157abdfd688a259b6648808757db9347af834624f27ec646da976aee5d"
+checksum = "a564d521dd56509c4c47480d00b80ee55f7e385ae48db5744c67ad50c92d2ebf"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.23",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
@@ -287,39 +287,39 @@
 name = "blake2b_simd"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c2f0dc9a68c6317d884f97cc36cf5a3d20ba14ce404227df55e1af708ab04bc"
 dependencies = [
  "arrayref",
  "arrayvec",
- "constant_time_eq",
+ "constant_time_eq 0.2.6",
 ]
 
 [[package]]
 name = "blake2s_simd"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6637f448b9e61dfadbdcbae9a885fadee1f3eaffb1f8d3c1965d3ade8bdfd44f"
 dependencies = [
  "arrayref",
  "arrayvec",
- "constant_time_eq",
+ "constant_time_eq 0.2.6",
 ]
 
 [[package]]
 name = "blake3"
-version = "1.4.0"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "729b71f35bd3fa1a4c86b85d32c8b9069ea7fe14f7a53cfabb65f62d4265b888"
+checksum = "199c42ab6972d92c9f8995f086273d25c42fc0f7b2a1fcefba465c1352d25ba5"
 dependencies = [
  "arrayref",
  "arrayvec",
  "cc",
  "cfg-if",
- "constant_time_eq",
+ "constant_time_eq 0.3.0",
 ]
 
 [[package]]
 name = "block-buffer"
 version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
@@ -405,26 +405,26 @@
  "multihash 0.18.1",
  "serde",
  "unsigned-varint",
 ]
 
 [[package]]
 name = "clap"
-version = "4.3.10"
+version = "4.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "384e169cc618c613d5e3ca6404dda77a8685a63e08660dcc64abaf7da7cb0c7a"
+checksum = "1640e5cc7fb47dbb8338fd471b105e7ed6c3cb2aeb00c2e067127ffd3764a05d"
 dependencies = [
  "clap_builder",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.3.10"
+version = "4.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef137bbe35aab78bdb468ccfba75a5f4d8321ae011d34063770780545176af2d"
+checksum = "98c59138d527eeaf9b53f35a77fcc1fad9d883116070c63d5de1c7dc7b00c72b"
 dependencies = [
  "anstream",
  "anstyle",
  "clap_lex",
  "once_cell",
  "strsim",
 ]
@@ -482,14 +482,20 @@
 [[package]]
 name = "constant_time_eq"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "21a53c0a4d288377e7415b53dcfc3c04da5cdc2cc95c8d5ac178b58f0b861ad6"
 
 [[package]]
+name = "constant_time_eq"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f7144d30dcf0fafbce74250a3963025d8d52177934239851c917d29f1df280c2"
+
+[[package]]
 name = "core-foundation"
 version = "0.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "194a7a9e6de53fa55116934067c844d9d749312f75c6f6d0980e8c252f8c2146"
 dependencies = [
  "core-foundation-sys",
  "libc",
@@ -508,17 +514,17 @@
 checksum = "b49ba7ef1ad6107f8824dbe97de947cbaac53c44e7f9756a1fba0d37c1eec505"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03e69e28e9f7f77debdedbaafa2866e1de9ba56df55a8bd7cfc724c25a09987c"
+checksum = "a17b76ff3a4162b0b27f354a0c87015ddad39d35f9c0c36607a3bdd175dde1f1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
 version = "1.3.2"
@@ -620,20 +626,20 @@
  "darling_core",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "dashmap"
-version = "5.4.0"
+version = "5.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "907076dfda823b0b36d2a1bb5f90c96660a5bbcd7729e10727f07858f22c4edc"
+checksum = "6943ae99c34386c84a470c499d3414f66502a41340aa895406e0d2e4a207b91d"
 dependencies = [
  "cfg-if",
- "hashbrown 0.12.3",
+ "hashbrown 0.14.0",
  "lock_api",
  "once_cell",
  "parking_lot_core 0.9.8",
 ]
 
 [[package]]
 name = "data-encoding"
@@ -865,15 +871,15 @@
 
 [[package]]
 name = "fs4"
 version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2eeb4ed9e12f43b7fa0baae3f9cdda28352770132ef2e09a23760c29cae8bd47"
 dependencies = [
- "rustix 0.38.2",
+ "rustix 0.38.4",
  "windows-sys",
 ]
 
 [[package]]
 name = "fuchsia-cprng"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -937,15 +943,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.23",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -1065,14 +1071,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43a3c133739dddd0d2990f9a4bdf8eb4b21ef50e4851ca85ab661199821d510e"
 dependencies = [
  "ahash 0.8.3",
 ]
 
 [[package]]
+name = "hashbrown"
+version = "0.14.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c6201b9ff9fd90a5a3bac2e56a830d0caa509576f0e503818ee82c181b3437a"
+
+[[package]]
 name = "headers"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f3e372db8e5c0d213e0cd0b9be18be2aca3d44cf2fe30a9d46a65581cd454584"
 dependencies = [
  "base64 0.13.1",
  "bitflags 1.3.2",
@@ -1297,33 +1309,42 @@
  "ipfs-hamt-directory",
  "multihash 0.18.1",
  "pyo3",
 ]
 
 [[package]]
 name = "is-terminal"
-version = "0.4.8"
+version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24fddda5af7e54bf7da53067d6e802dbcc381d0a8eef629df528e3ebf68755cb"
+checksum = "cb0889898416213fab133e1d33a0e5858a48177452750691bde3666d0fdbaf8b"
 dependencies = [
  "hermit-abi",
- "rustix 0.38.2",
+ "rustix 0.38.4",
  "windows-sys",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
+name = "itertools"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
+dependencies = [
+ "either",
+]
+
+[[package]]
 name = "itoa"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62b02a5381cc465bd3041d84623d0fa3b66738b52b8e2fc3bab8ad63ab032f4a"
 
 [[package]]
 name = "izihawa-fst"
@@ -1557,15 +1578,15 @@
 
 [[package]]
 name = "matchers"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8263075bb86c5a1b1427b5ae862e8889656f126e9f77c484496e8b47cf5c5558"
 dependencies = [
- "regex-automata",
+ "regex-automata 0.1.10",
 ]
 
 [[package]]
 name = "matches"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2532096657941c2fea9c289d370a250971c689d4f143798ff67113ec042024a5"
@@ -1863,15 +1884,15 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.23",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
@@ -1972,15 +1993,15 @@
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
 [[package]]
 name = "ownedbytes"
 version = "0.5.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4d4561067efc6cb42ec29e7e8ede621a06f5a41f"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4daac326412187591624078ba942246798c889a7"
 dependencies = [
  "stable_deref_trait",
 ]
 
 [[package]]
 name = "parking_lot"
 version = "0.11.2"
@@ -2085,15 +2106,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b3e8cba4ec22bada7fc55ffe51e2deb6a0e0db2d0b7ab0b103acc80d2510c190"
 dependencies = [
  "pest",
  "pest_meta",
  "proc-macro2",
  "quote",
- "syn 2.0.23",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "pest_meta"
 version = "2.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a01f71cb40bd8bb94232df14b946909e14660e33fc05db3e50ae2a82d7ea0ca0"
@@ -2126,15 +2147,15 @@
 name = "pin-project-internal"
 version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec2e072ecce94ec471b13398d5402c188e76ac03cf74dd1a975161b23a3f6d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.23",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c40d25201921e5ff0c862a505c6557ea88568a4e3ace775ab55e93f2f4f9d57"
@@ -2210,17 +2231,17 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.63"
+version = "1.0.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
+checksum = "78803b62cbf1f46fde80d7c0e803111524b9877184cfe7c3033659490ac7a7da"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "prometheus"
 version = "0.13.3"
@@ -2250,15 +2271,15 @@
 name = "prost-build"
 version = "0.11.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "119533552c9a7ffacc21e099c24a0ac8bb19c2a2a3f363de84cd9b844feab270"
 dependencies = [
  "bytes",
  "heck",
- "itertools",
+ "itertools 0.10.5",
  "lazy_static",
  "log",
  "multimap",
  "petgraph",
  "prettyplease",
  "prost",
  "prost-types",
@@ -2271,15 +2292,15 @@
 [[package]]
 name = "prost-derive"
 version = "0.11.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5d2d8d10f3c6ded6da8b05b5fb3b8a5082514344d56c9f871412d29b4e075b4"
 dependencies = [
  "anyhow",
- "itertools",
+ "itertools 0.10.5",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "prost-types"
@@ -2612,43 +2633,55 @@
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.4"
+version = "1.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
+checksum = "b2eae68fc220f7cf2532e4494aded17545fce192d59cd996e0fe7887f4ceb575"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax 0.7.2",
+ "regex-automata 0.3.2",
+ "regex-syntax 0.7.4",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
 dependencies = [
  "regex-syntax 0.6.29",
 ]
 
 [[package]]
+name = "regex-automata"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "83d3daa6976cffb758ec878f108ba0e062a45b2d6ca3a2cca965338855476caf"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-syntax 0.7.4",
+]
+
+[[package]]
 name = "regex-syntax"
 version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.2"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
+checksum = "e5ea92a5b6195c6ef2a0295ea818b312502c6fc94dde986c5553242e18fd4ce2"
 
 [[package]]
 name = "remove_dir_all"
 version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3acd125665422973a33ac9d3dd2df85edad0f4ae9b00dafb1a05e43a9f5ef8e7"
 dependencies = [
@@ -2718,31 +2751,31 @@
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustix"
-version = "0.37.22"
+version = "0.37.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8818fa822adcc98b18fedbb3632a6a33213c070556b5aa7c4c8cc21cff565c4c"
+checksum = "4d69718bf81c6127a49dc64e44a742e8bb9213c0ff8869a22c308f84c1d4ab06"
 dependencies = [
  "bitflags 1.3.2",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys 0.3.8",
  "windows-sys",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.2"
+version = "0.38.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aabcb0461ebd01d6b79945797c27f8529082226cb630a9865a71870ff63532a4"
+checksum = "0a962918ea88d644592894bc6dc55acc6c0956488adcebbfb6e273506b7fd6e5"
 dependencies = [
  "bitflags 2.3.3",
  "errno",
  "libc",
  "linux-raw-sys 0.4.3",
  "windows-sys",
 ]
@@ -2801,17 +2834,17 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.166"
+version = "1.0.171"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d01b7404f9d441d3ad40e6a636a7782c377d2abdbe4fa2440e2edcc2f4f10db8"
+checksum = "30e27d1e4fd7659406c492fd6cfaf2066ba8773de45ca75e855590f856dc34a9"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-wasm-bindgen"
 version = "0.5.0"
@@ -2821,17 +2854,17 @@
  "js-sys",
  "serde",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "serde_bytes"
-version = "0.11.10"
+version = "0.11.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f3c5113243e4a3a1c96587342d067f3e6b0f50790b6cf40d2868eb647a3eef0e"
+checksum = "5a16be4fe5320ade08736447e3198294a5ea9a6d44dde6f35f0a5e06859c427a"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_cbor"
 version = "0.11.2"
@@ -2840,21 +2873,21 @@
 dependencies = [
  "half",
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.166"
+version = "1.0.171"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5dd83d6dde2b6b2d466e14d9d1acce8816dedee94f735eac6395808b3483c6d6"
+checksum = "389894603bd18c46fa56231694f8d827779c0951a667087194cf9de94ed24682"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.23",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.100"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0f1e14e89be7aa4c4b78bdbdc9eb5bf8517829a600ae8eaa39a6e1d960b5185c"
@@ -2958,17 +2991,17 @@
  "libc",
  "log",
  "parking_lot 0.11.2",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "socket2"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "64a4a911eed85daf18834cfaa86a79b7d266ff93ff5ba14005426219480ed662"
 dependencies = [
@@ -3002,30 +3035,30 @@
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "summa-core"
-version = "0.17.7"
+version = "0.17.8"
 dependencies = [
  "anyhow",
  "async-trait",
  "base64 0.21.2",
  "bytes",
  "chrono",
  "config",
  "derive_builder",
  "downcast-rs",
  "fasteval2",
  "futures",
  "hyper",
  "hyper-tls",
  "instant",
- "itertools",
+ "itertools 0.10.5",
  "lru",
  "matches",
  "oneshot",
  "opentelemetry",
  "parking_lot 0.12.1",
  "pest",
  "pest_derive",
@@ -3043,22 +3076,22 @@
  "strfmt",
  "summa-proto",
  "take_mut",
  "tantivy",
  "tantivy-common",
  "tantivy-query-grammar",
  "thiserror",
- "time 0.3.22",
+ "time 0.3.23",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "summa-embed-py"
-version = "0.17.7"
+version = "0.17.8"
 dependencies = [
  "async-broadcast",
  "futures",
  "prost",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-log",
@@ -3084,27 +3117,27 @@
  "tonic",
  "tonic-build",
  "tonic-reflection",
 ]
 
 [[package]]
 name = "summa-server"
-version = "0.17.7"
+version = "0.17.8"
 dependencies = [
  "anyhow",
  "async-broadcast",
  "async-trait",
  "clap",
  "config",
  "derive_builder",
  "futures",
  "futures-util",
  "headers",
  "hyper",
- "itertools",
+ "itertools 0.10.5",
  "libz-sys",
  "opentelemetry",
  "opentelemetry-prometheus",
  "path-absolutize",
  "prometheus",
  "prost",
  "prost-types",
@@ -3119,15 +3152,15 @@
  "summa-proto",
  "take_mut",
  "tantivy",
  "tantivy-fst",
  "tempdir",
  "thiserror",
  "tikv-jemallocator",
- "time 0.3.22",
+ "time 0.3.23",
  "tokio",
  "tokio-stream",
  "tokio-util",
  "tonic",
  "tonic-build",
  "tonic-reflection",
  "tonic-web",
@@ -3137,15 +3170,15 @@
  "tracing-appender",
  "tracing-futures",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "summa-wasm"
-version = "0.125.0"
+version = "0.125.2"
 dependencies = [
  "async-trait",
  "console_error_panic_hook",
  "futures",
  "getrandom",
  "instant",
  "js-sys",
@@ -3175,17 +3208,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.23"
+version = "2.0.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "59fb7d6d8281a51045d62b8eb3a7d1ce347b76f312af50cd3dc0af39c87c1737"
+checksum = "15e3fc8c0c74267e2df136e5e5fb656a464158aa57624053375eb9c8c6e25ae2"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -3211,15 +3244,15 @@
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f764005d11ee5f36500a149ace24e00e3da98b0158b3e2d53a7495660d3f4d60"
 
 [[package]]
 name = "tantivy"
 version = "0.20.2"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4d4561067efc6cb42ec29e7e8ede621a06f5a41f"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4daac326412187591624078ba942246798c889a7"
 dependencies = [
  "aho-corasick",
  "arc-swap",
  "async-trait",
  "base64 0.21.2",
  "bitpacking",
  "byteorder",
@@ -3228,15 +3261,15 @@
  "crossbeam-channel",
  "downcast-rs",
  "fastdivide",
  "fs4",
  "futures",
  "futures-util",
  "htmlescape",
- "itertools",
+ "itertools 0.11.0",
  "izihawa-fst",
  "levenshtein_automata",
  "lockfree-object-pool",
  "log",
  "lru",
  "measure_time",
  "memmap2",
@@ -3257,54 +3290,54 @@
  "tantivy-common",
  "tantivy-query-grammar",
  "tantivy-sstable",
  "tantivy-stacker",
  "tantivy-tokenizer-api",
  "tempfile",
  "thiserror",
- "time 0.3.22",
+ "time 0.3.23",
  "tokio",
  "uuid",
  "winapi",
  "zstd",
 ]
 
 [[package]]
 name = "tantivy-bitpacker"
 version = "0.4.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4d4561067efc6cb42ec29e7e8ede621a06f5a41f"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4daac326412187591624078ba942246798c889a7"
 dependencies = [
  "bitpacking",
 ]
 
 [[package]]
 name = "tantivy-columnar"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4d4561067efc6cb42ec29e7e8ede621a06f5a41f"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4daac326412187591624078ba942246798c889a7"
 dependencies = [
  "fastdivide",
  "fnv",
- "itertools",
+ "itertools 0.11.0",
  "serde",
  "tantivy-bitpacker",
  "tantivy-common",
  "tantivy-sstable",
  "tantivy-stacker",
 ]
 
 [[package]]
 name = "tantivy-common"
 version = "0.5.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4d4561067efc6cb42ec29e7e8ede621a06f5a41f"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4daac326412187591624078ba942246798c889a7"
 dependencies = [
  "async-trait",
  "byteorder",
  "ownedbytes",
  "serde",
- "time 0.3.22",
+ "time 0.3.23",
 ]
 
 [[package]]
 name = "tantivy-fst"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fc3c506b1a8443a3a65352df6382a1fb6a7afe1a02e871cee0d25e2c3d5f3944"
@@ -3313,59 +3346,59 @@
  "regex-syntax 0.6.29",
  "utf8-ranges",
 ]
 
 [[package]]
 name = "tantivy-query-grammar"
 version = "0.20.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4d4561067efc6cb42ec29e7e8ede621a06f5a41f"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4daac326412187591624078ba942246798c889a7"
 dependencies = [
  "combine",
  "once_cell",
  "regex",
 ]
 
 [[package]]
 name = "tantivy-sstable"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4d4561067efc6cb42ec29e7e8ede621a06f5a41f"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4daac326412187591624078ba942246798c889a7"
 dependencies = [
  "izihawa-fst",
  "tantivy-common",
  "zstd",
 ]
 
 [[package]]
 name = "tantivy-stacker"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4d4561067efc6cb42ec29e7e8ede621a06f5a41f"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4daac326412187591624078ba942246798c889a7"
 dependencies = [
  "murmurhash32",
  "tantivy-common",
 ]
 
 [[package]]
 name = "tantivy-tokenizer-api"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4d4561067efc6cb42ec29e7e8ede621a06f5a41f"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#4daac326412187591624078ba942246798c889a7"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "tap"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.8"
+version = "0.12.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b1c7f239eb94671427157bd93b3694320f3668d4e1eff08c7285366fd777fac"
+checksum = "df8e77cb757a61f51b947ec4a7e3646efd825b73561db1c232a8ccb639e611a0"
 
 [[package]]
 name = "tempdir"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "15f2b5fb00ccdf689e0149d1b1b3c03fead81c2b37735d812fa8bddbbf41b6d8"
 dependencies = [
@@ -3379,36 +3412,36 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "31c0432476357e58790aaa47a8efb0c5138f137343f3b5f23bd36a27e3b0a6d6"
 dependencies = [
  "autocfg",
  "cfg-if",
  "fastrand",
  "redox_syscall 0.3.5",
- "rustix 0.37.22",
+ "rustix 0.37.23",
  "windows-sys",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.41"
+version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c16a64ba9387ef3fdae4f9c1a7f07a0997fce91985c0336f1ddc1822b3b37802"
+checksum = "a35fc5b8971143ca348fa6df4f024d4d55264f3468c71ad1c2f365b0a4d58c42"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.41"
+version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d14928354b01c4d6a4f0e549069adef399a284e7995c7ccca94e8a07a5346c59"
+checksum = "463fe12d7993d3b327787537ce8dd4dfa058de32fc2b195ef3cde03dc4771e8f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.23",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
@@ -3446,17 +3479,17 @@
  "libc",
  "wasi 0.10.0+wasi-snapshot-preview1",
  "winapi",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.22"
+version = "0.3.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea9e1b3cf1243ae005d9e74085d4d542f3125458f3a81af210d901dcd7411efd"
+checksum = "59e399c068f43a5d116fedaf73b203fa4f9c519f17e2b34f63221d3792f81446"
 dependencies = [
  "itoa",
  "js-sys",
  "serde",
  "time-core",
  "time-macros",
 ]
@@ -3465,17 +3498,17 @@
 name = "time-core"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
 
 [[package]]
 name = "time-macros"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
+checksum = "96ba15a897f3c86766b757e5ac7221554c6750054d74d5b28844fce5fb36a6c4"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
 name = "tokio"
 version = "1.29.1"
@@ -3510,15 +3543,15 @@
 name = "tokio-macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.23",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
@@ -3704,27 +3737,27 @@
 [[package]]
 name = "tracing-appender"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "09d48f71a791638519505cefafe162606f706c25592e4bde4d97600c0195312e"
 dependencies = [
  "crossbeam-channel",
- "time 0.3.22",
+ "time 0.3.23",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "tracing-attributes"
 version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5f4f31f56159e98206da9efd823404b79b6ef3143b4a7ab76e67b1751b25a4ab"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.23",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
@@ -3806,17 +3839,17 @@
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "ucd-trie"
-version = "0.1.5"
+version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e79c4d996edb816c91e4308506774452e55e95c3c9de07b6729e17e15a5ef81"
+checksum = "ed646292ffc8188ef8ea4d1e0e0150fb15a5c2e12ad9b8fc191ae7a8a7f3c4b9"
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "22049a19f4a68748a168c0fc439f9516686aa045927ff767eca0a85101fb6e73"
 
@@ -3939,15 +3972,15 @@
 checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.23",
+ "syn 2.0.25",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -3973,15 +4006,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.23",
+ "syn 2.0.25",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.87"
```

