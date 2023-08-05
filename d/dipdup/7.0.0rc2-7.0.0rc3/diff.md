# Comparing `tmp/dipdup-7.0.0rc2.tar.gz` & `tmp/dipdup-7.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dipdup-7.0.0rc2.tar", last modified: Thu Jul 27 00:48:02 2023, max compression
+gzip compressed data, was "dipdup-7.0.0rc3.tar", last modified: Sat Aug  5 20:38:09 2023, max compression
```

## Comparing `dipdup-7.0.0rc2.tar` & `dipdup-7.0.0rc3.tar`

### file list

```diff
@@ -1,1112 +1,1112 @@
--rw-r--r--   0        0        0     1067 2023-07-27 00:38:52.701560 dipdup-7.0.0rc2/LICENSE
--rw-r--r--   0        0        0     3816 2023-07-27 00:38:52.701560 dipdup-7.0.0rc2/README.md
--rw-r--r--   0        0        0     4545 2023-07-27 00:48:02.674639 dipdup-7.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0      255 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/.gitignore
--rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_auction/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_auction/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1156 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/README.md
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      149 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      399 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      400 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/configs/replay.yaml
--rw-r--r--   0        0        0      356 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/deploy/.keep
--rw-r--r--   0        0        0      148 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/deploy/Dockerfile
--rw-r--r--   0        0        0      348 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2686 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1247 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/deploy/compose.yaml
--rw-r--r--   0        0        0      279 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/deploy/sqlite.env.default
--rw-r--r--   0        0        0      318 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/deploy/swarm.env.default
--rw-r--r--   0        0        0     1077 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/handlers/.keep
--rw-r--r--   0        0        0      913 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/handlers/on_bid.py
--rw-r--r--   0        0        0     1619 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/handlers/on_create_auction.py
--rw-r--r--   0        0        0      712 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/handlers/on_withdraw.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/models/.keep
--rw-r--r--   0        0        0     1445 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:40:55.859497 dipdup-7.0.0rc2/src/demo_auction/py.typed
--rw-r--r--   0        0        0     1047 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/types/.keep
--rw-r--r--   0        0        0      177 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/types/tzcolors_auction/tezos_parameters/bid.py
--rw-r--r--   0        0        0      381 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/types/tzcolors_auction/tezos_parameters/create_auction.py
--rw-r--r--   0        0        0      187 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/types/tzcolors_auction/tezos_parameters/withdraw.py
--rw-r--r--   0        0        0      555 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/types/tzcolors_auction/tezos_storage.py
--rw-r--r--   0        0        0      255 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/.gitignore
--rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_big_maps/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_big_maps/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1159 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/README.md
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      150 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      401 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      404 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/configs/replay.yaml
--rw-r--r--   0        0        0      356 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/deploy/.keep
--rw-r--r--   0        0        0      150 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/deploy/Dockerfile
--rw-r--r--   0        0        0      350 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2688 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1248 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/deploy/compose.yaml
--rw-r--r--   0        0        0      280 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/deploy/sqlite.env.default
--rw-r--r--   0        0        0      318 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/deploy/swarm.env.default
--rw-r--r--   0        0        0      725 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/handlers/.keep
--rw-r--r--   0        0        0      846 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/handlers/on_update_expiry_map.py
--rw-r--r--   0        0        0     1688 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/handlers/on_update_records.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/models/.keep
--rw-r--r--   0        0        0      667 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:41:26.379975 dipdup-7.0.0rc2/src/demo_big_maps/py.typed
--rw-r--r--   0        0        0     1051 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/types/.keep
--rw-r--r--   0        0        0      199 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/types/name_registry/tezos_big_maps/store_expiry_map_key.py
--rw-r--r--   0        0        0      203 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/types/name_registry/tezos_big_maps/store_expiry_map_value.py
--rw-r--r--   0        0        0      194 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/types/name_registry/tezos_big_maps/store_records_key.py
--rw-r--r--   0        0        0      489 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/types/name_registry/tezos_big_maps/store_records_value.py
--rw-r--r--   0        0        0      255 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/.gitignore
--rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_blank/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_blank/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1160 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/README.md
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      147 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      395 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      402 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/configs/replay.yaml
--rw-r--r--   0        0        0      327 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/deploy/.keep
--rw-r--r--   0        0        0      144 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/deploy/Dockerfile
--rw-r--r--   0        0        0      344 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2682 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1245 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/deploy/compose.yaml
--rw-r--r--   0        0        0      248 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/deploy/sqlite.env.default
--rw-r--r--   0        0        0      289 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/deploy/swarm.env.default
--rw-r--r--   0        0        0       37 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/handlers/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/models/.keep
--rw-r--r--   0        0        0     1242 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/models/__init__.py
--rw-r--r--   0        0        0     1049 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/types/.keep
--rw-r--r--   0        0        0      255 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/.gitignore
--rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_dao/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_dao/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1149 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/README.md
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      145 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      391 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      389 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/configs/replay.yaml
--rw-r--r--   0        0        0      356 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/deploy/.keep
--rw-r--r--   0        0        0      140 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/deploy/Dockerfile
--rw-r--r--   0        0        0      340 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2678 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1243 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/deploy/compose.yaml
--rw-r--r--   0        0        0      275 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/deploy/sqlite.env.default
--rw-r--r--   0        0        0      318 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/deploy/swarm.env.default
--rw-r--r--   0        0        0      643 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/handlers/.keep
--rw-r--r--   0        0        0      408 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/handlers/on_origination.py
--rw-r--r--   0        0        0      506 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/handlers/on_propose.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/models/.keep
--rw-r--r--   0        0        0      782 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:41:09.423710 dipdup-7.0.0rc2/src/demo_dao/py.typed
--rw-r--r--   0        0        0     1036 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/types/.keep
--rw-r--r--   0        0        0      360 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/types/registry/tezos_parameters/propose.py
--rw-r--r--   0        0        0     2523 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/types/registry/tezos_storage.py
--rw-r--r--   0        0        0      255 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dex/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dex/.gitignore
--rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_dex/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_dex/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1164 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dex/README.md
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dex/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      145 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      391 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      404 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/configs/replay.yaml
--rw-r--r--   0        0        0      327 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/deploy/.keep
--rw-r--r--   0        0        0      140 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/deploy/Dockerfile
--rw-r--r--   0        0        0      340 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2678 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1243 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/deploy/compose.yaml
--rw-r--r--   0        0        0      246 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/deploy/sqlite.env.default
--rw-r--r--   0        0        0      289 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/deploy/swarm.env.default
--rw-r--r--   0        0        0     4845 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/.keep
--rw-r--r--   0        0        0     1829 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_divest_liquidity.py
--rw-r--r--   0        0        0     1737 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_invest_liquidity.py
--rw-r--r--   0        0        0      579 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_origination.py
--rw-r--r--   0        0        0     1610 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_tez_to_token.py
--rw-r--r--   0        0        0     1676 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_token_to_tez.py
--rw-r--r--   0        0        0     1022 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_transfer.py
--rw-r--r--   0        0        0      962 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_withdraw_profit.py
--rw-r--r--   0        0        0     1855 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_divest_liquidity.py
--rw-r--r--   0        0        0     1763 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_invest_liquidity.py
--rw-r--r--   0        0        0      573 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_origination.py
--rw-r--r--   0        0        0     1604 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_tez_to_token.py
--rw-r--r--   0        0        0     1642 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_token_to_tez.py
--rw-r--r--   0        0        0     1143 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_transfer.py
--rw-r--r--   0        0        0      958 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_withdraw_profit.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/models/.keep
--rw-r--r--   0        0        0      916 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:40:45.219330 dipdup-7.0.0rc2/src/demo_dex/py.typed
--rw-r--r--   0        0        0     1051 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/.keep
--rw-r--r--   0        0        0      340 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/fa12_token/tezos_parameters/transfer.py
--rw-r--r--   0        0        0      739 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/fa12_token/tezos_storage.py
--rw-r--r--   0        0        0      504 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/fa2_token/tezos_parameters/transfer.py
--rw-r--r--   0        0        0     1093 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/fa2_token/tezos_storage.py
--rw-r--r--   0        0        0      311 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa12/tezos_parameters/divest_liquidity.py
--rw-r--r--   0        0        0      201 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa12/tezos_parameters/invest_liquidity.py
--rw-r--r--   0        0        0      297 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa12/tezos_parameters/tez_to_token_payment.py
--rw-r--r--   0        0        0      313 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa12/tezos_parameters/token_to_tez_payment.py
--rw-r--r--   0        0        0      340 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa12/tezos_parameters/transfer.py
--rw-r--r--   0        0        0      199 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa12/tezos_parameters/withdraw_profit.py
--rw-r--r--   0        0        0     1455 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa12/tezos_storage.py
--rw-r--r--   0        0        0      311 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa2/tezos_parameters/divest_liquidity.py
--rw-r--r--   0        0        0      201 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa2/tezos_parameters/invest_liquidity.py
--rw-r--r--   0        0        0      297 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa2/tezos_parameters/tez_to_token_payment.py
--rw-r--r--   0        0        0      313 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa2/tezos_parameters/token_to_tez_payment.py
--rw-r--r--   0        0        0      504 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa2/tezos_parameters/transfer.py
--rw-r--r--   0        0        0      199 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa2/tezos_parameters/withdraw_profit.py
--rw-r--r--   0        0        0     1491 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa2/tezos_storage.py
--rw-r--r--   0        0        0      255 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/.gitignore
--rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_domains/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_domains/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1158 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/README.md
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      149 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      399 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      402 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/configs/replay.yaml
--rw-r--r--   0        0        0      356 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/deploy/.keep
--rw-r--r--   0        0        0      148 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/deploy/Dockerfile
--rw-r--r--   0        0        0      348 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2686 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1247 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/deploy/compose.yaml
--rw-r--r--   0        0        0      279 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/deploy/sqlite.env.default
--rw-r--r--   0        0        0      318 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/deploy/swarm.env.default
--rw-r--r--   0        0        0      845 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/handlers/.keep
--rw-r--r--   0        0        0      553 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/handlers/on_admin_update.py
--rw-r--r--   0        0        0      525 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/handlers/on_execute.py
--rw-r--r--   0        0        0     1437 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/handlers/on_storage_diff.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/models/.keep
--rw-r--r--   0        0        0      630 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:40:33.047144 dipdup-7.0.0rc2/src/demo_domains/py.typed
--rw-r--r--   0        0        0     1049 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/types/.keep
--rw-r--r--   0        0        0      194 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/types/name_registry/tezos_parameters/admin_update.py
--rw-r--r--   0        0        0      305 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/types/name_registry/tezos_parameters/execute.py
--rw-r--r--   0        0        0     1134 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/types/name_registry/tezos_storage.py
--rw-r--r--   0        0        0      255 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/.gitignore
--rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_events/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_events/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1157 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/README.md
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      148 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      397 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      400 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/configs/replay.yaml
--rw-r--r--   0        0        0      327 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/deploy/.keep
--rw-r--r--   0        0        0      146 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/deploy/Dockerfile
--rw-r--r--   0        0        0      346 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2684 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1246 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/deploy/compose.yaml
--rw-r--r--   0        0        0      249 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/deploy/sqlite.env.default
--rw-r--r--   0        0        0      289 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/deploy/swarm.env.default
--rw-r--r--   0        0        0      536 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/handlers/.keep
--rw-r--r--   0        0        0      311 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/handlers/on_move_event.py
--rw-r--r--   0        0        0      237 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/handlers/on_other_event.py
--rw-r--r--   0        0        0      311 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/handlers/on_roll_event.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/models/.keep
--rw-r--r--   0        0        0     1242 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/models/__init__.py
--rw-r--r--   0        0        0     1047 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_events/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_events/types/.keep
--rw-r--r--   0        0        0      317 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_events/types/events_contract/tezos_events/move.py
--rw-r--r--   0        0        0      266 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_events/types/events_contract/tezos_events/roll.py
--rw-r--r--   0        0        0      255 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/.gitignore
--rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_evm_events/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_evm_events/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1174 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/README.md
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/abi/.keep
--rw-r--r--   0        0        0    11460 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/abi/eth_usdt/abi.json
--rw-r--r--   0        0        0     2420 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/abi/eth_usdt/events.json
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      152 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      405 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      421 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/configs/replay.yaml
--rw-r--r--   0        0        0      409 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/deploy/.keep
--rw-r--r--   0        0        0      154 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/deploy/Dockerfile
--rw-r--r--   0        0        0      354 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2692 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1250 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/deploy/compose.yaml
--rw-r--r--   0        0        0      335 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/deploy/sqlite.env.default
--rw-r--r--   0        0        0      371 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/deploy/swarm.env.default
--rw-r--r--   0        0        0      694 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/handlers/.keep
--rw-r--r--   0        0        0      992 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/handlers/on_transfer.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/models/.keep
--rw-r--r--   0        0        0      368 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/models/__init__.py
--rw-r--r--   0        0        0     1068 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/types/.keep
--rw-r--r--   0        0        0      331 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/types/eth_usdt/evm_events/transfer.py
--rw-r--r--   0        0        0      255 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/.gitignore
--rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_factories/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_factories/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1173 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/README.md
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      151 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      403 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      419 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/configs/replay.yaml
--rw-r--r--   0        0        0      356 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/deploy/.keep
--rw-r--r--   0        0        0      152 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/deploy/Dockerfile
--rw-r--r--   0        0        0      352 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2690 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1249 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/deploy/compose.yaml
--rw-r--r--   0        0        0      281 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/deploy/sqlite.env.default
--rw-r--r--   0        0        0      318 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/deploy/swarm.env.default
--rw-r--r--   0        0        0      647 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/handlers/.keep
--rw-r--r--   0        0        0      420 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/handlers/on_origination.py
--rw-r--r--   0        0        0      524 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/handlers/on_propose.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/models/.keep
--rw-r--r--   0        0        0      782 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:41:22.215910 dipdup-7.0.0rc2/src/demo_factories/py.typed
--rw-r--r--   0        0        0     1066 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/types/.keep
--rw-r--r--   0        0        0      360 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/types/registry/tezos_parameters/propose.py
--rw-r--r--   0        0        0     2523 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/types/registry/tezos_storage.py
--rw-r--r--   0        0        0      255 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/.gitignore
--rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_head/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_head/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1159 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/README.md
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      146 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      393 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      400 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/configs/replay.yaml
--rw-r--r--   0        0        0      356 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/deploy/.keep
--rw-r--r--   0        0        0      142 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/deploy/Dockerfile
--rw-r--r--   0        0        0      342 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2680 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1244 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/deploy/compose.yaml
--rw-r--r--   0        0        0      276 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/deploy/sqlite.env.default
--rw-r--r--   0        0        0      318 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/deploy/swarm.env.default
--rw-r--r--   0        0        0      240 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/handlers/.keep
--rw-r--r--   0        0        0      237 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/handlers/on_mainnet_head.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/models/.keep
--rw-r--r--   0        0        0     1242 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/models/__init__.py
--rw-r--r--   0        0        0     1047 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/types/.keep
--rw-r--r--   0        0        0      255 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/.gitignore
--rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_nft_marketplace/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_nft_marketplace/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1167 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/README.md
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      157 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      415 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      419 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/configs/replay.yaml
--rw-r--r--   0        0        0      452 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/deploy/.keep
--rw-r--r--   0        0        0      164 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/deploy/Dockerfile
--rw-r--r--   0        0        0      364 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2702 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1255 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/deploy/compose.yaml
--rw-r--r--   0        0        0      383 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/deploy/sqlite.env.default
--rw-r--r--   0        0        0      414 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/deploy/swarm.env.default
--rw-r--r--   0        0        0     1199 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/handlers/.keep
--rw-r--r--   0        0        0      605 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/handlers/on_cancel_swap.py
--rw-r--r--   0        0        0     1037 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/handlers/on_collect.py
--rw-r--r--   0        0        0      977 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/handlers/on_mint.py
--rw-r--r--   0        0        0      885 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/handlers/on_swap.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/models/.keep
--rw-r--r--   0        0        0     1306 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:40:43.251300 dipdup-7.0.0rc2/src/demo_nft_marketplace/py.typed
--rw-r--r--   0        0        0     1066 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/types/.keep
--rw-r--r--   0        0        0      192 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/cancel_swap.py
--rw-r--r--   0        0        0      281 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/collect.py
--rw-r--r--   0        0        0      317 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/mint_objkt.py
--rw-r--r--   0        0        0      299 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/swap.py
--rw-r--r--   0        0        0      777 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/types/hen_minter/tezos_storage.py
--rw-r--r--   0        0        0      343 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/types/hen_objkts/tezos_parameters/mint.py
--rw-r--r--   0        0        0     1094 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/types/hen_objkts/tezos_storage.py
--rw-r--r--   0        0        0      255 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/.gitignore
--rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_raw/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_raw/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1186 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/README.md
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      145 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      391 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      426 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/configs/replay.yaml
--rw-r--r--   0        0        0      356 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/deploy/.keep
--rw-r--r--   0        0        0      140 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/deploy/Dockerfile
--rw-r--r--   0        0        0      340 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2678 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1243 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/deploy/compose.yaml
--rw-r--r--   0        0        0      275 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/deploy/sqlite.env.default
--rw-r--r--   0        0        0      318 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/deploy/swarm.env.default
--rw-r--r--   0        0        0      411 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/handlers/.keep
--rw-r--r--   0        0        0      350 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/handlers/on_operation.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/models/.keep
--rw-r--r--   0        0        0      245 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:41:32.164065 dipdup-7.0.0rc2/src/demo_raw/py.typed
--rw-r--r--   0        0        0     1073 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/types/.keep
--rw-r--r--   0        0        0      255 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/.gitignore
--rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_token/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_token/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1158 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/README.md
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      147 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      395 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      400 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/configs/replay.yaml
--rw-r--r--   0        0        0      327 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/deploy/.keep
--rw-r--r--   0        0        0      144 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/deploy/Dockerfile
--rw-r--r--   0        0        0      344 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2682 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1245 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/deploy/compose.yaml
--rw-r--r--   0        0        0      248 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/deploy/sqlite.env.default
--rw-r--r--   0        0        0      289 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/deploy/swarm.env.default
--rw-r--r--   0        0        0      730 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/handlers/.keep
--rw-r--r--   0        0        0      436 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/handlers/on_balance_update.py
--rw-r--r--   0        0        0      630 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/handlers/on_mint.py
--rw-r--r--   0        0        0      928 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/handlers/on_transfer.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/models/.keep
--rw-r--r--   0        0        0      370 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:40:33.047144 dipdup-7.0.0rc2/src/demo_token/py.typed
--rw-r--r--   0        0        0     1047 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/types/.keep
--rw-r--r--   0        0        0      263 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/types/tzbtc/tezos_parameters/mint.py
--rw-r--r--   0        0        0      340 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/types/tzbtc/tezos_parameters/transfer.py
--rw-r--r--   0        0        0      398 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/types/tzbtc/tezos_storage.py
--rw-r--r--   0        0        0      255 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/.gitignore
--rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_token_transfers/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_token_transfers/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1167 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/README.md
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      157 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      415 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      419 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/configs/replay.yaml
--rw-r--r--   0        0        0      327 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/deploy/.keep
--rw-r--r--   0        0        0      164 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/deploy/Dockerfile
--rw-r--r--   0        0        0      364 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2702 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1255 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/deploy/compose.yaml
--rw-r--r--   0        0        0      258 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/deploy/sqlite.env.default
--rw-r--r--   0        0        0      289 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/deploy/swarm.env.default
--rw-r--r--   0        0        0      409 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/handlers/.keep
--rw-r--r--   0        0        0      545 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/handlers/on_balance_update.py
--rw-r--r--   0        0        0      836 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/handlers/on_token_transfer.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/models/.keep
--rw-r--r--   0        0        0      370 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:41:06.455664 dipdup-7.0.0rc2/src/demo_token_transfers/py.typed
--rw-r--r--   0        0        0     1066 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/types/.keep
--rw-r--r--   0        0        0      255 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_uniswap/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_uniswap/.gitignore
--rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_uniswap/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_uniswap/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1179 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_uniswap/README.md
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/abi/.keep
--rw-r--r--   0        0        0     4418 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/abi/factory/abi.json
--rw-r--r--   0        0        0      919 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/abi/factory/events.json
--rw-r--r--   0        0        0    19609 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/abi/pool/abi.json
--rw-r--r--   0        0        0     3559 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/abi/pool/events.json
--rw-r--r--   0        0        0    24313 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/abi/position_manager/abi.json
--rw-r--r--   0        0        0     1984 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/abi/position_manager/events.json
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      149 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      399 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      423 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/configs/replay.yaml
--rw-r--r--   0        0        0      424 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/deploy/.keep
--rw-r--r--   0        0        0      148 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/deploy/Dockerfile
--rw-r--r--   0        0        0      348 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2686 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1247 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/deploy/compose.yaml
--rw-r--r--   0        0        0      347 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/deploy/sqlite.env.default
--rw-r--r--   0        0        0      386 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/deploy/swarm.env.default
--rw-r--r--   0        0        0     2236 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/handlers/.keep
--rw-r--r--   0        0        0     3060 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/handlers/factory/pool_created.py
--rw-r--r--   0        0        0      531 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/handlers/pool/burn.py
--rw-r--r--   0        0        0      291 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/handlers/pool/flash.py
--rw-r--r--   0        0        0      871 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/handlers/pool/initialize.py
--rw-r--r--   0        0        0     1330 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/handlers/pool/mint.py
--rw-r--r--   0        0        0     6558 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/handlers/pool/swap.py
--rw-r--r--   0        0        0     1227 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/handlers/position_manager/collect.py
--rw-r--r--   0        0        0     1361 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/handlers/position_manager/decrease_liquidity.py
--rw-r--r--   0        0        0     1449 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/handlers/position_manager/increase_liquidity.py
--rw-r--r--   0        0        0     1172 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/handlers/position_manager/transfer.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/models/.keep
--rw-r--r--   0        0        0    19932 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/models/__init__.py
--rw-r--r--   0        0        0      373 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/models/abi.py
--rw-r--r--   0        0        0     4162 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/models/pool.py
--rw-r--r--   0        0        0     2824 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/models/position.py
--rw-r--r--   0        0        0     1477 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/models/repo.py
--rw-r--r--   0        0        0      561 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/models/tick.py
--rw-r--r--   0        0        0     7160 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/models/token.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/py.typed
--rw-r--r--   0        0        0     1070 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/types/.keep
--rw-r--r--   0        0        0      321 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/types/factory/evm_events/pool_created.py
--rw-r--r--   0        0        0      330 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/types/pool/evm_events/burn.py
--rw-r--r--   0        0        0      339 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/types/pool/evm_events/collect.py
--rw-r--r--   0        0        0      328 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/types/pool/evm_events/flash.py
--rw-r--r--   0        0        0      275 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/types/pool/evm_events/initialize.py
--rw-r--r--   0        0        0      346 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/types/pool/evm_events/mint.py
--rw-r--r--   0        0        0      351 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/types/pool/evm_events/swap.py
--rw-r--r--   0        0        0      303 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/types/position_manager/evm_events/collect.py
--rw-r--r--   0        0        0      323 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/types/position_manager/evm_events/decrease_liquidity.py
--rw-r--r--   0        0        0      323 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/types/position_manager/evm_events/increase_liquidity.py
--rw-r--r--   0        0        0      333 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/types/position_manager/evm_events/transfer.py
--rw-r--r--   0        0        0      213 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/__init__.py
--rw-r--r--   0        0        0      105 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/__main__.py
--rw-r--r--   0        0        0      512 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/api.py
--rw-r--r--   0        0        0    21805 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/cli.py
--rw-r--r--   0        0        0     7735 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/codegen/__init__.py
--rw-r--r--   0        0        0     7038 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/codegen/evm_subsquid.py
--rw-r--r--   0        0        0    18129 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/codegen/tezos_tzkt.py
--rw-r--r--   0        0        0    41898 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/config/__init__.py
--rw-r--r--   0        0        0      554 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/config/abi_etherscan.py
--rw-r--r--   0        0        0      690 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/config/coinbase.py
--rw-r--r--   0        0        0     1469 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/config/evm.py
--rw-r--r--   0        0        0     1273 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/config/evm_node.py
--rw-r--r--   0        0        0     1375 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/config/evm_subsquid.py
--rw-r--r--   0        0        0     2578 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/config/evm_subsquid_events.py
--rw-r--r--   0        0        0     1495 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/config/evm_subsquid_operations.py
--rw-r--r--   0        0        0      446 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/config/http.py
--rw-r--r--   0        0        0      519 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/config/ipfs.py
--rw-r--r--   0        0        0     1532 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/config/tezos.py
--rw-r--r--   0        0        0     2157 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/config/tezos_tzkt.py
--rw-r--r--   0        0        0     3758 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/config/tezos_tzkt_big_maps.py
--rw-r--r--   0        0        0     3074 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/config/tezos_tzkt_events.py
--rw-r--r--   0        0        0     1424 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/config/tezos_tzkt_head.py
--rw-r--r--   0        0        0    12744 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/config/tezos_tzkt_operations.py
--rw-r--r--   0        0        0     3110 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/config/tezos_tzkt_token_transfers.py
--rw-r--r--   0        0        0      745 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/config/tzip_metadata.py
--rw-r--r--   0        0        0    28058 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/context.py
--rw-r--r--   0        0        0    14211 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/database.py
--rw-r--r--   0        0        0     4474 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/datasources/__init__.py
--rw-r--r--   0        0        0      915 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/datasources/abi_etherscan.py
--rw-r--r--   0        0        0     2274 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/datasources/coinbase.py
--rw-r--r--   0        0        0    12321 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/datasources/evm_node.py
--rw-r--r--   0        0        0     4013 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/datasources/evm_subsquid.py
--rw-r--r--   0        0        0      399 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/datasources/http.py
--rw-r--r--   0        0        0      524 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/datasources/ipfs.py
--rw-r--r--   0        0        0    43369 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/datasources/tezos_tzkt.py
--rw-r--r--   0        0        0     1545 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/datasources/tzip_metadata.py
--rw-r--r--   0        0        0    30184 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/dipdup.py
--rw-r--r--   0        0        0     1803 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/env.py
--rw-r--r--   0        0        0     8274 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/exceptions.py
--rw-r--r--   0        0        0     3981 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/fetcher.py
--rw-r--r--   0        0        0     6724 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/fields.py
--rw-r--r--   0        0        0    25644 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/hasura.py
--rw-r--r--   0        0        0    11008 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/http.py
--rw-r--r--   0        0        0     7426 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/index.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/__init__.py
--rw-r--r--   0        0        0     1229 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/evm_subsquid_events/fetcher.py
--rw-r--r--   0        0        0    10389 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/evm_subsquid_events/index.py
--rw-r--r--   0        0        0     3439 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/evm_subsquid_events/matcher.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/evm_subsquid_events/parser.py
--rw-r--r--   0        0        0      406 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/evm_subsquid_operations/index.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_big_maps/__init__.py
--rw-r--r--   0        0        0     3181 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_big_maps/fetcher.py
--rw-r--r--   0        0        0     7320 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_big_maps/index.py
--rw-r--r--   0        0        0     2684 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_big_maps/matcher.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_events/__init__.py
--rw-r--r--   0        0        0     1480 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_events/fetcher.py
--rw-r--r--   0        0        0     5539 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_events/index.py
--rw-r--r--   0        0        0     3888 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_events/matcher.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_head/__init__.py
--rw-r--r--   0        0        0     2349 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_head/index.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_operations/__init__.py
--rw-r--r--   0        0        0    20276 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_operations/fetcher.py
--rw-r--r--   0        0        0    13485 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_operations/index.py
--rw-r--r--   0        0        0     9135 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_operations/matcher.py
--rw-r--r--   0        0        0     7612 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_operations/parser.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_token_transfers/__init__.py
--rw-r--r--   0        0        0     1432 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_token_transfers/fetcher.py
--rw-r--r--   0        0        0     5520 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_token_transfers/index.py
--rw-r--r--   0        0        0     1808 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_token_transfers/matcher.py
--rwxr-xr-x   0        0        0     9379 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/install.py
--rw-r--r--   0        0        0    20461 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/models/__init__.py
--rw-r--r--   0        0        0     1309 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/models/coinbase.py
--rw-r--r--   0        0        0     3596 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/models/evm_node.py
--rw-r--r--   0        0        0     5045 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/models/evm_subsquid.py
--rw-r--r--   0        0        0    19800 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/models/tezos_tzkt.py
--rw-r--r--   0        0        0      165 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/models/tzip_metadata.py
--rw-r--r--   0        0        0     7085 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/package.py
--rw-r--r--   0        0        0     7091 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/performance.py
--rw-r--r--   0        0        0     8379 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/project.py
--rw-r--r--   0        0        0      256 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/base/.dockerignore.j2
--rw-r--r--   0        0        0      341 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/base/.gitignore.j2
--rw-r--r--   0        0        0     1163 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/base/README.md.j2
--rw-r--r--   0        0        0      380 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/base/configs/dipdup.compose.yaml.j2
--rw-r--r--   0        0        0      159 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/base/configs/dipdup.sqlite.yaml.j2
--rw-r--r--   0        0        0      418 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/base/configs/dipdup.swarm.yaml.j2
--rw-r--r--   0        0        0      221 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/base/deploy/Dockerfile.j2
--rw-r--r--   0        0        0      367 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/base/deploy/compose.sqlite.yaml.j2
--rw-r--r--   0        0        0     2748 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/base/deploy/compose.swarm.yaml.j2
--rw-r--r--   0        0        0     1273 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/base/deploy/compose.yaml.j2
--rw-r--r--   0        0        0     1240 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/base/pyproject.toml.j2
--rw-r--r--   0        0        0     1087 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_auction/dipdup.yaml.j2
--rw-r--r--   0        0        0      935 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_auction/handlers/on_bid.py.j2
--rw-r--r--   0        0        0     1641 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_auction/handlers/on_create_auction.py.j2
--rw-r--r--   0        0        0      734 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_auction/handlers/on_withdraw.py.j2
--rw-r--r--   0        0        0     1448 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_auction/models/__init__.py.j2
--rw-r--r--   0        0        0      114 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_auction/replay.yaml
--rw-r--r--   0        0        0      734 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_big_maps/dipdup.yaml.j2
--rw-r--r--   0        0        0      865 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_big_maps/handlers/on_update_expiry_map.py.j2
--rw-r--r--   0        0        0     1707 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_big_maps/handlers/on_update_records.py.j2
--rw-r--r--   0        0        0      669 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_big_maps/models/__init__.py.j2
--rw-r--r--   0        0        0      118 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_big_maps/replay.yaml
--rw-r--r--   0        0        0       49 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_blank/dipdup.yaml.j2
--rw-r--r--   0        0        0      116 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_blank/replay.yaml
--rw-r--r--   0        0        0      657 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dao/dipdup.yaml.j2
--rw-r--r--   0        0        0      431 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dao/handlers/on_origination.py.j2
--rw-r--r--   0        0        0      540 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dao/handlers/on_propose.py.j2
--rw-r--r--   0        0        0      784 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dao/models/__init__.py.j2
--rw-r--r--   0        0        0      103 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dao/replay.yaml
--rw-r--r--   0        0        0     4859 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/dipdup.yaml.j2
--rw-r--r--   0        0        0     1885 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_divest_liquidity.py.j2
--rw-r--r--   0        0        0     1793 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_invest_liquidity.py.j2
--rw-r--r--   0        0        0      602 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_origination.py.j2
--rw-r--r--   0        0        0     1666 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_tez_to_token.py.j2
--rw-r--r--   0        0        0     1732 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_token_to_tez.py.j2
--rw-r--r--   0        0        0     1056 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_transfer.py.j2
--rw-r--r--   0        0        0      996 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_withdraw_profit.py.j2
--rw-r--r--   0        0        0     1911 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_divest_liquidity.py.j2
--rw-r--r--   0        0        0     1819 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_invest_liquidity.py.j2
--rw-r--r--   0        0        0      596 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_origination.py.j2
--rw-r--r--   0        0        0     1660 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_tez_to_token.py.j2
--rw-r--r--   0        0        0     1698 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_token_to_tez.py.j2
--rw-r--r--   0        0        0     1177 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_transfer.py.j2
--rw-r--r--   0        0        0      992 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_withdraw_profit.py.j2
--rw-r--r--   0        0        0      918 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/models/__init__.py.j2
--rw-r--r--   0        0        0      118 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/replay.yaml
--rw-r--r--   0        0        0      855 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_domains/dipdup.yaml.j2
--rw-r--r--   0        0        0      581 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_domains/handlers/on_admin_update.py.j2
--rw-r--r--   0        0        0      553 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_domains/handlers/on_execute.py.j2
--rw-r--r--   0        0        0     1456 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_domains/handlers/on_storage_diff.py.j2
--rw-r--r--   0        0        0      632 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_domains/models/__init__.py.j2
--rw-r--r--   0        0        0      116 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_domains/replay.yaml
--rw-r--r--   0        0        0      547 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_events/dipdup.yaml.j2
--rw-r--r--   0        0        0      114 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_events/replay.yaml
--rw-r--r--   0        0        0      701 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_evm_events/dipdup.yaml.j2
--rw-r--r--   0        0        0     1005 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_evm_events/handlers/on_transfer.py.j2
--rw-r--r--   0        0        0      370 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_evm_events/models/__init__.py.j2
--rw-r--r--   0        0        0      135 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_evm_events/replay.yaml
--rw-r--r--   0        0        0      655 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_factories/dipdup.yaml.j2
--rw-r--r--   0        0        0      431 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_factories/handlers/on_origination.py.j2
--rw-r--r--   0        0        0      540 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_factories/handlers/on_propose.py.j2
--rw-r--r--   0        0        0      784 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_factories/models/__init__.py.j2
--rw-r--r--   0        0        0      133 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_factories/replay.yaml
--rw-r--r--   0        0        0      253 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_head/dipdup.yaml.j2
--rw-r--r--   0        0        0      114 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_head/replay.yaml
--rw-r--r--   0        0        0     1201 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/dipdup.yaml.j2
--rw-r--r--   0        0        0      603 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/handlers/on_cancel_swap.py.j2
--rw-r--r--   0        0        0     1035 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/handlers/on_collect.py.j2
--rw-r--r--   0        0        0      973 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/handlers/on_mint.py.j2
--rw-r--r--   0        0        0      883 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/handlers/on_swap.py.j2
--rw-r--r--   0        0        0     1309 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/models/__init__.py.j2
--rw-r--r--   0        0        0      133 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/replay.yaml
--rw-r--r--   0        0        0      425 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_raw/dipdup.yaml.j2
--rw-r--r--   0        0        0      364 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_raw/handlers/on_operation.py.j2
--rw-r--r--   0        0        0      247 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_raw/models/__init__.py.j2
--rw-r--r--   0        0        0      140 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_raw/replay.yaml
--rw-r--r--   0        0        0      742 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_token/dipdup.yaml.j2
--rw-r--r--   0        0        0      448 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_token/handlers/on_balance_update.py.j2
--rw-r--r--   0        0        0      664 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_token/handlers/on_mint.py.j2
--rw-r--r--   0        0        0      962 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_token/handlers/on_transfer.py.j2
--rw-r--r--   0        0        0      372 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_token/models/__init__.py.j2
--rw-r--r--   0        0        0      114 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_token/replay.yaml
--rw-r--r--   0        0        0      411 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_token_transfers/dipdup.yaml.j2
--rw-r--r--   0        0        0      545 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_token_transfers/handlers/on_balance_update.py.j2
--rw-r--r--   0        0        0      836 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_token_transfers/handlers/on_token_transfer.py.j2
--rw-r--r--   0        0        0      372 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_token_transfers/models/__init__.py.j2
--rw-r--r--   0        0        0      133 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_token_transfers/replay.yaml
--rw-r--r--   0        0        0     2255 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/dipdup.yaml.j2
--rw-r--r--   0        0        0     3097 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/factory/pool_created.py.j2
--rw-r--r--   0        0        0      568 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/pool/burn.py.j2
--rw-r--r--   0        0        0      310 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/pool/flash.py.j2
--rw-r--r--   0        0        0      899 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/pool/initialize.py.j2
--rw-r--r--   0        0        0     1376 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/pool/mint.py.j2
--rw-r--r--   0        0        0     6631 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/pool/swap.py.j2
--rw-r--r--   0        0        0     1264 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/position_manager/collect.py.j2
--rw-r--r--   0        0        0     1398 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/position_manager/decrease_liquidity.py.j2
--rw-r--r--   0        0        0     1486 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/position_manager/increase_liquidity.py.j2
--rw-r--r--   0        0        0     1200 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/position_manager/transfer.py.j2
--rw-r--r--   0        0        0    19933 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/__init__.py.j2
--rw-r--r--   0        0        0      374 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/abi.py.j2
--rw-r--r--   0        0        0     4226 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/pool.py.j2
--rw-r--r--   0        0        0     2844 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/position.py.j2
--rw-r--r--   0        0        0     1478 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/repo.py.j2
--rw-r--r--   0        0        0      571 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/tick.py.j2
--rw-r--r--   0        0        0     7188 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/token.py.j2
--rw-r--r--   0        0        0      137 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/replay.yaml
--rw-r--r--   0        0        0     4008 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/prometheus.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/py.typed
--rw-r--r--   0        0        0     1631 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/pysignalr.py
--rw-r--r--   0        0        0     1722 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/report.py
--rw-r--r--   0        0        0     4867 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/scheduler.py
--rw-r--r--   0        0        0     4613 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/sentry.py
--rw-r--r--   0        0        0      199 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/sql/dipdup_head_status.sql
--rw-r--r--   0        0        0     2111 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/sql/truncate_schema.sql
--rw-r--r--   0        0        0     2163 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/subscriptions.py
--rw-r--r--   0        0        0     1791 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/sys.py
--rw-r--r--   0        0        0      227 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/templates/callback.py.j2
--rw-r--r--   0        0        0     1242 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/templates/models.py
--rw-r--r--   0        0        0      186 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/templates/replay.yaml.j2
--rw-r--r--   0        0        0     3290 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/transactions.py
--rw-r--r--   0        0        0     6763 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/utils.py
--rw-r--r--   0        0        0     5411 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/yaml.py
--rw-r--r--   0        0        0      952 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/__init__.py
--rw-r--r--   0        0        0      496 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/asdf.yml
--rw-r--r--   0        0        0     1222 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_auction.yml
--rw-r--r--   0        0        0      780 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_big_maps.yml
--rw-r--r--   0        0        0      745 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_dao.yml
--rw-r--r--   0        0        0     5012 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_dex.yml
--rw-r--r--   0        0        0      898 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_domains.yml
--rw-r--r--   0        0        0      878 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_factories.yml
--rw-r--r--   0        0        0     1316 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_nft_marketplace.yml
--rw-r--r--   0        0        0      590 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_raw.yml
--rw-r--r--   0        0        0      711 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_token.yml
--rw-r--r--   0        0        0      527 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_token_transfers.yml
--rw-r--r--   0        0        0      527 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_token_transfers_2.yml
--rw-r--r--   0        0        0      527 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_token_transfers_3.yml
--rw-r--r--   0        0        0      814 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_token_transfers_4.yml
--rw-r--r--   0        0        0     1252 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/dipdup.yml
--rw-r--r--   0        0        0      521 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/hen_subjkt.yml
--rw-r--r--   0        0        0      496 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/hjkl.yml
--rw-r--r--   0        0        0      546 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/kolibri_ovens.yml
--rw-r--r--   0        0        0      684 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/operation_filters.yml
--rw-r--r--   0        0        0      496 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/qwer.yml
--rw-r--r--   0        0        0      496 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/rewq.yml
--rw-r--r--   0        0        0       44 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/sqlite.yaml
--rw-r--r--   0        0        0      534 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/yupana.yml
--rw-r--r--   0        0        0      496 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/zxcv.yml
--rw-r--r--   0        0        0     1285 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/profile_abi_decoding.py
--rw-r--r--   0        0        0        2 2023-07-27 00:40:35.863186 dipdup-7.0.0rc2/tests/replays/024e925225593fe9cd80f5a114201f74d9f3631cea6f03add3e88fc91fafd2d7
--rw-r--r--   0        0        0    11605 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/replays/0535b2dcc93076e6026fa48cc501adaed47b7b060e6483d8312f40c184d7287d
--rw-r--r--   0        0        0  2577538 2023-07-27 00:38:52.757561 dipdup-7.0.0rc2/tests/replays/064e788d2566d748f516b17c6a43ab34259443cc9537f0dec7c1a5a2bce704b2
--rw-r--r--   0        0        0      305 2023-07-27 00:41:39.640181 dipdup-7.0.0rc2/tests/replays/0b7d26b8f2813d12a80b9e96cc6f0bb186bf9ac5c5b0c0b3bb2cc8d750126843
--rw-r--r--   0        0        0      784 2023-07-27 00:38:52.757561 dipdup-7.0.0rc2/tests/replays/0eaaba2830dbdd3a80286fbc367084bce6e55c678e21da178a7eb16beef6c997
--rw-r--r--   0        0        0       20 2023-07-27 00:38:52.757561 dipdup-7.0.0rc2/tests/replays/1165d42ccbdd0f6c25cece69d2c579da07655a30d04f18840350a153a98827a0
--rw-r--r--   0        0        0     7446 2023-07-27 00:38:52.757561 dipdup-7.0.0rc2/tests/replays/1228b36594bb93d619170ad49373f1ceec52d10faafdd727b37f3cdeffd663db
--rw-r--r--   0        0        0   108455 2023-07-27 00:41:29.028017 dipdup-7.0.0rc2/tests/replays/136157c421184c218127595797f5fe0b774e2807f6f4605a1d1944a1738e2d6d
--rw-r--r--   0        0        0     4947 2023-07-27 00:38:52.757561 dipdup-7.0.0rc2/tests/replays/13afdf001ce3d6a0219c0f7f6d372d9b645770e5f4304576f7f7a37b45af96fc
--rw-r--r--   0        0        0      310 2023-07-27 00:38:52.757561 dipdup-7.0.0rc2/tests/replays/1430e37dce64ecb83499da8feaa3c0906e4fdf5d0a3c3570174645e97ba54bc4
--rw-r--r--   0        0        0    13275 2023-07-27 00:38:52.757561 dipdup-7.0.0rc2/tests/replays/14408f393a3e399b241184f858e70396e3b8313e32ee1a984913d43fb74dcfec
--rw-r--r--   0        0        0   855628 2023-07-27 00:40:48.107376 dipdup-7.0.0rc2/tests/replays/14cba0424c66b1869edc8e18ca3079856083cc3db7e68ef61fce165b6d7e1a6d
--rw-r--r--   0        0        0      129 2023-07-27 00:38:52.757561 dipdup-7.0.0rc2/tests/replays/14d37c70764fe50b4ea590691d5614f613f96b8ad98c5df189564778616f5261
--rw-r--r--   0        0        0      246 2023-07-27 00:38:52.757561 dipdup-7.0.0rc2/tests/replays/185f6628ac43f6ca728c5b79b7b81a3c3671efce7f14030a06a27e90cf641dea
--rw-r--r--   0        0        0      986 2023-07-27 00:38:52.757561 dipdup-7.0.0rc2/tests/replays/18d85ceab66daf057861b99b7e223a25067197b3b77edbf060390df58cb65eaa
--rw-r--r--   0        0        0     1448 2023-07-27 00:38:52.757561 dipdup-7.0.0rc2/tests/replays/19441b677ef5fd8ca39c37e6ddd2a7d9bc8cb3ab282b2a91ce4d8430f56f0fa9
--rw-r--r--   0        0        0   612008 2023-07-27 00:38:52.761561 dipdup-7.0.0rc2/tests/replays/1a43bd7d1397cc3169ad267cd2ef083a5a63eaac7ed5186aadfc01bb53636214
--rw-r--r--   0        0        0  1154515 2023-07-27 00:40:48.659384 dipdup-7.0.0rc2/tests/replays/1c07d3d72acc637fb46c59d0a6dc9749f3412a5d527ca2eb0cccc01720fda1c7
--rw-r--r--   0        0        0    89590 2023-07-27 00:38:52.761561 dipdup-7.0.0rc2/tests/replays/1c34d1f810ae474395893bf67fb8cfb27b0506ab94eebec42cd4d2d21bf3dfcd
--rw-r--r--   0        0        0        2 2023-07-27 00:40:35.871187 dipdup-7.0.0rc2/tests/replays/1c717490846300e1639e96a0c1438b6dd2abd6de013c5edec49042fa364c06e6
--rw-r--r--   0        0        0    12263 2023-07-27 00:38:52.761561 dipdup-7.0.0rc2/tests/replays/252fd058cfef21f9b5b7f4367f730ec7d41647253d7cc7ccfb1e22d42d1f366a
--rw-r--r--   0        0        0     1167 2023-07-27 00:38:52.761561 dipdup-7.0.0rc2/tests/replays/27373c23411bf37b605c8d0ead9a0e6c6c1f1718ce7863b095b759811e44e155
--rw-r--r--   0        0        0     1121 2023-07-27 00:38:52.761561 dipdup-7.0.0rc2/tests/replays/2a45ec6372b45e46199a6af24272cb93586777a0522cd1203b3eeef213ce4583
--rw-r--r--   0        0        0   209761 2023-07-27 00:40:48.735386 dipdup-7.0.0rc2/tests/replays/31cc70e13495f58ecde80847bc6c9e08536cc426c03bd2aa8c45c1b2c798e155
--rw-r--r--   0        0        0 21118960 2023-07-27 00:38:52.805561 dipdup-7.0.0rc2/tests/replays/31dd376b771f347a0d6fe4dd132a1f96f809274429b78ec86dd742e5589fbc23
--rw-r--r--   0        0        0  1807578 2023-07-27 00:40:36.439195 dipdup-7.0.0rc2/tests/replays/32e3a13cc470d8720ce28f5eaff327340fb25cbe712e5b5a348af1bc3c92235a
--rw-r--r--   0        0        0       65 2023-07-27 00:38:52.805561 dipdup-7.0.0rc2/tests/replays/33349b63491dc976a7a2332d3cca3bd9b3b831c02a6f474bb925876c1838633a
--rw-r--r--   0        0        0        2 2023-07-27 00:38:52.805561 dipdup-7.0.0rc2/tests/replays/34f3e33d677f85b633cb85c6dd205beb40e3d9c40cfafc7084b82c8123a54de1
--rw-r--r--   0        0        0    45221 2023-07-27 00:38:52.805561 dipdup-7.0.0rc2/tests/replays/36072e13c9ce265bb81142b8816da8c31bd9180e7c663ea4169bd259af107382
--rw-r--r--   0        0        0    81885 2023-07-27 00:38:52.809561 dipdup-7.0.0rc2/tests/replays/377ac31d6316391ed138df44bec374d65202f0577603e80465ced3c09140f78c
--rw-r--r--   0        0        0    54602 2023-07-27 00:40:58.807544 dipdup-7.0.0rc2/tests/replays/383899084f79460e96fd311bb64e4925738c486b39d6281539456c5fcac41620
--rw-r--r--   0        0        0      642 2023-07-27 00:41:24.739950 dipdup-7.0.0rc2/tests/replays/39b8664d1bca5d374ff905c8a3a396b53d19ee469dc37545a8ca6b080bd0e9e0
--rw-r--r--   0        0        0     1200 2023-07-27 00:41:40.600196 dipdup-7.0.0rc2/tests/replays/3a2bd8b6b72bf18152d2550c106789fa9b8abc98ea9d759a6597b7ebfbab0fc2
--rw-r--r--   0        0        0    81885 2023-07-27 00:38:52.809561 dipdup-7.0.0rc2/tests/replays/3c9ad6f98f79e72185ea58c4777115750c658c5defd616664212095bd440c10c
--rw-r--r--   0        0        0      332 2023-07-27 00:38:52.809561 dipdup-7.0.0rc2/tests/replays/3fdba02cbc415eba224604f4fea130acd4565d31e4a83cdbb679ec0b76c798ab
--rw-r--r--   0        0        0  3369404 2023-07-27 00:41:12.907765 dipdup-7.0.0rc2/tests/replays/42b7bf0da866257ef98e1f7124d2d21fe7d13228c076fffa32331da423f36933
--rw-r--r--   0        0        0      619 2023-07-27 00:38:52.809561 dipdup-7.0.0rc2/tests/replays/43cb0ab415d8b8b3f7addc3e82ea27d93b2c66ff55c117e1e0c7c64a0fcfc3f2
--rw-r--r--   0        0        0   530743 2023-07-27 00:38:52.809561 dipdup-7.0.0rc2/tests/replays/440173d32e95111ca7b080ccc4dc09bfab23c8361919b2c113f0ff9ab445eec2
--rw-r--r--   0        0        0  1594116 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/489233ce9373f7de4f7a9053055c74bc0df999bfe939ed67d98b6d67e676e35a
--rw-r--r--   0        0        0   109726 2023-07-27 00:40:46.155345 dipdup-7.0.0rc2/tests/replays/4a57776d93475adfd9c49b6c3295a7cedfc23b73733a1fb5f0c985ee039dc5dc
--rw-r--r--   0        0        0      984 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/4aa7f9b0657be0c44baf2caed8c7cb08d02097a4095cf6417f78cba3a25e8423
--rw-r--r--   0        0        0       67 2023-07-27 00:41:37.552149 dipdup-7.0.0rc2/tests/replays/4fbdb4667971fab446a5ac5937a7c8cc6ef5813ff00af24b6fd1b1a0427bedbb
--rw-r--r--   0        0        0   192680 2023-07-27 00:40:46.003343 dipdup-7.0.0rc2/tests/replays/5483a0e11009e0f186bf70c214e2597d267a75a1e19152a9e7ed1ec257ce88ca
--rw-r--r--   0        0        0       65 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/56eb33fbb563bf03ea7639659fae5102222d6e3cea882febf71f01bd383c6eed
--rw-r--r--   0        0        0    40432 2023-07-27 00:40:58.671542 dipdup-7.0.0rc2/tests/replays/587613799ebfae42b1884016d1a44a452d68e70e3ed80641d90b8e7657ba8ee5
--rw-r--r--   0        0        0       32 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/5b004196490632859ec1b019d640f6bbb93fc86a433c8969e10f36f51ac2c78d
--rw-r--r--   0        0        0     1907 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/5b7c31b4b73bc57e8296e6051b3bc7b2302b32588d8fbcafce8a66de3be743df
--rw-r--r--   0        0        0     7609 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/5b99bc4beb6a9a33f7d2f118426458e4c788e0ab6d9e51949d3ccbf8b4003fc1
--rw-r--r--   0        0        0      939 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/5d21060ba8e78279d2d1edaa2f266ecf36105eaccef5ebed15748441651f76fd
--rw-r--r--   0        0        0      400 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/5f63ef9dd15459ae14e715bb79da8f033a24b54504212ebc873ee8aa95679606
--rw-r--r--   0        0        0       67 2023-07-27 00:41:37.680151 dipdup-7.0.0rc2/tests/replays/60f48c13c47a1347786a6dcf6f741874e7b30b587d148faa67d15067bb3871de
--rw-r--r--   0        0        0       21 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/62e95f1d55b756895289374b351a1da94505ec2d95a1652c97765f36a2ef9341
--rw-r--r--   0        0        0   211527 2023-07-27 00:40:49.571399 dipdup-7.0.0rc2/tests/replays/6cc8d741a41b76983cd7e0f63e8f22a4c67cd946888f45a5b7ead8c3bb5ad2f1
--rw-r--r--   0        0        0   944885 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/6cff8d120db8fd3926a45714ce7f1d0560803eb5a7b4a413b64fee1b7fd7a8ff
--rw-r--r--   0        0        0      132 2023-07-27 00:41:38.316161 dipdup-7.0.0rc2/tests/replays/6d0c5443d41a15551acb41adc10d36d4895f5786d6922a878b5c5414610e0ebc
--rw-r--r--   0        0        0      754 2023-07-27 00:41:39.140174 dipdup-7.0.0rc2/tests/replays/6d76a3c3f427ff534c551de1793cb1d1dfbd22ccad97f5917a9f9b201a3f9804
--rw-r--r--   0        0        0      494 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/7132f07560319399092782debe6eb28926e961d8af215ce11e2c0efd8dab06da
--rw-r--r--   0        0        0      451 2023-07-27 00:41:39.760183 dipdup-7.0.0rc2/tests/replays/739d17c86095aac3da3508a16dc1c9ae9459ea86eeb09f62aaefc32de2997918
--rw-r--r--   0        0        0        2 2023-07-27 00:41:43.268237 dipdup-7.0.0rc2/tests/replays/759b79ec12b1305d9fa8e1a5218e62bb3d3ad913580e19914d30d8aa09920ae4
--rw-r--r--   0        0        0   209456 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/7669ea717d9759748aed86302326b79be5157a1a36d13b39b00f06bcbe22b309
--rw-r--r--   0        0        0      520 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/76d49ae3b723376c88ca65a3080a273e098d226932a1a49c38fbc4421e7c2e64
--rw-r--r--   0        0        0    50588 2023-07-27 00:41:15.991813 dipdup-7.0.0rc2/tests/replays/7b6cf9b8c69712bf26ed09059352ec740606969bf20eab0dedda870273f4fde9
--rw-r--r--   0        0        0 21649088 2023-07-27 00:41:14.223785 dipdup-7.0.0rc2/tests/replays/7b9c78209f98b2c3a6678ed224fa686eee25c3c63dddd7f9af77c734b0dfabb8
--rw-r--r--   0        0        0      807 2023-07-27 00:41:41.524210 dipdup-7.0.0rc2/tests/replays/803e05a8d0bb9e7cfb49530271d43ea62111b6419e7cded2d221f7e0e0c92ece
--rw-r--r--   0        0        0   517204 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/80921fd33043def891912a6ad57d76664399564fd813950eb11f4a0e69e3e28f
--rw-r--r--   0        0        0      129 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/815c066c21f7d2697ef107cad4624a9c4079a7a1dab7974d606fc42b81fe93c8
--rw-r--r--   0        0        0      939 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/816d08f71c84537ea8df05a40678b1addca15bf3a73c0e927c75d9f9c0f2d418
--rw-r--r--   0        0        0      395 2023-07-27 00:41:41.240206 dipdup-7.0.0rc2/tests/replays/8335acc6585656ec3a4301cd8b089401f2dc2c7d758b381c96c730e610b67f7b
--rw-r--r--   0        0        0   207502 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/84cf46aa9c8dbd3ca6c3d946c749713e6c70a6a20d9cc69b4156235fd099b2e3
--rw-r--r--   0        0        0        2 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/8ad31f6cf9c873b1fd9827b621529c43966f8376a86fcac3b1d20c260b78007e
--rw-r--r--   0        0        0       65 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/91787fdbd1634f277b20ac46cb30eba9770f83df7189df0903e22f5f4bbe1efa
--rw-r--r--   0        0        0     1151 2023-07-27 00:41:42.036218 dipdup-7.0.0rc2/tests/replays/93516225810a23a6799f2f9a1dee055ca79a66ee2b8d0f32be820c9c385e936b
--rw-r--r--   0        0        0      494 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/9ce1bc12a2adeddcf9d8854c4b63a8e65b58d9206fb8d2e3eedb24c44ea7f28a
--rw-r--r--   0        0        0       22 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/9de859083ed1dd278893f60b5a60feab02a04637327a664af23f52dabb139fe6
--rw-r--r--   0        0        0      706 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/9e6e907842da2cd494c558ea5ecc211fd12e56bfc547450978fb7dfe03853e58
--rw-r--r--   0        0        0     6981 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/a3ce91a1b0d505cc221f0e201781466ba1e2d6dc7b624b9bc75a03ce3dbb0f92
--rw-r--r--   0        0        0    38974 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/a795ef429bde71b3ba66b545c0048f57a78ab5d2247772761d8efe86567199b9
--rw-r--r--   0        0        0        2 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/a840afa5674efd06639c4692a8bfe9ed6e1346bfe9c414209eec5d9126333242
--rw-r--r--   0        0        0      675 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/aa8fe6037996b296bf9a3011e45cd9ecb92fb728592a843f91b03b2848cb1fb1
--rw-r--r--   0        0        0     1882 2023-07-27 00:41:09.003704 dipdup-7.0.0rc2/tests/replays/acc952ba1905717315212f952ed689d7b8f683165b31c0a7a25199aed9fda27f
--rw-r--r--   0        0        0      356 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/aeee37b6f63a3177e0e27ac472008c3cba3d30ebee691fb45de1bae91a87f2ce
--rw-r--r--   0        0        0       67 2023-07-27 00:41:37.424147 dipdup-7.0.0rc2/tests/replays/af37212b31e932f269c42c7f34ad8f3849bd8aed244652c41b9327c508985ce5
--rw-r--r--   0        0        0     1200 2023-07-27 00:41:35.848123 dipdup-7.0.0rc2/tests/replays/b3af887f7ad8172af75b94a09bedfb9ae1e14f8819a36d6ce9f709721068263b
--rw-r--r--   0        0        0  1214926 2023-07-27 00:40:48.319379 dipdup-7.0.0rc2/tests/replays/b49fb33ee80345b70414ad08806a860e2139c20d98a5150c6ccd1b28a90f311e
--rw-r--r--   0        0        0     2271 2023-07-27 00:41:34.632104 dipdup-7.0.0rc2/tests/replays/bec4433b4206f00c2310a7961cff7f539434b9161b45673793aa5a3b50234313
--rw-r--r--   0        0        0      310 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/bed2329e63d559db2fb81c69606e715d1f90aaacab6ae45b33516e7828841a3c
--rw-r--r--   0        0        0       65 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/bf941ceae7a6e3c40406438e067f137131e6605924a93d43bafc77682b602c55
--rw-r--r--   0        0        0   759209 2023-07-27 00:40:48.435381 dipdup-7.0.0rc2/tests/replays/c0202a433296436c27458b3d5ec5c72d5e2d47ff77c939ce399780cc0f3e56bc
--rw-r--r--   0        0        0    19100 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/c369836c15d9ed15477002b850d5cbb96b1ff5ff33e917b812ab9c0905063957
--rw-r--r--   0        0        0   918908 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/c8e8698717ada415bc10405da983c8357165914dd0219f3d09bb9a939705242d
--rw-r--r--   0        0        0   691878 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/cc162df04c4990c79f7507dd915601fd4d58c947a248156cbe302a64adfe898a
--rw-r--r--   0        0        0     7446 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/cc5d3d4a58d5cb6bc7270d38c797b7740b79f913590ef0164abd50e58fba9405
--rw-r--r--   0        0        0      301 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/cc648800928fd43f8e72db1d41115c26a22346c9c7831172fe422c1765cd67f2
--rw-r--r--   0        0        0      960 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/d0a594d14bcb3fbf916092ec6707dfd3c9f48f53f0a1ad40a32023e7a87f8ef5
--rw-r--r--   0        0        0     2403 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/d62748a927a09395579b5790c8f871cc8653081cf4475abc93173989f950b92b
--rw-r--r--   0        0        0     9089 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/d94397f6ecec8ce25f87177fe410f6498d7d30a04360506c0cd300d291c167e7
--rw-r--r--   0        0        0      132 2023-07-27 00:41:36.764137 dipdup-7.0.0rc2/tests/replays/db797e6bf4c1b9c3237af5dec694fb1b6d21418a5a2f7947eb7f54d4e9201baf
--rw-r--r--   0        0        0   548925 2023-07-27 00:41:14.491790 dipdup-7.0.0rc2/tests/replays/dc86d5e346c85e6f7953d7e01298a9db64d778e5ba717ddd07fff8b589081e98
--rw-r--r--   0        0        0    20467 2023-07-27 00:40:36.003188 dipdup-7.0.0rc2/tests/replays/dca9cf4f9f27623f10975d369444899458ab9ea85c22af2da6ce6ce8c09c2b58
--rw-r--r--   0        0        0      700 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/df62701276d6dbf4860058cc582c0b4f7b583758f4f5be96c9ee045757c151e3
--rw-r--r--   0        0        0   151396 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/e39ebba701031aa13dfd9eb5dba1effd2938e96682d1030dcbd70172f9f190a9
--rw-r--r--   0        0        0     7917 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/e4a563a0b19379a44e9d2dc398131e9fd30d6039ff4ffacf1252db0bf8b433aa
--rw-r--r--   0        0        0       67 2023-07-27 00:41:37.804153 dipdup-7.0.0rc2/tests/replays/e82ba90c8570b92c0b1fc360b853aca3f1d7de457aacb9f6f19fa3e43879a8b3
--rw-r--r--   0        0        0      132 2023-07-27 00:41:36.912139 dipdup-7.0.0rc2/tests/replays/e9fa56a94eb559c550dfbca4b27ef350a0b4a787afbe60205482a38223dcea04
--rw-r--r--   0        0        0   713738 2023-07-27 00:41:35.700120 dipdup-7.0.0rc2/tests/replays/eb8b6b33cb2e165d1a3a73c09938d3083671a82ad73d4c0cff1fb2a5e5715f76
--rw-r--r--   0        0        0    11290 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/eb8e2c3ce2fe7792d2c8e81c61d37821275b64021343103b0c955042ae802189
--rw-r--r--   0        0        0      584 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/ece1ebe13f9391555230d6b94f33d66a922e2ca71ef5fd39bbd8c2c37ddf54ec
--rw-r--r--   0        0        0     1089 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/ed3ec9fd9226e9f765b96dc1d5d5a455a7b2505da530961826910b08db693070
--rw-r--r--   0        0        0    17245 2023-07-27 00:41:20.451883 dipdup-7.0.0rc2/tests/replays/f3d608f99e6b92e28a064bb9c10c3c605c9c817383c1eebcc68f663d1d23d650
--rw-r--r--   0        0        0    32513 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/f60e794a9be14263cb10e48546ba5610302cc3e7af0a114a593bb50eb85ba5e7
--rw-r--r--   0        0        0       21 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/fd9e33296006ad295c9fdc4868763f954a9c6d7c81d543ba198c14a72eea7e6b
--rw-r--r--   0        0        0      832 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/ff51b3535acc2972090ecd5db3af8f827464c9d92f1aa661630976e5b4ed4cbe
--rw-r--r--   0        0        0     4599 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/responses/asdf.json
--rw-r--r--   0        0        0     6704 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/responses/ftzfun.json
--rw-r--r--   0        0        0     3445 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/responses/hen_subjkt.json
--rw-r--r--   0        0        0     5210 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/responses/hjkl.json
--rw-r--r--   0        0        0     2097 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/responses/kolibri_ovens.json
--rw-r--r--   0        0        0    11186 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/responses/ooQuCAKBHkmWy2VciDAV9c6CFTywuMLupLzVoKDwS1xvR4EdRng.json
--rw-r--r--   0        0        0     1811 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/responses/origination_amount.json
--rw-r--r--   0        0        0     4256 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/responses/qwer.json
--rw-r--r--   0        0        0     5307 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/responses/rewq.json
--rw-r--r--   0        0        0    38178 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/responses/yupana.json
--rw-r--r--   0        0        0     5909 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/responses/zxcv.json
--rw-r--r--   0        0        0     1077 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/schemas/asdf/storage.json
--rw-r--r--   0        0        0     2116 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/schemas/hen_subjkt/storage.json
--rw-r--r--   0        0        0     1638 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/schemas/hjkl/storage.json
--rw-r--r--   0        0        0      800 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/schemas/kolibri_ovens/storage.json
--rw-r--r--   0        0        0     1005 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/schemas/qwer/storage.json
--rw-r--r--   0        0        0     2212 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/schemas/rewq/storage.json
--rw-r--r--   0        0        0    12561 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/schemas/yupana/storage.json
--rw-r--r--   0        0        0     2660 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/schemas/zxcv/storage.json
--rw-r--r--   0        0        0     3767 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_config/test_callbacks.py
--rw-r--r--   0        0        0     4643 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_config/test_config.py
--rw-r--r--   0        0        0     4138 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_config/test_custom_config.py
--rw-r--r--   0        0        0     2486 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_context.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_datasources/__init__.py
--rw-r--r--   0        0        0      814 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_datasources/test_ipfs.py
--rw-r--r--   0        0        0      663 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_datasources/test_metadata.py
--rw-r--r--   0        0        0     8304 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_datasources/test_tzkt.py
--rw-r--r--   0        0        0     1223 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_datasources/test_tzkt_blocks.py
--rw-r--r--   0        0        0     1971 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_datasources/test_tzkt_buffer.py
--rw-r--r--   0        0        0     1433 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_datasources/test_tzkt_quotes.py
--rw-r--r--   0        0        0     8700 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_demos.py
--rw-r--r--   0        0        0     2734 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_dipdup.py
--rw-r--r--   0        0        0     5045 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_hasura.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_http.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_index/__init__.py
--rw-r--r--   0        0        0     3714 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_index/test_operation.py
--rw-r--r--   0        0        0     5772 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_introspection.py
--rw-r--r--   0        0        0    14279 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_models.py
--rw-r--r--   0        0        0    13401 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_rollback.py
--rw-r--r--   0        0        0     2628 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_utils.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/asdf/__init__.py
--rw-r--r--   0        0        0      504 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/asdf/storage.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/bazaar/__init__.py
--rw-r--r--   0        0        0      564 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/bazaar/storage.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/ftzfun/__init__.py
--rw-r--r--   0        0        0      929 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/ftzfun/storage.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/hen_subjkt/__init__.py
--rw-r--r--   0        0        0      583 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/hen_subjkt/storage.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/hjkl/__init__.py
--rw-r--r--   0        0        0      647 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/hjkl/storage.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/kolibri_ovens/__init__.py
--rw-r--r--   0        0        0      232 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/kolibri_ovens/set_delegate.py
--rw-r--r--   0        0        0      392 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/kolibri_ovens/storage.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/listofmaps/__init__.py
--rw-r--r--   0        0        0      153 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/listofmaps/storage.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/qwer/__init__.py
--rw-r--r--   0        0        0      532 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/qwer/storage.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/rewq/__init__.py
--rw-r--r--   0        0        0      831 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/rewq/storage.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/tezotop/__init__.py
--rw-r--r--   0        0        0      740 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/tezotop/storage.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/yupana/__init__.py
--rw-r--r--   0        0        0     2721 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/yupana/storage.py
--rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/zxcv/__init__.py
--rw-r--r--   0        0        0     1048 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/zxcv/storage.py
--rw-r--r--   0        0        0     5756 1970-01-01 00:00:00.000000 dipdup-7.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-05 20:28:16.554345 dipdup-7.0.0rc3/LICENSE
+-rw-r--r--   0        0        0     3816 2023-08-05 20:28:16.554345 dipdup-7.0.0rc3/README.md
+-rw-r--r--   0        0        0     4545 2023-08-05 20:38:09.611123 dipdup-7.0.0rc3/pyproject.toml
+-rw-r--r--   0        0        0      269 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/.dockerignore
+-rw-r--r--   0        0        0      355 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/.gitignore
+-rw-r--r--   0        0        0        1 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_auction/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_auction/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1159 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/README.md
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/abi/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/configs/.keep
+-rw-r--r--   0        0        0      379 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      149 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      399 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      400 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/configs/replay.yaml
+-rw-r--r--   0        0        0      356 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/deploy/.keep
+-rw-r--r--   0        0        0      148 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/deploy/Dockerfile
+-rw-r--r--   0        0        0      348 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2686 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1247 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/deploy/compose.yaml
+-rw-r--r--   0        0        0      279 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      318 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/deploy/swarm.env.default
+-rw-r--r--   0        0        0     1077 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/handlers/.keep
+-rw-r--r--   0        0        0      913 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/handlers/on_bid.py
+-rw-r--r--   0        0        0     1619 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/handlers/on_create_auction.py
+-rw-r--r--   0        0        0      712 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/handlers/on_withdraw.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/models/.keep
+-rw-r--r--   0        0        0     1445 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:30:55.310514 dipdup-7.0.0rc3/src/demo_auction/py.typed
+-rw-r--r--   0        0        0     1047 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/sql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/types/.keep
+-rw-r--r--   0        0        0      177 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/types/tzcolors_auction/tezos_parameters/bid.py
+-rw-r--r--   0        0        0      381 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/types/tzcolors_auction/tezos_parameters/create_auction.py
+-rw-r--r--   0        0        0      187 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/types/tzcolors_auction/tezos_parameters/withdraw.py
+-rw-r--r--   0        0        0      555 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_auction/types/tzcolors_auction/tezos_storage.py
+-rw-r--r--   0        0        0      270 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/.dockerignore
+-rw-r--r--   0        0        0      356 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/.gitignore
+-rw-r--r--   0        0        0        1 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_big_maps/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_big_maps/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1162 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/README.md
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/abi/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/configs/.keep
+-rw-r--r--   0        0        0      379 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      150 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      401 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      404 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/configs/replay.yaml
+-rw-r--r--   0        0        0      356 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/deploy/.keep
+-rw-r--r--   0        0        0      150 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/deploy/Dockerfile
+-rw-r--r--   0        0        0      350 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2688 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1248 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/deploy/compose.yaml
+-rw-r--r--   0        0        0      280 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      318 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/deploy/swarm.env.default
+-rw-r--r--   0        0        0      725 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/handlers/.keep
+-rw-r--r--   0        0        0      846 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/handlers/on_update_expiry_map.py
+-rw-r--r--   0        0        0     1688 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/handlers/on_update_records.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/models/.keep
+-rw-r--r--   0        0        0      667 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:31:25.335052 dipdup-7.0.0rc3/src/demo_big_maps/py.typed
+-rw-r--r--   0        0        0     1051 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/sql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/types/.keep
+-rw-r--r--   0        0        0      199 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/types/name_registry/tezos_big_maps/store_expiry_map_key.py
+-rw-r--r--   0        0        0      203 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/types/name_registry/tezos_big_maps/store_expiry_map_value.py
+-rw-r--r--   0        0        0      194 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/types/name_registry/tezos_big_maps/store_records_key.py
+-rw-r--r--   0        0        0      489 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_big_maps/types/name_registry/tezos_big_maps/store_records_value.py
+-rw-r--r--   0        0        0      267 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_blank/.dockerignore
+-rw-r--r--   0        0        0      353 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_blank/.gitignore
+-rw-r--r--   0        0        0        1 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_blank/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_blank/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1163 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_blank/README.md
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_blank/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_blank/abi/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_blank/configs/.keep
+-rw-r--r--   0        0        0      379 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_blank/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      147 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_blank/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      395 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_blank/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      402 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_blank/configs/replay.yaml
+-rw-r--r--   0        0        0      327 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_blank/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.566346 dipdup-7.0.0rc3/src/demo_blank/deploy/.keep
+-rw-r--r--   0        0        0      144 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_blank/deploy/Dockerfile
+-rw-r--r--   0        0        0      344 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_blank/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2682 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_blank/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1245 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_blank/deploy/compose.yaml
+-rw-r--r--   0        0        0      248 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_blank/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      289 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_blank/deploy/swarm.env.default
+-rw-r--r--   0        0        0       37 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_blank/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_blank/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_blank/handlers/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_blank/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_blank/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_blank/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_blank/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_blank/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_blank/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_blank/models/.keep
+-rw-r--r--   0        0        0     1241 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_blank/models/__init__.py
+-rw-r--r--   0        0        0     1049 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_blank/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_blank/sql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_blank/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_blank/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_blank/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_blank/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_blank/types/.keep
+-rw-r--r--   0        0        0      265 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/.dockerignore
+-rw-r--r--   0        0        0      351 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/.gitignore
+-rw-r--r--   0        0        0        1 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_dao/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_dao/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1152 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/README.md
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/abi/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/configs/.keep
+-rw-r--r--   0        0        0      379 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      145 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      391 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      389 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/configs/replay.yaml
+-rw-r--r--   0        0        0      356 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/deploy/.keep
+-rw-r--r--   0        0        0      140 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/deploy/Dockerfile
+-rw-r--r--   0        0        0      340 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2678 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1243 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/deploy/compose.yaml
+-rw-r--r--   0        0        0      275 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      318 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/deploy/swarm.env.default
+-rw-r--r--   0        0        0      643 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/handlers/.keep
+-rw-r--r--   0        0        0      408 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/handlers/on_origination.py
+-rw-r--r--   0        0        0      506 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/handlers/on_propose.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/models/.keep
+-rw-r--r--   0        0        0      782 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:31:08.246756 dipdup-7.0.0rc3/src/demo_dao/py.typed
+-rw-r--r--   0        0        0     1036 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/sql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/types/.keep
+-rw-r--r--   0        0        0      360 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/types/registry/tezos_parameters/propose.py
+-rw-r--r--   0        0        0     2523 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dao/types/registry/tezos_storage.py
+-rw-r--r--   0        0        0      265 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/.dockerignore
+-rw-r--r--   0        0        0      351 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/.gitignore
+-rw-r--r--   0        0        0        1 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_dex/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_dex/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1167 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/README.md
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/abi/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/configs/.keep
+-rw-r--r--   0        0        0      379 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      145 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      391 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      404 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/configs/replay.yaml
+-rw-r--r--   0        0        0      327 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/deploy/.keep
+-rw-r--r--   0        0        0      140 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/deploy/Dockerfile
+-rw-r--r--   0        0        0      340 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2678 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1243 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/deploy/compose.yaml
+-rw-r--r--   0        0        0      246 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      289 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/deploy/swarm.env.default
+-rw-r--r--   0        0        0     4845 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/handlers/.keep
+-rw-r--r--   0        0        0     1829 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa12_divest_liquidity.py
+-rw-r--r--   0        0        0     1737 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa12_invest_liquidity.py
+-rw-r--r--   0        0        0      579 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa12_origination.py
+-rw-r--r--   0        0        0     1610 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa12_tez_to_token.py
+-rw-r--r--   0        0        0     1676 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa12_token_to_tez.py
+-rw-r--r--   0        0        0     1022 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa12_transfer.py
+-rw-r--r--   0        0        0      962 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa12_withdraw_profit.py
+-rw-r--r--   0        0        0     1855 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa2_divest_liquidity.py
+-rw-r--r--   0        0        0     1763 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa2_invest_liquidity.py
+-rw-r--r--   0        0        0      573 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa2_origination.py
+-rw-r--r--   0        0        0     1604 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa2_tez_to_token.py
+-rw-r--r--   0        0        0     1642 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa2_token_to_tez.py
+-rw-r--r--   0        0        0     1143 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa2_transfer.py
+-rw-r--r--   0        0        0      958 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa2_withdraw_profit.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/models/.keep
+-rw-r--r--   0        0        0      916 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:30:44.610295 dipdup-7.0.0rc3/src/demo_dex/py.typed
+-rw-r--r--   0        0        0     1051 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/sql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/types/.keep
+-rw-r--r--   0        0        0      340 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/types/fa12_token/tezos_parameters/transfer.py
+-rw-r--r--   0        0        0      739 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/types/fa12_token/tezos_storage.py
+-rw-r--r--   0        0        0      504 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/types/fa2_token/tezos_parameters/transfer.py
+-rw-r--r--   0        0        0     1093 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/types/fa2_token/tezos_storage.py
+-rw-r--r--   0        0        0      311 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/types/quipu_fa12/tezos_parameters/divest_liquidity.py
+-rw-r--r--   0        0        0      201 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/types/quipu_fa12/tezos_parameters/invest_liquidity.py
+-rw-r--r--   0        0        0      297 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/types/quipu_fa12/tezos_parameters/tez_to_token_payment.py
+-rw-r--r--   0        0        0      313 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/types/quipu_fa12/tezos_parameters/token_to_tez_payment.py
+-rw-r--r--   0        0        0      340 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/types/quipu_fa12/tezos_parameters/transfer.py
+-rw-r--r--   0        0        0      199 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/types/quipu_fa12/tezos_parameters/withdraw_profit.py
+-rw-r--r--   0        0        0     1455 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/types/quipu_fa12/tezos_storage.py
+-rw-r--r--   0        0        0      311 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/types/quipu_fa2/tezos_parameters/divest_liquidity.py
+-rw-r--r--   0        0        0      201 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/types/quipu_fa2/tezos_parameters/invest_liquidity.py
+-rw-r--r--   0        0        0      297 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/types/quipu_fa2/tezos_parameters/tez_to_token_payment.py
+-rw-r--r--   0        0        0      313 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/types/quipu_fa2/tezos_parameters/token_to_tez_payment.py
+-rw-r--r--   0        0        0      504 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/types/quipu_fa2/tezos_parameters/transfer.py
+-rw-r--r--   0        0        0      199 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/types/quipu_fa2/tezos_parameters/withdraw_profit.py
+-rw-r--r--   0        0        0     1491 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_dex/types/quipu_fa2/tezos_storage.py
+-rw-r--r--   0        0        0      269 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_domains/.dockerignore
+-rw-r--r--   0        0        0      355 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_domains/.gitignore
+-rw-r--r--   0        0        0        1 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_domains/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_domains/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1161 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_domains/README.md
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.570346 dipdup-7.0.0rc3/src/demo_domains/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/abi/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/configs/.keep
+-rw-r--r--   0        0        0      379 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      149 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      399 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      402 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/configs/replay.yaml
+-rw-r--r--   0        0        0      356 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/deploy/.keep
+-rw-r--r--   0        0        0      148 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/deploy/Dockerfile
+-rw-r--r--   0        0        0      348 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2686 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1247 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/deploy/compose.yaml
+-rw-r--r--   0        0        0      279 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      318 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/deploy/swarm.env.default
+-rw-r--r--   0        0        0      845 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/handlers/.keep
+-rw-r--r--   0        0        0      553 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/handlers/on_admin_update.py
+-rw-r--r--   0        0        0      525 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/handlers/on_execute.py
+-rw-r--r--   0        0        0     1437 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/handlers/on_storage_diff.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/models/.keep
+-rw-r--r--   0        0        0      630 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:30:32.490048 dipdup-7.0.0rc3/src/demo_domains/py.typed
+-rw-r--r--   0        0        0     1049 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/sql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/types/.keep
+-rw-r--r--   0        0        0      194 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/types/name_registry/tezos_parameters/admin_update.py
+-rw-r--r--   0        0        0      305 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/types/name_registry/tezos_parameters/execute.py
+-rw-r--r--   0        0        0     1134 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_domains/types/name_registry/tezos_storage.py
+-rw-r--r--   0        0        0      268 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/.dockerignore
+-rw-r--r--   0        0        0      354 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/.gitignore
+-rw-r--r--   0        0        0        1 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_events/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_events/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1160 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/README.md
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/abi/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/configs/.keep
+-rw-r--r--   0        0        0      379 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      148 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      397 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      400 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/configs/replay.yaml
+-rw-r--r--   0        0        0      327 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/deploy/.keep
+-rw-r--r--   0        0        0      146 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/deploy/Dockerfile
+-rw-r--r--   0        0        0      346 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2684 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1246 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/deploy/compose.yaml
+-rw-r--r--   0        0        0      249 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      289 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/deploy/swarm.env.default
+-rw-r--r--   0        0        0      536 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/handlers/.keep
+-rw-r--r--   0        0        0      311 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/handlers/on_move_event.py
+-rw-r--r--   0        0        0      237 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/handlers/on_other_event.py
+-rw-r--r--   0        0        0      311 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/handlers/on_roll_event.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/models/.keep
+-rw-r--r--   0        0        0     1241 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/models/__init__.py
+-rw-r--r--   0        0        0     1047 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/sql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/types/.keep
+-rw-r--r--   0        0        0      317 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/types/events_contract/tezos_events/move.py
+-rw-r--r--   0        0        0      266 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_events/types/events_contract/tezos_events/roll.py
+-rw-r--r--   0        0        0      272 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/.dockerignore
+-rw-r--r--   0        0        0      358 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/.gitignore
+-rw-r--r--   0        0        0        1 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_evm_events/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_evm_events/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1177 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/README.md
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/abi/.keep
+-rw-r--r--   0        0        0    11460 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/abi/eth_usdt/abi.json
+-rw-r--r--   0        0        0     2420 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/abi/eth_usdt/events.json
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/configs/.keep
+-rw-r--r--   0        0        0      379 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      152 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      405 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      421 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/configs/replay.yaml
+-rw-r--r--   0        0        0      409 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/deploy/.keep
+-rw-r--r--   0        0        0      154 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/deploy/Dockerfile
+-rw-r--r--   0        0        0      354 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2692 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1250 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/deploy/compose.yaml
+-rw-r--r--   0        0        0      335 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      371 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/deploy/swarm.env.default
+-rw-r--r--   0        0        0      694 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/handlers/.keep
+-rw-r--r--   0        0        0      992 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/handlers/on_transfer.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/models/.keep
+-rw-r--r--   0        0        0      368 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/models/__init__.py
+-rw-r--r--   0        0        0     1068 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/sql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/types/.keep
+-rw-r--r--   0        0        0      331 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_evm_events/types/eth_usdt/evm_events/transfer.py
+-rw-r--r--   0        0        0      271 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_factories/.dockerignore
+-rw-r--r--   0        0        0      357 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_factories/.gitignore
+-rw-r--r--   0        0        0        1 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_factories/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_factories/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1176 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_factories/README.md
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_factories/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_factories/abi/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_factories/configs/.keep
+-rw-r--r--   0        0        0      379 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_factories/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      151 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_factories/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      403 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_factories/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      419 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_factories/configs/replay.yaml
+-rw-r--r--   0        0        0      356 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_factories/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_factories/deploy/.keep
+-rw-r--r--   0        0        0      152 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_factories/deploy/Dockerfile
+-rw-r--r--   0        0        0      352 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_factories/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2690 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_factories/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1249 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_factories/deploy/compose.yaml
+-rw-r--r--   0        0        0      281 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_factories/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      318 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_factories/deploy/swarm.env.default
+-rw-r--r--   0        0        0      647 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_factories/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_factories/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_factories/handlers/.keep
+-rw-r--r--   0        0        0      420 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_factories/handlers/on_origination.py
+-rw-r--r--   0        0        0      524 2023-08-05 20:28:16.574346 dipdup-7.0.0rc3/src/demo_factories/handlers/on_propose.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_factories/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_factories/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_factories/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_factories/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_factories/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_factories/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_factories/models/.keep
+-rw-r--r--   0        0        0      782 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_factories/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:31:26.315072 dipdup-7.0.0rc3/src/demo_factories/py.typed
+-rw-r--r--   0        0        0     1066 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_factories/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_factories/sql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_factories/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_factories/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_factories/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_factories/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_factories/types/.keep
+-rw-r--r--   0        0        0      360 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_factories/types/registry/tezos_parameters/propose.py
+-rw-r--r--   0        0        0     2523 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_factories/types/registry/tezos_storage.py
+-rw-r--r--   0        0        0      266 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/.dockerignore
+-rw-r--r--   0        0        0      352 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/.gitignore
+-rw-r--r--   0        0        0        1 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_head/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_head/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1162 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/README.md
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/abi/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/configs/.keep
+-rw-r--r--   0        0        0      379 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      146 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      393 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      400 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/configs/replay.yaml
+-rw-r--r--   0        0        0      356 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/deploy/.keep
+-rw-r--r--   0        0        0      142 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/deploy/Dockerfile
+-rw-r--r--   0        0        0      342 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2680 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1244 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/deploy/compose.yaml
+-rw-r--r--   0        0        0      276 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      318 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/deploy/swarm.env.default
+-rw-r--r--   0        0        0      240 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/handlers/.keep
+-rw-r--r--   0        0        0      237 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/handlers/on_mainnet_head.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/models/.keep
+-rw-r--r--   0        0        0     1241 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/models/__init__.py
+-rw-r--r--   0        0        0     1047 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/sql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_head/types/.keep
+-rw-r--r--   0        0        0      277 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/.dockerignore
+-rw-r--r--   0        0        0      363 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/.gitignore
+-rw-r--r--   0        0        0        1 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_nft_marketplace/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_nft_marketplace/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1170 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/README.md
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/abi/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/configs/.keep
+-rw-r--r--   0        0        0      379 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      157 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      415 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      419 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/configs/replay.yaml
+-rw-r--r--   0        0        0      452 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/deploy/.keep
+-rw-r--r--   0        0        0      164 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/deploy/Dockerfile
+-rw-r--r--   0        0        0      364 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2702 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1255 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/deploy/compose.yaml
+-rw-r--r--   0        0        0      383 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      414 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/deploy/swarm.env.default
+-rw-r--r--   0        0        0     1199 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/handlers/.keep
+-rw-r--r--   0        0        0      605 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/handlers/on_cancel_swap.py
+-rw-r--r--   0        0        0     1037 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/handlers/on_collect.py
+-rw-r--r--   0        0        0      977 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/handlers/on_mint.py
+-rw-r--r--   0        0        0      885 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/handlers/on_swap.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/models/.keep
+-rw-r--r--   0        0        0     1306 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:30:42.566248 dipdup-7.0.0rc3/src/demo_nft_marketplace/py.typed
+-rw-r--r--   0        0        0     1066 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/sql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/types/.keep
+-rw-r--r--   0        0        0      192 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/cancel_swap.py
+-rw-r--r--   0        0        0      281 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/collect.py
+-rw-r--r--   0        0        0      317 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/mint_objkt.py
+-rw-r--r--   0        0        0      299 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/swap.py
+-rw-r--r--   0        0        0      777 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/types/hen_minter/tezos_storage.py
+-rw-r--r--   0        0        0      343 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/types/hen_objkts/tezos_parameters/mint.py
+-rw-r--r--   0        0        0     1094 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_nft_marketplace/types/hen_objkts/tezos_storage.py
+-rw-r--r--   0        0        0      265 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/.dockerignore
+-rw-r--r--   0        0        0      351 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/.gitignore
+-rw-r--r--   0        0        0        1 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_raw/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_raw/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1189 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/README.md
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/abi/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/configs/.keep
+-rw-r--r--   0        0        0      379 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      145 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      391 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      426 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/configs/replay.yaml
+-rw-r--r--   0        0        0      356 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/deploy/.keep
+-rw-r--r--   0        0        0      140 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/deploy/Dockerfile
+-rw-r--r--   0        0        0      340 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2678 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1243 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/deploy/compose.yaml
+-rw-r--r--   0        0        0      275 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      318 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/deploy/swarm.env.default
+-rw-r--r--   0        0        0      411 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/handlers/.keep
+-rw-r--r--   0        0        0      350 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/handlers/on_operation.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/models/.keep
+-rw-r--r--   0        0        0      245 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:31:36.159211 dipdup-7.0.0rc3/src/demo_raw/py.typed
+-rw-r--r--   0        0        0     1073 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/sql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_raw/types/.keep
+-rw-r--r--   0        0        0      267 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_token/.dockerignore
+-rw-r--r--   0        0        0      353 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_token/.gitignore
+-rw-r--r--   0        0        0        1 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_token/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_token/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1161 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_token/README.md
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.578346 dipdup-7.0.0rc3/src/demo_token/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/abi/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/configs/.keep
+-rw-r--r--   0        0        0      379 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      147 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      395 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      400 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/configs/replay.yaml
+-rw-r--r--   0        0        0      327 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/deploy/.keep
+-rw-r--r--   0        0        0      144 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/deploy/Dockerfile
+-rw-r--r--   0        0        0      344 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2682 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1245 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/deploy/compose.yaml
+-rw-r--r--   0        0        0      248 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      289 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/deploy/swarm.env.default
+-rw-r--r--   0        0        0      730 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/handlers/.keep
+-rw-r--r--   0        0        0      436 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/handlers/on_balance_update.py
+-rw-r--r--   0        0        0      630 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/handlers/on_mint.py
+-rw-r--r--   0        0        0      928 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/handlers/on_transfer.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/models/.keep
+-rw-r--r--   0        0        0      370 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:30:32.490048 dipdup-7.0.0rc3/src/demo_token/py.typed
+-rw-r--r--   0        0        0     1047 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/sql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/types/.keep
+-rw-r--r--   0        0        0      263 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/types/tzbtc/tezos_parameters/mint.py
+-rw-r--r--   0        0        0      340 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/types/tzbtc/tezos_parameters/transfer.py
+-rw-r--r--   0        0        0      398 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token/types/tzbtc/tezos_storage.py
+-rw-r--r--   0        0        0      277 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/.dockerignore
+-rw-r--r--   0        0        0      363 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/.gitignore
+-rw-r--r--   0        0        0        1 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_token_transfers/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_token_transfers/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1170 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/README.md
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/abi/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/configs/.keep
+-rw-r--r--   0        0        0      379 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      157 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      415 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      419 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/configs/replay.yaml
+-rw-r--r--   0        0        0      327 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/deploy/.keep
+-rw-r--r--   0        0        0      164 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/deploy/Dockerfile
+-rw-r--r--   0        0        0      364 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2702 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1255 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/deploy/compose.yaml
+-rw-r--r--   0        0        0      258 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      289 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/deploy/swarm.env.default
+-rw-r--r--   0        0        0      409 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/handlers/.keep
+-rw-r--r--   0        0        0      545 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/handlers/on_balance_update.py
+-rw-r--r--   0        0        0      836 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/handlers/on_token_transfer.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/models/.keep
+-rw-r--r--   0        0        0      370 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:31:05.666705 dipdup-7.0.0rc3/src/demo_token_transfers/py.typed
+-rw-r--r--   0        0        0     1066 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/sql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_token_transfers/types/.keep
+-rw-r--r--   0        0        0      269 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/.dockerignore
+-rw-r--r--   0        0        0      355 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/.gitignore
+-rw-r--r--   0        0        0        1 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_uniswap/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-08-05 20:29:32.212624 dipdup-7.0.0rc3/src/demo_uniswap/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1182 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/README.md
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/abi/.keep
+-rw-r--r--   0        0        0     4418 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/abi/factory/abi.json
+-rw-r--r--   0        0        0      919 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/abi/factory/events.json
+-rw-r--r--   0        0        0    19609 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/abi/pool/abi.json
+-rw-r--r--   0        0        0     3559 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/abi/pool/events.json
+-rw-r--r--   0        0        0    24313 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/abi/position_manager/abi.json
+-rw-r--r--   0        0        0     1984 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/abi/position_manager/events.json
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/configs/.keep
+-rw-r--r--   0        0        0      379 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      149 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      399 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      423 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/configs/replay.yaml
+-rw-r--r--   0        0        0      424 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/deploy/.keep
+-rw-r--r--   0        0        0      148 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/deploy/Dockerfile
+-rw-r--r--   0        0        0      348 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2686 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1247 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/deploy/compose.yaml
+-rw-r--r--   0        0        0      347 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      386 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/deploy/swarm.env.default
+-rw-r--r--   0        0        0     2236 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/handlers/.keep
+-rw-r--r--   0        0        0     3060 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/handlers/factory/pool_created.py
+-rw-r--r--   0        0        0      531 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/handlers/pool/burn.py
+-rw-r--r--   0        0        0      291 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/handlers/pool/flash.py
+-rw-r--r--   0        0        0      871 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/handlers/pool/initialize.py
+-rw-r--r--   0        0        0     1330 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/handlers/pool/mint.py
+-rw-r--r--   0        0        0     6558 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/handlers/pool/swap.py
+-rw-r--r--   0        0        0     1227 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/handlers/position_manager/collect.py
+-rw-r--r--   0        0        0     1361 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/handlers/position_manager/decrease_liquidity.py
+-rw-r--r--   0        0        0     1449 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/handlers/position_manager/increase_liquidity.py
+-rw-r--r--   0        0        0     1172 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/handlers/position_manager/transfer.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/models/.keep
+-rw-r--r--   0        0        0    19932 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/models/__init__.py
+-rw-r--r--   0        0        0      373 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/models/abi.py
+-rw-r--r--   0        0        0     4162 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/models/pool.py
+-rw-r--r--   0        0        0     2824 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/models/position.py
+-rw-r--r--   0        0        0     1477 2023-08-05 20:28:16.582347 dipdup-7.0.0rc3/src/demo_uniswap/models/repo.py
+-rw-r--r--   0        0        0      561 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/demo_uniswap/models/tick.py
+-rw-r--r--   0        0        0     7160 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/demo_uniswap/models/token.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/demo_uniswap/py.typed
+-rw-r--r--   0        0        0     1070 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/demo_uniswap/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/demo_uniswap/sql/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/demo_uniswap/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/demo_uniswap/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/demo_uniswap/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/demo_uniswap/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/demo_uniswap/types/.keep
+-rw-r--r--   0        0        0      321 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/demo_uniswap/types/factory/evm_events/pool_created.py
+-rw-r--r--   0        0        0      330 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/demo_uniswap/types/pool/evm_events/burn.py
+-rw-r--r--   0        0        0      339 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/demo_uniswap/types/pool/evm_events/collect.py
+-rw-r--r--   0        0        0      328 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/demo_uniswap/types/pool/evm_events/flash.py
+-rw-r--r--   0        0        0      275 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/demo_uniswap/types/pool/evm_events/initialize.py
+-rw-r--r--   0        0        0      346 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/demo_uniswap/types/pool/evm_events/mint.py
+-rw-r--r--   0        0        0      351 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/demo_uniswap/types/pool/evm_events/swap.py
+-rw-r--r--   0        0        0      303 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/demo_uniswap/types/position_manager/evm_events/collect.py
+-rw-r--r--   0        0        0      323 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/demo_uniswap/types/position_manager/evm_events/decrease_liquidity.py
+-rw-r--r--   0        0        0      323 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/demo_uniswap/types/position_manager/evm_events/increase_liquidity.py
+-rw-r--r--   0        0        0      333 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/demo_uniswap/types/position_manager/evm_events/transfer.py
+-rw-r--r--   0        0        0      179 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/__init__.py
+-rw-r--r--   0        0        0      105 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/__main__.py
+-rw-r--r--   0        0        0      512 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/api.py
+-rw-r--r--   0        0        0    22027 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/cli.py
+-rw-r--r--   0        0        0     7972 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/codegen/__init__.py
+-rw-r--r--   0        0        0     7317 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/codegen/evm_subsquid.py
+-rw-r--r--   0        0        0    18580 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/codegen/tezos_tzkt.py
+-rw-r--r--   0        0        0    41898 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/config/__init__.py
+-rw-r--r--   0        0        0      554 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/config/abi_etherscan.py
+-rw-r--r--   0        0        0      690 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/config/coinbase.py
+-rw-r--r--   0        0        0     1469 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/config/evm.py
+-rw-r--r--   0        0        0     1273 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/config/evm_node.py
+-rw-r--r--   0        0        0     1375 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/config/evm_subsquid.py
+-rw-r--r--   0        0        0     2578 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/config/evm_subsquid_events.py
+-rw-r--r--   0        0        0     1495 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/config/evm_subsquid_operations.py
+-rw-r--r--   0        0        0      446 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/config/http.py
+-rw-r--r--   0        0        0      519 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/config/ipfs.py
+-rw-r--r--   0        0        0     1532 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/config/tezos.py
+-rw-r--r--   0        0        0     2157 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/config/tezos_tzkt.py
+-rw-r--r--   0        0        0     3758 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/config/tezos_tzkt_big_maps.py
+-rw-r--r--   0        0        0     3074 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/config/tezos_tzkt_events.py
+-rw-r--r--   0        0        0     1424 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/config/tezos_tzkt_head.py
+-rw-r--r--   0        0        0    12744 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/config/tezos_tzkt_operations.py
+-rw-r--r--   0        0        0     3110 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/config/tezos_tzkt_token_transfers.py
+-rw-r--r--   0        0        0      745 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/config/tzip_metadata.py
+-rw-r--r--   0        0        0    28058 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/context.py
+-rw-r--r--   0        0        0    14211 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/database.py
+-rw-r--r--   0        0        0     4474 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/datasources/__init__.py
+-rw-r--r--   0        0        0      915 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/datasources/abi_etherscan.py
+-rw-r--r--   0        0        0     2274 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/datasources/coinbase.py
+-rw-r--r--   0        0        0    12321 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/datasources/evm_node.py
+-rw-r--r--   0        0        0     4013 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/datasources/evm_subsquid.py
+-rw-r--r--   0        0        0      399 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/datasources/http.py
+-rw-r--r--   0        0        0      524 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/datasources/ipfs.py
+-rw-r--r--   0        0        0    43369 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/datasources/tezos_tzkt.py
+-rw-r--r--   0        0        0     1545 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/datasources/tzip_metadata.py
+-rw-r--r--   0        0        0    30185 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/dipdup.py
+-rw-r--r--   0        0        0     1957 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/env.py
+-rw-r--r--   0        0        0     8274 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/exceptions.py
+-rw-r--r--   0        0        0     3981 2023-08-05 20:28:16.586347 dipdup-7.0.0rc3/src/dipdup/fetcher.py
+-rw-r--r--   0        0        0     6724 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/fields.py
+-rw-r--r--   0        0        0    25644 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/hasura.py
+-rw-r--r--   0        0        0    11008 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/http.py
+-rw-r--r--   0        0        0     7426 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/index.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/__init__.py
+-rw-r--r--   0        0        0     1229 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/evm_subsquid_events/fetcher.py
+-rw-r--r--   0        0        0    10389 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/evm_subsquid_events/index.py
+-rw-r--r--   0        0        0     3439 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/evm_subsquid_events/matcher.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/evm_subsquid_events/parser.py
+-rw-r--r--   0        0        0      406 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/evm_subsquid_operations/index.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_big_maps/__init__.py
+-rw-r--r--   0        0        0     3181 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_big_maps/fetcher.py
+-rw-r--r--   0        0        0     7320 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_big_maps/index.py
+-rw-r--r--   0        0        0     2684 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_big_maps/matcher.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_events/__init__.py
+-rw-r--r--   0        0        0     1480 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_events/fetcher.py
+-rw-r--r--   0        0        0     5539 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_events/index.py
+-rw-r--r--   0        0        0     3895 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_events/matcher.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_head/__init__.py
+-rw-r--r--   0        0        0     2349 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_head/index.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_operations/__init__.py
+-rw-r--r--   0        0        0    20276 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_operations/fetcher.py
+-rw-r--r--   0        0        0    13485 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_operations/index.py
+-rw-r--r--   0        0        0     9165 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_operations/matcher.py
+-rw-r--r--   0        0        0     7612 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_operations/parser.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_token_transfers/__init__.py
+-rw-r--r--   0        0        0     1432 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_token_transfers/fetcher.py
+-rw-r--r--   0        0        0     5520 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_token_transfers/index.py
+-rw-r--r--   0        0        0     1808 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_token_transfers/matcher.py
+-rwxr-xr-x   0        0        0     9379 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/install.py
+-rw-r--r--   0        0        0    20461 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/models/__init__.py
+-rw-r--r--   0        0        0     1309 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/models/coinbase.py
+-rw-r--r--   0        0        0     3596 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/models/evm_node.py
+-rw-r--r--   0        0        0     5045 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/models/evm_subsquid.py
+-rw-r--r--   0        0        0    19886 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/models/tezos_tzkt.py
+-rw-r--r--   0        0        0      165 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/models/tzip_metadata.py
+-rw-r--r--   0        0        0     7226 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/package.py
+-rw-r--r--   0        0        0     7091 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/performance.py
+-rw-r--r--   0        0        0     8379 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/project.py
+-rw-r--r--   0        0        0      279 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/base/.dockerignore.j2
+-rw-r--r--   0        0        0      364 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/base/.gitignore.j2
+-rw-r--r--   0        0        0     1166 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/base/README.md.j2
+-rw-r--r--   0        0        0      380 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/base/configs/dipdup.compose.yaml.j2
+-rw-r--r--   0        0        0      159 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/base/configs/dipdup.sqlite.yaml.j2
+-rw-r--r--   0        0        0      418 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/base/configs/dipdup.swarm.yaml.j2
+-rw-r--r--   0        0        0      221 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/base/deploy/Dockerfile.j2
+-rw-r--r--   0        0        0      367 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/base/deploy/compose.sqlite.yaml.j2
+-rw-r--r--   0        0        0     2748 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/base/deploy/compose.swarm.yaml.j2
+-rw-r--r--   0        0        0     1273 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/base/deploy/compose.yaml.j2
+-rw-r--r--   0        0        0     1240 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/base/pyproject.toml.j2
+-rw-r--r--   0        0        0     1087 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_auction/dipdup.yaml.j2
+-rw-r--r--   0        0        0      935 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_auction/handlers/on_bid.py.j2
+-rw-r--r--   0        0        0     1641 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_auction/handlers/on_create_auction.py.j2
+-rw-r--r--   0        0        0      734 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_auction/handlers/on_withdraw.py.j2
+-rw-r--r--   0        0        0     1447 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_auction/models/__init__.py.j2
+-rw-r--r--   0        0        0      114 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_auction/replay.yaml
+-rw-r--r--   0        0        0      734 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_big_maps/dipdup.yaml.j2
+-rw-r--r--   0        0        0      865 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_big_maps/handlers/on_update_expiry_map.py.j2
+-rw-r--r--   0        0        0     1707 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_big_maps/handlers/on_update_records.py.j2
+-rw-r--r--   0        0        0      669 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_big_maps/models/__init__.py.j2
+-rw-r--r--   0        0        0      118 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_big_maps/replay.yaml
+-rw-r--r--   0        0        0       49 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_blank/dipdup.yaml.j2
+-rw-r--r--   0        0        0      116 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_blank/replay.yaml
+-rw-r--r--   0        0        0      657 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_dao/dipdup.yaml.j2
+-rw-r--r--   0        0        0      431 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_dao/handlers/on_origination.py.j2
+-rw-r--r--   0        0        0      540 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_dao/handlers/on_propose.py.j2
+-rw-r--r--   0        0        0      784 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_dao/models/__init__.py.j2
+-rw-r--r--   0        0        0      103 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_dao/replay.yaml
+-rw-r--r--   0        0        0     4859 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/dipdup.yaml.j2
+-rw-r--r--   0        0        0     1885 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa12_divest_liquidity.py.j2
+-rw-r--r--   0        0        0     1793 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa12_invest_liquidity.py.j2
+-rw-r--r--   0        0        0      602 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa12_origination.py.j2
+-rw-r--r--   0        0        0     1666 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa12_tez_to_token.py.j2
+-rw-r--r--   0        0        0     1732 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa12_token_to_tez.py.j2
+-rw-r--r--   0        0        0     1056 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa12_transfer.py.j2
+-rw-r--r--   0        0        0      996 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa12_withdraw_profit.py.j2
+-rw-r--r--   0        0        0     1911 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa2_divest_liquidity.py.j2
+-rw-r--r--   0        0        0     1819 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa2_invest_liquidity.py.j2
+-rw-r--r--   0        0        0      596 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa2_origination.py.j2
+-rw-r--r--   0        0        0     1660 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa2_tez_to_token.py.j2
+-rw-r--r--   0        0        0     1698 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa2_token_to_tez.py.j2
+-rw-r--r--   0        0        0     1177 2023-08-05 20:28:16.590347 dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa2_transfer.py.j2
+-rw-r--r--   0        0        0      992 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa2_withdraw_profit.py.j2
+-rw-r--r--   0        0        0      918 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/models/__init__.py.j2
+-rw-r--r--   0        0        0      118 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/replay.yaml
+-rw-r--r--   0        0        0      855 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_domains/dipdup.yaml.j2
+-rw-r--r--   0        0        0      581 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_domains/handlers/on_admin_update.py.j2
+-rw-r--r--   0        0        0      553 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_domains/handlers/on_execute.py.j2
+-rw-r--r--   0        0        0     1456 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_domains/handlers/on_storage_diff.py.j2
+-rw-r--r--   0        0        0      632 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_domains/models/__init__.py.j2
+-rw-r--r--   0        0        0      116 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_domains/replay.yaml
+-rw-r--r--   0        0        0      547 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_events/dipdup.yaml.j2
+-rw-r--r--   0        0        0      114 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_events/replay.yaml
+-rw-r--r--   0        0        0      701 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_evm_events/dipdup.yaml.j2
+-rw-r--r--   0        0        0     1005 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_evm_events/handlers/on_transfer.py.j2
+-rw-r--r--   0        0        0      370 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_evm_events/models/__init__.py.j2
+-rw-r--r--   0        0        0      135 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_evm_events/replay.yaml
+-rw-r--r--   0        0        0      655 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_factories/dipdup.yaml.j2
+-rw-r--r--   0        0        0      431 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_factories/handlers/on_origination.py.j2
+-rw-r--r--   0        0        0      540 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_factories/handlers/on_propose.py.j2
+-rw-r--r--   0        0        0      784 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_factories/models/__init__.py.j2
+-rw-r--r--   0        0        0      133 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_factories/replay.yaml
+-rw-r--r--   0        0        0      253 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_head/dipdup.yaml.j2
+-rw-r--r--   0        0        0      114 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_head/replay.yaml
+-rw-r--r--   0        0        0     1201 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_nft_marketplace/dipdup.yaml.j2
+-rw-r--r--   0        0        0      603 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_nft_marketplace/handlers/on_cancel_swap.py.j2
+-rw-r--r--   0        0        0     1035 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_nft_marketplace/handlers/on_collect.py.j2
+-rw-r--r--   0        0        0      973 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_nft_marketplace/handlers/on_mint.py.j2
+-rw-r--r--   0        0        0      883 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_nft_marketplace/handlers/on_swap.py.j2
+-rw-r--r--   0        0        0     1309 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_nft_marketplace/models/__init__.py.j2
+-rw-r--r--   0        0        0      133 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_nft_marketplace/replay.yaml
+-rw-r--r--   0        0        0      425 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_raw/dipdup.yaml.j2
+-rw-r--r--   0        0        0      364 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_raw/handlers/on_operation.py.j2
+-rw-r--r--   0        0        0      247 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_raw/models/__init__.py.j2
+-rw-r--r--   0        0        0      140 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_raw/replay.yaml
+-rw-r--r--   0        0        0      742 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_token/dipdup.yaml.j2
+-rw-r--r--   0        0        0      448 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_token/handlers/on_balance_update.py.j2
+-rw-r--r--   0        0        0      664 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_token/handlers/on_mint.py.j2
+-rw-r--r--   0        0        0      962 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_token/handlers/on_transfer.py.j2
+-rw-r--r--   0        0        0      372 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_token/models/__init__.py.j2
+-rw-r--r--   0        0        0      114 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_token/replay.yaml
+-rw-r--r--   0        0        0      411 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_token_transfers/dipdup.yaml.j2
+-rw-r--r--   0        0        0      545 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_token_transfers/handlers/on_balance_update.py.j2
+-rw-r--r--   0        0        0      836 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_token_transfers/handlers/on_token_transfer.py.j2
+-rw-r--r--   0        0        0      372 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_token_transfers/models/__init__.py.j2
+-rw-r--r--   0        0        0      133 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_token_transfers/replay.yaml
+-rw-r--r--   0        0        0     2255 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/dipdup.yaml.j2
+-rw-r--r--   0        0        0     3097 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/handlers/factory/pool_created.py.j2
+-rw-r--r--   0        0        0      568 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/handlers/pool/burn.py.j2
+-rw-r--r--   0        0        0      310 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/handlers/pool/flash.py.j2
+-rw-r--r--   0        0        0      899 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/handlers/pool/initialize.py.j2
+-rw-r--r--   0        0        0     1376 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/handlers/pool/mint.py.j2
+-rw-r--r--   0        0        0     6631 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/handlers/pool/swap.py.j2
+-rw-r--r--   0        0        0     1264 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/handlers/position_manager/collect.py.j2
+-rw-r--r--   0        0        0     1398 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/handlers/position_manager/decrease_liquidity.py.j2
+-rw-r--r--   0        0        0     1486 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/handlers/position_manager/increase_liquidity.py.j2
+-rw-r--r--   0        0        0     1200 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/handlers/position_manager/transfer.py.j2
+-rw-r--r--   0        0        0    19933 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/models/__init__.py.j2
+-rw-r--r--   0        0        0      374 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/models/abi.py.j2
+-rw-r--r--   0        0        0     4226 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/models/pool.py.j2
+-rw-r--r--   0        0        0     2844 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/models/position.py.j2
+-rw-r--r--   0        0        0     1478 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/models/repo.py.j2
+-rw-r--r--   0        0        0      571 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/models/tick.py.j2
+-rw-r--r--   0        0        0     7188 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/models/token.py.j2
+-rw-r--r--   0        0        0      137 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/replay.yaml
+-rw-r--r--   0        0        0     4008 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/prometheus.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/py.typed
+-rw-r--r--   0        0        0     1631 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/pysignalr.py
+-rw-r--r--   0        0        0     1722 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/report.py
+-rw-r--r--   0        0        0     4867 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/scheduler.py
+-rw-r--r--   0        0        0     4647 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/sentry.py
+-rw-r--r--   0        0        0      199 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/sql/dipdup_head_status.sql
+-rw-r--r--   0        0        0     2111 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/sql/truncate_schema.sql
+-rw-r--r--   0        0        0     2163 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/subscriptions.py
+-rw-r--r--   0        0        0     1791 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/sys.py
+-rw-r--r--   0        0        0      227 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/templates/callback.py.j2
+-rw-r--r--   0        0        0     1241 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/templates/models.py
+-rw-r--r--   0        0        0      186 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/templates/replay.yaml.j2
+-rw-r--r--   0        0        0     3290 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/transactions.py
+-rw-r--r--   0        0        0     7169 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/utils.py
+-rw-r--r--   0        0        0     5411 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/src/dipdup/yaml.py
+-rw-r--r--   0        0        0      952 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/__init__.py
+-rw-r--r--   0        0        0      496 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/configs/asdf.yml
+-rw-r--r--   0        0        0     1222 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/configs/demo_auction.yml
+-rw-r--r--   0        0        0      780 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/configs/demo_big_maps.yml
+-rw-r--r--   0        0        0      745 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/configs/demo_dao.yml
+-rw-r--r--   0        0        0     5012 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/configs/demo_dex.yml
+-rw-r--r--   0        0        0      898 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/configs/demo_domains.yml
+-rw-r--r--   0        0        0      878 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/configs/demo_factories.yml
+-rw-r--r--   0        0        0     1316 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/configs/demo_nft_marketplace.yml
+-rw-r--r--   0        0        0      590 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/configs/demo_raw.yml
+-rw-r--r--   0        0        0      711 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/configs/demo_token.yml
+-rw-r--r--   0        0        0      527 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/configs/demo_token_transfers.yml
+-rw-r--r--   0        0        0      527 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/configs/demo_token_transfers_2.yml
+-rw-r--r--   0        0        0      527 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/configs/demo_token_transfers_3.yml
+-rw-r--r--   0        0        0      814 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/configs/demo_token_transfers_4.yml
+-rw-r--r--   0        0        0     1252 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/configs/dipdup.yml
+-rw-r--r--   0        0        0      521 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/configs/hen_subjkt.yml
+-rw-r--r--   0        0        0      496 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/configs/hjkl.yml
+-rw-r--r--   0        0        0      546 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/configs/kolibri_ovens.yml
+-rw-r--r--   0        0        0      684 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/configs/operation_filters.yml
+-rw-r--r--   0        0        0      496 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/configs/qwer.yml
+-rw-r--r--   0        0        0      496 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/configs/rewq.yml
+-rw-r--r--   0        0        0       44 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/configs/sqlite.yaml
+-rw-r--r--   0        0        0      534 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/configs/yupana.yml
+-rw-r--r--   0        0        0      496 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/configs/zxcv.yml
+-rw-r--r--   0        0        0     1285 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/profile_abi_decoding.py
+-rw-r--r--   0        0        0        2 2023-08-05 20:30:35.354110 dipdup-7.0.0rc3/tests/replays/024e925225593fe9cd80f5a114201f74d9f3631cea6f03add3e88fc91fafd2d7
+-rw-r--r--   0        0        0    11605 2023-08-05 20:28:16.594347 dipdup-7.0.0rc3/tests/replays/0535b2dcc93076e6026fa48cc501adaed47b7b060e6483d8312f40c184d7287d
+-rw-r--r--   0        0        0  2577538 2023-08-05 20:28:16.610348 dipdup-7.0.0rc3/tests/replays/064e788d2566d748f516b17c6a43ab34259443cc9537f0dec7c1a5a2bce704b2
+-rw-r--r--   0        0        0      305 2023-08-05 20:31:38.827257 dipdup-7.0.0rc3/tests/replays/0b7d26b8f2813d12a80b9e96cc6f0bb186bf9ac5c5b0c0b3bb2cc8d750126843
+-rw-r--r--   0        0        0      784 2023-08-05 20:28:16.610348 dipdup-7.0.0rc3/tests/replays/0eaaba2830dbdd3a80286fbc367084bce6e55c678e21da178a7eb16beef6c997
+-rw-r--r--   0        0        0       20 2023-08-05 20:28:16.610348 dipdup-7.0.0rc3/tests/replays/1165d42ccbdd0f6c25cece69d2c579da07655a30d04f18840350a153a98827a0
+-rw-r--r--   0        0        0     7446 2023-08-05 20:28:16.610348 dipdup-7.0.0rc3/tests/replays/1228b36594bb93d619170ad49373f1ceec52d10faafdd727b37f3cdeffd663db
+-rw-r--r--   0        0        0   108455 2023-08-05 20:31:28.019087 dipdup-7.0.0rc3/tests/replays/136157c421184c218127595797f5fe0b774e2807f6f4605a1d1944a1738e2d6d
+-rw-r--r--   0        0        0     4947 2023-08-05 20:28:16.610348 dipdup-7.0.0rc3/tests/replays/13afdf001ce3d6a0219c0f7f6d372d9b645770e5f4304576f7f7a37b45af96fc
+-rw-r--r--   0        0        0      310 2023-08-05 20:28:16.610348 dipdup-7.0.0rc3/tests/replays/1430e37dce64ecb83499da8feaa3c0906e4fdf5d0a3c3570174645e97ba54bc4
+-rw-r--r--   0        0        0    13275 2023-08-05 20:28:16.610348 dipdup-7.0.0rc3/tests/replays/14408f393a3e399b241184f858e70396e3b8313e32ee1a984913d43fb74dcfec
+-rw-r--r--   0        0        0   855628 2023-08-05 20:30:47.378354 dipdup-7.0.0rc3/tests/replays/14cba0424c66b1869edc8e18ca3079856083cc3db7e68ef61fce165b6d7e1a6d
+-rw-r--r--   0        0        0      129 2023-08-05 20:28:16.610348 dipdup-7.0.0rc3/tests/replays/14d37c70764fe50b4ea590691d5614f613f96b8ad98c5df189564778616f5261
+-rw-r--r--   0        0        0      246 2023-08-05 20:28:16.610348 dipdup-7.0.0rc3/tests/replays/185f6628ac43f6ca728c5b79b7b81a3c3671efce7f14030a06a27e90cf641dea
+-rw-r--r--   0        0        0      986 2023-08-05 20:28:16.610348 dipdup-7.0.0rc3/tests/replays/18d85ceab66daf057861b99b7e223a25067197b3b77edbf060390df58cb65eaa
+-rw-r--r--   0        0        0     1448 2023-08-05 20:28:16.610348 dipdup-7.0.0rc3/tests/replays/19441b677ef5fd8ca39c37e6ddd2a7d9bc8cb3ab282b2a91ce4d8430f56f0fa9
+-rw-r--r--   0        0        0   612008 2023-08-05 20:28:16.610348 dipdup-7.0.0rc3/tests/replays/1a43bd7d1397cc3169ad267cd2ef083a5a63eaac7ed5186aadfc01bb53636214
+-rw-r--r--   0        0        0  1154515 2023-08-05 20:30:48.702377 dipdup-7.0.0rc3/tests/replays/1c07d3d72acc637fb46c59d0a6dc9749f3412a5d527ca2eb0cccc01720fda1c7
+-rw-r--r--   0        0        0    89590 2023-08-05 20:28:16.610348 dipdup-7.0.0rc3/tests/replays/1c34d1f810ae474395893bf67fb8cfb27b0506ab94eebec42cd4d2d21bf3dfcd
+-rw-r--r--   0        0        0        2 2023-08-05 20:30:35.350110 dipdup-7.0.0rc3/tests/replays/1c717490846300e1639e96a0c1438b6dd2abd6de013c5edec49042fa364c06e6
+-rw-r--r--   0        0        0    12263 2023-08-05 20:28:16.614348 dipdup-7.0.0rc3/tests/replays/252fd058cfef21f9b5b7f4367f730ec7d41647253d7cc7ccfb1e22d42d1f366a
+-rw-r--r--   0        0        0     1167 2023-08-05 20:28:16.614348 dipdup-7.0.0rc3/tests/replays/27373c23411bf37b605c8d0ead9a0e6c6c1f1718ce7863b095b759811e44e155
+-rw-r--r--   0        0        0     1121 2023-08-05 20:28:16.614348 dipdup-7.0.0rc3/tests/replays/2a45ec6372b45e46199a6af24272cb93586777a0522cd1203b3eeef213ce4583
+-rw-r--r--   0        0        0   209761 2023-08-05 20:30:47.818362 dipdup-7.0.0rc3/tests/replays/31cc70e13495f58ecde80847bc6c9e08536cc426c03bd2aa8c45c1b2c798e155
+-rw-r--r--   0        0        0 21118960 2023-08-05 20:28:16.658350 dipdup-7.0.0rc3/tests/replays/31dd376b771f347a0d6fe4dd132a1f96f809274429b78ec86dd742e5589fbc23
+-rw-r--r--   0        0        0  1807578 2023-08-05 20:30:35.934123 dipdup-7.0.0rc3/tests/replays/32e3a13cc470d8720ce28f5eaff327340fb25cbe712e5b5a348af1bc3c92235a
+-rw-r--r--   0        0        0       65 2023-08-05 20:28:16.658350 dipdup-7.0.0rc3/tests/replays/33349b63491dc976a7a2332d3cca3bd9b3b831c02a6f474bb925876c1838633a
+-rw-r--r--   0        0        0        2 2023-08-05 20:28:16.658350 dipdup-7.0.0rc3/tests/replays/34f3e33d677f85b633cb85c6dd205beb40e3d9c40cfafc7084b82c8123a54de1
+-rw-r--r--   0        0        0    45221 2023-08-05 20:28:16.658350 dipdup-7.0.0rc3/tests/replays/36072e13c9ce265bb81142b8816da8c31bd9180e7c663ea4169bd259af107382
+-rw-r--r--   0        0        0    81885 2023-08-05 20:28:16.658350 dipdup-7.0.0rc3/tests/replays/377ac31d6316391ed138df44bec374d65202f0577603e80465ced3c09140f78c
+-rw-r--r--   0        0        0    54602 2023-08-05 20:30:58.042565 dipdup-7.0.0rc3/tests/replays/383899084f79460e96fd311bb64e4925738c486b39d6281539456c5fcac41620
+-rw-r--r--   0        0        0      642 2023-08-05 20:31:23.643018 dipdup-7.0.0rc3/tests/replays/39b8664d1bca5d374ff905c8a3a396b53d19ee469dc37545a8ca6b080bd0e9e0
+-rw-r--r--   0        0        0     1200 2023-08-05 20:31:41.091295 dipdup-7.0.0rc3/tests/replays/3a2bd8b6b72bf18152d2550c106789fa9b8abc98ea9d759a6597b7ebfbab0fc2
+-rw-r--r--   0        0        0    81885 2023-08-05 20:28:16.658350 dipdup-7.0.0rc3/tests/replays/3c9ad6f98f79e72185ea58c4777115750c658c5defd616664212095bd440c10c
+-rw-r--r--   0        0        0      332 2023-08-05 20:28:16.658350 dipdup-7.0.0rc3/tests/replays/3fdba02cbc415eba224604f4fea130acd4565d31e4a83cdbb679ec0b76c798ab
+-rw-r--r--   0        0        0  3369404 2023-08-05 20:31:13.334859 dipdup-7.0.0rc3/tests/replays/42b7bf0da866257ef98e1f7124d2d21fe7d13228c076fffa32331da423f36933
+-rw-r--r--   0        0        0      619 2023-08-05 20:28:16.658350 dipdup-7.0.0rc3/tests/replays/43cb0ab415d8b8b3f7addc3e82ea27d93b2c66ff55c117e1e0c7c64a0fcfc3f2
+-rw-r--r--   0        0        0   530743 2023-08-05 20:28:16.662350 dipdup-7.0.0rc3/tests/replays/440173d32e95111ca7b080ccc4dc09bfab23c8361919b2c113f0ff9ab445eec2
+-rw-r--r--   0        0        0  1594116 2023-08-05 20:28:16.662350 dipdup-7.0.0rc3/tests/replays/489233ce9373f7de4f7a9053055c74bc0df999bfe939ed67d98b6d67e676e35a
+-rw-r--r--   0        0        0   109726 2023-08-05 20:30:45.550317 dipdup-7.0.0rc3/tests/replays/4a57776d93475adfd9c49b6c3295a7cedfc23b73733a1fb5f0c985ee039dc5dc
+-rw-r--r--   0        0        0      984 2023-08-05 20:28:16.662350 dipdup-7.0.0rc3/tests/replays/4aa7f9b0657be0c44baf2caed8c7cb08d02097a4095cf6417f78cba3a25e8423
+-rw-r--r--   0        0        0       67 2023-08-05 20:31:36.835223 dipdup-7.0.0rc3/tests/replays/4fbdb4667971fab446a5ac5937a7c8cc6ef5813ff00af24b6fd1b1a0427bedbb
+-rw-r--r--   0        0        0   192680 2023-08-05 20:30:45.382313 dipdup-7.0.0rc3/tests/replays/5483a0e11009e0f186bf70c214e2597d267a75a1e19152a9e7ed1ec257ce88ca
+-rw-r--r--   0        0        0       65 2023-08-05 20:28:16.662350 dipdup-7.0.0rc3/tests/replays/56eb33fbb563bf03ea7639659fae5102222d6e3cea882febf71f01bd383c6eed
+-rw-r--r--   0        0        0    40432 2023-08-05 20:30:57.906563 dipdup-7.0.0rc3/tests/replays/587613799ebfae42b1884016d1a44a452d68e70e3ed80641d90b8e7657ba8ee5
+-rw-r--r--   0        0        0       32 2023-08-05 20:28:16.662350 dipdup-7.0.0rc3/tests/replays/5b004196490632859ec1b019d640f6bbb93fc86a433c8969e10f36f51ac2c78d
+-rw-r--r--   0        0        0     1907 2023-08-05 20:28:16.662350 dipdup-7.0.0rc3/tests/replays/5b7c31b4b73bc57e8296e6051b3bc7b2302b32588d8fbcafce8a66de3be743df
+-rw-r--r--   0        0        0     7609 2023-08-05 20:28:16.662350 dipdup-7.0.0rc3/tests/replays/5b99bc4beb6a9a33f7d2f118426458e4c788e0ab6d9e51949d3ccbf8b4003fc1
+-rw-r--r--   0        0        0      939 2023-08-05 20:28:16.662350 dipdup-7.0.0rc3/tests/replays/5d21060ba8e78279d2d1edaa2f266ecf36105eaccef5ebed15748441651f76fd
+-rw-r--r--   0        0        0      400 2023-08-05 20:28:16.662350 dipdup-7.0.0rc3/tests/replays/5f63ef9dd15459ae14e715bb79da8f033a24b54504212ebc873ee8aa95679606
+-rw-r--r--   0        0        0       67 2023-08-05 20:31:36.963225 dipdup-7.0.0rc3/tests/replays/60f48c13c47a1347786a6dcf6f741874e7b30b587d148faa67d15067bb3871de
+-rw-r--r--   0        0        0       21 2023-08-05 20:28:16.662350 dipdup-7.0.0rc3/tests/replays/62e95f1d55b756895289374b351a1da94505ec2d95a1652c97765f36a2ef9341
+-rw-r--r--   0        0        0   211527 2023-08-05 20:30:48.906381 dipdup-7.0.0rc3/tests/replays/6cc8d741a41b76983cd7e0f63e8f22a4c67cd946888f45a5b7ead8c3bb5ad2f1
+-rw-r--r--   0        0        0   944885 2023-08-05 20:28:16.666350 dipdup-7.0.0rc3/tests/replays/6cff8d120db8fd3926a45714ce7f1d0560803eb5a7b4a413b64fee1b7fd7a8ff
+-rw-r--r--   0        0        0      132 2023-08-05 20:31:37.751238 dipdup-7.0.0rc3/tests/replays/6d0c5443d41a15551acb41adc10d36d4895f5786d6922a878b5c5414610e0ebc
+-rw-r--r--   0        0        0      754 2023-08-05 20:31:38.323248 dipdup-7.0.0rc3/tests/replays/6d76a3c3f427ff534c551de1793cb1d1dfbd22ccad97f5917a9f9b201a3f9804
+-rw-r--r--   0        0        0      494 2023-08-05 20:28:16.666350 dipdup-7.0.0rc3/tests/replays/7132f07560319399092782debe6eb28926e961d8af215ce11e2c0efd8dab06da
+-rw-r--r--   0        0        0      451 2023-08-05 20:31:38.955259 dipdup-7.0.0rc3/tests/replays/739d17c86095aac3da3508a16dc1c9ae9459ea86eeb09f62aaefc32de2997918
+-rw-r--r--   0        0        0        2 2023-08-05 20:31:43.799344 dipdup-7.0.0rc3/tests/replays/759b79ec12b1305d9fa8e1a5218e62bb3d3ad913580e19914d30d8aa09920ae4
+-rw-r--r--   0        0        0   209456 2023-08-05 20:28:16.666350 dipdup-7.0.0rc3/tests/replays/7669ea717d9759748aed86302326b79be5157a1a36d13b39b00f06bcbe22b309
+-rw-r--r--   0        0        0      520 2023-08-05 20:28:16.666350 dipdup-7.0.0rc3/tests/replays/76d49ae3b723376c88ca65a3080a273e098d226932a1a49c38fbc4421e7c2e64
+-rw-r--r--   0        0        0    50588 2023-08-05 20:31:14.894890 dipdup-7.0.0rc3/tests/replays/7b6cf9b8c69712bf26ed09059352ec740606969bf20eab0dedda870273f4fde9
+-rw-r--r--   0        0        0 21649088 2023-08-05 20:31:18.310957 dipdup-7.0.0rc3/tests/replays/7b9c78209f98b2c3a6678ed224fa686eee25c3c63dddd7f9af77c734b0dfabb8
+-rw-r--r--   0        0        0      807 2023-08-05 20:31:42.047311 dipdup-7.0.0rc3/tests/replays/803e05a8d0bb9e7cfb49530271d43ea62111b6419e7cded2d221f7e0e0c92ece
+-rw-r--r--   0        0        0   517204 2023-08-05 20:28:16.666350 dipdup-7.0.0rc3/tests/replays/80921fd33043def891912a6ad57d76664399564fd813950eb11f4a0e69e3e28f
+-rw-r--r--   0        0        0      129 2023-08-05 20:28:16.666350 dipdup-7.0.0rc3/tests/replays/815c066c21f7d2697ef107cad4624a9c4079a7a1dab7974d606fc42b81fe93c8
+-rw-r--r--   0        0        0      939 2023-08-05 20:28:16.666350 dipdup-7.0.0rc3/tests/replays/816d08f71c84537ea8df05a40678b1addca15bf3a73c0e927c75d9f9c0f2d418
+-rw-r--r--   0        0        0      395 2023-08-05 20:31:41.767306 dipdup-7.0.0rc3/tests/replays/8335acc6585656ec3a4301cd8b089401f2dc2c7d758b381c96c730e610b67f7b
+-rw-r--r--   0        0        0   207502 2023-08-05 20:28:16.666350 dipdup-7.0.0rc3/tests/replays/84cf46aa9c8dbd3ca6c3d946c749713e6c70a6a20d9cc69b4156235fd099b2e3
+-rw-r--r--   0        0        0        2 2023-08-05 20:28:16.666350 dipdup-7.0.0rc3/tests/replays/8ad31f6cf9c873b1fd9827b621529c43966f8376a86fcac3b1d20c260b78007e
+-rw-r--r--   0        0        0       65 2023-08-05 20:28:16.666350 dipdup-7.0.0rc3/tests/replays/91787fdbd1634f277b20ac46cb30eba9770f83df7189df0903e22f5f4bbe1efa
+-rw-r--r--   0        0        0     1151 2023-08-05 20:31:42.715322 dipdup-7.0.0rc3/tests/replays/93516225810a23a6799f2f9a1dee055ca79a66ee2b8d0f32be820c9c385e936b
+-rw-r--r--   0        0        0      494 2023-08-05 20:28:16.666350 dipdup-7.0.0rc3/tests/replays/9ce1bc12a2adeddcf9d8854c4b63a8e65b58d9206fb8d2e3eedb24c44ea7f28a
+-rw-r--r--   0        0        0       22 2023-08-05 20:28:16.666350 dipdup-7.0.0rc3/tests/replays/9de859083ed1dd278893f60b5a60feab02a04637327a664af23f52dabb139fe6
+-rw-r--r--   0        0        0      706 2023-08-05 20:28:16.666350 dipdup-7.0.0rc3/tests/replays/9e6e907842da2cd494c558ea5ecc211fd12e56bfc547450978fb7dfe03853e58
+-rw-r--r--   0        0        0     6981 2023-08-05 20:28:16.666350 dipdup-7.0.0rc3/tests/replays/a3ce91a1b0d505cc221f0e201781466ba1e2d6dc7b624b9bc75a03ce3dbb0f92
+-rw-r--r--   0        0        0    38974 2023-08-05 20:28:16.666350 dipdup-7.0.0rc3/tests/replays/a795ef429bde71b3ba66b545c0048f57a78ab5d2247772761d8efe86567199b9
+-rw-r--r--   0        0        0        2 2023-08-05 20:28:16.666350 dipdup-7.0.0rc3/tests/replays/a840afa5674efd06639c4692a8bfe9ed6e1346bfe9c414209eec5d9126333242
+-rw-r--r--   0        0        0      675 2023-08-05 20:28:16.666350 dipdup-7.0.0rc3/tests/replays/aa8fe6037996b296bf9a3011e45cd9ecb92fb728592a843f91b03b2848cb1fb1
+-rw-r--r--   0        0        0     1882 2023-08-05 20:31:08.174754 dipdup-7.0.0rc3/tests/replays/acc952ba1905717315212f952ed689d7b8f683165b31c0a7a25199aed9fda27f
+-rw-r--r--   0        0        0      356 2023-08-05 20:28:16.666350 dipdup-7.0.0rc3/tests/replays/aeee37b6f63a3177e0e27ac472008c3cba3d30ebee691fb45de1bae91a87f2ce
+-rw-r--r--   0        0        0       67 2023-08-05 20:31:36.707221 dipdup-7.0.0rc3/tests/replays/af37212b31e932f269c42c7f34ad8f3849bd8aed244652c41b9327c508985ce5
+-rw-r--r--   0        0        0     1200 2023-08-05 20:31:39.935275 dipdup-7.0.0rc3/tests/replays/b3af887f7ad8172af75b94a09bedfb9ae1e14f8819a36d6ce9f709721068263b
+-rw-r--r--   0        0        0  1214926 2023-08-05 20:30:47.514357 dipdup-7.0.0rc3/tests/replays/b49fb33ee80345b70414ad08806a860e2139c20d98a5150c6ccd1b28a90f311e
+-rw-r--r--   0        0        0     2271 2023-08-05 20:31:38.643253 dipdup-7.0.0rc3/tests/replays/bec4433b4206f00c2310a7961cff7f539434b9161b45673793aa5a3b50234313
+-rw-r--r--   0        0        0      310 2023-08-05 20:28:16.666350 dipdup-7.0.0rc3/tests/replays/bed2329e63d559db2fb81c69606e715d1f90aaacab6ae45b33516e7828841a3c
+-rw-r--r--   0        0        0       65 2023-08-05 20:28:16.666350 dipdup-7.0.0rc3/tests/replays/bf941ceae7a6e3c40406438e067f137131e6605924a93d43bafc77682b602c55
+-rw-r--r--   0        0        0   759209 2023-08-05 20:30:47.630359 dipdup-7.0.0rc3/tests/replays/c0202a433296436c27458b3d5ec5c72d5e2d47ff77c939ce399780cc0f3e56bc
+-rw-r--r--   0        0        0    19100 2023-08-05 20:28:16.670350 dipdup-7.0.0rc3/tests/replays/c369836c15d9ed15477002b850d5cbb96b1ff5ff33e917b812ab9c0905063957
+-rw-r--r--   0        0        0   918908 2023-08-05 20:28:16.670350 dipdup-7.0.0rc3/tests/replays/c8e8698717ada415bc10405da983c8357165914dd0219f3d09bb9a939705242d
+-rw-r--r--   0        0        0   691878 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/replays/cc162df04c4990c79f7507dd915601fd4d58c947a248156cbe302a64adfe898a
+-rw-r--r--   0        0        0     7446 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/replays/cc5d3d4a58d5cb6bc7270d38c797b7740b79f913590ef0164abd50e58fba9405
+-rw-r--r--   0        0        0      301 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/replays/cc648800928fd43f8e72db1d41115c26a22346c9c7831172fe422c1765cd67f2
+-rw-r--r--   0        0        0      960 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/replays/d0a594d14bcb3fbf916092ec6707dfd3c9f48f53f0a1ad40a32023e7a87f8ef5
+-rw-r--r--   0        0        0     2403 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/replays/d62748a927a09395579b5790c8f871cc8653081cf4475abc93173989f950b92b
+-rw-r--r--   0        0        0     9089 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/replays/d94397f6ecec8ce25f87177fe410f6498d7d30a04360506c0cd300d291c167e7
+-rw-r--r--   0        0        0      132 2023-08-05 20:31:35.915207 dipdup-7.0.0rc3/tests/replays/db797e6bf4c1b9c3237af5dec694fb1b6d21418a5a2f7947eb7f54d4e9201baf
+-rw-r--r--   0        0        0   548925 2023-08-05 20:31:18.614963 dipdup-7.0.0rc3/tests/replays/dc86d5e346c85e6f7953d7e01298a9db64d778e5ba717ddd07fff8b589081e98
+-rw-r--r--   0        0        0    20467 2023-08-05 20:30:35.482113 dipdup-7.0.0rc3/tests/replays/dca9cf4f9f27623f10975d369444899458ab9ea85c22af2da6ce6ce8c09c2b58
+-rw-r--r--   0        0        0      700 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/replays/df62701276d6dbf4860058cc582c0b4f7b583758f4f5be96c9ee045757c151e3
+-rw-r--r--   0        0        0   151396 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/replays/e39ebba701031aa13dfd9eb5dba1effd2938e96682d1030dcbd70172f9f190a9
+-rw-r--r--   0        0        0     7917 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/replays/e4a563a0b19379a44e9d2dc398131e9fd30d6039ff4ffacf1252db0bf8b433aa
+-rw-r--r--   0        0        0       67 2023-08-05 20:31:37.091227 dipdup-7.0.0rc3/tests/replays/e82ba90c8570b92c0b1fc360b853aca3f1d7de457aacb9f6f19fa3e43879a8b3
+-rw-r--r--   0        0        0      132 2023-08-05 20:31:36.043210 dipdup-7.0.0rc3/tests/replays/e9fa56a94eb559c550dfbca4b27ef350a0b4a787afbe60205482a38223dcea04
+-rw-r--r--   0        0        0   713738 2023-08-05 20:31:39.711271 dipdup-7.0.0rc3/tests/replays/eb8b6b33cb2e165d1a3a73c09938d3083671a82ad73d4c0cff1fb2a5e5715f76
+-rw-r--r--   0        0        0    11290 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/replays/eb8e2c3ce2fe7792d2c8e81c61d37821275b64021343103b0c955042ae802189
+-rw-r--r--   0        0        0      584 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/replays/ece1ebe13f9391555230d6b94f33d66a922e2ca71ef5fd39bbd8c2c37ddf54ec
+-rw-r--r--   0        0        0     1089 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/replays/ed3ec9fd9226e9f765b96dc1d5d5a455a7b2505da530961826910b08db693070
+-rw-r--r--   0        0        0    17245 2023-08-05 20:31:19.366969 dipdup-7.0.0rc3/tests/replays/f3d608f99e6b92e28a064bb9c10c3c605c9c817383c1eebcc68f663d1d23d650
+-rw-r--r--   0        0        0    32513 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/replays/f60e794a9be14263cb10e48546ba5610302cc3e7af0a114a593bb50eb85ba5e7
+-rw-r--r--   0        0        0       21 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/replays/fd9e33296006ad295c9fdc4868763f954a9c6d7c81d543ba198c14a72eea7e6b
+-rw-r--r--   0        0        0      832 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/replays/ff51b3535acc2972090ecd5db3af8f827464c9d92f1aa661630976e5b4ed4cbe
+-rw-r--r--   0        0        0     4599 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/responses/asdf.json
+-rw-r--r--   0        0        0     6704 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/responses/ftzfun.json
+-rw-r--r--   0        0        0     3445 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/responses/hen_subjkt.json
+-rw-r--r--   0        0        0     5210 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/responses/hjkl.json
+-rw-r--r--   0        0        0     2097 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/responses/kolibri_ovens.json
+-rw-r--r--   0        0        0    11186 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/responses/ooQuCAKBHkmWy2VciDAV9c6CFTywuMLupLzVoKDwS1xvR4EdRng.json
+-rw-r--r--   0        0        0     1811 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/responses/origination_amount.json
+-rw-r--r--   0        0        0     4256 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/responses/qwer.json
+-rw-r--r--   0        0        0     5307 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/responses/rewq.json
+-rw-r--r--   0        0        0    38178 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/responses/yupana.json
+-rw-r--r--   0        0        0     5909 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/responses/zxcv.json
+-rw-r--r--   0        0        0     1077 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/schemas/asdf/storage.json
+-rw-r--r--   0        0        0     2116 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/schemas/hen_subjkt/storage.json
+-rw-r--r--   0        0        0     1638 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/schemas/hjkl/storage.json
+-rw-r--r--   0        0        0      800 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/schemas/kolibri_ovens/storage.json
+-rw-r--r--   0        0        0     1005 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/schemas/qwer/storage.json
+-rw-r--r--   0        0        0     2212 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/schemas/rewq/storage.json
+-rw-r--r--   0        0        0    12561 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/schemas/yupana/storage.json
+-rw-r--r--   0        0        0     2660 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/schemas/zxcv/storage.json
+-rw-r--r--   0        0        0     3767 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/test_config/test_callbacks.py
+-rw-r--r--   0        0        0     4643 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/test_config/test_config.py
+-rw-r--r--   0        0        0     4138 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/test_config/test_custom_config.py
+-rw-r--r--   0        0        0     2486 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/test_context.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/test_datasources/__init__.py
+-rw-r--r--   0        0        0      814 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/test_datasources/test_ipfs.py
+-rw-r--r--   0        0        0      663 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/test_datasources/test_metadata.py
+-rw-r--r--   0        0        0     8304 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/test_datasources/test_tzkt.py
+-rw-r--r--   0        0        0     1223 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/test_datasources/test_tzkt_blocks.py
+-rw-r--r--   0        0        0     1971 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/test_datasources/test_tzkt_buffer.py
+-rw-r--r--   0        0        0     1433 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/test_datasources/test_tzkt_quotes.py
+-rw-r--r--   0        0        0     8700 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/test_demos.py
+-rw-r--r--   0        0        0     2734 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/test_dipdup.py
+-rw-r--r--   0        0        0     5045 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/test_hasura.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/test_http.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/test_index/__init__.py
+-rw-r--r--   0        0        0     3714 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/test_index/test_operation.py
+-rw-r--r--   0        0        0     5772 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/test_introspection.py
+-rw-r--r--   0        0        0    14279 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/test_models.py
+-rw-r--r--   0        0        0    13401 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/test_rollback.py
+-rw-r--r--   0        0        0     2628 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/types/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/types/asdf/__init__.py
+-rw-r--r--   0        0        0      504 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/types/asdf/storage.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/types/bazaar/__init__.py
+-rw-r--r--   0        0        0      564 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/types/bazaar/storage.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/types/ftzfun/__init__.py
+-rw-r--r--   0        0        0      929 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/types/ftzfun/storage.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/types/hen_subjkt/__init__.py
+-rw-r--r--   0        0        0      583 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/types/hen_subjkt/storage.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/types/hjkl/__init__.py
+-rw-r--r--   0        0        0      647 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/types/hjkl/storage.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/types/kolibri_ovens/__init__.py
+-rw-r--r--   0        0        0      232 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/types/kolibri_ovens/set_delegate.py
+-rw-r--r--   0        0        0      392 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/types/kolibri_ovens/storage.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/types/listofmaps/__init__.py
+-rw-r--r--   0        0        0      153 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/types/listofmaps/storage.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/types/qwer/__init__.py
+-rw-r--r--   0        0        0      532 2023-08-05 20:28:16.674350 dipdup-7.0.0rc3/tests/types/qwer/storage.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.678350 dipdup-7.0.0rc3/tests/types/rewq/__init__.py
+-rw-r--r--   0        0        0      831 2023-08-05 20:28:16.678350 dipdup-7.0.0rc3/tests/types/rewq/storage.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.678350 dipdup-7.0.0rc3/tests/types/tezotop/__init__.py
+-rw-r--r--   0        0        0      740 2023-08-05 20:28:16.678350 dipdup-7.0.0rc3/tests/types/tezotop/storage.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.678350 dipdup-7.0.0rc3/tests/types/yupana/__init__.py
+-rw-r--r--   0        0        0     2721 2023-08-05 20:28:16.678350 dipdup-7.0.0rc3/tests/types/yupana/storage.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:28:16.678350 dipdup-7.0.0rc3/tests/types/zxcv/__init__.py
+-rw-r--r--   0        0        0     1048 2023-08-05 20:28:16.678350 dipdup-7.0.0rc3/tests/types/zxcv/storage.py
+-rw-r--r--   0        0        0     5756 1970-01-01 00:00:00.000000 dipdup-7.0.0rc3/PKG-INFO
```

### Comparing `dipdup-7.0.0rc2/LICENSE` & `dipdup-7.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/README.md` & `dipdup-7.0.0rc3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 - **Ready to build your first indexer?** Head to [Quickstart](https://dipdup.io/docs/quickstart).
 
 - **Looking for examples?** Check out [Demo Projects](https://dipdup.io/docs/examples/demos) and [Built with DipDup](https://dipdup.io/docs/examples/built-with-dipdup) pages.
 
 - **Want to participate?** Vote for [open issues](https://github.com/dipdup-io/dipdup/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc), join [discussions](https://github.com/dipdup-io/dipdup/discussions) or [become a sponsor](https://github.com/sponsors/dipdup-io).
 
-- **Have a question?** Join our [Discord](https://discord.gg/NbANhqCJHA) or tag @dipdup_io on [Twitter](https://twitter.com/dipdup_io).
+- **Have a question?** Join our [Discord](https://discord.gg/aG8XKuwsQd) or tag @dipdup_io on [Twitter](https://twitter.com/dipdup_io).
 
 This project is maintained by the [Baking Bad](https://bakingbad.dev/) team.
 <br>
 Development is supported by [Tezos Foundation](https://tezos.foundation/) and [OnlyDust](https://www.onlydust.xyz).
 
 ## Thanks
```

### Comparing `dipdup-7.0.0rc2/pyproject.toml` & `dipdup-7.0.0rc3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "dipdup"
 description = "Modular framework for creating selective indexers and featureful backends for dapps"
-version = "7.0.0rc2"
+version = "7.0.0rc3"
 authors = [
     { name = "Lev Gorodetskii", email = "dipdup@drsr.io" },
     { name = "Vladimir Bobrikov", email = "vladimir_bobrikov@pm.me" },
     { name = "Michael Zaikin", email = "mz@baking-bad.org" },
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
@@ -41,15 +41,15 @@
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Typing :: Typed",
 ]
 dependencies = [
     "asyncpg~=0.28.0",
     "datamodel-code-generator~=0.21.1",
     "pydantic~=1.10.11",
-    "tortoise-orm===0.19.3",
+    "tortoise-orm==0.19.3",
     "aiohttp~=3.8",
     "aiolimiter~=1.0",
     "anyio~=3.3",
     "APScheduler~=3.8",
     "async-lru~=2.0",
     "asyncclick~=8.0",
     "eth-abi~=4.0",
@@ -57,15 +57,15 @@
     "prometheus-client~=0.17",
     "pyarrow~=12.0",
     "pycryptodome~=3.17",
     "pyhumps~=3.0",
     "pysignalr~=0.2",
     "python-dotenv~=1.0",
     "ruamel.yaml~=0.17",
-    "sentry-sdk~=1.4",
+    "sentry-sdk~=1.29",
     "sqlparse~=0.4",
     "survey~=4.4",
     "tabulate~=0.9",
     "web3~=6.2",
 ]
 
 [project.license]
```

### Comparing `dipdup-7.0.0rc2/src/demo_auction/README.md` & `dipdup-7.0.0rc3/src/demo_auction/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
 pdm install
-pdm venv activate
+$(pdm venv activate)
 ```
 
 Some tools are included to help you keep the code quality high: black, ruff and mypy.
 
 ```bash
 # Format code
 pdm fmt
```

### Comparing `dipdup-7.0.0rc2/src/demo_auction/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc3/src/demo_auction/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_auction/deploy/compose.yaml` & `dipdup-7.0.0rc3/src/demo_auction/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_auction/dipdup.yaml` & `dipdup-7.0.0rc3/src/demo_auction/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_auction/handlers/on_bid.py` & `dipdup-7.0.0rc3/src/demo_auction/handlers/on_bid.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_auction/handlers/on_create_auction.py` & `dipdup-7.0.0rc3/src/demo_auction/handlers/on_create_auction.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_auction/handlers/on_withdraw.py` & `dipdup-7.0.0rc3/src/demo_auction/handlers/on_withdraw.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_auction/models/__init__.py` & `dipdup-7.0.0rc3/src/demo_auction/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_auction/pyproject.toml` & `dipdup-7.0.0rc3/src/demo_auction/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc2,<8"
+    "dipdup>=7.0.0rc3,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
```

### Comparing `dipdup-7.0.0rc2/src/demo_auction/types/tzcolors_auction/tezos_storage.py` & `dipdup-7.0.0rc3/src/demo_auction/types/tzcolors_auction/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_big_maps/README.md` & `dipdup-7.0.0rc3/src/demo_big_maps/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
 pdm install
-pdm venv activate
+$(pdm venv activate)
 ```
 
 Some tools are included to help you keep the code quality high: black, ruff and mypy.
 
 ```bash
 # Format code
 pdm fmt
```

### Comparing `dipdup-7.0.0rc2/src/demo_big_maps/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc3/src/demo_big_maps/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_big_maps/deploy/compose.yaml` & `dipdup-7.0.0rc3/src/demo_big_maps/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_big_maps/dipdup.yaml` & `dipdup-7.0.0rc3/src/demo_big_maps/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_big_maps/handlers/on_update_expiry_map.py` & `dipdup-7.0.0rc3/src/demo_big_maps/handlers/on_update_expiry_map.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_big_maps/handlers/on_update_records.py` & `dipdup-7.0.0rc3/src/demo_big_maps/handlers/on_update_records.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_big_maps/models/__init__.py` & `dipdup-7.0.0rc3/src/demo_big_maps/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_big_maps/pyproject.toml` & `dipdup-7.0.0rc3/src/demo_big_maps/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc2,<8"
+    "dipdup>=7.0.0rc3,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
```

### Comparing `dipdup-7.0.0rc2/src/demo_blank/README.md` & `dipdup-7.0.0rc3/src/demo_domains/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# demo_blank
+# demo_domains
 
-Empty config for a fresh start
+Tezos Domains name service
 
 ## Installation
 
 This project is based on [DipDup](https://dipdup.io), a framework for building featureful dapps.
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
@@ -38,15 +38,15 @@
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
 pdm install
-pdm venv activate
+$(pdm venv activate)
 ```
 
 Some tools are included to help you keep the code quality high: black, ruff and mypy.
 
 ```bash
 # Format code
 pdm fmt
```

### Comparing `dipdup-7.0.0rc2/src/demo_blank/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc3/src/demo_blank/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_blank/deploy/compose.yaml` & `dipdup-7.0.0rc3/src/demo_blank/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_blank/models/__init__.py` & `dipdup-7.0.0rc3/src/demo_blank/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import enum
 
 from dipdup import fields
-from dipdup import models
+from dipdup.models import Model
 
 
-class ExampleModel(models.Model):
+class ExampleModel(Model):
     id = fields.IntField(pk=True)
     array = fields.ArrayField()
     big_int = fields.BigIntField()
     binary = fields.BinaryField()
     boolean = fields.BooleanField()
     decimal = fields.DecimalField(10, 2)
     date = fields.DateField()
```

### Comparing `dipdup-7.0.0rc2/src/demo_blank/pyproject.toml` & `dipdup-7.0.0rc3/src/demo_raw/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
-name = "demo_blank"
+name = "demo_raw"
 version = "0.0.1"
-description = "Empty config for a fresh start"
+description = "Process raw operations without filtering and strict typing"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc2,<8"
+    "dipdup>=7.0.0rc3,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
@@ -24,15 +24,15 @@
 _isort = "isort ."
 _black = "black ."
 _ruff = "ruff check --fix ."
 _mypy = "mypy ."
 all = { composite = ["fmt", "lint"] }
 fmt = { composite = ["_isort", "_black"] }
 lint = { composite = ["_ruff", "_mypy"] }
-image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_blank:latest"
+image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_raw:latest"
 
 [tool.isort]
 line_length = 120
 force_single_line = true
 
 [tool.black]
 line-length = 120
```

### Comparing `dipdup-7.0.0rc2/src/demo_dao/README.md` & `dipdup-7.0.0rc3/src/demo_raw/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# demo_dao
+# demo_raw
 
-Homebase DAO registry
+Process raw operations without filtering and strict typing
 
 ## Installation
 
 This project is based on [DipDup](https://dipdup.io), a framework for building featureful dapps.
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
@@ -38,15 +38,15 @@
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
 pdm install
-pdm venv activate
+$(pdm venv activate)
 ```
 
 Some tools are included to help you keep the code quality high: black, ruff and mypy.
 
 ```bash
 # Format code
 pdm fmt
```

### Comparing `dipdup-7.0.0rc2/src/demo_dao/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc3/src/demo_dao/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dao/deploy/compose.yaml` & `dipdup-7.0.0rc3/src/demo_dao/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dao/dipdup.yaml` & `dipdup-7.0.0rc3/src/demo_dao/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dao/models/__init__.py` & `dipdup-7.0.0rc3/src/demo_dao/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dao/pyproject.toml` & `dipdup-7.0.0rc3/src/demo_head/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
-name = "demo_dao"
+name = "demo_head"
 version = "0.0.1"
-description = "Homebase DAO registry"
+description = "Processing head block metadata"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc2,<8"
+    "dipdup>=7.0.0rc3,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
@@ -24,15 +24,15 @@
 _isort = "isort ."
 _black = "black ."
 _ruff = "ruff check --fix ."
 _mypy = "mypy ."
 all = { composite = ["fmt", "lint"] }
 fmt = { composite = ["_isort", "_black"] }
 lint = { composite = ["_ruff", "_mypy"] }
-image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_dao:latest"
+image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_head:latest"
 
 [tool.isort]
 line_length = 120
 force_single_line = true
 
 [tool.black]
 line-length = 120
```

### Comparing `dipdup-7.0.0rc2/src/demo_dao/types/registry/tezos_storage.py` & `dipdup-7.0.0rc3/src/demo_dao/types/registry/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dex/README.md` & `dipdup-7.0.0rc3/src/demo_dex/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
 pdm install
-pdm venv activate
+$(pdm venv activate)
 ```
 
 Some tools are included to help you keep the code quality high: black, ruff and mypy.
 
 ```bash
 # Format code
 pdm fmt
```

### Comparing `dipdup-7.0.0rc2/src/demo_dex/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc3/src/demo_dex/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dex/deploy/compose.yaml` & `dipdup-7.0.0rc3/src/demo_dex/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dex/dipdup.yaml` & `dipdup-7.0.0rc3/src/demo_dex/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_divest_liquidity.py` & `dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa12_divest_liquidity.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_invest_liquidity.py` & `dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa12_invest_liquidity.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_origination.py` & `dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa12_origination.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_tez_to_token.py` & `dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa12_tez_to_token.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_token_to_tez.py` & `dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa12_token_to_tez.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_transfer.py` & `dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa12_transfer.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_withdraw_profit.py` & `dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa12_withdraw_profit.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_divest_liquidity.py` & `dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa2_divest_liquidity.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_invest_liquidity.py` & `dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa2_invest_liquidity.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_origination.py` & `dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa2_origination.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_tez_to_token.py` & `dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa2_tez_to_token.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_token_to_tez.py` & `dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa2_token_to_tez.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_transfer.py` & `dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa2_transfer.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_withdraw_profit.py` & `dipdup-7.0.0rc3/src/demo_dex/handlers/on_fa2_withdraw_profit.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dex/models/__init__.py` & `dipdup-7.0.0rc3/src/demo_dex/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dex/pyproject.toml` & `dipdup-7.0.0rc3/src/demo_dex/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc2,<8"
+    "dipdup>=7.0.0rc3,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
```

### Comparing `dipdup-7.0.0rc2/src/demo_dex/types/fa12_token/tezos_storage.py` & `dipdup-7.0.0rc3/src/demo_dex/types/fa12_token/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dex/types/fa2_token/tezos_storage.py` & `dipdup-7.0.0rc3/src/demo_dex/types/fa2_token/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa12/tezos_storage.py` & `dipdup-7.0.0rc3/src/demo_dex/types/quipu_fa12/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa2/tezos_storage.py` & `dipdup-7.0.0rc3/src/demo_dex/types/quipu_fa2/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_domains/README.md` & `dipdup-7.0.0rc3/src/dipdup/projects/base/README.md.j2`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# demo_domains
+# {{project.package}}
 
-Tezos Domains name service
+{{project.description}}
 
 ## Installation
 
 This project is based on [DipDup](https://dipdup.io), a framework for building featureful dapps.
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
@@ -38,15 +38,15 @@
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
 pdm install
-pdm venv activate
+$(pdm venv activate)
 ```
 
 Some tools are included to help you keep the code quality high: black, ruff and mypy.
 
 ```bash
 # Format code
 pdm fmt
@@ -54,8 +54,8 @@
 # Lint code
 pdm lint
 
 # Build Docker image
 pdm image
 ```
 
-Inspect the `pyproject.toml` file. It contains all the dependencies and tools used in the project.
+Inspect the `pyproject.toml` file. It contains all the dependencies and tools used in the project.
```

### Comparing `dipdup-7.0.0rc2/src/demo_domains/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc3/src/demo_domains/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_domains/deploy/compose.yaml` & `dipdup-7.0.0rc3/src/demo_domains/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_domains/dipdup.yaml` & `dipdup-7.0.0rc3/src/demo_domains/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_domains/handlers/on_admin_update.py` & `dipdup-7.0.0rc3/src/demo_domains/handlers/on_admin_update.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_domains/handlers/on_execute.py` & `dipdup-7.0.0rc3/src/demo_domains/handlers/on_execute.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_domains/handlers/on_storage_diff.py` & `dipdup-7.0.0rc3/src/demo_domains/handlers/on_storage_diff.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_domains/models/__init__.py` & `dipdup-7.0.0rc3/src/demo_domains/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_domains/pyproject.toml` & `dipdup-7.0.0rc3/src/demo_nft_marketplace/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
-name = "demo_domains"
+name = "demo_nft_marketplace"
 version = "0.0.1"
-description = "Tezos Domains name service"
+description = "hic at nunc NFT marketplace"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc2,<8"
+    "dipdup>=7.0.0rc3,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
@@ -24,15 +24,15 @@
 _isort = "isort ."
 _black = "black ."
 _ruff = "ruff check --fix ."
 _mypy = "mypy ."
 all = { composite = ["fmt", "lint"] }
 fmt = { composite = ["_isort", "_black"] }
 lint = { composite = ["_ruff", "_mypy"] }
-image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_domains:latest"
+image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_nft_marketplace:latest"
 
 [tool.isort]
 line_length = 120
 force_single_line = true
 
 [tool.black]
 line-length = 120
```

### Comparing `dipdup-7.0.0rc2/src/demo_domains/types/name_registry/tezos_storage.py` & `dipdup-7.0.0rc3/src/demo_domains/types/name_registry/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_events/README.md` & `dipdup-7.0.0rc3/src/demo_events/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
 pdm install
-pdm venv activate
+$(pdm venv activate)
 ```
 
 Some tools are included to help you keep the code quality high: black, ruff and mypy.
 
 ```bash
 # Format code
 pdm fmt
```

### Comparing `dipdup-7.0.0rc2/src/demo_events/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc3/src/demo_events/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_events/deploy/compose.yaml` & `dipdup-7.0.0rc3/src/demo_events/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_events/dipdup.yaml` & `dipdup-7.0.0rc3/src/demo_events/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_events/models/__init__.py` & `dipdup-7.0.0rc3/src/demo_events/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import enum
 
 from dipdup import fields
-from dipdup import models
+from dipdup.models import Model
 
 
-class ExampleModel(models.Model):
+class ExampleModel(Model):
     id = fields.IntField(pk=True)
     array = fields.ArrayField()
     big_int = fields.BigIntField()
     binary = fields.BinaryField()
     boolean = fields.BooleanField()
     decimal = fields.DecimalField(10, 2)
     date = fields.DateField()
```

### Comparing `dipdup-7.0.0rc2/src/demo_events/pyproject.toml` & `dipdup-7.0.0rc3/src/demo_events/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc2,<8"
+    "dipdup>=7.0.0rc3,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
```

### Comparing `dipdup-7.0.0rc2/src/demo_evm_events/README.md` & `dipdup-7.0.0rc3/src/demo_factories/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# demo_evm_events
+# demo_factories
 
 A very basic indexer for USDt transfers
 
 ## Installation
 
 This project is based on [DipDup](https://dipdup.io), a framework for building featureful dapps.
 
@@ -38,15 +38,15 @@
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
 pdm install
-pdm venv activate
+$(pdm venv activate)
 ```
 
 Some tools are included to help you keep the code quality high: black, ruff and mypy.
 
 ```bash
 # Format code
 pdm fmt
```

### Comparing `dipdup-7.0.0rc2/src/demo_evm_events/abi/eth_usdt/abi.json` & `dipdup-7.0.0rc3/src/demo_evm_events/abi/eth_usdt/abi.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_evm_events/abi/eth_usdt/events.json` & `dipdup-7.0.0rc3/src/demo_evm_events/abi/eth_usdt/events.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_evm_events/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc3/src/demo_evm_events/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_evm_events/deploy/compose.yaml` & `dipdup-7.0.0rc3/src/demo_evm_events/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_evm_events/dipdup.yaml` & `dipdup-7.0.0rc3/src/demo_evm_events/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_evm_events/handlers/on_transfer.py` & `dipdup-7.0.0rc3/src/demo_evm_events/handlers/on_transfer.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_evm_events/pyproject.toml` & `dipdup-7.0.0rc3/src/demo_evm_events/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc2,<8"
+    "dipdup>=7.0.0rc3,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
```

### Comparing `dipdup-7.0.0rc2/src/demo_factories/README.md` & `dipdup-7.0.0rc3/src/demo_token_transfers/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# demo_factories
+# demo_token_transfers
 
-A very basic indexer for USDt transfers
+TzBTC FA1.2 token transfers
 
 ## Installation
 
 This project is based on [DipDup](https://dipdup.io), a framework for building featureful dapps.
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
@@ -38,15 +38,15 @@
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
 pdm install
-pdm venv activate
+$(pdm venv activate)
 ```
 
 Some tools are included to help you keep the code quality high: black, ruff and mypy.
 
 ```bash
 # Format code
 pdm fmt
```

### Comparing `dipdup-7.0.0rc2/src/demo_factories/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc3/src/demo_factories/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_factories/deploy/compose.yaml` & `dipdup-7.0.0rc3/src/demo_factories/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_factories/dipdup.yaml` & `dipdup-7.0.0rc3/src/demo_factories/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_factories/handlers/on_propose.py` & `dipdup-7.0.0rc3/src/demo_factories/handlers/on_propose.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_factories/models/__init__.py` & `dipdup-7.0.0rc3/src/demo_factories/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_factories/pyproject.toml` & `dipdup-7.0.0rc3/src/demo_factories/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc2,<8"
+    "dipdup>=7.0.0rc3,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
```

### Comparing `dipdup-7.0.0rc2/src/demo_factories/types/registry/tezos_storage.py` & `dipdup-7.0.0rc3/src/demo_factories/types/registry/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_head/README.md` & `dipdup-7.0.0rc3/src/demo_nft_marketplace/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# demo_head
+# demo_nft_marketplace
 
-Processing head block metadata
+hic at nunc NFT marketplace
 
 ## Installation
 
 This project is based on [DipDup](https://dipdup.io), a framework for building featureful dapps.
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
@@ -38,15 +38,15 @@
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
 pdm install
-pdm venv activate
+$(pdm venv activate)
 ```
 
 Some tools are included to help you keep the code quality high: black, ruff and mypy.
 
 ```bash
 # Format code
 pdm fmt
```

### Comparing `dipdup-7.0.0rc2/src/demo_head/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc3/src/demo_head/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_head/deploy/compose.yaml` & `dipdup-7.0.0rc3/src/demo_head/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_head/models/__init__.py` & `dipdup-7.0.0rc3/src/demo_head/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import enum
 
 from dipdup import fields
-from dipdup import models
+from dipdup.models import Model
 
 
-class ExampleModel(models.Model):
+class ExampleModel(Model):
     id = fields.IntField(pk=True)
     array = fields.ArrayField()
     big_int = fields.BigIntField()
     binary = fields.BinaryField()
     boolean = fields.BooleanField()
     decimal = fields.DecimalField(10, 2)
     date = fields.DateField()
```

### Comparing `dipdup-7.0.0rc2/src/demo_head/pyproject.toml` & `dipdup-7.0.0rc3/src/demo_dao/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
-name = "demo_head"
+name = "demo_dao"
 version = "0.0.1"
-description = "Processing head block metadata"
+description = "Homebase DAO registry"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc2,<8"
+    "dipdup>=7.0.0rc3,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
@@ -24,15 +24,15 @@
 _isort = "isort ."
 _black = "black ."
 _ruff = "ruff check --fix ."
 _mypy = "mypy ."
 all = { composite = ["fmt", "lint"] }
 fmt = { composite = ["_isort", "_black"] }
 lint = { composite = ["_ruff", "_mypy"] }
-image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_head:latest"
+image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_dao:latest"
 
 [tool.isort]
 line_length = 120
 force_single_line = true
 
 [tool.black]
 line-length = 120
```

### Comparing `dipdup-7.0.0rc2/src/demo_nft_marketplace/README.md` & `dipdup-7.0.0rc3/src/demo_evm_events/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# demo_nft_marketplace
+# demo_evm_events
 
-hic at nunc NFT marketplace
+A very basic indexer for USDt transfers
 
 ## Installation
 
 This project is based on [DipDup](https://dipdup.io), a framework for building featureful dapps.
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
@@ -38,15 +38,15 @@
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
 pdm install
-pdm venv activate
+$(pdm venv activate)
 ```
 
 Some tools are included to help you keep the code quality high: black, ruff and mypy.
 
 ```bash
 # Format code
 pdm fmt
```

### Comparing `dipdup-7.0.0rc2/src/demo_nft_marketplace/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc3/src/demo_nft_marketplace/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_nft_marketplace/deploy/compose.yaml` & `dipdup-7.0.0rc3/src/demo_nft_marketplace/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_nft_marketplace/dipdup.yaml` & `dipdup-7.0.0rc3/src/demo_nft_marketplace/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_nft_marketplace/handlers/on_cancel_swap.py` & `dipdup-7.0.0rc3/src/demo_nft_marketplace/handlers/on_cancel_swap.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_nft_marketplace/handlers/on_collect.py` & `dipdup-7.0.0rc3/src/demo_nft_marketplace/handlers/on_collect.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_nft_marketplace/handlers/on_mint.py` & `dipdup-7.0.0rc3/src/demo_nft_marketplace/handlers/on_mint.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_nft_marketplace/handlers/on_swap.py` & `dipdup-7.0.0rc3/src/demo_nft_marketplace/handlers/on_swap.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_nft_marketplace/models/__init__.py` & `dipdup-7.0.0rc3/src/demo_nft_marketplace/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_nft_marketplace/pyproject.toml` & `dipdup-7.0.0rc3/src/demo_token_transfers/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
-name = "demo_nft_marketplace"
+name = "demo_token_transfers"
 version = "0.0.1"
-description = "hic at nunc NFT marketplace"
+description = "TzBTC FA1.2 token transfers"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc2,<8"
+    "dipdup>=7.0.0rc3,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
@@ -24,15 +24,15 @@
 _isort = "isort ."
 _black = "black ."
 _ruff = "ruff check --fix ."
 _mypy = "mypy ."
 all = { composite = ["fmt", "lint"] }
 fmt = { composite = ["_isort", "_black"] }
 lint = { composite = ["_ruff", "_mypy"] }
-image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_nft_marketplace:latest"
+image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_token_transfers:latest"
 
 [tool.isort]
 line_length = 120
 force_single_line = true
 
 [tool.black]
 line-length = 120
```

### Comparing `dipdup-7.0.0rc2/src/demo_nft_marketplace/types/hen_minter/tezos_storage.py` & `dipdup-7.0.0rc3/src/demo_nft_marketplace/types/hen_minter/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_nft_marketplace/types/hen_objkts/tezos_storage.py` & `dipdup-7.0.0rc3/src/demo_nft_marketplace/types/hen_objkts/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_raw/README.md` & `dipdup-7.0.0rc3/src/demo_uniswap/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# demo_raw
+# demo_uniswap
 
-Process raw operations without filtering and strict typing
+Uniswap V3 pools, positions, swaps, ticks, etc.
 
 ## Installation
 
 This project is based on [DipDup](https://dipdup.io), a framework for building featureful dapps.
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
@@ -38,15 +38,15 @@
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
 pdm install
-pdm venv activate
+$(pdm venv activate)
 ```
 
 Some tools are included to help you keep the code quality high: black, ruff and mypy.
 
 ```bash
 # Format code
 pdm fmt
```

### Comparing `dipdup-7.0.0rc2/src/demo_raw/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc3/src/demo_raw/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_raw/deploy/compose.yaml` & `dipdup-7.0.0rc3/src/demo_raw/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_raw/pyproject.toml` & `dipdup-7.0.0rc3/src/demo_uniswap/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
-name = "demo_raw"
+name = "demo_uniswap"
 version = "0.0.1"
-description = "Process raw operations without filtering and strict typing"
+description = "Uniswap V3 pools, positions, swaps, ticks, etc."
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc2,<8"
+    "dipdup>=7.0.0rc3,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
@@ -24,15 +24,15 @@
 _isort = "isort ."
 _black = "black ."
 _ruff = "ruff check --fix ."
 _mypy = "mypy ."
 all = { composite = ["fmt", "lint"] }
 fmt = { composite = ["_isort", "_black"] }
 lint = { composite = ["_ruff", "_mypy"] }
-image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_raw:latest"
+image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_uniswap:latest"
 
 [tool.isort]
 line_length = 120
 force_single_line = true
 
 [tool.black]
 line-length = 120
```

### Comparing `dipdup-7.0.0rc2/src/demo_token/README.md` & `dipdup-7.0.0rc3/src/demo_token/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
 pdm install
-pdm venv activate
+$(pdm venv activate)
 ```
 
 Some tools are included to help you keep the code quality high: black, ruff and mypy.
 
 ```bash
 # Format code
 pdm fmt
```

### Comparing `dipdup-7.0.0rc2/src/demo_token/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc3/src/demo_token/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_token/deploy/compose.yaml` & `dipdup-7.0.0rc3/src/demo_token/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_token/dipdup.yaml` & `dipdup-7.0.0rc3/src/demo_token/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_token/handlers/on_mint.py` & `dipdup-7.0.0rc3/src/demo_token/handlers/on_mint.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_token/handlers/on_transfer.py` & `dipdup-7.0.0rc3/src/demo_token/handlers/on_transfer.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_token/pyproject.toml` & `dipdup-7.0.0rc3/src/demo_token/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc2,<8"
+    "dipdup>=7.0.0rc3,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
```

### Comparing `dipdup-7.0.0rc2/src/demo_token_transfers/README.md` & `dipdup-7.0.0rc3/src/demo_dao/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# demo_token_transfers
+# demo_dao
 
-TzBTC FA1.2 token transfers
+Homebase DAO registry
 
 ## Installation
 
 This project is based on [DipDup](https://dipdup.io), a framework for building featureful dapps.
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
@@ -38,15 +38,15 @@
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
 pdm install
-pdm venv activate
+$(pdm venv activate)
 ```
 
 Some tools are included to help you keep the code quality high: black, ruff and mypy.
 
 ```bash
 # Format code
 pdm fmt
```

### Comparing `dipdup-7.0.0rc2/src/demo_token_transfers/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc3/src/demo_token_transfers/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_token_transfers/deploy/compose.yaml` & `dipdup-7.0.0rc3/src/demo_token_transfers/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_token_transfers/handlers/on_balance_update.py` & `dipdup-7.0.0rc3/src/demo_token_transfers/handlers/on_balance_update.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_token_transfers/handlers/on_token_transfer.py` & `dipdup-7.0.0rc3/src/demo_token_transfers/handlers/on_token_transfer.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_token_transfers/pyproject.toml` & `dipdup-7.0.0rc3/src/demo_domains/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
-name = "demo_token_transfers"
+name = "demo_domains"
 version = "0.0.1"
-description = "TzBTC FA1.2 token transfers"
+description = "Tezos Domains name service"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc2,<8"
+    "dipdup>=7.0.0rc3,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
@@ -24,15 +24,15 @@
 _isort = "isort ."
 _black = "black ."
 _ruff = "ruff check --fix ."
 _mypy = "mypy ."
 all = { composite = ["fmt", "lint"] }
 fmt = { composite = ["_isort", "_black"] }
 lint = { composite = ["_ruff", "_mypy"] }
-image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_token_transfers:latest"
+image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_domains:latest"
 
 [tool.isort]
 line_length = 120
 force_single_line = true
 
 [tool.black]
 line-length = 120
```

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/README.md` & `dipdup-7.0.0rc3/src/demo_blank/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# demo_uniswap
+# demo_blank
 
-Uniswap V3 pools, positions, swaps, ticks, etc.
+Empty config for a fresh start
 
 ## Installation
 
 This project is based on [DipDup](https://dipdup.io), a framework for building featureful dapps.
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
@@ -38,15 +38,15 @@
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
 pdm install
-pdm venv activate
+$(pdm venv activate)
 ```
 
 Some tools are included to help you keep the code quality high: black, ruff and mypy.
 
 ```bash
 # Format code
 pdm fmt
```

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/abi/factory/abi.json` & `dipdup-7.0.0rc3/src/demo_uniswap/abi/factory/abi.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/abi/factory/events.json` & `dipdup-7.0.0rc3/src/demo_uniswap/abi/factory/events.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/abi/pool/abi.json` & `dipdup-7.0.0rc3/src/demo_uniswap/abi/pool/abi.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/abi/pool/events.json` & `dipdup-7.0.0rc3/src/demo_uniswap/abi/pool/events.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/abi/position_manager/abi.json` & `dipdup-7.0.0rc3/src/demo_uniswap/abi/position_manager/abi.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/abi/position_manager/events.json` & `dipdup-7.0.0rc3/src/demo_uniswap/abi/position_manager/events.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc3/src/demo_uniswap/deploy/compose.swarm.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/deploy/compose.yaml` & `dipdup-7.0.0rc3/src/demo_uniswap/deploy/compose.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/dipdup.yaml` & `dipdup-7.0.0rc3/src/demo_uniswap/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/handlers/factory/pool_created.py` & `dipdup-7.0.0rc3/src/demo_uniswap/handlers/factory/pool_created.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/handlers/pool/burn.py` & `dipdup-7.0.0rc3/src/demo_uniswap/handlers/pool/burn.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/handlers/pool/initialize.py` & `dipdup-7.0.0rc3/src/demo_uniswap/handlers/pool/initialize.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/handlers/pool/mint.py` & `dipdup-7.0.0rc3/src/demo_uniswap/handlers/pool/mint.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/handlers/pool/swap.py` & `dipdup-7.0.0rc3/src/demo_uniswap/handlers/pool/swap.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/handlers/position_manager/collect.py` & `dipdup-7.0.0rc3/src/demo_uniswap/handlers/position_manager/collect.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/handlers/position_manager/decrease_liquidity.py` & `dipdup-7.0.0rc3/src/demo_uniswap/handlers/position_manager/decrease_liquidity.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/handlers/position_manager/increase_liquidity.py` & `dipdup-7.0.0rc3/src/demo_uniswap/handlers/position_manager/increase_liquidity.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/handlers/position_manager/transfer.py` & `dipdup-7.0.0rc3/src/demo_uniswap/handlers/position_manager/transfer.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/models/__init__.py` & `dipdup-7.0.0rc3/src/demo_uniswap/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/models/pool.py` & `dipdup-7.0.0rc3/src/demo_uniswap/models/pool.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/models/position.py` & `dipdup-7.0.0rc3/src/demo_uniswap/models/position.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/models/repo.py` & `dipdup-7.0.0rc3/src/demo_uniswap/models/repo.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/models/tick.py` & `dipdup-7.0.0rc3/src/demo_uniswap/models/tick.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/models/token.py` & `dipdup-7.0.0rc3/src/demo_uniswap/models/token.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/demo_uniswap/pyproject.toml` & `dipdup-7.0.0rc3/src/demo_blank/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
-name = "demo_uniswap"
+name = "demo_blank"
 version = "0.0.1"
-description = "Uniswap V3 pools, positions, swaps, ticks, etc."
+description = "Empty config for a fresh start"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc2,<8"
+    "dipdup>=7.0.0rc3,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
@@ -24,15 +24,15 @@
 _isort = "isort ."
 _black = "black ."
 _ruff = "ruff check --fix ."
 _mypy = "mypy ."
 all = { composite = ["fmt", "lint"] }
 fmt = { composite = ["_isort", "_black"] }
 lint = { composite = ["_ruff", "_mypy"] }
-image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_uniswap:latest"
+image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_blank:latest"
 
 [tool.isort]
 line_length = 120
 force_single_line = true
 
 [tool.black]
 line-length = 120
```

### Comparing `dipdup-7.0.0rc2/src/dipdup/api.py` & `dipdup-7.0.0rc3/src/dipdup/api.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/cli.py` & `dipdup-7.0.0rc3/src/dipdup/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,14 +174,17 @@
 @_cli_wrapper
 async def cli(ctx: click.Context, config: list[str], env_file: list[str]) -> None:
     # NOTE: Workaround for help pages. First argument check is for the test runner.
     args = sys.argv[1:] if sys.argv else ['--help']
     if '--help' in args or args in (['config'], ['hasura'], ['schema']) or args[0] in ('self', 'report'):
         return
 
+    # NOTE: https://github.com/python/cpython/issues/95778
+    sys.set_int_max_str_digits(0)
+
     from dotenv import load_dotenv
 
     from dipdup.exceptions import ConfigurationError
     from dipdup.sys import set_up_logging
 
     set_up_logging()
 
@@ -248,26 +251,27 @@
 
     dipdup = DipDup(config)
     await dipdup.run()
 
 
 @cli.command()
 @click.option('--force', '-f', is_flag=True, help='Regenerate existing types and ABIs.')
+@click.option('--base', '-b', is_flag=True, help='Also generate tempalate base: pyproject.toml, README.md, etc.')
 @click.pass_context
 @_cli_wrapper
-async def init(ctx: click.Context, force: bool) -> None:
+async def init(ctx: click.Context, force: bool, base: bool) -> None:
     """Generate project tree, callbacks and types.
 
     This command is idempotent, meaning it won't overwrite previously generated files unless asked explicitly.
     """
     from dipdup.dipdup import DipDup
 
     config: DipDupConfig = ctx.obj.config
     dipdup = DipDup(config)
-    await dipdup.init(force)
+    await dipdup.init(force, base)
 
 
 @cli.command()
 @click.pass_context
 @_cli_wrapper
 async def migrate(ctx: click.Context) -> None:
     """
@@ -718,11 +722,11 @@
 async def package_tree(ctx: click.Context) -> None:
     from dipdup.package import DipDupPackage
     from dipdup.package import draw_package_tree
 
     config: DipDupConfig = ctx.obj.config
     package = DipDupPackage(config.package_path)
     package.create()
-    tree = package.discover()
+    tree = package.tree()
     echo(f'{package.name} [{package.root.relative_to(Path.cwd())}]')
     for line in draw_package_tree(package.root, tree):
         echo(line)
```

### Comparing `dipdup-7.0.0rc2/src/dipdup/codegen/__init__.py` & `dipdup-7.0.0rc3/src/dipdup/codegen/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import subprocess
 from abc import ABC
 from abc import abstractmethod
 from pathlib import Path
+from shutil import rmtree
 from shutil import which
 from typing import Any
 from typing import Awaitable
 from typing import Callable
 
 from pydantic import BaseModel
 
@@ -42,37 +43,40 @@
         self._package = package
         self._datasources = datasources
         self._logger = _logger
 
     async def init(
         self,
         force: bool = False,
+        base: bool = False,
     ) -> None:
         self._package.create()
-        if replay := self._package.replay:
-            _logger.info('Using replay `%s`', replay)
+
+        replay = self._package.replay
+        if base and replay:
+            _logger.info('Recreating base template with replay.yaml')
             render_base(replay, force)
 
         await self.generate_abi()
-        await self.generate_schemas()
+        await self.generate_schemas(force)
         await self._generate_types(force)
 
         await self._generate_models()
         await self.generate_hooks()
         await self.generate_system_hooks()
         await self.generate_handlers()
 
         # self._package.verify()
 
     @abstractmethod
     async def generate_abi(self) -> None:
         ...
 
     @abstractmethod
-    async def generate_schemas(self) -> None:
+    async def generate_schemas(self, force: bool = False) -> None:
         ...
 
     @abstractmethod
     async def generate_hooks(self) -> None:
         ...
 
     @abstractmethod
@@ -199,14 +203,18 @@
                 continue
             return
 
         path = self._package.models / PACKAGE_MARKER
         content_path = Path(__file__).parent.parent / 'templates' / 'models.py'
         write(path, content_path.read_text())
 
+    def _cleanup_schemas(self) -> None:
+        rmtree(self._package.schemas)
+        self._package.schemas.mkdir()
+
 
 async def generate_environments(config: DipDupConfig, package: DipDupPackage) -> None:
     for default_env_path in package.deploy.glob(f'*{DEFAULT_ENV}'):
         default_env_path.unlink()
 
     for config_path in package.configs.iterdir():
         if config_path.suffix not in ('.yml', '.yaml') or not config_path.stem.startswith('dipdup'):
```

### Comparing `dipdup-7.0.0rc2/src/dipdup/codegen/evm_subsquid.py` & `dipdup-7.0.0rc3/src/dipdup/codegen/evm_subsquid.py`

 * *Files 9% similar despite different names*

```diff
@@ -107,15 +107,18 @@
     async def generate_abi(self) -> None:
         for index_config in self._config.indexes.values():
             if isinstance(index_config, SubsquidEventsIndexConfig):
                 await self._fetch_abi(index_config)
             elif isinstance(index_config, SubsquidOperationsIndexConfig):
                 raise NotImplementedError
 
-    async def generate_schemas(self) -> None:
+    async def generate_schemas(self, force: bool = False) -> None:
+        if force:
+            self._cleanup_schemas()
+
         events: set[str] = set()
         functions: set[str] = set()
 
         for index_config in self._config.indexes.values():
             if isinstance(index_config, SubsquidEventsIndexConfig):
                 for handler_config in index_config.handlers:
                     events.add(handler_config.name)
@@ -176,7 +179,12 @@
         # if schema_path.parent.name == 'evm_events':
         #     class_name = f'{module_name}_event'
         # elif schema_path.parent.name == 'evm_functions':
         #     class_name = f'{module_name}_function'
         # else:
         #     class_name = module_name
         return module_name
+
+    async def _generate_type(self, schema_path: Path, force: bool) -> None:
+        if 'evm_events' not in schema_path.parts:
+            return
+        await super()._generate_type(schema_path, force)
```

### Comparing `dipdup-7.0.0rc2/src/dipdup/codegen/tezos_tzkt.py` & `dipdup-7.0.0rc3/src/dipdup/codegen/tezos_tzkt.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,17 +97,19 @@
             datasources=datasources,
         )
         self._schemas: dict[str, dict[str, dict[str, Any]]] = {}
 
     async def generate_abi(self) -> None:
         pass
 
-    async def generate_schemas(self) -> None:
+    async def generate_schemas(self, force: bool = False) -> None:
         """Fetch JSONSchemas for all contracts used in config"""
         self._logger.info('Fetching contract schemas')
+        if force:
+            self._cleanup_schemas()
 
         unused_operation_templates = [
             t for t in self._config.templates.values() if isinstance(t, TzktOperationsIndexConfig)
         ]
 
         for index_config in self._config.indexes.values():
             if isinstance(index_config, TzktOperationsIndexConfig):
@@ -167,23 +169,34 @@
                 await self._generate_callback(hook_config, 'hooks', sql=True)
 
     async def generate_system_hooks(self) -> None:
         pass
 
     def get_typeclass_name(self, schema_path: Path) -> str:
         module_name = schema_path.stem
-        if schema_path.name == 'tezos_storage.json':
+        if module_name == 'tezos_storage':
             class_name = f'{schema_path.parent.name}_storage'
         elif schema_path.parent.name == 'tezos_parameters':
             class_name = f'{module_name}_parameter'
         elif schema_path.parent.name == 'tezos_events':
             class_name = f'{module_name}_payload'
         else:
             class_name = module_name
-        return class_name
+        return snake_to_pascal(class_name)
+
+    async def _generate_type(self, schema_path: Path, force: bool) -> None:
+        markers = {
+            'tezos_storage.json',
+            'tezos_parameters',
+            'tezos_events',
+            'tezos_big_maps',
+        }
+        if not set(schema_path.parts).intersection(markers):
+            return
+        await super()._generate_type(schema_path, force)
 
     async def _get_schema(
         self,
         datasource_config: TzktDatasourceConfig,
         contract_config: TezosContractConfig,
     ) -> dict[str, Any]:
         """Get contract JSONSchema from TzKT or from cache"""
@@ -374,15 +387,15 @@
     module_name = f'tezos_parameters.{pascal_to_snake(entrypoint)}'
     cls_name = snake_to_pascal(entrypoint) + 'Parameter'
     return package.get_type(typename, module_name, cls_name)
 
 
 def get_event_payload_type(package: DipDupPackage, typename: str, tag: str) -> TypeClass:
     tag = pascal_to_snake(tag.replace('.', '_'))
-    module_name = f'tezos_event.{tag}'
+    module_name = f'tezos_events.{tag}'
     cls_name = snake_to_pascal(f'{tag}_payload')
     return package.get_type(typename, module_name, cls_name)
 
 
 def get_big_map_key_type(package: DipDupPackage, typename: str, path: str) -> TypeClass:
     path = pascal_to_snake(path.replace('.', '_'))
     module_name = f'tezos_big_maps.{path}_key'
```

### Comparing `dipdup-7.0.0rc2/src/dipdup/config/__init__.py` & `dipdup-7.0.0rc3/src/dipdup/config/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/config/abi_etherscan.py` & `dipdup-7.0.0rc3/src/dipdup/config/abi_etherscan.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/config/coinbase.py` & `dipdup-7.0.0rc3/src/dipdup/config/coinbase.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/config/evm.py` & `dipdup-7.0.0rc3/src/dipdup/config/evm.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/config/evm_node.py` & `dipdup-7.0.0rc3/src/dipdup/config/evm_node.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/config/evm_subsquid.py` & `dipdup-7.0.0rc3/src/dipdup/config/evm_subsquid.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/config/evm_subsquid_events.py` & `dipdup-7.0.0rc3/src/dipdup/config/evm_subsquid_events.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/config/evm_subsquid_operations.py` & `dipdup-7.0.0rc3/src/dipdup/config/evm_subsquid_operations.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/config/ipfs.py` & `dipdup-7.0.0rc3/src/dipdup/config/ipfs.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/config/tezos.py` & `dipdup-7.0.0rc3/src/dipdup/config/tezos.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/config/tezos_tzkt.py` & `dipdup-7.0.0rc3/src/dipdup/config/tezos_tzkt.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/config/tezos_tzkt_big_maps.py` & `dipdup-7.0.0rc3/src/dipdup/config/tezos_tzkt_big_maps.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/config/tezos_tzkt_events.py` & `dipdup-7.0.0rc3/src/dipdup/config/tezos_tzkt_events.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/config/tezos_tzkt_head.py` & `dipdup-7.0.0rc3/src/dipdup/config/tezos_tzkt_head.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/config/tezos_tzkt_operations.py` & `dipdup-7.0.0rc3/src/dipdup/config/tezos_tzkt_operations.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/config/tezos_tzkt_token_transfers.py` & `dipdup-7.0.0rc3/src/dipdup/config/tezos_tzkt_token_transfers.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/config/tzip_metadata.py` & `dipdup-7.0.0rc3/src/dipdup/config/tzip_metadata.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/context.py` & `dipdup-7.0.0rc3/src/dipdup/context.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/database.py` & `dipdup-7.0.0rc3/src/dipdup/database.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/datasources/__init__.py` & `dipdup-7.0.0rc3/src/dipdup/datasources/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/datasources/abi_etherscan.py` & `dipdup-7.0.0rc3/src/dipdup/datasources/abi_etherscan.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/datasources/coinbase.py` & `dipdup-7.0.0rc3/src/dipdup/datasources/coinbase.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/datasources/evm_node.py` & `dipdup-7.0.0rc3/src/dipdup/datasources/evm_node.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/datasources/evm_subsquid.py` & `dipdup-7.0.0rc3/src/dipdup/datasources/evm_subsquid.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/datasources/ipfs.py` & `dipdup-7.0.0rc3/src/dipdup/datasources/ipfs.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/datasources/tezos_tzkt.py` & `dipdup-7.0.0rc3/src/dipdup/datasources/tezos_tzkt.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/datasources/tzip_metadata.py` & `dipdup-7.0.0rc3/src/dipdup/datasources/tzip_metadata.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/dipdup.py` & `dipdup-7.0.0rc3/src/dipdup/dipdup.py`

 * *Files 1% similar despite different names*

```diff
@@ -496,33 +496,37 @@
         await dipdup._set_up_database(stack)
         await dipdup._set_up_hooks(set())
         await dipdup._initialize_schema()
         await dipdup._set_up_transactions(stack)
 
         return dipdup
 
-    async def init(self, overwrite_types: bool = False, keep_schemas: bool = False) -> None:
+    async def init(
+        self,
+        force: bool = False,
+        base: bool = False,
+    ) -> None:
         """Create new or update existing dipdup project"""
         from dipdup.codegen.evm_subsquid import SubsquidCodeGenerator
         from dipdup.codegen.tezos_tzkt import TzktCodeGenerator
 
         await self._create_datasources()
 
         async with AsyncExitStack() as stack:
             for datasource in self._datasources.values():
                 await stack.enter_async_context(datasource)
 
-            package = DipDupPackage(
-                root=self._config.package_path,
-                debug=keep_schemas,
-            )
+            package = DipDupPackage(self._config.package_path)
 
             for codegen_cls in (TzktCodeGenerator, SubsquidCodeGenerator):
                 codegen = codegen_cls(self._config, package, self._datasources)
-                await codegen.init(force=overwrite_types)
+                await codegen.init(
+                    force=force,
+                    base=base,
+                )
 
             await generate_environments(self._config, package)
 
     async def run(self) -> None:
         """Run indexing process"""
         # NOTE: DipDup is initialized layer by layer adding tasks to the loop and entering contexts.
         # NOTE: Order matters. But usually you can skip some layers if you don't need them.
```

### Comparing `dipdup-7.0.0rc2/src/dipdup/env.py` & `dipdup-7.0.0rc3/src/dipdup/env.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import importlib
 import importlib.util
 import platform
+import tomllib
 from contextlib import suppress
 from os import environ as env
 from pathlib import Path
 
 
 def get_package_path(package: str) -> Path:
     """Absolute path to the indexer package, existing or default"""
 
     # NOTE: Integration tests run in isolated environment
     if TEST:
         return Path.cwd() / package
 
     # NOTE: If cwd is a package, use it
-    if Path('pyproject.toml').exists() and Path.cwd().name == package:
-        return Path.cwd()
+    pyproject_path = Path('pyproject.toml')
+    if pyproject_path.exists():
+        pyproject_package = tomllib.loads(pyproject_path.read_text())['project']['name']
+        if pyproject_package == package:
+            return Path.cwd()
 
     # NOTE: Detect existing package in current environment
     with suppress(ImportError):
         module = importlib.import_module(package)
         if module.__file__ is None:
             raise ImportError(f'`{module.__name__}` package has no `__file__` attribute')
         return Path(module.__file__).parent
```

### Comparing `dipdup-7.0.0rc2/src/dipdup/exceptions.py` & `dipdup-7.0.0rc3/src/dipdup/exceptions.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/fetcher.py` & `dipdup-7.0.0rc3/src/dipdup/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/fields.py` & `dipdup-7.0.0rc3/src/dipdup/fields.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/hasura.py` & `dipdup-7.0.0rc3/src/dipdup/hasura.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/http.py` & `dipdup-7.0.0rc3/src/dipdup/http.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/index.py` & `dipdup-7.0.0rc3/src/dipdup/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/indexes/evm_subsquid_events/fetcher.py` & `dipdup-7.0.0rc3/src/dipdup/indexes/evm_subsquid_events/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/indexes/evm_subsquid_events/index.py` & `dipdup-7.0.0rc3/src/dipdup/indexes/evm_subsquid_events/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/indexes/evm_subsquid_events/matcher.py` & `dipdup-7.0.0rc3/src/dipdup/indexes/evm_subsquid_events/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_big_maps/fetcher.py` & `dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_big_maps/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_big_maps/index.py` & `dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_big_maps/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_big_maps/matcher.py` & `dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_big_maps/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_events/fetcher.py` & `dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_events/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_events/index.py` & `dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_events/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_events/matcher.py` & `dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_events/matcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,17 +42,18 @@
         )
 
     type_ = get_event_payload_type(
         package=package,
         typename=handler_config.contract.module_name,
         tag=handler_config.tag,
     )
+    if not matched_event.payload:
+        raise FrameworkException('Event is typed, but payload is empty')
+
     with suppress(InvalidDataError):
-        if not matched_event.payload:
-            raise FrameworkException('Event payload is empty')
         typed_payload = parse_object(type_, matched_event.payload)
         return TzktEvent(
             data=matched_event,
             payload=typed_payload,
         )
 
     return None
@@ -93,10 +94,10 @@
                 raise FrameworkException(f'Unexpected handler config type: {type(handler_config)}')
 
             events.remove(event)
 
     # NOTE: We don't care about `merge_subscriptions` here implying that all events will be processed
     # NOTE: Maybe "unfiltered" indexes will cover that case?
     for address in {event.contract_address for event in events}:
-        _logger.warning('Some events were not matched; fallback handler is missing for `{}`', address)
+        _logger.warning('Some events were not matched; fallback handler is missing for `%s`', address)
 
     return matched_handlers
```

### Comparing `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_head/index.py` & `dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_head/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_operations/fetcher.py` & `dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_operations/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_operations/index.py` & `dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_operations/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_operations/matcher.py` & `dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_operations/matcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,16 @@
             args.append(None)
 
         elif isinstance(pattern_config, TransactionPatternConfig):
             if not pattern_config.typed_contract or not pattern_config.entrypoint:
                 args.append(operation_data)
                 continue
 
-            if not operation_data.parameter_json:
-                raise FrameworkException('Transaction parameter is empty')
+            if operation_data.parameter_json is None:
+                raise FrameworkException('Processing typed transaction, but parameter_json is None')
             typename = pattern_config.typed_contract.module_name
             type_ = get_parameter_type(package, typename, pattern_config.entrypoint)
             parameter = parse_object(type_, operation_data.parameter_json) if type_ else None
 
             storage_type = get_storage_type(package, typename)
             operation_data, storage = deserialize_storage(operation_data, storage_type)
```

### Comparing `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_operations/parser.py` & `dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_operations/parser.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_token_transfers/fetcher.py` & `dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_token_transfers/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_token_transfers/index.py` & `dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_token_transfers/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_token_transfers/matcher.py` & `dipdup-7.0.0rc3/src/dipdup/indexes/tezos_tzkt_token_transfers/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/install.py` & `dipdup-7.0.0rc3/src/dipdup/install.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
      / /_/ // // /_/ // /_/ // /_/ // /_/ /
     /_____//_// .___//_____/ \__,_// .___/ 
              /_/                  /_/      
 """
 EPILOG = """\0
 Documentation:         https://dipdup.io/docs
 GitHub:                https://github.com/dipdup-io/dipdup
-Discord:               https://discord.gg/NbANhqCJHA
+Discord:               https://discord.gg/aG8XKuwsQd
 """
 
 
 class Colors:
     """ANSI color codes"""
 
     BLUE = '\033[34m'
@@ -163,15 +163,15 @@
 ) -> None:
     """Install DipDup and its dependencies with pipx"""
     if ref and path:
         fail('Specify either ref or path, not both')
 
     if not any((version, ref, path)):
         # FIXME: Temporary, remove when 7.0.0 is released
-        version = '7.0.0rc2'
+        version = '7.0.0rc3'
 
     env = DipDupEnvironment()
     env.prepare()
     if not quiet:
         env.print()
 
     force_str = '--force' if force else ''
```

### Comparing `dipdup-7.0.0rc2/src/dipdup/models/__init__.py` & `dipdup-7.0.0rc3/src/dipdup/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/models/coinbase.py` & `dipdup-7.0.0rc3/src/dipdup/models/coinbase.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/models/evm_node.py` & `dipdup-7.0.0rc3/src/dipdup/models/evm_node.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/models/evm_subsquid.py` & `dipdup-7.0.0rc3/src/dipdup/models/evm_subsquid.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/models/tezos_tzkt.py` & `dipdup-7.0.0rc3/src/dipdup/models/tezos_tzkt.py`

 * *Files 1% similar despite different names*

```diff
@@ -511,29 +511,32 @@
         """Convert raw token transfer message from REST or WS into dataclass"""
         token_json = token_transfer_json.get('token') or {}
         contract_json = token_json.get('contract') or {}
         from_json = token_transfer_json.get('from') or {}
         to_json = token_transfer_json.get('to') or {}
         standard = token_json.get('standard')
         metadata = token_json.get('metadata')
+        amount = token_transfer_json.get('amount')
+        amount = int(amount) if amount is not None else None
+
         return TzktTokenTransferData(
             id=token_transfer_json['id'],
             level=token_transfer_json['level'],
             timestamp=_parse_timestamp(token_transfer_json['timestamp']),
             tzkt_token_id=token_json['id'],
             contract_address=contract_json.get('address'),
             contract_alias=contract_json.get('alias'),
             token_id=token_json.get('tokenId'),
             standard=TzktTokenStandard(standard) if standard else None,
             metadata=metadata if isinstance(metadata, dict) else {},
             from_alias=from_json.get('alias'),
             from_address=from_json.get('address'),
             to_alias=to_json.get('alias'),
             to_address=to_json.get('address'),
-            amount=token_transfer_json.get('amount'),
+            amount=amount,
             tzkt_transaction_id=token_transfer_json.get('transactionId'),
             tzkt_origination_id=token_transfer_json.get('originationId'),
             tzkt_migration_id=token_transfer_json.get('migrationId'),
         )
 
 
 @dataclass(frozen=True)
```

### Comparing `dipdup-7.0.0rc2/src/dipdup/package.py` & `dipdup-7.0.0rc3/src/dipdup/package.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from dipdup.utils import import_submodules
 from dipdup.utils import pascal_to_snake
 from dipdup.utils import touch
 
 KEEP_MARKER = '.keep'
 PACKAGE_MARKER = '__init__.py'
 PEP_561_MARKER = 'py.typed'
-PYPROJECT = 'pyproject.toml'
 DEFAULT_ENV = '.env.default'
 
 EVM_ABI = 'abi.json'
 EVM_EVENTS = 'events.json'
 
 _branch = '│   '
 _tee = '├── '
@@ -55,17 +54,16 @@
 class EventAbiExtra:
     name: str
     topic0: str
     inputs: tuple[tuple[str, bool], ...]
 
 
 class DipDupPackage:
-    def __init__(self, root: Path, debug: bool = False) -> None:
+    def __init__(self, root: Path) -> None:
         self.root = root
-        self.debug = debug
         self.name = root.name
 
         # NOTE: Package sections with .keep markers
         self.abi = root / 'abi'
         self.configs = root / 'configs'
         self.deploy = root / 'deploy'
         self.graphql = root / 'graphql'
@@ -108,20 +106,17 @@
             self.hooks: '**/*.py',
             self.models: '**/*.py',
             self.sql: '**/*.sql',
             self.types: '**/*.py',
             # NOTE: Python metadata
             Path(PEP_561_MARKER): None,
             Path(PACKAGE_MARKER): None,
-            Path(PYPROJECT): None,
-            # NOTE: Not a part of package
-            self.schemas: '**/*.json',
         }
 
-    def discover(self) -> dict[str, tuple[Path, ...]]:
+    def tree(self) -> dict[str, tuple[Path, ...]]:
         tree = {}
         for path, exp in self.skel.items():
             tree[path.name] = tuple(path.glob(exp)) if exp else ()
         return tree
 
     def create(self) -> None:
         """Create Python package skeleton if not exists"""
@@ -139,15 +134,20 @@
     def _pre_init(self) -> None:
         if self.name != pascal_to_snake(self.name):
             raise ProjectImportError(f'`{self.name}` is not a valid Python package name')
         if self.root.exists() and not self.root.is_dir():
             raise ProjectImportError(f'`{self.root}` exists and not a directory')
 
     def _post_init(self) -> None:
-        pass
+        # NOTE: Allows plain package structure to be imported
+        symlink_path = self.root.joinpath(self.name)
+        if symlink_path.exists() and not symlink_path.is_symlink():
+            raise ProjectImportError(f'`{symlink_path}` exists and not a symlink')
+        if not symlink_path.exists():
+            symlink_path.symlink_to('.', True)
 
     def verify(self) -> None:
         _logger.debug('Verifying `%s` package', self.root)
         import_submodules(self.name)
 
     def get_type(self, typename: str, module: str, name: str) -> type[BaseModel]:
         key = f'{typename}{module}{name}'
```

### Comparing `dipdup-7.0.0rc2/src/dipdup/performance.py` & `dipdup-7.0.0rc3/src/dipdup/performance.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/project.py` & `dipdup-7.0.0rc3/src/dipdup/project.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/base/README.md.j2` & `dipdup-7.0.0rc3/src/demo_head/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# {{project.package}}
+# demo_head
 
-{{project.description}}
+Processing head block metadata
 
 ## Installation
 
 This project is based on [DipDup](https://dipdup.io), a framework for building featureful dapps.
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
@@ -38,15 +38,15 @@
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
 pdm install
-pdm venv activate
+$(pdm venv activate)
 ```
 
 Some tools are included to help you keep the code quality high: black, ruff and mypy.
 
 ```bash
 # Format code
 pdm fmt
@@ -54,8 +54,8 @@
 # Lint code
 pdm lint
 
 # Build Docker image
 pdm image
 ```
 
-Inspect the `pyproject.toml` file. It contains all the dependencies and tools used in the project.
+Inspect the `pyproject.toml` file. It contains all the dependencies and tools used in the project.
```

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/base/deploy/compose.swarm.yaml.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/base/deploy/compose.swarm.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/base/deploy/compose.yaml.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/base/deploy/compose.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/base/pyproject.toml.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/base/pyproject.toml.j2`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 license = { text = "{{ project.license }}" }
 authors = [
     { name = "{{ project.name }}", email = "{{ project.email }}" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>={{ project.dipdup_version }}.0.0rc1,<{{ project.dipdup_version | int + 1 }}"
+    "dipdup>={{ project.dipdup_version }}.0.0rc3,<{{ project.dipdup_version | int + 1 }}"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
```

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_auction/dipdup.yaml.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_auction/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_auction/handlers/on_bid.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_auction/handlers/on_bid.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_auction/handlers/on_create_auction.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_auction/handlers/on_create_auction.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_auction/handlers/on_withdraw.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_auction/handlers/on_withdraw.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_auction/models/__init__.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_auction/models/__init__.py.j2`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from enum import IntEnum
 
 
 from dipdup import fields
-
 from dipdup.models import Model
 
 
 class AuctionStatus(IntEnum):
     ACTIVE = 0
     FINISHED = 1
```

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_big_maps/dipdup.yaml.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_big_maps/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_big_maps/handlers/on_update_expiry_map.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_big_maps/handlers/on_update_expiry_map.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_big_maps/handlers/on_update_records.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_big_maps/handlers/on_update_records.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_big_maps/models/__init__.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_big_maps/models/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_dao/dipdup.yaml.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_dao/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_dao/handlers/on_propose.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_dao/handlers/on_propose.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_dao/models/__init__.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_dao/models/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/dipdup.yaml.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_divest_liquidity.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa12_divest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_invest_liquidity.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa12_invest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_origination.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa12_origination.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_tez_to_token.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa12_tez_to_token.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_token_to_tez.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa12_token_to_tez.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_transfer.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa12_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_withdraw_profit.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa12_withdraw_profit.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_divest_liquidity.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa2_divest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_invest_liquidity.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa2_invest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_origination.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa2_origination.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_tez_to_token.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa2_tez_to_token.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_token_to_tez.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa2_token_to_tez.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_transfer.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa2_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_withdraw_profit.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/handlers/on_fa2_withdraw_profit.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/models/__init__.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_dex/models/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_domains/dipdup.yaml.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_domains/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_domains/handlers/on_admin_update.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_domains/handlers/on_admin_update.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_domains/handlers/on_execute.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_domains/handlers/on_execute.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_domains/handlers/on_storage_diff.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_domains/handlers/on_storage_diff.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_domains/models/__init__.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_domains/models/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_events/dipdup.yaml.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_events/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_evm_events/dipdup.yaml.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_evm_events/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_evm_events/handlers/on_transfer.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_evm_events/handlers/on_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_factories/dipdup.yaml.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_factories/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_factories/handlers/on_propose.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_factories/handlers/on_propose.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_factories/models/__init__.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_factories/models/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/dipdup.yaml.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_nft_marketplace/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/handlers/on_cancel_swap.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_nft_marketplace/handlers/on_cancel_swap.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/handlers/on_collect.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_nft_marketplace/handlers/on_collect.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/handlers/on_mint.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_nft_marketplace/handlers/on_mint.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/handlers/on_swap.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_nft_marketplace/handlers/on_swap.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/models/__init__.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_nft_marketplace/models/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_token/dipdup.yaml.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_token/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_token/handlers/on_mint.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_token/handlers/on_mint.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_token/handlers/on_transfer.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_token/handlers/on_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_token_transfers/handlers/on_balance_update.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_token_transfers/handlers/on_balance_update.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_token_transfers/handlers/on_token_transfer.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_token_transfers/handlers/on_token_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/dipdup.yaml.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/factory/pool_created.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/handlers/factory/pool_created.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/pool/burn.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/handlers/pool/burn.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/pool/initialize.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/handlers/pool/initialize.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/pool/mint.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/handlers/pool/mint.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/pool/swap.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/handlers/pool/swap.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/position_manager/collect.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/handlers/position_manager/collect.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/position_manager/decrease_liquidity.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/handlers/position_manager/decrease_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/position_manager/increase_liquidity.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/handlers/position_manager/increase_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/position_manager/transfer.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/handlers/position_manager/transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/__init__.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/models/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/pool.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/models/pool.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/position.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/models/position.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/repo.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/models/repo.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/tick.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/models/tick.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/token.py.j2` & `dipdup-7.0.0rc3/src/dipdup/projects/demo_uniswap/models/token.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/prometheus.py` & `dipdup-7.0.0rc3/src/dipdup/prometheus.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/pysignalr.py` & `dipdup-7.0.0rc3/src/dipdup/pysignalr.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/report.py` & `dipdup-7.0.0rc3/src/dipdup/report.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/scheduler.py` & `dipdup-7.0.0rc3/src/dipdup/scheduler.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/sentry.py` & `dipdup-7.0.0rc3/src/dipdup/sentry.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import hashlib
 import logging
 import platform
 from contextlib import suppress
 from typing import Any
 
 import sentry_sdk
+import sentry_sdk.consts
 import sentry_sdk.serializer
-import sentry_sdk.utils
 from sentry_sdk.integrations.aiohttp import AioHttpIntegration
 from sentry_sdk.integrations.atexit import AtexitIntegration
 from sentry_sdk.integrations.logging import LoggingIntegration
 
 from dipdup import __version__
 from dipdup import env
 from dipdup.config import DipDupConfig
@@ -103,17 +103,17 @@
         dsn=dsn,
         integrations=integrations,
         attach_stacktrace=attach_stacktrace,
         before_send=before_send,
         release=release,
         environment=environment,
         server_name=server_name,
+        # NOTE: Increase __repr__ length limit
+        max_value_length=sentry_sdk.consts.DEFAULT_MAX_VALUE_LENGTH * 10,
     )
-    # NOTE: Increase __repr__ length limit
-    sentry_sdk.utils.MAX_STRING_LENGTH *= 10
 
     # NOTE: Setting session tags
     tags = {
         'python': platform.python_version(),
         'os': f'{platform.system().lower()}-{platform.machine()}',
         'version': __version__,
         'package': package,
```

### Comparing `dipdup-7.0.0rc2/src/dipdup/sql/truncate_schema.sql` & `dipdup-7.0.0rc3/src/dipdup/sql/truncate_schema.sql`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/subscriptions.py` & `dipdup-7.0.0rc3/src/dipdup/subscriptions.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/sys.py` & `dipdup-7.0.0rc3/src/dipdup/sys.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/templates/models.py` & `dipdup-7.0.0rc3/src/dipdup/templates/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import enum
 
 from dipdup import fields
-from dipdup import models
+from dipdup.models import Model
 
 
-class ExampleModel(models.Model):
+class ExampleModel(Model):
     id = fields.IntField(pk=True)
     array = fields.ArrayField()
     big_int = fields.BigIntField()
     binary = fields.BinaryField()
     boolean = fields.BooleanField()
     decimal = fields.DecimalField(10, 2)
     date = fields.DateField()
```

### Comparing `dipdup-7.0.0rc2/src/dipdup/transactions.py` & `dipdup-7.0.0rc3/src/dipdup/transactions.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/src/dipdup/utils.py` & `dipdup-7.0.0rc3/src/dipdup/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,25 @@
     return True
 
 
 def import_submodules(package: str) -> Dict[str, types.ModuleType]:
     """Recursively import all submodules of a package"""
     module = importlib.import_module(package)
     results = {}
+
+    # NOTE: The first level; walk_packages falls into recursion with root symlink.
+    if '.' not in package:
+        for attr in dir(module):
+            member = getattr(module, attr)
+            if not isinstance(member, types.ModuleType):
+                continue
+            full_name = package + '.' + attr
+            results[full_name] = importlib.import_module(full_name)
+        return results
+
     for subpackage in pkgutil.walk_packages(module.__path__):
         name = subpackage.name
         is_pkg = subpackage.ispkg
         full_name = package + '.' + name
         results[full_name] = importlib.import_module(full_name)
         if is_pkg:
             results.update(import_submodules(full_name))
```

### Comparing `dipdup-7.0.0rc2/src/dipdup/yaml.py` & `dipdup-7.0.0rc3/src/dipdup/yaml.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/__init__.py` & `dipdup-7.0.0rc3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/configs/demo_auction.yml` & `dipdup-7.0.0rc3/tests/configs/demo_auction.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/configs/demo_big_maps.yml` & `dipdup-7.0.0rc3/tests/configs/demo_big_maps.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/configs/demo_dao.yml` & `dipdup-7.0.0rc3/tests/configs/demo_dao.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/configs/demo_dex.yml` & `dipdup-7.0.0rc3/tests/configs/demo_dex.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/configs/demo_domains.yml` & `dipdup-7.0.0rc3/tests/configs/demo_domains.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/configs/demo_factories.yml` & `dipdup-7.0.0rc3/tests/configs/demo_factories.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/configs/demo_nft_marketplace.yml` & `dipdup-7.0.0rc3/tests/configs/demo_nft_marketplace.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/configs/demo_raw.yml` & `dipdup-7.0.0rc3/tests/configs/demo_raw.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/configs/demo_token.yml` & `dipdup-7.0.0rc3/tests/configs/demo_token.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/configs/demo_token_transfers.yml` & `dipdup-7.0.0rc3/tests/configs/demo_token_transfers.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/configs/demo_token_transfers_2.yml` & `dipdup-7.0.0rc3/tests/configs/demo_token_transfers_2.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/configs/demo_token_transfers_3.yml` & `dipdup-7.0.0rc3/tests/configs/demo_token_transfers_3.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/configs/demo_token_transfers_4.yml` & `dipdup-7.0.0rc3/tests/configs/demo_token_transfers_4.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/configs/dipdup.yml` & `dipdup-7.0.0rc3/tests/configs/dipdup.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/configs/hen_subjkt.yml` & `dipdup-7.0.0rc3/tests/configs/hen_subjkt.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/configs/kolibri_ovens.yml` & `dipdup-7.0.0rc3/tests/configs/kolibri_ovens.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/configs/operation_filters.yml` & `dipdup-7.0.0rc3/tests/configs/operation_filters.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/configs/yupana.yml` & `dipdup-7.0.0rc3/tests/configs/yupana.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/profile_abi_decoding.py` & `dipdup-7.0.0rc3/tests/profile_abi_decoding.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/0535b2dcc93076e6026fa48cc501adaed47b7b060e6483d8312f40c184d7287d` & `dipdup-7.0.0rc3/tests/replays/0535b2dcc93076e6026fa48cc501adaed47b7b060e6483d8312f40c184d7287d`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/064e788d2566d748f516b17c6a43ab34259443cc9537f0dec7c1a5a2bce704b2` & `dipdup-7.0.0rc3/tests/replays/064e788d2566d748f516b17c6a43ab34259443cc9537f0dec7c1a5a2bce704b2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/0eaaba2830dbdd3a80286fbc367084bce6e55c678e21da178a7eb16beef6c997` & `dipdup-7.0.0rc3/tests/replays/0eaaba2830dbdd3a80286fbc367084bce6e55c678e21da178a7eb16beef6c997`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/1228b36594bb93d619170ad49373f1ceec52d10faafdd727b37f3cdeffd663db` & `dipdup-7.0.0rc3/tests/replays/1228b36594bb93d619170ad49373f1ceec52d10faafdd727b37f3cdeffd663db`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/136157c421184c218127595797f5fe0b774e2807f6f4605a1d1944a1738e2d6d` & `dipdup-7.0.0rc3/tests/replays/136157c421184c218127595797f5fe0b774e2807f6f4605a1d1944a1738e2d6d`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/13afdf001ce3d6a0219c0f7f6d372d9b645770e5f4304576f7f7a37b45af96fc` & `dipdup-7.0.0rc3/tests/replays/13afdf001ce3d6a0219c0f7f6d372d9b645770e5f4304576f7f7a37b45af96fc`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/14408f393a3e399b241184f858e70396e3b8313e32ee1a984913d43fb74dcfec` & `dipdup-7.0.0rc3/tests/replays/14408f393a3e399b241184f858e70396e3b8313e32ee1a984913d43fb74dcfec`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/14cba0424c66b1869edc8e18ca3079856083cc3db7e68ef61fce165b6d7e1a6d` & `dipdup-7.0.0rc3/tests/replays/14cba0424c66b1869edc8e18ca3079856083cc3db7e68ef61fce165b6d7e1a6d`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/18d85ceab66daf057861b99b7e223a25067197b3b77edbf060390df58cb65eaa` & `dipdup-7.0.0rc3/tests/replays/18d85ceab66daf057861b99b7e223a25067197b3b77edbf060390df58cb65eaa`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/19441b677ef5fd8ca39c37e6ddd2a7d9bc8cb3ab282b2a91ce4d8430f56f0fa9` & `dipdup-7.0.0rc3/tests/replays/19441b677ef5fd8ca39c37e6ddd2a7d9bc8cb3ab282b2a91ce4d8430f56f0fa9`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/1a43bd7d1397cc3169ad267cd2ef083a5a63eaac7ed5186aadfc01bb53636214` & `dipdup-7.0.0rc3/tests/replays/1a43bd7d1397cc3169ad267cd2ef083a5a63eaac7ed5186aadfc01bb53636214`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/1c07d3d72acc637fb46c59d0a6dc9749f3412a5d527ca2eb0cccc01720fda1c7` & `dipdup-7.0.0rc3/tests/replays/1c07d3d72acc637fb46c59d0a6dc9749f3412a5d527ca2eb0cccc01720fda1c7`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/1c34d1f810ae474395893bf67fb8cfb27b0506ab94eebec42cd4d2d21bf3dfcd` & `dipdup-7.0.0rc3/tests/replays/1c34d1f810ae474395893bf67fb8cfb27b0506ab94eebec42cd4d2d21bf3dfcd`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/252fd058cfef21f9b5b7f4367f730ec7d41647253d7cc7ccfb1e22d42d1f366a` & `dipdup-7.0.0rc3/tests/replays/252fd058cfef21f9b5b7f4367f730ec7d41647253d7cc7ccfb1e22d42d1f366a`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/27373c23411bf37b605c8d0ead9a0e6c6c1f1718ce7863b095b759811e44e155` & `dipdup-7.0.0rc3/tests/replays/27373c23411bf37b605c8d0ead9a0e6c6c1f1718ce7863b095b759811e44e155`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/2a45ec6372b45e46199a6af24272cb93586777a0522cd1203b3eeef213ce4583` & `dipdup-7.0.0rc3/tests/replays/2a45ec6372b45e46199a6af24272cb93586777a0522cd1203b3eeef213ce4583`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/31cc70e13495f58ecde80847bc6c9e08536cc426c03bd2aa8c45c1b2c798e155` & `dipdup-7.0.0rc3/tests/replays/31cc70e13495f58ecde80847bc6c9e08536cc426c03bd2aa8c45c1b2c798e155`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/31dd376b771f347a0d6fe4dd132a1f96f809274429b78ec86dd742e5589fbc23` & `dipdup-7.0.0rc3/tests/replays/31dd376b771f347a0d6fe4dd132a1f96f809274429b78ec86dd742e5589fbc23`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/32e3a13cc470d8720ce28f5eaff327340fb25cbe712e5b5a348af1bc3c92235a` & `dipdup-7.0.0rc3/tests/replays/32e3a13cc470d8720ce28f5eaff327340fb25cbe712e5b5a348af1bc3c92235a`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/36072e13c9ce265bb81142b8816da8c31bd9180e7c663ea4169bd259af107382` & `dipdup-7.0.0rc3/tests/replays/36072e13c9ce265bb81142b8816da8c31bd9180e7c663ea4169bd259af107382`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/377ac31d6316391ed138df44bec374d65202f0577603e80465ced3c09140f78c` & `dipdup-7.0.0rc3/tests/replays/377ac31d6316391ed138df44bec374d65202f0577603e80465ced3c09140f78c`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/383899084f79460e96fd311bb64e4925738c486b39d6281539456c5fcac41620` & `dipdup-7.0.0rc3/tests/replays/383899084f79460e96fd311bb64e4925738c486b39d6281539456c5fcac41620`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/39b8664d1bca5d374ff905c8a3a396b53d19ee469dc37545a8ca6b080bd0e9e0` & `dipdup-7.0.0rc3/tests/replays/39b8664d1bca5d374ff905c8a3a396b53d19ee469dc37545a8ca6b080bd0e9e0`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/3a2bd8b6b72bf18152d2550c106789fa9b8abc98ea9d759a6597b7ebfbab0fc2` & `dipdup-7.0.0rc3/tests/replays/3a2bd8b6b72bf18152d2550c106789fa9b8abc98ea9d759a6597b7ebfbab0fc2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/3c9ad6f98f79e72185ea58c4777115750c658c5defd616664212095bd440c10c` & `dipdup-7.0.0rc3/tests/replays/3c9ad6f98f79e72185ea58c4777115750c658c5defd616664212095bd440c10c`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/42b7bf0da866257ef98e1f7124d2d21fe7d13228c076fffa32331da423f36933` & `dipdup-7.0.0rc3/tests/replays/42b7bf0da866257ef98e1f7124d2d21fe7d13228c076fffa32331da423f36933`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/43cb0ab415d8b8b3f7addc3e82ea27d93b2c66ff55c117e1e0c7c64a0fcfc3f2` & `dipdup-7.0.0rc3/tests/replays/43cb0ab415d8b8b3f7addc3e82ea27d93b2c66ff55c117e1e0c7c64a0fcfc3f2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/440173d32e95111ca7b080ccc4dc09bfab23c8361919b2c113f0ff9ab445eec2` & `dipdup-7.0.0rc3/tests/replays/440173d32e95111ca7b080ccc4dc09bfab23c8361919b2c113f0ff9ab445eec2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/489233ce9373f7de4f7a9053055c74bc0df999bfe939ed67d98b6d67e676e35a` & `dipdup-7.0.0rc3/tests/replays/489233ce9373f7de4f7a9053055c74bc0df999bfe939ed67d98b6d67e676e35a`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/4a57776d93475adfd9c49b6c3295a7cedfc23b73733a1fb5f0c985ee039dc5dc` & `dipdup-7.0.0rc3/tests/replays/4a57776d93475adfd9c49b6c3295a7cedfc23b73733a1fb5f0c985ee039dc5dc`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/4aa7f9b0657be0c44baf2caed8c7cb08d02097a4095cf6417f78cba3a25e8423` & `dipdup-7.0.0rc3/tests/replays/4aa7f9b0657be0c44baf2caed8c7cb08d02097a4095cf6417f78cba3a25e8423`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/5483a0e11009e0f186bf70c214e2597d267a75a1e19152a9e7ed1ec257ce88ca` & `dipdup-7.0.0rc3/tests/replays/5483a0e11009e0f186bf70c214e2597d267a75a1e19152a9e7ed1ec257ce88ca`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/587613799ebfae42b1884016d1a44a452d68e70e3ed80641d90b8e7657ba8ee5` & `dipdup-7.0.0rc3/tests/replays/587613799ebfae42b1884016d1a44a452d68e70e3ed80641d90b8e7657ba8ee5`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/5b7c31b4b73bc57e8296e6051b3bc7b2302b32588d8fbcafce8a66de3be743df` & `dipdup-7.0.0rc3/tests/replays/5b7c31b4b73bc57e8296e6051b3bc7b2302b32588d8fbcafce8a66de3be743df`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/5b99bc4beb6a9a33f7d2f118426458e4c788e0ab6d9e51949d3ccbf8b4003fc1` & `dipdup-7.0.0rc3/tests/replays/5b99bc4beb6a9a33f7d2f118426458e4c788e0ab6d9e51949d3ccbf8b4003fc1`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/5d21060ba8e78279d2d1edaa2f266ecf36105eaccef5ebed15748441651f76fd` & `dipdup-7.0.0rc3/tests/replays/5d21060ba8e78279d2d1edaa2f266ecf36105eaccef5ebed15748441651f76fd`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/6cc8d741a41b76983cd7e0f63e8f22a4c67cd946888f45a5b7ead8c3bb5ad2f1` & `dipdup-7.0.0rc3/tests/replays/6cc8d741a41b76983cd7e0f63e8f22a4c67cd946888f45a5b7ead8c3bb5ad2f1`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/6cff8d120db8fd3926a45714ce7f1d0560803eb5a7b4a413b64fee1b7fd7a8ff` & `dipdup-7.0.0rc3/tests/replays/6cff8d120db8fd3926a45714ce7f1d0560803eb5a7b4a413b64fee1b7fd7a8ff`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/6d76a3c3f427ff534c551de1793cb1d1dfbd22ccad97f5917a9f9b201a3f9804` & `dipdup-7.0.0rc3/tests/replays/6d76a3c3f427ff534c551de1793cb1d1dfbd22ccad97f5917a9f9b201a3f9804`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/7669ea717d9759748aed86302326b79be5157a1a36d13b39b00f06bcbe22b309` & `dipdup-7.0.0rc3/tests/replays/7669ea717d9759748aed86302326b79be5157a1a36d13b39b00f06bcbe22b309`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/76d49ae3b723376c88ca65a3080a273e098d226932a1a49c38fbc4421e7c2e64` & `dipdup-7.0.0rc3/tests/replays/76d49ae3b723376c88ca65a3080a273e098d226932a1a49c38fbc4421e7c2e64`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/7b6cf9b8c69712bf26ed09059352ec740606969bf20eab0dedda870273f4fde9` & `dipdup-7.0.0rc3/tests/replays/7b6cf9b8c69712bf26ed09059352ec740606969bf20eab0dedda870273f4fde9`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/7b9c78209f98b2c3a6678ed224fa686eee25c3c63dddd7f9af77c734b0dfabb8` & `dipdup-7.0.0rc3/tests/replays/7b9c78209f98b2c3a6678ed224fa686eee25c3c63dddd7f9af77c734b0dfabb8`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/803e05a8d0bb9e7cfb49530271d43ea62111b6419e7cded2d221f7e0e0c92ece` & `dipdup-7.0.0rc3/tests/replays/803e05a8d0bb9e7cfb49530271d43ea62111b6419e7cded2d221f7e0e0c92ece`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/80921fd33043def891912a6ad57d76664399564fd813950eb11f4a0e69e3e28f` & `dipdup-7.0.0rc3/tests/replays/80921fd33043def891912a6ad57d76664399564fd813950eb11f4a0e69e3e28f`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/816d08f71c84537ea8df05a40678b1addca15bf3a73c0e927c75d9f9c0f2d418` & `dipdup-7.0.0rc3/tests/replays/816d08f71c84537ea8df05a40678b1addca15bf3a73c0e927c75d9f9c0f2d418`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/84cf46aa9c8dbd3ca6c3d946c749713e6c70a6a20d9cc69b4156235fd099b2e3` & `dipdup-7.0.0rc3/tests/replays/84cf46aa9c8dbd3ca6c3d946c749713e6c70a6a20d9cc69b4156235fd099b2e3`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/93516225810a23a6799f2f9a1dee055ca79a66ee2b8d0f32be820c9c385e936b` & `dipdup-7.0.0rc3/tests/replays/93516225810a23a6799f2f9a1dee055ca79a66ee2b8d0f32be820c9c385e936b`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/9e6e907842da2cd494c558ea5ecc211fd12e56bfc547450978fb7dfe03853e58` & `dipdup-7.0.0rc3/tests/replays/9e6e907842da2cd494c558ea5ecc211fd12e56bfc547450978fb7dfe03853e58`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/a3ce91a1b0d505cc221f0e201781466ba1e2d6dc7b624b9bc75a03ce3dbb0f92` & `dipdup-7.0.0rc3/tests/replays/a3ce91a1b0d505cc221f0e201781466ba1e2d6dc7b624b9bc75a03ce3dbb0f92`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/a795ef429bde71b3ba66b545c0048f57a78ab5d2247772761d8efe86567199b9` & `dipdup-7.0.0rc3/tests/replays/a795ef429bde71b3ba66b545c0048f57a78ab5d2247772761d8efe86567199b9`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/aa8fe6037996b296bf9a3011e45cd9ecb92fb728592a843f91b03b2848cb1fb1` & `dipdup-7.0.0rc3/tests/replays/aa8fe6037996b296bf9a3011e45cd9ecb92fb728592a843f91b03b2848cb1fb1`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/acc952ba1905717315212f952ed689d7b8f683165b31c0a7a25199aed9fda27f` & `dipdup-7.0.0rc3/tests/replays/acc952ba1905717315212f952ed689d7b8f683165b31c0a7a25199aed9fda27f`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/b3af887f7ad8172af75b94a09bedfb9ae1e14f8819a36d6ce9f709721068263b` & `dipdup-7.0.0rc3/tests/replays/b3af887f7ad8172af75b94a09bedfb9ae1e14f8819a36d6ce9f709721068263b`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/b49fb33ee80345b70414ad08806a860e2139c20d98a5150c6ccd1b28a90f311e` & `dipdup-7.0.0rc3/tests/replays/b49fb33ee80345b70414ad08806a860e2139c20d98a5150c6ccd1b28a90f311e`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/bec4433b4206f00c2310a7961cff7f539434b9161b45673793aa5a3b50234313` & `dipdup-7.0.0rc3/tests/replays/bec4433b4206f00c2310a7961cff7f539434b9161b45673793aa5a3b50234313`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/c0202a433296436c27458b3d5ec5c72d5e2d47ff77c939ce399780cc0f3e56bc` & `dipdup-7.0.0rc3/tests/replays/c0202a433296436c27458b3d5ec5c72d5e2d47ff77c939ce399780cc0f3e56bc`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/c369836c15d9ed15477002b850d5cbb96b1ff5ff33e917b812ab9c0905063957` & `dipdup-7.0.0rc3/tests/replays/c369836c15d9ed15477002b850d5cbb96b1ff5ff33e917b812ab9c0905063957`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/c8e8698717ada415bc10405da983c8357165914dd0219f3d09bb9a939705242d` & `dipdup-7.0.0rc3/tests/replays/c8e8698717ada415bc10405da983c8357165914dd0219f3d09bb9a939705242d`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/cc162df04c4990c79f7507dd915601fd4d58c947a248156cbe302a64adfe898a` & `dipdup-7.0.0rc3/tests/replays/cc162df04c4990c79f7507dd915601fd4d58c947a248156cbe302a64adfe898a`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/cc5d3d4a58d5cb6bc7270d38c797b7740b79f913590ef0164abd50e58fba9405` & `dipdup-7.0.0rc3/tests/replays/cc5d3d4a58d5cb6bc7270d38c797b7740b79f913590ef0164abd50e58fba9405`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/d0a594d14bcb3fbf916092ec6707dfd3c9f48f53f0a1ad40a32023e7a87f8ef5` & `dipdup-7.0.0rc3/tests/replays/d0a594d14bcb3fbf916092ec6707dfd3c9f48f53f0a1ad40a32023e7a87f8ef5`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/d62748a927a09395579b5790c8f871cc8653081cf4475abc93173989f950b92b` & `dipdup-7.0.0rc3/tests/replays/d62748a927a09395579b5790c8f871cc8653081cf4475abc93173989f950b92b`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/d94397f6ecec8ce25f87177fe410f6498d7d30a04360506c0cd300d291c167e7` & `dipdup-7.0.0rc3/tests/replays/d94397f6ecec8ce25f87177fe410f6498d7d30a04360506c0cd300d291c167e7`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/dc86d5e346c85e6f7953d7e01298a9db64d778e5ba717ddd07fff8b589081e98` & `dipdup-7.0.0rc3/tests/replays/dc86d5e346c85e6f7953d7e01298a9db64d778e5ba717ddd07fff8b589081e98`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/dca9cf4f9f27623f10975d369444899458ab9ea85c22af2da6ce6ce8c09c2b58` & `dipdup-7.0.0rc3/tests/replays/dca9cf4f9f27623f10975d369444899458ab9ea85c22af2da6ce6ce8c09c2b58`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/df62701276d6dbf4860058cc582c0b4f7b583758f4f5be96c9ee045757c151e3` & `dipdup-7.0.0rc3/tests/replays/df62701276d6dbf4860058cc582c0b4f7b583758f4f5be96c9ee045757c151e3`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/e39ebba701031aa13dfd9eb5dba1effd2938e96682d1030dcbd70172f9f190a9` & `dipdup-7.0.0rc3/tests/replays/e39ebba701031aa13dfd9eb5dba1effd2938e96682d1030dcbd70172f9f190a9`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/e4a563a0b19379a44e9d2dc398131e9fd30d6039ff4ffacf1252db0bf8b433aa` & `dipdup-7.0.0rc3/tests/replays/e4a563a0b19379a44e9d2dc398131e9fd30d6039ff4ffacf1252db0bf8b433aa`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/eb8b6b33cb2e165d1a3a73c09938d3083671a82ad73d4c0cff1fb2a5e5715f76` & `dipdup-7.0.0rc3/tests/replays/eb8b6b33cb2e165d1a3a73c09938d3083671a82ad73d4c0cff1fb2a5e5715f76`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/eb8e2c3ce2fe7792d2c8e81c61d37821275b64021343103b0c955042ae802189` & `dipdup-7.0.0rc3/tests/replays/eb8e2c3ce2fe7792d2c8e81c61d37821275b64021343103b0c955042ae802189`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/ece1ebe13f9391555230d6b94f33d66a922e2ca71ef5fd39bbd8c2c37ddf54ec` & `dipdup-7.0.0rc3/tests/replays/ece1ebe13f9391555230d6b94f33d66a922e2ca71ef5fd39bbd8c2c37ddf54ec`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/ed3ec9fd9226e9f765b96dc1d5d5a455a7b2505da530961826910b08db693070` & `dipdup-7.0.0rc3/tests/replays/ed3ec9fd9226e9f765b96dc1d5d5a455a7b2505da530961826910b08db693070`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/f3d608f99e6b92e28a064bb9c10c3c605c9c817383c1eebcc68f663d1d23d650` & `dipdup-7.0.0rc3/tests/replays/f3d608f99e6b92e28a064bb9c10c3c605c9c817383c1eebcc68f663d1d23d650`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/f60e794a9be14263cb10e48546ba5610302cc3e7af0a114a593bb50eb85ba5e7` & `dipdup-7.0.0rc3/tests/replays/f60e794a9be14263cb10e48546ba5610302cc3e7af0a114a593bb50eb85ba5e7`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/replays/ff51b3535acc2972090ecd5db3af8f827464c9d92f1aa661630976e5b4ed4cbe` & `dipdup-7.0.0rc3/tests/replays/ff51b3535acc2972090ecd5db3af8f827464c9d92f1aa661630976e5b4ed4cbe`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/responses/asdf.json` & `dipdup-7.0.0rc3/tests/responses/asdf.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/responses/ftzfun.json` & `dipdup-7.0.0rc3/tests/responses/ftzfun.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/responses/hen_subjkt.json` & `dipdup-7.0.0rc3/tests/responses/hen_subjkt.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/responses/hjkl.json` & `dipdup-7.0.0rc3/tests/responses/hjkl.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/responses/kolibri_ovens.json` & `dipdup-7.0.0rc3/tests/responses/kolibri_ovens.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/responses/ooQuCAKBHkmWy2VciDAV9c6CFTywuMLupLzVoKDwS1xvR4EdRng.json` & `dipdup-7.0.0rc3/tests/responses/ooQuCAKBHkmWy2VciDAV9c6CFTywuMLupLzVoKDwS1xvR4EdRng.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/responses/origination_amount.json` & `dipdup-7.0.0rc3/tests/responses/origination_amount.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/responses/qwer.json` & `dipdup-7.0.0rc3/tests/responses/qwer.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/responses/rewq.json` & `dipdup-7.0.0rc3/tests/responses/rewq.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/responses/yupana.json` & `dipdup-7.0.0rc3/tests/responses/yupana.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/responses/zxcv.json` & `dipdup-7.0.0rc3/tests/responses/zxcv.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/schemas/asdf/storage.json` & `dipdup-7.0.0rc3/tests/schemas/asdf/storage.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/schemas/hen_subjkt/storage.json` & `dipdup-7.0.0rc3/tests/schemas/hen_subjkt/storage.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/schemas/hjkl/storage.json` & `dipdup-7.0.0rc3/tests/schemas/hjkl/storage.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/schemas/kolibri_ovens/storage.json` & `dipdup-7.0.0rc3/tests/schemas/kolibri_ovens/storage.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/schemas/qwer/storage.json` & `dipdup-7.0.0rc3/tests/schemas/qwer/storage.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/schemas/rewq/storage.json` & `dipdup-7.0.0rc3/tests/schemas/rewq/storage.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/schemas/yupana/storage.json` & `dipdup-7.0.0rc3/tests/schemas/yupana/storage.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/schemas/zxcv/storage.json` & `dipdup-7.0.0rc3/tests/schemas/zxcv/storage.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/test_config/test_callbacks.py` & `dipdup-7.0.0rc3/tests/test_config/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/test_config/test_config.py` & `dipdup-7.0.0rc3/tests/test_config/test_config.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/test_config/test_custom_config.py` & `dipdup-7.0.0rc3/tests/test_config/test_custom_config.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/test_context.py` & `dipdup-7.0.0rc3/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/test_datasources/test_ipfs.py` & `dipdup-7.0.0rc3/tests/test_datasources/test_ipfs.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/test_datasources/test_metadata.py` & `dipdup-7.0.0rc3/tests/test_datasources/test_metadata.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/test_datasources/test_tzkt.py` & `dipdup-7.0.0rc3/tests/test_datasources/test_tzkt.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/test_datasources/test_tzkt_blocks.py` & `dipdup-7.0.0rc3/tests/test_datasources/test_tzkt_blocks.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/test_datasources/test_tzkt_buffer.py` & `dipdup-7.0.0rc3/tests/test_datasources/test_tzkt_buffer.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/test_datasources/test_tzkt_quotes.py` & `dipdup-7.0.0rc3/tests/test_datasources/test_tzkt_quotes.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/test_demos.py` & `dipdup-7.0.0rc3/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/test_dipdup.py` & `dipdup-7.0.0rc3/tests/test_dipdup.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/test_hasura.py` & `dipdup-7.0.0rc3/tests/test_hasura.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/test_index/test_operation.py` & `dipdup-7.0.0rc3/tests/test_index/test_operation.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/test_introspection.py` & `dipdup-7.0.0rc3/tests/test_introspection.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/test_models.py` & `dipdup-7.0.0rc3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/test_rollback.py` & `dipdup-7.0.0rc3/tests/test_rollback.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/test_utils.py` & `dipdup-7.0.0rc3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/types/bazaar/storage.py` & `dipdup-7.0.0rc3/tests/types/bazaar/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/types/ftzfun/storage.py` & `dipdup-7.0.0rc3/tests/types/ftzfun/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/types/hen_subjkt/storage.py` & `dipdup-7.0.0rc3/tests/types/hen_subjkt/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/types/hjkl/storage.py` & `dipdup-7.0.0rc3/tests/types/hjkl/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/types/qwer/storage.py` & `dipdup-7.0.0rc3/tests/types/qwer/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/types/rewq/storage.py` & `dipdup-7.0.0rc3/tests/types/rewq/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/types/tezotop/storage.py` & `dipdup-7.0.0rc3/tests/types/tezotop/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/types/yupana/storage.py` & `dipdup-7.0.0rc3/tests/types/yupana/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/tests/types/zxcv/storage.py` & `dipdup-7.0.0rc3/tests/types/zxcv/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc2/PKG-INFO` & `dipdup-7.0.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dipdup
-Version: 7.0.0rc2
+Version: 7.0.0rc3
 Summary: Modular framework for creating selective indexers and featureful backends for dapps
 Keywords: api backend blockchain crypto cryptocurrencies dapp declarative ethereum evm framework indexer indexers michelson scheduler sdk smart-contracts tezos tzkt
 Author-Email: Lev Gorodetskii <dipdup@drsr.io>, Vladimir Bobrikov <vladimir_bobrikov@pm.me>, Michael Zaikin <mz@baking-bad.org>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,15 @@
 Project-URL: Homepage, https://dipdup.io/
 Project-URL: Documentation, https://dipdup.io/docs
 Project-URL: Repository, https://github.com/dipdup-io/dipdup
 Requires-Python: <3.12,>=3.11
 Requires-Dist: asyncpg~=0.28.0
 Requires-Dist: datamodel-code-generator~=0.21.1
 Requires-Dist: pydantic~=1.10.11
-Requires-Dist: tortoise-orm===0.19.3
+Requires-Dist: tortoise-orm==0.19.3
 Requires-Dist: aiohttp~=3.8
 Requires-Dist: aiolimiter~=1.0
 Requires-Dist: anyio~=3.3
 Requires-Dist: APScheduler~=3.8
 Requires-Dist: async-lru~=2.0
 Requires-Dist: asyncclick~=8.0
 Requires-Dist: eth-abi~=4.0
@@ -34,15 +34,15 @@
 Requires-Dist: prometheus-client~=0.17
 Requires-Dist: pyarrow~=12.0
 Requires-Dist: pycryptodome~=3.17
 Requires-Dist: pyhumps~=3.0
 Requires-Dist: pysignalr~=0.2
 Requires-Dist: python-dotenv~=1.0
 Requires-Dist: ruamel.yaml~=0.17
-Requires-Dist: sentry-sdk~=1.4
+Requires-Dist: sentry-sdk~=1.29
 Requires-Dist: sqlparse~=0.4
 Requires-Dist: survey~=4.4
 Requires-Dist: tabulate~=0.9
 Requires-Dist: web3~=6.2
 Description-Content-Type: text/markdown
 
 [![Twitter](https://badgen.net/badge/icon/dipdup_io?icon=twitter&label=)](https://twitter.com/dipdup_io)
@@ -62,15 +62,15 @@
 
 - **Ready to build your first indexer?** Head to [Quickstart](https://dipdup.io/docs/quickstart).
 
 - **Looking for examples?** Check out [Demo Projects](https://dipdup.io/docs/examples/demos) and [Built with DipDup](https://dipdup.io/docs/examples/built-with-dipdup) pages.
 
 - **Want to participate?** Vote for [open issues](https://github.com/dipdup-io/dipdup/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc), join [discussions](https://github.com/dipdup-io/dipdup/discussions) or [become a sponsor](https://github.com/sponsors/dipdup-io).
 
-- **Have a question?** Join our [Discord](https://discord.gg/NbANhqCJHA) or tag @dipdup_io on [Twitter](https://twitter.com/dipdup_io).
+- **Have a question?** Join our [Discord](https://discord.gg/aG8XKuwsQd) or tag @dipdup_io on [Twitter](https://twitter.com/dipdup_io).
 
 This project is maintained by the [Baking Bad](https://bakingbad.dev/) team.
 <br>
 Development is supported by [Tezos Foundation](https://tezos.foundation/) and [OnlyDust](https://www.onlydust.xyz).
 
 ## Thanks
```

