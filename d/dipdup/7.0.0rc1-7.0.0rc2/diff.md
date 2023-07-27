# Comparing `tmp/dipdup-7.0.0rc1.tar.gz` & `tmp/dipdup-7.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dipdup-7.0.0rc1.tar", last modified: Fri Jul 21 13:04:17 2023, max compression
+gzip compressed data, was "dipdup-7.0.0rc2.tar", last modified: Thu Jul 27 00:48:02 2023, max compression
```

## Comparing `dipdup-7.0.0rc1.tar` & `dipdup-7.0.0rc2.tar`

### file list

```diff
@@ -1,1111 +1,1112 @@
--rw-r--r--   0        0        0     1067 2023-07-21 12:53:39.283624 dipdup-7.0.0rc1/LICENSE
--rw-r--r--   0        0        0     3783 2023-07-21 12:53:39.283624 dipdup-7.0.0rc1/README.md
--rw-r--r--   0        0        0     4491 2023-07-21 13:04:17.446156 dipdup-7.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0      255 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/.gitignore
--rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_auction/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_auction/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1155 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/README.md
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      149 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      399 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      400 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/configs/replay.yaml
--rw-r--r--   0        0        0      356 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/deploy/.keep
--rw-r--r--   0        0        0      148 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/deploy/Dockerfile
--rw-r--r--   0        0        0      348 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2686 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1247 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/deploy/compose.yaml
--rw-r--r--   0        0        0      279 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/deploy/sqlite.env.default
--rw-r--r--   0        0        0      318 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/deploy/swarm.env.default
--rw-r--r--   0        0        0     1132 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/handlers/.keep
--rw-r--r--   0        0        0      913 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/handlers/on_bid.py
--rw-r--r--   0        0        0     1619 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/handlers/on_create_auction.py
--rw-r--r--   0        0        0      712 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/handlers/on_withdraw.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/models/.keep
--rw-r--r--   0        0        0     1445 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:55:57.658913 dipdup-7.0.0rc1/src/demo_auction/py.typed
--rw-r--r--   0        0        0     1089 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/types/.keep
--rw-r--r--   0        0        0      177 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/types/tzcolors_auction/tezos_parameters/bid.py
--rw-r--r--   0        0        0      381 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/types/tzcolors_auction/tezos_parameters/create_auction.py
--rw-r--r--   0        0        0      187 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/types/tzcolors_auction/tezos_parameters/withdraw.py
--rw-r--r--   0        0        0      555 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/types/tzcolors_auction/tezos_storage.py
--rw-r--r--   0        0        0      255 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/.gitignore
--rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_big_maps/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_big_maps/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1158 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/README.md
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      150 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      401 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      404 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/configs/replay.yaml
--rw-r--r--   0        0        0      356 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/deploy/.keep
--rw-r--r--   0        0        0      150 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/deploy/Dockerfile
--rw-r--r--   0        0        0      350 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2688 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1248 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/deploy/compose.yaml
--rw-r--r--   0        0        0      280 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/deploy/sqlite.env.default
--rw-r--r--   0        0        0      318 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/deploy/swarm.env.default
--rw-r--r--   0        0        0      781 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/handlers/.keep
--rw-r--r--   0        0        0      846 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/handlers/on_update_expiry_map.py
--rw-r--r--   0        0        0     1688 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/handlers/on_update_records.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/models/.keep
--rw-r--r--   0        0        0      667 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:56:31.459605 dipdup-7.0.0rc1/src/demo_big_maps/py.typed
--rw-r--r--   0        0        0     1093 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/types/.keep
--rw-r--r--   0        0        0      199 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/types/name_registry/tezos_big_maps/store_expiry_map_key.py
--rw-r--r--   0        0        0      203 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/types/name_registry/tezos_big_maps/store_expiry_map_value.py
--rw-r--r--   0        0        0      194 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/types/name_registry/tezos_big_maps/store_records_key.py
--rw-r--r--   0        0        0      489 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/types/name_registry/tezos_big_maps/store_records_value.py
--rw-r--r--   0        0        0      255 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/.gitignore
--rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_blank/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_blank/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1159 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/README.md
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      147 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      395 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      402 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/configs/replay.yaml
--rw-r--r--   0        0        0      327 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/deploy/.keep
--rw-r--r--   0        0        0      144 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/deploy/Dockerfile
--rw-r--r--   0        0        0      344 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2682 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1245 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/deploy/compose.yaml
--rw-r--r--   0        0        0      248 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/deploy/sqlite.env.default
--rw-r--r--   0        0        0      289 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/deploy/swarm.env.default
--rw-r--r--   0        0        0       37 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/handlers/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/models/.keep
--rw-r--r--   0        0        0     1242 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/models/__init__.py
--rw-r--r--   0        0        0     1091 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/types/.keep
--rw-r--r--   0        0        0      255 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/.gitignore
--rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_dao/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_dao/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1148 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/README.md
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      145 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      391 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      389 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/configs/replay.yaml
--rw-r--r--   0        0        0      356 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/deploy/.keep
--rw-r--r--   0        0        0      140 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/deploy/Dockerfile
--rw-r--r--   0        0        0      340 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2678 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1243 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/deploy/compose.yaml
--rw-r--r--   0        0        0      275 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/deploy/sqlite.env.default
--rw-r--r--   0        0        0      318 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/deploy/swarm.env.default
--rw-r--r--   0        0        0      694 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/handlers/.keep
--rw-r--r--   0        0        0      408 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/handlers/on_origination.py
--rw-r--r--   0        0        0      506 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/handlers/on_propose.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/models/.keep
--rw-r--r--   0        0        0      782 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:56:12.871220 dipdup-7.0.0rc1/src/demo_dao/py.typed
--rw-r--r--   0        0        0     1078 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/types/.keep
--rw-r--r--   0        0        0      360 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/types/registry/tezos_parameters/propose.py
--rw-r--r--   0        0        0     2523 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/types/registry/tezos_storage.py
--rw-r--r--   0        0        0      255 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/.gitignore
--rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_dex/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_dex/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1163 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/README.md
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      145 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      391 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      404 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/configs/replay.yaml
--rw-r--r--   0        0        0      327 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/deploy/.keep
--rw-r--r--   0        0        0      140 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/deploy/Dockerfile
--rw-r--r--   0        0        0      340 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2678 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1243 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/deploy/compose.yaml
--rw-r--r--   0        0        0      246 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/deploy/sqlite.env.default
--rw-r--r--   0        0        0      289 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/deploy/swarm.env.default
--rw-r--r--   0        0        0     4896 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/.keep
--rw-r--r--   0        0        0     1829 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_divest_liquidity.py
--rw-r--r--   0        0        0     1737 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_invest_liquidity.py
--rw-r--r--   0        0        0      579 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_origination.py
--rw-r--r--   0        0        0     1610 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_tez_to_token.py
--rw-r--r--   0        0        0     1676 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_token_to_tez.py
--rw-r--r--   0        0        0     1022 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_transfer.py
--rw-r--r--   0        0        0      962 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_withdraw_profit.py
--rw-r--r--   0        0        0     1855 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa2_divest_liquidity.py
--rw-r--r--   0        0        0     1763 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa2_invest_liquidity.py
--rw-r--r--   0        0        0      573 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa2_origination.py
--rw-r--r--   0        0        0     1604 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa2_tez_to_token.py
--rw-r--r--   0        0        0     1642 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa2_token_to_tez.py
--rw-r--r--   0        0        0     1143 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa2_transfer.py
--rw-r--r--   0        0        0      958 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa2_withdraw_profit.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/models/.keep
--rw-r--r--   0        0        0      916 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:55:45.466652 dipdup-7.0.0rc1/src/demo_dex/py.typed
--rw-r--r--   0        0        0     1093 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/.keep
--rw-r--r--   0        0        0      340 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/fa12_token/tezos_parameters/transfer.py
--rw-r--r--   0        0        0      739 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/fa12_token/tezos_storage.py
--rw-r--r--   0        0        0      504 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/fa2_token/tezos_parameters/transfer.py
--rw-r--r--   0        0        0     1093 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/fa2_token/tezos_storage.py
--rw-r--r--   0        0        0      311 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa12/tezos_parameters/divest_liquidity.py
--rw-r--r--   0        0        0      201 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa12/tezos_parameters/invest_liquidity.py
--rw-r--r--   0        0        0      297 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa12/tezos_parameters/tez_to_token_payment.py
--rw-r--r--   0        0        0      313 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa12/tezos_parameters/token_to_tez_payment.py
--rw-r--r--   0        0        0      340 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa12/tezos_parameters/transfer.py
--rw-r--r--   0        0        0      199 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa12/tezos_parameters/withdraw_profit.py
--rw-r--r--   0        0        0     1455 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa12/tezos_storage.py
--rw-r--r--   0        0        0      311 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa2/tezos_parameters/divest_liquidity.py
--rw-r--r--   0        0        0      201 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa2/tezos_parameters/invest_liquidity.py
--rw-r--r--   0        0        0      297 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa2/tezos_parameters/tez_to_token_payment.py
--rw-r--r--   0        0        0      313 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa2/tezos_parameters/token_to_tez_payment.py
--rw-r--r--   0        0        0      504 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa2/tezos_parameters/transfer.py
--rw-r--r--   0        0        0      199 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa2/tezos_parameters/withdraw_profit.py
--rw-r--r--   0        0        0     1491 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa2/tezos_storage.py
--rw-r--r--   0        0        0      255 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/.gitignore
--rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_domains/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_domains/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1157 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/README.md
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      149 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      399 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      402 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/configs/replay.yaml
--rw-r--r--   0        0        0      356 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/deploy/.keep
--rw-r--r--   0        0        0      148 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/deploy/Dockerfile
--rw-r--r--   0        0        0      348 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2686 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1247 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/deploy/compose.yaml
--rw-r--r--   0        0        0      279 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/deploy/sqlite.env.default
--rw-r--r--   0        0        0      318 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/deploy/swarm.env.default
--rw-r--r--   0        0        0      900 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/handlers/.keep
--rw-r--r--   0        0        0      553 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/handlers/on_admin_update.py
--rw-r--r--   0        0        0      525 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/handlers/on_execute.py
--rw-r--r--   0        0        0     1437 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/handlers/on_storage_diff.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/models/.keep
--rw-r--r--   0        0        0      630 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:55:31.318375 dipdup-7.0.0rc1/src/demo_domains/py.typed
--rw-r--r--   0        0        0     1091 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/types/.keep
--rw-r--r--   0        0        0      194 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/types/name_registry/tezos_parameters/admin_update.py
--rw-r--r--   0        0        0      305 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/types/name_registry/tezos_parameters/execute.py
--rw-r--r--   0        0        0     1134 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/types/name_registry/tezos_storage.py
--rw-r--r--   0        0        0      255 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/.gitignore
--rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_events/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_events/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1156 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/README.md
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      148 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      397 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      400 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/configs/replay.yaml
--rw-r--r--   0        0        0      327 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/deploy/.keep
--rw-r--r--   0        0        0      146 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/deploy/Dockerfile
--rw-r--r--   0        0        0      346 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2684 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1246 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/deploy/compose.yaml
--rw-r--r--   0        0        0      249 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/deploy/sqlite.env.default
--rw-r--r--   0        0        0      289 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/deploy/swarm.env.default
--rw-r--r--   0        0        0      590 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/handlers/.keep
--rw-r--r--   0        0        0      311 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/handlers/on_move_event.py
--rw-r--r--   0        0        0      237 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/handlers/on_other_event.py
--rw-r--r--   0        0        0      311 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/handlers/on_roll_event.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/models/.keep
--rw-r--r--   0        0        0     1242 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/models/__init__.py
--rw-r--r--   0        0        0     1089 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/types/.keep
--rw-r--r--   0        0        0      317 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/types/events_contract/tezos_events/move.py
--rw-r--r--   0        0        0      266 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/types/events_contract/tezos_events/roll.py
--rw-r--r--   0        0        0      255 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/.gitignore
--rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_evm_events/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_evm_events/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1173 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/README.md
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/abi/.keep
--rw-r--r--   0        0        0    11460 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/abi/eth_usdt/abi.json
--rw-r--r--   0        0        0     2420 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/abi/eth_usdt/events.json
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      152 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      405 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      421 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/configs/replay.yaml
--rw-r--r--   0        0        0      409 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/deploy/.keep
--rw-r--r--   0        0        0      154 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/deploy/Dockerfile
--rw-r--r--   0        0        0      354 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2692 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1250 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/deploy/compose.yaml
--rw-r--r--   0        0        0      335 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/deploy/sqlite.env.default
--rw-r--r--   0        0        0      371 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/deploy/swarm.env.default
--rw-r--r--   0        0        0      752 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/handlers/.keep
--rw-r--r--   0        0        0      992 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/handlers/on_transfer.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/models/.keep
--rw-r--r--   0        0        0      368 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/models/__init__.py
--rw-r--r--   0        0        0     1110 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/types/.keep
--rw-r--r--   0        0        0      331 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/types/eth_usdt/evm_events/transfer.py
--rw-r--r--   0        0        0      255 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/.gitignore
--rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_factories/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_factories/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1172 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/README.md
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      151 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      403 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      419 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/configs/replay.yaml
--rw-r--r--   0        0        0      356 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/deploy/.keep
--rw-r--r--   0        0        0      152 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/deploy/Dockerfile
--rw-r--r--   0        0        0      352 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2690 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1249 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/deploy/compose.yaml
--rw-r--r--   0        0        0      281 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/deploy/sqlite.env.default
--rw-r--r--   0        0        0      318 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/deploy/swarm.env.default
--rw-r--r--   0        0        0      704 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/handlers/.keep
--rw-r--r--   0        0        0      420 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/handlers/on_origination.py
--rw-r--r--   0        0        0      524 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/handlers/on_propose.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/models/.keep
--rw-r--r--   0        0        0      782 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:56:27.503526 dipdup-7.0.0rc1/src/demo_factories/py.typed
--rw-r--r--   0        0        0     1108 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/types/.keep
--rw-r--r--   0        0        0      360 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/types/registry/tezos_parameters/propose.py
--rw-r--r--   0        0        0     2523 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/types/registry/tezos_storage.py
--rw-r--r--   0        0        0      255 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/.gitignore
--rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_head/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_head/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1158 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/README.md
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      146 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      393 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      400 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/configs/replay.yaml
--rw-r--r--   0        0        0      356 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/deploy/.keep
--rw-r--r--   0        0        0      142 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/deploy/Dockerfile
--rw-r--r--   0        0        0      342 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2680 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1244 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/deploy/compose.yaml
--rw-r--r--   0        0        0      276 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/deploy/sqlite.env.default
--rw-r--r--   0        0        0      318 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/deploy/swarm.env.default
--rw-r--r--   0        0        0      292 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/handlers/.keep
--rw-r--r--   0        0        0      237 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/handlers/on_mainnet_head.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/models/.keep
--rw-r--r--   0        0        0     1242 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/models/__init__.py
--rw-r--r--   0        0        0     1089 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/types/.keep
--rw-r--r--   0        0        0      255 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/.gitignore
--rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_nft_marketplace/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_nft_marketplace/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1166 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/README.md
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      157 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      415 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      419 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/configs/replay.yaml
--rw-r--r--   0        0        0      452 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/deploy/.keep
--rw-r--r--   0        0        0      164 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/deploy/Dockerfile
--rw-r--r--   0        0        0      364 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2702 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1255 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/deploy/compose.yaml
--rw-r--r--   0        0        0      383 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/deploy/sqlite.env.default
--rw-r--r--   0        0        0      414 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/deploy/swarm.env.default
--rw-r--r--   0        0        0     1262 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/handlers/.keep
--rw-r--r--   0        0        0      605 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/handlers/on_cancel_swap.py
--rw-r--r--   0        0        0     1037 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/handlers/on_collect.py
--rw-r--r--   0        0        0      977 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/handlers/on_mint.py
--rw-r--r--   0        0        0      885 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/handlers/on_swap.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/models/.keep
--rw-r--r--   0        0        0     1306 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:55:43.058599 dipdup-7.0.0rc1/src/demo_nft_marketplace/py.typed
--rw-r--r--   0        0        0     1108 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/types/.keep
--rw-r--r--   0        0        0      192 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/cancel_swap.py
--rw-r--r--   0        0        0      281 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/collect.py
--rw-r--r--   0        0        0      317 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/mint_objkt.py
--rw-r--r--   0        0        0      299 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/swap.py
--rw-r--r--   0        0        0      777 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/types/hen_minter/tezos_storage.py
--rw-r--r--   0        0        0      343 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/types/hen_objkts/tezos_parameters/mint.py
--rw-r--r--   0        0        0     1094 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/types/hen_objkts/tezos_storage.py
--rw-r--r--   0        0        0      255 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/.gitignore
--rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_raw/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_raw/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1185 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/README.md
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      145 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      391 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      426 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/configs/replay.yaml
--rw-r--r--   0        0        0      356 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/deploy/.keep
--rw-r--r--   0        0        0      140 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/deploy/Dockerfile
--rw-r--r--   0        0        0      340 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2678 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1243 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/deploy/compose.yaml
--rw-r--r--   0        0        0      275 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/deploy/sqlite.env.default
--rw-r--r--   0        0        0      318 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/deploy/swarm.env.default
--rw-r--r--   0        0        0      462 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/handlers/.keep
--rw-r--r--   0        0        0      350 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/handlers/on_operation.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_raw/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_raw/models/.keep
--rw-r--r--   0        0        0      245 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_raw/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:56:38.667706 dipdup-7.0.0rc1/src/demo_raw/py.typed
--rw-r--r--   0        0        0     1115 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_raw/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_raw/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_raw/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_raw/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_raw/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_raw/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_raw/types/.keep
--rw-r--r--   0        0        0      255 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/.gitignore
--rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_token/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_token/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1157 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/README.md
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      147 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      395 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      400 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/configs/replay.yaml
--rw-r--r--   0        0        0      327 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/deploy/.keep
--rw-r--r--   0        0        0      144 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/deploy/Dockerfile
--rw-r--r--   0        0        0      344 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2682 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1245 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/deploy/compose.yaml
--rw-r--r--   0        0        0      248 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/deploy/sqlite.env.default
--rw-r--r--   0        0        0      289 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/deploy/swarm.env.default
--rw-r--r--   0        0        0      783 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/handlers/.keep
--rw-r--r--   0        0        0      436 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/handlers/on_balance_update.py
--rw-r--r--   0        0        0      630 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/handlers/on_mint.py
--rw-r--r--   0        0        0      928 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/handlers/on_transfer.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/models/.keep
--rw-r--r--   0        0        0      370 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:55:31.318375 dipdup-7.0.0rc1/src/demo_token/py.typed
--rw-r--r--   0        0        0     1089 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/types/.keep
--rw-r--r--   0        0        0      263 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/types/tzbtc/tezos_parameters/mint.py
--rw-r--r--   0        0        0      340 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/types/tzbtc/tezos_parameters/transfer.py
--rw-r--r--   0        0        0      398 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/types/tzbtc/tezos_storage.py
--rw-r--r--   0        0        0      255 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/.gitignore
--rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_token_transfers/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_token_transfers/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1166 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/README.md
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/abi/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      157 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      415 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      419 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/configs/replay.yaml
--rw-r--r--   0        0        0      327 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/deploy/.keep
--rw-r--r--   0        0        0      164 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/deploy/Dockerfile
--rw-r--r--   0        0        0      364 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2702 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1255 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/deploy/compose.yaml
--rw-r--r--   0        0        0      258 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/deploy/sqlite.env.default
--rw-r--r--   0        0        0      289 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/deploy/swarm.env.default
--rw-r--r--   0        0        0      472 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/handlers/.keep
--rw-r--r--   0        0        0      545 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/handlers/on_balance_update.py
--rw-r--r--   0        0        0      836 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/handlers/on_token_transfer.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/models/.keep
--rw-r--r--   0        0        0      370 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:56:09.391146 dipdup-7.0.0rc1/src/demo_token_transfers/py.typed
--rw-r--r--   0        0        0     1108 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/types/.keep
--rw-r--r--   0        0        0      255 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/.dockerignore
--rw-r--r--   0        0        0      341 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/.gitignore
--rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_uniswap/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_uniswap/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     1178 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/README.md
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/abi/.keep
--rw-r--r--   0        0        0     4418 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/abi/factory/abi.json
--rw-r--r--   0        0        0      919 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/abi/factory/events.json
--rw-r--r--   0        0        0    19609 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/abi/pool/abi.json
--rw-r--r--   0        0        0     3559 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/abi/pool/events.json
--rw-r--r--   0        0        0    24313 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/abi/position_manager/abi.json
--rw-r--r--   0        0        0     1984 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/abi/position_manager/events.json
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/configs/.keep
--rw-r--r--   0        0        0      379 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/configs/dipdup.compose.yaml
--rw-r--r--   0        0        0      149 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/configs/dipdup.sqlite.yaml
--rw-r--r--   0        0        0      399 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/configs/dipdup.swarm.yaml
--rw-r--r--   0        0        0      423 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/configs/replay.yaml
--rw-r--r--   0        0        0      424 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/deploy/.env.default
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/deploy/.keep
--rw-r--r--   0        0        0      148 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/deploy/Dockerfile
--rw-r--r--   0        0        0      348 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/deploy/compose.sqlite.yaml
--rw-r--r--   0        0        0     2686 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/deploy/compose.swarm.yaml
--rw-r--r--   0        0        0     1247 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/deploy/compose.yaml
--rw-r--r--   0        0        0      347 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/deploy/sqlite.env.default
--rw-r--r--   0        0        0      386 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/deploy/swarm.env.default
--rw-r--r--   0        0        0     2236 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/dipdup.yaml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/graphql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/handlers/.keep
--rw-r--r--   0        0        0     3060 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/handlers/factory/pool_created.py
--rw-r--r--   0        0        0      531 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/handlers/pool/burn.py
--rw-r--r--   0        0        0      291 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/handlers/pool/flash.py
--rw-r--r--   0        0        0      871 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/handlers/pool/initialize.py
--rw-r--r--   0        0        0     1330 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/handlers/pool/mint.py
--rw-r--r--   0        0        0     6558 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/handlers/pool/swap.py
--rw-r--r--   0        0        0     1227 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/handlers/position_manager/collect.py
--rw-r--r--   0        0        0     1361 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/handlers/position_manager/decrease_liquidity.py
--rw-r--r--   0        0        0     1449 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/handlers/position_manager/increase_liquidity.py
--rw-r--r--   0        0        0     1172 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/handlers/position_manager/transfer.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/hasura/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/hooks/.keep
--rw-r--r--   0        0        0      378 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/hooks/on_index_rollback.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/hooks/on_reindex.py
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/hooks/on_restart.py
--rw-r--r--   0        0        0      145 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/hooks/on_synchronized.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/models/.keep
--rw-r--r--   0        0        0    19932 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/models/__init__.py
--rw-r--r--   0        0        0      373 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/models/abi.py
--rw-r--r--   0        0        0     4162 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/models/pool.py
--rw-r--r--   0        0        0     2824 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/models/position.py
--rw-r--r--   0        0        0     1477 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/models/repo.py
--rw-r--r--   0        0        0      561 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/models/tick.py
--rw-r--r--   0        0        0     7160 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/models/token.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/py.typed
--rw-r--r--   0        0        0     1112 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/sql/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/sql/on_index_rollback/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/sql/on_reindex/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/sql/on_restart/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/sql/on_synchronized/.keep
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/types/.keep
--rw-r--r--   0        0        0      321 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/types/factory/evm_events/pool_created.py
--rw-r--r--   0        0        0      330 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/types/pool/evm_events/burn.py
--rw-r--r--   0        0        0      339 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/types/pool/evm_events/collect.py
--rw-r--r--   0        0        0      328 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/types/pool/evm_events/flash.py
--rw-r--r--   0        0        0      275 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/types/pool/evm_events/initialize.py
--rw-r--r--   0        0        0      346 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/types/pool/evm_events/mint.py
--rw-r--r--   0        0        0      351 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/types/pool/evm_events/swap.py
--rw-r--r--   0        0        0      303 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/types/position_manager/evm_events/collect.py
--rw-r--r--   0        0        0      323 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/types/position_manager/evm_events/decrease_liquidity.py
--rw-r--r--   0        0        0      323 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/types/position_manager/evm_events/increase_liquidity.py
--rw-r--r--   0        0        0      333 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/types/position_manager/evm_events/transfer.py
--rw-r--r--   0        0        0      213 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/__init__.py
--rw-r--r--   0        0        0      105 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/__main__.py
--rw-r--r--   0        0        0      512 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/api.py
--rw-r--r--   0        0        0    21805 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/cli.py
--rw-r--r--   0        0        0     7560 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/codegen/__init__.py
--rw-r--r--   0        0        0     7038 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/codegen/evm_subsquid.py
--rw-r--r--   0        0        0    18129 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/codegen/tezos_tzkt.py
--rw-r--r--   0        0        0    41898 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/config/__init__.py
--rw-r--r--   0        0        0      554 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/config/abi_etherscan.py
--rw-r--r--   0        0        0      690 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/config/coinbase.py
--rw-r--r--   0        0        0     1469 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/config/evm.py
--rw-r--r--   0        0        0     1273 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/config/evm_node.py
--rw-r--r--   0        0        0     1375 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/config/evm_subsquid.py
--rw-r--r--   0        0        0     2578 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/config/evm_subsquid_events.py
--rw-r--r--   0        0        0     1495 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/config/evm_subsquid_operations.py
--rw-r--r--   0        0        0      446 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/config/http.py
--rw-r--r--   0        0        0      519 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/config/ipfs.py
--rw-r--r--   0        0        0     1532 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/config/tezos.py
--rw-r--r--   0        0        0     2157 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/config/tezos_tzkt.py
--rw-r--r--   0        0        0     3758 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/config/tezos_tzkt_big_maps.py
--rw-r--r--   0        0        0     3074 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/config/tezos_tzkt_events.py
--rw-r--r--   0        0        0     1424 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/config/tezos_tzkt_head.py
--rw-r--r--   0        0        0    12744 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/config/tezos_tzkt_operations.py
--rw-r--r--   0        0        0     3110 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/config/tezos_tzkt_token_transfers.py
--rw-r--r--   0        0        0      745 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/config/tzip_metadata.py
--rw-r--r--   0        0        0    28058 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/context.py
--rw-r--r--   0        0        0    14006 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/database.py
--rw-r--r--   0        0        0     4474 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/datasources/__init__.py
--rw-r--r--   0        0        0      915 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/datasources/abi_etherscan.py
--rw-r--r--   0        0        0     2274 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/datasources/coinbase.py
--rw-r--r--   0        0        0    12321 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/datasources/evm_node.py
--rw-r--r--   0        0        0     4013 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/datasources/evm_subsquid.py
--rw-r--r--   0        0        0      399 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/datasources/http.py
--rw-r--r--   0        0        0      524 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/datasources/ipfs.py
--rw-r--r--   0        0        0    43369 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/datasources/tezos_tzkt.py
--rw-r--r--   0        0        0     1545 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/datasources/tzip_metadata.py
--rw-r--r--   0        0        0    30432 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/dipdup.py
--rw-r--r--   0        0        0     1803 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/env.py
--rw-r--r--   0        0        0     8274 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/exceptions.py
--rw-r--r--   0        0        0     3981 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/fetcher.py
--rw-r--r--   0        0        0     6724 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/fields.py
--rw-r--r--   0        0        0    25644 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/hasura.py
--rw-r--r--   0        0        0    11008 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/http.py
--rw-r--r--   0        0        0     7426 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/index.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/__init__.py
--rw-r--r--   0        0        0     1229 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/evm_subsquid_events/fetcher.py
--rw-r--r--   0        0        0    10389 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/evm_subsquid_events/index.py
--rw-r--r--   0        0        0     3439 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/evm_subsquid_events/matcher.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/evm_subsquid_events/parser.py
--rw-r--r--   0        0        0      406 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/evm_subsquid_operations/index.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_big_maps/__init__.py
--rw-r--r--   0        0        0     3181 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_big_maps/fetcher.py
--rw-r--r--   0        0        0     7320 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_big_maps/index.py
--rw-r--r--   0        0        0     2684 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_big_maps/matcher.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_events/__init__.py
--rw-r--r--   0        0        0     1480 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_events/fetcher.py
--rw-r--r--   0        0        0     5539 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_events/index.py
--rw-r--r--   0        0        0     3888 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_events/matcher.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_head/__init__.py
--rw-r--r--   0        0        0     2349 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_head/index.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_operations/__init__.py
--rw-r--r--   0        0        0    20276 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_operations/fetcher.py
--rw-r--r--   0        0        0    13485 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_operations/index.py
--rw-r--r--   0        0        0     9135 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_operations/matcher.py
--rw-r--r--   0        0        0     7612 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_operations/parser.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_token_transfers/__init__.py
--rw-r--r--   0        0        0     1432 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_token_transfers/fetcher.py
--rw-r--r--   0        0        0     5520 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_token_transfers/index.py
--rw-r--r--   0        0        0     1808 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_token_transfers/matcher.py
--rwxr-xr-x   0        0        0     9379 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/install.py
--rw-r--r--   0        0        0    20461 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/models/__init__.py
--rw-r--r--   0        0        0     1309 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/models/coinbase.py
--rw-r--r--   0        0        0     3596 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/models/evm_node.py
--rw-r--r--   0        0        0     5045 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/models/evm_subsquid.py
--rw-r--r--   0        0        0    19800 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/models/tezos_tzkt.py
--rw-r--r--   0        0        0      165 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/models/tzip_metadata.py
--rw-r--r--   0        0        0     6687 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/package.py
--rw-r--r--   0        0        0     7091 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/performance.py
--rw-r--r--   0        0        0     7834 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/project.py
--rw-r--r--   0        0        0      256 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/base/.dockerignore.j2
--rw-r--r--   0        0        0      341 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/base/.gitignore.j2
--rw-r--r--   0        0        0     1163 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/base/README.md.j2
--rw-r--r--   0        0        0      380 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/base/configs/dipdup.compose.yaml.j2
--rw-r--r--   0        0        0      159 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/base/configs/dipdup.sqlite.yaml.j2
--rw-r--r--   0        0        0      418 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/base/configs/dipdup.swarm.yaml.j2
--rw-r--r--   0        0        0      221 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/base/deploy/Dockerfile.j2
--rw-r--r--   0        0        0      367 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/base/deploy/compose.sqlite.yaml.j2
--rw-r--r--   0        0        0     2748 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/base/deploy/compose.swarm.yaml.j2
--rw-r--r--   0        0        0     1273 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/base/deploy/compose.yaml.j2
--rw-r--r--   0        0        0     1282 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/base/pyproject.toml.j2
--rw-r--r--   0        0        0     1151 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_auction/dipdup.yaml.j2
--rw-r--r--   0        0        0      935 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_auction/handlers/on_bid.py.j2
--rw-r--r--   0        0        0     1641 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_auction/handlers/on_create_auction.py.j2
--rw-r--r--   0        0        0      734 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_auction/handlers/on_withdraw.py.j2
--rw-r--r--   0        0        0     1448 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_auction/models/__init__.py.j2
--rw-r--r--   0        0        0      114 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_auction/replay.yaml
--rw-r--r--   0        0        0      798 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_big_maps/dipdup.yaml.j2
--rw-r--r--   0        0        0      865 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_big_maps/handlers/on_update_expiry_map.py.j2
--rw-r--r--   0        0        0     1707 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_big_maps/handlers/on_update_records.py.j2
--rw-r--r--   0        0        0      669 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_big_maps/models/__init__.py.j2
--rw-r--r--   0        0        0      118 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_big_maps/replay.yaml
--rw-r--r--   0        0        0       49 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_blank/dipdup.yaml.j2
--rw-r--r--   0        0        0      116 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_blank/replay.yaml
--rw-r--r--   0        0        0      721 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dao/dipdup.yaml.j2
--rw-r--r--   0        0        0      431 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dao/handlers/on_origination.py.j2
--rw-r--r--   0        0        0      540 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dao/handlers/on_propose.py.j2
--rw-r--r--   0        0        0      784 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dao/models/__init__.py.j2
--rw-r--r--   0        0        0      103 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dao/replay.yaml
--rw-r--r--   0        0        0     4923 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/dipdup.yaml.j2
--rw-r--r--   0        0        0     1885 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa12_divest_liquidity.py.j2
--rw-r--r--   0        0        0     1793 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa12_invest_liquidity.py.j2
--rw-r--r--   0        0        0      602 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa12_origination.py.j2
--rw-r--r--   0        0        0     1666 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa12_tez_to_token.py.j2
--rw-r--r--   0        0        0     1732 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa12_token_to_tez.py.j2
--rw-r--r--   0        0        0     1056 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa12_transfer.py.j2
--rw-r--r--   0        0        0      996 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa12_withdraw_profit.py.j2
--rw-r--r--   0        0        0     1911 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_divest_liquidity.py.j2
--rw-r--r--   0        0        0     1819 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_invest_liquidity.py.j2
--rw-r--r--   0        0        0      596 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_origination.py.j2
--rw-r--r--   0        0        0     1660 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_tez_to_token.py.j2
--rw-r--r--   0        0        0     1698 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_token_to_tez.py.j2
--rw-r--r--   0        0        0     1177 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_transfer.py.j2
--rw-r--r--   0        0        0      992 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_withdraw_profit.py.j2
--rw-r--r--   0        0        0      918 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/models/__init__.py.j2
--rw-r--r--   0        0        0      118 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/replay.yaml
--rw-r--r--   0        0        0      919 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_domains/dipdup.yaml.j2
--rw-r--r--   0        0        0      581 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_domains/handlers/on_admin_update.py.j2
--rw-r--r--   0        0        0      553 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_domains/handlers/on_execute.py.j2
--rw-r--r--   0        0        0     1456 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_domains/handlers/on_storage_diff.py.j2
--rw-r--r--   0        0        0      632 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_domains/models/__init__.py.j2
--rw-r--r--   0        0        0      116 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_domains/replay.yaml
--rw-r--r--   0        0        0      611 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_events/dipdup.yaml.j2
--rw-r--r--   0        0        0      114 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_events/replay.yaml
--rw-r--r--   0        0        0      765 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_evm_events/dipdup.yaml.j2
--rw-r--r--   0        0        0     1005 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_evm_events/handlers/on_transfer.py.j2
--rw-r--r--   0        0        0      370 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_evm_events/models/__init__.py.j2
--rw-r--r--   0        0        0      135 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_evm_events/replay.yaml
--rw-r--r--   0        0        0      719 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_factories/dipdup.yaml.j2
--rw-r--r--   0        0        0      431 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_factories/handlers/on_origination.py.j2
--rw-r--r--   0        0        0      540 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_factories/handlers/on_propose.py.j2
--rw-r--r--   0        0        0      784 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_factories/models/__init__.py.j2
--rw-r--r--   0        0        0      133 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_factories/replay.yaml
--rw-r--r--   0        0        0      317 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_head/dipdup.yaml.j2
--rw-r--r--   0        0        0      114 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_head/replay.yaml
--rw-r--r--   0        0        0     1265 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_nft_marketplace/dipdup.yaml.j2
--rw-r--r--   0        0        0      603 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_nft_marketplace/handlers/on_cancel_swap.py.j2
--rw-r--r--   0        0        0     1035 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_nft_marketplace/handlers/on_collect.py.j2
--rw-r--r--   0        0        0      973 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_nft_marketplace/handlers/on_mint.py.j2
--rw-r--r--   0        0        0      883 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_nft_marketplace/handlers/on_swap.py.j2
--rw-r--r--   0        0        0     1309 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_nft_marketplace/models/__init__.py.j2
--rw-r--r--   0        0        0      133 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_nft_marketplace/replay.yaml
--rw-r--r--   0        0        0      489 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_raw/dipdup.yaml.j2
--rw-r--r--   0        0        0      364 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_raw/handlers/on_operation.py.j2
--rw-r--r--   0        0        0      247 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_raw/models/__init__.py.j2
--rw-r--r--   0        0        0      140 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_raw/replay.yaml
--rw-r--r--   0        0        0      806 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_token/dipdup.yaml.j2
--rw-r--r--   0        0        0      448 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_token/handlers/on_balance_update.py.j2
--rw-r--r--   0        0        0      664 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_token/handlers/on_mint.py.j2
--rw-r--r--   0        0        0      962 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_token/handlers/on_transfer.py.j2
--rw-r--r--   0        0        0      372 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_token/models/__init__.py.j2
--rw-r--r--   0        0        0      114 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_token/replay.yaml
--rw-r--r--   0        0        0      475 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_token_transfers/dipdup.yaml.j2
--rw-r--r--   0        0        0      545 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_token_transfers/handlers/on_balance_update.py.j2
--rw-r--r--   0        0        0      836 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_token_transfers/handlers/on_token_transfer.py.j2
--rw-r--r--   0        0        0      372 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_token_transfers/models/__init__.py.j2
--rw-r--r--   0        0        0      133 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_token_transfers/replay.yaml
--rw-r--r--   0        0        0     2255 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/dipdup.yaml.j2
--rw-r--r--   0        0        0     3097 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/factory/pool_created.py.j2
--rw-r--r--   0        0        0      568 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/pool/burn.py.j2
--rw-r--r--   0        0        0      310 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/pool/flash.py.j2
--rw-r--r--   0        0        0      899 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/pool/initialize.py.j2
--rw-r--r--   0        0        0     1376 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/pool/mint.py.j2
--rw-r--r--   0        0        0     6631 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/pool/swap.py.j2
--rw-r--r--   0        0        0     1264 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/position_manager/collect.py.j2
--rw-r--r--   0        0        0     1398 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/position_manager/decrease_liquidity.py.j2
--rw-r--r--   0        0        0     1486 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/position_manager/increase_liquidity.py.j2
--rw-r--r--   0        0        0     1200 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/position_manager/transfer.py.j2
--rw-r--r--   0        0        0    19933 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/models/__init__.py.j2
--rw-r--r--   0        0        0      374 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/models/abi.py.j2
--rw-r--r--   0        0        0     4226 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/models/pool.py.j2
--rw-r--r--   0        0        0     2844 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/models/position.py.j2
--rw-r--r--   0        0        0     1478 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/models/repo.py.j2
--rw-r--r--   0        0        0      571 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/models/tick.py.j2
--rw-r--r--   0        0        0     7188 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/models/token.py.j2
--rw-r--r--   0        0        0      137 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/replay.yaml
--rw-r--r--   0        0        0     4008 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/prometheus.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/py.typed
--rw-r--r--   0        0        0     1631 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/pysignalr.py
--rw-r--r--   0        0        0     1722 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/report.py
--rw-r--r--   0        0        0     4867 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/scheduler.py
--rw-r--r--   0        0        0     4613 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/sentry.py
--rw-r--r--   0        0        0      199 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/sql/dipdup_head_status.sql
--rw-r--r--   0        0        0     2111 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/sql/truncate_schema.sql
--rw-r--r--   0        0        0     2163 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/subscriptions.py
--rw-r--r--   0        0        0     1791 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/sys.py
--rw-r--r--   0        0        0      227 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/templates/callback.py.j2
--rw-r--r--   0        0        0     1242 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/templates/models.py
--rw-r--r--   0        0        0      186 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/templates/replay.yaml.j2
--rw-r--r--   0        0        0     3290 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/transactions.py
--rw-r--r--   0        0        0     6763 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/utils.py
--rw-r--r--   0        0        0     5411 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/yaml.py
--rw-r--r--   0        0        0      952 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/__init__.py
--rw-r--r--   0        0        0      496 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/configs/asdf.yml
--rw-r--r--   0        0        0     1267 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/configs/demo_auction.yml
--rw-r--r--   0        0        0      825 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/configs/demo_big_maps.yml
--rw-r--r--   0        0        0      790 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/configs/demo_dao.yml
--rw-r--r--   0        0        0     5057 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/configs/demo_dex.yml
--rw-r--r--   0        0        0      943 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/configs/demo_domains.yml
--rw-r--r--   0        0        0      923 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/configs/demo_factories.yml
--rw-r--r--   0        0        0     1361 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/configs/demo_nft_marketplace.yml
--rw-r--r--   0        0        0      635 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/configs/demo_raw.yml
--rw-r--r--   0        0        0      756 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/configs/demo_token.yml
--rw-r--r--   0        0        0      572 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/configs/demo_token_transfers.yml
--rw-r--r--   0        0        0      572 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/configs/demo_token_transfers_2.yml
--rw-r--r--   0        0        0      572 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/configs/demo_token_transfers_3.yml
--rw-r--r--   0        0        0      859 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/configs/demo_token_transfers_4.yml
--rw-r--r--   0        0        0     1297 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/configs/dipdup.yml
--rw-r--r--   0        0        0      521 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/configs/hen_subjkt.yml
--rw-r--r--   0        0        0      496 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/configs/hjkl.yml
--rw-r--r--   0        0        0      546 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/configs/kolibri_ovens.yml
--rw-r--r--   0        0        0      684 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/configs/operation_filters.yml
--rw-r--r--   0        0        0      496 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/configs/qwer.yml
--rw-r--r--   0        0        0      496 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/configs/rewq.yml
--rw-r--r--   0        0        0      534 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/configs/yupana.yml
--rw-r--r--   0        0        0      496 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/configs/zxcv.yml
--rw-r--r--   0        0        0     1285 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/profile_abi_decoding.py
--rw-r--r--   0        0        0        2 2023-07-21 12:55:34.610438 dipdup-7.0.0rc1/tests/replays/024e925225593fe9cd80f5a114201f74d9f3631cea6f03add3e88fc91fafd2d7
--rw-r--r--   0        0        0    11605 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/replays/0535b2dcc93076e6026fa48cc501adaed47b7b060e6483d8312f40c184d7287d
--rw-r--r--   0        0        0  2577538 2023-07-21 12:53:39.351626 dipdup-7.0.0rc1/tests/replays/064e788d2566d748f516b17c6a43ab34259443cc9537f0dec7c1a5a2bce704b2
--rw-r--r--   0        0        0      305 2023-07-21 12:56:47.355883 dipdup-7.0.0rc1/tests/replays/0b7d26b8f2813d12a80b9e96cc6f0bb186bf9ac5c5b0c0b3bb2cc8d750126843
--rw-r--r--   0        0        0      784 2023-07-21 12:53:39.351626 dipdup-7.0.0rc1/tests/replays/0eaaba2830dbdd3a80286fbc367084bce6e55c678e21da178a7eb16beef6c997
--rw-r--r--   0        0        0       20 2023-07-21 12:53:39.351626 dipdup-7.0.0rc1/tests/replays/1165d42ccbdd0f6c25cece69d2c579da07655a30d04f18840350a153a98827a0
--rw-r--r--   0        0        0     7446 2023-07-21 12:53:39.351626 dipdup-7.0.0rc1/tests/replays/1228b36594bb93d619170ad49373f1ceec52d10faafdd727b37f3cdeffd663db
--rw-r--r--   0        0        0     4947 2023-07-21 12:53:39.351626 dipdup-7.0.0rc1/tests/replays/13afdf001ce3d6a0219c0f7f6d372d9b645770e5f4304576f7f7a37b45af96fc
--rw-r--r--   0        0        0      310 2023-07-21 12:53:39.351626 dipdup-7.0.0rc1/tests/replays/1430e37dce64ecb83499da8feaa3c0906e4fdf5d0a3c3570174645e97ba54bc4
--rw-r--r--   0        0        0    13275 2023-07-21 12:53:39.351626 dipdup-7.0.0rc1/tests/replays/14408f393a3e399b241184f858e70396e3b8313e32ee1a984913d43fb74dcfec
--rw-r--r--   0        0        0   855628 2023-07-21 12:55:48.762722 dipdup-7.0.0rc1/tests/replays/14cba0424c66b1869edc8e18ca3079856083cc3db7e68ef61fce165b6d7e1a6d
--rw-r--r--   0        0        0      129 2023-07-21 12:53:39.351626 dipdup-7.0.0rc1/tests/replays/14d37c70764fe50b4ea590691d5614f613f96b8ad98c5df189564778616f5261
--rw-r--r--   0        0        0      246 2023-07-21 12:53:39.351626 dipdup-7.0.0rc1/tests/replays/185f6628ac43f6ca728c5b79b7b81a3c3671efce7f14030a06a27e90cf641dea
--rw-r--r--   0        0        0      986 2023-07-21 12:53:39.351626 dipdup-7.0.0rc1/tests/replays/18d85ceab66daf057861b99b7e223a25067197b3b77edbf060390df58cb65eaa
--rw-r--r--   0        0        0     1448 2023-07-21 12:53:39.351626 dipdup-7.0.0rc1/tests/replays/19441b677ef5fd8ca39c37e6ddd2a7d9bc8cb3ab282b2a91ce4d8430f56f0fa9
--rw-r--r--   0        0        0   612008 2023-07-21 12:53:39.355626 dipdup-7.0.0rc1/tests/replays/1a43bd7d1397cc3169ad267cd2ef083a5a63eaac7ed5186aadfc01bb53636214
--rw-r--r--   0        0        0  1154515 2023-07-21 12:55:49.350735 dipdup-7.0.0rc1/tests/replays/1c07d3d72acc637fb46c59d0a6dc9749f3412a5d527ca2eb0cccc01720fda1c7
--rw-r--r--   0        0        0    89590 2023-07-21 12:53:39.355626 dipdup-7.0.0rc1/tests/replays/1c34d1f810ae474395893bf67fb8cfb27b0506ab94eebec42cd4d2d21bf3dfcd
--rw-r--r--   0        0        0        2 2023-07-21 12:55:34.610438 dipdup-7.0.0rc1/tests/replays/1c717490846300e1639e96a0c1438b6dd2abd6de013c5edec49042fa364c06e6
--rw-r--r--   0        0        0    12263 2023-07-21 12:53:39.355626 dipdup-7.0.0rc1/tests/replays/252fd058cfef21f9b5b7f4367f730ec7d41647253d7cc7ccfb1e22d42d1f366a
--rw-r--r--   0        0        0     1167 2023-07-21 12:53:39.355626 dipdup-7.0.0rc1/tests/replays/27373c23411bf37b605c8d0ead9a0e6c6c1f1718ce7863b095b759811e44e155
--rw-r--r--   0        0        0     1121 2023-07-21 12:53:39.355626 dipdup-7.0.0rc1/tests/replays/2a45ec6372b45e46199a6af24272cb93586777a0522cd1203b3eeef213ce4583
--rw-r--r--   0        0        0   209761 2023-07-21 12:55:49.434737 dipdup-7.0.0rc1/tests/replays/31cc70e13495f58ecde80847bc6c9e08536cc426c03bd2aa8c45c1b2c798e155
--rw-r--r--   0        0        0 21118960 2023-07-21 12:53:39.411627 dipdup-7.0.0rc1/tests/replays/31dd376b771f347a0d6fe4dd132a1f96f809274429b78ec86dd742e5589fbc23
--rw-r--r--   0        0        0  1807578 2023-07-21 12:55:35.338455 dipdup-7.0.0rc1/tests/replays/32e3a13cc470d8720ce28f5eaff327340fb25cbe712e5b5a348af1bc3c92235a
--rw-r--r--   0        0        0       65 2023-07-21 12:53:39.411627 dipdup-7.0.0rc1/tests/replays/33349b63491dc976a7a2332d3cca3bd9b3b831c02a6f474bb925876c1838633a
--rw-r--r--   0        0        0        2 2023-07-21 12:53:39.411627 dipdup-7.0.0rc1/tests/replays/34f3e33d677f85b633cb85c6dd205beb40e3d9c40cfafc7084b82c8123a54de1
--rw-r--r--   0        0        0    45221 2023-07-21 12:53:39.411627 dipdup-7.0.0rc1/tests/replays/36072e13c9ce265bb81142b8816da8c31bd9180e7c663ea4169bd259af107382
--rw-r--r--   0        0        0    81885 2023-07-21 12:53:39.411627 dipdup-7.0.0rc1/tests/replays/377ac31d6316391ed138df44bec374d65202f0577603e80465ced3c09140f78c
--rw-r--r--   0        0        0    54602 2023-07-21 12:56:00.634976 dipdup-7.0.0rc1/tests/replays/383899084f79460e96fd311bb64e4925738c486b39d6281539456c5fcac41620
--rw-r--r--   0        0        0      642 2023-07-21 12:56:29.599568 dipdup-7.0.0rc1/tests/replays/39b8664d1bca5d374ff905c8a3a396b53d19ee469dc37545a8ca6b080bd0e9e0
--rw-r--r--   0        0        0     1200 2023-07-21 12:56:48.327902 dipdup-7.0.0rc1/tests/replays/3a2bd8b6b72bf18152d2550c106789fa9b8abc98ea9d759a6597b7ebfbab0fc2
--rw-r--r--   0        0        0    81885 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/3c9ad6f98f79e72185ea58c4777115750c658c5defd616664212095bd440c10c
--rw-r--r--   0        0        0      332 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/3fdba02cbc415eba224604f4fea130acd4565d31e4a83cdbb679ec0b76c798ab
--rw-r--r--   0        0        0  3369404 2023-07-21 12:56:17.091309 dipdup-7.0.0rc1/tests/replays/42b7bf0da866257ef98e1f7124d2d21fe7d13228c076fffa32331da423f36933
--rw-r--r--   0        0        0      619 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/43cb0ab415d8b8b3f7addc3e82ea27d93b2c66ff55c117e1e0c7c64a0fcfc3f2
--rw-r--r--   0        0        0   530743 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/440173d32e95111ca7b080ccc4dc09bfab23c8361919b2c113f0ff9ab445eec2
--rw-r--r--   0        0        0  1594116 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/489233ce9373f7de4f7a9053055c74bc0df999bfe939ed67d98b6d67e676e35a
--rw-r--r--   0        0        0   109726 2023-07-21 12:55:46.378672 dipdup-7.0.0rc1/tests/replays/4a57776d93475adfd9c49b6c3295a7cedfc23b73733a1fb5f0c985ee039dc5dc
--rw-r--r--   0        0        0      984 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/4aa7f9b0657be0c44baf2caed8c7cb08d02097a4095cf6417f78cba3a25e8423
--rw-r--r--   0        0        0       67 2023-07-21 12:56:44.951834 dipdup-7.0.0rc1/tests/replays/4fbdb4667971fab446a5ac5937a7c8cc6ef5813ff00af24b6fd1b1a0427bedbb
--rw-r--r--   0        0        0   192680 2023-07-21 12:55:46.178667 dipdup-7.0.0rc1/tests/replays/5483a0e11009e0f186bf70c214e2597d267a75a1e19152a9e7ed1ec257ce88ca
--rw-r--r--   0        0        0       65 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/56eb33fbb563bf03ea7639659fae5102222d6e3cea882febf71f01bd383c6eed
--rw-r--r--   0        0        0    40432 2023-07-21 12:56:00.458973 dipdup-7.0.0rc1/tests/replays/587613799ebfae42b1884016d1a44a452d68e70e3ed80641d90b8e7657ba8ee5
--rw-r--r--   0        0        0       32 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/5b004196490632859ec1b019d640f6bbb93fc86a433c8969e10f36f51ac2c78d
--rw-r--r--   0        0        0     1907 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/5b7c31b4b73bc57e8296e6051b3bc7b2302b32588d8fbcafce8a66de3be743df
--rw-r--r--   0        0        0     7609 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/5b99bc4beb6a9a33f7d2f118426458e4c788e0ab6d9e51949d3ccbf8b4003fc1
--rw-r--r--   0        0        0      939 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/5d21060ba8e78279d2d1edaa2f266ecf36105eaccef5ebed15748441651f76fd
--rw-r--r--   0        0        0      400 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/5f63ef9dd15459ae14e715bb79da8f033a24b54504212ebc873ee8aa95679606
--rw-r--r--   0        0        0       67 2023-07-21 12:56:45.119838 dipdup-7.0.0rc1/tests/replays/60f48c13c47a1347786a6dcf6f741874e7b30b587d148faa67d15067bb3871de
--rw-r--r--   0        0        0       21 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/62e95f1d55b756895289374b351a1da94505ec2d95a1652c97765f36a2ef9341
--rw-r--r--   0        0        0   211527 2023-07-21 12:55:50.442758 dipdup-7.0.0rc1/tests/replays/6cc8d741a41b76983cd7e0f63e8f22a4c67cd946888f45a5b7ead8c3bb5ad2f1
--rw-r--r--   0        0        0   944885 2023-07-21 12:53:39.419628 dipdup-7.0.0rc1/tests/replays/6cff8d120db8fd3926a45714ce7f1d0560803eb5a7b4a413b64fee1b7fd7a8ff
--rw-r--r--   0        0        0      132 2023-07-21 12:56:45.951854 dipdup-7.0.0rc1/tests/replays/6d0c5443d41a15551acb41adc10d36d4895f5786d6922a878b5c5414610e0ebc
--rw-r--r--   0        0        0      754 2023-07-21 12:56:46.687869 dipdup-7.0.0rc1/tests/replays/6d76a3c3f427ff534c551de1793cb1d1dfbd22ccad97f5917a9f9b201a3f9804
--rw-r--r--   0        0        0      494 2023-07-21 12:53:39.419628 dipdup-7.0.0rc1/tests/replays/7132f07560319399092782debe6eb28926e961d8af215ce11e2c0efd8dab06da
--rw-r--r--   0        0        0      451 2023-07-21 12:56:47.519886 dipdup-7.0.0rc1/tests/replays/739d17c86095aac3da3508a16dc1c9ae9459ea86eeb09f62aaefc32de2997918
--rw-r--r--   0        0        0        2 2023-07-21 12:56:51.639967 dipdup-7.0.0rc1/tests/replays/759b79ec12b1305d9fa8e1a5218e62bb3d3ad913580e19914d30d8aa09920ae4
--rw-r--r--   0        0        0   209456 2023-07-21 12:53:39.419628 dipdup-7.0.0rc1/tests/replays/7669ea717d9759748aed86302326b79be5157a1a36d13b39b00f06bcbe22b309
--rw-r--r--   0        0        0      520 2023-07-21 12:53:39.419628 dipdup-7.0.0rc1/tests/replays/76d49ae3b723376c88ca65a3080a273e098d226932a1a49c38fbc4421e7c2e64
--rw-r--r--   0        0        0    50588 2023-07-21 12:56:19.739365 dipdup-7.0.0rc1/tests/replays/7b6cf9b8c69712bf26ed09059352ec740606969bf20eab0dedda870273f4fde9
--rw-r--r--   0        0        0 21649088 2023-07-21 12:56:18.547340 dipdup-7.0.0rc1/tests/replays/7b9c78209f98b2c3a6678ed224fa686eee25c3c63dddd7f9af77c734b0dfabb8
--rw-r--r--   0        0        0   108455 2023-07-21 12:56:34.275649 dipdup-7.0.0rc1/tests/replays/7d4a99edf5845445bbeb894ad34b063c985ca061ffed162093721c0032210e31
--rw-r--r--   0        0        0      807 2023-07-21 12:56:49.403924 dipdup-7.0.0rc1/tests/replays/803e05a8d0bb9e7cfb49530271d43ea62111b6419e7cded2d221f7e0e0c92ece
--rw-r--r--   0        0        0   517204 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/80921fd33043def891912a6ad57d76664399564fd813950eb11f4a0e69e3e28f
--rw-r--r--   0        0        0      129 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/815c066c21f7d2697ef107cad4624a9c4079a7a1dab7974d606fc42b81fe93c8
--rw-r--r--   0        0        0      939 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/816d08f71c84537ea8df05a40678b1addca15bf3a73c0e927c75d9f9c0f2d418
--rw-r--r--   0        0        0      395 2023-07-21 12:56:49.115918 dipdup-7.0.0rc1/tests/replays/8335acc6585656ec3a4301cd8b089401f2dc2c7d758b381c96c730e610b67f7b
--rw-r--r--   0        0        0   207502 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/84cf46aa9c8dbd3ca6c3d946c749713e6c70a6a20d9cc69b4156235fd099b2e3
--rw-r--r--   0        0        0        2 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/8ad31f6cf9c873b1fd9827b621529c43966f8376a86fcac3b1d20c260b78007e
--rw-r--r--   0        0        0       65 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/91787fdbd1634f277b20ac46cb30eba9770f83df7189df0903e22f5f4bbe1efa
--rw-r--r--   0        0        0     1151 2023-07-21 12:56:50.067937 dipdup-7.0.0rc1/tests/replays/93516225810a23a6799f2f9a1dee055ca79a66ee2b8d0f32be820c9c385e936b
--rw-r--r--   0        0        0      494 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/9ce1bc12a2adeddcf9d8854c4b63a8e65b58d9206fb8d2e3eedb24c44ea7f28a
--rw-r--r--   0        0        0       22 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/9de859083ed1dd278893f60b5a60feab02a04637327a664af23f52dabb139fe6
--rw-r--r--   0        0        0      706 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/9e6e907842da2cd494c558ea5ecc211fd12e56bfc547450978fb7dfe03853e58
--rw-r--r--   0        0        0     6981 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/a3ce91a1b0d505cc221f0e201781466ba1e2d6dc7b624b9bc75a03ce3dbb0f92
--rw-r--r--   0        0        0    38974 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/a795ef429bde71b3ba66b545c0048f57a78ab5d2247772761d8efe86567199b9
--rw-r--r--   0        0        0        2 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/a840afa5674efd06639c4692a8bfe9ed6e1346bfe9c414209eec5d9126333242
--rw-r--r--   0        0        0      675 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/aa8fe6037996b296bf9a3011e45cd9ecb92fb728592a843f91b03b2848cb1fb1
--rw-r--r--   0        0        0     1882 2023-07-21 12:56:12.215206 dipdup-7.0.0rc1/tests/replays/acc952ba1905717315212f952ed689d7b8f683165b31c0a7a25199aed9fda27f
--rw-r--r--   0        0        0      356 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/aeee37b6f63a3177e0e27ac472008c3cba3d30ebee691fb45de1bae91a87f2ce
--rw-r--r--   0        0        0       67 2023-07-21 12:56:44.787831 dipdup-7.0.0rc1/tests/replays/af37212b31e932f269c42c7f34ad8f3849bd8aed244652c41b9327c508985ce5
--rw-r--r--   0        0        0     1200 2023-07-21 12:56:42.831792 dipdup-7.0.0rc1/tests/replays/b3af887f7ad8172af75b94a09bedfb9ae1e14f8819a36d6ce9f709721068263b
--rw-r--r--   0        0        0  1214926 2023-07-21 12:55:48.978727 dipdup-7.0.0rc1/tests/replays/b49fb33ee80345b70414ad08806a860e2139c20d98a5150c6ccd1b28a90f311e
--rw-r--r--   0        0        0     2271 2023-07-21 12:56:41.487764 dipdup-7.0.0rc1/tests/replays/bec4433b4206f00c2310a7961cff7f539434b9161b45673793aa5a3b50234313
--rw-r--r--   0        0        0      310 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/bed2329e63d559db2fb81c69606e715d1f90aaacab6ae45b33516e7828841a3c
--rw-r--r--   0        0        0       65 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/bf941ceae7a6e3c40406438e067f137131e6605924a93d43bafc77682b602c55
--rw-r--r--   0        0        0   759209 2023-07-21 12:55:49.114730 dipdup-7.0.0rc1/tests/replays/c0202a433296436c27458b3d5ec5c72d5e2d47ff77c939ce399780cc0f3e56bc
--rw-r--r--   0        0        0    19100 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/c369836c15d9ed15477002b850d5cbb96b1ff5ff33e917b812ab9c0905063957
--rw-r--r--   0        0        0   918908 2023-07-21 12:53:39.427628 dipdup-7.0.0rc1/tests/replays/c8e8698717ada415bc10405da983c8357165914dd0219f3d09bb9a939705242d
--rw-r--r--   0        0        0   691878 2023-07-21 12:53:39.427628 dipdup-7.0.0rc1/tests/replays/cc162df04c4990c79f7507dd915601fd4d58c947a248156cbe302a64adfe898a
--rw-r--r--   0        0        0     7446 2023-07-21 12:53:39.427628 dipdup-7.0.0rc1/tests/replays/cc5d3d4a58d5cb6bc7270d38c797b7740b79f913590ef0164abd50e58fba9405
--rw-r--r--   0        0        0      301 2023-07-21 12:53:39.427628 dipdup-7.0.0rc1/tests/replays/cc648800928fd43f8e72db1d41115c26a22346c9c7831172fe422c1765cd67f2
--rw-r--r--   0        0        0      960 2023-07-21 12:53:39.427628 dipdup-7.0.0rc1/tests/replays/d0a594d14bcb3fbf916092ec6707dfd3c9f48f53f0a1ad40a32023e7a87f8ef5
--rw-r--r--   0        0        0     2403 2023-07-21 12:53:39.427628 dipdup-7.0.0rc1/tests/replays/d62748a927a09395579b5790c8f871cc8653081cf4475abc93173989f950b92b
--rw-r--r--   0        0        0     9089 2023-07-21 12:53:39.427628 dipdup-7.0.0rc1/tests/replays/d94397f6ecec8ce25f87177fe410f6498d7d30a04360506c0cd300d291c167e7
--rw-r--r--   0        0        0      132 2023-07-21 12:56:43.959814 dipdup-7.0.0rc1/tests/replays/db797e6bf4c1b9c3237af5dec694fb1b6d21418a5a2f7947eb7f54d4e9201baf
--rw-r--r--   0        0        0   548925 2023-07-21 12:56:18.855346 dipdup-7.0.0rc1/tests/replays/dc86d5e346c85e6f7953d7e01298a9db64d778e5ba717ddd07fff8b589081e98
--rw-r--r--   0        0        0    20467 2023-07-21 12:55:34.782442 dipdup-7.0.0rc1/tests/replays/dca9cf4f9f27623f10975d369444899458ab9ea85c22af2da6ce6ce8c09c2b58
--rw-r--r--   0        0        0      700 2023-07-21 12:53:39.427628 dipdup-7.0.0rc1/tests/replays/df62701276d6dbf4860058cc582c0b4f7b583758f4f5be96c9ee045757c151e3
--rw-r--r--   0        0        0   151396 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/replays/e39ebba701031aa13dfd9eb5dba1effd2938e96682d1030dcbd70172f9f190a9
--rw-r--r--   0        0        0     7917 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/replays/e4a563a0b19379a44e9d2dc398131e9fd30d6039ff4ffacf1252db0bf8b433aa
--rw-r--r--   0        0        0       67 2023-07-21 12:56:45.283841 dipdup-7.0.0rc1/tests/replays/e82ba90c8570b92c0b1fc360b853aca3f1d7de457aacb9f6f19fa3e43879a8b3
--rw-r--r--   0        0        0      132 2023-07-21 12:56:44.123818 dipdup-7.0.0rc1/tests/replays/e9fa56a94eb559c550dfbca4b27ef350a0b4a787afbe60205482a38223dcea04
--rw-r--r--   0        0        0   713724 2023-07-21 12:56:42.639788 dipdup-7.0.0rc1/tests/replays/eb8b6b33cb2e165d1a3a73c09938d3083671a82ad73d4c0cff1fb2a5e5715f76
--rw-r--r--   0        0        0    11290 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/replays/eb8e2c3ce2fe7792d2c8e81c61d37821275b64021343103b0c955042ae802189
--rw-r--r--   0        0        0      584 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/replays/ece1ebe13f9391555230d6b94f33d66a922e2ca71ef5fd39bbd8c2c37ddf54ec
--rw-r--r--   0        0        0     1089 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/replays/ed3ec9fd9226e9f765b96dc1d5d5a455a7b2505da530961826910b08db693070
--rw-r--r--   0        0        0    17245 2023-07-21 12:56:24.819472 dipdup-7.0.0rc1/tests/replays/f3d608f99e6b92e28a064bb9c10c3c605c9c817383c1eebcc68f663d1d23d650
--rw-r--r--   0        0        0    32513 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/replays/f60e794a9be14263cb10e48546ba5610302cc3e7af0a114a593bb50eb85ba5e7
--rw-r--r--   0        0        0       21 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/replays/fd9e33296006ad295c9fdc4868763f954a9c6d7c81d543ba198c14a72eea7e6b
--rw-r--r--   0        0        0      832 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/replays/ff51b3535acc2972090ecd5db3af8f827464c9d92f1aa661630976e5b4ed4cbe
--rw-r--r--   0        0        0     4599 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/responses/asdf.json
--rw-r--r--   0        0        0     6704 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/responses/ftzfun.json
--rw-r--r--   0        0        0     3445 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/responses/hen_subjkt.json
--rw-r--r--   0        0        0     5210 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/responses/hjkl.json
--rw-r--r--   0        0        0     2097 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/responses/kolibri_ovens.json
--rw-r--r--   0        0        0    11186 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/responses/ooQuCAKBHkmWy2VciDAV9c6CFTywuMLupLzVoKDwS1xvR4EdRng.json
--rw-r--r--   0        0        0     1811 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/responses/origination_amount.json
--rw-r--r--   0        0        0     4256 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/responses/qwer.json
--rw-r--r--   0        0        0     5307 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/responses/rewq.json
--rw-r--r--   0        0        0    38178 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/responses/yupana.json
--rw-r--r--   0        0        0     5909 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/responses/zxcv.json
--rw-r--r--   0        0        0     1077 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/schemas/asdf/storage.json
--rw-r--r--   0        0        0     2116 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/schemas/hen_subjkt/storage.json
--rw-r--r--   0        0        0     1638 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/schemas/hjkl/storage.json
--rw-r--r--   0        0        0      800 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/schemas/kolibri_ovens/storage.json
--rw-r--r--   0        0        0     1005 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/schemas/qwer/storage.json
--rw-r--r--   0        0        0     2212 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/schemas/rewq/storage.json
--rw-r--r--   0        0        0    12561 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/schemas/yupana/storage.json
--rw-r--r--   0        0        0     2660 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/schemas/zxcv/storage.json
--rw-r--r--   0        0        0     3767 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_config/test_callbacks.py
--rw-r--r--   0        0        0     4643 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_config/test_config.py
--rw-r--r--   0        0        0     4138 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_config/test_custom_config.py
--rw-r--r--   0        0        0     2486 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_context.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_datasources/__init__.py
--rw-r--r--   0        0        0      814 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_datasources/test_ipfs.py
--rw-r--r--   0        0        0      663 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_datasources/test_metadata.py
--rw-r--r--   0        0        0     8304 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_datasources/test_tzkt.py
--rw-r--r--   0        0        0     1223 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_datasources/test_tzkt_blocks.py
--rw-r--r--   0        0        0     1971 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_datasources/test_tzkt_buffer.py
--rw-r--r--   0        0        0     1433 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_datasources/test_tzkt_quotes.py
--rw-r--r--   0        0        0     8601 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_demos.py
--rw-r--r--   0        0        0     2734 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_dipdup.py
--rw-r--r--   0        0        0     5045 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_hasura.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_http.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_index/__init__.py
--rw-r--r--   0        0        0     3714 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_index/test_operation.py
--rw-r--r--   0        0        0     5772 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_introspection.py
--rw-r--r--   0        0        0    14279 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_models.py
--rw-r--r--   0        0        0    13401 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_rollback.py
--rw-r--r--   0        0        0     2628 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_utils.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/asdf/__init__.py
--rw-r--r--   0        0        0      504 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/asdf/storage.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/bazaar/__init__.py
--rw-r--r--   0        0        0      564 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/bazaar/storage.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/ftzfun/__init__.py
--rw-r--r--   0        0        0      929 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/ftzfun/storage.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/hen_subjkt/__init__.py
--rw-r--r--   0        0        0      583 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/hen_subjkt/storage.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/hjkl/__init__.py
--rw-r--r--   0        0        0      647 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/hjkl/storage.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/kolibri_ovens/__init__.py
--rw-r--r--   0        0        0      232 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/kolibri_ovens/set_delegate.py
--rw-r--r--   0        0        0      392 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/kolibri_ovens/storage.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/listofmaps/__init__.py
--rw-r--r--   0        0        0      153 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/listofmaps/storage.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/qwer/__init__.py
--rw-r--r--   0        0        0      532 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/qwer/storage.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/rewq/__init__.py
--rw-r--r--   0        0        0      831 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/rewq/storage.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/tezotop/__init__.py
--rw-r--r--   0        0        0      740 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/tezotop/storage.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/yupana/__init__.py
--rw-r--r--   0        0        0     2721 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/yupana/storage.py
--rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/zxcv/__init__.py
--rw-r--r--   0        0        0     1048 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/zxcv/storage.py
--rw-r--r--   0        0        0     5723 1970-01-01 00:00:00.000000 dipdup-7.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-27 00:38:52.701560 dipdup-7.0.0rc2/LICENSE
+-rw-r--r--   0        0        0     3816 2023-07-27 00:38:52.701560 dipdup-7.0.0rc2/README.md
+-rw-r--r--   0        0        0     4545 2023-07-27 00:48:02.674639 dipdup-7.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0      255 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_auction/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_auction/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1156 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      149 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      399 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      400 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/configs/replay.yaml
+-rw-r--r--   0        0        0      356 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/deploy/.keep
+-rw-r--r--   0        0        0      148 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/deploy/Dockerfile
+-rw-r--r--   0        0        0      348 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2686 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1247 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/deploy/compose.yaml
+-rw-r--r--   0        0        0      279 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      318 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/deploy/swarm.env.default
+-rw-r--r--   0        0        0     1077 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/handlers/.keep
+-rw-r--r--   0        0        0      913 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/handlers/on_bid.py
+-rw-r--r--   0        0        0     1619 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/handlers/on_create_auction.py
+-rw-r--r--   0        0        0      712 2023-07-27 00:38:52.713560 dipdup-7.0.0rc2/src/demo_auction/handlers/on_withdraw.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/models/.keep
+-rw-r--r--   0        0        0     1445 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:40:55.859497 dipdup-7.0.0rc2/src/demo_auction/py.typed
+-rw-r--r--   0        0        0     1047 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/types/.keep
+-rw-r--r--   0        0        0      177 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/types/tzcolors_auction/tezos_parameters/bid.py
+-rw-r--r--   0        0        0      381 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/types/tzcolors_auction/tezos_parameters/create_auction.py
+-rw-r--r--   0        0        0      187 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/types/tzcolors_auction/tezos_parameters/withdraw.py
+-rw-r--r--   0        0        0      555 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_auction/types/tzcolors_auction/tezos_storage.py
+-rw-r--r--   0        0        0      255 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_big_maps/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_big_maps/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1159 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      150 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      401 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      404 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/configs/replay.yaml
+-rw-r--r--   0        0        0      356 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/deploy/.keep
+-rw-r--r--   0        0        0      150 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/deploy/Dockerfile
+-rw-r--r--   0        0        0      350 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2688 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1248 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/deploy/compose.yaml
+-rw-r--r--   0        0        0      280 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      318 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/deploy/swarm.env.default
+-rw-r--r--   0        0        0      725 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/handlers/.keep
+-rw-r--r--   0        0        0      846 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/handlers/on_update_expiry_map.py
+-rw-r--r--   0        0        0     1688 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/handlers/on_update_records.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/models/.keep
+-rw-r--r--   0        0        0      667 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:41:26.379975 dipdup-7.0.0rc2/src/demo_big_maps/py.typed
+-rw-r--r--   0        0        0     1051 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/types/.keep
+-rw-r--r--   0        0        0      199 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/types/name_registry/tezos_big_maps/store_expiry_map_key.py
+-rw-r--r--   0        0        0      203 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/types/name_registry/tezos_big_maps/store_expiry_map_value.py
+-rw-r--r--   0        0        0      194 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/types/name_registry/tezos_big_maps/store_records_key.py
+-rw-r--r--   0        0        0      489 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_big_maps/types/name_registry/tezos_big_maps/store_records_value.py
+-rw-r--r--   0        0        0      255 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_blank/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_blank/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1160 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      147 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      395 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      402 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/configs/replay.yaml
+-rw-r--r--   0        0        0      327 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/deploy/.keep
+-rw-r--r--   0        0        0      144 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/deploy/Dockerfile
+-rw-r--r--   0        0        0      344 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2682 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1245 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/deploy/compose.yaml
+-rw-r--r--   0        0        0      248 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      289 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/deploy/swarm.env.default
+-rw-r--r--   0        0        0       37 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/handlers/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/models/.keep
+-rw-r--r--   0        0        0     1242 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/models/__init__.py
+-rw-r--r--   0        0        0     1049 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_blank/types/.keep
+-rw-r--r--   0        0        0      255 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_dao/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_dao/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1149 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      145 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      391 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      389 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/configs/replay.yaml
+-rw-r--r--   0        0        0      356 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/deploy/.keep
+-rw-r--r--   0        0        0      140 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/deploy/Dockerfile
+-rw-r--r--   0        0        0      340 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2678 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1243 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/deploy/compose.yaml
+-rw-r--r--   0        0        0      275 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      318 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/deploy/swarm.env.default
+-rw-r--r--   0        0        0      643 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/handlers/.keep
+-rw-r--r--   0        0        0      408 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/handlers/on_origination.py
+-rw-r--r--   0        0        0      506 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/handlers/on_propose.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/models/.keep
+-rw-r--r--   0        0        0      782 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:41:09.423710 dipdup-7.0.0rc2/src/demo_dao/py.typed
+-rw-r--r--   0        0        0     1036 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/types/.keep
+-rw-r--r--   0        0        0      360 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/types/registry/tezos_parameters/propose.py
+-rw-r--r--   0        0        0     2523 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dao/types/registry/tezos_storage.py
+-rw-r--r--   0        0        0      255 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dex/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dex/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_dex/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_dex/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1164 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dex/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.717560 dipdup-7.0.0rc2/src/demo_dex/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      145 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      391 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      404 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/configs/replay.yaml
+-rw-r--r--   0        0        0      327 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/deploy/.keep
+-rw-r--r--   0        0        0      140 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/deploy/Dockerfile
+-rw-r--r--   0        0        0      340 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2678 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1243 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/deploy/compose.yaml
+-rw-r--r--   0        0        0      246 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      289 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/deploy/swarm.env.default
+-rw-r--r--   0        0        0     4845 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/.keep
+-rw-r--r--   0        0        0     1829 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_divest_liquidity.py
+-rw-r--r--   0        0        0     1737 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_invest_liquidity.py
+-rw-r--r--   0        0        0      579 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_origination.py
+-rw-r--r--   0        0        0     1610 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_tez_to_token.py
+-rw-r--r--   0        0        0     1676 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_token_to_tez.py
+-rw-r--r--   0        0        0     1022 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_transfer.py
+-rw-r--r--   0        0        0      962 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_withdraw_profit.py
+-rw-r--r--   0        0        0     1855 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_divest_liquidity.py
+-rw-r--r--   0        0        0     1763 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_invest_liquidity.py
+-rw-r--r--   0        0        0      573 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_origination.py
+-rw-r--r--   0        0        0     1604 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_tez_to_token.py
+-rw-r--r--   0        0        0     1642 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_token_to_tez.py
+-rw-r--r--   0        0        0     1143 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_transfer.py
+-rw-r--r--   0        0        0      958 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_withdraw_profit.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/models/.keep
+-rw-r--r--   0        0        0      916 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:40:45.219330 dipdup-7.0.0rc2/src/demo_dex/py.typed
+-rw-r--r--   0        0        0     1051 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/.keep
+-rw-r--r--   0        0        0      340 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/fa12_token/tezos_parameters/transfer.py
+-rw-r--r--   0        0        0      739 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/fa12_token/tezos_storage.py
+-rw-r--r--   0        0        0      504 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/fa2_token/tezos_parameters/transfer.py
+-rw-r--r--   0        0        0     1093 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/fa2_token/tezos_storage.py
+-rw-r--r--   0        0        0      311 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa12/tezos_parameters/divest_liquidity.py
+-rw-r--r--   0        0        0      201 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa12/tezos_parameters/invest_liquidity.py
+-rw-r--r--   0        0        0      297 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa12/tezos_parameters/tez_to_token_payment.py
+-rw-r--r--   0        0        0      313 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa12/tezos_parameters/token_to_tez_payment.py
+-rw-r--r--   0        0        0      340 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa12/tezos_parameters/transfer.py
+-rw-r--r--   0        0        0      199 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa12/tezos_parameters/withdraw_profit.py
+-rw-r--r--   0        0        0     1455 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa12/tezos_storage.py
+-rw-r--r--   0        0        0      311 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa2/tezos_parameters/divest_liquidity.py
+-rw-r--r--   0        0        0      201 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa2/tezos_parameters/invest_liquidity.py
+-rw-r--r--   0        0        0      297 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa2/tezos_parameters/tez_to_token_payment.py
+-rw-r--r--   0        0        0      313 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa2/tezos_parameters/token_to_tez_payment.py
+-rw-r--r--   0        0        0      504 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa2/tezos_parameters/transfer.py
+-rw-r--r--   0        0        0      199 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa2/tezos_parameters/withdraw_profit.py
+-rw-r--r--   0        0        0     1491 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa2/tezos_storage.py
+-rw-r--r--   0        0        0      255 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_domains/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_domains/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1158 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      149 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      399 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      402 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/configs/replay.yaml
+-rw-r--r--   0        0        0      356 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/deploy/.keep
+-rw-r--r--   0        0        0      148 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/deploy/Dockerfile
+-rw-r--r--   0        0        0      348 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2686 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1247 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/deploy/compose.yaml
+-rw-r--r--   0        0        0      279 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      318 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/deploy/swarm.env.default
+-rw-r--r--   0        0        0      845 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/handlers/.keep
+-rw-r--r--   0        0        0      553 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/handlers/on_admin_update.py
+-rw-r--r--   0        0        0      525 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/handlers/on_execute.py
+-rw-r--r--   0        0        0     1437 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/handlers/on_storage_diff.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/models/.keep
+-rw-r--r--   0        0        0      630 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:40:33.047144 dipdup-7.0.0rc2/src/demo_domains/py.typed
+-rw-r--r--   0        0        0     1049 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/types/.keep
+-rw-r--r--   0        0        0      194 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/types/name_registry/tezos_parameters/admin_update.py
+-rw-r--r--   0        0        0      305 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/types/name_registry/tezos_parameters/execute.py
+-rw-r--r--   0        0        0     1134 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_domains/types/name_registry/tezos_storage.py
+-rw-r--r--   0        0        0      255 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_events/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_events/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1157 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      148 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      397 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      400 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/configs/replay.yaml
+-rw-r--r--   0        0        0      327 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/deploy/.keep
+-rw-r--r--   0        0        0      146 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/deploy/Dockerfile
+-rw-r--r--   0        0        0      346 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2684 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1246 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/deploy/compose.yaml
+-rw-r--r--   0        0        0      249 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      289 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/deploy/swarm.env.default
+-rw-r--r--   0        0        0      536 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/handlers/.keep
+-rw-r--r--   0        0        0      311 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/handlers/on_move_event.py
+-rw-r--r--   0        0        0      237 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/handlers/on_other_event.py
+-rw-r--r--   0        0        0      311 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/handlers/on_roll_event.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/models/.keep
+-rw-r--r--   0        0        0     1242 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/models/__init__.py
+-rw-r--r--   0        0        0     1047 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.721560 dipdup-7.0.0rc2/src/demo_events/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_events/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_events/types/.keep
+-rw-r--r--   0        0        0      317 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_events/types/events_contract/tezos_events/move.py
+-rw-r--r--   0        0        0      266 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_events/types/events_contract/tezos_events/roll.py
+-rw-r--r--   0        0        0      255 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_evm_events/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_evm_events/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1174 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/abi/.keep
+-rw-r--r--   0        0        0    11460 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/abi/eth_usdt/abi.json
+-rw-r--r--   0        0        0     2420 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/abi/eth_usdt/events.json
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      152 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      405 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      421 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/configs/replay.yaml
+-rw-r--r--   0        0        0      409 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/deploy/.keep
+-rw-r--r--   0        0        0      154 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/deploy/Dockerfile
+-rw-r--r--   0        0        0      354 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2692 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1250 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/deploy/compose.yaml
+-rw-r--r--   0        0        0      335 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      371 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/deploy/swarm.env.default
+-rw-r--r--   0        0        0      694 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/handlers/.keep
+-rw-r--r--   0        0        0      992 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/handlers/on_transfer.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/models/.keep
+-rw-r--r--   0        0        0      368 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/models/__init__.py
+-rw-r--r--   0        0        0     1068 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/types/.keep
+-rw-r--r--   0        0        0      331 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_evm_events/types/eth_usdt/evm_events/transfer.py
+-rw-r--r--   0        0        0      255 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_factories/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_factories/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1173 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      151 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      403 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      419 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/configs/replay.yaml
+-rw-r--r--   0        0        0      356 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/deploy/.keep
+-rw-r--r--   0        0        0      152 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/deploy/Dockerfile
+-rw-r--r--   0        0        0      352 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2690 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1249 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/deploy/compose.yaml
+-rw-r--r--   0        0        0      281 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      318 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/deploy/swarm.env.default
+-rw-r--r--   0        0        0      647 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/handlers/.keep
+-rw-r--r--   0        0        0      420 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/handlers/on_origination.py
+-rw-r--r--   0        0        0      524 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/handlers/on_propose.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/models/.keep
+-rw-r--r--   0        0        0      782 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:41:22.215910 dipdup-7.0.0rc2/src/demo_factories/py.typed
+-rw-r--r--   0        0        0     1066 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/types/.keep
+-rw-r--r--   0        0        0      360 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/types/registry/tezos_parameters/propose.py
+-rw-r--r--   0        0        0     2523 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_factories/types/registry/tezos_storage.py
+-rw-r--r--   0        0        0      255 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_head/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_head/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1159 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      146 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      393 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      400 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/configs/replay.yaml
+-rw-r--r--   0        0        0      356 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/deploy/.keep
+-rw-r--r--   0        0        0      142 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/deploy/Dockerfile
+-rw-r--r--   0        0        0      342 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2680 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1244 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/deploy/compose.yaml
+-rw-r--r--   0        0        0      276 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      318 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/deploy/swarm.env.default
+-rw-r--r--   0        0        0      240 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/handlers/.keep
+-rw-r--r--   0        0        0      237 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/handlers/on_mainnet_head.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/models/.keep
+-rw-r--r--   0        0        0     1242 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/models/__init__.py
+-rw-r--r--   0        0        0     1047 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_head/types/.keep
+-rw-r--r--   0        0        0      255 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_nft_marketplace/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_nft_marketplace/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1167 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      157 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      415 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      419 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/configs/replay.yaml
+-rw-r--r--   0        0        0      452 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/deploy/.keep
+-rw-r--r--   0        0        0      164 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/deploy/Dockerfile
+-rw-r--r--   0        0        0      364 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2702 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1255 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/deploy/compose.yaml
+-rw-r--r--   0        0        0      383 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      414 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/deploy/swarm.env.default
+-rw-r--r--   0        0        0     1199 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/handlers/.keep
+-rw-r--r--   0        0        0      605 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/handlers/on_cancel_swap.py
+-rw-r--r--   0        0        0     1037 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/handlers/on_collect.py
+-rw-r--r--   0        0        0      977 2023-07-27 00:38:52.725560 dipdup-7.0.0rc2/src/demo_nft_marketplace/handlers/on_mint.py
+-rw-r--r--   0        0        0      885 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/handlers/on_swap.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/models/.keep
+-rw-r--r--   0        0        0     1306 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:40:43.251300 dipdup-7.0.0rc2/src/demo_nft_marketplace/py.typed
+-rw-r--r--   0        0        0     1066 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/types/.keep
+-rw-r--r--   0        0        0      192 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/cancel_swap.py
+-rw-r--r--   0        0        0      281 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/collect.py
+-rw-r--r--   0        0        0      317 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/mint_objkt.py
+-rw-r--r--   0        0        0      299 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/swap.py
+-rw-r--r--   0        0        0      777 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/types/hen_minter/tezos_storage.py
+-rw-r--r--   0        0        0      343 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/types/hen_objkts/tezos_parameters/mint.py
+-rw-r--r--   0        0        0     1094 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_nft_marketplace/types/hen_objkts/tezos_storage.py
+-rw-r--r--   0        0        0      255 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_raw/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_raw/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1186 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      145 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      391 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      426 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/configs/replay.yaml
+-rw-r--r--   0        0        0      356 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/deploy/.keep
+-rw-r--r--   0        0        0      140 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/deploy/Dockerfile
+-rw-r--r--   0        0        0      340 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2678 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1243 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/deploy/compose.yaml
+-rw-r--r--   0        0        0      275 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      318 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/deploy/swarm.env.default
+-rw-r--r--   0        0        0      411 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/handlers/.keep
+-rw-r--r--   0        0        0      350 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/handlers/on_operation.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/models/.keep
+-rw-r--r--   0        0        0      245 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:41:32.164065 dipdup-7.0.0rc2/src/demo_raw/py.typed
+-rw-r--r--   0        0        0     1073 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_raw/types/.keep
+-rw-r--r--   0        0        0      255 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_token/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_token/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1158 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      147 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      395 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      400 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/configs/replay.yaml
+-rw-r--r--   0        0        0      327 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/deploy/.keep
+-rw-r--r--   0        0        0      144 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/deploy/Dockerfile
+-rw-r--r--   0        0        0      344 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2682 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1245 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/deploy/compose.yaml
+-rw-r--r--   0        0        0      248 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      289 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/deploy/swarm.env.default
+-rw-r--r--   0        0        0      730 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/handlers/.keep
+-rw-r--r--   0        0        0      436 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/handlers/on_balance_update.py
+-rw-r--r--   0        0        0      630 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/handlers/on_mint.py
+-rw-r--r--   0        0        0      928 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/handlers/on_transfer.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/models/.keep
+-rw-r--r--   0        0        0      370 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:40:33.047144 dipdup-7.0.0rc2/src/demo_token/py.typed
+-rw-r--r--   0        0        0     1047 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/types/.keep
+-rw-r--r--   0        0        0      263 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/types/tzbtc/tezos_parameters/mint.py
+-rw-r--r--   0        0        0      340 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/types/tzbtc/tezos_parameters/transfer.py
+-rw-r--r--   0        0        0      398 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token/types/tzbtc/tezos_storage.py
+-rw-r--r--   0        0        0      255 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_token_transfers/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_token_transfers/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1167 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      157 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      415 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      419 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/configs/replay.yaml
+-rw-r--r--   0        0        0      327 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/deploy/.keep
+-rw-r--r--   0        0        0      164 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/deploy/Dockerfile
+-rw-r--r--   0        0        0      364 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2702 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1255 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/deploy/compose.yaml
+-rw-r--r--   0        0        0      258 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      289 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/deploy/swarm.env.default
+-rw-r--r--   0        0        0      409 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/handlers/.keep
+-rw-r--r--   0        0        0      545 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/handlers/on_balance_update.py
+-rw-r--r--   0        0        0      836 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/handlers/on_token_transfer.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/models/.keep
+-rw-r--r--   0        0        0      370 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:41:06.455664 dipdup-7.0.0rc2/src/demo_token_transfers/py.typed
+-rw-r--r--   0        0        0     1066 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_token_transfers/types/.keep
+-rw-r--r--   0        0        0      255 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_uniswap/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_uniswap/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_uniswap/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-27 00:40:07.250778 dipdup-7.0.0rc2/src/demo_uniswap/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1179 2023-07-27 00:38:52.729560 dipdup-7.0.0rc2/src/demo_uniswap/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/abi/.keep
+-rw-r--r--   0        0        0     4418 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/abi/factory/abi.json
+-rw-r--r--   0        0        0      919 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/abi/factory/events.json
+-rw-r--r--   0        0        0    19609 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/abi/pool/abi.json
+-rw-r--r--   0        0        0     3559 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/abi/pool/events.json
+-rw-r--r--   0        0        0    24313 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/abi/position_manager/abi.json
+-rw-r--r--   0        0        0     1984 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/abi/position_manager/events.json
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      149 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      399 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      423 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/configs/replay.yaml
+-rw-r--r--   0        0        0      424 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/deploy/.keep
+-rw-r--r--   0        0        0      148 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/deploy/Dockerfile
+-rw-r--r--   0        0        0      348 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2686 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1247 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/deploy/compose.yaml
+-rw-r--r--   0        0        0      347 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      386 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/deploy/swarm.env.default
+-rw-r--r--   0        0        0     2236 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/handlers/.keep
+-rw-r--r--   0        0        0     3060 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/handlers/factory/pool_created.py
+-rw-r--r--   0        0        0      531 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/handlers/pool/burn.py
+-rw-r--r--   0        0        0      291 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/handlers/pool/flash.py
+-rw-r--r--   0        0        0      871 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/handlers/pool/initialize.py
+-rw-r--r--   0        0        0     1330 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/handlers/pool/mint.py
+-rw-r--r--   0        0        0     6558 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/handlers/pool/swap.py
+-rw-r--r--   0        0        0     1227 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/handlers/position_manager/collect.py
+-rw-r--r--   0        0        0     1361 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/handlers/position_manager/decrease_liquidity.py
+-rw-r--r--   0        0        0     1449 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/handlers/position_manager/increase_liquidity.py
+-rw-r--r--   0        0        0     1172 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/handlers/position_manager/transfer.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/models/.keep
+-rw-r--r--   0        0        0    19932 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/models/__init__.py
+-rw-r--r--   0        0        0      373 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/models/abi.py
+-rw-r--r--   0        0        0     4162 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/models/pool.py
+-rw-r--r--   0        0        0     2824 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/models/position.py
+-rw-r--r--   0        0        0     1477 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/models/repo.py
+-rw-r--r--   0        0        0      561 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/models/tick.py
+-rw-r--r--   0        0        0     7160 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/models/token.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/py.typed
+-rw-r--r--   0        0        0     1070 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/types/.keep
+-rw-r--r--   0        0        0      321 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/types/factory/evm_events/pool_created.py
+-rw-r--r--   0        0        0      330 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/types/pool/evm_events/burn.py
+-rw-r--r--   0        0        0      339 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/types/pool/evm_events/collect.py
+-rw-r--r--   0        0        0      328 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/types/pool/evm_events/flash.py
+-rw-r--r--   0        0        0      275 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/types/pool/evm_events/initialize.py
+-rw-r--r--   0        0        0      346 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/types/pool/evm_events/mint.py
+-rw-r--r--   0        0        0      351 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/types/pool/evm_events/swap.py
+-rw-r--r--   0        0        0      303 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/types/position_manager/evm_events/collect.py
+-rw-r--r--   0        0        0      323 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/types/position_manager/evm_events/decrease_liquidity.py
+-rw-r--r--   0        0        0      323 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/types/position_manager/evm_events/increase_liquidity.py
+-rw-r--r--   0        0        0      333 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/demo_uniswap/types/position_manager/evm_events/transfer.py
+-rw-r--r--   0        0        0      213 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/__init__.py
+-rw-r--r--   0        0        0      105 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/__main__.py
+-rw-r--r--   0        0        0      512 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/api.py
+-rw-r--r--   0        0        0    21805 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/cli.py
+-rw-r--r--   0        0        0     7735 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/codegen/__init__.py
+-rw-r--r--   0        0        0     7038 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/codegen/evm_subsquid.py
+-rw-r--r--   0        0        0    18129 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/codegen/tezos_tzkt.py
+-rw-r--r--   0        0        0    41898 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/config/__init__.py
+-rw-r--r--   0        0        0      554 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/config/abi_etherscan.py
+-rw-r--r--   0        0        0      690 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/config/coinbase.py
+-rw-r--r--   0        0        0     1469 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/config/evm.py
+-rw-r--r--   0        0        0     1273 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/config/evm_node.py
+-rw-r--r--   0        0        0     1375 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/config/evm_subsquid.py
+-rw-r--r--   0        0        0     2578 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/config/evm_subsquid_events.py
+-rw-r--r--   0        0        0     1495 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/config/evm_subsquid_operations.py
+-rw-r--r--   0        0        0      446 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/config/http.py
+-rw-r--r--   0        0        0      519 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/config/ipfs.py
+-rw-r--r--   0        0        0     1532 2023-07-27 00:38:52.733560 dipdup-7.0.0rc2/src/dipdup/config/tezos.py
+-rw-r--r--   0        0        0     2157 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/config/tezos_tzkt.py
+-rw-r--r--   0        0        0     3758 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/config/tezos_tzkt_big_maps.py
+-rw-r--r--   0        0        0     3074 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/config/tezos_tzkt_events.py
+-rw-r--r--   0        0        0     1424 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/config/tezos_tzkt_head.py
+-rw-r--r--   0        0        0    12744 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/config/tezos_tzkt_operations.py
+-rw-r--r--   0        0        0     3110 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/config/tezos_tzkt_token_transfers.py
+-rw-r--r--   0        0        0      745 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/config/tzip_metadata.py
+-rw-r--r--   0        0        0    28058 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/context.py
+-rw-r--r--   0        0        0    14211 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/database.py
+-rw-r--r--   0        0        0     4474 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/datasources/__init__.py
+-rw-r--r--   0        0        0      915 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/datasources/abi_etherscan.py
+-rw-r--r--   0        0        0     2274 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/datasources/coinbase.py
+-rw-r--r--   0        0        0    12321 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/datasources/evm_node.py
+-rw-r--r--   0        0        0     4013 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/datasources/evm_subsquid.py
+-rw-r--r--   0        0        0      399 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/datasources/http.py
+-rw-r--r--   0        0        0      524 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/datasources/ipfs.py
+-rw-r--r--   0        0        0    43369 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/datasources/tezos_tzkt.py
+-rw-r--r--   0        0        0     1545 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/datasources/tzip_metadata.py
+-rw-r--r--   0        0        0    30184 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/dipdup.py
+-rw-r--r--   0        0        0     1803 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/env.py
+-rw-r--r--   0        0        0     8274 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/exceptions.py
+-rw-r--r--   0        0        0     3981 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/fetcher.py
+-rw-r--r--   0        0        0     6724 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/fields.py
+-rw-r--r--   0        0        0    25644 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/hasura.py
+-rw-r--r--   0        0        0    11008 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/http.py
+-rw-r--r--   0        0        0     7426 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/index.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/__init__.py
+-rw-r--r--   0        0        0     1229 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/evm_subsquid_events/fetcher.py
+-rw-r--r--   0        0        0    10389 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/evm_subsquid_events/index.py
+-rw-r--r--   0        0        0     3439 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/evm_subsquid_events/matcher.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/evm_subsquid_events/parser.py
+-rw-r--r--   0        0        0      406 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/evm_subsquid_operations/index.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_big_maps/__init__.py
+-rw-r--r--   0        0        0     3181 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_big_maps/fetcher.py
+-rw-r--r--   0        0        0     7320 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_big_maps/index.py
+-rw-r--r--   0        0        0     2684 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_big_maps/matcher.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_events/__init__.py
+-rw-r--r--   0        0        0     1480 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_events/fetcher.py
+-rw-r--r--   0        0        0     5539 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_events/index.py
+-rw-r--r--   0        0        0     3888 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_events/matcher.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_head/__init__.py
+-rw-r--r--   0        0        0     2349 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_head/index.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_operations/__init__.py
+-rw-r--r--   0        0        0    20276 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_operations/fetcher.py
+-rw-r--r--   0        0        0    13485 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_operations/index.py
+-rw-r--r--   0        0        0     9135 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_operations/matcher.py
+-rw-r--r--   0        0        0     7612 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_operations/parser.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_token_transfers/__init__.py
+-rw-r--r--   0        0        0     1432 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_token_transfers/fetcher.py
+-rw-r--r--   0        0        0     5520 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_token_transfers/index.py
+-rw-r--r--   0        0        0     1808 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_token_transfers/matcher.py
+-rwxr-xr-x   0        0        0     9379 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/install.py
+-rw-r--r--   0        0        0    20461 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/models/__init__.py
+-rw-r--r--   0        0        0     1309 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/models/coinbase.py
+-rw-r--r--   0        0        0     3596 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/models/evm_node.py
+-rw-r--r--   0        0        0     5045 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/models/evm_subsquid.py
+-rw-r--r--   0        0        0    19800 2023-07-27 00:38:52.737560 dipdup-7.0.0rc2/src/dipdup/models/tezos_tzkt.py
+-rw-r--r--   0        0        0      165 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/models/tzip_metadata.py
+-rw-r--r--   0        0        0     7085 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/package.py
+-rw-r--r--   0        0        0     7091 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/performance.py
+-rw-r--r--   0        0        0     8379 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/project.py
+-rw-r--r--   0        0        0      256 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/base/.dockerignore.j2
+-rw-r--r--   0        0        0      341 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/base/.gitignore.j2
+-rw-r--r--   0        0        0     1163 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/base/README.md.j2
+-rw-r--r--   0        0        0      380 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/base/configs/dipdup.compose.yaml.j2
+-rw-r--r--   0        0        0      159 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/base/configs/dipdup.sqlite.yaml.j2
+-rw-r--r--   0        0        0      418 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/base/configs/dipdup.swarm.yaml.j2
+-rw-r--r--   0        0        0      221 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/base/deploy/Dockerfile.j2
+-rw-r--r--   0        0        0      367 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/base/deploy/compose.sqlite.yaml.j2
+-rw-r--r--   0        0        0     2748 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/base/deploy/compose.swarm.yaml.j2
+-rw-r--r--   0        0        0     1273 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/base/deploy/compose.yaml.j2
+-rw-r--r--   0        0        0     1240 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/base/pyproject.toml.j2
+-rw-r--r--   0        0        0     1087 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_auction/dipdup.yaml.j2
+-rw-r--r--   0        0        0      935 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_auction/handlers/on_bid.py.j2
+-rw-r--r--   0        0        0     1641 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_auction/handlers/on_create_auction.py.j2
+-rw-r--r--   0        0        0      734 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_auction/handlers/on_withdraw.py.j2
+-rw-r--r--   0        0        0     1448 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_auction/models/__init__.py.j2
+-rw-r--r--   0        0        0      114 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_auction/replay.yaml
+-rw-r--r--   0        0        0      734 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_big_maps/dipdup.yaml.j2
+-rw-r--r--   0        0        0      865 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_big_maps/handlers/on_update_expiry_map.py.j2
+-rw-r--r--   0        0        0     1707 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_big_maps/handlers/on_update_records.py.j2
+-rw-r--r--   0        0        0      669 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_big_maps/models/__init__.py.j2
+-rw-r--r--   0        0        0      118 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_big_maps/replay.yaml
+-rw-r--r--   0        0        0       49 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_blank/dipdup.yaml.j2
+-rw-r--r--   0        0        0      116 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_blank/replay.yaml
+-rw-r--r--   0        0        0      657 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dao/dipdup.yaml.j2
+-rw-r--r--   0        0        0      431 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dao/handlers/on_origination.py.j2
+-rw-r--r--   0        0        0      540 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dao/handlers/on_propose.py.j2
+-rw-r--r--   0        0        0      784 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dao/models/__init__.py.j2
+-rw-r--r--   0        0        0      103 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dao/replay.yaml
+-rw-r--r--   0        0        0     4859 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/dipdup.yaml.j2
+-rw-r--r--   0        0        0     1885 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_divest_liquidity.py.j2
+-rw-r--r--   0        0        0     1793 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_invest_liquidity.py.j2
+-rw-r--r--   0        0        0      602 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_origination.py.j2
+-rw-r--r--   0        0        0     1666 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_tez_to_token.py.j2
+-rw-r--r--   0        0        0     1732 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_token_to_tez.py.j2
+-rw-r--r--   0        0        0     1056 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_transfer.py.j2
+-rw-r--r--   0        0        0      996 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_withdraw_profit.py.j2
+-rw-r--r--   0        0        0     1911 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_divest_liquidity.py.j2
+-rw-r--r--   0        0        0     1819 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_invest_liquidity.py.j2
+-rw-r--r--   0        0        0      596 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_origination.py.j2
+-rw-r--r--   0        0        0     1660 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_tez_to_token.py.j2
+-rw-r--r--   0        0        0     1698 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_token_to_tez.py.j2
+-rw-r--r--   0        0        0     1177 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_transfer.py.j2
+-rw-r--r--   0        0        0      992 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_withdraw_profit.py.j2
+-rw-r--r--   0        0        0      918 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/models/__init__.py.j2
+-rw-r--r--   0        0        0      118 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/replay.yaml
+-rw-r--r--   0        0        0      855 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_domains/dipdup.yaml.j2
+-rw-r--r--   0        0        0      581 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_domains/handlers/on_admin_update.py.j2
+-rw-r--r--   0        0        0      553 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_domains/handlers/on_execute.py.j2
+-rw-r--r--   0        0        0     1456 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_domains/handlers/on_storage_diff.py.j2
+-rw-r--r--   0        0        0      632 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_domains/models/__init__.py.j2
+-rw-r--r--   0        0        0      116 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_domains/replay.yaml
+-rw-r--r--   0        0        0      547 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_events/dipdup.yaml.j2
+-rw-r--r--   0        0        0      114 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_events/replay.yaml
+-rw-r--r--   0        0        0      701 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_evm_events/dipdup.yaml.j2
+-rw-r--r--   0        0        0     1005 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_evm_events/handlers/on_transfer.py.j2
+-rw-r--r--   0        0        0      370 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_evm_events/models/__init__.py.j2
+-rw-r--r--   0        0        0      135 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_evm_events/replay.yaml
+-rw-r--r--   0        0        0      655 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_factories/dipdup.yaml.j2
+-rw-r--r--   0        0        0      431 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_factories/handlers/on_origination.py.j2
+-rw-r--r--   0        0        0      540 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_factories/handlers/on_propose.py.j2
+-rw-r--r--   0        0        0      784 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_factories/models/__init__.py.j2
+-rw-r--r--   0        0        0      133 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_factories/replay.yaml
+-rw-r--r--   0        0        0      253 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_head/dipdup.yaml.j2
+-rw-r--r--   0        0        0      114 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_head/replay.yaml
+-rw-r--r--   0        0        0     1201 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/dipdup.yaml.j2
+-rw-r--r--   0        0        0      603 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/handlers/on_cancel_swap.py.j2
+-rw-r--r--   0        0        0     1035 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/handlers/on_collect.py.j2
+-rw-r--r--   0        0        0      973 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/handlers/on_mint.py.j2
+-rw-r--r--   0        0        0      883 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/handlers/on_swap.py.j2
+-rw-r--r--   0        0        0     1309 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/models/__init__.py.j2
+-rw-r--r--   0        0        0      133 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/replay.yaml
+-rw-r--r--   0        0        0      425 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_raw/dipdup.yaml.j2
+-rw-r--r--   0        0        0      364 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_raw/handlers/on_operation.py.j2
+-rw-r--r--   0        0        0      247 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_raw/models/__init__.py.j2
+-rw-r--r--   0        0        0      140 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_raw/replay.yaml
+-rw-r--r--   0        0        0      742 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_token/dipdup.yaml.j2
+-rw-r--r--   0        0        0      448 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_token/handlers/on_balance_update.py.j2
+-rw-r--r--   0        0        0      664 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_token/handlers/on_mint.py.j2
+-rw-r--r--   0        0        0      962 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_token/handlers/on_transfer.py.j2
+-rw-r--r--   0        0        0      372 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_token/models/__init__.py.j2
+-rw-r--r--   0        0        0      114 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_token/replay.yaml
+-rw-r--r--   0        0        0      411 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_token_transfers/dipdup.yaml.j2
+-rw-r--r--   0        0        0      545 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_token_transfers/handlers/on_balance_update.py.j2
+-rw-r--r--   0        0        0      836 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_token_transfers/handlers/on_token_transfer.py.j2
+-rw-r--r--   0        0        0      372 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_token_transfers/models/__init__.py.j2
+-rw-r--r--   0        0        0      133 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_token_transfers/replay.yaml
+-rw-r--r--   0        0        0     2255 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/dipdup.yaml.j2
+-rw-r--r--   0        0        0     3097 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/factory/pool_created.py.j2
+-rw-r--r--   0        0        0      568 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/pool/burn.py.j2
+-rw-r--r--   0        0        0      310 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/pool/flash.py.j2
+-rw-r--r--   0        0        0      899 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/pool/initialize.py.j2
+-rw-r--r--   0        0        0     1376 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/pool/mint.py.j2
+-rw-r--r--   0        0        0     6631 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/pool/swap.py.j2
+-rw-r--r--   0        0        0     1264 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/position_manager/collect.py.j2
+-rw-r--r--   0        0        0     1398 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/position_manager/decrease_liquidity.py.j2
+-rw-r--r--   0        0        0     1486 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/position_manager/increase_liquidity.py.j2
+-rw-r--r--   0        0        0     1200 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/position_manager/transfer.py.j2
+-rw-r--r--   0        0        0    19933 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/__init__.py.j2
+-rw-r--r--   0        0        0      374 2023-07-27 00:38:52.741560 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/abi.py.j2
+-rw-r--r--   0        0        0     4226 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/pool.py.j2
+-rw-r--r--   0        0        0     2844 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/position.py.j2
+-rw-r--r--   0        0        0     1478 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/repo.py.j2
+-rw-r--r--   0        0        0      571 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/tick.py.j2
+-rw-r--r--   0        0        0     7188 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/token.py.j2
+-rw-r--r--   0        0        0      137 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/replay.yaml
+-rw-r--r--   0        0        0     4008 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/prometheus.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/py.typed
+-rw-r--r--   0        0        0     1631 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/pysignalr.py
+-rw-r--r--   0        0        0     1722 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/report.py
+-rw-r--r--   0        0        0     4867 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/scheduler.py
+-rw-r--r--   0        0        0     4613 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/sentry.py
+-rw-r--r--   0        0        0      199 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/sql/dipdup_head_status.sql
+-rw-r--r--   0        0        0     2111 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/sql/truncate_schema.sql
+-rw-r--r--   0        0        0     2163 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/subscriptions.py
+-rw-r--r--   0        0        0     1791 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/sys.py
+-rw-r--r--   0        0        0      227 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/templates/callback.py.j2
+-rw-r--r--   0        0        0     1242 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/templates/models.py
+-rw-r--r--   0        0        0      186 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/templates/replay.yaml.j2
+-rw-r--r--   0        0        0     3290 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/transactions.py
+-rw-r--r--   0        0        0     6763 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/utils.py
+-rw-r--r--   0        0        0     5411 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/src/dipdup/yaml.py
+-rw-r--r--   0        0        0      952 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/__init__.py
+-rw-r--r--   0        0        0      496 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/asdf.yml
+-rw-r--r--   0        0        0     1222 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_auction.yml
+-rw-r--r--   0        0        0      780 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_big_maps.yml
+-rw-r--r--   0        0        0      745 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_dao.yml
+-rw-r--r--   0        0        0     5012 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_dex.yml
+-rw-r--r--   0        0        0      898 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_domains.yml
+-rw-r--r--   0        0        0      878 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_factories.yml
+-rw-r--r--   0        0        0     1316 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_nft_marketplace.yml
+-rw-r--r--   0        0        0      590 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_raw.yml
+-rw-r--r--   0        0        0      711 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_token.yml
+-rw-r--r--   0        0        0      527 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_token_transfers.yml
+-rw-r--r--   0        0        0      527 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_token_transfers_2.yml
+-rw-r--r--   0        0        0      527 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_token_transfers_3.yml
+-rw-r--r--   0        0        0      814 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/demo_token_transfers_4.yml
+-rw-r--r--   0        0        0     1252 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/dipdup.yml
+-rw-r--r--   0        0        0      521 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/hen_subjkt.yml
+-rw-r--r--   0        0        0      496 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/hjkl.yml
+-rw-r--r--   0        0        0      546 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/kolibri_ovens.yml
+-rw-r--r--   0        0        0      684 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/operation_filters.yml
+-rw-r--r--   0        0        0      496 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/qwer.yml
+-rw-r--r--   0        0        0      496 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/rewq.yml
+-rw-r--r--   0        0        0       44 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/sqlite.yaml
+-rw-r--r--   0        0        0      534 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/yupana.yml
+-rw-r--r--   0        0        0      496 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/configs/zxcv.yml
+-rw-r--r--   0        0        0     1285 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/profile_abi_decoding.py
+-rw-r--r--   0        0        0        2 2023-07-27 00:40:35.863186 dipdup-7.0.0rc2/tests/replays/024e925225593fe9cd80f5a114201f74d9f3631cea6f03add3e88fc91fafd2d7
+-rw-r--r--   0        0        0    11605 2023-07-27 00:38:52.745561 dipdup-7.0.0rc2/tests/replays/0535b2dcc93076e6026fa48cc501adaed47b7b060e6483d8312f40c184d7287d
+-rw-r--r--   0        0        0  2577538 2023-07-27 00:38:52.757561 dipdup-7.0.0rc2/tests/replays/064e788d2566d748f516b17c6a43ab34259443cc9537f0dec7c1a5a2bce704b2
+-rw-r--r--   0        0        0      305 2023-07-27 00:41:39.640181 dipdup-7.0.0rc2/tests/replays/0b7d26b8f2813d12a80b9e96cc6f0bb186bf9ac5c5b0c0b3bb2cc8d750126843
+-rw-r--r--   0        0        0      784 2023-07-27 00:38:52.757561 dipdup-7.0.0rc2/tests/replays/0eaaba2830dbdd3a80286fbc367084bce6e55c678e21da178a7eb16beef6c997
+-rw-r--r--   0        0        0       20 2023-07-27 00:38:52.757561 dipdup-7.0.0rc2/tests/replays/1165d42ccbdd0f6c25cece69d2c579da07655a30d04f18840350a153a98827a0
+-rw-r--r--   0        0        0     7446 2023-07-27 00:38:52.757561 dipdup-7.0.0rc2/tests/replays/1228b36594bb93d619170ad49373f1ceec52d10faafdd727b37f3cdeffd663db
+-rw-r--r--   0        0        0   108455 2023-07-27 00:41:29.028017 dipdup-7.0.0rc2/tests/replays/136157c421184c218127595797f5fe0b774e2807f6f4605a1d1944a1738e2d6d
+-rw-r--r--   0        0        0     4947 2023-07-27 00:38:52.757561 dipdup-7.0.0rc2/tests/replays/13afdf001ce3d6a0219c0f7f6d372d9b645770e5f4304576f7f7a37b45af96fc
+-rw-r--r--   0        0        0      310 2023-07-27 00:38:52.757561 dipdup-7.0.0rc2/tests/replays/1430e37dce64ecb83499da8feaa3c0906e4fdf5d0a3c3570174645e97ba54bc4
+-rw-r--r--   0        0        0    13275 2023-07-27 00:38:52.757561 dipdup-7.0.0rc2/tests/replays/14408f393a3e399b241184f858e70396e3b8313e32ee1a984913d43fb74dcfec
+-rw-r--r--   0        0        0   855628 2023-07-27 00:40:48.107376 dipdup-7.0.0rc2/tests/replays/14cba0424c66b1869edc8e18ca3079856083cc3db7e68ef61fce165b6d7e1a6d
+-rw-r--r--   0        0        0      129 2023-07-27 00:38:52.757561 dipdup-7.0.0rc2/tests/replays/14d37c70764fe50b4ea590691d5614f613f96b8ad98c5df189564778616f5261
+-rw-r--r--   0        0        0      246 2023-07-27 00:38:52.757561 dipdup-7.0.0rc2/tests/replays/185f6628ac43f6ca728c5b79b7b81a3c3671efce7f14030a06a27e90cf641dea
+-rw-r--r--   0        0        0      986 2023-07-27 00:38:52.757561 dipdup-7.0.0rc2/tests/replays/18d85ceab66daf057861b99b7e223a25067197b3b77edbf060390df58cb65eaa
+-rw-r--r--   0        0        0     1448 2023-07-27 00:38:52.757561 dipdup-7.0.0rc2/tests/replays/19441b677ef5fd8ca39c37e6ddd2a7d9bc8cb3ab282b2a91ce4d8430f56f0fa9
+-rw-r--r--   0        0        0   612008 2023-07-27 00:38:52.761561 dipdup-7.0.0rc2/tests/replays/1a43bd7d1397cc3169ad267cd2ef083a5a63eaac7ed5186aadfc01bb53636214
+-rw-r--r--   0        0        0  1154515 2023-07-27 00:40:48.659384 dipdup-7.0.0rc2/tests/replays/1c07d3d72acc637fb46c59d0a6dc9749f3412a5d527ca2eb0cccc01720fda1c7
+-rw-r--r--   0        0        0    89590 2023-07-27 00:38:52.761561 dipdup-7.0.0rc2/tests/replays/1c34d1f810ae474395893bf67fb8cfb27b0506ab94eebec42cd4d2d21bf3dfcd
+-rw-r--r--   0        0        0        2 2023-07-27 00:40:35.871187 dipdup-7.0.0rc2/tests/replays/1c717490846300e1639e96a0c1438b6dd2abd6de013c5edec49042fa364c06e6
+-rw-r--r--   0        0        0    12263 2023-07-27 00:38:52.761561 dipdup-7.0.0rc2/tests/replays/252fd058cfef21f9b5b7f4367f730ec7d41647253d7cc7ccfb1e22d42d1f366a
+-rw-r--r--   0        0        0     1167 2023-07-27 00:38:52.761561 dipdup-7.0.0rc2/tests/replays/27373c23411bf37b605c8d0ead9a0e6c6c1f1718ce7863b095b759811e44e155
+-rw-r--r--   0        0        0     1121 2023-07-27 00:38:52.761561 dipdup-7.0.0rc2/tests/replays/2a45ec6372b45e46199a6af24272cb93586777a0522cd1203b3eeef213ce4583
+-rw-r--r--   0        0        0   209761 2023-07-27 00:40:48.735386 dipdup-7.0.0rc2/tests/replays/31cc70e13495f58ecde80847bc6c9e08536cc426c03bd2aa8c45c1b2c798e155
+-rw-r--r--   0        0        0 21118960 2023-07-27 00:38:52.805561 dipdup-7.0.0rc2/tests/replays/31dd376b771f347a0d6fe4dd132a1f96f809274429b78ec86dd742e5589fbc23
+-rw-r--r--   0        0        0  1807578 2023-07-27 00:40:36.439195 dipdup-7.0.0rc2/tests/replays/32e3a13cc470d8720ce28f5eaff327340fb25cbe712e5b5a348af1bc3c92235a
+-rw-r--r--   0        0        0       65 2023-07-27 00:38:52.805561 dipdup-7.0.0rc2/tests/replays/33349b63491dc976a7a2332d3cca3bd9b3b831c02a6f474bb925876c1838633a
+-rw-r--r--   0        0        0        2 2023-07-27 00:38:52.805561 dipdup-7.0.0rc2/tests/replays/34f3e33d677f85b633cb85c6dd205beb40e3d9c40cfafc7084b82c8123a54de1
+-rw-r--r--   0        0        0    45221 2023-07-27 00:38:52.805561 dipdup-7.0.0rc2/tests/replays/36072e13c9ce265bb81142b8816da8c31bd9180e7c663ea4169bd259af107382
+-rw-r--r--   0        0        0    81885 2023-07-27 00:38:52.809561 dipdup-7.0.0rc2/tests/replays/377ac31d6316391ed138df44bec374d65202f0577603e80465ced3c09140f78c
+-rw-r--r--   0        0        0    54602 2023-07-27 00:40:58.807544 dipdup-7.0.0rc2/tests/replays/383899084f79460e96fd311bb64e4925738c486b39d6281539456c5fcac41620
+-rw-r--r--   0        0        0      642 2023-07-27 00:41:24.739950 dipdup-7.0.0rc2/tests/replays/39b8664d1bca5d374ff905c8a3a396b53d19ee469dc37545a8ca6b080bd0e9e0
+-rw-r--r--   0        0        0     1200 2023-07-27 00:41:40.600196 dipdup-7.0.0rc2/tests/replays/3a2bd8b6b72bf18152d2550c106789fa9b8abc98ea9d759a6597b7ebfbab0fc2
+-rw-r--r--   0        0        0    81885 2023-07-27 00:38:52.809561 dipdup-7.0.0rc2/tests/replays/3c9ad6f98f79e72185ea58c4777115750c658c5defd616664212095bd440c10c
+-rw-r--r--   0        0        0      332 2023-07-27 00:38:52.809561 dipdup-7.0.0rc2/tests/replays/3fdba02cbc415eba224604f4fea130acd4565d31e4a83cdbb679ec0b76c798ab
+-rw-r--r--   0        0        0  3369404 2023-07-27 00:41:12.907765 dipdup-7.0.0rc2/tests/replays/42b7bf0da866257ef98e1f7124d2d21fe7d13228c076fffa32331da423f36933
+-rw-r--r--   0        0        0      619 2023-07-27 00:38:52.809561 dipdup-7.0.0rc2/tests/replays/43cb0ab415d8b8b3f7addc3e82ea27d93b2c66ff55c117e1e0c7c64a0fcfc3f2
+-rw-r--r--   0        0        0   530743 2023-07-27 00:38:52.809561 dipdup-7.0.0rc2/tests/replays/440173d32e95111ca7b080ccc4dc09bfab23c8361919b2c113f0ff9ab445eec2
+-rw-r--r--   0        0        0  1594116 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/489233ce9373f7de4f7a9053055c74bc0df999bfe939ed67d98b6d67e676e35a
+-rw-r--r--   0        0        0   109726 2023-07-27 00:40:46.155345 dipdup-7.0.0rc2/tests/replays/4a57776d93475adfd9c49b6c3295a7cedfc23b73733a1fb5f0c985ee039dc5dc
+-rw-r--r--   0        0        0      984 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/4aa7f9b0657be0c44baf2caed8c7cb08d02097a4095cf6417f78cba3a25e8423
+-rw-r--r--   0        0        0       67 2023-07-27 00:41:37.552149 dipdup-7.0.0rc2/tests/replays/4fbdb4667971fab446a5ac5937a7c8cc6ef5813ff00af24b6fd1b1a0427bedbb
+-rw-r--r--   0        0        0   192680 2023-07-27 00:40:46.003343 dipdup-7.0.0rc2/tests/replays/5483a0e11009e0f186bf70c214e2597d267a75a1e19152a9e7ed1ec257ce88ca
+-rw-r--r--   0        0        0       65 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/56eb33fbb563bf03ea7639659fae5102222d6e3cea882febf71f01bd383c6eed
+-rw-r--r--   0        0        0    40432 2023-07-27 00:40:58.671542 dipdup-7.0.0rc2/tests/replays/587613799ebfae42b1884016d1a44a452d68e70e3ed80641d90b8e7657ba8ee5
+-rw-r--r--   0        0        0       32 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/5b004196490632859ec1b019d640f6bbb93fc86a433c8969e10f36f51ac2c78d
+-rw-r--r--   0        0        0     1907 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/5b7c31b4b73bc57e8296e6051b3bc7b2302b32588d8fbcafce8a66de3be743df
+-rw-r--r--   0        0        0     7609 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/5b99bc4beb6a9a33f7d2f118426458e4c788e0ab6d9e51949d3ccbf8b4003fc1
+-rw-r--r--   0        0        0      939 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/5d21060ba8e78279d2d1edaa2f266ecf36105eaccef5ebed15748441651f76fd
+-rw-r--r--   0        0        0      400 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/5f63ef9dd15459ae14e715bb79da8f033a24b54504212ebc873ee8aa95679606
+-rw-r--r--   0        0        0       67 2023-07-27 00:41:37.680151 dipdup-7.0.0rc2/tests/replays/60f48c13c47a1347786a6dcf6f741874e7b30b587d148faa67d15067bb3871de
+-rw-r--r--   0        0        0       21 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/62e95f1d55b756895289374b351a1da94505ec2d95a1652c97765f36a2ef9341
+-rw-r--r--   0        0        0   211527 2023-07-27 00:40:49.571399 dipdup-7.0.0rc2/tests/replays/6cc8d741a41b76983cd7e0f63e8f22a4c67cd946888f45a5b7ead8c3bb5ad2f1
+-rw-r--r--   0        0        0   944885 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/6cff8d120db8fd3926a45714ce7f1d0560803eb5a7b4a413b64fee1b7fd7a8ff
+-rw-r--r--   0        0        0      132 2023-07-27 00:41:38.316161 dipdup-7.0.0rc2/tests/replays/6d0c5443d41a15551acb41adc10d36d4895f5786d6922a878b5c5414610e0ebc
+-rw-r--r--   0        0        0      754 2023-07-27 00:41:39.140174 dipdup-7.0.0rc2/tests/replays/6d76a3c3f427ff534c551de1793cb1d1dfbd22ccad97f5917a9f9b201a3f9804
+-rw-r--r--   0        0        0      494 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/7132f07560319399092782debe6eb28926e961d8af215ce11e2c0efd8dab06da
+-rw-r--r--   0        0        0      451 2023-07-27 00:41:39.760183 dipdup-7.0.0rc2/tests/replays/739d17c86095aac3da3508a16dc1c9ae9459ea86eeb09f62aaefc32de2997918
+-rw-r--r--   0        0        0        2 2023-07-27 00:41:43.268237 dipdup-7.0.0rc2/tests/replays/759b79ec12b1305d9fa8e1a5218e62bb3d3ad913580e19914d30d8aa09920ae4
+-rw-r--r--   0        0        0   209456 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/7669ea717d9759748aed86302326b79be5157a1a36d13b39b00f06bcbe22b309
+-rw-r--r--   0        0        0      520 2023-07-27 00:38:52.813562 dipdup-7.0.0rc2/tests/replays/76d49ae3b723376c88ca65a3080a273e098d226932a1a49c38fbc4421e7c2e64
+-rw-r--r--   0        0        0    50588 2023-07-27 00:41:15.991813 dipdup-7.0.0rc2/tests/replays/7b6cf9b8c69712bf26ed09059352ec740606969bf20eab0dedda870273f4fde9
+-rw-r--r--   0        0        0 21649088 2023-07-27 00:41:14.223785 dipdup-7.0.0rc2/tests/replays/7b9c78209f98b2c3a6678ed224fa686eee25c3c63dddd7f9af77c734b0dfabb8
+-rw-r--r--   0        0        0      807 2023-07-27 00:41:41.524210 dipdup-7.0.0rc2/tests/replays/803e05a8d0bb9e7cfb49530271d43ea62111b6419e7cded2d221f7e0e0c92ece
+-rw-r--r--   0        0        0   517204 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/80921fd33043def891912a6ad57d76664399564fd813950eb11f4a0e69e3e28f
+-rw-r--r--   0        0        0      129 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/815c066c21f7d2697ef107cad4624a9c4079a7a1dab7974d606fc42b81fe93c8
+-rw-r--r--   0        0        0      939 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/816d08f71c84537ea8df05a40678b1addca15bf3a73c0e927c75d9f9c0f2d418
+-rw-r--r--   0        0        0      395 2023-07-27 00:41:41.240206 dipdup-7.0.0rc2/tests/replays/8335acc6585656ec3a4301cd8b089401f2dc2c7d758b381c96c730e610b67f7b
+-rw-r--r--   0        0        0   207502 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/84cf46aa9c8dbd3ca6c3d946c749713e6c70a6a20d9cc69b4156235fd099b2e3
+-rw-r--r--   0        0        0        2 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/8ad31f6cf9c873b1fd9827b621529c43966f8376a86fcac3b1d20c260b78007e
+-rw-r--r--   0        0        0       65 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/91787fdbd1634f277b20ac46cb30eba9770f83df7189df0903e22f5f4bbe1efa
+-rw-r--r--   0        0        0     1151 2023-07-27 00:41:42.036218 dipdup-7.0.0rc2/tests/replays/93516225810a23a6799f2f9a1dee055ca79a66ee2b8d0f32be820c9c385e936b
+-rw-r--r--   0        0        0      494 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/9ce1bc12a2adeddcf9d8854c4b63a8e65b58d9206fb8d2e3eedb24c44ea7f28a
+-rw-r--r--   0        0        0       22 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/9de859083ed1dd278893f60b5a60feab02a04637327a664af23f52dabb139fe6
+-rw-r--r--   0        0        0      706 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/9e6e907842da2cd494c558ea5ecc211fd12e56bfc547450978fb7dfe03853e58
+-rw-r--r--   0        0        0     6981 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/a3ce91a1b0d505cc221f0e201781466ba1e2d6dc7b624b9bc75a03ce3dbb0f92
+-rw-r--r--   0        0        0    38974 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/a795ef429bde71b3ba66b545c0048f57a78ab5d2247772761d8efe86567199b9
+-rw-r--r--   0        0        0        2 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/a840afa5674efd06639c4692a8bfe9ed6e1346bfe9c414209eec5d9126333242
+-rw-r--r--   0        0        0      675 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/aa8fe6037996b296bf9a3011e45cd9ecb92fb728592a843f91b03b2848cb1fb1
+-rw-r--r--   0        0        0     1882 2023-07-27 00:41:09.003704 dipdup-7.0.0rc2/tests/replays/acc952ba1905717315212f952ed689d7b8f683165b31c0a7a25199aed9fda27f
+-rw-r--r--   0        0        0      356 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/aeee37b6f63a3177e0e27ac472008c3cba3d30ebee691fb45de1bae91a87f2ce
+-rw-r--r--   0        0        0       67 2023-07-27 00:41:37.424147 dipdup-7.0.0rc2/tests/replays/af37212b31e932f269c42c7f34ad8f3849bd8aed244652c41b9327c508985ce5
+-rw-r--r--   0        0        0     1200 2023-07-27 00:41:35.848123 dipdup-7.0.0rc2/tests/replays/b3af887f7ad8172af75b94a09bedfb9ae1e14f8819a36d6ce9f709721068263b
+-rw-r--r--   0        0        0  1214926 2023-07-27 00:40:48.319379 dipdup-7.0.0rc2/tests/replays/b49fb33ee80345b70414ad08806a860e2139c20d98a5150c6ccd1b28a90f311e
+-rw-r--r--   0        0        0     2271 2023-07-27 00:41:34.632104 dipdup-7.0.0rc2/tests/replays/bec4433b4206f00c2310a7961cff7f539434b9161b45673793aa5a3b50234313
+-rw-r--r--   0        0        0      310 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/bed2329e63d559db2fb81c69606e715d1f90aaacab6ae45b33516e7828841a3c
+-rw-r--r--   0        0        0       65 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/bf941ceae7a6e3c40406438e067f137131e6605924a93d43bafc77682b602c55
+-rw-r--r--   0        0        0   759209 2023-07-27 00:40:48.435381 dipdup-7.0.0rc2/tests/replays/c0202a433296436c27458b3d5ec5c72d5e2d47ff77c939ce399780cc0f3e56bc
+-rw-r--r--   0        0        0    19100 2023-07-27 00:38:52.817561 dipdup-7.0.0rc2/tests/replays/c369836c15d9ed15477002b850d5cbb96b1ff5ff33e917b812ab9c0905063957
+-rw-r--r--   0        0        0   918908 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/c8e8698717ada415bc10405da983c8357165914dd0219f3d09bb9a939705242d
+-rw-r--r--   0        0        0   691878 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/cc162df04c4990c79f7507dd915601fd4d58c947a248156cbe302a64adfe898a
+-rw-r--r--   0        0        0     7446 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/cc5d3d4a58d5cb6bc7270d38c797b7740b79f913590ef0164abd50e58fba9405
+-rw-r--r--   0        0        0      301 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/cc648800928fd43f8e72db1d41115c26a22346c9c7831172fe422c1765cd67f2
+-rw-r--r--   0        0        0      960 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/d0a594d14bcb3fbf916092ec6707dfd3c9f48f53f0a1ad40a32023e7a87f8ef5
+-rw-r--r--   0        0        0     2403 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/d62748a927a09395579b5790c8f871cc8653081cf4475abc93173989f950b92b
+-rw-r--r--   0        0        0     9089 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/d94397f6ecec8ce25f87177fe410f6498d7d30a04360506c0cd300d291c167e7
+-rw-r--r--   0        0        0      132 2023-07-27 00:41:36.764137 dipdup-7.0.0rc2/tests/replays/db797e6bf4c1b9c3237af5dec694fb1b6d21418a5a2f7947eb7f54d4e9201baf
+-rw-r--r--   0        0        0   548925 2023-07-27 00:41:14.491790 dipdup-7.0.0rc2/tests/replays/dc86d5e346c85e6f7953d7e01298a9db64d778e5ba717ddd07fff8b589081e98
+-rw-r--r--   0        0        0    20467 2023-07-27 00:40:36.003188 dipdup-7.0.0rc2/tests/replays/dca9cf4f9f27623f10975d369444899458ab9ea85c22af2da6ce6ce8c09c2b58
+-rw-r--r--   0        0        0      700 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/df62701276d6dbf4860058cc582c0b4f7b583758f4f5be96c9ee045757c151e3
+-rw-r--r--   0        0        0   151396 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/e39ebba701031aa13dfd9eb5dba1effd2938e96682d1030dcbd70172f9f190a9
+-rw-r--r--   0        0        0     7917 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/e4a563a0b19379a44e9d2dc398131e9fd30d6039ff4ffacf1252db0bf8b433aa
+-rw-r--r--   0        0        0       67 2023-07-27 00:41:37.804153 dipdup-7.0.0rc2/tests/replays/e82ba90c8570b92c0b1fc360b853aca3f1d7de457aacb9f6f19fa3e43879a8b3
+-rw-r--r--   0        0        0      132 2023-07-27 00:41:36.912139 dipdup-7.0.0rc2/tests/replays/e9fa56a94eb559c550dfbca4b27ef350a0b4a787afbe60205482a38223dcea04
+-rw-r--r--   0        0        0   713738 2023-07-27 00:41:35.700120 dipdup-7.0.0rc2/tests/replays/eb8b6b33cb2e165d1a3a73c09938d3083671a82ad73d4c0cff1fb2a5e5715f76
+-rw-r--r--   0        0        0    11290 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/eb8e2c3ce2fe7792d2c8e81c61d37821275b64021343103b0c955042ae802189
+-rw-r--r--   0        0        0      584 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/ece1ebe13f9391555230d6b94f33d66a922e2ca71ef5fd39bbd8c2c37ddf54ec
+-rw-r--r--   0        0        0     1089 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/ed3ec9fd9226e9f765b96dc1d5d5a455a7b2505da530961826910b08db693070
+-rw-r--r--   0        0        0    17245 2023-07-27 00:41:20.451883 dipdup-7.0.0rc2/tests/replays/f3d608f99e6b92e28a064bb9c10c3c605c9c817383c1eebcc68f663d1d23d650
+-rw-r--r--   0        0        0    32513 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/f60e794a9be14263cb10e48546ba5610302cc3e7af0a114a593bb50eb85ba5e7
+-rw-r--r--   0        0        0       21 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/fd9e33296006ad295c9fdc4868763f954a9c6d7c81d543ba198c14a72eea7e6b
+-rw-r--r--   0        0        0      832 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/replays/ff51b3535acc2972090ecd5db3af8f827464c9d92f1aa661630976e5b4ed4cbe
+-rw-r--r--   0        0        0     4599 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/responses/asdf.json
+-rw-r--r--   0        0        0     6704 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/responses/ftzfun.json
+-rw-r--r--   0        0        0     3445 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/responses/hen_subjkt.json
+-rw-r--r--   0        0        0     5210 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/responses/hjkl.json
+-rw-r--r--   0        0        0     2097 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/responses/kolibri_ovens.json
+-rw-r--r--   0        0        0    11186 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/responses/ooQuCAKBHkmWy2VciDAV9c6CFTywuMLupLzVoKDwS1xvR4EdRng.json
+-rw-r--r--   0        0        0     1811 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/responses/origination_amount.json
+-rw-r--r--   0        0        0     4256 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/responses/qwer.json
+-rw-r--r--   0        0        0     5307 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/responses/rewq.json
+-rw-r--r--   0        0        0    38178 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/responses/yupana.json
+-rw-r--r--   0        0        0     5909 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/responses/zxcv.json
+-rw-r--r--   0        0        0     1077 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/schemas/asdf/storage.json
+-rw-r--r--   0        0        0     2116 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/schemas/hen_subjkt/storage.json
+-rw-r--r--   0        0        0     1638 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/schemas/hjkl/storage.json
+-rw-r--r--   0        0        0      800 2023-07-27 00:38:52.821561 dipdup-7.0.0rc2/tests/schemas/kolibri_ovens/storage.json
+-rw-r--r--   0        0        0     1005 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/schemas/qwer/storage.json
+-rw-r--r--   0        0        0     2212 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/schemas/rewq/storage.json
+-rw-r--r--   0        0        0    12561 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/schemas/yupana/storage.json
+-rw-r--r--   0        0        0     2660 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/schemas/zxcv/storage.json
+-rw-r--r--   0        0        0     3767 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_config/test_callbacks.py
+-rw-r--r--   0        0        0     4643 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_config/test_config.py
+-rw-r--r--   0        0        0     4138 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_config/test_custom_config.py
+-rw-r--r--   0        0        0     2486 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_context.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_datasources/__init__.py
+-rw-r--r--   0        0        0      814 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_datasources/test_ipfs.py
+-rw-r--r--   0        0        0      663 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_datasources/test_metadata.py
+-rw-r--r--   0        0        0     8304 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_datasources/test_tzkt.py
+-rw-r--r--   0        0        0     1223 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_datasources/test_tzkt_blocks.py
+-rw-r--r--   0        0        0     1971 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_datasources/test_tzkt_buffer.py
+-rw-r--r--   0        0        0     1433 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_datasources/test_tzkt_quotes.py
+-rw-r--r--   0        0        0     8700 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_demos.py
+-rw-r--r--   0        0        0     2734 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_dipdup.py
+-rw-r--r--   0        0        0     5045 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_hasura.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_http.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_index/__init__.py
+-rw-r--r--   0        0        0     3714 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_index/test_operation.py
+-rw-r--r--   0        0        0     5772 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_introspection.py
+-rw-r--r--   0        0        0    14279 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_models.py
+-rw-r--r--   0        0        0    13401 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_rollback.py
+-rw-r--r--   0        0        0     2628 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/asdf/__init__.py
+-rw-r--r--   0        0        0      504 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/asdf/storage.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/bazaar/__init__.py
+-rw-r--r--   0        0        0      564 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/bazaar/storage.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/ftzfun/__init__.py
+-rw-r--r--   0        0        0      929 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/ftzfun/storage.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/hen_subjkt/__init__.py
+-rw-r--r--   0        0        0      583 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/hen_subjkt/storage.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/hjkl/__init__.py
+-rw-r--r--   0        0        0      647 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/hjkl/storage.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/kolibri_ovens/__init__.py
+-rw-r--r--   0        0        0      232 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/kolibri_ovens/set_delegate.py
+-rw-r--r--   0        0        0      392 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/kolibri_ovens/storage.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/listofmaps/__init__.py
+-rw-r--r--   0        0        0      153 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/listofmaps/storage.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/qwer/__init__.py
+-rw-r--r--   0        0        0      532 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/qwer/storage.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/rewq/__init__.py
+-rw-r--r--   0        0        0      831 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/rewq/storage.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/tezotop/__init__.py
+-rw-r--r--   0        0        0      740 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/tezotop/storage.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/yupana/__init__.py
+-rw-r--r--   0        0        0     2721 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/yupana/storage.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/zxcv/__init__.py
+-rw-r--r--   0        0        0     1048 2023-07-27 00:38:52.825562 dipdup-7.0.0rc2/tests/types/zxcv/storage.py
+-rw-r--r--   0        0        0     5756 1970-01-01 00:00:00.000000 dipdup-7.0.0rc2/PKG-INFO
```

### Comparing `dipdup-7.0.0rc1/LICENSE` & `dipdup-7.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/README.md` & `dipdup-7.0.0rc2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 [![GitHub issues](https://img.shields.io/github/issues/dipdup-io/dipdup?color=2c2c2c)](https://github.com/dipdup-io/dipdup/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/dipdup-io/dipdup?color=2c2c2c)](https://github.com/dipdup-io/dipdup/pulls)
 
 <h3 align="center"><img src="https://actual-docs.interface-1bp.pages.dev/_nuxt/logo.9b02ab5e.svg" alt="DipDup logo"></h3>
 
 DipDup is a Python framework for building smart contract indexers. It helps developers focus on business logic instead of writing a boilerplate to store and serve data. DipDup-based indexers are selective, which means only required data is requested. This approach allows to achieve faster indexing times and decreased load on underlying APIs.
 
-* **Ready to build your first indexer?** Head to [Quickstart](https://docs.dipdup.io/quickstart).
+- **Ready to build your first indexer?** Head to [Quickstart](https://dipdup.io/docs/quickstart).
 
-* **Looking for examples?** Check out [Demo Projects](https://docs.dipdup.io/examples/demo-projects) and [Built with DipDup](https://docs.dipdup.io/examples/built-with-dipdup) pages.
+- **Looking for examples?** Check out [Demo Projects](https://dipdup.io/docs/examples/demos) and [Built with DipDup](https://dipdup.io/docs/examples/built-with-dipdup) pages.
 
-* **Want to participate?** Vote for [open issues](https://github.com/dipdup-io/dipdup/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc), join [discussions](https://github.com/dipdup-io/dipdup/discussions) or [become a sponsor](https://github.com/sponsors/dipdup-io).
+- **Want to participate?** Vote for [open issues](https://github.com/dipdup-io/dipdup/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc), join [discussions](https://github.com/dipdup-io/dipdup/discussions) or [become a sponsor](https://github.com/sponsors/dipdup-io).
 
-* **Have a question?** Join our [Discord](https://discord.gg/NbANhqCJHA) or tag @dipdup_io on [Twitter](https://twitter.com/dipdup_io).
+- **Have a question?** Join our [Discord](https://discord.gg/NbANhqCJHA) or tag @dipdup_io on [Twitter](https://twitter.com/dipdup_io).
 
 This project is maintained by the [Baking Bad](https://bakingbad.dev/) team.
 <br>
-Development is supported by [Tezos Foundation](https://tezos.foundation/).
+Development is supported by [Tezos Foundation](https://tezos.foundation/) and [OnlyDust](https://www.onlydust.xyz).
 
 ## Thanks
 
 ### Sponsors
 
 Decentralized web requires decentralized funding. The following people and organizations help the project to be sustainable.
```

### Comparing `dipdup-7.0.0rc1/pyproject.toml` & `dipdup-7.0.0rc2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "dipdup"
 description = "Modular framework for creating selective indexers and featureful backends for dapps"
-version = "7.0.0rc1"
+version = "7.0.0rc2"
 authors = [
     { name = "Lev Gorodetskii", email = "dipdup@drsr.io" },
     { name = "Vladimir Bobrikov", email = "vladimir_bobrikov@pm.me" },
     { name = "Michael Zaikin", email = "mz@baking-bad.org" },
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
@@ -69,15 +69,15 @@
 ]
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://dipdup.io/"
-Documentation = "https://docs.dipdup.io"
+Documentation = "https://dipdup.io/docs"
 Repository = "https://github.com/dipdup-io/dipdup"
 
 [project.scripts]
 dipdup = "dipdup.cli:cli"
 
 [tool.pdm.dev-dependencies]
 dev = [
@@ -107,14 +107,15 @@
 _mypy = "mypy src tests scripts"
 test = "pytest --cov-report=term-missing --cov=dipdup --cov-report=xml -n auto -s -v tests"
 image = "docker buildx build . --load --progress plain -t dipdup:latest"
 clean = "git clean -xdf --exclude=.venv"
 docs_build = "python scripts/docs.py --source docs --destination {args:../interface}/content/docs"
 docs_serve = "python scripts/docs.py --source docs --destination {args:../interface}/content/docs --watch --serve"
 docs_watch = "python scripts/docs.py --source docs --destination {args:../interface}/content/docs --watch"
+docs_references = "python scripts/dump_references.py"
 
 [tool.pdm.scripts.all]
 composite = [
     "fmt",
     "lint",
     "test",
 ]
```

### Comparing `dipdup-7.0.0rc1/src/demo_auction/README.md` & `dipdup-7.0.0rc2/src/demo_auction/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
 ```bash
 curl -Lsf https://dipdup.io/install.py | python3
 ```
 
-See the [Installation](https://docs.dipdup.io/installation) page for all options.
+See the [Installation](https://dipdup.io/docs/installation) page for all options.
 
 ## Usage
 
 Run the indexer in-memory:
 
 ```bash
 dipdup run
@@ -27,17 +27,17 @@
 ```bash
 dipdup -c . -c configs/dipdup.sqlite.yml run
 ```
 
 Or spawn a docker-compose stack:
 
 ```bash
-cp deploy/.env.example .env
+cp deploy/.env.default deploy/.env
 # Edit .env before running
-docker-compose -f deploy/docker-compose.yml up
+docker-compose -f deploy/compose.yaml up
 ```
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
```

### Comparing `dipdup-7.0.0rc1/src/demo_auction/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc2/src/demo_auction/deploy/compose.swarm.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     deploy:
       mode: replicated
       replicas: 1
       placement: *placement
     logging: *logging
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     depends_on:
       - db
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@demo_auction_db:5432/dipdup
       - HASURA_GRAPHQL_ADMIN_SECRET=${HASURA_SECRET}
       - HASURA_GRAPHQL_ENABLE_CONSOLE=true
       - HASURA_GRAPHQL_DEV_MODE=false
```

### Comparing `dipdup-7.0.0rc1/src/demo_auction/deploy/compose.yaml` & `dipdup-7.0.0rc2/src/demo_auction/deploy/compose.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     healthcheck:
       test: ["CMD-SHELL", "pg_isready -U dipdup"]
       interval: 10s
       timeout: 5s
       retries: 5
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     ports:
       - 8080
     depends_on:
       - db
     restart: always
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@db:5432/dipdup
```

### Comparing `dipdup-7.0.0rc1/src/demo_auction/dipdup.yaml` & `dipdup-7.0.0rc2/src/demo_auction/dipdup.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,71 +1,68 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
-00000020: 6175 6374 696f 6e0a 0a64 6174 6162 6173  auction..databas
-00000030: 653a 0a20 206b 696e 643a 2073 716c 6974  e:.  kind: sqlit
-00000040: 650a 2020 7061 7468 3a20 6465 6d6f 5f61  e.  path: demo_a
-00000050: 7563 7469 6f6e 2e73 716c 6974 6533 0a0a  uction.sqlite3..
-00000060: 636f 6e74 7261 6374 733a 0a20 2074 7a63  contracts:.  tzc
-00000070: 6f6c 6f72 735f 6d69 6e74 6572 3a0a 2020  olors_minter:.  
-00000080: 2020 6b69 6e64 3a20 7465 7a6f 730a 2020    kind: tezos.  
-00000090: 2020 6164 6472 6573 733a 204b 5431 4679    address: KT1Fy
-000000a0: 6144 7169 4d51 5767 3745 786f 3756 5569  aDqiMQWg7Exo7VUi
-000000b0: 5841 675a 6264 326b 437a 6f33 6434 730a  XAgZbd2kCzo3d4s.
-000000c0: 2020 2020 7479 7065 6e61 6d65 3a20 747a      typename: tz
-000000d0: 636f 6c6f 7273 5f6d 696e 7465 720a 2020  colors_minter.  
-000000e0: 747a 636f 6c6f 7273 5f61 7563 7469 6f6e  tzcolors_auction
-000000f0: 3a0a 2020 2020 6b69 6e64 3a20 7465 7a6f  :.    kind: tezo
-00000100: 730a 2020 2020 6164 6472 6573 733a 204b  s.    address: K
-00000110: 5431 4370 6553 514b 646b 6857 6934 7069  T1CpeSQKdkhWi4pi
-00000120: 6e59 6373 6543 464b 6d44 6873 354d 3734  nYcseCFKmDhs5M74
-00000130: 426b 550a 2020 2020 7479 7065 6e61 6d65  BkU.    typename
-00000140: 3a20 747a 636f 6c6f 7273 5f61 7563 7469  : tzcolors_aucti
-00000150: 6f6e 0a0a 6461 7461 736f 7572 6365 733a  on..datasources:
-00000160: 0a20 2074 7a6b 743a 0a20 2020 206b 696e  .  tzkt:.    kin
-00000170: 643a 2074 657a 6f73 2e74 7a6b 740a 2020  d: tezos.tzkt.  
-00000180: 2020 7572 6c3a 2024 7b54 5a4b 545f 5552    url: ${TZKT_UR
-00000190: 4c3a 2d68 7474 7073 3a2f 2f61 7069 2e74  L:-https://api.t
-000001a0: 7a6b 742e 696f 7d0a 0a74 656d 706c 6174  zkt.io}..templat
-000001b0: 6573 3a0a 2020 6175 6374 696f 6e3a 0a20  es:.  auction:. 
-000001c0: 2020 206b 696e 643a 2074 657a 6f73 2e74     kind: tezos.t
-000001d0: 7a6b 742e 6f70 6572 6174 696f 6e73 0a20  zkt.operations. 
-000001e0: 2020 2064 6174 6173 6f75 7263 653a 203c     datasource: <
-000001f0: 6461 7461 736f 7572 6365 3e0a 2020 2020  datasource>.    
-00000200: 636f 6e74 7261 6374 733a 0a20 2020 2020  contracts:.     
-00000210: 202d 203c 6175 6374 696f 6e3e 0a20 2020   - <auction>.   
-00000220: 2068 616e 646c 6572 733a 0a20 2020 2020   handlers:.     
-00000230: 202d 2063 616c 6c62 6163 6b3a 206f 6e5f   - callback: on_
-00000240: 6372 6561 7465 5f61 7563 7469 6f6e 0a20  create_auction. 
-00000250: 2020 2020 2020 2070 6174 7465 726e 3a0a         pattern:.
-00000260: 2020 2020 2020 2020 2020 2d20 7479 7065            - type
-00000270: 3a20 7472 616e 7361 6374 696f 6e0a 2020  : transaction.  
-00000280: 2020 2020 2020 2020 2020 6465 7374 696e            destin
-00000290: 6174 696f 6e3a 203c 6175 6374 696f 6e3e  ation: <auction>
-000002a0: 0a20 2020 2020 2020 2020 2020 2065 6e74  .            ent
-000002b0: 7279 706f 696e 743a 2063 7265 6174 655f  rypoint: create_
-000002c0: 6175 6374 696f 6e0a 2020 2020 2020 2d20  auction.      - 
-000002d0: 6361 6c6c 6261 636b 3a20 6f6e 5f62 6964  callback: on_bid
-000002e0: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
-000002f0: 3a0a 2020 2020 2020 2020 2020 2d20 7479  :.          - ty
-00000300: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
-00000310: 2020 2020 2020 2020 2020 2020 6465 7374              dest
-00000320: 696e 6174 696f 6e3a 203c 6175 6374 696f  ination: <auctio
-00000330: 6e3e 0a20 2020 2020 2020 2020 2020 2065  n>.            e
-00000340: 6e74 7279 706f 696e 743a 2062 6964 0a20  ntrypoint: bid. 
-00000350: 2020 2020 202d 2063 616c 6c62 6163 6b3a       - callback:
-00000360: 206f 6e5f 7769 7468 6472 6177 0a20 2020   on_withdraw.   
-00000370: 2020 2020 2070 6174 7465 726e 3a0a 2020       pattern:.  
-00000380: 2020 2020 2020 2020 2d20 7479 7065 3a20          - type: 
-00000390: 7472 616e 7361 6374 696f 6e0a 2020 2020  transaction.    
-000003a0: 2020 2020 2020 2020 6465 7374 696e 6174          destinat
-000003b0: 696f 6e3a 203c 6175 6374 696f 6e3e 0a20  ion: <auction>. 
-000003c0: 2020 2020 2020 2020 2020 2065 6e74 7279             entry
-000003d0: 706f 696e 743a 2077 6974 6864 7261 770a  point: withdraw.
-000003e0: 0a69 6e64 6578 6573 3a0a 2020 747a 636f  .indexes:.  tzco
-000003f0: 6c6f 7273 3a0a 2020 2020 7465 6d70 6c61  lors:.    templa
-00000400: 7465 3a20 6175 6374 696f 6e0a 2020 2020  te: auction.    
-00000410: 7661 6c75 6573 3a0a 2020 2020 2020 6461  values:.      da
-00000420: 7461 736f 7572 6365 3a20 747a 6b74 0a20  tasource: tzkt. 
-00000430: 2020 2020 206d 696e 7465 723a 2074 7a63       minter: tzc
-00000440: 6f6c 6f72 735f 6d69 6e74 6572 0a20 2020  olors_minter.   
-00000450: 2020 2061 7563 7469 6f6e 3a20 747a 636f     auction: tzco
-00000460: 6c6f 7273 5f61 7563 7469 6f6e            lors_auction
+00000020: 6175 6374 696f 6e0a 0a63 6f6e 7472 6163  auction..contrac
+00000030: 7473 3a0a 2020 747a 636f 6c6f 7273 5f6d  ts:.  tzcolors_m
+00000040: 696e 7465 723a 0a20 2020 206b 696e 643a  inter:.    kind:
+00000050: 2074 657a 6f73 0a20 2020 2061 6464 7265   tezos.    addre
+00000060: 7373 3a20 4b54 3146 7961 4471 694d 5157  ss: KT1FyaDqiMQW
+00000070: 6737 4578 6f37 5655 6958 4167 5a62 6432  g7Exo7VUiXAgZbd2
+00000080: 6b43 7a6f 3364 3473 0a20 2020 2074 7970  kCzo3d4s.    typ
+00000090: 656e 616d 653a 2074 7a63 6f6c 6f72 735f  ename: tzcolors_
+000000a0: 6d69 6e74 6572 0a20 2074 7a63 6f6c 6f72  minter.  tzcolor
+000000b0: 735f 6175 6374 696f 6e3a 0a20 2020 206b  s_auction:.    k
+000000c0: 696e 643a 2074 657a 6f73 0a20 2020 2061  ind: tezos.    a
+000000d0: 6464 7265 7373 3a20 4b54 3143 7065 5351  ddress: KT1CpeSQ
+000000e0: 4b64 6b68 5769 3470 696e 5963 7365 4346  KdkhWi4pinYcseCF
+000000f0: 4b6d 4468 7335 4d37 3442 6b55 0a20 2020  KmDhs5M74BkU.   
+00000100: 2074 7970 656e 616d 653a 2074 7a63 6f6c   typename: tzcol
+00000110: 6f72 735f 6175 6374 696f 6e0a 0a64 6174  ors_auction..dat
+00000120: 6173 6f75 7263 6573 3a0a 2020 747a 6b74  asources:.  tzkt
+00000130: 3a0a 2020 2020 6b69 6e64 3a20 7465 7a6f  :.    kind: tezo
+00000140: 732e 747a 6b74 0a20 2020 2075 726c 3a20  s.tzkt.    url: 
+00000150: 247b 545a 4b54 5f55 524c 3a2d 6874 7470  ${TZKT_URL:-http
+00000160: 733a 2f2f 6170 692e 747a 6b74 2e69 6f7d  s://api.tzkt.io}
+00000170: 0a0a 7465 6d70 6c61 7465 733a 0a20 2061  ..templates:.  a
+00000180: 7563 7469 6f6e 3a0a 2020 2020 6b69 6e64  uction:.    kind
+00000190: 3a20 7465 7a6f 732e 747a 6b74 2e6f 7065  : tezos.tzkt.ope
+000001a0: 7261 7469 6f6e 730a 2020 2020 6461 7461  rations.    data
+000001b0: 736f 7572 6365 3a20 3c64 6174 6173 6f75  source: <datasou
+000001c0: 7263 653e 0a20 2020 2063 6f6e 7472 6163  rce>.    contrac
+000001d0: 7473 3a0a 2020 2020 2020 2d20 3c61 7563  ts:.      - <auc
+000001e0: 7469 6f6e 3e0a 2020 2020 6861 6e64 6c65  tion>.    handle
+000001f0: 7273 3a0a 2020 2020 2020 2d20 6361 6c6c  rs:.      - call
+00000200: 6261 636b 3a20 6f6e 5f63 7265 6174 655f  back: on_create_
+00000210: 6175 6374 696f 6e0a 2020 2020 2020 2020  auction.        
+00000220: 7061 7474 6572 6e3a 0a20 2020 2020 2020  pattern:.       
+00000230: 2020 202d 2074 7970 653a 2074 7261 6e73     - type: trans
+00000240: 6163 7469 6f6e 0a20 2020 2020 2020 2020  action.         
+00000250: 2020 2064 6573 7469 6e61 7469 6f6e 3a20     destination: 
+00000260: 3c61 7563 7469 6f6e 3e0a 2020 2020 2020  <auction>.      
+00000270: 2020 2020 2020 656e 7472 7970 6f69 6e74        entrypoint
+00000280: 3a20 6372 6561 7465 5f61 7563 7469 6f6e  : create_auction
+00000290: 0a20 2020 2020 202d 2063 616c 6c62 6163  .      - callbac
+000002a0: 6b3a 206f 6e5f 6269 640a 2020 2020 2020  k: on_bid.      
+000002b0: 2020 7061 7474 6572 6e3a 0a20 2020 2020    pattern:.     
+000002c0: 2020 2020 202d 2074 7970 653a 2074 7261       - type: tra
+000002d0: 6e73 6163 7469 6f6e 0a20 2020 2020 2020  nsaction.       
+000002e0: 2020 2020 2064 6573 7469 6e61 7469 6f6e       destination
+000002f0: 3a20 3c61 7563 7469 6f6e 3e0a 2020 2020  : <auction>.    
+00000300: 2020 2020 2020 2020 656e 7472 7970 6f69          entrypoi
+00000310: 6e74 3a20 6269 640a 2020 2020 2020 2d20  nt: bid.      - 
+00000320: 6361 6c6c 6261 636b 3a20 6f6e 5f77 6974  callback: on_wit
+00000330: 6864 7261 770a 2020 2020 2020 2020 7061  hdraw.        pa
+00000340: 7474 6572 6e3a 0a20 2020 2020 2020 2020  ttern:.         
+00000350: 202d 2074 7970 653a 2074 7261 6e73 6163   - type: transac
+00000360: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+00000370: 2064 6573 7469 6e61 7469 6f6e 3a20 3c61   destination: <a
+00000380: 7563 7469 6f6e 3e0a 2020 2020 2020 2020  uction>.        
+00000390: 2020 2020 656e 7472 7970 6f69 6e74 3a20      entrypoint: 
+000003a0: 7769 7468 6472 6177 0a0a 696e 6465 7865  withdraw..indexe
+000003b0: 733a 0a20 2074 7a63 6f6c 6f72 733a 0a20  s:.  tzcolors:. 
+000003c0: 2020 2074 656d 706c 6174 653a 2061 7563     template: auc
+000003d0: 7469 6f6e 0a20 2020 2076 616c 7565 733a  tion.    values:
+000003e0: 0a20 2020 2020 2064 6174 6173 6f75 7263  .      datasourc
+000003f0: 653a 2074 7a6b 740a 2020 2020 2020 6d69  e: tzkt.      mi
+00000400: 6e74 6572 3a20 747a 636f 6c6f 7273 5f6d  nter: tzcolors_m
+00000410: 696e 7465 720a 2020 2020 2020 6175 6374  inter.      auct
+00000420: 696f 6e3a 2074 7a63 6f6c 6f72 735f 6175  ion: tzcolors_au
+00000430: 6374 696f 6e                             ction
```

### Comparing `dipdup-7.0.0rc1/src/demo_auction/handlers/on_bid.py` & `dipdup-7.0.0rc2/src/demo_auction/handlers/on_bid.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_auction/handlers/on_create_auction.py` & `dipdup-7.0.0rc2/src/demo_auction/handlers/on_create_auction.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_auction/handlers/on_withdraw.py` & `dipdup-7.0.0rc2/src/demo_auction/handlers/on_withdraw.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_auction/models/__init__.py` & `dipdup-7.0.0rc2/src/demo_auction/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_auction/pyproject.toml` & `dipdup-7.0.0rc2/src/demo_auction/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc1,<8"
+    "dipdup>=7.0.0rc2,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
@@ -26,16 +26,14 @@
 _ruff = "ruff check --fix ."
 _mypy = "mypy ."
 all = { composite = ["fmt", "lint"] }
 fmt = { composite = ["_isort", "_black"] }
 lint = { composite = ["_ruff", "_mypy"] }
 image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_auction:latest"
 
-clean = "git clean -xdf --exclude=.venv"
-
 [tool.isort]
 line_length = 120
 force_single_line = true
 
 [tool.black]
 line-length = 120
 target-version = ['py311']
```

### Comparing `dipdup-7.0.0rc1/src/demo_auction/types/tzcolors_auction/tezos_storage.py` & `dipdup-7.0.0rc2/src/demo_auction/types/tzcolors_auction/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_big_maps/README.md` & `dipdup-7.0.0rc2/src/demo_blank/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# demo_big_maps
+# demo_blank
 
-Indexing specific big maps
+Empty config for a fresh start
 
 ## Installation
 
 This project is based on [DipDup](https://dipdup.io), a framework for building featureful dapps.
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
 ```bash
 curl -Lsf https://dipdup.io/install.py | python3
 ```
 
-See the [Installation](https://docs.dipdup.io/installation) page for all options.
+See the [Installation](https://dipdup.io/docs/installation) page for all options.
 
 ## Usage
 
 Run the indexer in-memory:
 
 ```bash
 dipdup run
@@ -27,17 +27,17 @@
 ```bash
 dipdup -c . -c configs/dipdup.sqlite.yml run
 ```
 
 Or spawn a docker-compose stack:
 
 ```bash
-cp deploy/.env.example .env
+cp deploy/.env.default deploy/.env
 # Edit .env before running
-docker-compose -f deploy/docker-compose.yml up
+docker-compose -f deploy/compose.yaml up
 ```
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
```

### Comparing `dipdup-7.0.0rc1/src/demo_big_maps/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc2/src/demo_big_maps/deploy/compose.swarm.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     deploy:
       mode: replicated
       replicas: 1
       placement: *placement
     logging: *logging
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     depends_on:
       - db
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@demo_big_maps_db:5432/dipdup
       - HASURA_GRAPHQL_ADMIN_SECRET=${HASURA_SECRET}
       - HASURA_GRAPHQL_ENABLE_CONSOLE=true
       - HASURA_GRAPHQL_DEV_MODE=false
```

### Comparing `dipdup-7.0.0rc1/src/demo_big_maps/deploy/compose.yaml` & `dipdup-7.0.0rc2/src/demo_big_maps/deploy/compose.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     healthcheck:
       test: ["CMD-SHELL", "pg_isready -U dipdup"]
       interval: 10s
       timeout: 5s
       retries: 5
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     ports:
       - 8080
     depends_on:
       - db
     restart: always
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@db:5432/dipdup
```

### Comparing `dipdup-7.0.0rc1/src/demo_big_maps/dipdup.yaml` & `dipdup-7.0.0rc2/tests/configs/demo_big_maps.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
-00000020: 6269 675f 6d61 7073 0a0a 6461 7461 6261  big_maps..databa
-00000030: 7365 3a0a 2020 6b69 6e64 3a20 7371 6c69  se:.  kind: sqli
-00000040: 7465 0a20 2070 6174 683a 2064 656d 6f5f  te.  path: demo_
-00000050: 6269 675f 6d61 7073 2e73 716c 6974 6533  big_maps.sqlite3
-00000060: 0a0a 636f 6e74 7261 6374 733a 0a20 206d  ..contracts:.  m
-00000070: 6169 6e6e 6574 5f6e 616d 655f 7265 6769  ainnet_name_regi
-00000080: 7374 7279 3a0a 2020 2020 6b69 6e64 3a20  stry:.    kind: 
-00000090: 7465 7a6f 730a 2020 2020 6164 6472 6573  tezos.    addres
-000000a0: 733a 204b 5431 4742 5a6d 5378 6d6e 4b4a  s: KT1GBZmSxmnKJ
-000000b0: 5847 4d64 4d4c 6275 6750 664c 7955 506d  XGMdMLbugPfLyUPm
-000000c0: 754c 534d 774b 530a 2020 2020 7479 7065  uLSMwKS.    type
-000000d0: 6e61 6d65 3a20 6e61 6d65 5f72 6567 6973  name: name_regis
-000000e0: 7472 790a 0a64 6174 6173 6f75 7263 6573  try..datasources
-000000f0: 3a0a 2020 747a 6b74 5f6d 6169 6e6e 6574  :.  tzkt_mainnet
-00000100: 3a0a 2020 2020 6b69 6e64 3a20 7465 7a6f  :.    kind: tezo
-00000110: 732e 747a 6b74 0a20 2020 2075 726c 3a20  s.tzkt.    url: 
-00000120: 247b 545a 4b54 5f55 524c 3a2d 6874 7470  ${TZKT_URL:-http
-00000130: 733a 2f2f 6170 692e 747a 6b74 2e69 6f7d  s://api.tzkt.io}
-00000140: 0a0a 7465 6d70 6c61 7465 733a 0a20 2062  ..templates:.  b
-00000150: 6967 5f6d 6170 733a 0a20 2020 206b 696e  ig_maps:.    kin
-00000160: 643a 2074 657a 6f73 2e74 7a6b 742e 6269  d: tezos.tzkt.bi
-00000170: 675f 6d61 7073 0a20 2020 2064 6174 6173  g_maps.    datas
-00000180: 6f75 7263 653a 203c 6461 7461 736f 7572  ource: <datasour
-00000190: 6365 3e0a 2020 2020 736b 6970 5f68 6973  ce>.    skip_his
-000001a0: 746f 7279 3a20 6f6e 6365 0a20 2020 2068  tory: once.    h
-000001b0: 616e 646c 6572 733a 0a20 2020 2020 202d  andlers:.      -
-000001c0: 2063 616c 6c62 6163 6b3a 206f 6e5f 7570   callback: on_up
-000001d0: 6461 7465 5f72 6563 6f72 6473 0a20 2020  date_records.   
-000001e0: 2020 2020 2063 6f6e 7472 6163 743a 203c       contract: <
-000001f0: 6e61 6d65 5f72 6567 6973 7472 793e 0a20  name_registry>. 
-00000200: 2020 2020 2020 2070 6174 683a 2073 746f         path: sto
-00000210: 7265 2e72 6563 6f72 6473 0a20 2020 2020  re.records.     
-00000220: 202d 2063 616c 6c62 6163 6b3a 206f 6e5f   - callback: on_
-00000230: 7570 6461 7465 5f65 7870 6972 795f 6d61  update_expiry_ma
-00000240: 700a 2020 2020 2020 2020 636f 6e74 7261  p.        contra
-00000250: 6374 3a20 3c6e 616d 655f 7265 6769 7374  ct: <name_regist
-00000260: 7279 3e0a 2020 2020 2020 2020 7061 7468  ry>.        path
-00000270: 3a20 7374 6f72 652e 6578 7069 7279 5f6d  : store.expiry_m
-00000280: 6170 0a0a 696e 6465 7865 733a 0a20 2062  ap..indexes:.  b
-00000290: 6967 5f6d 6170 735f 6d61 696e 6e65 743a  ig_maps_mainnet:
-000002a0: 0a20 2020 2074 656d 706c 6174 653a 2062  .    template: b
-000002b0: 6967 5f6d 6170 730a 2020 2020 7661 6c75  ig_maps.    valu
-000002c0: 6573 3a0a 2020 2020 2020 6461 7461 736f  es:.      dataso
-000002d0: 7572 6365 3a20 747a 6b74 5f6d 6169 6e6e  urce: tzkt_mainn
-000002e0: 6574 0a20 2020 2020 206e 616d 655f 7265  et.      name_re
-000002f0: 6769 7374 7279 3a20 6d61 696e 6e65 745f  gistry: mainnet_
-00000300: 6e61 6d65 5f72 6567 6973 7472 79         name_registry
+00000020: 6269 675f 6d61 7073 0a0a 636f 6e74 7261  big_maps..contra
+00000030: 6374 733a 0a20 206e 616d 655f 7265 6769  cts:.  name_regi
+00000040: 7374 7279 3a0a 2020 2020 6b69 6e64 3a20  stry:.    kind: 
+00000050: 7465 7a6f 730a 2020 2020 6164 6472 6573  tezos.    addres
+00000060: 733a 204b 5431 4742 5a6d 5378 6d6e 4b4a  s: KT1GBZmSxmnKJ
+00000070: 5847 4d64 4d4c 6275 6750 664c 7955 506d  XGMdMLbugPfLyUPm
+00000080: 754c 534d 774b 530a 2020 2020 7479 7065  uLSMwKS.    type
+00000090: 6e61 6d65 3a20 6e61 6d65 5f72 6567 6973  name: name_regis
+000000a0: 7472 790a 0a64 6174 6173 6f75 7263 6573  try..datasources
+000000b0: 3a0a 2020 747a 6b74 3a0a 2020 2020 6b69  :.  tzkt:.    ki
+000000c0: 6e64 3a20 7465 7a6f 732e 747a 6b74 0a20  nd: tezos.tzkt. 
+000000d0: 2020 2075 726c 3a20 247b 545a 4b54 5f55     url: ${TZKT_U
+000000e0: 524c 3a2d 6874 7470 733a 2f2f 6170 692e  RL:-https://api.
+000000f0: 747a 6b74 2e69 6f7d 0a20 2020 2068 7474  tzkt.io}.    htt
+00000100: 703a 0a20 2020 2020 2072 6570 6c61 795f  p:.      replay_
+00000110: 7061 7468 3a20 247b 4449 5044 5550 5f52  path: ${DIPDUP_R
+00000120: 4550 4c41 595f 5041 5448 3a2d 7d0a 0a74  EPLAY_PATH:-}..t
+00000130: 656d 706c 6174 6573 3a0a 2020 6269 675f  emplates:.  big_
+00000140: 6d61 7073 3a0a 2020 2020 6b69 6e64 3a20  maps:.    kind: 
+00000150: 7465 7a6f 732e 747a 6b74 2e62 6967 5f6d  tezos.tzkt.big_m
+00000160: 6170 730a 2020 2020 6461 7461 736f 7572  aps.    datasour
+00000170: 6365 3a20 3c64 6174 6173 6f75 7263 653e  ce: <datasource>
+00000180: 0a20 2020 2068 616e 646c 6572 733a 0a20  .    handlers:. 
+00000190: 2020 2020 202d 2063 616c 6c62 6163 6b3a       - callback:
+000001a0: 206f 6e5f 7570 6461 7465 5f72 6563 6f72   on_update_recor
+000001b0: 6473 0a20 2020 2020 2020 2063 6f6e 7472  ds.        contr
+000001c0: 6163 743a 203c 6e61 6d65 5f72 6567 6973  act: <name_regis
+000001d0: 7472 793e 0a20 2020 2020 2020 2070 6174  try>.        pat
+000001e0: 683a 2073 746f 7265 2e72 6563 6f72 6473  h: store.records
+000001f0: 0a20 2020 2020 202d 2063 616c 6c62 6163  .      - callbac
+00000200: 6b3a 206f 6e5f 7570 6461 7465 5f65 7870  k: on_update_exp
+00000210: 6972 795f 6d61 700a 2020 2020 2020 2020  iry_map.        
+00000220: 636f 6e74 7261 6374 3a20 3c6e 616d 655f  contract: <name_
+00000230: 7265 6769 7374 7279 3e0a 2020 2020 2020  registry>.      
+00000240: 2020 7061 7468 3a20 7374 6f72 652e 6578    path: store.ex
+00000250: 7069 7279 5f6d 6170 0a0a 696e 6465 7865  piry_map..indexe
+00000260: 733a 0a20 2062 6967 5f6d 6170 733a 0a20  s:.  big_maps:. 
+00000270: 2020 2074 656d 706c 6174 653a 2062 6967     template: big
+00000280: 5f6d 6170 730a 2020 2020 6669 7273 745f  _maps.    first_
+00000290: 6c65 7665 6c3a 2031 3431 3538 3532 0a20  level: 1415852. 
+000002a0: 2020 206c 6173 745f 6c65 7665 6c3a 2031     last_level: 1
+000002b0: 3431 3838 3030 0a20 2020 2076 616c 7565  418800.    value
+000002c0: 733a 0a20 2020 2020 2064 6174 6173 6f75  s:.      datasou
+000002d0: 7263 653a 2074 7a6b 740a 2020 2020 2020  rce: tzkt.      
+000002e0: 6e61 6d65 5f72 6567 6973 7472 793a 206e  name_registry: n
+000002f0: 616d 655f 7265 6769 7374 7279 0a0a 6c6f  ame_registry..lo
+00000300: 6767 696e 673a 2057 4152 4e0a            gging: WARN.
```

### Comparing `dipdup-7.0.0rc1/src/demo_big_maps/handlers/on_update_expiry_map.py` & `dipdup-7.0.0rc2/src/demo_big_maps/handlers/on_update_expiry_map.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_big_maps/handlers/on_update_records.py` & `dipdup-7.0.0rc2/src/demo_big_maps/handlers/on_update_records.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_big_maps/models/__init__.py` & `dipdup-7.0.0rc2/src/demo_big_maps/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_big_maps/pyproject.toml` & `dipdup-7.0.0rc2/src/demo_big_maps/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc1,<8"
+    "dipdup>=7.0.0rc2,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
@@ -26,16 +26,14 @@
 _ruff = "ruff check --fix ."
 _mypy = "mypy ."
 all = { composite = ["fmt", "lint"] }
 fmt = { composite = ["_isort", "_black"] }
 lint = { composite = ["_ruff", "_mypy"] }
 image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_big_maps:latest"
 
-clean = "git clean -xdf --exclude=.venv"
-
 [tool.isort]
 line_length = 120
 force_single_line = true
 
 [tool.black]
 line-length = 120
 target-version = ['py311']
```

### Comparing `dipdup-7.0.0rc1/src/demo_blank/README.md` & `dipdup-7.0.0rc2/src/demo_token/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# demo_blank
+# demo_token
 
-Empty config for a fresh start
+TzBTC FA1.2 token operations
 
 ## Installation
 
 This project is based on [DipDup](https://dipdup.io), a framework for building featureful dapps.
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
 ```bash
 curl -Lsf https://dipdup.io/install.py | python3
 ```
 
-See the [Installation](https://docs.dipdup.io/installation) page for all options.
+See the [Installation](https://dipdup.io/docs/installation) page for all options.
 
 ## Usage
 
 Run the indexer in-memory:
 
 ```bash
 dipdup run
@@ -27,17 +27,17 @@
 ```bash
 dipdup -c . -c configs/dipdup.sqlite.yml run
 ```
 
 Or spawn a docker-compose stack:
 
 ```bash
-cp deploy/.env.example .env
+cp deploy/.env.default deploy/.env
 # Edit .env before running
-docker-compose -f deploy/docker-compose.yml up
+docker-compose -f deploy/compose.yaml up
 ```
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
```

### Comparing `dipdup-7.0.0rc1/src/demo_blank/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc2/src/demo_blank/deploy/compose.swarm.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     deploy:
       mode: replicated
       replicas: 1
       placement: *placement
     logging: *logging
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     depends_on:
       - db
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@demo_blank_db:5432/dipdup
       - HASURA_GRAPHQL_ADMIN_SECRET=${HASURA_SECRET}
       - HASURA_GRAPHQL_ENABLE_CONSOLE=true
       - HASURA_GRAPHQL_DEV_MODE=false
```

### Comparing `dipdup-7.0.0rc1/src/demo_blank/deploy/compose.yaml` & `dipdup-7.0.0rc2/src/demo_blank/deploy/compose.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     healthcheck:
       test: ["CMD-SHELL", "pg_isready -U dipdup"]
       interval: 10s
       timeout: 5s
       retries: 5
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     ports:
       - 8080
     depends_on:
       - db
     restart: always
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@db:5432/dipdup
```

### Comparing `dipdup-7.0.0rc1/src/demo_blank/models/__init__.py` & `dipdup-7.0.0rc2/src/demo_blank/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_blank/pyproject.toml` & `dipdup-7.0.0rc2/src/demo_evm_events/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
-name = "demo_blank"
+name = "demo_evm_events"
 version = "0.0.1"
-description = "Empty config for a fresh start"
+description = "A very basic indexer for USDt transfers"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc1,<8"
+    "dipdup>=7.0.0rc2,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
@@ -24,17 +24,15 @@
 _isort = "isort ."
 _black = "black ."
 _ruff = "ruff check --fix ."
 _mypy = "mypy ."
 all = { composite = ["fmt", "lint"] }
 fmt = { composite = ["_isort", "_black"] }
 lint = { composite = ["_ruff", "_mypy"] }
-image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_blank:latest"
-
-clean = "git clean -xdf --exclude=.venv"
+image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_evm_events:latest"
 
 [tool.isort]
 line_length = 120
 force_single_line = true
 
 [tool.black]
 line-length = 120
```

### Comparing `dipdup-7.0.0rc1/src/demo_dao/README.md` & `dipdup-7.0.0rc2/src/demo_dao/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
 ```bash
 curl -Lsf https://dipdup.io/install.py | python3
 ```
 
-See the [Installation](https://docs.dipdup.io/installation) page for all options.
+See the [Installation](https://dipdup.io/docs/installation) page for all options.
 
 ## Usage
 
 Run the indexer in-memory:
 
 ```bash
 dipdup run
@@ -27,17 +27,17 @@
 ```bash
 dipdup -c . -c configs/dipdup.sqlite.yml run
 ```
 
 Or spawn a docker-compose stack:
 
 ```bash
-cp deploy/.env.example .env
+cp deploy/.env.default deploy/.env
 # Edit .env before running
-docker-compose -f deploy/docker-compose.yml up
+docker-compose -f deploy/compose.yaml up
 ```
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
```

### Comparing `dipdup-7.0.0rc1/src/demo_dao/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc2/src/demo_dao/deploy/compose.swarm.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     deploy:
       mode: replicated
       replicas: 1
       placement: *placement
     logging: *logging
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     depends_on:
       - db
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@demo_dao_db:5432/dipdup
       - HASURA_GRAPHQL_ADMIN_SECRET=${HASURA_SECRET}
       - HASURA_GRAPHQL_ENABLE_CONSOLE=true
       - HASURA_GRAPHQL_DEV_MODE=false
```

### Comparing `dipdup-7.0.0rc1/src/demo_dao/deploy/compose.yaml` & `dipdup-7.0.0rc2/src/demo_dao/deploy/compose.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     healthcheck:
       test: ["CMD-SHELL", "pg_isready -U dipdup"]
       interval: 10s
       timeout: 5s
       retries: 5
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     ports:
       - 8080
     depends_on:
       - db
     restart: always
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@db:5432/dipdup
```

### Comparing `dipdup-7.0.0rc1/src/demo_dao/dipdup.yaml` & `dipdup-7.0.0rc2/src/demo_dao/dipdup.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
-00000020: 6461 6f0a 0a64 6174 6162 6173 653a 0a20  dao..database:. 
-00000030: 206b 696e 643a 2073 716c 6974 650a 2020   kind: sqlite.  
-00000040: 7061 7468 3a20 6465 6d6f 5f64 616f 2e73  path: demo_dao.s
-00000050: 716c 6974 6533 0a0a 636f 6e74 7261 6374  qlite3..contract
-00000060: 733a 0a20 2072 6567 6973 7472 793a 0a20  s:.  registry:. 
-00000070: 2020 206b 696e 643a 2074 657a 6f73 0a20     kind: tezos. 
-00000080: 2020 2063 6f64 655f 6861 7368 3a20 4b54     code_hash: KT
-00000090: 3139 4346 334b 4b72 7664 5737 3774 7446  19CF3KKrvdW77ttF
-000000a0: 6f6d 4375 696e 326b 3475 4156 6b72 7959  omCuin2k4uAVkryY
-000000b0: 7168 0a20 2020 2074 7970 656e 616d 653a  qh.    typename:
-000000c0: 2072 6567 6973 7472 790a 0a64 6174 6173   registry..datas
-000000d0: 6f75 7263 6573 3a0a 2020 747a 6b74 3a0a  ources:.  tzkt:.
-000000e0: 2020 2020 6b69 6e64 3a20 7465 7a6f 732e      kind: tezos.
-000000f0: 747a 6b74 0a20 2020 2075 726c 3a20 247b  tzkt.    url: ${
-00000100: 545a 4b54 5f55 524c 3a2d 6874 7470 733a  TZKT_URL:-https:
-00000110: 2f2f 6170 692e 747a 6b74 2e69 6f7d 0a0a  //api.tzkt.io}..
-00000120: 696e 6465 7865 733a 0a20 2072 6567 6973  indexes:.  regis
-00000130: 7472 795f 6461 6f3a 0a20 2020 206b 696e  try_dao:.    kin
-00000140: 643a 2074 657a 6f73 2e74 7a6b 742e 6f70  d: tezos.tzkt.op
-00000150: 6572 6174 696f 6e73 0a20 2020 2064 6174  erations.    dat
-00000160: 6173 6f75 7263 653a 2074 7a6b 740a 2020  asource: tzkt.  
-00000170: 2020 7479 7065 733a 0a20 2020 2020 202d    types:.      -
-00000180: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
-00000190: 2020 202d 206f 7269 6769 6e61 7469 6f6e     - origination
-000001a0: 0a20 2020 2068 616e 646c 6572 733a 0a20  .    handlers:. 
-000001b0: 2020 2020 202d 2063 616c 6c62 6163 6b3a       - callback:
-000001c0: 206f 6e5f 6f72 6967 696e 6174 696f 6e0a   on_origination.
-000001d0: 2020 2020 2020 2020 7061 7474 6572 6e3a          pattern:
-000001e0: 0a20 2020 2020 2020 2020 202d 2074 7970  .          - typ
-000001f0: 653a 206f 7269 6769 6e61 7469 6f6e 0a20  e: origination. 
-00000200: 2020 2020 2020 2020 2020 206f 7269 6769             origi
-00000210: 6e61 7465 645f 636f 6e74 7261 6374 3a20  nated_contract: 
-00000220: 7265 6769 7374 7279 0a20 2020 2020 202d  registry.      -
-00000230: 2063 616c 6c62 6163 6b3a 206f 6e5f 7072   callback: on_pr
-00000240: 6f70 6f73 650a 2020 2020 2020 2020 7061  opose.        pa
-00000250: 7474 6572 6e3a 0a20 2020 2020 2020 2020  ttern:.         
-00000260: 202d 2074 7970 653a 2074 7261 6e73 6163   - type: transac
-00000270: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-00000280: 2064 6573 7469 6e61 7469 6f6e 3a20 7265   destination: re
-00000290: 6769 7374 7279 0a20 2020 2020 2020 2020  gistry.         
-000002a0: 2020 2065 6e74 7279 706f 696e 743a 2070     entrypoint: p
-000002b0: 726f 706f 7365                           ropose
+00000020: 6461 6f0a 0a63 6f6e 7472 6163 7473 3a0a  dao..contracts:.
+00000030: 2020 7265 6769 7374 7279 3a0a 2020 2020    registry:.    
+00000040: 6b69 6e64 3a20 7465 7a6f 730a 2020 2020  kind: tezos.    
+00000050: 636f 6465 5f68 6173 683a 204b 5431 3943  code_hash: KT19C
+00000060: 4633 4b4b 7276 6457 3737 7474 466f 6d43  F3KKrvdW77ttFomC
+00000070: 7569 6e32 6b34 7541 566b 7279 5971 680a  uin2k4uAVkryYqh.
+00000080: 2020 2020 7479 7065 6e61 6d65 3a20 7265      typename: re
+00000090: 6769 7374 7279 0a0a 6461 7461 736f 7572  gistry..datasour
+000000a0: 6365 733a 0a20 2074 7a6b 743a 0a20 2020  ces:.  tzkt:.   
+000000b0: 206b 696e 643a 2074 657a 6f73 2e74 7a6b   kind: tezos.tzk
+000000c0: 740a 2020 2020 7572 6c3a 2024 7b54 5a4b  t.    url: ${TZK
+000000d0: 545f 5552 4c3a 2d68 7474 7073 3a2f 2f61  T_URL:-https://a
+000000e0: 7069 2e74 7a6b 742e 696f 7d0a 0a69 6e64  pi.tzkt.io}..ind
+000000f0: 6578 6573 3a0a 2020 7265 6769 7374 7279  exes:.  registry
+00000100: 5f64 616f 3a0a 2020 2020 6b69 6e64 3a20  _dao:.    kind: 
+00000110: 7465 7a6f 732e 747a 6b74 2e6f 7065 7261  tezos.tzkt.opera
+00000120: 7469 6f6e 730a 2020 2020 6461 7461 736f  tions.    dataso
+00000130: 7572 6365 3a20 747a 6b74 0a20 2020 2074  urce: tzkt.    t
+00000140: 7970 6573 3a0a 2020 2020 2020 2d20 7472  ypes:.      - tr
+00000150: 616e 7361 6374 696f 6e0a 2020 2020 2020  ansaction.      
+00000160: 2d20 6f72 6967 696e 6174 696f 6e0a 2020  - origination.  
+00000170: 2020 6861 6e64 6c65 7273 3a0a 2020 2020    handlers:.    
+00000180: 2020 2d20 6361 6c6c 6261 636b 3a20 6f6e    - callback: on
+00000190: 5f6f 7269 6769 6e61 7469 6f6e 0a20 2020  _origination.   
+000001a0: 2020 2020 2070 6174 7465 726e 3a0a 2020       pattern:.  
+000001b0: 2020 2020 2020 2020 2d20 7479 7065 3a20          - type: 
+000001c0: 6f72 6967 696e 6174 696f 6e0a 2020 2020  origination.    
+000001d0: 2020 2020 2020 2020 6f72 6967 696e 6174          originat
+000001e0: 6564 5f63 6f6e 7472 6163 743a 2072 6567  ed_contract: reg
+000001f0: 6973 7472 790a 2020 2020 2020 2d20 6361  istry.      - ca
+00000200: 6c6c 6261 636b 3a20 6f6e 5f70 726f 706f  llback: on_propo
+00000210: 7365 0a20 2020 2020 2020 2070 6174 7465  se.        patte
+00000220: 726e 3a0a 2020 2020 2020 2020 2020 2d20  rn:.          - 
+00000230: 7479 7065 3a20 7472 616e 7361 6374 696f  type: transactio
+00000240: 6e0a 2020 2020 2020 2020 2020 2020 6465  n.            de
+00000250: 7374 696e 6174 696f 6e3a 2072 6567 6973  stination: regis
+00000260: 7472 790a 2020 2020 2020 2020 2020 2020  try.            
+00000270: 656e 7472 7970 6f69 6e74 3a20 7072 6f70  entrypoint: prop
+00000280: 6f73 65                                  ose
```

### Comparing `dipdup-7.0.0rc1/src/demo_dao/models/__init__.py` & `dipdup-7.0.0rc2/src/demo_dao/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_dao/pyproject.toml` & `dipdup-7.0.0rc2/src/demo_dao/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc1,<8"
+    "dipdup>=7.0.0rc2,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
@@ -26,16 +26,14 @@
 _ruff = "ruff check --fix ."
 _mypy = "mypy ."
 all = { composite = ["fmt", "lint"] }
 fmt = { composite = ["_isort", "_black"] }
 lint = { composite = ["_ruff", "_mypy"] }
 image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_dao:latest"
 
-clean = "git clean -xdf --exclude=.venv"
-
 [tool.isort]
 line_length = 120
 force_single_line = true
 
 [tool.black]
 line-length = 120
 target-version = ['py311']
```

### Comparing `dipdup-7.0.0rc1/src/demo_dao/types/registry/tezos_storage.py` & `dipdup-7.0.0rc2/src/demo_dao/types/registry/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_dex/README.md` & `dipdup-7.0.0rc2/src/demo_dex/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
 ```bash
 curl -Lsf https://dipdup.io/install.py | python3
 ```
 
-See the [Installation](https://docs.dipdup.io/installation) page for all options.
+See the [Installation](https://dipdup.io/docs/installation) page for all options.
 
 ## Usage
 
 Run the indexer in-memory:
 
 ```bash
 dipdup run
@@ -27,17 +27,17 @@
 ```bash
 dipdup -c . -c configs/dipdup.sqlite.yml run
 ```
 
 Or spawn a docker-compose stack:
 
 ```bash
-cp deploy/.env.example .env
+cp deploy/.env.default deploy/.env
 # Edit .env before running
-docker-compose -f deploy/docker-compose.yml up
+docker-compose -f deploy/compose.yaml up
 ```
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
```

### Comparing `dipdup-7.0.0rc1/src/demo_dex/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc2/src/demo_dex/deploy/compose.swarm.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     deploy:
       mode: replicated
       replicas: 1
       placement: *placement
     logging: *logging
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     depends_on:
       - db
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@demo_dex_db:5432/dipdup
       - HASURA_GRAPHQL_ADMIN_SECRET=${HASURA_SECRET}
       - HASURA_GRAPHQL_ENABLE_CONSOLE=true
       - HASURA_GRAPHQL_DEV_MODE=false
```

### Comparing `dipdup-7.0.0rc1/src/demo_dex/deploy/compose.yaml` & `dipdup-7.0.0rc2/src/demo_uniswap/deploy/compose.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: demo_dex
+name: demo_uniswap
 
 services:
   dipdup:
     build:
       context: ..
       dockerfile: deploy/Dockerfile
     restart: always
@@ -30,15 +30,15 @@
     healthcheck:
       test: ["CMD-SHELL", "pg_isready -U dipdup"]
       interval: 10s
       timeout: 5s
       retries: 5
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     ports:
       - 8080
     depends_on:
       - db
     restart: always
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@db:5432/dipdup
```

### Comparing `dipdup-7.0.0rc1/src/demo_dex/dipdup.yaml` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/dipdup.yaml.j2`

 * *Files 2% similar despite different names*

```diff
@@ -1,306 +1,304 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
-00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
-00000020: 6465 780a 0a64 6174 6162 6173 653a 0a20  dex..database:. 
-00000030: 206b 696e 643a 2073 716c 6974 650a 2020   kind: sqlite.  
-00000040: 7061 7468 3a20 6465 6d6f 5f64 6578 2e73  path: demo_dex.s
-00000050: 716c 6974 6533 0a0a 636f 6e74 7261 6374  qlite3..contract
-00000060: 733a 0a20 206b 7573 645f 6465 785f 6d61  s:.  kusd_dex_ma
-00000070: 696e 6e65 743a 0a20 2020 206b 696e 643a  innet:.    kind:
-00000080: 2074 657a 6f73 0a20 2020 2061 6464 7265   tezos.    addre
-00000090: 7373 3a20 4b54 314b 3445 7754 7062 7659  ss: KT1K4EwTpbvY
-000000a0: 4e39 6167 4a64 6a70 794a 6d34 5a5a 6468  N9agJdjpyJm4ZZdh
-000000b0: 7055 4e4b 4233 4636 0a20 2020 2074 7970  pUNKB3F6.    typ
-000000c0: 656e 616d 653a 2071 7569 7075 5f66 6131  ename: quipu_fa1
-000000d0: 320a 2020 6b75 7364 5f74 6f6b 656e 5f6d  2.  kusd_token_m
-000000e0: 6169 6e6e 6574 3a0a 2020 2020 6b69 6e64  ainnet:.    kind
-000000f0: 3a20 7465 7a6f 730a 2020 2020 6164 6472  : tezos.    addr
-00000100: 6573 733a 204b 5431 4b39 6743 5267 614c  ess: KT1K9gCRgaL
-00000110: 5246 4b54 4572 5974 3177 5678 4133 4672  RFKTErYt1wVxA3Fr
-00000120: 6239 466a 6173 6a54 560a 2020 2020 7479  b9FjasjTV.    ty
-00000130: 7065 6e61 6d65 3a20 6661 3132 5f74 6f6b  pename: fa12_tok
-00000140: 656e 0a20 2068 6461 6f5f 6465 785f 6d61  en.  hdao_dex_ma
-00000150: 696e 6e65 743a 0a20 2020 206b 696e 643a  innet:.    kind:
-00000160: 2074 657a 6f73 0a20 2020 2061 6464 7265   tezos.    addre
-00000170: 7373 3a20 4b54 3151 784c 7175 6b79 666f  ss: KT1QxLqukyfo
-00000180: 6850 5635 6b50 6b77 3937 5273 3663 7731  hPV5kPkw97Rs6cw1
-00000190: 4444 4476 5967 6242 0a20 2020 2074 7970  DDDvYgbB.    typ
-000001a0: 656e 616d 653a 2071 7569 7075 5f66 6132  ename: quipu_fa2
-000001b0: 0a20 2068 6461 6f5f 746f 6b65 6e5f 6d61  .  hdao_token_ma
-000001c0: 696e 6e65 743a 0a20 2020 206b 696e 643a  innet:.    kind:
-000001d0: 2074 657a 6f73 0a20 2020 2061 6464 7265   tezos.    addre
-000001e0: 7373 3a20 4b54 3141 4641 326d 774e 554d  ss: KT1AFA2mwNUM
-000001f0: 4e64 3453 7375 6a45 3159 5970 3239 7664  Nd4SsujE1YYp29vd
-00000200: 3842 5a65 6a79 4b57 0a20 2020 2074 7970  8BZejyKW.    typ
-00000210: 656e 616d 653a 2066 6132 5f74 6f6b 656e  ename: fa2_token
-00000220: 0a0a 6461 7461 736f 7572 6365 733a 0a20  ..datasources:. 
-00000230: 2074 7a6b 745f 6d61 696e 6e65 743a 0a20   tzkt_mainnet:. 
-00000240: 2020 206b 696e 643a 2074 657a 6f73 2e74     kind: tezos.t
-00000250: 7a6b 740a 2020 2020 7572 6c3a 2068 7474  zkt.    url: htt
-00000260: 7073 3a2f 2f61 7069 2e74 7a6b 742e 696f  ps://api.tzkt.io
-00000270: 0a0a 7465 6d70 6c61 7465 733a 0a20 2071  ..templates:.  q
-00000280: 7569 7075 7377 6170 5f66 6131 323a 0a20  uipuswap_fa12:. 
-00000290: 2020 206b 696e 643a 2074 657a 6f73 2e74     kind: tezos.t
-000002a0: 7a6b 742e 6f70 6572 6174 696f 6e73 0a20  zkt.operations. 
-000002b0: 2020 2064 6174 6173 6f75 7263 653a 2074     datasource: t
-000002c0: 7a6b 745f 6d61 696e 6e65 740a 2020 2020  zkt_mainnet.    
-000002d0: 636f 6e74 7261 6374 733a 0a20 2020 2020  contracts:.     
-000002e0: 202d 203c 6465 785f 636f 6e74 7261 6374   - <dex_contract
-000002f0: 3e0a 2020 2020 7479 7065 733a 0a20 2020  >.    types:.   
-00000300: 2020 202d 2074 7261 6e73 6163 7469 6f6e     - transaction
-00000310: 0a20 2020 2020 202d 206f 7269 6769 6e61  .      - origina
-00000320: 7469 6f6e 0a20 2020 2068 616e 646c 6572  tion.    handler
-00000330: 733a 0a20 2020 2020 202d 2063 616c 6c62  s:.      - callb
-00000340: 6163 6b3a 206f 6e5f 6661 3132 5f6f 7269  ack: on_fa12_ori
-00000350: 6769 6e61 7469 6f6e 0a20 2020 2020 2020  gination.       
-00000360: 2070 6174 7465 726e 3a0a 2020 2020 2020   pattern:.      
-00000370: 2020 2020 2d20 7479 7065 3a20 6f72 6967      - type: orig
-00000380: 696e 6174 696f 6e0a 2020 2020 2020 2020  ination.        
-00000390: 2020 2020 6f72 6967 696e 6174 6564 5f63      originated_c
-000003a0: 6f6e 7472 6163 743a 203c 6465 785f 636f  ontract: <dex_co
-000003b0: 6e74 7261 6374 3e0a 2020 2020 2020 2d20  ntract>.      - 
-000003c0: 6361 6c6c 6261 636b 3a20 6f6e 5f66 6131  callback: on_fa1
-000003d0: 325f 746f 6b65 6e5f 746f 5f74 657a 0a20  2_token_to_tez. 
-000003e0: 2020 2020 2020 2070 6174 7465 726e 3a0a         pattern:.
-000003f0: 2020 2020 2020 2020 2020 2d20 7479 7065            - type
-00000400: 3a20 7472 616e 7361 6374 696f 6e0a 2020  : transaction.  
-00000410: 2020 2020 2020 2020 2020 6465 7374 696e            destin
-00000420: 6174 696f 6e3a 203c 6465 785f 636f 6e74  ation: <dex_cont
-00000430: 7261 6374 3e0a 2020 2020 2020 2020 2020  ract>.          
-00000440: 2020 656e 7472 7970 6f69 6e74 3a20 746f    entrypoint: to
-00000450: 6b65 6e54 6f54 657a 5061 796d 656e 740a  kenToTezPayment.
-00000460: 2020 2020 2020 2020 2020 2d20 7479 7065            - type
-00000470: 3a20 7472 616e 7361 6374 696f 6e0a 2020  : transaction.  
-00000480: 2020 2020 2020 2020 2020 6465 7374 696e            destin
-00000490: 6174 696f 6e3a 203c 746f 6b65 6e5f 636f  ation: <token_co
-000004a0: 6e74 7261 6374 3e0a 2020 2020 2020 2020  ntract>.        
-000004b0: 2020 2020 656e 7472 7970 6f69 6e74 3a20      entrypoint: 
-000004c0: 7472 616e 7366 6572 0a20 2020 2020 2020  transfer.       
-000004d0: 2020 202d 2074 7970 653a 2074 7261 6e73     - type: trans
-000004e0: 6163 7469 6f6e 0a20 2020 2020 2020 2020  action.         
-000004f0: 2020 2073 6f75 7263 653a 203c 6465 785f     source: <dex_
-00000500: 636f 6e74 7261 6374 3e0a 2020 2020 2020  contract>.      
-00000510: 2d20 6361 6c6c 6261 636b 3a20 6f6e 5f66  - callback: on_f
-00000520: 6131 325f 7465 7a5f 746f 5f74 6f6b 656e  a12_tez_to_token
-00000530: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
-00000540: 3a0a 2020 2020 2020 2020 2020 2d20 7479  :.          - ty
-00000550: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
-00000560: 2020 2020 2020 2020 2020 2020 6465 7374              dest
-00000570: 696e 6174 696f 6e3a 203c 6465 785f 636f  ination: <dex_co
-00000580: 6e74 7261 6374 3e0a 2020 2020 2020 2020  ntract>.        
-00000590: 2020 2020 656e 7472 7970 6f69 6e74 3a20      entrypoint: 
-000005a0: 7465 7a54 6f54 6f6b 656e 5061 796d 656e  tezToTokenPaymen
-000005b0: 740a 2020 2020 2020 2020 2020 2d20 7479  t.          - ty
-000005c0: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
-000005d0: 2020 2020 2020 2020 2020 2020 6465 7374              dest
-000005e0: 696e 6174 696f 6e3a 203c 746f 6b65 6e5f  ination: <token_
-000005f0: 636f 6e74 7261 6374 3e0a 2020 2020 2020  contract>.      
-00000600: 2020 2020 2020 656e 7472 7970 6f69 6e74        entrypoint
-00000610: 3a20 7472 616e 7366 6572 0a20 2020 2020  : transfer.     
-00000620: 202d 2063 616c 6c62 6163 6b3a 206f 6e5f   - callback: on_
-00000630: 6661 3132 5f69 6e76 6573 745f 6c69 7175  fa12_invest_liqu
-00000640: 6964 6974 790a 2020 2020 2020 2020 7061  idity.        pa
-00000650: 7474 6572 6e3a 0a20 2020 2020 2020 2020  ttern:.         
-00000660: 202d 2074 7970 653a 2074 7261 6e73 6163   - type: transac
-00000670: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-00000680: 2064 6573 7469 6e61 7469 6f6e 3a20 3c64   destination: <d
-00000690: 6578 5f63 6f6e 7472 6163 743e 0a20 2020  ex_contract>.   
-000006a0: 2020 2020 2020 2020 2065 6e74 7279 706f           entrypo
-000006b0: 696e 743a 2069 6e76 6573 744c 6971 7569  int: investLiqui
-000006c0: 6469 7479 0a20 2020 2020 2020 2020 202d  dity.          -
-000006d0: 2074 7970 653a 2074 7261 6e73 6163 7469   type: transacti
-000006e0: 6f6e 0a20 2020 2020 2020 2020 2020 2064  on.            d
-000006f0: 6573 7469 6e61 7469 6f6e 3a20 3c74 6f6b  estination: <tok
-00000700: 656e 5f63 6f6e 7472 6163 743e 0a20 2020  en_contract>.   
-00000710: 2020 2020 2020 2020 2065 6e74 7279 706f           entrypo
-00000720: 696e 743a 2074 7261 6e73 6665 720a 2020  int: transfer.  
-00000730: 2020 2020 2d20 6361 6c6c 6261 636b 3a20      - callback: 
-00000740: 6f6e 5f66 6131 325f 7472 616e 7366 6572  on_fa12_transfer
-00000750: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
-00000760: 3a0a 2020 2020 2020 2020 2020 2d20 7479  :.          - ty
-00000770: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
-00000780: 2020 2020 2020 2020 2020 2020 6465 7374              dest
-00000790: 696e 6174 696f 6e3a 203c 6465 785f 636f  ination: <dex_co
-000007a0: 6e74 7261 6374 3e0a 2020 2020 2020 2020  ntract>.        
-000007b0: 2020 2020 656e 7472 7970 6f69 6e74 3a20      entrypoint: 
-000007c0: 7472 616e 7366 6572 0a20 2020 2020 202d  transfer.      -
-000007d0: 2063 616c 6c62 6163 6b3a 206f 6e5f 6661   callback: on_fa
-000007e0: 3132 5f64 6976 6573 745f 6c69 7175 6964  12_divest_liquid
-000007f0: 6974 790a 2020 2020 2020 2020 7061 7474  ity.        patt
-00000800: 6572 6e3a 0a20 2020 2020 2020 2020 202d  ern:.          -
-00000810: 2074 7970 653a 2074 7261 6e73 6163 7469   type: transacti
-00000820: 6f6e 0a20 2020 2020 2020 2020 2020 2064  on.            d
-00000830: 6573 7469 6e61 7469 6f6e 3a20 3c64 6578  estination: <dex
-00000840: 5f63 6f6e 7472 6163 743e 0a20 2020 2020  _contract>.     
-00000850: 2020 2020 2020 2065 6e74 7279 706f 696e         entrypoin
-00000860: 743a 2064 6976 6573 744c 6971 7569 6469  t: divestLiquidi
-00000870: 7479 0a20 2020 2020 2020 2020 202d 2074  ty.          - t
-00000880: 7970 653a 2074 7261 6e73 6163 7469 6f6e  ype: transaction
-00000890: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-000008a0: 7469 6e61 7469 6f6e 3a20 3c74 6f6b 656e  tination: <token
-000008b0: 5f63 6f6e 7472 6163 743e 0a20 2020 2020  _contract>.     
-000008c0: 2020 2020 2020 2065 6e74 7279 706f 696e         entrypoin
-000008d0: 743a 2074 7261 6e73 6665 720a 2020 2020  t: transfer.    
-000008e0: 2020 2020 2020 2d20 7479 7065 3a20 7472        - type: tr
-000008f0: 616e 7361 6374 696f 6e0a 2020 2020 2020  ansaction.      
-00000900: 2020 2020 2020 736f 7572 6365 3a20 3c64        source: <d
-00000910: 6578 5f63 6f6e 7472 6163 743e 0a20 2020  ex_contract>.   
-00000920: 2020 202d 2063 616c 6c62 6163 6b3a 206f     - callback: o
-00000930: 6e5f 6661 3132 5f77 6974 6864 7261 775f  n_fa12_withdraw_
-00000940: 7072 6f66 6974 0a20 2020 2020 2020 2070  profit.        p
-00000950: 6174 7465 726e 3a0a 2020 2020 2020 2020  attern:.        
-00000960: 2020 2d20 7479 7065 3a20 7472 616e 7361    - type: transa
-00000970: 6374 696f 6e0a 2020 2020 2020 2020 2020  ction.          
-00000980: 2020 6465 7374 696e 6174 696f 6e3a 203c    destination: <
-00000990: 6465 785f 636f 6e74 7261 6374 3e0a 2020  dex_contract>.  
-000009a0: 2020 2020 2020 2020 2020 656e 7472 7970            entryp
-000009b0: 6f69 6e74 3a20 7769 7468 6472 6177 5072  oint: withdrawPr
-000009c0: 6f66 6974 0a20 2020 2020 2020 2020 202d  ofit.          -
-000009d0: 2074 7970 653a 2074 7261 6e73 6163 7469   type: transacti
-000009e0: 6f6e 0a20 2020 2020 2020 2020 2020 2073  on.            s
-000009f0: 6f75 7263 653a 203c 6465 785f 636f 6e74  ource: <dex_cont
-00000a00: 7261 6374 3e0a 2020 2020 2020 2020 2020  ract>.          
-00000a10: 2020 6f70 7469 6f6e 616c 3a20 5472 7565    optional: True
-00000a20: 0a0a 2020 7175 6970 7573 7761 705f 6661  ..  quipuswap_fa
-00000a30: 323a 0a20 2020 206b 696e 643a 2074 657a  2:.    kind: tez
-00000a40: 6f73 2e74 7a6b 742e 6f70 6572 6174 696f  os.tzkt.operatio
-00000a50: 6e73 0a20 2020 2064 6174 6173 6f75 7263  ns.    datasourc
-00000a60: 653a 2074 7a6b 745f 6d61 696e 6e65 740a  e: tzkt_mainnet.
-00000a70: 2020 2020 636f 6e74 7261 6374 733a 0a20      contracts:. 
-00000a80: 2020 2020 202d 203c 6465 785f 636f 6e74       - <dex_cont
-00000a90: 7261 6374 3e0a 2020 2020 7479 7065 733a  ract>.    types:
-00000aa0: 0a20 2020 2020 202d 2074 7261 6e73 6163  .      - transac
-00000ab0: 7469 6f6e 0a20 2020 2020 202d 206f 7269  tion.      - ori
-00000ac0: 6769 6e61 7469 6f6e 0a20 2020 2068 616e  gination.    han
-00000ad0: 646c 6572 733a 0a20 2020 2020 202d 2063  dlers:.      - c
-00000ae0: 616c 6c62 6163 6b3a 206f 6e5f 6661 325f  allback: on_fa2_
-00000af0: 6f72 6967 696e 6174 696f 6e0a 2020 2020  origination.    
-00000b00: 2020 2020 7061 7474 6572 6e3a 0a20 2020      pattern:.   
-00000b10: 2020 2020 2020 202d 2074 7970 653a 206f         - type: o
-00000b20: 7269 6769 6e61 7469 6f6e 0a20 2020 2020  rigination.     
-00000b30: 2020 2020 2020 206f 7269 6769 6e61 7465         originate
-00000b40: 645f 636f 6e74 7261 6374 3a20 3c64 6578  d_contract: <dex
-00000b50: 5f63 6f6e 7472 6163 743e 0a20 2020 2020  _contract>.     
-00000b60: 202d 2063 616c 6c62 6163 6b3a 206f 6e5f   - callback: on_
-00000b70: 6661 325f 746f 6b65 6e5f 746f 5f74 657a  fa2_token_to_tez
-00000b80: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
-00000b90: 3a0a 2020 2020 2020 2020 2020 2d20 7479  :.          - ty
-00000ba0: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
-00000bb0: 2020 2020 2020 2020 2020 2020 6465 7374              dest
-00000bc0: 696e 6174 696f 6e3a 203c 6465 785f 636f  ination: <dex_co
-00000bd0: 6e74 7261 6374 3e0a 2020 2020 2020 2020  ntract>.        
-00000be0: 2020 2020 656e 7472 7970 6f69 6e74 3a20      entrypoint: 
-00000bf0: 746f 6b65 6e54 6f54 657a 5061 796d 656e  tokenToTezPaymen
-00000c00: 740a 2020 2020 2020 2020 2020 2d20 7479  t.          - ty
-00000c10: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
-00000c20: 2020 2020 2020 2020 2020 2020 6465 7374              dest
-00000c30: 696e 6174 696f 6e3a 203c 746f 6b65 6e5f  ination: <token_
-00000c40: 636f 6e74 7261 6374 3e0a 2020 2020 2020  contract>.      
-00000c50: 2020 2020 2020 656e 7472 7970 6f69 6e74        entrypoint
-00000c60: 3a20 7472 616e 7366 6572 0a20 2020 2020  : transfer.     
-00000c70: 2020 2020 202d 2074 7970 653a 2074 7261       - type: tra
-00000c80: 6e73 6163 7469 6f6e 0a20 2020 2020 2020  nsaction.       
-00000c90: 2020 2020 2073 6f75 7263 653a 203c 6465       source: <de
-00000ca0: 785f 636f 6e74 7261 6374 3e0a 2020 2020  x_contract>.    
-00000cb0: 2020 2d20 6361 6c6c 6261 636b 3a20 6f6e    - callback: on
-00000cc0: 5f66 6132 5f74 657a 5f74 6f5f 746f 6b65  _fa2_tez_to_toke
-00000cd0: 6e0a 2020 2020 2020 2020 7061 7474 6572  n.        patter
-00000ce0: 6e3a 0a20 2020 2020 2020 2020 202d 2074  n:.          - t
-00000cf0: 7970 653a 2074 7261 6e73 6163 7469 6f6e  ype: transaction
-00000d00: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-00000d10: 7469 6e61 7469 6f6e 3a20 3c64 6578 5f63  tination: <dex_c
-00000d20: 6f6e 7472 6163 743e 0a20 2020 2020 2020  ontract>.       
-00000d30: 2020 2020 2065 6e74 7279 706f 696e 743a       entrypoint:
-00000d40: 2074 657a 546f 546f 6b65 6e50 6179 6d65   tezToTokenPayme
-00000d50: 6e74 0a20 2020 2020 2020 2020 202d 2074  nt.          - t
-00000d60: 7970 653a 2074 7261 6e73 6163 7469 6f6e  ype: transaction
-00000d70: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-00000d80: 7469 6e61 7469 6f6e 3a20 3c74 6f6b 656e  tination: <token
-00000d90: 5f63 6f6e 7472 6163 743e 0a20 2020 2020  _contract>.     
-00000da0: 2020 2020 2020 2065 6e74 7279 706f 696e         entrypoin
-00000db0: 743a 2074 7261 6e73 6665 720a 2020 2020  t: transfer.    
-00000dc0: 2020 2d20 6361 6c6c 6261 636b 3a20 6f6e    - callback: on
-00000dd0: 5f66 6132 5f69 6e76 6573 745f 6c69 7175  _fa2_invest_liqu
-00000de0: 6964 6974 790a 2020 2020 2020 2020 7061  idity.        pa
-00000df0: 7474 6572 6e3a 0a20 2020 2020 2020 2020  ttern:.         
-00000e00: 202d 2074 7970 653a 2074 7261 6e73 6163   - type: transac
-00000e10: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-00000e20: 2064 6573 7469 6e61 7469 6f6e 3a20 3c64   destination: <d
-00000e30: 6578 5f63 6f6e 7472 6163 743e 0a20 2020  ex_contract>.   
-00000e40: 2020 2020 2020 2020 2065 6e74 7279 706f           entrypo
-00000e50: 696e 743a 2069 6e76 6573 744c 6971 7569  int: investLiqui
-00000e60: 6469 7479 0a20 2020 2020 2020 2020 202d  dity.          -
-00000e70: 2074 7970 653a 2074 7261 6e73 6163 7469   type: transacti
-00000e80: 6f6e 0a20 2020 2020 2020 2020 2020 2064  on.            d
-00000e90: 6573 7469 6e61 7469 6f6e 3a20 3c74 6f6b  estination: <tok
-00000ea0: 656e 5f63 6f6e 7472 6163 743e 0a20 2020  en_contract>.   
-00000eb0: 2020 2020 2020 2020 2065 6e74 7279 706f           entrypo
-00000ec0: 696e 743a 2074 7261 6e73 6665 720a 2020  int: transfer.  
-00000ed0: 2020 2020 2d20 6361 6c6c 6261 636b 3a20      - callback: 
-00000ee0: 6f6e 5f66 6132 5f74 7261 6e73 6665 720a  on_fa2_transfer.
-00000ef0: 2020 2020 2020 2020 7061 7474 6572 6e3a          pattern:
-00000f00: 0a20 2020 2020 2020 2020 202d 2074 7970  .          - typ
-00000f10: 653a 2074 7261 6e73 6163 7469 6f6e 0a20  e: transaction. 
-00000f20: 2020 2020 2020 2020 2020 2064 6573 7469             desti
-00000f30: 6e61 7469 6f6e 3a20 3c64 6578 5f63 6f6e  nation: <dex_con
-00000f40: 7472 6163 743e 0a20 2020 2020 2020 2020  tract>.         
-00000f50: 2020 2065 6e74 7279 706f 696e 743a 2074     entrypoint: t
-00000f60: 7261 6e73 6665 720a 2020 2020 2020 2d20  ransfer.      - 
-00000f70: 6361 6c6c 6261 636b 3a20 6f6e 5f66 6132  callback: on_fa2
-00000f80: 5f64 6976 6573 745f 6c69 7175 6964 6974  _divest_liquidit
-00000f90: 790a 2020 2020 2020 2020 7061 7474 6572  y.        patter
-00000fa0: 6e3a 0a20 2020 2020 2020 2020 202d 2074  n:.          - t
-00000fb0: 7970 653a 2074 7261 6e73 6163 7469 6f6e  ype: transaction
-00000fc0: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-00000fd0: 7469 6e61 7469 6f6e 3a20 3c64 6578 5f63  tination: <dex_c
-00000fe0: 6f6e 7472 6163 743e 0a20 2020 2020 2020  ontract>.       
-00000ff0: 2020 2020 2065 6e74 7279 706f 696e 743a       entrypoint:
-00001000: 2064 6976 6573 744c 6971 7569 6469 7479   divestLiquidity
-00001010: 0a20 2020 2020 2020 2020 202d 2074 7970  .          - typ
-00001020: 653a 2074 7261 6e73 6163 7469 6f6e 0a20  e: transaction. 
-00001030: 2020 2020 2020 2020 2020 2064 6573 7469             desti
-00001040: 6e61 7469 6f6e 3a20 3c74 6f6b 656e 5f63  nation: <token_c
-00001050: 6f6e 7472 6163 743e 0a20 2020 2020 2020  ontract>.       
-00001060: 2020 2020 2065 6e74 7279 706f 696e 743a       entrypoint:
-00001070: 2074 7261 6e73 6665 720a 2020 2020 2020   transfer.      
-00001080: 2020 2020 2d20 7479 7065 3a20 7472 616e      - type: tran
-00001090: 7361 6374 696f 6e0a 2020 2020 2020 2020  saction.        
-000010a0: 2020 2020 736f 7572 6365 3a20 3c64 6578      source: <dex
-000010b0: 5f63 6f6e 7472 6163 743e 0a20 2020 2020  _contract>.     
-000010c0: 202d 2063 616c 6c62 6163 6b3a 206f 6e5f   - callback: on_
-000010d0: 6661 325f 7769 7468 6472 6177 5f70 726f  fa2_withdraw_pro
-000010e0: 6669 740a 2020 2020 2020 2020 7061 7474  fit.        patt
-000010f0: 6572 6e3a 0a20 2020 2020 2020 2020 202d  ern:.          -
-00001100: 2074 7970 653a 2074 7261 6e73 6163 7469   type: transacti
-00001110: 6f6e 0a20 2020 2020 2020 2020 2020 2064  on.            d
-00001120: 6573 7469 6e61 7469 6f6e 3a20 3c64 6578  estination: <dex
-00001130: 5f63 6f6e 7472 6163 743e 0a20 2020 2020  _contract>.     
-00001140: 2020 2020 2020 2065 6e74 7279 706f 696e         entrypoin
-00001150: 743a 2077 6974 6864 7261 7750 726f 6669  t: withdrawProfi
-00001160: 740a 2020 2020 2020 2020 2020 2d20 7479  t.          - ty
-00001170: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
-00001180: 2020 2020 2020 2020 2020 2020 736f 7572              sour
-00001190: 6365 3a20 3c64 6578 5f63 6f6e 7472 6163  ce: <dex_contrac
-000011a0: 743e 0a20 2020 2020 2020 2020 2020 206f  t>.            o
-000011b0: 7074 696f 6e61 6c3a 2054 7275 650a 0a69  ptional: True..i
-000011c0: 6e64 6578 6573 3a0a 2020 6b75 7364 5f6d  ndexes:.  kusd_m
-000011d0: 6169 6e6e 6574 3a0a 2020 2020 7465 6d70  ainnet:.    temp
-000011e0: 6c61 7465 3a20 7175 6970 7573 7761 705f  late: quipuswap_
-000011f0: 6661 3132 0a20 2020 2076 616c 7565 733a  fa12.    values:
-00001200: 0a20 2020 2020 2064 6578 5f63 6f6e 7472  .      dex_contr
-00001210: 6163 743a 206b 7573 645f 6465 785f 6d61  act: kusd_dex_ma
-00001220: 696e 6e65 740a 2020 2020 2020 746f 6b65  innet.      toke
-00001230: 6e5f 636f 6e74 7261 6374 3a20 6b75 7364  n_contract: kusd
-00001240: 5f74 6f6b 656e 5f6d 6169 6e6e 6574 0a20  _token_mainnet. 
-00001250: 2020 2020 2073 796d 626f 6c3a 206b 5553       symbol: kUS
-00001260: 440a 2020 2020 2020 6465 6369 6d61 6c73  D.      decimals
-00001270: 3a20 3138 0a0a 2020 6864 616f 5f6d 6169  : 18..  hdao_mai
-00001280: 6e6e 6574 3a0a 2020 2020 7465 6d70 6c61  nnet:.    templa
-00001290: 7465 3a20 7175 6970 7573 7761 705f 6661  te: quipuswap_fa
-000012a0: 320a 2020 2020 7661 6c75 6573 3a0a 2020  2.    values:.  
-000012b0: 2020 2020 6465 785f 636f 6e74 7261 6374      dex_contract
-000012c0: 3a20 6864 616f 5f64 6578 5f6d 6169 6e6e  : hdao_dex_mainn
-000012d0: 6574 0a20 2020 2020 2074 6f6b 656e 5f63  et.      token_c
-000012e0: 6f6e 7472 6163 743a 2068 6461 6f5f 746f  ontract: hdao_to
-000012f0: 6b65 6e5f 6d61 696e 6e65 740a 2020 2020  ken_mainnet.    
-00001300: 2020 7379 6d62 6f6c 3a20 6844 414f 0a20    symbol: hDAO. 
-00001310: 2020 2020 2064 6563 696d 616c 733a 2036       decimals: 6
+00000010: 300a 7061 636b 6167 653a 207b 7b20 7072  0.package: {{ pr
+00000020: 6f6a 6563 742e 7061 636b 6167 6520 7d7d  oject.package }}
+00000030: 0a0a 636f 6e74 7261 6374 733a 0a20 206b  ..contracts:.  k
+00000040: 7573 645f 6465 785f 6d61 696e 6e65 743a  usd_dex_mainnet:
+00000050: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
+00000060: 0a20 2020 2061 6464 7265 7373 3a20 4b54  .    address: KT
+00000070: 314b 3445 7754 7062 7659 4e39 6167 4a64  1K4EwTpbvYN9agJd
+00000080: 6a70 794a 6d34 5a5a 6468 7055 4e4b 4233  jpyJm4ZZdhpUNKB3
+00000090: 4636 0a20 2020 2074 7970 656e 616d 653a  F6.    typename:
+000000a0: 2071 7569 7075 5f66 6131 320a 2020 6b75   quipu_fa12.  ku
+000000b0: 7364 5f74 6f6b 656e 5f6d 6169 6e6e 6574  sd_token_mainnet
+000000c0: 3a0a 2020 2020 6b69 6e64 3a20 7465 7a6f  :.    kind: tezo
+000000d0: 730a 2020 2020 6164 6472 6573 733a 204b  s.    address: K
+000000e0: 5431 4b39 6743 5267 614c 5246 4b54 4572  T1K9gCRgaLRFKTEr
+000000f0: 5974 3177 5678 4133 4672 6239 466a 6173  Yt1wVxA3Frb9Fjas
+00000100: 6a54 560a 2020 2020 7479 7065 6e61 6d65  jTV.    typename
+00000110: 3a20 6661 3132 5f74 6f6b 656e 0a20 2068  : fa12_token.  h
+00000120: 6461 6f5f 6465 785f 6d61 696e 6e65 743a  dao_dex_mainnet:
+00000130: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
+00000140: 0a20 2020 2061 6464 7265 7373 3a20 4b54  .    address: KT
+00000150: 3151 784c 7175 6b79 666f 6850 5635 6b50  1QxLqukyfohPV5kP
+00000160: 6b77 3937 5273 3663 7731 4444 4476 5967  kw97Rs6cw1DDDvYg
+00000170: 6242 0a20 2020 2074 7970 656e 616d 653a  bB.    typename:
+00000180: 2071 7569 7075 5f66 6132 0a20 2068 6461   quipu_fa2.  hda
+00000190: 6f5f 746f 6b65 6e5f 6d61 696e 6e65 743a  o_token_mainnet:
+000001a0: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
+000001b0: 0a20 2020 2061 6464 7265 7373 3a20 4b54  .    address: KT
+000001c0: 3141 4641 326d 774e 554d 4e64 3453 7375  1AFA2mwNUMNd4Ssu
+000001d0: 6a45 3159 5970 3239 7664 3842 5a65 6a79  jE1YYp29vd8BZejy
+000001e0: 4b57 0a20 2020 2074 7970 656e 616d 653a  KW.    typename:
+000001f0: 2066 6132 5f74 6f6b 656e 0a0a 6461 7461   fa2_token..data
+00000200: 736f 7572 6365 733a 0a20 2074 7a6b 745f  sources:.  tzkt_
+00000210: 6d61 696e 6e65 743a 0a20 2020 206b 696e  mainnet:.    kin
+00000220: 643a 2074 657a 6f73 2e74 7a6b 740a 2020  d: tezos.tzkt.  
+00000230: 2020 7572 6c3a 2068 7474 7073 3a2f 2f61    url: https://a
+00000240: 7069 2e74 7a6b 742e 696f 0a0a 7465 6d70  pi.tzkt.io..temp
+00000250: 6c61 7465 733a 0a20 2071 7569 7075 7377  lates:.  quipusw
+00000260: 6170 5f66 6131 323a 0a20 2020 206b 696e  ap_fa12:.    kin
+00000270: 643a 2074 657a 6f73 2e74 7a6b 742e 6f70  d: tezos.tzkt.op
+00000280: 6572 6174 696f 6e73 0a20 2020 2064 6174  erations.    dat
+00000290: 6173 6f75 7263 653a 2074 7a6b 745f 6d61  asource: tzkt_ma
+000002a0: 696e 6e65 740a 2020 2020 636f 6e74 7261  innet.    contra
+000002b0: 6374 733a 0a20 2020 2020 202d 203c 6465  cts:.      - <de
+000002c0: 785f 636f 6e74 7261 6374 3e0a 2020 2020  x_contract>.    
+000002d0: 7479 7065 733a 0a20 2020 2020 202d 2074  types:.      - t
+000002e0: 7261 6e73 6163 7469 6f6e 0a20 2020 2020  ransaction.     
+000002f0: 202d 206f 7269 6769 6e61 7469 6f6e 0a20   - origination. 
+00000300: 2020 2068 616e 646c 6572 733a 0a20 2020     handlers:.   
+00000310: 2020 202d 2063 616c 6c62 6163 6b3a 206f     - callback: o
+00000320: 6e5f 6661 3132 5f6f 7269 6769 6e61 7469  n_fa12_originati
+00000330: 6f6e 0a20 2020 2020 2020 2070 6174 7465  on.        patte
+00000340: 726e 3a0a 2020 2020 2020 2020 2020 2d20  rn:.          - 
+00000350: 7479 7065 3a20 6f72 6967 696e 6174 696f  type: originatio
+00000360: 6e0a 2020 2020 2020 2020 2020 2020 6f72  n.            or
+00000370: 6967 696e 6174 6564 5f63 6f6e 7472 6163  iginated_contrac
+00000380: 743a 203c 6465 785f 636f 6e74 7261 6374  t: <dex_contract
+00000390: 3e0a 2020 2020 2020 2d20 6361 6c6c 6261  >.      - callba
+000003a0: 636b 3a20 6f6e 5f66 6131 325f 746f 6b65  ck: on_fa12_toke
+000003b0: 6e5f 746f 5f74 657a 0a20 2020 2020 2020  n_to_tez.       
+000003c0: 2070 6174 7465 726e 3a0a 2020 2020 2020   pattern:.      
+000003d0: 2020 2020 2d20 7479 7065 3a20 7472 616e      - type: tran
+000003e0: 7361 6374 696f 6e0a 2020 2020 2020 2020  saction.        
+000003f0: 2020 2020 6465 7374 696e 6174 696f 6e3a      destination:
+00000400: 203c 6465 785f 636f 6e74 7261 6374 3e0a   <dex_contract>.
+00000410: 2020 2020 2020 2020 2020 2020 656e 7472              entr
+00000420: 7970 6f69 6e74 3a20 746f 6b65 6e54 6f54  ypoint: tokenToT
+00000430: 657a 5061 796d 656e 740a 2020 2020 2020  ezPayment.      
+00000440: 2020 2020 2d20 7479 7065 3a20 7472 616e      - type: tran
+00000450: 7361 6374 696f 6e0a 2020 2020 2020 2020  saction.        
+00000460: 2020 2020 6465 7374 696e 6174 696f 6e3a      destination:
+00000470: 203c 746f 6b65 6e5f 636f 6e74 7261 6374   <token_contract
+00000480: 3e0a 2020 2020 2020 2020 2020 2020 656e  >.            en
+00000490: 7472 7970 6f69 6e74 3a20 7472 616e 7366  trypoint: transf
+000004a0: 6572 0a20 2020 2020 2020 2020 202d 2074  er.          - t
+000004b0: 7970 653a 2074 7261 6e73 6163 7469 6f6e  ype: transaction
+000004c0: 0a20 2020 2020 2020 2020 2020 2073 6f75  .            sou
+000004d0: 7263 653a 203c 6465 785f 636f 6e74 7261  rce: <dex_contra
+000004e0: 6374 3e0a 2020 2020 2020 2d20 6361 6c6c  ct>.      - call
+000004f0: 6261 636b 3a20 6f6e 5f66 6131 325f 7465  back: on_fa12_te
+00000500: 7a5f 746f 5f74 6f6b 656e 0a20 2020 2020  z_to_token.     
+00000510: 2020 2070 6174 7465 726e 3a0a 2020 2020     pattern:.    
+00000520: 2020 2020 2020 2d20 7479 7065 3a20 7472        - type: tr
+00000530: 616e 7361 6374 696f 6e0a 2020 2020 2020  ansaction.      
+00000540: 2020 2020 2020 6465 7374 696e 6174 696f        destinatio
+00000550: 6e3a 203c 6465 785f 636f 6e74 7261 6374  n: <dex_contract
+00000560: 3e0a 2020 2020 2020 2020 2020 2020 656e  >.            en
+00000570: 7472 7970 6f69 6e74 3a20 7465 7a54 6f54  trypoint: tezToT
+00000580: 6f6b 656e 5061 796d 656e 740a 2020 2020  okenPayment.    
+00000590: 2020 2020 2020 2d20 7479 7065 3a20 7472        - type: tr
+000005a0: 616e 7361 6374 696f 6e0a 2020 2020 2020  ansaction.      
+000005b0: 2020 2020 2020 6465 7374 696e 6174 696f        destinatio
+000005c0: 6e3a 203c 746f 6b65 6e5f 636f 6e74 7261  n: <token_contra
+000005d0: 6374 3e0a 2020 2020 2020 2020 2020 2020  ct>.            
+000005e0: 656e 7472 7970 6f69 6e74 3a20 7472 616e  entrypoint: tran
+000005f0: 7366 6572 0a20 2020 2020 202d 2063 616c  sfer.      - cal
+00000600: 6c62 6163 6b3a 206f 6e5f 6661 3132 5f69  lback: on_fa12_i
+00000610: 6e76 6573 745f 6c69 7175 6964 6974 790a  nvest_liquidity.
+00000620: 2020 2020 2020 2020 7061 7474 6572 6e3a          pattern:
+00000630: 0a20 2020 2020 2020 2020 202d 2074 7970  .          - typ
+00000640: 653a 2074 7261 6e73 6163 7469 6f6e 0a20  e: transaction. 
+00000650: 2020 2020 2020 2020 2020 2064 6573 7469             desti
+00000660: 6e61 7469 6f6e 3a20 3c64 6578 5f63 6f6e  nation: <dex_con
+00000670: 7472 6163 743e 0a20 2020 2020 2020 2020  tract>.         
+00000680: 2020 2065 6e74 7279 706f 696e 743a 2069     entrypoint: i
+00000690: 6e76 6573 744c 6971 7569 6469 7479 0a20  nvestLiquidity. 
+000006a0: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
+000006b0: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
+000006c0: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
+000006d0: 7469 6f6e 3a20 3c74 6f6b 656e 5f63 6f6e  tion: <token_con
+000006e0: 7472 6163 743e 0a20 2020 2020 2020 2020  tract>.         
+000006f0: 2020 2065 6e74 7279 706f 696e 743a 2074     entrypoint: t
+00000700: 7261 6e73 6665 720a 2020 2020 2020 2d20  ransfer.      - 
+00000710: 6361 6c6c 6261 636b 3a20 6f6e 5f66 6131  callback: on_fa1
+00000720: 325f 7472 616e 7366 6572 0a20 2020 2020  2_transfer.     
+00000730: 2020 2070 6174 7465 726e 3a0a 2020 2020     pattern:.    
+00000740: 2020 2020 2020 2d20 7479 7065 3a20 7472        - type: tr
+00000750: 616e 7361 6374 696f 6e0a 2020 2020 2020  ansaction.      
+00000760: 2020 2020 2020 6465 7374 696e 6174 696f        destinatio
+00000770: 6e3a 203c 6465 785f 636f 6e74 7261 6374  n: <dex_contract
+00000780: 3e0a 2020 2020 2020 2020 2020 2020 656e  >.            en
+00000790: 7472 7970 6f69 6e74 3a20 7472 616e 7366  trypoint: transf
+000007a0: 6572 0a20 2020 2020 202d 2063 616c 6c62  er.      - callb
+000007b0: 6163 6b3a 206f 6e5f 6661 3132 5f64 6976  ack: on_fa12_div
+000007c0: 6573 745f 6c69 7175 6964 6974 790a 2020  est_liquidity.  
+000007d0: 2020 2020 2020 7061 7474 6572 6e3a 0a20        pattern:. 
+000007e0: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
+000007f0: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
+00000800: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
+00000810: 7469 6f6e 3a20 3c64 6578 5f63 6f6e 7472  tion: <dex_contr
+00000820: 6163 743e 0a20 2020 2020 2020 2020 2020  act>.           
+00000830: 2065 6e74 7279 706f 696e 743a 2064 6976   entrypoint: div
+00000840: 6573 744c 6971 7569 6469 7479 0a20 2020  estLiquidity.   
+00000850: 2020 2020 2020 202d 2074 7970 653a 2074         - type: t
+00000860: 7261 6e73 6163 7469 6f6e 0a20 2020 2020  ransaction.     
+00000870: 2020 2020 2020 2064 6573 7469 6e61 7469         destinati
+00000880: 6f6e 3a20 3c74 6f6b 656e 5f63 6f6e 7472  on: <token_contr
+00000890: 6163 743e 0a20 2020 2020 2020 2020 2020  act>.           
+000008a0: 2065 6e74 7279 706f 696e 743a 2074 7261   entrypoint: tra
+000008b0: 6e73 6665 720a 2020 2020 2020 2020 2020  nsfer.          
+000008c0: 2d20 7479 7065 3a20 7472 616e 7361 6374  - type: transact
+000008d0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+000008e0: 736f 7572 6365 3a20 3c64 6578 5f63 6f6e  source: <dex_con
+000008f0: 7472 6163 743e 0a20 2020 2020 202d 2063  tract>.      - c
+00000900: 616c 6c62 6163 6b3a 206f 6e5f 6661 3132  allback: on_fa12
+00000910: 5f77 6974 6864 7261 775f 7072 6f66 6974  _withdraw_profit
+00000920: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
+00000930: 3a0a 2020 2020 2020 2020 2020 2d20 7479  :.          - ty
+00000940: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
+00000950: 2020 2020 2020 2020 2020 2020 6465 7374              dest
+00000960: 696e 6174 696f 6e3a 203c 6465 785f 636f  ination: <dex_co
+00000970: 6e74 7261 6374 3e0a 2020 2020 2020 2020  ntract>.        
+00000980: 2020 2020 656e 7472 7970 6f69 6e74 3a20      entrypoint: 
+00000990: 7769 7468 6472 6177 5072 6f66 6974 0a20  withdrawProfit. 
+000009a0: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
+000009b0: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
+000009c0: 2020 2020 2020 2020 2073 6f75 7263 653a           source:
+000009d0: 203c 6465 785f 636f 6e74 7261 6374 3e0a   <dex_contract>.
+000009e0: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
+000009f0: 6f6e 616c 3a20 5472 7565 0a0a 2020 7175  onal: True..  qu
+00000a00: 6970 7573 7761 705f 6661 323a 0a20 2020  ipuswap_fa2:.   
+00000a10: 206b 696e 643a 2074 657a 6f73 2e74 7a6b   kind: tezos.tzk
+00000a20: 742e 6f70 6572 6174 696f 6e73 0a20 2020  t.operations.   
+00000a30: 2064 6174 6173 6f75 7263 653a 2074 7a6b   datasource: tzk
+00000a40: 745f 6d61 696e 6e65 740a 2020 2020 636f  t_mainnet.    co
+00000a50: 6e74 7261 6374 733a 0a20 2020 2020 202d  ntracts:.      -
+00000a60: 203c 6465 785f 636f 6e74 7261 6374 3e0a   <dex_contract>.
+00000a70: 2020 2020 7479 7065 733a 0a20 2020 2020      types:.     
+00000a80: 202d 2074 7261 6e73 6163 7469 6f6e 0a20   - transaction. 
+00000a90: 2020 2020 202d 206f 7269 6769 6e61 7469       - originati
+00000aa0: 6f6e 0a20 2020 2068 616e 646c 6572 733a  on.    handlers:
+00000ab0: 0a20 2020 2020 202d 2063 616c 6c62 6163  .      - callbac
+00000ac0: 6b3a 206f 6e5f 6661 325f 6f72 6967 696e  k: on_fa2_origin
+00000ad0: 6174 696f 6e0a 2020 2020 2020 2020 7061  ation.        pa
+00000ae0: 7474 6572 6e3a 0a20 2020 2020 2020 2020  ttern:.         
+00000af0: 202d 2074 7970 653a 206f 7269 6769 6e61   - type: origina
+00000b00: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+00000b10: 206f 7269 6769 6e61 7465 645f 636f 6e74   originated_cont
+00000b20: 7261 6374 3a20 3c64 6578 5f63 6f6e 7472  ract: <dex_contr
+00000b30: 6163 743e 0a20 2020 2020 202d 2063 616c  act>.      - cal
+00000b40: 6c62 6163 6b3a 206f 6e5f 6661 325f 746f  lback: on_fa2_to
+00000b50: 6b65 6e5f 746f 5f74 657a 0a20 2020 2020  ken_to_tez.     
+00000b60: 2020 2070 6174 7465 726e 3a0a 2020 2020     pattern:.    
+00000b70: 2020 2020 2020 2d20 7479 7065 3a20 7472        - type: tr
+00000b80: 616e 7361 6374 696f 6e0a 2020 2020 2020  ansaction.      
+00000b90: 2020 2020 2020 6465 7374 696e 6174 696f        destinatio
+00000ba0: 6e3a 203c 6465 785f 636f 6e74 7261 6374  n: <dex_contract
+00000bb0: 3e0a 2020 2020 2020 2020 2020 2020 656e  >.            en
+00000bc0: 7472 7970 6f69 6e74 3a20 746f 6b65 6e54  trypoint: tokenT
+00000bd0: 6f54 657a 5061 796d 656e 740a 2020 2020  oTezPayment.    
+00000be0: 2020 2020 2020 2d20 7479 7065 3a20 7472        - type: tr
+00000bf0: 616e 7361 6374 696f 6e0a 2020 2020 2020  ansaction.      
+00000c00: 2020 2020 2020 6465 7374 696e 6174 696f        destinatio
+00000c10: 6e3a 203c 746f 6b65 6e5f 636f 6e74 7261  n: <token_contra
+00000c20: 6374 3e0a 2020 2020 2020 2020 2020 2020  ct>.            
+00000c30: 656e 7472 7970 6f69 6e74 3a20 7472 616e  entrypoint: tran
+00000c40: 7366 6572 0a20 2020 2020 2020 2020 202d  sfer.          -
+00000c50: 2074 7970 653a 2074 7261 6e73 6163 7469   type: transacti
+00000c60: 6f6e 0a20 2020 2020 2020 2020 2020 2073  on.            s
+00000c70: 6f75 7263 653a 203c 6465 785f 636f 6e74  ource: <dex_cont
+00000c80: 7261 6374 3e0a 2020 2020 2020 2d20 6361  ract>.      - ca
+00000c90: 6c6c 6261 636b 3a20 6f6e 5f66 6132 5f74  llback: on_fa2_t
+00000ca0: 657a 5f74 6f5f 746f 6b65 6e0a 2020 2020  ez_to_token.    
+00000cb0: 2020 2020 7061 7474 6572 6e3a 0a20 2020      pattern:.   
+00000cc0: 2020 2020 2020 202d 2074 7970 653a 2074         - type: t
+00000cd0: 7261 6e73 6163 7469 6f6e 0a20 2020 2020  ransaction.     
+00000ce0: 2020 2020 2020 2064 6573 7469 6e61 7469         destinati
+00000cf0: 6f6e 3a20 3c64 6578 5f63 6f6e 7472 6163  on: <dex_contrac
+00000d00: 743e 0a20 2020 2020 2020 2020 2020 2065  t>.            e
+00000d10: 6e74 7279 706f 696e 743a 2074 657a 546f  ntrypoint: tezTo
+00000d20: 546f 6b65 6e50 6179 6d65 6e74 0a20 2020  TokenPayment.   
+00000d30: 2020 2020 2020 202d 2074 7970 653a 2074         - type: t
+00000d40: 7261 6e73 6163 7469 6f6e 0a20 2020 2020  ransaction.     
+00000d50: 2020 2020 2020 2064 6573 7469 6e61 7469         destinati
+00000d60: 6f6e 3a20 3c74 6f6b 656e 5f63 6f6e 7472  on: <token_contr
+00000d70: 6163 743e 0a20 2020 2020 2020 2020 2020  act>.           
+00000d80: 2065 6e74 7279 706f 696e 743a 2074 7261   entrypoint: tra
+00000d90: 6e73 6665 720a 2020 2020 2020 2d20 6361  nsfer.      - ca
+00000da0: 6c6c 6261 636b 3a20 6f6e 5f66 6132 5f69  llback: on_fa2_i
+00000db0: 6e76 6573 745f 6c69 7175 6964 6974 790a  nvest_liquidity.
+00000dc0: 2020 2020 2020 2020 7061 7474 6572 6e3a          pattern:
+00000dd0: 0a20 2020 2020 2020 2020 202d 2074 7970  .          - typ
+00000de0: 653a 2074 7261 6e73 6163 7469 6f6e 0a20  e: transaction. 
+00000df0: 2020 2020 2020 2020 2020 2064 6573 7469             desti
+00000e00: 6e61 7469 6f6e 3a20 3c64 6578 5f63 6f6e  nation: <dex_con
+00000e10: 7472 6163 743e 0a20 2020 2020 2020 2020  tract>.         
+00000e20: 2020 2065 6e74 7279 706f 696e 743a 2069     entrypoint: i
+00000e30: 6e76 6573 744c 6971 7569 6469 7479 0a20  nvestLiquidity. 
+00000e40: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
+00000e50: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
+00000e60: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
+00000e70: 7469 6f6e 3a20 3c74 6f6b 656e 5f63 6f6e  tion: <token_con
+00000e80: 7472 6163 743e 0a20 2020 2020 2020 2020  tract>.         
+00000e90: 2020 2065 6e74 7279 706f 696e 743a 2074     entrypoint: t
+00000ea0: 7261 6e73 6665 720a 2020 2020 2020 2d20  ransfer.      - 
+00000eb0: 6361 6c6c 6261 636b 3a20 6f6e 5f66 6132  callback: on_fa2
+00000ec0: 5f74 7261 6e73 6665 720a 2020 2020 2020  _transfer.      
+00000ed0: 2020 7061 7474 6572 6e3a 0a20 2020 2020    pattern:.     
+00000ee0: 2020 2020 202d 2074 7970 653a 2074 7261       - type: tra
+00000ef0: 6e73 6163 7469 6f6e 0a20 2020 2020 2020  nsaction.       
+00000f00: 2020 2020 2064 6573 7469 6e61 7469 6f6e       destination
+00000f10: 3a20 3c64 6578 5f63 6f6e 7472 6163 743e  : <dex_contract>
+00000f20: 0a20 2020 2020 2020 2020 2020 2065 6e74  .            ent
+00000f30: 7279 706f 696e 743a 2074 7261 6e73 6665  rypoint: transfe
+00000f40: 720a 2020 2020 2020 2d20 6361 6c6c 6261  r.      - callba
+00000f50: 636b 3a20 6f6e 5f66 6132 5f64 6976 6573  ck: on_fa2_dives
+00000f60: 745f 6c69 7175 6964 6974 790a 2020 2020  t_liquidity.    
+00000f70: 2020 2020 7061 7474 6572 6e3a 0a20 2020      pattern:.   
+00000f80: 2020 2020 2020 202d 2074 7970 653a 2074         - type: t
+00000f90: 7261 6e73 6163 7469 6f6e 0a20 2020 2020  ransaction.     
+00000fa0: 2020 2020 2020 2064 6573 7469 6e61 7469         destinati
+00000fb0: 6f6e 3a20 3c64 6578 5f63 6f6e 7472 6163  on: <dex_contrac
+00000fc0: 743e 0a20 2020 2020 2020 2020 2020 2065  t>.            e
+00000fd0: 6e74 7279 706f 696e 743a 2064 6976 6573  ntrypoint: dives
+00000fe0: 744c 6971 7569 6469 7479 0a20 2020 2020  tLiquidity.     
+00000ff0: 2020 2020 202d 2074 7970 653a 2074 7261       - type: tra
+00001000: 6e73 6163 7469 6f6e 0a20 2020 2020 2020  nsaction.       
+00001010: 2020 2020 2064 6573 7469 6e61 7469 6f6e       destination
+00001020: 3a20 3c74 6f6b 656e 5f63 6f6e 7472 6163  : <token_contrac
+00001030: 743e 0a20 2020 2020 2020 2020 2020 2065  t>.            e
+00001040: 6e74 7279 706f 696e 743a 2074 7261 6e73  ntrypoint: trans
+00001050: 6665 720a 2020 2020 2020 2020 2020 2d20  fer.          - 
+00001060: 7479 7065 3a20 7472 616e 7361 6374 696f  type: transactio
+00001070: 6e0a 2020 2020 2020 2020 2020 2020 736f  n.            so
+00001080: 7572 6365 3a20 3c64 6578 5f63 6f6e 7472  urce: <dex_contr
+00001090: 6163 743e 0a20 2020 2020 202d 2063 616c  act>.      - cal
+000010a0: 6c62 6163 6b3a 206f 6e5f 6661 325f 7769  lback: on_fa2_wi
+000010b0: 7468 6472 6177 5f70 726f 6669 740a 2020  thdraw_profit.  
+000010c0: 2020 2020 2020 7061 7474 6572 6e3a 0a20        pattern:. 
+000010d0: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
+000010e0: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
+000010f0: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
+00001100: 7469 6f6e 3a20 3c64 6578 5f63 6f6e 7472  tion: <dex_contr
+00001110: 6163 743e 0a20 2020 2020 2020 2020 2020  act>.           
+00001120: 2065 6e74 7279 706f 696e 743a 2077 6974   entrypoint: wit
+00001130: 6864 7261 7750 726f 6669 740a 2020 2020  hdrawProfit.    
+00001140: 2020 2020 2020 2d20 7479 7065 3a20 7472        - type: tr
+00001150: 616e 7361 6374 696f 6e0a 2020 2020 2020  ansaction.      
+00001160: 2020 2020 2020 736f 7572 6365 3a20 3c64        source: <d
+00001170: 6578 5f63 6f6e 7472 6163 743e 0a20 2020  ex_contract>.   
+00001180: 2020 2020 2020 2020 206f 7074 696f 6e61           optiona
+00001190: 6c3a 2054 7275 650a 0a69 6e64 6578 6573  l: True..indexes
+000011a0: 3a0a 2020 6b75 7364 5f6d 6169 6e6e 6574  :.  kusd_mainnet
+000011b0: 3a0a 2020 2020 7465 6d70 6c61 7465 3a20  :.    template: 
+000011c0: 7175 6970 7573 7761 705f 6661 3132 0a20  quipuswap_fa12. 
+000011d0: 2020 2076 616c 7565 733a 0a20 2020 2020     values:.     
+000011e0: 2064 6578 5f63 6f6e 7472 6163 743a 206b   dex_contract: k
+000011f0: 7573 645f 6465 785f 6d61 696e 6e65 740a  usd_dex_mainnet.
+00001200: 2020 2020 2020 746f 6b65 6e5f 636f 6e74        token_cont
+00001210: 7261 6374 3a20 6b75 7364 5f74 6f6b 656e  ract: kusd_token
+00001220: 5f6d 6169 6e6e 6574 0a20 2020 2020 2073  _mainnet.      s
+00001230: 796d 626f 6c3a 206b 5553 440a 2020 2020  ymbol: kUSD.    
+00001240: 2020 6465 6369 6d61 6c73 3a20 3138 0a0a    decimals: 18..
+00001250: 2020 6864 616f 5f6d 6169 6e6e 6574 3a0a    hdao_mainnet:.
+00001260: 2020 2020 7465 6d70 6c61 7465 3a20 7175      template: qu
+00001270: 6970 7573 7761 705f 6661 320a 2020 2020  ipuswap_fa2.    
+00001280: 7661 6c75 6573 3a0a 2020 2020 2020 6465  values:.      de
+00001290: 785f 636f 6e74 7261 6374 3a20 6864 616f  x_contract: hdao
+000012a0: 5f64 6578 5f6d 6169 6e6e 6574 0a20 2020  _dex_mainnet.   
+000012b0: 2020 2074 6f6b 656e 5f63 6f6e 7472 6163     token_contrac
+000012c0: 743a 2068 6461 6f5f 746f 6b65 6e5f 6d61  t: hdao_token_ma
+000012d0: 696e 6e65 740a 2020 2020 2020 7379 6d62  innet.      symb
+000012e0: 6f6c 3a20 6844 414f 0a20 2020 2020 2064  ol: hDAO.      d
+000012f0: 6563 696d 616c 733a 2036 0a              ecimals: 6.
```

### Comparing `dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_divest_liquidity.py` & `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_divest_liquidity.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_invest_liquidity.py` & `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_invest_liquidity.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_origination.py` & `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_origination.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_tez_to_token.py` & `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_tez_to_token.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_token_to_tez.py` & `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_token_to_tez.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_transfer.py` & `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_transfer.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_withdraw_profit.py` & `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa12_withdraw_profit.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa2_divest_liquidity.py` & `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_divest_liquidity.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa2_invest_liquidity.py` & `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_invest_liquidity.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa2_origination.py` & `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_origination.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa2_tez_to_token.py` & `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_tez_to_token.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa2_token_to_tez.py` & `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_token_to_tez.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa2_transfer.py` & `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_transfer.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa2_withdraw_profit.py` & `dipdup-7.0.0rc2/src/demo_dex/handlers/on_fa2_withdraw_profit.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_dex/models/__init__.py` & `dipdup-7.0.0rc2/src/demo_dex/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_dex/pyproject.toml` & `dipdup-7.0.0rc2/src/demo_events/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
-name = "demo_dex"
+name = "demo_events"
 version = "0.0.1"
-description = "Quipuswap DEX balances and liquidity"
+description = "Processing contract events"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc1,<8"
+    "dipdup>=7.0.0rc2,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
@@ -24,17 +24,15 @@
 _isort = "isort ."
 _black = "black ."
 _ruff = "ruff check --fix ."
 _mypy = "mypy ."
 all = { composite = ["fmt", "lint"] }
 fmt = { composite = ["_isort", "_black"] }
 lint = { composite = ["_ruff", "_mypy"] }
-image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_dex:latest"
-
-clean = "git clean -xdf --exclude=.venv"
+image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_events:latest"
 
 [tool.isort]
 line_length = 120
 force_single_line = true
 
 [tool.black]
 line-length = 120
```

### Comparing `dipdup-7.0.0rc1/src/demo_dex/types/fa12_token/tezos_storage.py` & `dipdup-7.0.0rc2/src/demo_dex/types/fa12_token/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_dex/types/fa2_token/tezos_storage.py` & `dipdup-7.0.0rc2/src/demo_dex/types/fa2_token/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa12/tezos_storage.py` & `dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa12/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa2/tezos_storage.py` & `dipdup-7.0.0rc2/src/demo_dex/types/quipu_fa2/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_domains/README.md` & `dipdup-7.0.0rc2/src/demo_domains/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
 ```bash
 curl -Lsf https://dipdup.io/install.py | python3
 ```
 
-See the [Installation](https://docs.dipdup.io/installation) page for all options.
+See the [Installation](https://dipdup.io/docs/installation) page for all options.
 
 ## Usage
 
 Run the indexer in-memory:
 
 ```bash
 dipdup run
@@ -27,17 +27,17 @@
 ```bash
 dipdup -c . -c configs/dipdup.sqlite.yml run
 ```
 
 Or spawn a docker-compose stack:
 
 ```bash
-cp deploy/.env.example .env
+cp deploy/.env.default deploy/.env
 # Edit .env before running
-docker-compose -f deploy/docker-compose.yml up
+docker-compose -f deploy/compose.yaml up
 ```
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
```

### Comparing `dipdup-7.0.0rc1/src/demo_domains/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc2/src/demo_domains/deploy/compose.swarm.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     deploy:
       mode: replicated
       replicas: 1
       placement: *placement
     logging: *logging
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     depends_on:
       - db
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@demo_domains_db:5432/dipdup
       - HASURA_GRAPHQL_ADMIN_SECRET=${HASURA_SECRET}
       - HASURA_GRAPHQL_ENABLE_CONSOLE=true
       - HASURA_GRAPHQL_DEV_MODE=false
```

### Comparing `dipdup-7.0.0rc1/src/demo_domains/deploy/compose.yaml` & `dipdup-7.0.0rc2/src/demo_domains/deploy/compose.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     healthcheck:
       test: ["CMD-SHELL", "pg_isready -U dipdup"]
       interval: 10s
       timeout: 5s
       retries: 5
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     ports:
       - 8080
     depends_on:
       - db
     restart: always
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@db:5432/dipdup
```

### Comparing `dipdup-7.0.0rc1/src/demo_domains/dipdup.yaml` & `dipdup-7.0.0rc2/src/demo_domains/dipdup.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,53 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
-00000020: 646f 6d61 696e 730a 0a64 6174 6162 6173  domains..databas
-00000030: 653a 0a20 206b 696e 643a 2073 716c 6974  e:.  kind: sqlit
-00000040: 650a 2020 7061 7468 3a20 6465 6d6f 5f64  e.  path: demo_d
-00000050: 6f6d 6169 6e73 2e73 716c 6974 6533 0a0a  omains.sqlite3..
-00000060: 636f 6e74 7261 6374 733a 0a20 206d 6169  contracts:.  mai
-00000070: 6e6e 6574 5f6e 616d 655f 7265 6769 7374  nnet_name_regist
-00000080: 7279 3a0a 2020 2020 6b69 6e64 3a20 7465  ry:.    kind: te
-00000090: 7a6f 730a 2020 2020 6164 6472 6573 733a  zos.    address:
-000000a0: 204b 5431 4742 5a6d 5378 6d6e 4b4a 5847   KT1GBZmSxmnKJXG
-000000b0: 4d64 4d4c 6275 6750 664c 7955 506d 754c  MdMLbugPfLyUPmuL
-000000c0: 534d 774b 530a 2020 2020 7479 7065 6e61  SMwKS.    typena
-000000d0: 6d65 3a20 6e61 6d65 5f72 6567 6973 7472  me: name_registr
-000000e0: 790a 0a64 6174 6173 6f75 7263 6573 3a0a  y..datasources:.
-000000f0: 2020 747a 6b74 5f6d 6169 6e6e 6574 3a0a    tzkt_mainnet:.
-00000100: 2020 2020 6b69 6e64 3a20 7465 7a6f 732e      kind: tezos.
-00000110: 747a 6b74 0a20 2020 2075 726c 3a20 247b  tzkt.    url: ${
-00000120: 545a 4b54 5f55 524c 3a2d 6874 7470 733a  TZKT_URL:-https:
-00000130: 2f2f 6170 692e 747a 6b74 2e69 6f7d 0a0a  //api.tzkt.io}..
-00000140: 7465 6d70 6c61 7465 733a 0a20 2064 6f6d  templates:.  dom
-00000150: 6169 6e73 3a0a 2020 2020 6b69 6e64 3a20  ains:.    kind: 
-00000160: 7465 7a6f 732e 747a 6b74 2e6f 7065 7261  tezos.tzkt.opera
-00000170: 7469 6f6e 730a 2020 2020 6461 7461 736f  tions.    dataso
-00000180: 7572 6365 3a20 3c64 6174 6173 6f75 7263  urce: <datasourc
-00000190: 653e 0a20 2020 2063 6f6e 7472 6163 7473  e>.    contracts
-000001a0: 3a0a 2020 2020 2020 2d20 3c6e 616d 655f  :.      - <name_
-000001b0: 7265 6769 7374 7279 3e0a 2020 2020 6861  registry>.    ha
-000001c0: 6e64 6c65 7273 3a0a 2020 2020 2020 2d20  ndlers:.      - 
-000001d0: 6361 6c6c 6261 636b 3a20 6f6e 5f61 646d  callback: on_adm
-000001e0: 696e 5f75 7064 6174 650a 2020 2020 2020  in_update.      
-000001f0: 2020 7061 7474 6572 6e3a 0a20 2020 2020    pattern:.     
-00000200: 2020 2020 202d 2074 7970 653a 2074 7261       - type: tra
-00000210: 6e73 6163 7469 6f6e 0a20 2020 2020 2020  nsaction.       
-00000220: 2020 2020 2064 6573 7469 6e61 7469 6f6e       destination
-00000230: 3a20 3c6e 616d 655f 7265 6769 7374 7279  : <name_registry
-00000240: 3e0a 2020 2020 2020 2020 2020 2020 656e  >.            en
-00000250: 7472 7970 6f69 6e74 3a20 6164 6d69 6e5f  trypoint: admin_
-00000260: 7570 6461 7465 0a20 2020 2020 202d 2063  update.      - c
-00000270: 616c 6c62 6163 6b3a 206f 6e5f 6578 6563  allback: on_exec
-00000280: 7574 650a 2020 2020 2020 2020 7061 7474  ute.        patt
-00000290: 6572 6e3a 0a20 2020 2020 2020 2020 202d  ern:.          -
-000002a0: 2074 7970 653a 2074 7261 6e73 6163 7469   type: transacti
-000002b0: 6f6e 0a20 2020 2020 2020 2020 2020 2064  on.            d
-000002c0: 6573 7469 6e61 7469 6f6e 3a20 3c6e 616d  estination: <nam
-000002d0: 655f 7265 6769 7374 7279 3e0a 2020 2020  e_registry>.    
-000002e0: 2020 2020 2020 2020 656e 7472 7970 6f69          entrypoi
-000002f0: 6e74 3a20 6578 6563 7574 650a 0a69 6e64  nt: execute..ind
-00000300: 6578 6573 3a0a 2020 646f 6d61 696e 735f  exes:.  domains_
-00000310: 6d61 696e 6e65 743a 0a20 2020 2074 656d  mainnet:.    tem
-00000320: 706c 6174 653a 2064 6f6d 6169 6e73 0a20  plate: domains. 
-00000330: 2020 2076 616c 7565 733a 0a20 2020 2020     values:.     
-00000340: 2064 6174 6173 6f75 7263 653a 2074 7a6b   datasource: tzk
-00000350: 745f 6d61 696e 6e65 740a 2020 2020 2020  t_mainnet.      
-00000360: 6e61 6d65 5f72 6567 6973 7472 793a 206d  name_registry: m
-00000370: 6169 6e6e 6574 5f6e 616d 655f 7265 6769  ainnet_name_regi
-00000380: 7374 7279                                stry
+00000020: 646f 6d61 696e 730a 0a63 6f6e 7472 6163  domains..contrac
+00000030: 7473 3a0a 2020 6d61 696e 6e65 745f 6e61  ts:.  mainnet_na
+00000040: 6d65 5f72 6567 6973 7472 793a 0a20 2020  me_registry:.   
+00000050: 206b 696e 643a 2074 657a 6f73 0a20 2020   kind: tezos.   
+00000060: 2061 6464 7265 7373 3a20 4b54 3147 425a   address: KT1GBZ
+00000070: 6d53 786d 6e4b 4a58 474d 644d 4c62 7567  mSxmnKJXGMdMLbug
+00000080: 5066 4c79 5550 6d75 4c53 4d77 4b53 0a20  PfLyUPmuLSMwKS. 
+00000090: 2020 2074 7970 656e 616d 653a 206e 616d     typename: nam
+000000a0: 655f 7265 6769 7374 7279 0a0a 6461 7461  e_registry..data
+000000b0: 736f 7572 6365 733a 0a20 2074 7a6b 745f  sources:.  tzkt_
+000000c0: 6d61 696e 6e65 743a 0a20 2020 206b 696e  mainnet:.    kin
+000000d0: 643a 2074 657a 6f73 2e74 7a6b 740a 2020  d: tezos.tzkt.  
+000000e0: 2020 7572 6c3a 2024 7b54 5a4b 545f 5552    url: ${TZKT_UR
+000000f0: 4c3a 2d68 7474 7073 3a2f 2f61 7069 2e74  L:-https://api.t
+00000100: 7a6b 742e 696f 7d0a 0a74 656d 706c 6174  zkt.io}..templat
+00000110: 6573 3a0a 2020 646f 6d61 696e 733a 0a20  es:.  domains:. 
+00000120: 2020 206b 696e 643a 2074 657a 6f73 2e74     kind: tezos.t
+00000130: 7a6b 742e 6f70 6572 6174 696f 6e73 0a20  zkt.operations. 
+00000140: 2020 2064 6174 6173 6f75 7263 653a 203c     datasource: <
+00000150: 6461 7461 736f 7572 6365 3e0a 2020 2020  datasource>.    
+00000160: 636f 6e74 7261 6374 733a 0a20 2020 2020  contracts:.     
+00000170: 202d 203c 6e61 6d65 5f72 6567 6973 7472   - <name_registr
+00000180: 793e 0a20 2020 2068 616e 646c 6572 733a  y>.    handlers:
+00000190: 0a20 2020 2020 202d 2063 616c 6c62 6163  .      - callbac
+000001a0: 6b3a 206f 6e5f 6164 6d69 6e5f 7570 6461  k: on_admin_upda
+000001b0: 7465 0a20 2020 2020 2020 2070 6174 7465  te.        patte
+000001c0: 726e 3a0a 2020 2020 2020 2020 2020 2d20  rn:.          - 
+000001d0: 7479 7065 3a20 7472 616e 7361 6374 696f  type: transactio
+000001e0: 6e0a 2020 2020 2020 2020 2020 2020 6465  n.            de
+000001f0: 7374 696e 6174 696f 6e3a 203c 6e61 6d65  stination: <name
+00000200: 5f72 6567 6973 7472 793e 0a20 2020 2020  _registry>.     
+00000210: 2020 2020 2020 2065 6e74 7279 706f 696e         entrypoin
+00000220: 743a 2061 646d 696e 5f75 7064 6174 650a  t: admin_update.
+00000230: 2020 2020 2020 2d20 6361 6c6c 6261 636b        - callback
+00000240: 3a20 6f6e 5f65 7865 6375 7465 0a20 2020  : on_execute.   
+00000250: 2020 2020 2070 6174 7465 726e 3a0a 2020       pattern:.  
+00000260: 2020 2020 2020 2020 2d20 7479 7065 3a20          - type: 
+00000270: 7472 616e 7361 6374 696f 6e0a 2020 2020  transaction.    
+00000280: 2020 2020 2020 2020 6465 7374 696e 6174          destinat
+00000290: 696f 6e3a 203c 6e61 6d65 5f72 6567 6973  ion: <name_regis
+000002a0: 7472 793e 0a20 2020 2020 2020 2020 2020  try>.           
+000002b0: 2065 6e74 7279 706f 696e 743a 2065 7865   entrypoint: exe
+000002c0: 6375 7465 0a0a 696e 6465 7865 733a 0a20  cute..indexes:. 
+000002d0: 2064 6f6d 6169 6e73 5f6d 6169 6e6e 6574   domains_mainnet
+000002e0: 3a0a 2020 2020 7465 6d70 6c61 7465 3a20  :.    template: 
+000002f0: 646f 6d61 696e 730a 2020 2020 7661 6c75  domains.    valu
+00000300: 6573 3a0a 2020 2020 2020 6461 7461 736f  es:.      dataso
+00000310: 7572 6365 3a20 747a 6b74 5f6d 6169 6e6e  urce: tzkt_mainn
+00000320: 6574 0a20 2020 2020 206e 616d 655f 7265  et.      name_re
+00000330: 6769 7374 7279 3a20 6d61 696e 6e65 745f  gistry: mainnet_
+00000340: 6e61 6d65 5f72 6567 6973 7472 79         name_registry
```

### Comparing `dipdup-7.0.0rc1/src/demo_domains/handlers/on_admin_update.py` & `dipdup-7.0.0rc2/src/demo_domains/handlers/on_admin_update.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_domains/handlers/on_execute.py` & `dipdup-7.0.0rc2/src/demo_domains/handlers/on_execute.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_domains/handlers/on_storage_diff.py` & `dipdup-7.0.0rc2/src/demo_domains/handlers/on_storage_diff.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_domains/models/__init__.py` & `dipdup-7.0.0rc2/src/demo_domains/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_domains/pyproject.toml` & `dipdup-7.0.0rc2/src/demo_factories/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
-name = "demo_domains"
+name = "demo_factories"
 version = "0.0.1"
-description = "Tezos Domains name service"
+description = "A very basic indexer for USDt transfers"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc1,<8"
+    "dipdup>=7.0.0rc2,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
@@ -24,17 +24,15 @@
 _isort = "isort ."
 _black = "black ."
 _ruff = "ruff check --fix ."
 _mypy = "mypy ."
 all = { composite = ["fmt", "lint"] }
 fmt = { composite = ["_isort", "_black"] }
 lint = { composite = ["_ruff", "_mypy"] }
-image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_domains:latest"
-
-clean = "git clean -xdf --exclude=.venv"
+image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_factories:latest"
 
 [tool.isort]
 line_length = 120
 force_single_line = true
 
 [tool.black]
 line-length = 120
```

### Comparing `dipdup-7.0.0rc1/src/demo_domains/types/name_registry/tezos_storage.py` & `dipdup-7.0.0rc2/src/demo_domains/types/name_registry/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_events/README.md` & `dipdup-7.0.0rc2/src/demo_events/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
 ```bash
 curl -Lsf https://dipdup.io/install.py | python3
 ```
 
-See the [Installation](https://docs.dipdup.io/installation) page for all options.
+See the [Installation](https://dipdup.io/docs/installation) page for all options.
 
 ## Usage
 
 Run the indexer in-memory:
 
 ```bash
 dipdup run
@@ -27,17 +27,17 @@
 ```bash
 dipdup -c . -c configs/dipdup.sqlite.yml run
 ```
 
 Or spawn a docker-compose stack:
 
 ```bash
-cp deploy/.env.example .env
+cp deploy/.env.default deploy/.env
 # Edit .env before running
-docker-compose -f deploy/docker-compose.yml up
+docker-compose -f deploy/compose.yaml up
 ```
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
```

### Comparing `dipdup-7.0.0rc1/src/demo_events/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc2/src/demo_events/deploy/compose.swarm.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     deploy:
       mode: replicated
       replicas: 1
       placement: *placement
     logging: *logging
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     depends_on:
       - db
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@demo_events_db:5432/dipdup
       - HASURA_GRAPHQL_ADMIN_SECRET=${HASURA_SECRET}
       - HASURA_GRAPHQL_ENABLE_CONSOLE=true
       - HASURA_GRAPHQL_DEV_MODE=false
```

### Comparing `dipdup-7.0.0rc1/src/demo_events/deploy/compose.yaml` & `dipdup-7.0.0rc2/src/demo_events/deploy/compose.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     healthcheck:
       test: ["CMD-SHELL", "pg_isready -U dipdup"]
       interval: 10s
       timeout: 5s
       retries: 5
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     ports:
       - 8080
     depends_on:
       - db
     restart: always
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@db:5432/dipdup
```

### Comparing `dipdup-7.0.0rc1/src/demo_events/dipdup.yaml` & `dipdup-7.0.0rc2/src/demo_events/dipdup.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
-00000020: 6576 656e 7473 0a0a 6461 7461 6261 7365  events..database
-00000030: 3a0a 2020 6b69 6e64 3a20 7371 6c69 7465  :.  kind: sqlite
-00000040: 0a20 2070 6174 683a 2064 656d 6f5f 6576  .  path: demo_ev
-00000050: 656e 7473 2e73 716c 6974 6533 0a0a 6461  ents.sqlite3..da
-00000060: 7461 736f 7572 6365 733a 0a20 2074 7a6b  tasources:.  tzk
-00000070: 743a 0a20 2020 206b 696e 643a 2074 657a  t:.    kind: tez
-00000080: 6f73 2e74 7a6b 740a 2020 2020 7572 6c3a  os.tzkt.    url:
-00000090: 2068 7474 7073 3a2f 2f61 7069 2e67 686f   https://api.gho
-000000a0: 7374 6e65 742e 747a 6b74 2e69 6f0a 0a63  stnet.tzkt.io..c
-000000b0: 6f6e 7472 6163 7473 3a0a 2020 6576 656e  ontracts:.  even
-000000c0: 7473 5f63 6f6e 7472 6163 743a 0a20 2020  ts_contract:.   
-000000d0: 206b 696e 643a 2074 657a 6f73 0a20 2020   kind: tezos.   
-000000e0: 2063 6f64 655f 6861 7368 3a20 4b54 3155   code_hash: KT1U
-000000f0: 7036 414d 6568 7a65 3256 5464 7433 7738  p6AMehze2VTdt3w8
-00000100: 3578 615a 5074 7245 576e 3141 6579 5233  5xaZPtrEWn1AeyR3
-00000110: 0a0a 696e 6465 7865 733a 0a20 2065 7665  ..indexes:.  eve
-00000120: 6e74 733a 0a20 2020 206b 696e 643a 2074  nts:.    kind: t
-00000130: 657a 6f73 2e74 7a6b 742e 6576 656e 7473  ezos.tzkt.events
-00000140: 0a20 2020 2064 6174 6173 6f75 7263 653a  .    datasource:
-00000150: 2074 7a6b 740a 2020 2020 6861 6e64 6c65   tzkt.    handle
-00000160: 7273 3a0a 2020 2020 2020 2d20 6361 6c6c  rs:.      - call
-00000170: 6261 636b 3a20 6f6e 5f6d 6f76 655f 6576  back: on_move_ev
-00000180: 656e 740a 2020 2020 2020 2020 636f 6e74  ent.        cont
-00000190: 7261 6374 3a20 6576 656e 7473 5f63 6f6e  ract: events_con
-000001a0: 7472 6163 740a 2020 2020 2020 2020 7461  tract.        ta
-000001b0: 673a 206d 6f76 650a 2020 2020 2020 2d20  g: move.      - 
-000001c0: 6361 6c6c 6261 636b 3a20 6f6e 5f72 6f6c  callback: on_rol
-000001d0: 6c5f 6576 656e 740a 2020 2020 2020 2020  l_event.        
-000001e0: 636f 6e74 7261 6374 3a20 6576 656e 7473  contract: events
-000001f0: 5f63 6f6e 7472 6163 740a 2020 2020 2020  _contract.      
-00000200: 2020 7461 673a 2072 6f6c 6c0a 2020 2020    tag: roll.    
-00000210: 2020 2d20 6361 6c6c 6261 636b 3a20 6f6e    - callback: on
-00000220: 5f6f 7468 6572 5f65 7665 6e74 0a20 2020  _other_event.   
-00000230: 2020 2020 2063 6f6e 7472 6163 743a 2065       contract: e
-00000240: 7665 6e74 735f 636f 6e74 7261 6374       vents_contract
+00000020: 6576 656e 7473 0a0a 6461 7461 736f 7572  events..datasour
+00000030: 6365 733a 0a20 2074 7a6b 743a 0a20 2020  ces:.  tzkt:.   
+00000040: 206b 696e 643a 2074 657a 6f73 2e74 7a6b   kind: tezos.tzk
+00000050: 740a 2020 2020 7572 6c3a 2068 7474 7073  t.    url: https
+00000060: 3a2f 2f61 7069 2e67 686f 7374 6e65 742e  ://api.ghostnet.
+00000070: 747a 6b74 2e69 6f0a 0a63 6f6e 7472 6163  tzkt.io..contrac
+00000080: 7473 3a0a 2020 6576 656e 7473 5f63 6f6e  ts:.  events_con
+00000090: 7472 6163 743a 0a20 2020 206b 696e 643a  tract:.    kind:
+000000a0: 2074 657a 6f73 0a20 2020 2063 6f64 655f   tezos.    code_
+000000b0: 6861 7368 3a20 4b54 3155 7036 414d 6568  hash: KT1Up6AMeh
+000000c0: 7a65 3256 5464 7433 7738 3578 615a 5074  ze2VTdt3w85xaZPt
+000000d0: 7245 576e 3141 6579 5233 0a0a 696e 6465  rEWn1AeyR3..inde
+000000e0: 7865 733a 0a20 2065 7665 6e74 733a 0a20  xes:.  events:. 
+000000f0: 2020 206b 696e 643a 2074 657a 6f73 2e74     kind: tezos.t
+00000100: 7a6b 742e 6576 656e 7473 0a20 2020 2064  zkt.events.    d
+00000110: 6174 6173 6f75 7263 653a 2074 7a6b 740a  atasource: tzkt.
+00000120: 2020 2020 6861 6e64 6c65 7273 3a0a 2020      handlers:.  
+00000130: 2020 2020 2d20 6361 6c6c 6261 636b 3a20      - callback: 
+00000140: 6f6e 5f6d 6f76 655f 6576 656e 740a 2020  on_move_event.  
+00000150: 2020 2020 2020 636f 6e74 7261 6374 3a20        contract: 
+00000160: 6576 656e 7473 5f63 6f6e 7472 6163 740a  events_contract.
+00000170: 2020 2020 2020 2020 7461 673a 206d 6f76          tag: mov
+00000180: 650a 2020 2020 2020 2d20 6361 6c6c 6261  e.      - callba
+00000190: 636b 3a20 6f6e 5f72 6f6c 6c5f 6576 656e  ck: on_roll_even
+000001a0: 740a 2020 2020 2020 2020 636f 6e74 7261  t.        contra
+000001b0: 6374 3a20 6576 656e 7473 5f63 6f6e 7472  ct: events_contr
+000001c0: 6163 740a 2020 2020 2020 2020 7461 673a  act.        tag:
+000001d0: 2072 6f6c 6c0a 2020 2020 2020 2d20 6361   roll.      - ca
+000001e0: 6c6c 6261 636b 3a20 6f6e 5f6f 7468 6572  llback: on_other
+000001f0: 5f65 7665 6e74 0a20 2020 2020 2020 2063  _event.        c
+00000200: 6f6e 7472 6163 743a 2065 7665 6e74 735f  ontract: events_
+00000210: 636f 6e74 7261 6374                      contract
```

### Comparing `dipdup-7.0.0rc1/src/demo_events/models/__init__.py` & `dipdup-7.0.0rc2/src/demo_events/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_events/pyproject.toml` & `dipdup-7.0.0rc2/src/demo_head/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
-name = "demo_events"
+name = "demo_head"
 version = "0.0.1"
-description = "Processing contract events"
+description = "Processing head block metadata"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc1,<8"
+    "dipdup>=7.0.0rc2,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
@@ -24,17 +24,15 @@
 _isort = "isort ."
 _black = "black ."
 _ruff = "ruff check --fix ."
 _mypy = "mypy ."
 all = { composite = ["fmt", "lint"] }
 fmt = { composite = ["_isort", "_black"] }
 lint = { composite = ["_ruff", "_mypy"] }
-image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_events:latest"
-
-clean = "git clean -xdf --exclude=.venv"
+image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_head:latest"
 
 [tool.isort]
 line_length = 120
 force_single_line = true
 
 [tool.black]
 line-length = 120
```

### Comparing `dipdup-7.0.0rc1/src/demo_evm_events/README.md` & `dipdup-7.0.0rc2/src/demo_uniswap/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# demo_evm_events
+# demo_uniswap
 
-A very basic indexer for USDt transfers
+Uniswap V3 pools, positions, swaps, ticks, etc.
 
 ## Installation
 
 This project is based on [DipDup](https://dipdup.io), a framework for building featureful dapps.
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
 ```bash
 curl -Lsf https://dipdup.io/install.py | python3
 ```
 
-See the [Installation](https://docs.dipdup.io/installation) page for all options.
+See the [Installation](https://dipdup.io/docs/installation) page for all options.
 
 ## Usage
 
 Run the indexer in-memory:
 
 ```bash
 dipdup run
@@ -27,17 +27,17 @@
 ```bash
 dipdup -c . -c configs/dipdup.sqlite.yml run
 ```
 
 Or spawn a docker-compose stack:
 
 ```bash
-cp deploy/.env.example .env
+cp deploy/.env.default deploy/.env
 # Edit .env before running
-docker-compose -f deploy/docker-compose.yml up
+docker-compose -f deploy/compose.yaml up
 ```
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
```

### Comparing `dipdup-7.0.0rc1/src/demo_evm_events/abi/eth_usdt/abi.json` & `dipdup-7.0.0rc2/src/demo_evm_events/abi/eth_usdt/abi.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_evm_events/abi/eth_usdt/events.json` & `dipdup-7.0.0rc2/src/demo_evm_events/abi/eth_usdt/events.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_evm_events/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc2/src/demo_evm_events/deploy/compose.swarm.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     deploy:
       mode: replicated
       replicas: 1
       placement: *placement
     logging: *logging
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     depends_on:
       - db
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@demo_evm_events_db:5432/dipdup
       - HASURA_GRAPHQL_ADMIN_SECRET=${HASURA_SECRET}
       - HASURA_GRAPHQL_ENABLE_CONSOLE=true
       - HASURA_GRAPHQL_DEV_MODE=false
```

### Comparing `dipdup-7.0.0rc1/src/demo_evm_events/deploy/compose.yaml` & `dipdup-7.0.0rc2/src/demo_evm_events/deploy/compose.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     healthcheck:
       test: ["CMD-SHELL", "pg_isready -U dipdup"]
       interval: 10s
       timeout: 5s
       retries: 5
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     ports:
       - 8080
     depends_on:
       - db
     restart: always
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@db:5432/dipdup
```

### Comparing `dipdup-7.0.0rc1/src/demo_evm_events/dipdup.yaml` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_evm_events/dipdup.yaml.j2`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,44 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
-00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
-00000020: 6576 6d5f 6576 656e 7473 0a0a 6461 7461  evm_events..data
-00000030: 6261 7365 3a0a 2020 6b69 6e64 3a20 7371  base:.  kind: sq
-00000040: 6c69 7465 0a20 2070 6174 683a 2064 656d  lite.  path: dem
-00000050: 6f5f 6576 6d5f 6576 656e 7473 2e73 716c  o_evm_events.sql
-00000060: 6974 6533 0a0a 6461 7461 736f 7572 6365  ite3..datasource
-00000070: 733a 0a20 2065 7468 7363 616e 3a0a 2020  s:.  ethscan:.  
-00000080: 2020 6b69 6e64 3a20 6162 692e 6574 6865    kind: abi.ethe
-00000090: 7273 6361 6e0a 0a20 206d 6169 6e6e 6574  rscan..  mainnet
-000000a0: 5f6e 6f64 653a 0a20 2020 206b 696e 643a  _node:.    kind:
-000000b0: 2065 766d 2e6e 6f64 650a 2020 2020 7572   evm.node.    ur
-000000c0: 6c3a 2068 7474 7073 3a2f 2f6d 6169 6e6e  l: https://mainn
-000000d0: 6574 2e69 6e66 7572 612e 696f 2f76 332f  et.infura.io/v3/
-000000e0: 247b 494e 4655 5241 5f4b 4559 3a2d 2727  ${INFURA_KEY:-''
-000000f0: 7d0a 2020 2020 7773 5f75 726c 3a20 7773  }.    ws_url: ws
-00000100: 733a 2f2f 6d61 696e 6e65 742e 696e 6675  s://mainnet.infu
-00000110: 7261 2e69 6f2f 7773 2f76 332f 247b 494e  ra.io/ws/v3/${IN
-00000120: 4655 5241 5f4b 4559 3a2d 2727 7d0a 0a20  FURA_KEY:-''}.. 
-00000130: 206d 6169 6e6e 6574 5f73 7562 7371 7569   mainnet_subsqui
-00000140: 643a 0a20 2020 206b 696e 643a 2065 766d  d:.    kind: evm
-00000150: 2e73 7562 7371 7569 640a 2020 2020 7572  .subsquid.    ur
-00000160: 6c3a 2024 7b41 5243 4849 5645 5f55 524c  l: ${ARCHIVE_URL
-00000170: 3a2d 6874 7470 733a 2f2f 7632 2e61 7263  :-https://v2.arc
-00000180: 6869 7665 2e73 7562 7371 7569 642e 696f  hive.subsquid.io
-00000190: 2f6e 6574 776f 726b 2f65 7468 6572 6575  /network/ethereu
-000001a0: 6d2d 6d61 696e 6e65 747d 0a20 2020 206e  m-mainnet}.    n
-000001b0: 6f64 653a 206d 6169 6e6e 6574 5f6e 6f64  ode: mainnet_nod
-000001c0: 650a 0a63 6f6e 7472 6163 7473 3a0a 2020  e..contracts:.  
-000001d0: 6574 685f 7573 6474 3a0a 2020 2020 6b69  eth_usdt:.    ki
-000001e0: 6e64 3a20 6576 6d0a 2020 2020 6164 6472  nd: evm.    addr
-000001f0: 6573 733a 2030 7864 6163 3137 6639 3538  ess: 0xdac17f958
-00000200: 6432 6565 3532 3361 3232 3036 3230 3639  d2ee523a22062069
-00000210: 3934 3539 3763 3133 6438 3331 6563 370a  94597c13d831ec7.
-00000220: 2020 2020 7479 7065 6e61 6d65 3a20 6574      typename: et
-00000230: 685f 7573 6474 0a0a 696e 6465 7865 733a  h_usdt..indexes:
-00000240: 0a20 2065 7468 5f75 7364 745f 6576 656e  .  eth_usdt_even
-00000250: 7473 3a0a 2020 2020 6b69 6e64 3a20 6576  ts:.    kind: ev
-00000260: 6d2e 7375 6273 7175 6964 2e65 7665 6e74  m.subsquid.event
-00000270: 730a 2020 2020 6461 7461 736f 7572 6365  s.    datasource
-00000280: 3a20 6d61 696e 6e65 745f 7375 6273 7175  : mainnet_subsqu
-00000290: 6964 0a20 2020 2068 616e 646c 6572 733a  id.    handlers:
-000002a0: 0a20 2020 2020 202d 2063 616c 6c62 6163  .      - callbac
-000002b0: 6b3a 206f 6e5f 7472 616e 7366 6572 0a20  k: on_transfer. 
-000002c0: 2020 2020 2020 2063 6f6e 7472 6163 743a         contract:
-000002d0: 2065 7468 5f75 7364 740a 2020 2020 2020   eth_usdt.      
-000002e0: 2020 6e61 6d65 3a20 5472 616e 7366 6572    name: Transfer
+00000010: 300a 7061 636b 6167 653a 207b 7b20 7072  0.package: {{ pr
+00000020: 6f6a 6563 742e 7061 636b 6167 6520 7d7d  oject.package }}
+00000030: 0a0a 6461 7461 736f 7572 6365 733a 0a20  ..datasources:. 
+00000040: 2065 7468 7363 616e 3a0a 2020 2020 6b69   ethscan:.    ki
+00000050: 6e64 3a20 6162 692e 6574 6865 7273 6361  nd: abi.ethersca
+00000060: 6e0a 0a20 206d 6169 6e6e 6574 5f6e 6f64  n..  mainnet_nod
+00000070: 653a 0a20 2020 206b 696e 643a 2065 766d  e:.    kind: evm
+00000080: 2e6e 6f64 650a 2020 2020 7572 6c3a 2068  .node.    url: h
+00000090: 7474 7073 3a2f 2f6d 6169 6e6e 6574 2e69  ttps://mainnet.i
+000000a0: 6e66 7572 612e 696f 2f76 332f 247b 494e  nfura.io/v3/${IN
+000000b0: 4655 5241 5f4b 4559 3a2d 2727 7d0a 2020  FURA_KEY:-''}.  
+000000c0: 2020 7773 5f75 726c 3a20 7773 733a 2f2f    ws_url: wss://
+000000d0: 6d61 696e 6e65 742e 696e 6675 7261 2e69  mainnet.infura.i
+000000e0: 6f2f 7773 2f76 332f 247b 494e 4655 5241  o/ws/v3/${INFURA
+000000f0: 5f4b 4559 3a2d 2727 7d0a 0a20 206d 6169  _KEY:-''}..  mai
+00000100: 6e6e 6574 5f73 7562 7371 7569 643a 0a20  nnet_subsquid:. 
+00000110: 2020 206b 696e 643a 2065 766d 2e73 7562     kind: evm.sub
+00000120: 7371 7569 640a 2020 2020 7572 6c3a 2024  squid.    url: $
+00000130: 7b41 5243 4849 5645 5f55 524c 3a2d 6874  {ARCHIVE_URL:-ht
+00000140: 7470 733a 2f2f 7632 2e61 7263 6869 7665  tps://v2.archive
+00000150: 2e73 7562 7371 7569 642e 696f 2f6e 6574  .subsquid.io/net
+00000160: 776f 726b 2f65 7468 6572 6575 6d2d 6d61  work/ethereum-ma
+00000170: 696e 6e65 747d 0a20 2020 206e 6f64 653a  innet}.    node:
+00000180: 206d 6169 6e6e 6574 5f6e 6f64 650a 0a63   mainnet_node..c
+00000190: 6f6e 7472 6163 7473 3a0a 2020 6574 685f  ontracts:.  eth_
+000001a0: 7573 6474 3a0a 2020 2020 6b69 6e64 3a20  usdt:.    kind: 
+000001b0: 6576 6d0a 2020 2020 6164 6472 6573 733a  evm.    address:
+000001c0: 2030 7864 6163 3137 6639 3538 6432 6565   0xdac17f958d2ee
+000001d0: 3532 3361 3232 3036 3230 3639 3934 3539  523a220620699459
+000001e0: 3763 3133 6438 3331 6563 370a 2020 2020  7c13d831ec7.    
+000001f0: 7479 7065 6e61 6d65 3a20 6574 685f 7573  typename: eth_us
+00000200: 6474 0a0a 696e 6465 7865 733a 0a20 2065  dt..indexes:.  e
+00000210: 7468 5f75 7364 745f 6576 656e 7473 3a0a  th_usdt_events:.
+00000220: 2020 2020 6b69 6e64 3a20 6576 6d2e 7375      kind: evm.su
+00000230: 6273 7175 6964 2e65 7665 6e74 730a 2020  bsquid.events.  
+00000240: 2020 6461 7461 736f 7572 6365 3a20 6d61    datasource: ma
+00000250: 696e 6e65 745f 7375 6273 7175 6964 0a20  innet_subsquid. 
+00000260: 2020 2068 616e 646c 6572 733a 0a20 2020     handlers:.   
+00000270: 2020 202d 2063 616c 6c62 6163 6b3a 206f     - callback: o
+00000280: 6e5f 7472 616e 7366 6572 0a20 2020 2020  n_transfer.     
+00000290: 2020 2063 6f6e 7472 6163 743a 2065 7468     contract: eth
+000002a0: 5f75 7364 740a 2020 2020 2020 2020 6e61  _usdt.        na
+000002b0: 6d65 3a20 5472 616e 7366 6572 0a         me: Transfer.
```

### Comparing `dipdup-7.0.0rc1/src/demo_evm_events/handlers/on_transfer.py` & `dipdup-7.0.0rc2/src/demo_evm_events/handlers/on_transfer.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_evm_events/pyproject.toml` & `dipdup-7.0.0rc2/src/demo_blank/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
-name = "demo_evm_events"
+name = "demo_blank"
 version = "0.0.1"
-description = "A very basic indexer for USDt transfers"
+description = "Empty config for a fresh start"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc1,<8"
+    "dipdup>=7.0.0rc2,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
@@ -24,17 +24,15 @@
 _isort = "isort ."
 _black = "black ."
 _ruff = "ruff check --fix ."
 _mypy = "mypy ."
 all = { composite = ["fmt", "lint"] }
 fmt = { composite = ["_isort", "_black"] }
 lint = { composite = ["_ruff", "_mypy"] }
-image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_evm_events:latest"
-
-clean = "git clean -xdf --exclude=.venv"
+image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_blank:latest"
 
 [tool.isort]
 line_length = 120
 force_single_line = true
 
 [tool.black]
 line-length = 120
```

### Comparing `dipdup-7.0.0rc1/src/demo_factories/README.md` & `dipdup-7.0.0rc2/src/demo_factories/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
 ```bash
 curl -Lsf https://dipdup.io/install.py | python3
 ```
 
-See the [Installation](https://docs.dipdup.io/installation) page for all options.
+See the [Installation](https://dipdup.io/docs/installation) page for all options.
 
 ## Usage
 
 Run the indexer in-memory:
 
 ```bash
 dipdup run
@@ -27,17 +27,17 @@
 ```bash
 dipdup -c . -c configs/dipdup.sqlite.yml run
 ```
 
 Or spawn a docker-compose stack:
 
 ```bash
-cp deploy/.env.example .env
+cp deploy/.env.default deploy/.env
 # Edit .env before running
-docker-compose -f deploy/docker-compose.yml up
+docker-compose -f deploy/compose.yaml up
 ```
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
```

### Comparing `dipdup-7.0.0rc1/src/demo_factories/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc2/src/demo_factories/deploy/compose.swarm.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     deploy:
       mode: replicated
       replicas: 1
       placement: *placement
     logging: *logging
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     depends_on:
       - db
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@demo_factories_db:5432/dipdup
       - HASURA_GRAPHQL_ADMIN_SECRET=${HASURA_SECRET}
       - HASURA_GRAPHQL_ENABLE_CONSOLE=true
       - HASURA_GRAPHQL_DEV_MODE=false
```

### Comparing `dipdup-7.0.0rc1/src/demo_factories/deploy/compose.yaml` & `dipdup-7.0.0rc2/src/demo_token_transfers/deploy/compose.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: demo_factories
+name: demo_token_transfers
 
 services:
   dipdup:
     build:
       context: ..
       dockerfile: deploy/Dockerfile
     restart: always
@@ -30,15 +30,15 @@
     healthcheck:
       test: ["CMD-SHELL", "pg_isready -U dipdup"]
       interval: 10s
       timeout: 5s
       retries: 5
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     ports:
       - 8080
     depends_on:
       - db
     restart: always
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@db:5432/dipdup
```

### Comparing `dipdup-7.0.0rc1/src/demo_factories/dipdup.yaml` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_dao/dipdup.yaml.j2`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
-00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
-00000020: 6661 6374 6f72 6965 730a 0a64 6174 6162  factories..datab
-00000030: 6173 653a 0a20 206b 696e 643a 2073 716c  ase:.  kind: sql
-00000040: 6974 650a 2020 7061 7468 3a20 6465 6d6f  ite.  path: demo
-00000050: 5f66 6163 746f 7269 6573 2e73 716c 6974  _factories.sqlit
-00000060: 6533 0a0a 636f 6e74 7261 6374 733a 0a20  e3..contracts:. 
-00000070: 2072 6567 6973 7472 793a 0a20 2020 206b   registry:.    k
-00000080: 696e 643a 2074 657a 6f73 0a20 2020 2061  ind: tezos.    a
-00000090: 6464 7265 7373 3a20 4b54 3139 4346 334b  ddress: KT19CF3K
-000000a0: 4b72 7664 5737 3774 7446 6f6d 4375 696e  KrvdW77ttFomCuin
-000000b0: 326b 3475 4156 6b72 7959 7168 0a20 2020  2k4uAVkryYqh.   
-000000c0: 2074 7970 656e 616d 653a 2072 6567 6973   typename: regis
-000000d0: 7472 790a 0a64 6174 6173 6f75 7263 6573  try..datasources
-000000e0: 3a0a 2020 747a 6b74 3a0a 2020 2020 6b69  :.  tzkt:.    ki
-000000f0: 6e64 3a20 7465 7a6f 732e 747a 6b74 0a20  nd: tezos.tzkt. 
-00000100: 2020 2075 726c 3a20 247b 545a 4b54 5f55     url: ${TZKT_U
-00000110: 524c 3a2d 6874 7470 733a 2f2f 6170 692e  RL:-https://api.
-00000120: 747a 6b74 2e69 6f7d 0a0a 696e 6465 7865  tzkt.io}..indexe
-00000130: 733a 0a20 2072 6567 6973 7472 795f 6461  s:.  registry_da
-00000140: 6f3a 0a20 2020 206b 696e 643a 2074 657a  o:.    kind: tez
-00000150: 6f73 2e74 7a6b 742e 6f70 6572 6174 696f  os.tzkt.operatio
-00000160: 6e73 0a20 2020 2064 6174 6173 6f75 7263  ns.    datasourc
-00000170: 653a 2074 7a6b 740a 2020 2020 7479 7065  e: tzkt.    type
-00000180: 733a 0a20 2020 2020 202d 2074 7261 6e73  s:.      - trans
-00000190: 6163 7469 6f6e 0a20 2020 2020 202d 206f  action.      - o
-000001a0: 7269 6769 6e61 7469 6f6e 0a20 2020 2068  rigination.    h
-000001b0: 616e 646c 6572 733a 0a20 2020 2020 202d  andlers:.      -
-000001c0: 2063 616c 6c62 6163 6b3a 206f 6e5f 6f72   callback: on_or
-000001d0: 6967 696e 6174 696f 6e0a 2020 2020 2020  igination.      
-000001e0: 2020 7061 7474 6572 6e3a 0a20 2020 2020    pattern:.     
-000001f0: 2020 2020 202d 2074 7970 653a 206f 7269       - type: ori
-00000200: 6769 6e61 7469 6f6e 0a20 2020 2020 2020  gination.       
-00000210: 2020 2020 206f 7269 6769 6e61 7465 645f       originated_
-00000220: 636f 6e74 7261 6374 3a20 7265 6769 7374  contract: regist
-00000230: 7279 0a20 2020 2020 202d 2063 616c 6c62  ry.      - callb
-00000240: 6163 6b3a 206f 6e5f 7072 6f70 6f73 650a  ack: on_propose.
-00000250: 2020 2020 2020 2020 7061 7474 6572 6e3a          pattern:
-00000260: 0a20 2020 2020 2020 2020 202d 2074 7970  .          - typ
-00000270: 653a 2074 7261 6e73 6163 7469 6f6e 0a20  e: transaction. 
-00000280: 2020 2020 2020 2020 2020 2064 6573 7469             desti
-00000290: 6e61 7469 6f6e 3a20 7265 6769 7374 7279  nation: registry
-000002a0: 0a20 2020 2020 2020 2020 2020 2065 6e74  .            ent
-000002b0: 7279 706f 696e 743a 2070 726f 706f 7365  rypoint: propose
+00000010: 300a 7061 636b 6167 653a 207b 7b20 7072  0.package: {{ pr
+00000020: 6f6a 6563 742e 7061 636b 6167 6520 7d7d  oject.package }}
+00000030: 0a0a 636f 6e74 7261 6374 733a 0a20 2072  ..contracts:.  r
+00000040: 6567 6973 7472 793a 0a20 2020 206b 696e  egistry:.    kin
+00000050: 643a 2074 657a 6f73 0a20 2020 2063 6f64  d: tezos.    cod
+00000060: 655f 6861 7368 3a20 4b54 3139 4346 334b  e_hash: KT19CF3K
+00000070: 4b72 7664 5737 3774 7446 6f6d 4375 696e  KrvdW77ttFomCuin
+00000080: 326b 3475 4156 6b72 7959 7168 0a20 2020  2k4uAVkryYqh.   
+00000090: 2074 7970 656e 616d 653a 2072 6567 6973   typename: regis
+000000a0: 7472 790a 0a64 6174 6173 6f75 7263 6573  try..datasources
+000000b0: 3a0a 2020 747a 6b74 3a0a 2020 2020 6b69  :.  tzkt:.    ki
+000000c0: 6e64 3a20 7465 7a6f 732e 747a 6b74 0a20  nd: tezos.tzkt. 
+000000d0: 2020 2075 726c 3a20 247b 545a 4b54 5f55     url: ${TZKT_U
+000000e0: 524c 3a2d 6874 7470 733a 2f2f 6170 692e  RL:-https://api.
+000000f0: 747a 6b74 2e69 6f7d 0a0a 696e 6465 7865  tzkt.io}..indexe
+00000100: 733a 0a20 2072 6567 6973 7472 795f 6461  s:.  registry_da
+00000110: 6f3a 0a20 2020 206b 696e 643a 2074 657a  o:.    kind: tez
+00000120: 6f73 2e74 7a6b 742e 6f70 6572 6174 696f  os.tzkt.operatio
+00000130: 6e73 0a20 2020 2064 6174 6173 6f75 7263  ns.    datasourc
+00000140: 653a 2074 7a6b 740a 2020 2020 7479 7065  e: tzkt.    type
+00000150: 733a 0a20 2020 2020 202d 2074 7261 6e73  s:.      - trans
+00000160: 6163 7469 6f6e 0a20 2020 2020 202d 206f  action.      - o
+00000170: 7269 6769 6e61 7469 6f6e 0a20 2020 2068  rigination.    h
+00000180: 616e 646c 6572 733a 0a20 2020 2020 202d  andlers:.      -
+00000190: 2063 616c 6c62 6163 6b3a 206f 6e5f 6f72   callback: on_or
+000001a0: 6967 696e 6174 696f 6e0a 2020 2020 2020  igination.      
+000001b0: 2020 7061 7474 6572 6e3a 0a20 2020 2020    pattern:.     
+000001c0: 2020 2020 202d 2074 7970 653a 206f 7269       - type: ori
+000001d0: 6769 6e61 7469 6f6e 0a20 2020 2020 2020  gination.       
+000001e0: 2020 2020 206f 7269 6769 6e61 7465 645f       originated_
+000001f0: 636f 6e74 7261 6374 3a20 7265 6769 7374  contract: regist
+00000200: 7279 0a20 2020 2020 202d 2063 616c 6c62  ry.      - callb
+00000210: 6163 6b3a 206f 6e5f 7072 6f70 6f73 650a  ack: on_propose.
+00000220: 2020 2020 2020 2020 7061 7474 6572 6e3a          pattern:
+00000230: 0a20 2020 2020 2020 2020 202d 2074 7970  .          - typ
+00000240: 653a 2074 7261 6e73 6163 7469 6f6e 0a20  e: transaction. 
+00000250: 2020 2020 2020 2020 2020 2064 6573 7469             desti
+00000260: 6e61 7469 6f6e 3a20 7265 6769 7374 7279  nation: registry
+00000270: 0a20 2020 2020 2020 2020 2020 2065 6e74  .            ent
+00000280: 7279 706f 696e 743a 2070 726f 706f 7365  rypoint: propose
+00000290: 0a                                       .
```

### Comparing `dipdup-7.0.0rc1/src/demo_factories/handlers/on_propose.py` & `dipdup-7.0.0rc2/src/demo_factories/handlers/on_propose.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_factories/models/__init__.py` & `dipdup-7.0.0rc2/src/demo_factories/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_factories/pyproject.toml` & `dipdup-7.0.0rc2/src/demo_token_transfers/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
-name = "demo_factories"
+name = "demo_token_transfers"
 version = "0.0.1"
-description = "A very basic indexer for USDt transfers"
+description = "TzBTC FA1.2 token transfers"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc1,<8"
+    "dipdup>=7.0.0rc2,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
@@ -24,17 +24,15 @@
 _isort = "isort ."
 _black = "black ."
 _ruff = "ruff check --fix ."
 _mypy = "mypy ."
 all = { composite = ["fmt", "lint"] }
 fmt = { composite = ["_isort", "_black"] }
 lint = { composite = ["_ruff", "_mypy"] }
-image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_factories:latest"
-
-clean = "git clean -xdf --exclude=.venv"
+image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_token_transfers:latest"
 
 [tool.isort]
 line_length = 120
 force_single_line = true
 
 [tool.black]
 line-length = 120
```

### Comparing `dipdup-7.0.0rc1/src/demo_factories/types/registry/tezos_storage.py` & `dipdup-7.0.0rc2/src/demo_factories/types/registry/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_head/README.md` & `dipdup-7.0.0rc2/src/demo_head/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
 ```bash
 curl -Lsf https://dipdup.io/install.py | python3
 ```
 
-See the [Installation](https://docs.dipdup.io/installation) page for all options.
+See the [Installation](https://dipdup.io/docs/installation) page for all options.
 
 ## Usage
 
 Run the indexer in-memory:
 
 ```bash
 dipdup run
@@ -27,17 +27,17 @@
 ```bash
 dipdup -c . -c configs/dipdup.sqlite.yml run
 ```
 
 Or spawn a docker-compose stack:
 
 ```bash
-cp deploy/.env.example .env
+cp deploy/.env.default deploy/.env
 # Edit .env before running
-docker-compose -f deploy/docker-compose.yml up
+docker-compose -f deploy/compose.yaml up
 ```
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
```

### Comparing `dipdup-7.0.0rc1/src/demo_head/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc2/src/demo_head/deploy/compose.swarm.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     deploy:
       mode: replicated
       replicas: 1
       placement: *placement
     logging: *logging
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     depends_on:
       - db
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@demo_head_db:5432/dipdup
       - HASURA_GRAPHQL_ADMIN_SECRET=${HASURA_SECRET}
       - HASURA_GRAPHQL_ENABLE_CONSOLE=true
       - HASURA_GRAPHQL_DEV_MODE=false
```

### Comparing `dipdup-7.0.0rc1/src/demo_head/deploy/compose.yaml` & `dipdup-7.0.0rc2/src/demo_head/deploy/compose.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     healthcheck:
       test: ["CMD-SHELL", "pg_isready -U dipdup"]
       interval: 10s
       timeout: 5s
       retries: 5
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     ports:
       - 8080
     depends_on:
       - db
     restart: always
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@db:5432/dipdup
```

### Comparing `dipdup-7.0.0rc1/src/demo_head/models/__init__.py` & `dipdup-7.0.0rc2/src/demo_head/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_head/pyproject.toml` & `dipdup-7.0.0rc2/src/demo_dex/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
-name = "demo_head"
+name = "demo_dex"
 version = "0.0.1"
-description = "Processing head block metadata"
+description = "Quipuswap DEX balances and liquidity"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc1,<8"
+    "dipdup>=7.0.0rc2,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
@@ -24,17 +24,15 @@
 _isort = "isort ."
 _black = "black ."
 _ruff = "ruff check --fix ."
 _mypy = "mypy ."
 all = { composite = ["fmt", "lint"] }
 fmt = { composite = ["_isort", "_black"] }
 lint = { composite = ["_ruff", "_mypy"] }
-image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_head:latest"
-
-clean = "git clean -xdf --exclude=.venv"
+image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_dex:latest"
 
 [tool.isort]
 line_length = 120
 force_single_line = true
 
 [tool.black]
 line-length = 120
```

### Comparing `dipdup-7.0.0rc1/src/demo_nft_marketplace/README.md` & `dipdup-7.0.0rc2/src/demo_nft_marketplace/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
 ```bash
 curl -Lsf https://dipdup.io/install.py | python3
 ```
 
-See the [Installation](https://docs.dipdup.io/installation) page for all options.
+See the [Installation](https://dipdup.io/docs/installation) page for all options.
 
 ## Usage
 
 Run the indexer in-memory:
 
 ```bash
 dipdup run
@@ -27,17 +27,17 @@
 ```bash
 dipdup -c . -c configs/dipdup.sqlite.yml run
 ```
 
 Or spawn a docker-compose stack:
 
 ```bash
-cp deploy/.env.example .env
+cp deploy/.env.default deploy/.env
 # Edit .env before running
-docker-compose -f deploy/docker-compose.yml up
+docker-compose -f deploy/compose.yaml up
 ```
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
```

### Comparing `dipdup-7.0.0rc1/src/demo_nft_marketplace/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc2/src/demo_nft_marketplace/deploy/compose.swarm.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     deploy:
       mode: replicated
       replicas: 1
       placement: *placement
     logging: *logging
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     depends_on:
       - db
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@demo_nft_marketplace_db:5432/dipdup
       - HASURA_GRAPHQL_ADMIN_SECRET=${HASURA_SECRET}
       - HASURA_GRAPHQL_ENABLE_CONSOLE=true
       - HASURA_GRAPHQL_DEV_MODE=false
```

### Comparing `dipdup-7.0.0rc1/src/demo_nft_marketplace/deploy/compose.yaml` & `dipdup-7.0.0rc2/src/demo_nft_marketplace/deploy/compose.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     healthcheck:
       test: ["CMD-SHELL", "pg_isready -U dipdup"]
       interval: 10s
       timeout: 5s
       retries: 5
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     ports:
       - 8080
     depends_on:
       - db
     restart: always
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@db:5432/dipdup
```

### Comparing `dipdup-7.0.0rc1/src/demo_nft_marketplace/dipdup.yaml` & `dipdup-7.0.0rc2/src/demo_nft_marketplace/dipdup.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,79 +1,75 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
 00000020: 6e66 745f 6d61 726b 6574 706c 6163 650a  nft_marketplace.
-00000030: 0a64 6174 6162 6173 653a 0a20 206b 696e  .database:.  kin
-00000040: 643a 2073 716c 6974 650a 2020 7061 7468  d: sqlite.  path
-00000050: 3a20 6465 6d6f 5f6e 6674 5f6d 6172 6b65  : demo_nft_marke
-00000060: 7470 6c61 6365 2e73 716c 6974 6533 0a0a  tplace.sqlite3..
-00000070: 6461 7461 736f 7572 6365 733a 0a20 2074  datasources:.  t
-00000080: 7a6b 745f 6d61 696e 6e65 743a 0a20 2020  zkt_mainnet:.   
-00000090: 206b 696e 643a 2074 657a 6f73 2e74 7a6b   kind: tezos.tzk
-000000a0: 740a 2020 2020 7572 6c3a 2024 7b54 5a4b  t.    url: ${TZK
-000000b0: 545f 5552 4c3a 2d68 7474 7073 3a2f 2f61  T_URL:-https://a
-000000c0: 7069 2e74 7a6b 742e 696f 7d0a 0a63 6f6e  pi.tzkt.io}..con
-000000d0: 7472 6163 7473 3a0a 2020 4845 4e5f 6f62  tracts:.  HEN_ob
-000000e0: 6a6b 7473 3a0a 2020 2020 6b69 6e64 3a20  jkts:.    kind: 
-000000f0: 7465 7a6f 730a 2020 2020 6164 6472 6573  tezos.    addres
-00000100: 733a 2024 7b48 454e 5f4f 424a 4b54 533a  s: ${HEN_OBJKTS:
-00000110: 2d4b 5431 524a 3650 626a 4870 7763 334d  -KT1RJ6PbjHpwc3M
-00000120: 3572 7735 7332 4e62 6d65 6677 6275 7762  5rw5s2Nbmefwbuwb
-00000130: 6478 746f 6e7d 0a20 2020 2074 7970 656e  dxton}.    typen
-00000140: 616d 653a 2068 656e 5f6f 626a 6b74 730a  ame: hen_objkts.
-00000150: 2020 4845 4e5f 6d69 6e74 6572 3a0a 2020    HEN_minter:.  
-00000160: 2020 6b69 6e64 3a20 7465 7a6f 730a 2020    kind: tezos.  
-00000170: 2020 6164 6472 6573 733a 2024 7b48 454e    address: ${HEN
-00000180: 5f4d 494e 5445 523a 2d4b 5431 486b 6735  _MINTER:-KT1Hkg5
-00000190: 7165 4e68 6677 704b 5734 6658 7671 3748  qeNhfwpKW4fXvq7H
-000001a0: 475a 4239 7a32 456e 6d43 4341 397d 0a20  GZB9z2EnmCCA9}. 
-000001b0: 2020 2074 7970 656e 616d 653a 2068 656e     typename: hen
-000001c0: 5f6d 696e 7465 720a 0a69 6e64 6578 6573  _minter..indexes
-000001d0: 3a0a 2020 6865 6e5f 6d61 696e 6e65 743a  :.  hen_mainnet:
-000001e0: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
-000001f0: 2e74 7a6b 742e 6f70 6572 6174 696f 6e73  .tzkt.operations
-00000200: 0a20 2020 2064 6174 6173 6f75 7263 653a  .    datasource:
-00000210: 2074 7a6b 745f 6d61 696e 6e65 740a 2020   tzkt_mainnet.  
-00000220: 2020 636f 6e74 7261 6374 733a 0a20 2020    contracts:.   
-00000230: 2020 202d 2048 454e 5f6d 696e 7465 720a     - HEN_minter.
-00000240: 2020 2020 6861 6e64 6c65 7273 3a0a 2020      handlers:.  
-00000250: 2020 2020 2d20 6361 6c6c 6261 636b 3a20      - callback: 
-00000260: 6f6e 5f6d 696e 740a 2020 2020 2020 2020  on_mint.        
-00000270: 7061 7474 6572 6e3a 0a20 2020 2020 2020  pattern:.       
-00000280: 2020 202d 2074 7970 653a 2074 7261 6e73     - type: trans
-00000290: 6163 7469 6f6e 0a20 2020 2020 2020 2020  action.         
-000002a0: 2020 2064 6573 7469 6e61 7469 6f6e 3a20     destination: 
-000002b0: 4845 4e5f 6d69 6e74 6572 0a20 2020 2020  HEN_minter.     
-000002c0: 2020 2020 2020 2065 6e74 7279 706f 696e         entrypoin
-000002d0: 743a 206d 696e 745f 4f42 4a4b 540a 2020  t: mint_OBJKT.  
-000002e0: 2020 2020 2020 2020 2d20 7479 7065 3a20          - type: 
-000002f0: 7472 616e 7361 6374 696f 6e0a 2020 2020  transaction.    
-00000300: 2020 2020 2020 2020 6465 7374 696e 6174          destinat
-00000310: 696f 6e3a 2048 454e 5f6f 626a 6b74 730a  ion: HEN_objkts.
-00000320: 2020 2020 2020 2020 2020 2020 656e 7472              entr
-00000330: 7970 6f69 6e74 3a20 6d69 6e74 0a20 2020  ypoint: mint.   
-00000340: 2020 202d 2063 616c 6c62 6163 6b3a 206f     - callback: o
-00000350: 6e5f 7377 6170 0a20 2020 2020 2020 2070  n_swap.        p
-00000360: 6174 7465 726e 3a0a 2020 2020 2020 2020  attern:.        
-00000370: 2020 2d20 7479 7065 3a20 7472 616e 7361    - type: transa
-00000380: 6374 696f 6e0a 2020 2020 2020 2020 2020  ction.          
-00000390: 2020 6465 7374 696e 6174 696f 6e3a 2048    destination: H
-000003a0: 454e 5f6d 696e 7465 720a 2020 2020 2020  EN_minter.      
-000003b0: 2020 2020 2020 656e 7472 7970 6f69 6e74        entrypoint
-000003c0: 3a20 7377 6170 0a20 2020 2020 202d 2063  : swap.      - c
-000003d0: 616c 6c62 6163 6b3a 206f 6e5f 6361 6e63  allback: on_canc
-000003e0: 656c 5f73 7761 700a 2020 2020 2020 2020  el_swap.        
-000003f0: 7061 7474 6572 6e3a 0a20 2020 2020 2020  pattern:.       
-00000400: 2020 202d 2074 7970 653a 2074 7261 6e73     - type: trans
-00000410: 6163 7469 6f6e 0a20 2020 2020 2020 2020  action.         
-00000420: 2020 2064 6573 7469 6e61 7469 6f6e 3a20     destination: 
-00000430: 4845 4e5f 6d69 6e74 6572 0a20 2020 2020  HEN_minter.     
-00000440: 2020 2020 2020 2065 6e74 7279 706f 696e         entrypoin
-00000450: 743a 2063 616e 6365 6c5f 7377 6170 0a20  t: cancel_swap. 
-00000460: 2020 2020 202d 2063 616c 6c62 6163 6b3a       - callback:
-00000470: 206f 6e5f 636f 6c6c 6563 740a 2020 2020   on_collect.    
-00000480: 2020 2020 7061 7474 6572 6e3a 0a20 2020      pattern:.   
-00000490: 2020 2020 2020 202d 2074 7970 653a 2074         - type: t
-000004a0: 7261 6e73 6163 7469 6f6e 0a20 2020 2020  ransaction.     
-000004b0: 2020 2020 2020 2064 6573 7469 6e61 7469         destinati
-000004c0: 6f6e 3a20 4845 4e5f 6d69 6e74 6572 0a20  on: HEN_minter. 
-000004d0: 2020 2020 2020 2020 2020 2065 6e74 7279             entry
-000004e0: 706f 696e 743a 2063 6f6c 6c65 6374       point: collect
+00000030: 0a64 6174 6173 6f75 7263 6573 3a0a 2020  .datasources:.  
+00000040: 747a 6b74 5f6d 6169 6e6e 6574 3a0a 2020  tzkt_mainnet:.  
+00000050: 2020 6b69 6e64 3a20 7465 7a6f 732e 747a    kind: tezos.tz
+00000060: 6b74 0a20 2020 2075 726c 3a20 247b 545a  kt.    url: ${TZ
+00000070: 4b54 5f55 524c 3a2d 6874 7470 733a 2f2f  KT_URL:-https://
+00000080: 6170 692e 747a 6b74 2e69 6f7d 0a0a 636f  api.tzkt.io}..co
+00000090: 6e74 7261 6374 733a 0a20 2048 454e 5f6f  ntracts:.  HEN_o
+000000a0: 626a 6b74 733a 0a20 2020 206b 696e 643a  bjkts:.    kind:
+000000b0: 2074 657a 6f73 0a20 2020 2061 6464 7265   tezos.    addre
+000000c0: 7373 3a20 247b 4845 4e5f 4f42 4a4b 5453  ss: ${HEN_OBJKTS
+000000d0: 3a2d 4b54 3152 4a36 5062 6a48 7077 6333  :-KT1RJ6PbjHpwc3
+000000e0: 4d35 7277 3573 324e 626d 6566 7762 7577  M5rw5s2Nbmefwbuw
+000000f0: 6264 7874 6f6e 7d0a 2020 2020 7479 7065  bdxton}.    type
+00000100: 6e61 6d65 3a20 6865 6e5f 6f62 6a6b 7473  name: hen_objkts
+00000110: 0a20 2048 454e 5f6d 696e 7465 723a 0a20  .  HEN_minter:. 
+00000120: 2020 206b 696e 643a 2074 657a 6f73 0a20     kind: tezos. 
+00000130: 2020 2061 6464 7265 7373 3a20 247b 4845     address: ${HE
+00000140: 4e5f 4d49 4e54 4552 3a2d 4b54 3148 6b67  N_MINTER:-KT1Hkg
+00000150: 3571 654e 6866 7770 4b57 3466 5876 7137  5qeNhfwpKW4fXvq7
+00000160: 4847 5a42 397a 3245 6e6d 4343 4139 7d0a  HGZB9z2EnmCCA9}.
+00000170: 2020 2020 7479 7065 6e61 6d65 3a20 6865      typename: he
+00000180: 6e5f 6d69 6e74 6572 0a0a 696e 6465 7865  n_minter..indexe
+00000190: 733a 0a20 2068 656e 5f6d 6169 6e6e 6574  s:.  hen_mainnet
+000001a0: 3a0a 2020 2020 6b69 6e64 3a20 7465 7a6f  :.    kind: tezo
+000001b0: 732e 747a 6b74 2e6f 7065 7261 7469 6f6e  s.tzkt.operation
+000001c0: 730a 2020 2020 6461 7461 736f 7572 6365  s.    datasource
+000001d0: 3a20 747a 6b74 5f6d 6169 6e6e 6574 0a20  : tzkt_mainnet. 
+000001e0: 2020 2063 6f6e 7472 6163 7473 3a0a 2020     contracts:.  
+000001f0: 2020 2020 2d20 4845 4e5f 6d69 6e74 6572      - HEN_minter
+00000200: 0a20 2020 2068 616e 646c 6572 733a 0a20  .    handlers:. 
+00000210: 2020 2020 202d 2063 616c 6c62 6163 6b3a       - callback:
+00000220: 206f 6e5f 6d69 6e74 0a20 2020 2020 2020   on_mint.       
+00000230: 2070 6174 7465 726e 3a0a 2020 2020 2020   pattern:.      
+00000240: 2020 2020 2d20 7479 7065 3a20 7472 616e      - type: tran
+00000250: 7361 6374 696f 6e0a 2020 2020 2020 2020  saction.        
+00000260: 2020 2020 6465 7374 696e 6174 696f 6e3a      destination:
+00000270: 2048 454e 5f6d 696e 7465 720a 2020 2020   HEN_minter.    
+00000280: 2020 2020 2020 2020 656e 7472 7970 6f69          entrypoi
+00000290: 6e74 3a20 6d69 6e74 5f4f 424a 4b54 0a20  nt: mint_OBJKT. 
+000002a0: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
+000002b0: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
+000002c0: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
+000002d0: 7469 6f6e 3a20 4845 4e5f 6f62 6a6b 7473  tion: HEN_objkts
+000002e0: 0a20 2020 2020 2020 2020 2020 2065 6e74  .            ent
+000002f0: 7279 706f 696e 743a 206d 696e 740a 2020  rypoint: mint.  
+00000300: 2020 2020 2d20 6361 6c6c 6261 636b 3a20      - callback: 
+00000310: 6f6e 5f73 7761 700a 2020 2020 2020 2020  on_swap.        
+00000320: 7061 7474 6572 6e3a 0a20 2020 2020 2020  pattern:.       
+00000330: 2020 202d 2074 7970 653a 2074 7261 6e73     - type: trans
+00000340: 6163 7469 6f6e 0a20 2020 2020 2020 2020  action.         
+00000350: 2020 2064 6573 7469 6e61 7469 6f6e 3a20     destination: 
+00000360: 4845 4e5f 6d69 6e74 6572 0a20 2020 2020  HEN_minter.     
+00000370: 2020 2020 2020 2065 6e74 7279 706f 696e         entrypoin
+00000380: 743a 2073 7761 700a 2020 2020 2020 2d20  t: swap.      - 
+00000390: 6361 6c6c 6261 636b 3a20 6f6e 5f63 616e  callback: on_can
+000003a0: 6365 6c5f 7377 6170 0a20 2020 2020 2020  cel_swap.       
+000003b0: 2070 6174 7465 726e 3a0a 2020 2020 2020   pattern:.      
+000003c0: 2020 2020 2d20 7479 7065 3a20 7472 616e      - type: tran
+000003d0: 7361 6374 696f 6e0a 2020 2020 2020 2020  saction.        
+000003e0: 2020 2020 6465 7374 696e 6174 696f 6e3a      destination:
+000003f0: 2048 454e 5f6d 696e 7465 720a 2020 2020   HEN_minter.    
+00000400: 2020 2020 2020 2020 656e 7472 7970 6f69          entrypoi
+00000410: 6e74 3a20 6361 6e63 656c 5f73 7761 700a  nt: cancel_swap.
+00000420: 2020 2020 2020 2d20 6361 6c6c 6261 636b        - callback
+00000430: 3a20 6f6e 5f63 6f6c 6c65 6374 0a20 2020  : on_collect.   
+00000440: 2020 2020 2070 6174 7465 726e 3a0a 2020       pattern:.  
+00000450: 2020 2020 2020 2020 2d20 7479 7065 3a20          - type: 
+00000460: 7472 616e 7361 6374 696f 6e0a 2020 2020  transaction.    
+00000470: 2020 2020 2020 2020 6465 7374 696e 6174          destinat
+00000480: 696f 6e3a 2048 454e 5f6d 696e 7465 720a  ion: HEN_minter.
+00000490: 2020 2020 2020 2020 2020 2020 656e 7472              entr
+000004a0: 7970 6f69 6e74 3a20 636f 6c6c 6563 74    ypoint: collect
```

### Comparing `dipdup-7.0.0rc1/src/demo_nft_marketplace/handlers/on_cancel_swap.py` & `dipdup-7.0.0rc2/src/demo_nft_marketplace/handlers/on_cancel_swap.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_nft_marketplace/handlers/on_collect.py` & `dipdup-7.0.0rc2/src/demo_nft_marketplace/handlers/on_collect.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_nft_marketplace/handlers/on_mint.py` & `dipdup-7.0.0rc2/src/demo_nft_marketplace/handlers/on_mint.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_nft_marketplace/handlers/on_swap.py` & `dipdup-7.0.0rc2/src/demo_nft_marketplace/handlers/on_swap.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_nft_marketplace/models/__init__.py` & `dipdup-7.0.0rc2/src/demo_nft_marketplace/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_nft_marketplace/pyproject.toml` & `dipdup-7.0.0rc2/src/demo_nft_marketplace/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc1,<8"
+    "dipdup>=7.0.0rc2,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
@@ -26,16 +26,14 @@
 _ruff = "ruff check --fix ."
 _mypy = "mypy ."
 all = { composite = ["fmt", "lint"] }
 fmt = { composite = ["_isort", "_black"] }
 lint = { composite = ["_ruff", "_mypy"] }
 image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_nft_marketplace:latest"
 
-clean = "git clean -xdf --exclude=.venv"
-
 [tool.isort]
 line_length = 120
 force_single_line = true
 
 [tool.black]
 line-length = 120
 target-version = ['py311']
```

### Comparing `dipdup-7.0.0rc1/src/demo_nft_marketplace/types/hen_minter/tezos_storage.py` & `dipdup-7.0.0rc2/src/demo_nft_marketplace/types/hen_minter/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_nft_marketplace/types/hen_objkts/tezos_storage.py` & `dipdup-7.0.0rc2/src/demo_nft_marketplace/types/hen_objkts/tezos_storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_raw/README.md` & `dipdup-7.0.0rc2/src/demo_raw/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
 ```bash
 curl -Lsf https://dipdup.io/install.py | python3
 ```
 
-See the [Installation](https://docs.dipdup.io/installation) page for all options.
+See the [Installation](https://dipdup.io/docs/installation) page for all options.
 
 ## Usage
 
 Run the indexer in-memory:
 
 ```bash
 dipdup run
@@ -27,17 +27,17 @@
 ```bash
 dipdup -c . -c configs/dipdup.sqlite.yml run
 ```
 
 Or spawn a docker-compose stack:
 
 ```bash
-cp deploy/.env.example .env
+cp deploy/.env.default deploy/.env
 # Edit .env before running
-docker-compose -f deploy/docker-compose.yml up
+docker-compose -f deploy/compose.yaml up
 ```
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
```

### Comparing `dipdup-7.0.0rc1/src/demo_raw/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc2/src/demo_raw/deploy/compose.swarm.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     deploy:
       mode: replicated
       replicas: 1
       placement: *placement
     logging: *logging
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     depends_on:
       - db
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@demo_raw_db:5432/dipdup
       - HASURA_GRAPHQL_ADMIN_SECRET=${HASURA_SECRET}
       - HASURA_GRAPHQL_ENABLE_CONSOLE=true
       - HASURA_GRAPHQL_DEV_MODE=false
```

### Comparing `dipdup-7.0.0rc1/src/demo_raw/deploy/compose.yaml` & `dipdup-7.0.0rc2/src/demo_raw/deploy/compose.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     healthcheck:
       test: ["CMD-SHELL", "pg_isready -U dipdup"]
       interval: 10s
       timeout: 5s
       retries: 5
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     ports:
       - 8080
     depends_on:
       - db
     restart: always
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@db:5432/dipdup
```

### Comparing `dipdup-7.0.0rc1/src/demo_raw/pyproject.toml` & `dipdup-7.0.0rc2/src/demo_raw/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc1,<8"
+    "dipdup>=7.0.0rc2,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
@@ -26,16 +26,14 @@
 _ruff = "ruff check --fix ."
 _mypy = "mypy ."
 all = { composite = ["fmt", "lint"] }
 fmt = { composite = ["_isort", "_black"] }
 lint = { composite = ["_ruff", "_mypy"] }
 image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_raw:latest"
 
-clean = "git clean -xdf --exclude=.venv"
-
 [tool.isort]
 line_length = 120
 force_single_line = true
 
 [tool.black]
 line-length = 120
 target-version = ['py311']
```

### Comparing `dipdup-7.0.0rc1/src/demo_token/README.md` & `dipdup-7.0.0rc2/src/demo_big_maps/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# demo_token
+# demo_big_maps
 
-TzBTC FA1.2 token operations
+Indexing specific big maps
 
 ## Installation
 
 This project is based on [DipDup](https://dipdup.io), a framework for building featureful dapps.
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
 ```bash
 curl -Lsf https://dipdup.io/install.py | python3
 ```
 
-See the [Installation](https://docs.dipdup.io/installation) page for all options.
+See the [Installation](https://dipdup.io/docs/installation) page for all options.
 
 ## Usage
 
 Run the indexer in-memory:
 
 ```bash
 dipdup run
@@ -27,17 +27,17 @@
 ```bash
 dipdup -c . -c configs/dipdup.sqlite.yml run
 ```
 
 Or spawn a docker-compose stack:
 
 ```bash
-cp deploy/.env.example .env
+cp deploy/.env.default deploy/.env
 # Edit .env before running
-docker-compose -f deploy/docker-compose.yml up
+docker-compose -f deploy/compose.yaml up
 ```
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
```

### Comparing `dipdup-7.0.0rc1/src/demo_token/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc2/src/demo_token/deploy/compose.swarm.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     deploy:
       mode: replicated
       replicas: 1
       placement: *placement
     logging: *logging
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     depends_on:
       - db
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@demo_token_db:5432/dipdup
       - HASURA_GRAPHQL_ADMIN_SECRET=${HASURA_SECRET}
       - HASURA_GRAPHQL_ENABLE_CONSOLE=true
       - HASURA_GRAPHQL_DEV_MODE=false
```

### Comparing `dipdup-7.0.0rc1/src/demo_token/deploy/compose.yaml` & `dipdup-7.0.0rc2/src/demo_dex/deploy/compose.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: demo_token
+name: demo_dex
 
 services:
   dipdup:
     build:
       context: ..
       dockerfile: deploy/Dockerfile
     restart: always
@@ -30,15 +30,15 @@
     healthcheck:
       test: ["CMD-SHELL", "pg_isready -U dipdup"]
       interval: 10s
       timeout: 5s
       retries: 5
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     ports:
       - 8080
     depends_on:
       - db
     restart: always
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@db:5432/dipdup
```

### Comparing `dipdup-7.0.0rc1/src/demo_token/dipdup.yaml` & `dipdup-7.0.0rc2/src/demo_token/dipdup.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,46 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
-00000020: 746f 6b65 6e0a 0a64 6174 6162 6173 653a  token..database:
-00000030: 0a20 206b 696e 643a 2073 716c 6974 650a  .  kind: sqlite.
-00000040: 2020 7061 7468 3a20 6465 6d6f 5f74 6f6b    path: demo_tok
-00000050: 656e 2e73 716c 6974 6533 0a0a 636f 6e74  en.sqlite3..cont
-00000060: 7261 6374 733a 0a20 2074 7a62 7463 5f6d  racts:.  tzbtc_m
-00000070: 6169 6e6e 6574 3a0a 2020 2020 6b69 6e64  ainnet:.    kind
-00000080: 3a20 7465 7a6f 730a 2020 2020 6164 6472  : tezos.    addr
-00000090: 6573 733a 204b 5431 5057 7832 6d6e 4475  ess: KT1PWx2mnDu
-000000a0: 656f 6f64 3766 456d 6662 4244 4b78 3144  eood7fEmfbBDKx1D
-000000b0: 3942 416e 6e58 6974 6e0a 2020 2020 7479  9BAnnXitn.    ty
-000000c0: 7065 6e61 6d65 3a20 747a 6274 630a 0a64  pename: tzbtc..d
-000000d0: 6174 6173 6f75 7263 6573 3a0a 2020 747a  atasources:.  tz
-000000e0: 6b74 5f6d 6169 6e6e 6574 3a0a 2020 2020  kt_mainnet:.    
-000000f0: 6b69 6e64 3a20 7465 7a6f 732e 747a 6b74  kind: tezos.tzkt
-00000100: 0a20 2020 2075 726c 3a20 6874 7470 733a  .    url: https:
-00000110: 2f2f 6170 692e 747a 6b74 2e69 6f0a 0a69  //api.tzkt.io..i
-00000120: 6e64 6578 6573 3a0a 2020 747a 6274 635f  ndexes:.  tzbtc_
-00000130: 686f 6c64 6572 735f 6d61 696e 6e65 743a  holders_mainnet:
-00000140: 0a20 2020 2074 656d 706c 6174 653a 2074  .    template: t
-00000150: 7a62 7463 5f68 6f6c 6465 7273 0a20 2020  zbtc_holders.   
-00000160: 2076 616c 7565 733a 0a20 2020 2020 2063   values:.      c
-00000170: 6f6e 7472 6163 743a 2074 7a62 7463 5f6d  ontract: tzbtc_m
-00000180: 6169 6e6e 6574 0a20 2020 2020 2064 6174  ainnet.      dat
-00000190: 6173 6f75 7263 653a 2074 7a6b 745f 6d61  asource: tzkt_ma
-000001a0: 696e 6e65 740a 0a74 656d 706c 6174 6573  innet..templates
-000001b0: 3a0a 2020 747a 6274 635f 686f 6c64 6572  :.  tzbtc_holder
-000001c0: 733a 0a20 2020 206b 696e 643a 2074 657a  s:.    kind: tez
-000001d0: 6f73 2e74 7a6b 742e 6f70 6572 6174 696f  os.tzkt.operatio
-000001e0: 6e73 0a20 2020 2064 6174 6173 6f75 7263  ns.    datasourc
-000001f0: 653a 203c 6461 7461 736f 7572 6365 3e0a  e: <datasource>.
-00000200: 2020 2020 636f 6e74 7261 6374 733a 0a20      contracts:. 
-00000210: 2020 2020 202d 203c 636f 6e74 7261 6374       - <contract
-00000220: 3e0a 2020 2020 6861 6e64 6c65 7273 3a0a  >.    handlers:.
-00000230: 2020 2020 2020 2d20 6361 6c6c 6261 636b        - callback
-00000240: 3a20 6f6e 5f74 7261 6e73 6665 720a 2020  : on_transfer.  
-00000250: 2020 2020 2020 7061 7474 6572 6e3a 0a20        pattern:. 
-00000260: 2020 2020 2020 2020 202d 2064 6573 7469           - desti
-00000270: 6e61 7469 6f6e 3a20 3c63 6f6e 7472 6163  nation: <contrac
-00000280: 743e 0a20 2020 2020 2020 2020 2020 2065  t>.            e
-00000290: 6e74 7279 706f 696e 743a 2074 7261 6e73  ntrypoint: trans
-000002a0: 6665 720a 2020 2020 2020 2d20 6361 6c6c  fer.      - call
-000002b0: 6261 636b 3a20 6f6e 5f6d 696e 740a 2020  back: on_mint.  
-000002c0: 2020 2020 2020 7061 7474 6572 6e3a 0a20        pattern:. 
-000002d0: 2020 2020 2020 2020 202d 2064 6573 7469           - desti
-000002e0: 6e61 7469 6f6e 3a20 3c63 6f6e 7472 6163  nation: <contrac
-000002f0: 743e 0a20 2020 2020 2020 2020 2020 2065  t>.            e
-00000300: 6e74 7279 706f 696e 743a 206d 696e 74    ntrypoint: mint
+00000020: 746f 6b65 6e0a 0a63 6f6e 7472 6163 7473  token..contracts
+00000030: 3a0a 2020 747a 6274 635f 6d61 696e 6e65  :.  tzbtc_mainne
+00000040: 743a 0a20 2020 206b 696e 643a 2074 657a  t:.    kind: tez
+00000050: 6f73 0a20 2020 2061 6464 7265 7373 3a20  os.    address: 
+00000060: 4b54 3150 5778 326d 6e44 7565 6f6f 6437  KT1PWx2mnDueood7
+00000070: 6645 6d66 6242 444b 7831 4439 4241 6e6e  fEmfbBDKx1D9BAnn
+00000080: 5869 746e 0a20 2020 2074 7970 656e 616d  Xitn.    typenam
+00000090: 653a 2074 7a62 7463 0a0a 6461 7461 736f  e: tzbtc..dataso
+000000a0: 7572 6365 733a 0a20 2074 7a6b 745f 6d61  urces:.  tzkt_ma
+000000b0: 696e 6e65 743a 0a20 2020 206b 696e 643a  innet:.    kind:
+000000c0: 2074 657a 6f73 2e74 7a6b 740a 2020 2020   tezos.tzkt.    
+000000d0: 7572 6c3a 2068 7474 7073 3a2f 2f61 7069  url: https://api
+000000e0: 2e74 7a6b 742e 696f 0a0a 696e 6465 7865  .tzkt.io..indexe
+000000f0: 733a 0a20 2074 7a62 7463 5f68 6f6c 6465  s:.  tzbtc_holde
+00000100: 7273 5f6d 6169 6e6e 6574 3a0a 2020 2020  rs_mainnet:.    
+00000110: 7465 6d70 6c61 7465 3a20 747a 6274 635f  template: tzbtc_
+00000120: 686f 6c64 6572 730a 2020 2020 7661 6c75  holders.    valu
+00000130: 6573 3a0a 2020 2020 2020 636f 6e74 7261  es:.      contra
+00000140: 6374 3a20 747a 6274 635f 6d61 696e 6e65  ct: tzbtc_mainne
+00000150: 740a 2020 2020 2020 6461 7461 736f 7572  t.      datasour
+00000160: 6365 3a20 747a 6b74 5f6d 6169 6e6e 6574  ce: tzkt_mainnet
+00000170: 0a0a 7465 6d70 6c61 7465 733a 0a20 2074  ..templates:.  t
+00000180: 7a62 7463 5f68 6f6c 6465 7273 3a0a 2020  zbtc_holders:.  
+00000190: 2020 6b69 6e64 3a20 7465 7a6f 732e 747a    kind: tezos.tz
+000001a0: 6b74 2e6f 7065 7261 7469 6f6e 730a 2020  kt.operations.  
+000001b0: 2020 6461 7461 736f 7572 6365 3a20 3c64    datasource: <d
+000001c0: 6174 6173 6f75 7263 653e 0a20 2020 2063  atasource>.    c
+000001d0: 6f6e 7472 6163 7473 3a0a 2020 2020 2020  ontracts:.      
+000001e0: 2d20 3c63 6f6e 7472 6163 743e 0a20 2020  - <contract>.   
+000001f0: 2068 616e 646c 6572 733a 0a20 2020 2020   handlers:.     
+00000200: 202d 2063 616c 6c62 6163 6b3a 206f 6e5f   - callback: on_
+00000210: 7472 616e 7366 6572 0a20 2020 2020 2020  transfer.       
+00000220: 2070 6174 7465 726e 3a0a 2020 2020 2020   pattern:.      
+00000230: 2020 2020 2d20 6465 7374 696e 6174 696f      - destinatio
+00000240: 6e3a 203c 636f 6e74 7261 6374 3e0a 2020  n: <contract>.  
+00000250: 2020 2020 2020 2020 2020 656e 7472 7970            entryp
+00000260: 6f69 6e74 3a20 7472 616e 7366 6572 0a20  oint: transfer. 
+00000270: 2020 2020 202d 2063 616c 6c62 6163 6b3a       - callback:
+00000280: 206f 6e5f 6d69 6e74 0a20 2020 2020 2020   on_mint.       
+00000290: 2070 6174 7465 726e 3a0a 2020 2020 2020   pattern:.      
+000002a0: 2020 2020 2d20 6465 7374 696e 6174 696f      - destinatio
+000002b0: 6e3a 203c 636f 6e74 7261 6374 3e0a 2020  n: <contract>.  
+000002c0: 2020 2020 2020 2020 2020 656e 7472 7970            entryp
+000002d0: 6f69 6e74 3a20 6d69 6e74                 oint: mint
```

### Comparing `dipdup-7.0.0rc1/src/demo_token/handlers/on_mint.py` & `dipdup-7.0.0rc2/src/demo_token/handlers/on_mint.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_token/handlers/on_transfer.py` & `dipdup-7.0.0rc2/src/demo_token/handlers/on_transfer.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_token/pyproject.toml` & `dipdup-7.0.0rc2/src/demo_domains/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
-name = "demo_token"
+name = "demo_domains"
 version = "0.0.1"
-description = "TzBTC FA1.2 token operations"
+description = "Tezos Domains name service"
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc1,<8"
+    "dipdup>=7.0.0rc2,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
@@ -24,17 +24,15 @@
 _isort = "isort ."
 _black = "black ."
 _ruff = "ruff check --fix ."
 _mypy = "mypy ."
 all = { composite = ["fmt", "lint"] }
 fmt = { composite = ["_isort", "_black"] }
 lint = { composite = ["_ruff", "_mypy"] }
-image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_token:latest"
-
-clean = "git clean -xdf --exclude=.venv"
+image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_domains:latest"
 
 [tool.isort]
 line_length = 120
 force_single_line = true
 
 [tool.black]
 line-length = 120
```

### Comparing `dipdup-7.0.0rc1/src/demo_token_transfers/README.md` & `dipdup-7.0.0rc2/src/demo_token_transfers/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
 ```bash
 curl -Lsf https://dipdup.io/install.py | python3
 ```
 
-See the [Installation](https://docs.dipdup.io/installation) page for all options.
+See the [Installation](https://dipdup.io/docs/installation) page for all options.
 
 ## Usage
 
 Run the indexer in-memory:
 
 ```bash
 dipdup run
@@ -27,17 +27,17 @@
 ```bash
 dipdup -c . -c configs/dipdup.sqlite.yml run
 ```
 
 Or spawn a docker-compose stack:
 
 ```bash
-cp deploy/.env.example .env
+cp deploy/.env.default deploy/.env
 # Edit .env before running
-docker-compose -f deploy/docker-compose.yml up
+docker-compose -f deploy/compose.yaml up
 ```
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
```

### Comparing `dipdup-7.0.0rc1/src/demo_token_transfers/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc2/src/demo_token_transfers/deploy/compose.swarm.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     deploy:
       mode: replicated
       replicas: 1
       placement: *placement
     logging: *logging
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     depends_on:
       - db
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@demo_token_transfers_db:5432/dipdup
       - HASURA_GRAPHQL_ADMIN_SECRET=${HASURA_SECRET}
       - HASURA_GRAPHQL_ENABLE_CONSOLE=true
       - HASURA_GRAPHQL_DEV_MODE=false
```

### Comparing `dipdup-7.0.0rc1/src/demo_token_transfers/deploy/compose.yaml` & `dipdup-7.0.0rc2/src/demo_token/deploy/compose.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: demo_token_transfers
+name: demo_token
 
 services:
   dipdup:
     build:
       context: ..
       dockerfile: deploy/Dockerfile
     restart: always
@@ -30,15 +30,15 @@
     healthcheck:
       test: ["CMD-SHELL", "pg_isready -U dipdup"]
       interval: 10s
       timeout: 5s
       retries: 5
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     ports:
       - 8080
     depends_on:
       - db
     restart: always
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@db:5432/dipdup
```

### Comparing `dipdup-7.0.0rc1/src/demo_token_transfers/handlers/on_balance_update.py` & `dipdup-7.0.0rc2/src/demo_token_transfers/handlers/on_balance_update.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_token_transfers/handlers/on_token_transfer.py` & `dipdup-7.0.0rc2/src/demo_token_transfers/handlers/on_token_transfer.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_token_transfers/pyproject.toml` & `dipdup-7.0.0rc2/src/demo_uniswap/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
-name = "demo_token_transfers"
+name = "demo_uniswap"
 version = "0.0.1"
-description = "TzBTC FA1.2 token transfers"
+description = "Uniswap V3 pools, positions, swaps, ticks, etc."
 license = { text = "MIT" }
 authors = [
     { name = "John Doe", email = "john_doe@example.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc1,<8"
+    "dipdup>=7.0.0rc2,<8"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
@@ -24,17 +24,15 @@
 _isort = "isort ."
 _black = "black ."
 _ruff = "ruff check --fix ."
 _mypy = "mypy ."
 all = { composite = ["fmt", "lint"] }
 fmt = { composite = ["_isort", "_black"] }
 lint = { composite = ["_ruff", "_mypy"] }
-image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_token_transfers:latest"
-
-clean = "git clean -xdf --exclude=.venv"
+image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_uniswap:latest"
 
 [tool.isort]
 line_length = 120
 force_single_line = true
 
 [tool.black]
 line-length = 120
```

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/README.md` & `dipdup-7.0.0rc2/src/demo_evm_events/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# demo_uniswap
+# demo_evm_events
 
-Uniswap V3 pools, positions, swaps, ticks, etc.
+A very basic indexer for USDt transfers
 
 ## Installation
 
 This project is based on [DipDup](https://dipdup.io), a framework for building featureful dapps.
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
 ```bash
 curl -Lsf https://dipdup.io/install.py | python3
 ```
 
-See the [Installation](https://docs.dipdup.io/installation) page for all options.
+See the [Installation](https://dipdup.io/docs/installation) page for all options.
 
 ## Usage
 
 Run the indexer in-memory:
 
 ```bash
 dipdup run
@@ -27,17 +27,17 @@
 ```bash
 dipdup -c . -c configs/dipdup.sqlite.yml run
 ```
 
 Or spawn a docker-compose stack:
 
 ```bash
-cp deploy/.env.example .env
+cp deploy/.env.default deploy/.env
 # Edit .env before running
-docker-compose -f deploy/docker-compose.yml up
+docker-compose -f deploy/compose.yaml up
 ```
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
 
 ```bash
```

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/abi/factory/abi.json` & `dipdup-7.0.0rc2/src/demo_uniswap/abi/factory/abi.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/abi/factory/events.json` & `dipdup-7.0.0rc2/src/demo_uniswap/abi/factory/events.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/abi/pool/abi.json` & `dipdup-7.0.0rc2/src/demo_uniswap/abi/pool/abi.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/abi/pool/events.json` & `dipdup-7.0.0rc2/src/demo_uniswap/abi/pool/events.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/abi/position_manager/abi.json` & `dipdup-7.0.0rc2/src/demo_uniswap/abi/position_manager/abi.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/abi/position_manager/events.json` & `dipdup-7.0.0rc2/src/demo_uniswap/abi/position_manager/events.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/deploy/compose.swarm.yaml` & `dipdup-7.0.0rc2/src/demo_uniswap/deploy/compose.swarm.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     deploy:
       mode: replicated
       replicas: 1
       placement: *placement
     logging: *logging
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: hasura/graphql-engine:v2.30.1
     depends_on:
       - db
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@demo_uniswap_db:5432/dipdup
       - HASURA_GRAPHQL_ADMIN_SECRET=${HASURA_SECRET}
       - HASURA_GRAPHQL_ENABLE_CONSOLE=true
       - HASURA_GRAPHQL_DEV_MODE=false
```

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/deploy/compose.yaml` & `dipdup-7.0.0rc2/src/dipdup/projects/base/deploy/compose.yaml.j2`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: demo_uniswap
+name: {{ project.package }}
 
 services:
   dipdup:
     build:
       context: ..
       dockerfile: deploy/Dockerfile
     restart: always
@@ -12,15 +12,15 @@
       - 9000
     command: ["-c", "dipdup.yaml", "-c", "configs/dipdup.compose.yaml", "run"]
     depends_on:
       - db
       - hasura
 
   db:
-    image: postgres:15
+    image: {{ project.postgresql_image }}
     ports:
       - 5432
     volumes:
       - db:/var/lib/postgresql/data
     restart: always
     env_file: .env
     environment:
@@ -30,15 +30,15 @@
     healthcheck:
       test: ["CMD-SHELL", "pg_isready -U dipdup"]
       interval: 10s
       timeout: 5s
       retries: 5
 
   hasura:
-    image: hasura/graphql-engine:v2.30.0
+    image: {{ project.hasura_image }}
     ports:
       - 8080
     depends_on:
       - db
     restart: always
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@db:5432/dipdup
@@ -47,8 +47,8 @@
       - HASURA_GRAPHQL_DEV_MODE=true
       - HASURA_GRAPHQL_LOG_LEVEL=info
       - HASURA_GRAPHQL_ENABLE_TELEMETRY=false
       - HASURA_GRAPHQL_UNAUTHORIZED_ROLE=user
       - HASURA_GRAPHQL_STRINGIFY_NUMERIC_TYPES=true
 
 volumes:
-  db:
+  db:
```

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/dipdup.yaml` & `dipdup-7.0.0rc2/src/demo_uniswap/dipdup.yaml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/handlers/factory/pool_created.py` & `dipdup-7.0.0rc2/src/demo_uniswap/handlers/factory/pool_created.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/handlers/pool/burn.py` & `dipdup-7.0.0rc2/src/demo_uniswap/handlers/pool/burn.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/handlers/pool/initialize.py` & `dipdup-7.0.0rc2/src/demo_uniswap/handlers/pool/initialize.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/handlers/pool/mint.py` & `dipdup-7.0.0rc2/src/demo_uniswap/handlers/pool/mint.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/handlers/pool/swap.py` & `dipdup-7.0.0rc2/src/demo_uniswap/handlers/pool/swap.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/handlers/position_manager/collect.py` & `dipdup-7.0.0rc2/src/demo_uniswap/handlers/position_manager/collect.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/handlers/position_manager/decrease_liquidity.py` & `dipdup-7.0.0rc2/src/demo_uniswap/handlers/position_manager/decrease_liquidity.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/handlers/position_manager/increase_liquidity.py` & `dipdup-7.0.0rc2/src/demo_uniswap/handlers/position_manager/increase_liquidity.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/handlers/position_manager/transfer.py` & `dipdup-7.0.0rc2/src/demo_uniswap/handlers/position_manager/transfer.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/models/__init__.py` & `dipdup-7.0.0rc2/src/demo_uniswap/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/models/pool.py` & `dipdup-7.0.0rc2/src/demo_uniswap/models/pool.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/models/position.py` & `dipdup-7.0.0rc2/src/demo_uniswap/models/position.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/models/repo.py` & `dipdup-7.0.0rc2/src/demo_uniswap/models/repo.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/models/tick.py` & `dipdup-7.0.0rc2/src/demo_uniswap/models/tick.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/models/token.py` & `dipdup-7.0.0rc2/src/demo_uniswap/models/token.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/demo_uniswap/pyproject.toml` & `dipdup-7.0.0rc2/src/dipdup/projects/base/pyproject.toml.j2`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
-name = "demo_uniswap"
-version = "0.0.1"
-description = "Uniswap V3 pools, positions, swaps, ticks, etc."
-license = { text = "MIT" }
+name = "{{ project.package }}"
+version = "{{ project.version }}"
+description = "{{ project.description }}"
+license = { text = "{{ project.license }}" }
 authors = [
-    { name = "John Doe", email = "john_doe@example.com" }
+    { name = "{{ project.name }}", email = "{{ project.email }}" }
 ]
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 dependencies = [
-    "dipdup>=7.0.0rc1,<8"
+    "dipdup>={{ project.dipdup_version }}.0.0rc1,<{{ project.dipdup_version | int + 1 }}"
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort",
     "black",
     "ruff",
@@ -24,31 +24,29 @@
 _isort = "isort ."
 _black = "black ."
 _ruff = "ruff check --fix ."
 _mypy = "mypy ."
 all = { composite = ["fmt", "lint"] }
 fmt = { composite = ["_isort", "_black"] }
 lint = { composite = ["_ruff", "_mypy"] }
-image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t demo_uniswap:latest"
-
-clean = "git clean -xdf --exclude=.venv"
+image = "docker buildx build . --load --progress plain -f deploy/Dockerfile -t {{ project.package }}:latest"
 
 [tool.isort]
-line_length = 120
+line_length = {{ project.line_length }}
 force_single_line = true
 
 [tool.black]
-line-length = 120
+line-length = {{ project.line_length }}
 target-version = ['py311']
 skip-string-normalization = true
 
 [tool.ruff]
-line-length = 120
+line-length = {{ project.line_length }}
 target-version = 'py311'
 
 [tool.mypy]
 python_version = "3.11"
 plugins = ["pydantic.mypy"]
 
 [build-system]
 requires = ["pdm-backend"]
-build-backend = "pdm.backend"
+build-backend = "pdm.backend"
```

### Comparing `dipdup-7.0.0rc1/src/dipdup/api.py` & `dipdup-7.0.0rc2/src/dipdup/api.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/cli.py` & `dipdup-7.0.0rc2/src/dipdup/cli.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/codegen/__init__.py` & `dipdup-7.0.0rc2/src/dipdup/codegen/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from dipdup.config import DipDupConfig
 from dipdup.datasources import Datasource
 from dipdup.exceptions import FrameworkException
 from dipdup.package import DEFAULT_ENV
 from dipdup.package import KEEP_MARKER
 from dipdup.package import PACKAGE_MARKER
 from dipdup.package import DipDupPackage
+from dipdup.project import render_base
 from dipdup.utils import load_template
 from dipdup.utils import pascal_to_snake
 from dipdup.utils import touch
 from dipdup.utils import write
 from dipdup.yaml import DipDupYAMLConfig
 
 Callback = Callable[..., Awaitable[None]]
@@ -43,14 +44,17 @@
         self._logger = _logger
 
     async def init(
         self,
         force: bool = False,
     ) -> None:
         self._package.create()
+        if replay := self._package.replay:
+            _logger.info('Using replay `%s`', replay)
+            render_base(replay, force)
 
         await self.generate_abi()
         await self.generate_schemas()
         await self._generate_types(force)
 
         await self._generate_models()
         await self.generate_hooks()
```

### Comparing `dipdup-7.0.0rc1/src/dipdup/codegen/evm_subsquid.py` & `dipdup-7.0.0rc2/src/dipdup/codegen/evm_subsquid.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/codegen/tezos_tzkt.py` & `dipdup-7.0.0rc2/src/dipdup/codegen/tezos_tzkt.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/config/__init__.py` & `dipdup-7.0.0rc2/src/dipdup/config/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/config/abi_etherscan.py` & `dipdup-7.0.0rc2/src/dipdup/config/abi_etherscan.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/config/coinbase.py` & `dipdup-7.0.0rc2/src/dipdup/config/coinbase.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/config/evm.py` & `dipdup-7.0.0rc2/src/dipdup/config/evm.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/config/evm_node.py` & `dipdup-7.0.0rc2/src/dipdup/config/evm_node.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/config/evm_subsquid.py` & `dipdup-7.0.0rc2/src/dipdup/config/evm_subsquid.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/config/evm_subsquid_events.py` & `dipdup-7.0.0rc2/src/dipdup/config/evm_subsquid_events.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/config/evm_subsquid_operations.py` & `dipdup-7.0.0rc2/src/dipdup/config/evm_subsquid_operations.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/config/ipfs.py` & `dipdup-7.0.0rc2/src/dipdup/config/ipfs.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/config/tezos.py` & `dipdup-7.0.0rc2/src/dipdup/config/tezos.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/config/tezos_tzkt.py` & `dipdup-7.0.0rc2/src/dipdup/config/tezos_tzkt.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/config/tezos_tzkt_big_maps.py` & `dipdup-7.0.0rc2/src/dipdup/config/tezos_tzkt_big_maps.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/config/tezos_tzkt_events.py` & `dipdup-7.0.0rc2/src/dipdup/config/tezos_tzkt_events.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/config/tezos_tzkt_head.py` & `dipdup-7.0.0rc2/src/dipdup/config/tezos_tzkt_head.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/config/tezos_tzkt_operations.py` & `dipdup-7.0.0rc2/src/dipdup/config/tezos_tzkt_operations.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/config/tezos_tzkt_token_transfers.py` & `dipdup-7.0.0rc2/src/dipdup/config/tezos_tzkt_token_transfers.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/config/tzip_metadata.py` & `dipdup-7.0.0rc2/src/dipdup/config/tzip_metadata.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/context.py` & `dipdup-7.0.0rc2/src/dipdup/context.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/database.py` & `dipdup-7.0.0rc2/src/dipdup/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,19 @@
     url: str,
     models: str | None = None,
     timeout: int = 60,
     decimal_precision: int | None = None,
     unsafe_sqlite: bool = False,
 ) -> AsyncIterator[None]:
     """Initialize Tortoise with internal and project models, close connections when done"""
+    if ':memory' in url:
+        _logger.warning('Using in-memory database; data will be lost on exit')
+    if '/tmp/' in url:
+        _logger.warning('Using tmpfs database; data will be lost on reboot')
+
     model_modules: dict[str, Iterable[str | ModuleType]] = {
         'int_models': ['dipdup.models'],
     }
     if models:
         if not models.endswith('.models'):
             models += '.models'
         model_modules['models'] = [models]
```

### Comparing `dipdup-7.0.0rc1/src/dipdup/datasources/__init__.py` & `dipdup-7.0.0rc2/src/dipdup/datasources/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/datasources/abi_etherscan.py` & `dipdup-7.0.0rc2/src/dipdup/datasources/abi_etherscan.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/datasources/coinbase.py` & `dipdup-7.0.0rc2/src/dipdup/datasources/coinbase.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/datasources/evm_node.py` & `dipdup-7.0.0rc2/src/dipdup/datasources/evm_node.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/datasources/evm_subsquid.py` & `dipdup-7.0.0rc2/src/dipdup/datasources/evm_subsquid.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/datasources/ipfs.py` & `dipdup-7.0.0rc2/src/dipdup/datasources/ipfs.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/datasources/tezos_tzkt.py` & `dipdup-7.0.0rc2/src/dipdup/datasources/tezos_tzkt.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/datasources/tzip_metadata.py` & `dipdup-7.0.0rc2/src/dipdup/datasources/tzip_metadata.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/dipdup.py` & `dipdup-7.0.0rc2/src/dipdup/dipdup.py`

 * *Files 1% similar despite different names*

```diff
@@ -625,18 +625,14 @@
         await self._ctx.fire_hook('on_restart')
 
     async def _set_up_transactions(self, stack: AsyncExitStack) -> None:
         await stack.enter_async_context(self._transactions.register())
 
     async def _set_up_database(self, stack: AsyncExitStack) -> None:
         self._logger.info('Setting up database')
-        database_config = self._config.database
-        if isinstance(database_config, SqliteDatabaseConfig) and database_config.path == ':memory:':
-            self._logger.warning('Using in-memory SQLite database; data will be lost on restart')
-
         await stack.enter_async_context(
             tortoise_wrapper(
                 url=self._config.database.connection_string,
                 models=self._config.package,
                 timeout=self._config.database.connection_timeout,
                 decimal_precision=self._config.advanced.decimal_precision,
                 unsafe_sqlite=self._config.advanced.unsafe_sqlite,
```

### Comparing `dipdup-7.0.0rc1/src/dipdup/env.py` & `dipdup-7.0.0rc2/src/dipdup/env.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/exceptions.py` & `dipdup-7.0.0rc2/src/dipdup/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
     def _help(self) -> str:
         return f"""
             `{self.datasource}` datasource returned an error.
             
             {self.msg}
 
-            See https://docs.dipdup.io/getting-started/datasources
+            See https://dipdup.io/docs/getting-started/datasources
         """
 
 
 @dataclass(repr=False)
 class InvalidRequestError(Error):
     """API returned an unexpected response"""
 
@@ -110,15 +110,15 @@
 
     msg: str
 
     def _help(self) -> str:
         return f"""
             {self.msg}
 
-            See https://docs.dipdup.io/getting-started/config
+            See https://dipdup.io/docs/getting-started/config
         """
 
 
 @dataclass(repr=False)
 class InvalidModelsError(Error):
     """Can't initialize database, `models.py` module is invalid"""
 
@@ -130,15 +130,15 @@
         return f"""
             {self.msg}
 
               model: `{self.model._meta._model.__name__}`
               table: `{self.model._meta.db_table}`
               field: `{self.field or ''}`
 
-            See https://docs.dipdup.io/getting-started/models
+            See https://dipdup.io/docs/getting-started/models
         """
 
 
 @dataclass(repr=False)
 class ReindexingRequiredError(Error):
     """Unable to continue indexing with existing database"""
 
@@ -156,15 +156,15 @@
             Reindexing required! Reason: {reason}.
               {context}
             You may want to backup database before proceeding. After that perform one of the following actions:
 
               - Eliminate the cause of reindexing and run `dipdup schema approve`.
               - Drop database and start indexing from scratch with `dipdup schema wipe` command.
 
-            See https://docs.dipdup.io/advanced/reindexing for more information.
+            See https://dipdup.io/docs/advanced/reindexing for more information.
         """.format(
             reason=self.reason.value,
             context=context,
         )
 
 
 @dataclass(repr=False)
@@ -282,16 +282,16 @@
 
               argument: `{self.arg}`
               type: {self.type_}
               expected type: {self.expected_type}
 
             Make sure to set correct typenames in config and run `dipdup init --force` to regenerate typeclasses.
 
-            See https://docs.dipdup.io/getting-started/package
-            See https://docs.dipdup.io/references/cli#init
+            See https://dipdup.io/docs/getting-started/package
+            See https://dipdup.io/docs/references/cli#init
         """
 
 
 @dataclass(repr=False)
 class HasuraError(Error):
     """Failed to configure Hasura instance"""
 
@@ -301,15 +301,15 @@
         return f"""
             Failed to configure Hasura:
 
               {self.msg}
 
             If it's `400 Bad Request`, check out Hasura logs for more information.
 
-            See https://docs.dipdup.io/graphql/hasura
+            See https://dipdup.io/docs/graphql/hasura
         """
 
 
 @dataclass(repr=False)
 class UnsupportedAPIError(Error):
     """Datasource instance runs an unsupported software version"""
```

### Comparing `dipdup-7.0.0rc1/src/dipdup/fetcher.py` & `dipdup-7.0.0rc2/src/dipdup/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/fields.py` & `dipdup-7.0.0rc2/src/dipdup/fields.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/hasura.py` & `dipdup-7.0.0rc2/src/dipdup/hasura.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/http.py` & `dipdup-7.0.0rc2/src/dipdup/http.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/index.py` & `dipdup-7.0.0rc2/src/dipdup/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/indexes/evm_subsquid_events/fetcher.py` & `dipdup-7.0.0rc2/src/dipdup/indexes/evm_subsquid_events/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/indexes/evm_subsquid_events/index.py` & `dipdup-7.0.0rc2/src/dipdup/indexes/evm_subsquid_events/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/indexes/evm_subsquid_events/matcher.py` & `dipdup-7.0.0rc2/src/dipdup/indexes/evm_subsquid_events/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_big_maps/fetcher.py` & `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_big_maps/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_big_maps/index.py` & `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_big_maps/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_big_maps/matcher.py` & `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_big_maps/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_events/fetcher.py` & `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_events/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_events/index.py` & `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_events/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_events/matcher.py` & `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_events/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_head/index.py` & `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_head/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_operations/fetcher.py` & `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_operations/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_operations/index.py` & `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_operations/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_operations/matcher.py` & `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_operations/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_operations/parser.py` & `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_operations/parser.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_token_transfers/fetcher.py` & `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_token_transfers/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_token_transfers/index.py` & `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_token_transfers/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_token_transfers/matcher.py` & `dipdup-7.0.0rc2/src/dipdup/indexes/tezos_tzkt_token_transfers/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/install.py` & `dipdup-7.0.0rc2/src/dipdup/install.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
        / __ \ (_)____   / __ \ __  __ ____ 
       / / / // // __ \ / / / // / / // __ \\
      / /_/ // // /_/ // /_/ // /_/ // /_/ /
     /_____//_// .___//_____/ \__,_// .___/ 
              /_/                  /_/      
 """
 EPILOG = """\0
-Documentation:         https://docs.dipdup.io
+Documentation:         https://dipdup.io/docs
 GitHub:                https://github.com/dipdup-io/dipdup
 Discord:               https://discord.gg/NbANhqCJHA
 """
 
 
 class Colors:
     """ANSI color codes"""
@@ -163,15 +163,15 @@
 ) -> None:
     """Install DipDup and its dependencies with pipx"""
     if ref and path:
         fail('Specify either ref or path, not both')
 
     if not any((version, ref, path)):
         # FIXME: Temporary, remove when 7.0.0 is released
-        version = '7.0.0rc1'
+        version = '7.0.0rc2'
 
     env = DipDupEnvironment()
     env.prepare()
     if not quiet:
         env.print()
 
     force_str = '--force' if force else ''
```

### Comparing `dipdup-7.0.0rc1/src/dipdup/models/__init__.py` & `dipdup-7.0.0rc2/src/dipdup/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/models/coinbase.py` & `dipdup-7.0.0rc2/src/dipdup/models/coinbase.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/models/evm_node.py` & `dipdup-7.0.0rc2/src/dipdup/models/evm_node.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/models/evm_subsquid.py` & `dipdup-7.0.0rc2/src/dipdup/models/evm_subsquid.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/models/tezos_tzkt.py` & `dipdup-7.0.0rc2/src/dipdup/models/tezos_tzkt.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/package.py` & `dipdup-7.0.0rc2/src/dipdup/package.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import logging
 from collections import deque
+from contextlib import suppress
 from pathlib import Path
 from typing import Any
 from typing import Awaitable
 from typing import Callable
 from typing import cast
 
 import orjson
 from pydantic import BaseModel
 from pydantic.dataclasses import dataclass
 
 from dipdup.exceptions import ProjectImportError
+from dipdup.project import Answers
+from dipdup.project import answers_from_replay
 from dipdup.utils import import_from
 from dipdup.utils import import_submodules
 from dipdup.utils import pascal_to_snake
 from dipdup.utils import touch
 
 KEEP_MARKER = '.keep'
 PACKAGE_MARKER = '__init__.py'
@@ -74,21 +77,29 @@
         self.types = root / 'types'
 
         # NOTE: Shared directories; not a part of package
         self._xdg_shared_dir = Path.home() / '.local' / 'share' / 'dipdup'
         self.schemas = self._xdg_shared_dir / 'schemas' / self.name
 
         # NOTE: Finally, internal in-memory stuff
+        self._replay: Answers | None = None
         self._callbacks: dict[str, Callable[..., Awaitable[Any]]] = {}
         self._types: dict[str, type[BaseModel]] = {}
         self._evm_abis: dict[str, dict[str, dict[str, Any]]] = {}
         self._evm_events: dict[str, dict[str, EventAbiExtra]] = {}
         self._evm_topics: dict[str, dict[str, str]] = {}
 
     @property
+    def replay(self) -> Answers | None:
+        if not self._replay:
+            with suppress(Exception):
+                self._replay = answers_from_replay(self.root / 'configs' / 'replay.yaml')
+        return self._replay
+
+    @property
     def skel(self) -> dict[Path, str | None]:
         return {
             # NOTE: Package sections
             self.abi: '**/*.json',
             self.configs: '**/*.y[a]ml',
             self.deploy: '**/*[Dockerfile|.env.default|yml|yaml]',
             self.graphql: '**/*.graphql',
```

### Comparing `dipdup-7.0.0rc1/src/dipdup/performance.py` & `dipdup-7.0.0rc2/src/dipdup/performance.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/project.py` & `dipdup-7.0.0rc2/src/dipdup/project.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import asyncclick as cl
 import survey  # type: ignore[import]
 from pydantic.dataclasses import dataclass
 from tabulate import tabulate
 
 from dipdup import __version__
+from dipdup.env import get_package_path
 from dipdup.utils import load_template
 from dipdup.utils import write
 from dipdup.yaml import DipDupYAMLConfig
 
 _logger = logging.getLogger(__name__)
 
 
@@ -78,15 +79,15 @@
     version='0.0.1',
     description='A blockchain indexer built with DipDup',
     license='MIT',
     name='John Doe',
     email='john_doe@example.com',
     postgresql_image='postgres:15',
     # TODO: fetch latest from GH
-    hasura_image='hasura/graphql-engine:v2.30.0',
+    hasura_image='hasura/graphql-engine:v2.30.1',
     line_length='120',
 )
 
 
 def prompt_anyof(
     question: str,
     options: tuple[str, ...],
@@ -245,32 +246,49 @@
         answers,
         template_path=Path(__file__).parent / 'templates' / 'replay.yaml.j2',
         output_path=Path(answers['package']) / 'configs' / 'replay.yaml',
         force=force,
     )
 
 
-def _render_templates(answers: Answers, path: Path, force: bool = False) -> None:
+def render_base(
+    answers: Answers,
+    force: bool = False,
+) -> None:
+    """Render base from template"""
+    # NOTE: Common base
+    _render_templates(answers, Path('base'), force, refresh=True)
+
+    _render(
+        answers,
+        template_path=Path(__file__).parent / 'templates' / 'replay.yaml.j2',
+        output_path=Path('configs') / 'replay.yaml',
+        force=force,
+    )
+
+
+def _render_templates(answers: Answers, path: Path, force: bool = False, refresh: bool = False) -> None:
     from jinja2 import Template
 
     project_path = Path(__file__).parent / 'projects' / path
     project_paths = project_path.glob('**/*.j2')
 
     for path in project_paths:
         template_path = path.relative_to(Path(__file__).parent)
+        output_base = get_package_path(answers['package']) if refresh else Path(answers['package'])
         output_path = Path(
-            answers['package'],
+            output_base,
             *path.relative_to(project_path).parts,
             # NOTE: Remove ".j2" from extension
         ).with_suffix(path.suffix[:-3])
         output_path = Path(Template(str(output_path)).render(project=answers))
         _render(answers, template_path, output_path, force)
 
 
 def _render(answers: Answers, template_path: Path, output_path: Path, force: bool) -> None:
     if output_path.exists() and not force:
-        _logger.warning('File `%s` already exists, skipping', output_path)
+        _logger.info('File `%s` already exists, skipping', output_path)
 
     _logger.info('Generating `%s`', output_path)
     template = load_template(str(template_path))
     content = template.render(project=answers)
     write(output_path, content, overwrite=force)
```

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/base/README.md.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/base/README.md.j2`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 You need a Linux/macOS system with Python 3.11 installed. Use our installer for easy setup:
 
 ```bash
 curl -Lsf https://dipdup.io/install.py | python3
 ```
 
-See the [Installation](https://docs.dipdup.io/installation) page for all options.
+See the [Installation](https://dipdup.io/docs/installation) page for all options.
 
 ## Usage
 
 Run the indexer in-memory:
 
 ```bash
 dipdup run
@@ -27,15 +27,15 @@
 ```bash
 dipdup -c . -c configs/dipdup.sqlite.yml run
 ```
 
 Or spawn a docker-compose stack:
 
 ```bash
-cp deploy/.env.example deploy/.env
+cp deploy/.env.default deploy/.env
 # Edit .env before running
 docker-compose -f deploy/compose.yaml up
 ```
 
 ## Development setup
 
 We recommend [PDM](https://pdm.fming.dev/latest/) for managing Python projects. To set up the development environment:
```

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/base/deploy/compose.swarm.yaml.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/base/deploy/compose.swarm.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/base/deploy/compose.yaml.j2` & `dipdup-7.0.0rc2/src/demo_factories/deploy/compose.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: {{ project.package }}
+name: demo_factories
 
 services:
   dipdup:
     build:
       context: ..
       dockerfile: deploy/Dockerfile
     restart: always
@@ -12,15 +12,15 @@
       - 9000
     command: ["-c", "dipdup.yaml", "-c", "configs/dipdup.compose.yaml", "run"]
     depends_on:
       - db
       - hasura
 
   db:
-    image: {{ project.postgresql_image }}
+    image: postgres:15
     ports:
       - 5432
     volumes:
       - db:/var/lib/postgresql/data
     restart: always
     env_file: .env
     environment:
@@ -30,15 +30,15 @@
     healthcheck:
       test: ["CMD-SHELL", "pg_isready -U dipdup"]
       interval: 10s
       timeout: 5s
       retries: 5
 
   hasura:
-    image: {{ project.hasura_image }}
+    image: hasura/graphql-engine:v2.30.1
     ports:
       - 8080
     depends_on:
       - db
     restart: always
     environment:
       - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@db:5432/dipdup
@@ -47,8 +47,8 @@
       - HASURA_GRAPHQL_DEV_MODE=true
       - HASURA_GRAPHQL_LOG_LEVEL=info
       - HASURA_GRAPHQL_ENABLE_TELEMETRY=false
       - HASURA_GRAPHQL_UNAUTHORIZED_ROLE=user
       - HASURA_GRAPHQL_STRINGIFY_NUMERIC_TYPES=true
 
 volumes:
-  db:
+  db:
```

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_auction/dipdup.yaml.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_auction/dipdup.yaml.j2`

 * *Files 4% similar despite different names*

```diff
@@ -1,72 +1,68 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 207b 7b20 7072  0.package: {{ pr
 00000020: 6f6a 6563 742e 7061 636b 6167 6520 7d7d  oject.package }}
-00000030: 0a0a 6461 7461 6261 7365 3a0a 2020 6b69  ..database:.  ki
-00000040: 6e64 3a20 7371 6c69 7465 0a20 2070 6174  nd: sqlite.  pat
-00000050: 683a 207b 7b20 7072 6f6a 6563 742e 7061  h: {{ project.pa
-00000060: 636b 6167 6520 7d7d 2e73 716c 6974 6533  ckage }}.sqlite3
-00000070: 0a0a 636f 6e74 7261 6374 733a 0a20 2074  ..contracts:.  t
-00000080: 7a63 6f6c 6f72 735f 6d69 6e74 6572 3a0a  zcolors_minter:.
-00000090: 2020 2020 6b69 6e64 3a20 7465 7a6f 730a      kind: tezos.
-000000a0: 2020 2020 6164 6472 6573 733a 204b 5431      address: KT1
-000000b0: 4679 6144 7169 4d51 5767 3745 786f 3756  FyaDqiMQWg7Exo7V
-000000c0: 5569 5841 675a 6264 326b 437a 6f33 6434  UiXAgZbd2kCzo3d4
-000000d0: 730a 2020 2020 7479 7065 6e61 6d65 3a20  s.    typename: 
-000000e0: 747a 636f 6c6f 7273 5f6d 696e 7465 720a  tzcolors_minter.
-000000f0: 2020 747a 636f 6c6f 7273 5f61 7563 7469    tzcolors_aucti
-00000100: 6f6e 3a0a 2020 2020 6b69 6e64 3a20 7465  on:.    kind: te
-00000110: 7a6f 730a 2020 2020 6164 6472 6573 733a  zos.    address:
-00000120: 204b 5431 4370 6553 514b 646b 6857 6934   KT1CpeSQKdkhWi4
-00000130: 7069 6e59 6373 6543 464b 6d44 6873 354d  pinYcseCFKmDhs5M
-00000140: 3734 426b 550a 2020 2020 7479 7065 6e61  74BkU.    typena
-00000150: 6d65 3a20 747a 636f 6c6f 7273 5f61 7563  me: tzcolors_auc
-00000160: 7469 6f6e 0a0a 6461 7461 736f 7572 6365  tion..datasource
-00000170: 733a 0a20 2074 7a6b 743a 0a20 2020 206b  s:.  tzkt:.    k
-00000180: 696e 643a 2074 657a 6f73 2e74 7a6b 740a  ind: tezos.tzkt.
-00000190: 2020 2020 7572 6c3a 2024 7b54 5a4b 545f      url: ${TZKT_
-000001a0: 5552 4c3a 2d68 7474 7073 3a2f 2f61 7069  URL:-https://api
-000001b0: 2e74 7a6b 742e 696f 7d0a 0a74 656d 706c  .tzkt.io}..templ
-000001c0: 6174 6573 3a0a 2020 6175 6374 696f 6e3a  ates:.  auction:
-000001d0: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
-000001e0: 2e74 7a6b 742e 6f70 6572 6174 696f 6e73  .tzkt.operations
-000001f0: 0a20 2020 2064 6174 6173 6f75 7263 653a  .    datasource:
-00000200: 203c 6461 7461 736f 7572 6365 3e0a 2020   <datasource>.  
-00000210: 2020 636f 6e74 7261 6374 733a 0a20 2020    contracts:.   
-00000220: 2020 202d 203c 6175 6374 696f 6e3e 0a20     - <auction>. 
-00000230: 2020 2068 616e 646c 6572 733a 0a20 2020     handlers:.   
-00000240: 2020 202d 2063 616c 6c62 6163 6b3a 206f     - callback: o
-00000250: 6e5f 6372 6561 7465 5f61 7563 7469 6f6e  n_create_auction
-00000260: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
-00000270: 3a0a 2020 2020 2020 2020 2020 2d20 7479  :.          - ty
-00000280: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
-00000290: 2020 2020 2020 2020 2020 2020 6465 7374              dest
-000002a0: 696e 6174 696f 6e3a 203c 6175 6374 696f  ination: <auctio
-000002b0: 6e3e 0a20 2020 2020 2020 2020 2020 2065  n>.            e
-000002c0: 6e74 7279 706f 696e 743a 2063 7265 6174  ntrypoint: creat
-000002d0: 655f 6175 6374 696f 6e0a 2020 2020 2020  e_auction.      
-000002e0: 2d20 6361 6c6c 6261 636b 3a20 6f6e 5f62  - callback: on_b
-000002f0: 6964 0a20 2020 2020 2020 2070 6174 7465  id.        patte
-00000300: 726e 3a0a 2020 2020 2020 2020 2020 2d20  rn:.          - 
-00000310: 7479 7065 3a20 7472 616e 7361 6374 696f  type: transactio
-00000320: 6e0a 2020 2020 2020 2020 2020 2020 6465  n.            de
-00000330: 7374 696e 6174 696f 6e3a 203c 6175 6374  stination: <auct
-00000340: 696f 6e3e 0a20 2020 2020 2020 2020 2020  ion>.           
-00000350: 2065 6e74 7279 706f 696e 743a 2062 6964   entrypoint: bid
-00000360: 0a20 2020 2020 202d 2063 616c 6c62 6163  .      - callbac
-00000370: 6b3a 206f 6e5f 7769 7468 6472 6177 0a20  k: on_withdraw. 
-00000380: 2020 2020 2020 2070 6174 7465 726e 3a0a         pattern:.
-00000390: 2020 2020 2020 2020 2020 2d20 7479 7065            - type
-000003a0: 3a20 7472 616e 7361 6374 696f 6e0a 2020  : transaction.  
-000003b0: 2020 2020 2020 2020 2020 6465 7374 696e            destin
-000003c0: 6174 696f 6e3a 203c 6175 6374 696f 6e3e  ation: <auction>
-000003d0: 0a20 2020 2020 2020 2020 2020 2065 6e74  .            ent
-000003e0: 7279 706f 696e 743a 2077 6974 6864 7261  rypoint: withdra
-000003f0: 770a 0a69 6e64 6578 6573 3a0a 2020 747a  w..indexes:.  tz
-00000400: 636f 6c6f 7273 3a0a 2020 2020 7465 6d70  colors:.    temp
-00000410: 6c61 7465 3a20 6175 6374 696f 6e0a 2020  late: auction.  
-00000420: 2020 7661 6c75 6573 3a0a 2020 2020 2020    values:.      
-00000430: 6461 7461 736f 7572 6365 3a20 747a 6b74  datasource: tzkt
-00000440: 0a20 2020 2020 206d 696e 7465 723a 2074  .      minter: t
-00000450: 7a63 6f6c 6f72 735f 6d69 6e74 6572 0a20  zcolors_minter. 
-00000460: 2020 2020 2061 7563 7469 6f6e 3a20 747a       auction: tz
-00000470: 636f 6c6f 7273 5f61 7563 7469 6f6e 0a    colors_auction.
+00000030: 0a0a 636f 6e74 7261 6374 733a 0a20 2074  ..contracts:.  t
+00000040: 7a63 6f6c 6f72 735f 6d69 6e74 6572 3a0a  zcolors_minter:.
+00000050: 2020 2020 6b69 6e64 3a20 7465 7a6f 730a      kind: tezos.
+00000060: 2020 2020 6164 6472 6573 733a 204b 5431      address: KT1
+00000070: 4679 6144 7169 4d51 5767 3745 786f 3756  FyaDqiMQWg7Exo7V
+00000080: 5569 5841 675a 6264 326b 437a 6f33 6434  UiXAgZbd2kCzo3d4
+00000090: 730a 2020 2020 7479 7065 6e61 6d65 3a20  s.    typename: 
+000000a0: 747a 636f 6c6f 7273 5f6d 696e 7465 720a  tzcolors_minter.
+000000b0: 2020 747a 636f 6c6f 7273 5f61 7563 7469    tzcolors_aucti
+000000c0: 6f6e 3a0a 2020 2020 6b69 6e64 3a20 7465  on:.    kind: te
+000000d0: 7a6f 730a 2020 2020 6164 6472 6573 733a  zos.    address:
+000000e0: 204b 5431 4370 6553 514b 646b 6857 6934   KT1CpeSQKdkhWi4
+000000f0: 7069 6e59 6373 6543 464b 6d44 6873 354d  pinYcseCFKmDhs5M
+00000100: 3734 426b 550a 2020 2020 7479 7065 6e61  74BkU.    typena
+00000110: 6d65 3a20 747a 636f 6c6f 7273 5f61 7563  me: tzcolors_auc
+00000120: 7469 6f6e 0a0a 6461 7461 736f 7572 6365  tion..datasource
+00000130: 733a 0a20 2074 7a6b 743a 0a20 2020 206b  s:.  tzkt:.    k
+00000140: 696e 643a 2074 657a 6f73 2e74 7a6b 740a  ind: tezos.tzkt.
+00000150: 2020 2020 7572 6c3a 2024 7b54 5a4b 545f      url: ${TZKT_
+00000160: 5552 4c3a 2d68 7474 7073 3a2f 2f61 7069  URL:-https://api
+00000170: 2e74 7a6b 742e 696f 7d0a 0a74 656d 706c  .tzkt.io}..templ
+00000180: 6174 6573 3a0a 2020 6175 6374 696f 6e3a  ates:.  auction:
+00000190: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
+000001a0: 2e74 7a6b 742e 6f70 6572 6174 696f 6e73  .tzkt.operations
+000001b0: 0a20 2020 2064 6174 6173 6f75 7263 653a  .    datasource:
+000001c0: 203c 6461 7461 736f 7572 6365 3e0a 2020   <datasource>.  
+000001d0: 2020 636f 6e74 7261 6374 733a 0a20 2020    contracts:.   
+000001e0: 2020 202d 203c 6175 6374 696f 6e3e 0a20     - <auction>. 
+000001f0: 2020 2068 616e 646c 6572 733a 0a20 2020     handlers:.   
+00000200: 2020 202d 2063 616c 6c62 6163 6b3a 206f     - callback: o
+00000210: 6e5f 6372 6561 7465 5f61 7563 7469 6f6e  n_create_auction
+00000220: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
+00000230: 3a0a 2020 2020 2020 2020 2020 2d20 7479  :.          - ty
+00000240: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
+00000250: 2020 2020 2020 2020 2020 2020 6465 7374              dest
+00000260: 696e 6174 696f 6e3a 203c 6175 6374 696f  ination: <auctio
+00000270: 6e3e 0a20 2020 2020 2020 2020 2020 2065  n>.            e
+00000280: 6e74 7279 706f 696e 743a 2063 7265 6174  ntrypoint: creat
+00000290: 655f 6175 6374 696f 6e0a 2020 2020 2020  e_auction.      
+000002a0: 2d20 6361 6c6c 6261 636b 3a20 6f6e 5f62  - callback: on_b
+000002b0: 6964 0a20 2020 2020 2020 2070 6174 7465  id.        patte
+000002c0: 726e 3a0a 2020 2020 2020 2020 2020 2d20  rn:.          - 
+000002d0: 7479 7065 3a20 7472 616e 7361 6374 696f  type: transactio
+000002e0: 6e0a 2020 2020 2020 2020 2020 2020 6465  n.            de
+000002f0: 7374 696e 6174 696f 6e3a 203c 6175 6374  stination: <auct
+00000300: 696f 6e3e 0a20 2020 2020 2020 2020 2020  ion>.           
+00000310: 2065 6e74 7279 706f 696e 743a 2062 6964   entrypoint: bid
+00000320: 0a20 2020 2020 202d 2063 616c 6c62 6163  .      - callbac
+00000330: 6b3a 206f 6e5f 7769 7468 6472 6177 0a20  k: on_withdraw. 
+00000340: 2020 2020 2020 2070 6174 7465 726e 3a0a         pattern:.
+00000350: 2020 2020 2020 2020 2020 2d20 7479 7065            - type
+00000360: 3a20 7472 616e 7361 6374 696f 6e0a 2020  : transaction.  
+00000370: 2020 2020 2020 2020 2020 6465 7374 696e            destin
+00000380: 6174 696f 6e3a 203c 6175 6374 696f 6e3e  ation: <auction>
+00000390: 0a20 2020 2020 2020 2020 2020 2065 6e74  .            ent
+000003a0: 7279 706f 696e 743a 2077 6974 6864 7261  rypoint: withdra
+000003b0: 770a 0a69 6e64 6578 6573 3a0a 2020 747a  w..indexes:.  tz
+000003c0: 636f 6c6f 7273 3a0a 2020 2020 7465 6d70  colors:.    temp
+000003d0: 6c61 7465 3a20 6175 6374 696f 6e0a 2020  late: auction.  
+000003e0: 2020 7661 6c75 6573 3a0a 2020 2020 2020    values:.      
+000003f0: 6461 7461 736f 7572 6365 3a20 747a 6b74  datasource: tzkt
+00000400: 0a20 2020 2020 206d 696e 7465 723a 2074  .      minter: t
+00000410: 7a63 6f6c 6f72 735f 6d69 6e74 6572 0a20  zcolors_minter. 
+00000420: 2020 2020 2061 7563 7469 6f6e 3a20 747a       auction: tz
+00000430: 636f 6c6f 7273 5f61 7563 7469 6f6e 0a    colors_auction.
```

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_auction/handlers/on_bid.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_auction/handlers/on_bid.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_auction/handlers/on_create_auction.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_auction/handlers/on_create_auction.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_auction/handlers/on_withdraw.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_auction/handlers/on_withdraw.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_auction/models/__init__.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_auction/models/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_big_maps/dipdup.yaml.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_big_maps/dipdup.yaml.j2`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,46 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 207b 7b20 7072  0.package: {{ pr
 00000020: 6f6a 6563 742e 7061 636b 6167 6520 7d7d  oject.package }}
-00000030: 0a0a 6461 7461 6261 7365 3a0a 2020 6b69  ..database:.  ki
-00000040: 6e64 3a20 7371 6c69 7465 0a20 2070 6174  nd: sqlite.  pat
-00000050: 683a 207b 7b20 7072 6f6a 6563 742e 7061  h: {{ project.pa
-00000060: 636b 6167 6520 7d7d 2e73 716c 6974 6533  ckage }}.sqlite3
-00000070: 0a0a 636f 6e74 7261 6374 733a 0a20 206d  ..contracts:.  m
-00000080: 6169 6e6e 6574 5f6e 616d 655f 7265 6769  ainnet_name_regi
-00000090: 7374 7279 3a0a 2020 2020 6b69 6e64 3a20  stry:.    kind: 
-000000a0: 7465 7a6f 730a 2020 2020 6164 6472 6573  tezos.    addres
-000000b0: 733a 204b 5431 4742 5a6d 5378 6d6e 4b4a  s: KT1GBZmSxmnKJ
-000000c0: 5847 4d64 4d4c 6275 6750 664c 7955 506d  XGMdMLbugPfLyUPm
-000000d0: 754c 534d 774b 530a 2020 2020 7479 7065  uLSMwKS.    type
-000000e0: 6e61 6d65 3a20 6e61 6d65 5f72 6567 6973  name: name_regis
-000000f0: 7472 790a 0a64 6174 6173 6f75 7263 6573  try..datasources
-00000100: 3a0a 2020 747a 6b74 5f6d 6169 6e6e 6574  :.  tzkt_mainnet
-00000110: 3a0a 2020 2020 6b69 6e64 3a20 7465 7a6f  :.    kind: tezo
-00000120: 732e 747a 6b74 0a20 2020 2075 726c 3a20  s.tzkt.    url: 
-00000130: 247b 545a 4b54 5f55 524c 3a2d 6874 7470  ${TZKT_URL:-http
-00000140: 733a 2f2f 6170 692e 747a 6b74 2e69 6f7d  s://api.tzkt.io}
-00000150: 0a0a 7465 6d70 6c61 7465 733a 0a20 2062  ..templates:.  b
-00000160: 6967 5f6d 6170 733a 0a20 2020 206b 696e  ig_maps:.    kin
-00000170: 643a 2074 657a 6f73 2e74 7a6b 742e 6269  d: tezos.tzkt.bi
-00000180: 675f 6d61 7073 0a20 2020 2064 6174 6173  g_maps.    datas
-00000190: 6f75 7263 653a 203c 6461 7461 736f 7572  ource: <datasour
-000001a0: 6365 3e0a 2020 2020 736b 6970 5f68 6973  ce>.    skip_his
-000001b0: 746f 7279 3a20 6f6e 6365 0a20 2020 2068  tory: once.    h
-000001c0: 616e 646c 6572 733a 0a20 2020 2020 202d  andlers:.      -
-000001d0: 2063 616c 6c62 6163 6b3a 206f 6e5f 7570   callback: on_up
-000001e0: 6461 7465 5f72 6563 6f72 6473 0a20 2020  date_records.   
-000001f0: 2020 2020 2063 6f6e 7472 6163 743a 203c       contract: <
-00000200: 6e61 6d65 5f72 6567 6973 7472 793e 0a20  name_registry>. 
-00000210: 2020 2020 2020 2070 6174 683a 2073 746f         path: sto
-00000220: 7265 2e72 6563 6f72 6473 0a20 2020 2020  re.records.     
-00000230: 202d 2063 616c 6c62 6163 6b3a 206f 6e5f   - callback: on_
-00000240: 7570 6461 7465 5f65 7870 6972 795f 6d61  update_expiry_ma
-00000250: 700a 2020 2020 2020 2020 636f 6e74 7261  p.        contra
-00000260: 6374 3a20 3c6e 616d 655f 7265 6769 7374  ct: <name_regist
-00000270: 7279 3e0a 2020 2020 2020 2020 7061 7468  ry>.        path
-00000280: 3a20 7374 6f72 652e 6578 7069 7279 5f6d  : store.expiry_m
-00000290: 6170 0a0a 696e 6465 7865 733a 0a20 2062  ap..indexes:.  b
-000002a0: 6967 5f6d 6170 735f 6d61 696e 6e65 743a  ig_maps_mainnet:
-000002b0: 0a20 2020 2074 656d 706c 6174 653a 2062  .    template: b
-000002c0: 6967 5f6d 6170 730a 2020 2020 7661 6c75  ig_maps.    valu
-000002d0: 6573 3a0a 2020 2020 2020 6461 7461 736f  es:.      dataso
-000002e0: 7572 6365 3a20 747a 6b74 5f6d 6169 6e6e  urce: tzkt_mainn
-000002f0: 6574 0a20 2020 2020 206e 616d 655f 7265  et.      name_re
-00000300: 6769 7374 7279 3a20 6d61 696e 6e65 745f  gistry: mainnet_
-00000310: 6e61 6d65 5f72 6567 6973 7472 790a       name_registry.
+00000030: 0a0a 636f 6e74 7261 6374 733a 0a20 206d  ..contracts:.  m
+00000040: 6169 6e6e 6574 5f6e 616d 655f 7265 6769  ainnet_name_regi
+00000050: 7374 7279 3a0a 2020 2020 6b69 6e64 3a20  stry:.    kind: 
+00000060: 7465 7a6f 730a 2020 2020 6164 6472 6573  tezos.    addres
+00000070: 733a 204b 5431 4742 5a6d 5378 6d6e 4b4a  s: KT1GBZmSxmnKJ
+00000080: 5847 4d64 4d4c 6275 6750 664c 7955 506d  XGMdMLbugPfLyUPm
+00000090: 754c 534d 774b 530a 2020 2020 7479 7065  uLSMwKS.    type
+000000a0: 6e61 6d65 3a20 6e61 6d65 5f72 6567 6973  name: name_regis
+000000b0: 7472 790a 0a64 6174 6173 6f75 7263 6573  try..datasources
+000000c0: 3a0a 2020 747a 6b74 5f6d 6169 6e6e 6574  :.  tzkt_mainnet
+000000d0: 3a0a 2020 2020 6b69 6e64 3a20 7465 7a6f  :.    kind: tezo
+000000e0: 732e 747a 6b74 0a20 2020 2075 726c 3a20  s.tzkt.    url: 
+000000f0: 247b 545a 4b54 5f55 524c 3a2d 6874 7470  ${TZKT_URL:-http
+00000100: 733a 2f2f 6170 692e 747a 6b74 2e69 6f7d  s://api.tzkt.io}
+00000110: 0a0a 7465 6d70 6c61 7465 733a 0a20 2062  ..templates:.  b
+00000120: 6967 5f6d 6170 733a 0a20 2020 206b 696e  ig_maps:.    kin
+00000130: 643a 2074 657a 6f73 2e74 7a6b 742e 6269  d: tezos.tzkt.bi
+00000140: 675f 6d61 7073 0a20 2020 2064 6174 6173  g_maps.    datas
+00000150: 6f75 7263 653a 203c 6461 7461 736f 7572  ource: <datasour
+00000160: 6365 3e0a 2020 2020 736b 6970 5f68 6973  ce>.    skip_his
+00000170: 746f 7279 3a20 6f6e 6365 0a20 2020 2068  tory: once.    h
+00000180: 616e 646c 6572 733a 0a20 2020 2020 202d  andlers:.      -
+00000190: 2063 616c 6c62 6163 6b3a 206f 6e5f 7570   callback: on_up
+000001a0: 6461 7465 5f72 6563 6f72 6473 0a20 2020  date_records.   
+000001b0: 2020 2020 2063 6f6e 7472 6163 743a 203c       contract: <
+000001c0: 6e61 6d65 5f72 6567 6973 7472 793e 0a20  name_registry>. 
+000001d0: 2020 2020 2020 2070 6174 683a 2073 746f         path: sto
+000001e0: 7265 2e72 6563 6f72 6473 0a20 2020 2020  re.records.     
+000001f0: 202d 2063 616c 6c62 6163 6b3a 206f 6e5f   - callback: on_
+00000200: 7570 6461 7465 5f65 7870 6972 795f 6d61  update_expiry_ma
+00000210: 700a 2020 2020 2020 2020 636f 6e74 7261  p.        contra
+00000220: 6374 3a20 3c6e 616d 655f 7265 6769 7374  ct: <name_regist
+00000230: 7279 3e0a 2020 2020 2020 2020 7061 7468  ry>.        path
+00000240: 3a20 7374 6f72 652e 6578 7069 7279 5f6d  : store.expiry_m
+00000250: 6170 0a0a 696e 6465 7865 733a 0a20 2062  ap..indexes:.  b
+00000260: 6967 5f6d 6170 735f 6d61 696e 6e65 743a  ig_maps_mainnet:
+00000270: 0a20 2020 2074 656d 706c 6174 653a 2062  .    template: b
+00000280: 6967 5f6d 6170 730a 2020 2020 7661 6c75  ig_maps.    valu
+00000290: 6573 3a0a 2020 2020 2020 6461 7461 736f  es:.      dataso
+000002a0: 7572 6365 3a20 747a 6b74 5f6d 6169 6e6e  urce: tzkt_mainn
+000002b0: 6574 0a20 2020 2020 206e 616d 655f 7265  et.      name_re
+000002c0: 6769 7374 7279 3a20 6d61 696e 6e65 745f  gistry: mainnet_
+000002d0: 6e61 6d65 5f72 6567 6973 7472 790a       name_registry.
```

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_big_maps/handlers/on_update_expiry_map.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_big_maps/handlers/on_update_expiry_map.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_big_maps/handlers/on_update_records.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_big_maps/handlers/on_update_records.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_big_maps/models/__init__.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_big_maps/models/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_dao/dipdup.yaml.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_factories/dipdup.yaml.j2`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 207b 7b20 7072  0.package: {{ pr
 00000020: 6f6a 6563 742e 7061 636b 6167 6520 7d7d  oject.package }}
-00000030: 0a0a 6461 7461 6261 7365 3a0a 2020 6b69  ..database:.  ki
-00000040: 6e64 3a20 7371 6c69 7465 0a20 2070 6174  nd: sqlite.  pat
-00000050: 683a 207b 7b20 7072 6f6a 6563 742e 7061  h: {{ project.pa
-00000060: 636b 6167 6520 7d7d 2e73 716c 6974 6533  ckage }}.sqlite3
-00000070: 0a0a 636f 6e74 7261 6374 733a 0a20 2072  ..contracts:.  r
-00000080: 6567 6973 7472 793a 0a20 2020 206b 696e  egistry:.    kin
-00000090: 643a 2074 657a 6f73 0a20 2020 2063 6f64  d: tezos.    cod
-000000a0: 655f 6861 7368 3a20 4b54 3139 4346 334b  e_hash: KT19CF3K
-000000b0: 4b72 7664 5737 3774 7446 6f6d 4375 696e  KrvdW77ttFomCuin
-000000c0: 326b 3475 4156 6b72 7959 7168 0a20 2020  2k4uAVkryYqh.   
-000000d0: 2074 7970 656e 616d 653a 2072 6567 6973   typename: regis
-000000e0: 7472 790a 0a64 6174 6173 6f75 7263 6573  try..datasources
-000000f0: 3a0a 2020 747a 6b74 3a0a 2020 2020 6b69  :.  tzkt:.    ki
-00000100: 6e64 3a20 7465 7a6f 732e 747a 6b74 0a20  nd: tezos.tzkt. 
-00000110: 2020 2075 726c 3a20 247b 545a 4b54 5f55     url: ${TZKT_U
-00000120: 524c 3a2d 6874 7470 733a 2f2f 6170 692e  RL:-https://api.
-00000130: 747a 6b74 2e69 6f7d 0a0a 696e 6465 7865  tzkt.io}..indexe
-00000140: 733a 0a20 2072 6567 6973 7472 795f 6461  s:.  registry_da
-00000150: 6f3a 0a20 2020 206b 696e 643a 2074 657a  o:.    kind: tez
-00000160: 6f73 2e74 7a6b 742e 6f70 6572 6174 696f  os.tzkt.operatio
-00000170: 6e73 0a20 2020 2064 6174 6173 6f75 7263  ns.    datasourc
-00000180: 653a 2074 7a6b 740a 2020 2020 7479 7065  e: tzkt.    type
-00000190: 733a 0a20 2020 2020 202d 2074 7261 6e73  s:.      - trans
-000001a0: 6163 7469 6f6e 0a20 2020 2020 202d 206f  action.      - o
-000001b0: 7269 6769 6e61 7469 6f6e 0a20 2020 2068  rigination.    h
-000001c0: 616e 646c 6572 733a 0a20 2020 2020 202d  andlers:.      -
-000001d0: 2063 616c 6c62 6163 6b3a 206f 6e5f 6f72   callback: on_or
-000001e0: 6967 696e 6174 696f 6e0a 2020 2020 2020  igination.      
-000001f0: 2020 7061 7474 6572 6e3a 0a20 2020 2020    pattern:.     
-00000200: 2020 2020 202d 2074 7970 653a 206f 7269       - type: ori
-00000210: 6769 6e61 7469 6f6e 0a20 2020 2020 2020  gination.       
-00000220: 2020 2020 206f 7269 6769 6e61 7465 645f       originated_
-00000230: 636f 6e74 7261 6374 3a20 7265 6769 7374  contract: regist
-00000240: 7279 0a20 2020 2020 202d 2063 616c 6c62  ry.      - callb
-00000250: 6163 6b3a 206f 6e5f 7072 6f70 6f73 650a  ack: on_propose.
-00000260: 2020 2020 2020 2020 7061 7474 6572 6e3a          pattern:
-00000270: 0a20 2020 2020 2020 2020 202d 2074 7970  .          - typ
-00000280: 653a 2074 7261 6e73 6163 7469 6f6e 0a20  e: transaction. 
-00000290: 2020 2020 2020 2020 2020 2064 6573 7469             desti
-000002a0: 6e61 7469 6f6e 3a20 7265 6769 7374 7279  nation: registry
-000002b0: 0a20 2020 2020 2020 2020 2020 2065 6e74  .            ent
-000002c0: 7279 706f 696e 743a 2070 726f 706f 7365  rypoint: propose
-000002d0: 0a                                       .
+00000030: 0a0a 636f 6e74 7261 6374 733a 0a20 2072  ..contracts:.  r
+00000040: 6567 6973 7472 793a 0a20 2020 206b 696e  egistry:.    kin
+00000050: 643a 2074 657a 6f73 0a20 2020 2061 6464  d: tezos.    add
+00000060: 7265 7373 3a20 4b54 3139 4346 334b 4b72  ress: KT19CF3KKr
+00000070: 7664 5737 3774 7446 6f6d 4375 696e 326b  vdW77ttFomCuin2k
+00000080: 3475 4156 6b72 7959 7168 0a20 2020 2074  4uAVkryYqh.    t
+00000090: 7970 656e 616d 653a 2072 6567 6973 7472  ypename: registr
+000000a0: 790a 0a64 6174 6173 6f75 7263 6573 3a0a  y..datasources:.
+000000b0: 2020 747a 6b74 3a0a 2020 2020 6b69 6e64    tzkt:.    kind
+000000c0: 3a20 7465 7a6f 732e 747a 6b74 0a20 2020  : tezos.tzkt.   
+000000d0: 2075 726c 3a20 247b 545a 4b54 5f55 524c   url: ${TZKT_URL
+000000e0: 3a2d 6874 7470 733a 2f2f 6170 692e 747a  :-https://api.tz
+000000f0: 6b74 2e69 6f7d 0a0a 696e 6465 7865 733a  kt.io}..indexes:
+00000100: 0a20 2072 6567 6973 7472 795f 6461 6f3a  .  registry_dao:
+00000110: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
+00000120: 2e74 7a6b 742e 6f70 6572 6174 696f 6e73  .tzkt.operations
+00000130: 0a20 2020 2064 6174 6173 6f75 7263 653a  .    datasource:
+00000140: 2074 7a6b 740a 2020 2020 7479 7065 733a   tzkt.    types:
+00000150: 0a20 2020 2020 202d 2074 7261 6e73 6163  .      - transac
+00000160: 7469 6f6e 0a20 2020 2020 202d 206f 7269  tion.      - ori
+00000170: 6769 6e61 7469 6f6e 0a20 2020 2068 616e  gination.    han
+00000180: 646c 6572 733a 0a20 2020 2020 202d 2063  dlers:.      - c
+00000190: 616c 6c62 6163 6b3a 206f 6e5f 6f72 6967  allback: on_orig
+000001a0: 696e 6174 696f 6e0a 2020 2020 2020 2020  ination.        
+000001b0: 7061 7474 6572 6e3a 0a20 2020 2020 2020  pattern:.       
+000001c0: 2020 202d 2074 7970 653a 206f 7269 6769     - type: origi
+000001d0: 6e61 7469 6f6e 0a20 2020 2020 2020 2020  nation.         
+000001e0: 2020 206f 7269 6769 6e61 7465 645f 636f     originated_co
+000001f0: 6e74 7261 6374 3a20 7265 6769 7374 7279  ntract: registry
+00000200: 0a20 2020 2020 202d 2063 616c 6c62 6163  .      - callbac
+00000210: 6b3a 206f 6e5f 7072 6f70 6f73 650a 2020  k: on_propose.  
+00000220: 2020 2020 2020 7061 7474 6572 6e3a 0a20        pattern:. 
+00000230: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
+00000240: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
+00000250: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
+00000260: 7469 6f6e 3a20 7265 6769 7374 7279 0a20  tion: registry. 
+00000270: 2020 2020 2020 2020 2020 2065 6e74 7279             entry
+00000280: 706f 696e 743a 2070 726f 706f 7365 0a    point: propose.
```

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_dao/handlers/on_propose.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_dao/handlers/on_propose.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_dao/models/__init__.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_dao/models/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/dipdup.yaml.j2` & `dipdup-7.0.0rc2/src/demo_dex/dipdup.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,308 +1,303 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
-00000010: 300a 7061 636b 6167 653a 207b 7b20 7072  0.package: {{ pr
-00000020: 6f6a 6563 742e 7061 636b 6167 6520 7d7d  oject.package }}
-00000030: 0a0a 6461 7461 6261 7365 3a0a 2020 6b69  ..database:.  ki
-00000040: 6e64 3a20 7371 6c69 7465 0a20 2070 6174  nd: sqlite.  pat
-00000050: 683a 207b 7b20 7072 6f6a 6563 742e 7061  h: {{ project.pa
-00000060: 636b 6167 6520 7d7d 2e73 716c 6974 6533  ckage }}.sqlite3
-00000070: 0a0a 636f 6e74 7261 6374 733a 0a20 206b  ..contracts:.  k
-00000080: 7573 645f 6465 785f 6d61 696e 6e65 743a  usd_dex_mainnet:
-00000090: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
-000000a0: 0a20 2020 2061 6464 7265 7373 3a20 4b54  .    address: KT
-000000b0: 314b 3445 7754 7062 7659 4e39 6167 4a64  1K4EwTpbvYN9agJd
-000000c0: 6a70 794a 6d34 5a5a 6468 7055 4e4b 4233  jpyJm4ZZdhpUNKB3
-000000d0: 4636 0a20 2020 2074 7970 656e 616d 653a  F6.    typename:
-000000e0: 2071 7569 7075 5f66 6131 320a 2020 6b75   quipu_fa12.  ku
-000000f0: 7364 5f74 6f6b 656e 5f6d 6169 6e6e 6574  sd_token_mainnet
-00000100: 3a0a 2020 2020 6b69 6e64 3a20 7465 7a6f  :.    kind: tezo
-00000110: 730a 2020 2020 6164 6472 6573 733a 204b  s.    address: K
-00000120: 5431 4b39 6743 5267 614c 5246 4b54 4572  T1K9gCRgaLRFKTEr
-00000130: 5974 3177 5678 4133 4672 6239 466a 6173  Yt1wVxA3Frb9Fjas
-00000140: 6a54 560a 2020 2020 7479 7065 6e61 6d65  jTV.    typename
-00000150: 3a20 6661 3132 5f74 6f6b 656e 0a20 2068  : fa12_token.  h
-00000160: 6461 6f5f 6465 785f 6d61 696e 6e65 743a  dao_dex_mainnet:
-00000170: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
-00000180: 0a20 2020 2061 6464 7265 7373 3a20 4b54  .    address: KT
-00000190: 3151 784c 7175 6b79 666f 6850 5635 6b50  1QxLqukyfohPV5kP
-000001a0: 6b77 3937 5273 3663 7731 4444 4476 5967  kw97Rs6cw1DDDvYg
-000001b0: 6242 0a20 2020 2074 7970 656e 616d 653a  bB.    typename:
-000001c0: 2071 7569 7075 5f66 6132 0a20 2068 6461   quipu_fa2.  hda
-000001d0: 6f5f 746f 6b65 6e5f 6d61 696e 6e65 743a  o_token_mainnet:
-000001e0: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
-000001f0: 0a20 2020 2061 6464 7265 7373 3a20 4b54  .    address: KT
-00000200: 3141 4641 326d 774e 554d 4e64 3453 7375  1AFA2mwNUMNd4Ssu
-00000210: 6a45 3159 5970 3239 7664 3842 5a65 6a79  jE1YYp29vd8BZejy
-00000220: 4b57 0a20 2020 2074 7970 656e 616d 653a  KW.    typename:
-00000230: 2066 6132 5f74 6f6b 656e 0a0a 6461 7461   fa2_token..data
-00000240: 736f 7572 6365 733a 0a20 2074 7a6b 745f  sources:.  tzkt_
-00000250: 6d61 696e 6e65 743a 0a20 2020 206b 696e  mainnet:.    kin
-00000260: 643a 2074 657a 6f73 2e74 7a6b 740a 2020  d: tezos.tzkt.  
-00000270: 2020 7572 6c3a 2068 7474 7073 3a2f 2f61    url: https://a
-00000280: 7069 2e74 7a6b 742e 696f 0a0a 7465 6d70  pi.tzkt.io..temp
-00000290: 6c61 7465 733a 0a20 2071 7569 7075 7377  lates:.  quipusw
-000002a0: 6170 5f66 6131 323a 0a20 2020 206b 696e  ap_fa12:.    kin
-000002b0: 643a 2074 657a 6f73 2e74 7a6b 742e 6f70  d: tezos.tzkt.op
-000002c0: 6572 6174 696f 6e73 0a20 2020 2064 6174  erations.    dat
-000002d0: 6173 6f75 7263 653a 2074 7a6b 745f 6d61  asource: tzkt_ma
-000002e0: 696e 6e65 740a 2020 2020 636f 6e74 7261  innet.    contra
-000002f0: 6374 733a 0a20 2020 2020 202d 203c 6465  cts:.      - <de
-00000300: 785f 636f 6e74 7261 6374 3e0a 2020 2020  x_contract>.    
-00000310: 7479 7065 733a 0a20 2020 2020 202d 2074  types:.      - t
-00000320: 7261 6e73 6163 7469 6f6e 0a20 2020 2020  ransaction.     
-00000330: 202d 206f 7269 6769 6e61 7469 6f6e 0a20   - origination. 
-00000340: 2020 2068 616e 646c 6572 733a 0a20 2020     handlers:.   
-00000350: 2020 202d 2063 616c 6c62 6163 6b3a 206f     - callback: o
-00000360: 6e5f 6661 3132 5f6f 7269 6769 6e61 7469  n_fa12_originati
-00000370: 6f6e 0a20 2020 2020 2020 2070 6174 7465  on.        patte
-00000380: 726e 3a0a 2020 2020 2020 2020 2020 2d20  rn:.          - 
-00000390: 7479 7065 3a20 6f72 6967 696e 6174 696f  type: originatio
-000003a0: 6e0a 2020 2020 2020 2020 2020 2020 6f72  n.            or
-000003b0: 6967 696e 6174 6564 5f63 6f6e 7472 6163  iginated_contrac
-000003c0: 743a 203c 6465 785f 636f 6e74 7261 6374  t: <dex_contract
-000003d0: 3e0a 2020 2020 2020 2d20 6361 6c6c 6261  >.      - callba
-000003e0: 636b 3a20 6f6e 5f66 6131 325f 746f 6b65  ck: on_fa12_toke
-000003f0: 6e5f 746f 5f74 657a 0a20 2020 2020 2020  n_to_tez.       
-00000400: 2070 6174 7465 726e 3a0a 2020 2020 2020   pattern:.      
-00000410: 2020 2020 2d20 7479 7065 3a20 7472 616e      - type: tran
-00000420: 7361 6374 696f 6e0a 2020 2020 2020 2020  saction.        
-00000430: 2020 2020 6465 7374 696e 6174 696f 6e3a      destination:
-00000440: 203c 6465 785f 636f 6e74 7261 6374 3e0a   <dex_contract>.
-00000450: 2020 2020 2020 2020 2020 2020 656e 7472              entr
-00000460: 7970 6f69 6e74 3a20 746f 6b65 6e54 6f54  ypoint: tokenToT
-00000470: 657a 5061 796d 656e 740a 2020 2020 2020  ezPayment.      
-00000480: 2020 2020 2d20 7479 7065 3a20 7472 616e      - type: tran
-00000490: 7361 6374 696f 6e0a 2020 2020 2020 2020  saction.        
-000004a0: 2020 2020 6465 7374 696e 6174 696f 6e3a      destination:
-000004b0: 203c 746f 6b65 6e5f 636f 6e74 7261 6374   <token_contract
-000004c0: 3e0a 2020 2020 2020 2020 2020 2020 656e  >.            en
-000004d0: 7472 7970 6f69 6e74 3a20 7472 616e 7366  trypoint: transf
-000004e0: 6572 0a20 2020 2020 2020 2020 202d 2074  er.          - t
-000004f0: 7970 653a 2074 7261 6e73 6163 7469 6f6e  ype: transaction
-00000500: 0a20 2020 2020 2020 2020 2020 2073 6f75  .            sou
-00000510: 7263 653a 203c 6465 785f 636f 6e74 7261  rce: <dex_contra
-00000520: 6374 3e0a 2020 2020 2020 2d20 6361 6c6c  ct>.      - call
-00000530: 6261 636b 3a20 6f6e 5f66 6131 325f 7465  back: on_fa12_te
-00000540: 7a5f 746f 5f74 6f6b 656e 0a20 2020 2020  z_to_token.     
-00000550: 2020 2070 6174 7465 726e 3a0a 2020 2020     pattern:.    
-00000560: 2020 2020 2020 2d20 7479 7065 3a20 7472        - type: tr
-00000570: 616e 7361 6374 696f 6e0a 2020 2020 2020  ansaction.      
-00000580: 2020 2020 2020 6465 7374 696e 6174 696f        destinatio
-00000590: 6e3a 203c 6465 785f 636f 6e74 7261 6374  n: <dex_contract
-000005a0: 3e0a 2020 2020 2020 2020 2020 2020 656e  >.            en
-000005b0: 7472 7970 6f69 6e74 3a20 7465 7a54 6f54  trypoint: tezToT
-000005c0: 6f6b 656e 5061 796d 656e 740a 2020 2020  okenPayment.    
-000005d0: 2020 2020 2020 2d20 7479 7065 3a20 7472        - type: tr
-000005e0: 616e 7361 6374 696f 6e0a 2020 2020 2020  ansaction.      
-000005f0: 2020 2020 2020 6465 7374 696e 6174 696f        destinatio
-00000600: 6e3a 203c 746f 6b65 6e5f 636f 6e74 7261  n: <token_contra
-00000610: 6374 3e0a 2020 2020 2020 2020 2020 2020  ct>.            
-00000620: 656e 7472 7970 6f69 6e74 3a20 7472 616e  entrypoint: tran
-00000630: 7366 6572 0a20 2020 2020 202d 2063 616c  sfer.      - cal
-00000640: 6c62 6163 6b3a 206f 6e5f 6661 3132 5f69  lback: on_fa12_i
-00000650: 6e76 6573 745f 6c69 7175 6964 6974 790a  nvest_liquidity.
-00000660: 2020 2020 2020 2020 7061 7474 6572 6e3a          pattern:
-00000670: 0a20 2020 2020 2020 2020 202d 2074 7970  .          - typ
-00000680: 653a 2074 7261 6e73 6163 7469 6f6e 0a20  e: transaction. 
-00000690: 2020 2020 2020 2020 2020 2064 6573 7469             desti
-000006a0: 6e61 7469 6f6e 3a20 3c64 6578 5f63 6f6e  nation: <dex_con
-000006b0: 7472 6163 743e 0a20 2020 2020 2020 2020  tract>.         
-000006c0: 2020 2065 6e74 7279 706f 696e 743a 2069     entrypoint: i
-000006d0: 6e76 6573 744c 6971 7569 6469 7479 0a20  nvestLiquidity. 
-000006e0: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
-000006f0: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
-00000700: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
-00000710: 7469 6f6e 3a20 3c74 6f6b 656e 5f63 6f6e  tion: <token_con
-00000720: 7472 6163 743e 0a20 2020 2020 2020 2020  tract>.         
-00000730: 2020 2065 6e74 7279 706f 696e 743a 2074     entrypoint: t
-00000740: 7261 6e73 6665 720a 2020 2020 2020 2d20  ransfer.      - 
-00000750: 6361 6c6c 6261 636b 3a20 6f6e 5f66 6131  callback: on_fa1
-00000760: 325f 7472 616e 7366 6572 0a20 2020 2020  2_transfer.     
-00000770: 2020 2070 6174 7465 726e 3a0a 2020 2020     pattern:.    
-00000780: 2020 2020 2020 2d20 7479 7065 3a20 7472        - type: tr
-00000790: 616e 7361 6374 696f 6e0a 2020 2020 2020  ansaction.      
-000007a0: 2020 2020 2020 6465 7374 696e 6174 696f        destinatio
-000007b0: 6e3a 203c 6465 785f 636f 6e74 7261 6374  n: <dex_contract
-000007c0: 3e0a 2020 2020 2020 2020 2020 2020 656e  >.            en
-000007d0: 7472 7970 6f69 6e74 3a20 7472 616e 7366  trypoint: transf
-000007e0: 6572 0a20 2020 2020 202d 2063 616c 6c62  er.      - callb
-000007f0: 6163 6b3a 206f 6e5f 6661 3132 5f64 6976  ack: on_fa12_div
-00000800: 6573 745f 6c69 7175 6964 6974 790a 2020  est_liquidity.  
-00000810: 2020 2020 2020 7061 7474 6572 6e3a 0a20        pattern:. 
-00000820: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
-00000830: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
-00000840: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
-00000850: 7469 6f6e 3a20 3c64 6578 5f63 6f6e 7472  tion: <dex_contr
-00000860: 6163 743e 0a20 2020 2020 2020 2020 2020  act>.           
-00000870: 2065 6e74 7279 706f 696e 743a 2064 6976   entrypoint: div
-00000880: 6573 744c 6971 7569 6469 7479 0a20 2020  estLiquidity.   
-00000890: 2020 2020 2020 202d 2074 7970 653a 2074         - type: t
-000008a0: 7261 6e73 6163 7469 6f6e 0a20 2020 2020  ransaction.     
-000008b0: 2020 2020 2020 2064 6573 7469 6e61 7469         destinati
-000008c0: 6f6e 3a20 3c74 6f6b 656e 5f63 6f6e 7472  on: <token_contr
-000008d0: 6163 743e 0a20 2020 2020 2020 2020 2020  act>.           
-000008e0: 2065 6e74 7279 706f 696e 743a 2074 7261   entrypoint: tra
-000008f0: 6e73 6665 720a 2020 2020 2020 2020 2020  nsfer.          
-00000900: 2d20 7479 7065 3a20 7472 616e 7361 6374  - type: transact
-00000910: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-00000920: 736f 7572 6365 3a20 3c64 6578 5f63 6f6e  source: <dex_con
-00000930: 7472 6163 743e 0a20 2020 2020 202d 2063  tract>.      - c
-00000940: 616c 6c62 6163 6b3a 206f 6e5f 6661 3132  allback: on_fa12
-00000950: 5f77 6974 6864 7261 775f 7072 6f66 6974  _withdraw_profit
-00000960: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
-00000970: 3a0a 2020 2020 2020 2020 2020 2d20 7479  :.          - ty
-00000980: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
-00000990: 2020 2020 2020 2020 2020 2020 6465 7374              dest
-000009a0: 696e 6174 696f 6e3a 203c 6465 785f 636f  ination: <dex_co
-000009b0: 6e74 7261 6374 3e0a 2020 2020 2020 2020  ntract>.        
-000009c0: 2020 2020 656e 7472 7970 6f69 6e74 3a20      entrypoint: 
-000009d0: 7769 7468 6472 6177 5072 6f66 6974 0a20  withdrawProfit. 
-000009e0: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
-000009f0: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
-00000a00: 2020 2020 2020 2020 2073 6f75 7263 653a           source:
-00000a10: 203c 6465 785f 636f 6e74 7261 6374 3e0a   <dex_contract>.
-00000a20: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
-00000a30: 6f6e 616c 3a20 5472 7565 0a0a 2020 7175  onal: True..  qu
-00000a40: 6970 7573 7761 705f 6661 323a 0a20 2020  ipuswap_fa2:.   
-00000a50: 206b 696e 643a 2074 657a 6f73 2e74 7a6b   kind: tezos.tzk
-00000a60: 742e 6f70 6572 6174 696f 6e73 0a20 2020  t.operations.   
-00000a70: 2064 6174 6173 6f75 7263 653a 2074 7a6b   datasource: tzk
-00000a80: 745f 6d61 696e 6e65 740a 2020 2020 636f  t_mainnet.    co
-00000a90: 6e74 7261 6374 733a 0a20 2020 2020 202d  ntracts:.      -
-00000aa0: 203c 6465 785f 636f 6e74 7261 6374 3e0a   <dex_contract>.
-00000ab0: 2020 2020 7479 7065 733a 0a20 2020 2020      types:.     
-00000ac0: 202d 2074 7261 6e73 6163 7469 6f6e 0a20   - transaction. 
-00000ad0: 2020 2020 202d 206f 7269 6769 6e61 7469       - originati
-00000ae0: 6f6e 0a20 2020 2068 616e 646c 6572 733a  on.    handlers:
-00000af0: 0a20 2020 2020 202d 2063 616c 6c62 6163  .      - callbac
-00000b00: 6b3a 206f 6e5f 6661 325f 6f72 6967 696e  k: on_fa2_origin
-00000b10: 6174 696f 6e0a 2020 2020 2020 2020 7061  ation.        pa
-00000b20: 7474 6572 6e3a 0a20 2020 2020 2020 2020  ttern:.         
-00000b30: 202d 2074 7970 653a 206f 7269 6769 6e61   - type: origina
-00000b40: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-00000b50: 206f 7269 6769 6e61 7465 645f 636f 6e74   originated_cont
-00000b60: 7261 6374 3a20 3c64 6578 5f63 6f6e 7472  ract: <dex_contr
-00000b70: 6163 743e 0a20 2020 2020 202d 2063 616c  act>.      - cal
-00000b80: 6c62 6163 6b3a 206f 6e5f 6661 325f 746f  lback: on_fa2_to
-00000b90: 6b65 6e5f 746f 5f74 657a 0a20 2020 2020  ken_to_tez.     
-00000ba0: 2020 2070 6174 7465 726e 3a0a 2020 2020     pattern:.    
-00000bb0: 2020 2020 2020 2d20 7479 7065 3a20 7472        - type: tr
-00000bc0: 616e 7361 6374 696f 6e0a 2020 2020 2020  ansaction.      
-00000bd0: 2020 2020 2020 6465 7374 696e 6174 696f        destinatio
-00000be0: 6e3a 203c 6465 785f 636f 6e74 7261 6374  n: <dex_contract
-00000bf0: 3e0a 2020 2020 2020 2020 2020 2020 656e  >.            en
-00000c00: 7472 7970 6f69 6e74 3a20 746f 6b65 6e54  trypoint: tokenT
-00000c10: 6f54 657a 5061 796d 656e 740a 2020 2020  oTezPayment.    
-00000c20: 2020 2020 2020 2d20 7479 7065 3a20 7472        - type: tr
-00000c30: 616e 7361 6374 696f 6e0a 2020 2020 2020  ansaction.      
-00000c40: 2020 2020 2020 6465 7374 696e 6174 696f        destinatio
-00000c50: 6e3a 203c 746f 6b65 6e5f 636f 6e74 7261  n: <token_contra
-00000c60: 6374 3e0a 2020 2020 2020 2020 2020 2020  ct>.            
-00000c70: 656e 7472 7970 6f69 6e74 3a20 7472 616e  entrypoint: tran
-00000c80: 7366 6572 0a20 2020 2020 2020 2020 202d  sfer.          -
-00000c90: 2074 7970 653a 2074 7261 6e73 6163 7469   type: transacti
-00000ca0: 6f6e 0a20 2020 2020 2020 2020 2020 2073  on.            s
-00000cb0: 6f75 7263 653a 203c 6465 785f 636f 6e74  ource: <dex_cont
-00000cc0: 7261 6374 3e0a 2020 2020 2020 2d20 6361  ract>.      - ca
-00000cd0: 6c6c 6261 636b 3a20 6f6e 5f66 6132 5f74  llback: on_fa2_t
-00000ce0: 657a 5f74 6f5f 746f 6b65 6e0a 2020 2020  ez_to_token.    
-00000cf0: 2020 2020 7061 7474 6572 6e3a 0a20 2020      pattern:.   
-00000d00: 2020 2020 2020 202d 2074 7970 653a 2074         - type: t
-00000d10: 7261 6e73 6163 7469 6f6e 0a20 2020 2020  ransaction.     
-00000d20: 2020 2020 2020 2064 6573 7469 6e61 7469         destinati
-00000d30: 6f6e 3a20 3c64 6578 5f63 6f6e 7472 6163  on: <dex_contrac
-00000d40: 743e 0a20 2020 2020 2020 2020 2020 2065  t>.            e
-00000d50: 6e74 7279 706f 696e 743a 2074 657a 546f  ntrypoint: tezTo
-00000d60: 546f 6b65 6e50 6179 6d65 6e74 0a20 2020  TokenPayment.   
-00000d70: 2020 2020 2020 202d 2074 7970 653a 2074         - type: t
-00000d80: 7261 6e73 6163 7469 6f6e 0a20 2020 2020  ransaction.     
-00000d90: 2020 2020 2020 2064 6573 7469 6e61 7469         destinati
-00000da0: 6f6e 3a20 3c74 6f6b 656e 5f63 6f6e 7472  on: <token_contr
-00000db0: 6163 743e 0a20 2020 2020 2020 2020 2020  act>.           
-00000dc0: 2065 6e74 7279 706f 696e 743a 2074 7261   entrypoint: tra
-00000dd0: 6e73 6665 720a 2020 2020 2020 2d20 6361  nsfer.      - ca
-00000de0: 6c6c 6261 636b 3a20 6f6e 5f66 6132 5f69  llback: on_fa2_i
-00000df0: 6e76 6573 745f 6c69 7175 6964 6974 790a  nvest_liquidity.
-00000e00: 2020 2020 2020 2020 7061 7474 6572 6e3a          pattern:
-00000e10: 0a20 2020 2020 2020 2020 202d 2074 7970  .          - typ
-00000e20: 653a 2074 7261 6e73 6163 7469 6f6e 0a20  e: transaction. 
-00000e30: 2020 2020 2020 2020 2020 2064 6573 7469             desti
-00000e40: 6e61 7469 6f6e 3a20 3c64 6578 5f63 6f6e  nation: <dex_con
-00000e50: 7472 6163 743e 0a20 2020 2020 2020 2020  tract>.         
-00000e60: 2020 2065 6e74 7279 706f 696e 743a 2069     entrypoint: i
-00000e70: 6e76 6573 744c 6971 7569 6469 7479 0a20  nvestLiquidity. 
-00000e80: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
-00000e90: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
-00000ea0: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
-00000eb0: 7469 6f6e 3a20 3c74 6f6b 656e 5f63 6f6e  tion: <token_con
-00000ec0: 7472 6163 743e 0a20 2020 2020 2020 2020  tract>.         
-00000ed0: 2020 2065 6e74 7279 706f 696e 743a 2074     entrypoint: t
-00000ee0: 7261 6e73 6665 720a 2020 2020 2020 2d20  ransfer.      - 
-00000ef0: 6361 6c6c 6261 636b 3a20 6f6e 5f66 6132  callback: on_fa2
-00000f00: 5f74 7261 6e73 6665 720a 2020 2020 2020  _transfer.      
-00000f10: 2020 7061 7474 6572 6e3a 0a20 2020 2020    pattern:.     
-00000f20: 2020 2020 202d 2074 7970 653a 2074 7261       - type: tra
-00000f30: 6e73 6163 7469 6f6e 0a20 2020 2020 2020  nsaction.       
-00000f40: 2020 2020 2064 6573 7469 6e61 7469 6f6e       destination
-00000f50: 3a20 3c64 6578 5f63 6f6e 7472 6163 743e  : <dex_contract>
-00000f60: 0a20 2020 2020 2020 2020 2020 2065 6e74  .            ent
-00000f70: 7279 706f 696e 743a 2074 7261 6e73 6665  rypoint: transfe
-00000f80: 720a 2020 2020 2020 2d20 6361 6c6c 6261  r.      - callba
-00000f90: 636b 3a20 6f6e 5f66 6132 5f64 6976 6573  ck: on_fa2_dives
-00000fa0: 745f 6c69 7175 6964 6974 790a 2020 2020  t_liquidity.    
-00000fb0: 2020 2020 7061 7474 6572 6e3a 0a20 2020      pattern:.   
-00000fc0: 2020 2020 2020 202d 2074 7970 653a 2074         - type: t
-00000fd0: 7261 6e73 6163 7469 6f6e 0a20 2020 2020  ransaction.     
-00000fe0: 2020 2020 2020 2064 6573 7469 6e61 7469         destinati
-00000ff0: 6f6e 3a20 3c64 6578 5f63 6f6e 7472 6163  on: <dex_contrac
-00001000: 743e 0a20 2020 2020 2020 2020 2020 2065  t>.            e
-00001010: 6e74 7279 706f 696e 743a 2064 6976 6573  ntrypoint: dives
-00001020: 744c 6971 7569 6469 7479 0a20 2020 2020  tLiquidity.     
-00001030: 2020 2020 202d 2074 7970 653a 2074 7261       - type: tra
-00001040: 6e73 6163 7469 6f6e 0a20 2020 2020 2020  nsaction.       
-00001050: 2020 2020 2064 6573 7469 6e61 7469 6f6e       destination
-00001060: 3a20 3c74 6f6b 656e 5f63 6f6e 7472 6163  : <token_contrac
-00001070: 743e 0a20 2020 2020 2020 2020 2020 2065  t>.            e
-00001080: 6e74 7279 706f 696e 743a 2074 7261 6e73  ntrypoint: trans
-00001090: 6665 720a 2020 2020 2020 2020 2020 2d20  fer.          - 
-000010a0: 7479 7065 3a20 7472 616e 7361 6374 696f  type: transactio
-000010b0: 6e0a 2020 2020 2020 2020 2020 2020 736f  n.            so
-000010c0: 7572 6365 3a20 3c64 6578 5f63 6f6e 7472  urce: <dex_contr
-000010d0: 6163 743e 0a20 2020 2020 202d 2063 616c  act>.      - cal
-000010e0: 6c62 6163 6b3a 206f 6e5f 6661 325f 7769  lback: on_fa2_wi
-000010f0: 7468 6472 6177 5f70 726f 6669 740a 2020  thdraw_profit.  
-00001100: 2020 2020 2020 7061 7474 6572 6e3a 0a20        pattern:. 
-00001110: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
-00001120: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
-00001130: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
-00001140: 7469 6f6e 3a20 3c64 6578 5f63 6f6e 7472  tion: <dex_contr
-00001150: 6163 743e 0a20 2020 2020 2020 2020 2020  act>.           
-00001160: 2065 6e74 7279 706f 696e 743a 2077 6974   entrypoint: wit
-00001170: 6864 7261 7750 726f 6669 740a 2020 2020  hdrawProfit.    
-00001180: 2020 2020 2020 2d20 7479 7065 3a20 7472        - type: tr
-00001190: 616e 7361 6374 696f 6e0a 2020 2020 2020  ansaction.      
-000011a0: 2020 2020 2020 736f 7572 6365 3a20 3c64        source: <d
-000011b0: 6578 5f63 6f6e 7472 6163 743e 0a20 2020  ex_contract>.   
-000011c0: 2020 2020 2020 2020 206f 7074 696f 6e61           optiona
-000011d0: 6c3a 2054 7275 650a 0a69 6e64 6578 6573  l: True..indexes
-000011e0: 3a0a 2020 6b75 7364 5f6d 6169 6e6e 6574  :.  kusd_mainnet
-000011f0: 3a0a 2020 2020 7465 6d70 6c61 7465 3a20  :.    template: 
-00001200: 7175 6970 7573 7761 705f 6661 3132 0a20  quipuswap_fa12. 
-00001210: 2020 2076 616c 7565 733a 0a20 2020 2020     values:.     
-00001220: 2064 6578 5f63 6f6e 7472 6163 743a 206b   dex_contract: k
-00001230: 7573 645f 6465 785f 6d61 696e 6e65 740a  usd_dex_mainnet.
-00001240: 2020 2020 2020 746f 6b65 6e5f 636f 6e74        token_cont
-00001250: 7261 6374 3a20 6b75 7364 5f74 6f6b 656e  ract: kusd_token
-00001260: 5f6d 6169 6e6e 6574 0a20 2020 2020 2073  _mainnet.      s
-00001270: 796d 626f 6c3a 206b 5553 440a 2020 2020  ymbol: kUSD.    
-00001280: 2020 6465 6369 6d61 6c73 3a20 3138 0a0a    decimals: 18..
-00001290: 2020 6864 616f 5f6d 6169 6e6e 6574 3a0a    hdao_mainnet:.
-000012a0: 2020 2020 7465 6d70 6c61 7465 3a20 7175      template: qu
-000012b0: 6970 7573 7761 705f 6661 320a 2020 2020  ipuswap_fa2.    
-000012c0: 7661 6c75 6573 3a0a 2020 2020 2020 6465  values:.      de
-000012d0: 785f 636f 6e74 7261 6374 3a20 6864 616f  x_contract: hdao
-000012e0: 5f64 6578 5f6d 6169 6e6e 6574 0a20 2020  _dex_mainnet.   
-000012f0: 2020 2074 6f6b 656e 5f63 6f6e 7472 6163     token_contrac
-00001300: 743a 2068 6461 6f5f 746f 6b65 6e5f 6d61  t: hdao_token_ma
-00001310: 696e 6e65 740a 2020 2020 2020 7379 6d62  innet.      symb
-00001320: 6f6c 3a20 6844 414f 0a20 2020 2020 2064  ol: hDAO.      d
-00001330: 6563 696d 616c 733a 2036 0a              ecimals: 6.
+00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
+00000020: 6465 780a 0a63 6f6e 7472 6163 7473 3a0a  dex..contracts:.
+00000030: 2020 6b75 7364 5f64 6578 5f6d 6169 6e6e    kusd_dex_mainn
+00000040: 6574 3a0a 2020 2020 6b69 6e64 3a20 7465  et:.    kind: te
+00000050: 7a6f 730a 2020 2020 6164 6472 6573 733a  zos.    address:
+00000060: 204b 5431 4b34 4577 5470 6276 594e 3961   KT1K4EwTpbvYN9a
+00000070: 674a 646a 7079 4a6d 345a 5a64 6870 554e  gJdjpyJm4ZZdhpUN
+00000080: 4b42 3346 360a 2020 2020 7479 7065 6e61  KB3F6.    typena
+00000090: 6d65 3a20 7175 6970 755f 6661 3132 0a20  me: quipu_fa12. 
+000000a0: 206b 7573 645f 746f 6b65 6e5f 6d61 696e   kusd_token_main
+000000b0: 6e65 743a 0a20 2020 206b 696e 643a 2074  net:.    kind: t
+000000c0: 657a 6f73 0a20 2020 2061 6464 7265 7373  ezos.    address
+000000d0: 3a20 4b54 314b 3967 4352 6761 4c52 464b  : KT1K9gCRgaLRFK
+000000e0: 5445 7259 7431 7756 7841 3346 7262 3946  TErYt1wVxA3Frb9F
+000000f0: 6a61 736a 5456 0a20 2020 2074 7970 656e  jasjTV.    typen
+00000100: 616d 653a 2066 6131 325f 746f 6b65 6e0a  ame: fa12_token.
+00000110: 2020 6864 616f 5f64 6578 5f6d 6169 6e6e    hdao_dex_mainn
+00000120: 6574 3a0a 2020 2020 6b69 6e64 3a20 7465  et:.    kind: te
+00000130: 7a6f 730a 2020 2020 6164 6472 6573 733a  zos.    address:
+00000140: 204b 5431 5178 4c71 756b 7966 6f68 5056   KT1QxLqukyfohPV
+00000150: 356b 506b 7739 3752 7336 6377 3144 4444  5kPkw97Rs6cw1DDD
+00000160: 7659 6762 420a 2020 2020 7479 7065 6e61  vYgbB.    typena
+00000170: 6d65 3a20 7175 6970 755f 6661 320a 2020  me: quipu_fa2.  
+00000180: 6864 616f 5f74 6f6b 656e 5f6d 6169 6e6e  hdao_token_mainn
+00000190: 6574 3a0a 2020 2020 6b69 6e64 3a20 7465  et:.    kind: te
+000001a0: 7a6f 730a 2020 2020 6164 6472 6573 733a  zos.    address:
+000001b0: 204b 5431 4146 4132 6d77 4e55 4d4e 6434   KT1AFA2mwNUMNd4
+000001c0: 5373 756a 4531 5959 7032 3976 6438 425a  SsujE1YYp29vd8BZ
+000001d0: 656a 794b 570a 2020 2020 7479 7065 6e61  ejyKW.    typena
+000001e0: 6d65 3a20 6661 325f 746f 6b65 6e0a 0a64  me: fa2_token..d
+000001f0: 6174 6173 6f75 7263 6573 3a0a 2020 747a  atasources:.  tz
+00000200: 6b74 5f6d 6169 6e6e 6574 3a0a 2020 2020  kt_mainnet:.    
+00000210: 6b69 6e64 3a20 7465 7a6f 732e 747a 6b74  kind: tezos.tzkt
+00000220: 0a20 2020 2075 726c 3a20 6874 7470 733a  .    url: https:
+00000230: 2f2f 6170 692e 747a 6b74 2e69 6f0a 0a74  //api.tzkt.io..t
+00000240: 656d 706c 6174 6573 3a0a 2020 7175 6970  emplates:.  quip
+00000250: 7573 7761 705f 6661 3132 3a0a 2020 2020  uswap_fa12:.    
+00000260: 6b69 6e64 3a20 7465 7a6f 732e 747a 6b74  kind: tezos.tzkt
+00000270: 2e6f 7065 7261 7469 6f6e 730a 2020 2020  .operations.    
+00000280: 6461 7461 736f 7572 6365 3a20 747a 6b74  datasource: tzkt
+00000290: 5f6d 6169 6e6e 6574 0a20 2020 2063 6f6e  _mainnet.    con
+000002a0: 7472 6163 7473 3a0a 2020 2020 2020 2d20  tracts:.      - 
+000002b0: 3c64 6578 5f63 6f6e 7472 6163 743e 0a20  <dex_contract>. 
+000002c0: 2020 2074 7970 6573 3a0a 2020 2020 2020     types:.      
+000002d0: 2d20 7472 616e 7361 6374 696f 6e0a 2020  - transaction.  
+000002e0: 2020 2020 2d20 6f72 6967 696e 6174 696f      - originatio
+000002f0: 6e0a 2020 2020 6861 6e64 6c65 7273 3a0a  n.    handlers:.
+00000300: 2020 2020 2020 2d20 6361 6c6c 6261 636b        - callback
+00000310: 3a20 6f6e 5f66 6131 325f 6f72 6967 696e  : on_fa12_origin
+00000320: 6174 696f 6e0a 2020 2020 2020 2020 7061  ation.        pa
+00000330: 7474 6572 6e3a 0a20 2020 2020 2020 2020  ttern:.         
+00000340: 202d 2074 7970 653a 206f 7269 6769 6e61   - type: origina
+00000350: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+00000360: 206f 7269 6769 6e61 7465 645f 636f 6e74   originated_cont
+00000370: 7261 6374 3a20 3c64 6578 5f63 6f6e 7472  ract: <dex_contr
+00000380: 6163 743e 0a20 2020 2020 202d 2063 616c  act>.      - cal
+00000390: 6c62 6163 6b3a 206f 6e5f 6661 3132 5f74  lback: on_fa12_t
+000003a0: 6f6b 656e 5f74 6f5f 7465 7a0a 2020 2020  oken_to_tez.    
+000003b0: 2020 2020 7061 7474 6572 6e3a 0a20 2020      pattern:.   
+000003c0: 2020 2020 2020 202d 2074 7970 653a 2074         - type: t
+000003d0: 7261 6e73 6163 7469 6f6e 0a20 2020 2020  ransaction.     
+000003e0: 2020 2020 2020 2064 6573 7469 6e61 7469         destinati
+000003f0: 6f6e 3a20 3c64 6578 5f63 6f6e 7472 6163  on: <dex_contrac
+00000400: 743e 0a20 2020 2020 2020 2020 2020 2065  t>.            e
+00000410: 6e74 7279 706f 696e 743a 2074 6f6b 656e  ntrypoint: token
+00000420: 546f 5465 7a50 6179 6d65 6e74 0a20 2020  ToTezPayment.   
+00000430: 2020 2020 2020 202d 2074 7970 653a 2074         - type: t
+00000440: 7261 6e73 6163 7469 6f6e 0a20 2020 2020  ransaction.     
+00000450: 2020 2020 2020 2064 6573 7469 6e61 7469         destinati
+00000460: 6f6e 3a20 3c74 6f6b 656e 5f63 6f6e 7472  on: <token_contr
+00000470: 6163 743e 0a20 2020 2020 2020 2020 2020  act>.           
+00000480: 2065 6e74 7279 706f 696e 743a 2074 7261   entrypoint: tra
+00000490: 6e73 6665 720a 2020 2020 2020 2020 2020  nsfer.          
+000004a0: 2d20 7479 7065 3a20 7472 616e 7361 6374  - type: transact
+000004b0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+000004c0: 736f 7572 6365 3a20 3c64 6578 5f63 6f6e  source: <dex_con
+000004d0: 7472 6163 743e 0a20 2020 2020 202d 2063  tract>.      - c
+000004e0: 616c 6c62 6163 6b3a 206f 6e5f 6661 3132  allback: on_fa12
+000004f0: 5f74 657a 5f74 6f5f 746f 6b65 6e0a 2020  _tez_to_token.  
+00000500: 2020 2020 2020 7061 7474 6572 6e3a 0a20        pattern:. 
+00000510: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
+00000520: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
+00000530: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
+00000540: 7469 6f6e 3a20 3c64 6578 5f63 6f6e 7472  tion: <dex_contr
+00000550: 6163 743e 0a20 2020 2020 2020 2020 2020  act>.           
+00000560: 2065 6e74 7279 706f 696e 743a 2074 657a   entrypoint: tez
+00000570: 546f 546f 6b65 6e50 6179 6d65 6e74 0a20  ToTokenPayment. 
+00000580: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
+00000590: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
+000005a0: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
+000005b0: 7469 6f6e 3a20 3c74 6f6b 656e 5f63 6f6e  tion: <token_con
+000005c0: 7472 6163 743e 0a20 2020 2020 2020 2020  tract>.         
+000005d0: 2020 2065 6e74 7279 706f 696e 743a 2074     entrypoint: t
+000005e0: 7261 6e73 6665 720a 2020 2020 2020 2d20  ransfer.      - 
+000005f0: 6361 6c6c 6261 636b 3a20 6f6e 5f66 6131  callback: on_fa1
+00000600: 325f 696e 7665 7374 5f6c 6971 7569 6469  2_invest_liquidi
+00000610: 7479 0a20 2020 2020 2020 2070 6174 7465  ty.        patte
+00000620: 726e 3a0a 2020 2020 2020 2020 2020 2d20  rn:.          - 
+00000630: 7479 7065 3a20 7472 616e 7361 6374 696f  type: transactio
+00000640: 6e0a 2020 2020 2020 2020 2020 2020 6465  n.            de
+00000650: 7374 696e 6174 696f 6e3a 203c 6465 785f  stination: <dex_
+00000660: 636f 6e74 7261 6374 3e0a 2020 2020 2020  contract>.      
+00000670: 2020 2020 2020 656e 7472 7970 6f69 6e74        entrypoint
+00000680: 3a20 696e 7665 7374 4c69 7175 6964 6974  : investLiquidit
+00000690: 790a 2020 2020 2020 2020 2020 2d20 7479  y.          - ty
+000006a0: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
+000006b0: 2020 2020 2020 2020 2020 2020 6465 7374              dest
+000006c0: 696e 6174 696f 6e3a 203c 746f 6b65 6e5f  ination: <token_
+000006d0: 636f 6e74 7261 6374 3e0a 2020 2020 2020  contract>.      
+000006e0: 2020 2020 2020 656e 7472 7970 6f69 6e74        entrypoint
+000006f0: 3a20 7472 616e 7366 6572 0a20 2020 2020  : transfer.     
+00000700: 202d 2063 616c 6c62 6163 6b3a 206f 6e5f   - callback: on_
+00000710: 6661 3132 5f74 7261 6e73 6665 720a 2020  fa12_transfer.  
+00000720: 2020 2020 2020 7061 7474 6572 6e3a 0a20        pattern:. 
+00000730: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
+00000740: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
+00000750: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
+00000760: 7469 6f6e 3a20 3c64 6578 5f63 6f6e 7472  tion: <dex_contr
+00000770: 6163 743e 0a20 2020 2020 2020 2020 2020  act>.           
+00000780: 2065 6e74 7279 706f 696e 743a 2074 7261   entrypoint: tra
+00000790: 6e73 6665 720a 2020 2020 2020 2d20 6361  nsfer.      - ca
+000007a0: 6c6c 6261 636b 3a20 6f6e 5f66 6131 325f  llback: on_fa12_
+000007b0: 6469 7665 7374 5f6c 6971 7569 6469 7479  divest_liquidity
+000007c0: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
+000007d0: 3a0a 2020 2020 2020 2020 2020 2d20 7479  :.          - ty
+000007e0: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
+000007f0: 2020 2020 2020 2020 2020 2020 6465 7374              dest
+00000800: 696e 6174 696f 6e3a 203c 6465 785f 636f  ination: <dex_co
+00000810: 6e74 7261 6374 3e0a 2020 2020 2020 2020  ntract>.        
+00000820: 2020 2020 656e 7472 7970 6f69 6e74 3a20      entrypoint: 
+00000830: 6469 7665 7374 4c69 7175 6964 6974 790a  divestLiquidity.
+00000840: 2020 2020 2020 2020 2020 2d20 7479 7065            - type
+00000850: 3a20 7472 616e 7361 6374 696f 6e0a 2020  : transaction.  
+00000860: 2020 2020 2020 2020 2020 6465 7374 696e            destin
+00000870: 6174 696f 6e3a 203c 746f 6b65 6e5f 636f  ation: <token_co
+00000880: 6e74 7261 6374 3e0a 2020 2020 2020 2020  ntract>.        
+00000890: 2020 2020 656e 7472 7970 6f69 6e74 3a20      entrypoint: 
+000008a0: 7472 616e 7366 6572 0a20 2020 2020 2020  transfer.       
+000008b0: 2020 202d 2074 7970 653a 2074 7261 6e73     - type: trans
+000008c0: 6163 7469 6f6e 0a20 2020 2020 2020 2020  action.         
+000008d0: 2020 2073 6f75 7263 653a 203c 6465 785f     source: <dex_
+000008e0: 636f 6e74 7261 6374 3e0a 2020 2020 2020  contract>.      
+000008f0: 2d20 6361 6c6c 6261 636b 3a20 6f6e 5f66  - callback: on_f
+00000900: 6131 325f 7769 7468 6472 6177 5f70 726f  a12_withdraw_pro
+00000910: 6669 740a 2020 2020 2020 2020 7061 7474  fit.        patt
+00000920: 6572 6e3a 0a20 2020 2020 2020 2020 202d  ern:.          -
+00000930: 2074 7970 653a 2074 7261 6e73 6163 7469   type: transacti
+00000940: 6f6e 0a20 2020 2020 2020 2020 2020 2064  on.            d
+00000950: 6573 7469 6e61 7469 6f6e 3a20 3c64 6578  estination: <dex
+00000960: 5f63 6f6e 7472 6163 743e 0a20 2020 2020  _contract>.     
+00000970: 2020 2020 2020 2065 6e74 7279 706f 696e         entrypoin
+00000980: 743a 2077 6974 6864 7261 7750 726f 6669  t: withdrawProfi
+00000990: 740a 2020 2020 2020 2020 2020 2d20 7479  t.          - ty
+000009a0: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
+000009b0: 2020 2020 2020 2020 2020 2020 736f 7572              sour
+000009c0: 6365 3a20 3c64 6578 5f63 6f6e 7472 6163  ce: <dex_contrac
+000009d0: 743e 0a20 2020 2020 2020 2020 2020 206f  t>.            o
+000009e0: 7074 696f 6e61 6c3a 2054 7275 650a 0a20  ptional: True.. 
+000009f0: 2071 7569 7075 7377 6170 5f66 6132 3a0a   quipuswap_fa2:.
+00000a00: 2020 2020 6b69 6e64 3a20 7465 7a6f 732e      kind: tezos.
+00000a10: 747a 6b74 2e6f 7065 7261 7469 6f6e 730a  tzkt.operations.
+00000a20: 2020 2020 6461 7461 736f 7572 6365 3a20      datasource: 
+00000a30: 747a 6b74 5f6d 6169 6e6e 6574 0a20 2020  tzkt_mainnet.   
+00000a40: 2063 6f6e 7472 6163 7473 3a0a 2020 2020   contracts:.    
+00000a50: 2020 2d20 3c64 6578 5f63 6f6e 7472 6163    - <dex_contrac
+00000a60: 743e 0a20 2020 2074 7970 6573 3a0a 2020  t>.    types:.  
+00000a70: 2020 2020 2d20 7472 616e 7361 6374 696f      - transactio
+00000a80: 6e0a 2020 2020 2020 2d20 6f72 6967 696e  n.      - origin
+00000a90: 6174 696f 6e0a 2020 2020 6861 6e64 6c65  ation.    handle
+00000aa0: 7273 3a0a 2020 2020 2020 2d20 6361 6c6c  rs:.      - call
+00000ab0: 6261 636b 3a20 6f6e 5f66 6132 5f6f 7269  back: on_fa2_ori
+00000ac0: 6769 6e61 7469 6f6e 0a20 2020 2020 2020  gination.       
+00000ad0: 2070 6174 7465 726e 3a0a 2020 2020 2020   pattern:.      
+00000ae0: 2020 2020 2d20 7479 7065 3a20 6f72 6967      - type: orig
+00000af0: 696e 6174 696f 6e0a 2020 2020 2020 2020  ination.        
+00000b00: 2020 2020 6f72 6967 696e 6174 6564 5f63      originated_c
+00000b10: 6f6e 7472 6163 743a 203c 6465 785f 636f  ontract: <dex_co
+00000b20: 6e74 7261 6374 3e0a 2020 2020 2020 2d20  ntract>.      - 
+00000b30: 6361 6c6c 6261 636b 3a20 6f6e 5f66 6132  callback: on_fa2
+00000b40: 5f74 6f6b 656e 5f74 6f5f 7465 7a0a 2020  _token_to_tez.  
+00000b50: 2020 2020 2020 7061 7474 6572 6e3a 0a20        pattern:. 
+00000b60: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
+00000b70: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
+00000b80: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
+00000b90: 7469 6f6e 3a20 3c64 6578 5f63 6f6e 7472  tion: <dex_contr
+00000ba0: 6163 743e 0a20 2020 2020 2020 2020 2020  act>.           
+00000bb0: 2065 6e74 7279 706f 696e 743a 2074 6f6b   entrypoint: tok
+00000bc0: 656e 546f 5465 7a50 6179 6d65 6e74 0a20  enToTezPayment. 
+00000bd0: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
+00000be0: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
+00000bf0: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
+00000c00: 7469 6f6e 3a20 3c74 6f6b 656e 5f63 6f6e  tion: <token_con
+00000c10: 7472 6163 743e 0a20 2020 2020 2020 2020  tract>.         
+00000c20: 2020 2065 6e74 7279 706f 696e 743a 2074     entrypoint: t
+00000c30: 7261 6e73 6665 720a 2020 2020 2020 2020  ransfer.        
+00000c40: 2020 2d20 7479 7065 3a20 7472 616e 7361    - type: transa
+00000c50: 6374 696f 6e0a 2020 2020 2020 2020 2020  ction.          
+00000c60: 2020 736f 7572 6365 3a20 3c64 6578 5f63    source: <dex_c
+00000c70: 6f6e 7472 6163 743e 0a20 2020 2020 202d  ontract>.      -
+00000c80: 2063 616c 6c62 6163 6b3a 206f 6e5f 6661   callback: on_fa
+00000c90: 325f 7465 7a5f 746f 5f74 6f6b 656e 0a20  2_tez_to_token. 
+00000ca0: 2020 2020 2020 2070 6174 7465 726e 3a0a         pattern:.
+00000cb0: 2020 2020 2020 2020 2020 2d20 7479 7065            - type
+00000cc0: 3a20 7472 616e 7361 6374 696f 6e0a 2020  : transaction.  
+00000cd0: 2020 2020 2020 2020 2020 6465 7374 696e            destin
+00000ce0: 6174 696f 6e3a 203c 6465 785f 636f 6e74  ation: <dex_cont
+00000cf0: 7261 6374 3e0a 2020 2020 2020 2020 2020  ract>.          
+00000d00: 2020 656e 7472 7970 6f69 6e74 3a20 7465    entrypoint: te
+00000d10: 7a54 6f54 6f6b 656e 5061 796d 656e 740a  zToTokenPayment.
+00000d20: 2020 2020 2020 2020 2020 2d20 7479 7065            - type
+00000d30: 3a20 7472 616e 7361 6374 696f 6e0a 2020  : transaction.  
+00000d40: 2020 2020 2020 2020 2020 6465 7374 696e            destin
+00000d50: 6174 696f 6e3a 203c 746f 6b65 6e5f 636f  ation: <token_co
+00000d60: 6e74 7261 6374 3e0a 2020 2020 2020 2020  ntract>.        
+00000d70: 2020 2020 656e 7472 7970 6f69 6e74 3a20      entrypoint: 
+00000d80: 7472 616e 7366 6572 0a20 2020 2020 202d  transfer.      -
+00000d90: 2063 616c 6c62 6163 6b3a 206f 6e5f 6661   callback: on_fa
+00000da0: 325f 696e 7665 7374 5f6c 6971 7569 6469  2_invest_liquidi
+00000db0: 7479 0a20 2020 2020 2020 2070 6174 7465  ty.        patte
+00000dc0: 726e 3a0a 2020 2020 2020 2020 2020 2d20  rn:.          - 
+00000dd0: 7479 7065 3a20 7472 616e 7361 6374 696f  type: transactio
+00000de0: 6e0a 2020 2020 2020 2020 2020 2020 6465  n.            de
+00000df0: 7374 696e 6174 696f 6e3a 203c 6465 785f  stination: <dex_
+00000e00: 636f 6e74 7261 6374 3e0a 2020 2020 2020  contract>.      
+00000e10: 2020 2020 2020 656e 7472 7970 6f69 6e74        entrypoint
+00000e20: 3a20 696e 7665 7374 4c69 7175 6964 6974  : investLiquidit
+00000e30: 790a 2020 2020 2020 2020 2020 2d20 7479  y.          - ty
+00000e40: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
+00000e50: 2020 2020 2020 2020 2020 2020 6465 7374              dest
+00000e60: 696e 6174 696f 6e3a 203c 746f 6b65 6e5f  ination: <token_
+00000e70: 636f 6e74 7261 6374 3e0a 2020 2020 2020  contract>.      
+00000e80: 2020 2020 2020 656e 7472 7970 6f69 6e74        entrypoint
+00000e90: 3a20 7472 616e 7366 6572 0a20 2020 2020  : transfer.     
+00000ea0: 202d 2063 616c 6c62 6163 6b3a 206f 6e5f   - callback: on_
+00000eb0: 6661 325f 7472 616e 7366 6572 0a20 2020  fa2_transfer.   
+00000ec0: 2020 2020 2070 6174 7465 726e 3a0a 2020       pattern:.  
+00000ed0: 2020 2020 2020 2020 2d20 7479 7065 3a20          - type: 
+00000ee0: 7472 616e 7361 6374 696f 6e0a 2020 2020  transaction.    
+00000ef0: 2020 2020 2020 2020 6465 7374 696e 6174          destinat
+00000f00: 696f 6e3a 203c 6465 785f 636f 6e74 7261  ion: <dex_contra
+00000f10: 6374 3e0a 2020 2020 2020 2020 2020 2020  ct>.            
+00000f20: 656e 7472 7970 6f69 6e74 3a20 7472 616e  entrypoint: tran
+00000f30: 7366 6572 0a20 2020 2020 202d 2063 616c  sfer.      - cal
+00000f40: 6c62 6163 6b3a 206f 6e5f 6661 325f 6469  lback: on_fa2_di
+00000f50: 7665 7374 5f6c 6971 7569 6469 7479 0a20  vest_liquidity. 
+00000f60: 2020 2020 2020 2070 6174 7465 726e 3a0a         pattern:.
+00000f70: 2020 2020 2020 2020 2020 2d20 7479 7065            - type
+00000f80: 3a20 7472 616e 7361 6374 696f 6e0a 2020  : transaction.  
+00000f90: 2020 2020 2020 2020 2020 6465 7374 696e            destin
+00000fa0: 6174 696f 6e3a 203c 6465 785f 636f 6e74  ation: <dex_cont
+00000fb0: 7261 6374 3e0a 2020 2020 2020 2020 2020  ract>.          
+00000fc0: 2020 656e 7472 7970 6f69 6e74 3a20 6469    entrypoint: di
+00000fd0: 7665 7374 4c69 7175 6964 6974 790a 2020  vestLiquidity.  
+00000fe0: 2020 2020 2020 2020 2d20 7479 7065 3a20          - type: 
+00000ff0: 7472 616e 7361 6374 696f 6e0a 2020 2020  transaction.    
+00001000: 2020 2020 2020 2020 6465 7374 696e 6174          destinat
+00001010: 696f 6e3a 203c 746f 6b65 6e5f 636f 6e74  ion: <token_cont
+00001020: 7261 6374 3e0a 2020 2020 2020 2020 2020  ract>.          
+00001030: 2020 656e 7472 7970 6f69 6e74 3a20 7472    entrypoint: tr
+00001040: 616e 7366 6572 0a20 2020 2020 2020 2020  ansfer.         
+00001050: 202d 2074 7970 653a 2074 7261 6e73 6163   - type: transac
+00001060: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+00001070: 2073 6f75 7263 653a 203c 6465 785f 636f   source: <dex_co
+00001080: 6e74 7261 6374 3e0a 2020 2020 2020 2d20  ntract>.      - 
+00001090: 6361 6c6c 6261 636b 3a20 6f6e 5f66 6132  callback: on_fa2
+000010a0: 5f77 6974 6864 7261 775f 7072 6f66 6974  _withdraw_profit
+000010b0: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
+000010c0: 3a0a 2020 2020 2020 2020 2020 2d20 7479  :.          - ty
+000010d0: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
+000010e0: 2020 2020 2020 2020 2020 2020 6465 7374              dest
+000010f0: 696e 6174 696f 6e3a 203c 6465 785f 636f  ination: <dex_co
+00001100: 6e74 7261 6374 3e0a 2020 2020 2020 2020  ntract>.        
+00001110: 2020 2020 656e 7472 7970 6f69 6e74 3a20      entrypoint: 
+00001120: 7769 7468 6472 6177 5072 6f66 6974 0a20  withdrawProfit. 
+00001130: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
+00001140: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
+00001150: 2020 2020 2020 2020 2073 6f75 7263 653a           source:
+00001160: 203c 6465 785f 636f 6e74 7261 6374 3e0a   <dex_contract>.
+00001170: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
+00001180: 6f6e 616c 3a20 5472 7565 0a0a 696e 6465  onal: True..inde
+00001190: 7865 733a 0a20 206b 7573 645f 6d61 696e  xes:.  kusd_main
+000011a0: 6e65 743a 0a20 2020 2074 656d 706c 6174  net:.    templat
+000011b0: 653a 2071 7569 7075 7377 6170 5f66 6131  e: quipuswap_fa1
+000011c0: 320a 2020 2020 7661 6c75 6573 3a0a 2020  2.    values:.  
+000011d0: 2020 2020 6465 785f 636f 6e74 7261 6374      dex_contract
+000011e0: 3a20 6b75 7364 5f64 6578 5f6d 6169 6e6e  : kusd_dex_mainn
+000011f0: 6574 0a20 2020 2020 2074 6f6b 656e 5f63  et.      token_c
+00001200: 6f6e 7472 6163 743a 206b 7573 645f 746f  ontract: kusd_to
+00001210: 6b65 6e5f 6d61 696e 6e65 740a 2020 2020  ken_mainnet.    
+00001220: 2020 7379 6d62 6f6c 3a20 6b55 5344 0a20    symbol: kUSD. 
+00001230: 2020 2020 2064 6563 696d 616c 733a 2031       decimals: 1
+00001240: 380a 0a20 2068 6461 6f5f 6d61 696e 6e65  8..  hdao_mainne
+00001250: 743a 0a20 2020 2074 656d 706c 6174 653a  t:.    template:
+00001260: 2071 7569 7075 7377 6170 5f66 6132 0a20   quipuswap_fa2. 
+00001270: 2020 2076 616c 7565 733a 0a20 2020 2020     values:.     
+00001280: 2064 6578 5f63 6f6e 7472 6163 743a 2068   dex_contract: h
+00001290: 6461 6f5f 6465 785f 6d61 696e 6e65 740a  dao_dex_mainnet.
+000012a0: 2020 2020 2020 746f 6b65 6e5f 636f 6e74        token_cont
+000012b0: 7261 6374 3a20 6864 616f 5f74 6f6b 656e  ract: hdao_token
+000012c0: 5f6d 6169 6e6e 6574 0a20 2020 2020 2073  _mainnet.      s
+000012d0: 796d 626f 6c3a 2068 4441 4f0a 2020 2020  ymbol: hDAO.    
+000012e0: 2020 6465 6369 6d61 6c73 3a20 36           decimals: 6
```

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa12_divest_liquidity.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_divest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa12_invest_liquidity.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_invest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa12_origination.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_origination.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa12_tez_to_token.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_tez_to_token.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa12_token_to_tez.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_token_to_tez.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa12_transfer.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa12_withdraw_profit.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa12_withdraw_profit.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_divest_liquidity.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_divest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_invest_liquidity.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_invest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_origination.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_origination.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_tez_to_token.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_tez_to_token.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_token_to_tez.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_token_to_tez.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_transfer.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_withdraw_profit.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/handlers/on_fa2_withdraw_profit.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/models/__init__.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_dex/models/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_domains/dipdup.yaml.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_domains/dipdup.yaml.j2`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,54 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 207b 7b20 7072  0.package: {{ pr
 00000020: 6f6a 6563 742e 7061 636b 6167 6520 7d7d  oject.package }}
-00000030: 0a0a 6461 7461 6261 7365 3a0a 2020 6b69  ..database:.  ki
-00000040: 6e64 3a20 7371 6c69 7465 0a20 2070 6174  nd: sqlite.  pat
-00000050: 683a 207b 7b20 7072 6f6a 6563 742e 7061  h: {{ project.pa
-00000060: 636b 6167 6520 7d7d 2e73 716c 6974 6533  ckage }}.sqlite3
-00000070: 0a0a 636f 6e74 7261 6374 733a 0a20 206d  ..contracts:.  m
-00000080: 6169 6e6e 6574 5f6e 616d 655f 7265 6769  ainnet_name_regi
-00000090: 7374 7279 3a0a 2020 2020 6b69 6e64 3a20  stry:.    kind: 
-000000a0: 7465 7a6f 730a 2020 2020 6164 6472 6573  tezos.    addres
-000000b0: 733a 204b 5431 4742 5a6d 5378 6d6e 4b4a  s: KT1GBZmSxmnKJ
-000000c0: 5847 4d64 4d4c 6275 6750 664c 7955 506d  XGMdMLbugPfLyUPm
-000000d0: 754c 534d 774b 530a 2020 2020 7479 7065  uLSMwKS.    type
-000000e0: 6e61 6d65 3a20 6e61 6d65 5f72 6567 6973  name: name_regis
-000000f0: 7472 790a 0a64 6174 6173 6f75 7263 6573  try..datasources
-00000100: 3a0a 2020 747a 6b74 5f6d 6169 6e6e 6574  :.  tzkt_mainnet
-00000110: 3a0a 2020 2020 6b69 6e64 3a20 7465 7a6f  :.    kind: tezo
-00000120: 732e 747a 6b74 0a20 2020 2075 726c 3a20  s.tzkt.    url: 
-00000130: 247b 545a 4b54 5f55 524c 3a2d 6874 7470  ${TZKT_URL:-http
-00000140: 733a 2f2f 6170 692e 747a 6b74 2e69 6f7d  s://api.tzkt.io}
-00000150: 0a0a 7465 6d70 6c61 7465 733a 0a20 2064  ..templates:.  d
-00000160: 6f6d 6169 6e73 3a0a 2020 2020 6b69 6e64  omains:.    kind
-00000170: 3a20 7465 7a6f 732e 747a 6b74 2e6f 7065  : tezos.tzkt.ope
-00000180: 7261 7469 6f6e 730a 2020 2020 6461 7461  rations.    data
-00000190: 736f 7572 6365 3a20 3c64 6174 6173 6f75  source: <datasou
-000001a0: 7263 653e 0a20 2020 2063 6f6e 7472 6163  rce>.    contrac
-000001b0: 7473 3a0a 2020 2020 2020 2d20 3c6e 616d  ts:.      - <nam
-000001c0: 655f 7265 6769 7374 7279 3e0a 2020 2020  e_registry>.    
-000001d0: 6861 6e64 6c65 7273 3a0a 2020 2020 2020  handlers:.      
-000001e0: 2d20 6361 6c6c 6261 636b 3a20 6f6e 5f61  - callback: on_a
-000001f0: 646d 696e 5f75 7064 6174 650a 2020 2020  dmin_update.    
-00000200: 2020 2020 7061 7474 6572 6e3a 0a20 2020      pattern:.   
-00000210: 2020 2020 2020 202d 2074 7970 653a 2074         - type: t
-00000220: 7261 6e73 6163 7469 6f6e 0a20 2020 2020  ransaction.     
-00000230: 2020 2020 2020 2064 6573 7469 6e61 7469         destinati
-00000240: 6f6e 3a20 3c6e 616d 655f 7265 6769 7374  on: <name_regist
-00000250: 7279 3e0a 2020 2020 2020 2020 2020 2020  ry>.            
-00000260: 656e 7472 7970 6f69 6e74 3a20 6164 6d69  entrypoint: admi
-00000270: 6e5f 7570 6461 7465 0a20 2020 2020 202d  n_update.      -
-00000280: 2063 616c 6c62 6163 6b3a 206f 6e5f 6578   callback: on_ex
-00000290: 6563 7574 650a 2020 2020 2020 2020 7061  ecute.        pa
-000002a0: 7474 6572 6e3a 0a20 2020 2020 2020 2020  ttern:.         
-000002b0: 202d 2074 7970 653a 2074 7261 6e73 6163   - type: transac
-000002c0: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-000002d0: 2064 6573 7469 6e61 7469 6f6e 3a20 3c6e   destination: <n
-000002e0: 616d 655f 7265 6769 7374 7279 3e0a 2020  ame_registry>.  
-000002f0: 2020 2020 2020 2020 2020 656e 7472 7970            entryp
-00000300: 6f69 6e74 3a20 6578 6563 7574 650a 0a69  oint: execute..i
-00000310: 6e64 6578 6573 3a0a 2020 646f 6d61 696e  ndexes:.  domain
-00000320: 735f 6d61 696e 6e65 743a 0a20 2020 2074  s_mainnet:.    t
-00000330: 656d 706c 6174 653a 2064 6f6d 6169 6e73  emplate: domains
-00000340: 0a20 2020 2076 616c 7565 733a 0a20 2020  .    values:.   
-00000350: 2020 2064 6174 6173 6f75 7263 653a 2074     datasource: t
-00000360: 7a6b 745f 6d61 696e 6e65 740a 2020 2020  zkt_mainnet.    
-00000370: 2020 6e61 6d65 5f72 6567 6973 7472 793a    name_registry:
-00000380: 206d 6169 6e6e 6574 5f6e 616d 655f 7265   mainnet_name_re
-00000390: 6769 7374 7279 0a                        gistry.
+00000030: 0a0a 636f 6e74 7261 6374 733a 0a20 206d  ..contracts:.  m
+00000040: 6169 6e6e 6574 5f6e 616d 655f 7265 6769  ainnet_name_regi
+00000050: 7374 7279 3a0a 2020 2020 6b69 6e64 3a20  stry:.    kind: 
+00000060: 7465 7a6f 730a 2020 2020 6164 6472 6573  tezos.    addres
+00000070: 733a 204b 5431 4742 5a6d 5378 6d6e 4b4a  s: KT1GBZmSxmnKJ
+00000080: 5847 4d64 4d4c 6275 6750 664c 7955 506d  XGMdMLbugPfLyUPm
+00000090: 754c 534d 774b 530a 2020 2020 7479 7065  uLSMwKS.    type
+000000a0: 6e61 6d65 3a20 6e61 6d65 5f72 6567 6973  name: name_regis
+000000b0: 7472 790a 0a64 6174 6173 6f75 7263 6573  try..datasources
+000000c0: 3a0a 2020 747a 6b74 5f6d 6169 6e6e 6574  :.  tzkt_mainnet
+000000d0: 3a0a 2020 2020 6b69 6e64 3a20 7465 7a6f  :.    kind: tezo
+000000e0: 732e 747a 6b74 0a20 2020 2075 726c 3a20  s.tzkt.    url: 
+000000f0: 247b 545a 4b54 5f55 524c 3a2d 6874 7470  ${TZKT_URL:-http
+00000100: 733a 2f2f 6170 692e 747a 6b74 2e69 6f7d  s://api.tzkt.io}
+00000110: 0a0a 7465 6d70 6c61 7465 733a 0a20 2064  ..templates:.  d
+00000120: 6f6d 6169 6e73 3a0a 2020 2020 6b69 6e64  omains:.    kind
+00000130: 3a20 7465 7a6f 732e 747a 6b74 2e6f 7065  : tezos.tzkt.ope
+00000140: 7261 7469 6f6e 730a 2020 2020 6461 7461  rations.    data
+00000150: 736f 7572 6365 3a20 3c64 6174 6173 6f75  source: <datasou
+00000160: 7263 653e 0a20 2020 2063 6f6e 7472 6163  rce>.    contrac
+00000170: 7473 3a0a 2020 2020 2020 2d20 3c6e 616d  ts:.      - <nam
+00000180: 655f 7265 6769 7374 7279 3e0a 2020 2020  e_registry>.    
+00000190: 6861 6e64 6c65 7273 3a0a 2020 2020 2020  handlers:.      
+000001a0: 2d20 6361 6c6c 6261 636b 3a20 6f6e 5f61  - callback: on_a
+000001b0: 646d 696e 5f75 7064 6174 650a 2020 2020  dmin_update.    
+000001c0: 2020 2020 7061 7474 6572 6e3a 0a20 2020      pattern:.   
+000001d0: 2020 2020 2020 202d 2074 7970 653a 2074         - type: t
+000001e0: 7261 6e73 6163 7469 6f6e 0a20 2020 2020  ransaction.     
+000001f0: 2020 2020 2020 2064 6573 7469 6e61 7469         destinati
+00000200: 6f6e 3a20 3c6e 616d 655f 7265 6769 7374  on: <name_regist
+00000210: 7279 3e0a 2020 2020 2020 2020 2020 2020  ry>.            
+00000220: 656e 7472 7970 6f69 6e74 3a20 6164 6d69  entrypoint: admi
+00000230: 6e5f 7570 6461 7465 0a20 2020 2020 202d  n_update.      -
+00000240: 2063 616c 6c62 6163 6b3a 206f 6e5f 6578   callback: on_ex
+00000250: 6563 7574 650a 2020 2020 2020 2020 7061  ecute.        pa
+00000260: 7474 6572 6e3a 0a20 2020 2020 2020 2020  ttern:.         
+00000270: 202d 2074 7970 653a 2074 7261 6e73 6163   - type: transac
+00000280: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+00000290: 2064 6573 7469 6e61 7469 6f6e 3a20 3c6e   destination: <n
+000002a0: 616d 655f 7265 6769 7374 7279 3e0a 2020  ame_registry>.  
+000002b0: 2020 2020 2020 2020 2020 656e 7472 7970            entryp
+000002c0: 6f69 6e74 3a20 6578 6563 7574 650a 0a69  oint: execute..i
+000002d0: 6e64 6578 6573 3a0a 2020 646f 6d61 696e  ndexes:.  domain
+000002e0: 735f 6d61 696e 6e65 743a 0a20 2020 2074  s_mainnet:.    t
+000002f0: 656d 706c 6174 653a 2064 6f6d 6169 6e73  emplate: domains
+00000300: 0a20 2020 2076 616c 7565 733a 0a20 2020  .    values:.   
+00000310: 2020 2064 6174 6173 6f75 7263 653a 2074     datasource: t
+00000320: 7a6b 745f 6d61 696e 6e65 740a 2020 2020  zkt_mainnet.    
+00000330: 2020 6e61 6d65 5f72 6567 6973 7472 793a    name_registry:
+00000340: 206d 6169 6e6e 6574 5f6e 616d 655f 7265   mainnet_name_re
+00000350: 6769 7374 7279 0a                        gistry.
```

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_domains/handlers/on_admin_update.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_domains/handlers/on_admin_update.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_domains/handlers/on_execute.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_domains/handlers/on_execute.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_domains/handlers/on_storage_diff.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_domains/handlers/on_storage_diff.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_domains/models/__init__.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_domains/models/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_events/dipdup.yaml.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_events/dipdup.yaml.j2`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 207b 7b20 7072  0.package: {{ pr
 00000020: 6f6a 6563 742e 7061 636b 6167 6520 7d7d  oject.package }}
-00000030: 0a0a 6461 7461 6261 7365 3a0a 2020 6b69  ..database:.  ki
-00000040: 6e64 3a20 7371 6c69 7465 0a20 2070 6174  nd: sqlite.  pat
-00000050: 683a 207b 7b20 7072 6f6a 6563 742e 7061  h: {{ project.pa
-00000060: 636b 6167 6520 7d7d 2e73 716c 6974 6533  ckage }}.sqlite3
-00000070: 0a0a 6461 7461 736f 7572 6365 733a 0a20  ..datasources:. 
-00000080: 2074 7a6b 743a 0a20 2020 206b 696e 643a   tzkt:.    kind:
-00000090: 2074 657a 6f73 2e74 7a6b 740a 2020 2020   tezos.tzkt.    
-000000a0: 7572 6c3a 2068 7474 7073 3a2f 2f61 7069  url: https://api
-000000b0: 2e67 686f 7374 6e65 742e 747a 6b74 2e69  .ghostnet.tzkt.i
-000000c0: 6f0a 0a63 6f6e 7472 6163 7473 3a0a 2020  o..contracts:.  
-000000d0: 6576 656e 7473 5f63 6f6e 7472 6163 743a  events_contract:
-000000e0: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
-000000f0: 0a20 2020 2063 6f64 655f 6861 7368 3a20  .    code_hash: 
-00000100: 4b54 3155 7036 414d 6568 7a65 3256 5464  KT1Up6AMehze2VTd
-00000110: 7433 7738 3578 615a 5074 7245 576e 3141  t3w85xaZPtrEWn1A
-00000120: 6579 5233 0a0a 696e 6465 7865 733a 0a20  eyR3..indexes:. 
-00000130: 2065 7665 6e74 733a 0a20 2020 206b 696e   events:.    kin
-00000140: 643a 2074 657a 6f73 2e74 7a6b 742e 6576  d: tezos.tzkt.ev
-00000150: 656e 7473 0a20 2020 2064 6174 6173 6f75  ents.    datasou
-00000160: 7263 653a 2074 7a6b 740a 2020 2020 6861  rce: tzkt.    ha
-00000170: 6e64 6c65 7273 3a0a 2020 2020 2020 2d20  ndlers:.      - 
-00000180: 6361 6c6c 6261 636b 3a20 6f6e 5f6d 6f76  callback: on_mov
-00000190: 655f 6576 656e 740a 2020 2020 2020 2020  e_event.        
-000001a0: 636f 6e74 7261 6374 3a20 6576 656e 7473  contract: events
-000001b0: 5f63 6f6e 7472 6163 740a 2020 2020 2020  _contract.      
-000001c0: 2020 7461 673a 206d 6f76 650a 2020 2020    tag: move.    
-000001d0: 2020 2d20 6361 6c6c 6261 636b 3a20 6f6e    - callback: on
-000001e0: 5f72 6f6c 6c5f 6576 656e 740a 2020 2020  _roll_event.    
-000001f0: 2020 2020 636f 6e74 7261 6374 3a20 6576      contract: ev
-00000200: 656e 7473 5f63 6f6e 7472 6163 740a 2020  ents_contract.  
-00000210: 2020 2020 2020 7461 673a 2072 6f6c 6c0a        tag: roll.
-00000220: 2020 2020 2020 2d20 6361 6c6c 6261 636b        - callback
-00000230: 3a20 6f6e 5f6f 7468 6572 5f65 7665 6e74  : on_other_event
-00000240: 0a20 2020 2020 2020 2063 6f6e 7472 6163  .        contrac
-00000250: 743a 2065 7665 6e74 735f 636f 6e74 7261  t: events_contra
-00000260: 6374 0a                                  ct.
+00000030: 0a0a 6461 7461 736f 7572 6365 733a 0a20  ..datasources:. 
+00000040: 2074 7a6b 743a 0a20 2020 206b 696e 643a   tzkt:.    kind:
+00000050: 2074 657a 6f73 2e74 7a6b 740a 2020 2020   tezos.tzkt.    
+00000060: 7572 6c3a 2068 7474 7073 3a2f 2f61 7069  url: https://api
+00000070: 2e67 686f 7374 6e65 742e 747a 6b74 2e69  .ghostnet.tzkt.i
+00000080: 6f0a 0a63 6f6e 7472 6163 7473 3a0a 2020  o..contracts:.  
+00000090: 6576 656e 7473 5f63 6f6e 7472 6163 743a  events_contract:
+000000a0: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
+000000b0: 0a20 2020 2063 6f64 655f 6861 7368 3a20  .    code_hash: 
+000000c0: 4b54 3155 7036 414d 6568 7a65 3256 5464  KT1Up6AMehze2VTd
+000000d0: 7433 7738 3578 615a 5074 7245 576e 3141  t3w85xaZPtrEWn1A
+000000e0: 6579 5233 0a0a 696e 6465 7865 733a 0a20  eyR3..indexes:. 
+000000f0: 2065 7665 6e74 733a 0a20 2020 206b 696e   events:.    kin
+00000100: 643a 2074 657a 6f73 2e74 7a6b 742e 6576  d: tezos.tzkt.ev
+00000110: 656e 7473 0a20 2020 2064 6174 6173 6f75  ents.    datasou
+00000120: 7263 653a 2074 7a6b 740a 2020 2020 6861  rce: tzkt.    ha
+00000130: 6e64 6c65 7273 3a0a 2020 2020 2020 2d20  ndlers:.      - 
+00000140: 6361 6c6c 6261 636b 3a20 6f6e 5f6d 6f76  callback: on_mov
+00000150: 655f 6576 656e 740a 2020 2020 2020 2020  e_event.        
+00000160: 636f 6e74 7261 6374 3a20 6576 656e 7473  contract: events
+00000170: 5f63 6f6e 7472 6163 740a 2020 2020 2020  _contract.      
+00000180: 2020 7461 673a 206d 6f76 650a 2020 2020    tag: move.    
+00000190: 2020 2d20 6361 6c6c 6261 636b 3a20 6f6e    - callback: on
+000001a0: 5f72 6f6c 6c5f 6576 656e 740a 2020 2020  _roll_event.    
+000001b0: 2020 2020 636f 6e74 7261 6374 3a20 6576      contract: ev
+000001c0: 656e 7473 5f63 6f6e 7472 6163 740a 2020  ents_contract.  
+000001d0: 2020 2020 2020 7461 673a 2072 6f6c 6c0a        tag: roll.
+000001e0: 2020 2020 2020 2d20 6361 6c6c 6261 636b        - callback
+000001f0: 3a20 6f6e 5f6f 7468 6572 5f65 7665 6e74  : on_other_event
+00000200: 0a20 2020 2020 2020 2063 6f6e 7472 6163  .        contrac
+00000210: 743a 2065 7665 6e74 735f 636f 6e74 7261  t: events_contra
+00000220: 6374 0a                                  ct.
```

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_evm_events/handlers/on_transfer.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_evm_events/handlers/on_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_factories/dipdup.yaml.j2` & `dipdup-7.0.0rc2/tests/configs/demo_dao.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
-00000010: 300a 7061 636b 6167 653a 207b 7b20 7072  0.package: {{ pr
-00000020: 6f6a 6563 742e 7061 636b 6167 6520 7d7d  oject.package }}
-00000030: 0a0a 6461 7461 6261 7365 3a0a 2020 6b69  ..database:.  ki
-00000040: 6e64 3a20 7371 6c69 7465 0a20 2070 6174  nd: sqlite.  pat
-00000050: 683a 207b 7b20 7072 6f6a 6563 742e 7061  h: {{ project.pa
-00000060: 636b 6167 6520 7d7d 2e73 716c 6974 6533  ckage }}.sqlite3
-00000070: 0a0a 636f 6e74 7261 6374 733a 0a20 2072  ..contracts:.  r
-00000080: 6567 6973 7472 793a 0a20 2020 206b 696e  egistry:.    kin
-00000090: 643a 2074 657a 6f73 0a20 2020 2061 6464  d: tezos.    add
-000000a0: 7265 7373 3a20 4b54 3139 4346 334b 4b72  ress: KT19CF3KKr
-000000b0: 7664 5737 3774 7446 6f6d 4375 696e 326b  vdW77ttFomCuin2k
-000000c0: 3475 4156 6b72 7959 7168 0a20 2020 2074  4uAVkryYqh.    t
-000000d0: 7970 656e 616d 653a 2072 6567 6973 7472  ypename: registr
-000000e0: 790a 0a64 6174 6173 6f75 7263 6573 3a0a  y..datasources:.
-000000f0: 2020 747a 6b74 3a0a 2020 2020 6b69 6e64    tzkt:.    kind
-00000100: 3a20 7465 7a6f 732e 747a 6b74 0a20 2020  : tezos.tzkt.   
-00000110: 2075 726c 3a20 247b 545a 4b54 5f55 524c   url: ${TZKT_URL
-00000120: 3a2d 6874 7470 733a 2f2f 6170 692e 747a  :-https://api.tz
-00000130: 6b74 2e69 6f7d 0a0a 696e 6465 7865 733a  kt.io}..indexes:
-00000140: 0a20 2072 6567 6973 7472 795f 6461 6f3a  .  registry_dao:
-00000150: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
-00000160: 2e74 7a6b 742e 6f70 6572 6174 696f 6e73  .tzkt.operations
-00000170: 0a20 2020 2064 6174 6173 6f75 7263 653a  .    datasource:
-00000180: 2074 7a6b 740a 2020 2020 7479 7065 733a   tzkt.    types:
-00000190: 0a20 2020 2020 202d 2074 7261 6e73 6163  .      - transac
-000001a0: 7469 6f6e 0a20 2020 2020 202d 206f 7269  tion.      - ori
-000001b0: 6769 6e61 7469 6f6e 0a20 2020 2068 616e  gination.    han
-000001c0: 646c 6572 733a 0a20 2020 2020 202d 2063  dlers:.      - c
-000001d0: 616c 6c62 6163 6b3a 206f 6e5f 6f72 6967  allback: on_orig
-000001e0: 696e 6174 696f 6e0a 2020 2020 2020 2020  ination.        
-000001f0: 7061 7474 6572 6e3a 0a20 2020 2020 2020  pattern:.       
-00000200: 2020 202d 2074 7970 653a 206f 7269 6769     - type: origi
-00000210: 6e61 7469 6f6e 0a20 2020 2020 2020 2020  nation.         
-00000220: 2020 206f 7269 6769 6e61 7465 645f 636f     originated_co
-00000230: 6e74 7261 6374 3a20 7265 6769 7374 7279  ntract: registry
-00000240: 0a20 2020 2020 202d 2063 616c 6c62 6163  .      - callbac
-00000250: 6b3a 206f 6e5f 7072 6f70 6f73 650a 2020  k: on_propose.  
-00000260: 2020 2020 2020 7061 7474 6572 6e3a 0a20        pattern:. 
-00000270: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
-00000280: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
-00000290: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
-000002a0: 7469 6f6e 3a20 7265 6769 7374 7279 0a20  tion: registry. 
-000002b0: 2020 2020 2020 2020 2020 2065 6e74 7279             entry
-000002c0: 706f 696e 743a 2070 726f 706f 7365 0a    point: propose.
+00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
+00000020: 6461 6f0a 0a63 6f6e 7472 6163 7473 3a0a  dao..contracts:.
+00000030: 2020 7265 6769 7374 7279 3a0a 2020 2020    registry:.    
+00000040: 6b69 6e64 3a20 7465 7a6f 730a 2020 2020  kind: tezos.    
+00000050: 636f 6465 5f68 6173 683a 204b 5431 3943  code_hash: KT19C
+00000060: 4633 4b4b 7276 6457 3737 7474 466f 6d43  F3KKrvdW77ttFomC
+00000070: 7569 6e32 6b34 7541 566b 7279 5971 680a  uin2k4uAVkryYqh.
+00000080: 2020 2020 7479 7065 6e61 6d65 3a20 7265      typename: re
+00000090: 6769 7374 7279 0a0a 6461 7461 736f 7572  gistry..datasour
+000000a0: 6365 733a 0a20 2074 7a6b 743a 0a20 2020  ces:.  tzkt:.   
+000000b0: 206b 696e 643a 2074 657a 6f73 2e74 7a6b   kind: tezos.tzk
+000000c0: 740a 2020 2020 7572 6c3a 2024 7b54 5a4b  t.    url: ${TZK
+000000d0: 545f 5552 4c3a 2d68 7474 7073 3a2f 2f61  T_URL:-https://a
+000000e0: 7069 2e74 7a6b 742e 696f 7d0a 2020 2020  pi.tzkt.io}.    
+000000f0: 6874 7470 3a0a 2020 2020 2020 7265 706c  http:.      repl
+00000100: 6179 5f70 6174 683a 2024 7b44 4950 4455  ay_path: ${DIPDU
+00000110: 505f 5245 504c 4159 5f50 4154 483a 2d7d  P_REPLAY_PATH:-}
+00000120: 0a0a 696e 6465 7865 733a 0a20 2072 6567  ..indexes:.  reg
+00000130: 6973 7472 795f 6461 6f3a 0a20 2020 206b  istry_dao:.    k
+00000140: 696e 643a 2074 657a 6f73 2e74 7a6b 742e  ind: tezos.tzkt.
+00000150: 6f70 6572 6174 696f 6e73 0a20 2020 2064  operations.    d
+00000160: 6174 6173 6f75 7263 653a 2074 7a6b 740a  atasource: tzkt.
+00000170: 2020 2020 7479 7065 733a 0a20 2020 2020      types:.     
+00000180: 202d 2074 7261 6e73 6163 7469 6f6e 0a20   - transaction. 
+00000190: 2020 2020 202d 206f 7269 6769 6e61 7469       - originati
+000001a0: 6f6e 0a20 2020 2068 616e 646c 6572 733a  on.    handlers:
+000001b0: 0a20 2020 2020 202d 2063 616c 6c62 6163  .      - callbac
+000001c0: 6b3a 206f 6e5f 6f72 6967 696e 6174 696f  k: on_originatio
+000001d0: 6e0a 2020 2020 2020 2020 7061 7474 6572  n.        patter
+000001e0: 6e3a 0a20 2020 2020 2020 2020 202d 2074  n:.          - t
+000001f0: 7970 653a 206f 7269 6769 6e61 7469 6f6e  ype: origination
+00000200: 0a20 2020 2020 2020 2020 2020 206f 7269  .            ori
+00000210: 6769 6e61 7465 645f 636f 6e74 7261 6374  ginated_contract
+00000220: 3a20 7265 6769 7374 7279 0a20 2020 2020  : registry.     
+00000230: 202d 2063 616c 6c62 6163 6b3a 206f 6e5f   - callback: on_
+00000240: 7072 6f70 6f73 650a 2020 2020 2020 2020  propose.        
+00000250: 7061 7474 6572 6e3a 0a20 2020 2020 2020  pattern:.       
+00000260: 2020 202d 2074 7970 653a 2074 7261 6e73     - type: trans
+00000270: 6163 7469 6f6e 0a20 2020 2020 2020 2020  action.         
+00000280: 2020 2064 6573 7469 6e61 7469 6f6e 3a20     destination: 
+00000290: 7265 6769 7374 7279 0a20 2020 2020 2020  registry.       
+000002a0: 2020 2020 2065 6e74 7279 706f 696e 743a       entrypoint:
+000002b0: 2070 726f 706f 7365 0a20 2020 2066 6972   propose.    fir
+000002c0: 7374 5f6c 6576 656c 3a20 3138 3831 3631  st_level: 188161
+000002d0: 390a 2020 2020 6c61 7374 5f6c 6576 656c  9.    last_level
+000002e0: 3a20 3239 3333 3530 35                   : 2933505
```

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_factories/handlers/on_propose.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_factories/handlers/on_propose.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_factories/models/__init__.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_factories/models/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_nft_marketplace/dipdup.yaml.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/dipdup.yaml.j2`

 * *Files 6% similar despite different names*

```diff
@@ -1,80 +1,76 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 207b 7b20 7072  0.package: {{ pr
 00000020: 6f6a 6563 742e 7061 636b 6167 6520 7d7d  oject.package }}
-00000030: 0a0a 6461 7461 6261 7365 3a0a 2020 6b69  ..database:.  ki
-00000040: 6e64 3a20 7371 6c69 7465 0a20 2070 6174  nd: sqlite.  pat
-00000050: 683a 207b 7b20 7072 6f6a 6563 742e 7061  h: {{ project.pa
-00000060: 636b 6167 6520 7d7d 2e73 716c 6974 6533  ckage }}.sqlite3
-00000070: 0a0a 6461 7461 736f 7572 6365 733a 0a20  ..datasources:. 
-00000080: 2074 7a6b 745f 6d61 696e 6e65 743a 0a20   tzkt_mainnet:. 
-00000090: 2020 206b 696e 643a 2074 657a 6f73 2e74     kind: tezos.t
-000000a0: 7a6b 740a 2020 2020 7572 6c3a 2024 7b54  zkt.    url: ${T
-000000b0: 5a4b 545f 5552 4c3a 2d68 7474 7073 3a2f  ZKT_URL:-https:/
-000000c0: 2f61 7069 2e74 7a6b 742e 696f 7d0a 0a63  /api.tzkt.io}..c
-000000d0: 6f6e 7472 6163 7473 3a0a 2020 4845 4e5f  ontracts:.  HEN_
-000000e0: 6f62 6a6b 7473 3a0a 2020 2020 6b69 6e64  objkts:.    kind
-000000f0: 3a20 7465 7a6f 730a 2020 2020 6164 6472  : tezos.    addr
-00000100: 6573 733a 2024 7b48 454e 5f4f 424a 4b54  ess: ${HEN_OBJKT
-00000110: 533a 2d4b 5431 524a 3650 626a 4870 7763  S:-KT1RJ6PbjHpwc
-00000120: 334d 3572 7735 7332 4e62 6d65 6677 6275  3M5rw5s2Nbmefwbu
-00000130: 7762 6478 746f 6e7d 0a20 2020 2074 7970  wbdxton}.    typ
-00000140: 656e 616d 653a 2068 656e 5f6f 626a 6b74  ename: hen_objkt
-00000150: 730a 2020 4845 4e5f 6d69 6e74 6572 3a0a  s.  HEN_minter:.
-00000160: 2020 2020 6b69 6e64 3a20 7465 7a6f 730a      kind: tezos.
-00000170: 2020 2020 6164 6472 6573 733a 2024 7b48      address: ${H
-00000180: 454e 5f4d 494e 5445 523a 2d4b 5431 486b  EN_MINTER:-KT1Hk
-00000190: 6735 7165 4e68 6677 704b 5734 6658 7671  g5qeNhfwpKW4fXvq
-000001a0: 3748 475a 4239 7a32 456e 6d43 4341 397d  7HGZB9z2EnmCCA9}
-000001b0: 0a20 2020 2074 7970 656e 616d 653a 2068  .    typename: h
-000001c0: 656e 5f6d 696e 7465 720a 0a69 6e64 6578  en_minter..index
-000001d0: 6573 3a0a 2020 6865 6e5f 6d61 696e 6e65  es:.  hen_mainne
-000001e0: 743a 0a20 2020 206b 696e 643a 2074 657a  t:.    kind: tez
-000001f0: 6f73 2e74 7a6b 742e 6f70 6572 6174 696f  os.tzkt.operatio
-00000200: 6e73 0a20 2020 2064 6174 6173 6f75 7263  ns.    datasourc
-00000210: 653a 2074 7a6b 745f 6d61 696e 6e65 740a  e: tzkt_mainnet.
-00000220: 2020 2020 636f 6e74 7261 6374 733a 0a20      contracts:. 
-00000230: 2020 2020 202d 2048 454e 5f6d 696e 7465       - HEN_minte
-00000240: 720a 2020 2020 6861 6e64 6c65 7273 3a0a  r.    handlers:.
-00000250: 2020 2020 2020 2d20 6361 6c6c 6261 636b        - callback
-00000260: 3a20 6f6e 5f6d 696e 740a 2020 2020 2020  : on_mint.      
-00000270: 2020 7061 7474 6572 6e3a 0a20 2020 2020    pattern:.     
-00000280: 2020 2020 202d 2074 7970 653a 2074 7261       - type: tra
-00000290: 6e73 6163 7469 6f6e 0a20 2020 2020 2020  nsaction.       
-000002a0: 2020 2020 2064 6573 7469 6e61 7469 6f6e       destination
-000002b0: 3a20 4845 4e5f 6d69 6e74 6572 0a20 2020  : HEN_minter.   
-000002c0: 2020 2020 2020 2020 2065 6e74 7279 706f           entrypo
-000002d0: 696e 743a 206d 696e 745f 4f42 4a4b 540a  int: mint_OBJKT.
-000002e0: 2020 2020 2020 2020 2020 2d20 7479 7065            - type
-000002f0: 3a20 7472 616e 7361 6374 696f 6e0a 2020  : transaction.  
-00000300: 2020 2020 2020 2020 2020 6465 7374 696e            destin
-00000310: 6174 696f 6e3a 2048 454e 5f6f 626a 6b74  ation: HEN_objkt
-00000320: 730a 2020 2020 2020 2020 2020 2020 656e  s.            en
-00000330: 7472 7970 6f69 6e74 3a20 6d69 6e74 0a20  trypoint: mint. 
-00000340: 2020 2020 202d 2063 616c 6c62 6163 6b3a       - callback:
-00000350: 206f 6e5f 7377 6170 0a20 2020 2020 2020   on_swap.       
-00000360: 2070 6174 7465 726e 3a0a 2020 2020 2020   pattern:.      
-00000370: 2020 2020 2d20 7479 7065 3a20 7472 616e      - type: tran
-00000380: 7361 6374 696f 6e0a 2020 2020 2020 2020  saction.        
-00000390: 2020 2020 6465 7374 696e 6174 696f 6e3a      destination:
-000003a0: 2048 454e 5f6d 696e 7465 720a 2020 2020   HEN_minter.    
-000003b0: 2020 2020 2020 2020 656e 7472 7970 6f69          entrypoi
-000003c0: 6e74 3a20 7377 6170 0a20 2020 2020 202d  nt: swap.      -
-000003d0: 2063 616c 6c62 6163 6b3a 206f 6e5f 6361   callback: on_ca
-000003e0: 6e63 656c 5f73 7761 700a 2020 2020 2020  ncel_swap.      
-000003f0: 2020 7061 7474 6572 6e3a 0a20 2020 2020    pattern:.     
-00000400: 2020 2020 202d 2074 7970 653a 2074 7261       - type: tra
-00000410: 6e73 6163 7469 6f6e 0a20 2020 2020 2020  nsaction.       
-00000420: 2020 2020 2064 6573 7469 6e61 7469 6f6e       destination
-00000430: 3a20 4845 4e5f 6d69 6e74 6572 0a20 2020  : HEN_minter.   
-00000440: 2020 2020 2020 2020 2065 6e74 7279 706f           entrypo
-00000450: 696e 743a 2063 616e 6365 6c5f 7377 6170  int: cancel_swap
-00000460: 0a20 2020 2020 202d 2063 616c 6c62 6163  .      - callbac
-00000470: 6b3a 206f 6e5f 636f 6c6c 6563 740a 2020  k: on_collect.  
-00000480: 2020 2020 2020 7061 7474 6572 6e3a 0a20        pattern:. 
-00000490: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
-000004a0: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
-000004b0: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
-000004c0: 7469 6f6e 3a20 4845 4e5f 6d69 6e74 6572  tion: HEN_minter
-000004d0: 0a20 2020 2020 2020 2020 2020 2065 6e74  .            ent
-000004e0: 7279 706f 696e 743a 2063 6f6c 6c65 6374  rypoint: collect
-000004f0: 0a                                       .
+00000030: 0a0a 6461 7461 736f 7572 6365 733a 0a20  ..datasources:. 
+00000040: 2074 7a6b 745f 6d61 696e 6e65 743a 0a20   tzkt_mainnet:. 
+00000050: 2020 206b 696e 643a 2074 657a 6f73 2e74     kind: tezos.t
+00000060: 7a6b 740a 2020 2020 7572 6c3a 2024 7b54  zkt.    url: ${T
+00000070: 5a4b 545f 5552 4c3a 2d68 7474 7073 3a2f  ZKT_URL:-https:/
+00000080: 2f61 7069 2e74 7a6b 742e 696f 7d0a 0a63  /api.tzkt.io}..c
+00000090: 6f6e 7472 6163 7473 3a0a 2020 4845 4e5f  ontracts:.  HEN_
+000000a0: 6f62 6a6b 7473 3a0a 2020 2020 6b69 6e64  objkts:.    kind
+000000b0: 3a20 7465 7a6f 730a 2020 2020 6164 6472  : tezos.    addr
+000000c0: 6573 733a 2024 7b48 454e 5f4f 424a 4b54  ess: ${HEN_OBJKT
+000000d0: 533a 2d4b 5431 524a 3650 626a 4870 7763  S:-KT1RJ6PbjHpwc
+000000e0: 334d 3572 7735 7332 4e62 6d65 6677 6275  3M5rw5s2Nbmefwbu
+000000f0: 7762 6478 746f 6e7d 0a20 2020 2074 7970  wbdxton}.    typ
+00000100: 656e 616d 653a 2068 656e 5f6f 626a 6b74  ename: hen_objkt
+00000110: 730a 2020 4845 4e5f 6d69 6e74 6572 3a0a  s.  HEN_minter:.
+00000120: 2020 2020 6b69 6e64 3a20 7465 7a6f 730a      kind: tezos.
+00000130: 2020 2020 6164 6472 6573 733a 2024 7b48      address: ${H
+00000140: 454e 5f4d 494e 5445 523a 2d4b 5431 486b  EN_MINTER:-KT1Hk
+00000150: 6735 7165 4e68 6677 704b 5734 6658 7671  g5qeNhfwpKW4fXvq
+00000160: 3748 475a 4239 7a32 456e 6d43 4341 397d  7HGZB9z2EnmCCA9}
+00000170: 0a20 2020 2074 7970 656e 616d 653a 2068  .    typename: h
+00000180: 656e 5f6d 696e 7465 720a 0a69 6e64 6578  en_minter..index
+00000190: 6573 3a0a 2020 6865 6e5f 6d61 696e 6e65  es:.  hen_mainne
+000001a0: 743a 0a20 2020 206b 696e 643a 2074 657a  t:.    kind: tez
+000001b0: 6f73 2e74 7a6b 742e 6f70 6572 6174 696f  os.tzkt.operatio
+000001c0: 6e73 0a20 2020 2064 6174 6173 6f75 7263  ns.    datasourc
+000001d0: 653a 2074 7a6b 745f 6d61 696e 6e65 740a  e: tzkt_mainnet.
+000001e0: 2020 2020 636f 6e74 7261 6374 733a 0a20      contracts:. 
+000001f0: 2020 2020 202d 2048 454e 5f6d 696e 7465       - HEN_minte
+00000200: 720a 2020 2020 6861 6e64 6c65 7273 3a0a  r.    handlers:.
+00000210: 2020 2020 2020 2d20 6361 6c6c 6261 636b        - callback
+00000220: 3a20 6f6e 5f6d 696e 740a 2020 2020 2020  : on_mint.      
+00000230: 2020 7061 7474 6572 6e3a 0a20 2020 2020    pattern:.     
+00000240: 2020 2020 202d 2074 7970 653a 2074 7261       - type: tra
+00000250: 6e73 6163 7469 6f6e 0a20 2020 2020 2020  nsaction.       
+00000260: 2020 2020 2064 6573 7469 6e61 7469 6f6e       destination
+00000270: 3a20 4845 4e5f 6d69 6e74 6572 0a20 2020  : HEN_minter.   
+00000280: 2020 2020 2020 2020 2065 6e74 7279 706f           entrypo
+00000290: 696e 743a 206d 696e 745f 4f42 4a4b 540a  int: mint_OBJKT.
+000002a0: 2020 2020 2020 2020 2020 2d20 7479 7065            - type
+000002b0: 3a20 7472 616e 7361 6374 696f 6e0a 2020  : transaction.  
+000002c0: 2020 2020 2020 2020 2020 6465 7374 696e            destin
+000002d0: 6174 696f 6e3a 2048 454e 5f6f 626a 6b74  ation: HEN_objkt
+000002e0: 730a 2020 2020 2020 2020 2020 2020 656e  s.            en
+000002f0: 7472 7970 6f69 6e74 3a20 6d69 6e74 0a20  trypoint: mint. 
+00000300: 2020 2020 202d 2063 616c 6c62 6163 6b3a       - callback:
+00000310: 206f 6e5f 7377 6170 0a20 2020 2020 2020   on_swap.       
+00000320: 2070 6174 7465 726e 3a0a 2020 2020 2020   pattern:.      
+00000330: 2020 2020 2d20 7479 7065 3a20 7472 616e      - type: tran
+00000340: 7361 6374 696f 6e0a 2020 2020 2020 2020  saction.        
+00000350: 2020 2020 6465 7374 696e 6174 696f 6e3a      destination:
+00000360: 2048 454e 5f6d 696e 7465 720a 2020 2020   HEN_minter.    
+00000370: 2020 2020 2020 2020 656e 7472 7970 6f69          entrypoi
+00000380: 6e74 3a20 7377 6170 0a20 2020 2020 202d  nt: swap.      -
+00000390: 2063 616c 6c62 6163 6b3a 206f 6e5f 6361   callback: on_ca
+000003a0: 6e63 656c 5f73 7761 700a 2020 2020 2020  ncel_swap.      
+000003b0: 2020 7061 7474 6572 6e3a 0a20 2020 2020    pattern:.     
+000003c0: 2020 2020 202d 2074 7970 653a 2074 7261       - type: tra
+000003d0: 6e73 6163 7469 6f6e 0a20 2020 2020 2020  nsaction.       
+000003e0: 2020 2020 2064 6573 7469 6e61 7469 6f6e       destination
+000003f0: 3a20 4845 4e5f 6d69 6e74 6572 0a20 2020  : HEN_minter.   
+00000400: 2020 2020 2020 2020 2065 6e74 7279 706f           entrypo
+00000410: 696e 743a 2063 616e 6365 6c5f 7377 6170  int: cancel_swap
+00000420: 0a20 2020 2020 202d 2063 616c 6c62 6163  .      - callbac
+00000430: 6b3a 206f 6e5f 636f 6c6c 6563 740a 2020  k: on_collect.  
+00000440: 2020 2020 2020 7061 7474 6572 6e3a 0a20        pattern:. 
+00000450: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
+00000460: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
+00000470: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
+00000480: 7469 6f6e 3a20 4845 4e5f 6d69 6e74 6572  tion: HEN_minter
+00000490: 0a20 2020 2020 2020 2020 2020 2065 6e74  .            ent
+000004a0: 7279 706f 696e 743a 2063 6f6c 6c65 6374  rypoint: collect
+000004b0: 0a                                       .
```

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_nft_marketplace/handlers/on_cancel_swap.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/handlers/on_cancel_swap.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_nft_marketplace/handlers/on_collect.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/handlers/on_collect.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_nft_marketplace/handlers/on_mint.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/handlers/on_mint.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_nft_marketplace/handlers/on_swap.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/handlers/on_swap.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_nft_marketplace/models/__init__.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_nft_marketplace/models/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_token/dipdup.yaml.j2` & `dipdup-7.0.0rc2/tests/configs/demo_token.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,45 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
-00000010: 300a 7061 636b 6167 653a 207b 7b20 7072  0.package: {{ pr
-00000020: 6f6a 6563 742e 7061 636b 6167 6520 7d7d  oject.package }}
-00000030: 0a0a 6461 7461 6261 7365 3a0a 2020 6b69  ..database:.  ki
-00000040: 6e64 3a20 7371 6c69 7465 0a20 2070 6174  nd: sqlite.  pat
-00000050: 683a 207b 7b20 7072 6f6a 6563 742e 7061  h: {{ project.pa
-00000060: 636b 6167 6520 7d7d 2e73 716c 6974 6533  ckage }}.sqlite3
-00000070: 0a0a 636f 6e74 7261 6374 733a 0a20 2074  ..contracts:.  t
-00000080: 7a62 7463 5f6d 6169 6e6e 6574 3a0a 2020  zbtc_mainnet:.  
-00000090: 2020 6b69 6e64 3a20 7465 7a6f 730a 2020    kind: tezos.  
-000000a0: 2020 6164 6472 6573 733a 204b 5431 5057    address: KT1PW
-000000b0: 7832 6d6e 4475 656f 6f64 3766 456d 6662  x2mnDueood7fEmfb
-000000c0: 4244 4b78 3144 3942 416e 6e58 6974 6e0a  BDKx1D9BAnnXitn.
-000000d0: 2020 2020 7479 7065 6e61 6d65 3a20 747a      typename: tz
-000000e0: 6274 630a 0a64 6174 6173 6f75 7263 6573  btc..datasources
-000000f0: 3a0a 2020 747a 6b74 5f6d 6169 6e6e 6574  :.  tzkt_mainnet
-00000100: 3a0a 2020 2020 6b69 6e64 3a20 7465 7a6f  :.    kind: tezo
-00000110: 732e 747a 6b74 0a20 2020 2075 726c 3a20  s.tzkt.    url: 
-00000120: 6874 7470 733a 2f2f 6170 692e 747a 6b74  https://api.tzkt
-00000130: 2e69 6f0a 0a69 6e64 6578 6573 3a0a 2020  .io..indexes:.  
-00000140: 747a 6274 635f 686f 6c64 6572 735f 6d61  tzbtc_holders_ma
-00000150: 696e 6e65 743a 0a20 2020 2074 656d 706c  innet:.    templ
-00000160: 6174 653a 2074 7a62 7463 5f68 6f6c 6465  ate: tzbtc_holde
-00000170: 7273 0a20 2020 2076 616c 7565 733a 0a20  rs.    values:. 
-00000180: 2020 2020 2063 6f6e 7472 6163 743a 2074       contract: t
-00000190: 7a62 7463 5f6d 6169 6e6e 6574 0a20 2020  zbtc_mainnet.   
-000001a0: 2020 2064 6174 6173 6f75 7263 653a 2074     datasource: t
-000001b0: 7a6b 745f 6d61 696e 6e65 740a 0a74 656d  zkt_mainnet..tem
-000001c0: 706c 6174 6573 3a0a 2020 747a 6274 635f  plates:.  tzbtc_
-000001d0: 686f 6c64 6572 733a 0a20 2020 206b 696e  holders:.    kin
-000001e0: 643a 2074 657a 6f73 2e74 7a6b 742e 6f70  d: tezos.tzkt.op
-000001f0: 6572 6174 696f 6e73 0a20 2020 2064 6174  erations.    dat
-00000200: 6173 6f75 7263 653a 203c 6461 7461 736f  asource: <dataso
-00000210: 7572 6365 3e0a 2020 2020 636f 6e74 7261  urce>.    contra
-00000220: 6374 733a 0a20 2020 2020 202d 203c 636f  cts:.      - <co
-00000230: 6e74 7261 6374 3e0a 2020 2020 6861 6e64  ntract>.    hand
-00000240: 6c65 7273 3a0a 2020 2020 2020 2d20 6361  lers:.      - ca
-00000250: 6c6c 6261 636b 3a20 6f6e 5f74 7261 6e73  llback: on_trans
-00000260: 6665 720a 2020 2020 2020 2020 7061 7474  fer.        patt
-00000270: 6572 6e3a 0a20 2020 2020 2020 2020 202d  ern:.          -
-00000280: 2064 6573 7469 6e61 7469 6f6e 3a20 3c63   destination: <c
-00000290: 6f6e 7472 6163 743e 0a20 2020 2020 2020  ontract>.       
-000002a0: 2020 2020 2065 6e74 7279 706f 696e 743a       entrypoint:
-000002b0: 2074 7261 6e73 6665 720a 2020 2020 2020   transfer.      
-000002c0: 2d20 6361 6c6c 6261 636b 3a20 6f6e 5f6d  - callback: on_m
-000002d0: 696e 740a 2020 2020 2020 2020 7061 7474  int.        patt
-000002e0: 6572 6e3a 0a20 2020 2020 2020 2020 202d  ern:.          -
-000002f0: 2064 6573 7469 6e61 7469 6f6e 3a20 3c63   destination: <c
-00000300: 6f6e 7472 6163 743e 0a20 2020 2020 2020  ontract>.       
-00000310: 2020 2020 2065 6e74 7279 706f 696e 743a       entrypoint:
-00000320: 206d 696e 740a                            mint.
+00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
+00000020: 746f 6b65 6e0a 0a63 6f6e 7472 6163 7473  token..contracts
+00000030: 3a0a 2020 747a 6274 635f 6d61 696e 6e65  :.  tzbtc_mainne
+00000040: 743a 0a20 2020 206b 696e 643a 2074 657a  t:.    kind: tez
+00000050: 6f73 0a20 2020 2061 6464 7265 7373 3a20  os.    address: 
+00000060: 4b54 3150 5778 326d 6e44 7565 6f6f 6437  KT1PWx2mnDueood7
+00000070: 6645 6d66 6242 444b 7831 4439 4241 6e6e  fEmfbBDKx1D9BAnn
+00000080: 5869 746e 0a20 2020 2074 7970 656e 616d  Xitn.    typenam
+00000090: 653a 2074 7a62 7463 0a0a 6461 7461 736f  e: tzbtc..dataso
+000000a0: 7572 6365 733a 0a20 2074 7a6b 743a 0a20  urces:.  tzkt:. 
+000000b0: 2020 206b 696e 643a 2074 657a 6f73 2e74     kind: tezos.t
+000000c0: 7a6b 740a 2020 2020 7572 6c3a 2068 7474  zkt.    url: htt
+000000d0: 7073 3a2f 2f61 7069 2e74 7a6b 742e 696f  ps://api.tzkt.io
+000000e0: 0a20 2020 2068 7474 703a 0a20 2020 2020  .    http:.     
+000000f0: 2072 6570 6c61 795f 7061 7468 3a20 247b   replay_path: ${
+00000100: 4449 5044 5550 5f52 4550 4c41 595f 5041  DIPDUP_REPLAY_PA
+00000110: 5448 3a2d 7d0a 0a69 6e64 6578 6573 3a0a  TH:-}..indexes:.
+00000120: 2020 747a 6274 635f 686f 6c64 6572 735f    tzbtc_holders_
+00000130: 6d61 696e 6e65 743a 0a20 2020 206b 696e  mainnet:.    kin
+00000140: 643a 2074 657a 6f73 2e74 7a6b 742e 6f70  d: tezos.tzkt.op
+00000150: 6572 6174 696f 6e73 0a20 2020 2064 6174  erations.    dat
+00000160: 6173 6f75 7263 653a 2074 7a6b 740a 2020  asource: tzkt.  
+00000170: 2020 636f 6e74 7261 6374 733a 0a20 2020    contracts:.   
+00000180: 2020 202d 2074 7a62 7463 5f6d 6169 6e6e     - tzbtc_mainn
+00000190: 6574 0a20 2020 2068 616e 646c 6572 733a  et.    handlers:
+000001a0: 0a20 2020 2020 202d 2063 616c 6c62 6163  .      - callbac
+000001b0: 6b3a 206f 6e5f 7472 616e 7366 6572 0a20  k: on_transfer. 
+000001c0: 2020 2020 2020 2070 6174 7465 726e 3a0a         pattern:.
+000001d0: 2020 2020 2020 2020 2020 2d20 6465 7374            - dest
+000001e0: 696e 6174 696f 6e3a 2074 7a62 7463 5f6d  ination: tzbtc_m
+000001f0: 6169 6e6e 6574 0a20 2020 2020 2020 2020  ainnet.         
+00000200: 2020 2065 6e74 7279 706f 696e 743a 2074     entrypoint: t
+00000210: 7261 6e73 6665 720a 2020 2020 2020 2d20  ransfer.      - 
+00000220: 6361 6c6c 6261 636b 3a20 6f6e 5f6d 696e  callback: on_min
+00000230: 740a 2020 2020 2020 2020 7061 7474 6572  t.        patter
+00000240: 6e3a 0a20 2020 2020 2020 2020 202d 2064  n:.          - d
+00000250: 6573 7469 6e61 7469 6f6e 3a20 747a 6274  estination: tzbt
+00000260: 635f 6d61 696e 6e65 740a 2020 2020 2020  c_mainnet.      
+00000270: 2020 2020 2020 656e 7472 7970 6f69 6e74        entrypoint
+00000280: 3a20 6d69 6e74 0a20 2020 2066 6972 7374  : mint.    first
+00000290: 5f6c 6576 656c 3a20 3133 3635 3030 300a  _level: 1365000.
+000002a0: 2020 2020 6c61 7374 5f6c 6576 656c 3a20      last_level: 
+000002b0: 3133 3636 3030 300a 0a6c 6f67 6769 6e67  1366000..logging
+000002c0: 3a20 5741 524e 0a                        : WARN.
```

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_token/handlers/on_mint.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_token/handlers/on_mint.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_token/handlers/on_transfer.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_token/handlers/on_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_token_transfers/handlers/on_balance_update.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_token_transfers/handlers/on_balance_update.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_token_transfers/handlers/on_token_transfer.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_token_transfers/handlers/on_token_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/dipdup.yaml.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/dipdup.yaml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/factory/pool_created.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/factory/pool_created.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/pool/burn.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/pool/burn.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/pool/initialize.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/pool/initialize.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/pool/mint.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/pool/mint.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/pool/swap.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/pool/swap.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/position_manager/collect.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/position_manager/collect.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/position_manager/decrease_liquidity.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/position_manager/decrease_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/position_manager/increase_liquidity.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/position_manager/increase_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/position_manager/transfer.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/handlers/position_manager/transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/models/__init__.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/models/pool.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/pool.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/models/position.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/position.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/models/repo.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/repo.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/models/tick.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/tick.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/models/token.py.j2` & `dipdup-7.0.0rc2/src/dipdup/projects/demo_uniswap/models/token.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/prometheus.py` & `dipdup-7.0.0rc2/src/dipdup/prometheus.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/pysignalr.py` & `dipdup-7.0.0rc2/src/dipdup/pysignalr.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/report.py` & `dipdup-7.0.0rc2/src/dipdup/report.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/scheduler.py` & `dipdup-7.0.0rc2/src/dipdup/scheduler.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/sentry.py` & `dipdup-7.0.0rc2/src/dipdup/sentry.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/sql/truncate_schema.sql` & `dipdup-7.0.0rc2/src/dipdup/sql/truncate_schema.sql`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/subscriptions.py` & `dipdup-7.0.0rc2/src/dipdup/subscriptions.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/sys.py` & `dipdup-7.0.0rc2/src/dipdup/sys.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/templates/models.py` & `dipdup-7.0.0rc2/src/dipdup/templates/models.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/transactions.py` & `dipdup-7.0.0rc2/src/dipdup/transactions.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/utils.py` & `dipdup-7.0.0rc2/src/dipdup/utils.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/src/dipdup/yaml.py` & `dipdup-7.0.0rc2/src/dipdup/yaml.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         return dump(self)
 
     def validate_version(self) -> None:
         config_spec_version = self['spec_version']
         if config_spec_version != __spec_version__:
             raise ConfigurationError(
                 f'Incompatible spec version: expected {__spec_version__}, got {config_spec_version}. See'
-                ' https://docs.dipdup.io/config/spec_version'
+                ' https://dipdup.io/docs/config/spec_version'
             )
 
     def _post_load_hooks(self) -> None:
         self.validate_version()
         # FIXME: Can't use `from_` field alias in dataclass
         # FIXME: See https://github.com/pydantic/pydantic/issues/4286 (fixed in upcoming v2)
         fix_dataclass_field_aliases(self)
```

### Comparing `dipdup-7.0.0rc1/tests/__init__.py` & `dipdup-7.0.0rc2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/configs/demo_auction.yml` & `dipdup-7.0.0rc2/tests/configs/demo_auction.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,80 +1,77 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
-00000020: 6175 6374 696f 6e0a 0a64 6174 6162 6173  auction..databas
-00000030: 653a 0a20 206b 696e 643a 2073 716c 6974  e:.  kind: sqlit
-00000040: 650a 2020 7061 7468 3a20 6462 2e73 716c  e.  path: db.sql
-00000050: 6974 6533 0a0a 6461 7461 736f 7572 6365  ite3..datasource
-00000060: 733a 0a20 2074 7a6b 743a 0a20 2020 206b  s:.  tzkt:.    k
-00000070: 696e 643a 2074 657a 6f73 2e74 7a6b 740a  ind: tezos.tzkt.
-00000080: 2020 2020 7572 6c3a 2024 7b54 5a4b 545f      url: ${TZKT_
-00000090: 5552 4c3a 2d68 7474 7073 3a2f 2f61 7069  URL:-https://api
-000000a0: 2e74 7a6b 742e 696f 7d0a 2020 2020 6874  .tzkt.io}.    ht
-000000b0: 7470 3a0a 2020 2020 2020 7265 706c 6179  tp:.      replay
-000000c0: 5f70 6174 683a 2024 7b44 4950 4455 505f  _path: ${DIPDUP_
-000000d0: 5245 504c 4159 5f50 4154 483a 2d7d 0a0a  REPLAY_PATH:-}..
-000000e0: 636f 6e74 7261 6374 733a 0a20 2074 7a63  contracts:.  tzc
-000000f0: 6f6c 6f72 735f 6d69 6e74 6572 3a0a 2020  olors_minter:.  
-00000100: 2020 6b69 6e64 3a20 7465 7a6f 730a 2020    kind: tezos.  
-00000110: 2020 6164 6472 6573 733a 204b 5431 4679    address: KT1Fy
-00000120: 6144 7169 4d51 5767 3745 786f 3756 5569  aDqiMQWg7Exo7VUi
-00000130: 5841 675a 6264 326b 437a 6f33 6434 730a  XAgZbd2kCzo3d4s.
-00000140: 2020 2020 7479 7065 6e61 6d65 3a20 747a      typename: tz
-00000150: 636f 6c6f 7273 5f6d 696e 7465 720a 2020  colors_minter.  
-00000160: 747a 636f 6c6f 7273 5f61 7563 7469 6f6e  tzcolors_auction
-00000170: 3a0a 2020 2020 6b69 6e64 3a20 7465 7a6f  :.    kind: tezo
-00000180: 730a 2020 2020 6164 6472 6573 733a 204b  s.    address: K
-00000190: 5431 4370 6553 514b 646b 6857 6934 7069  T1CpeSQKdkhWi4pi
-000001a0: 6e59 6373 6543 464b 6d44 6873 354d 3734  nYcseCFKmDhs5M74
-000001b0: 426b 550a 2020 2020 7479 7065 6e61 6d65  BkU.    typename
-000001c0: 3a20 747a 636f 6c6f 7273 5f61 7563 7469  : tzcolors_aucti
-000001d0: 6f6e 0a0a 0a74 656d 706c 6174 6573 3a0a  on...templates:.
-000001e0: 2020 747a 636f 6c6f 7273 5f61 7563 7469    tzcolors_aucti
-000001f0: 6f6e 3a0a 2020 2020 6b69 6e64 3a20 7465  on:.    kind: te
-00000200: 7a6f 732e 747a 6b74 2e6f 7065 7261 7469  zos.tzkt.operati
-00000210: 6f6e 730a 2020 2020 6461 7461 736f 7572  ons.    datasour
-00000220: 6365 3a20 3c64 6174 6173 6f75 7263 653e  ce: <datasource>
-00000230: 0a20 2020 2063 6f6e 7472 6163 7473 3a0a  .    contracts:.
-00000240: 2020 2020 2020 2d20 3c61 7563 7469 6f6e        - <auction
-00000250: 3e0a 2020 2020 6861 6e64 6c65 7273 3a0a  >.    handlers:.
-00000260: 2020 2020 2020 2d20 6361 6c6c 6261 636b        - callback
-00000270: 3a20 6f6e 5f63 7265 6174 655f 6175 6374  : on_create_auct
-00000280: 696f 6e0a 2020 2020 2020 2020 7061 7474  ion.        patt
-00000290: 6572 6e3a 0a20 2020 2020 2020 2020 202d  ern:.          -
-000002a0: 2074 7970 653a 2074 7261 6e73 6163 7469   type: transacti
-000002b0: 6f6e 0a20 2020 2020 2020 2020 2020 2064  on.            d
-000002c0: 6573 7469 6e61 7469 6f6e 3a20 3c61 7563  estination: <auc
-000002d0: 7469 6f6e 3e0a 2020 2020 2020 2020 2020  tion>.          
-000002e0: 2020 656e 7472 7970 6f69 6e74 3a20 6372    entrypoint: cr
-000002f0: 6561 7465 5f61 7563 7469 6f6e 0a20 2020  eate_auction.   
-00000300: 2020 202d 2063 616c 6c62 6163 6b3a 206f     - callback: o
-00000310: 6e5f 6269 640a 2020 2020 2020 2020 7061  n_bid.        pa
-00000320: 7474 6572 6e3a 0a20 2020 2020 2020 2020  ttern:.         
-00000330: 202d 2074 7970 653a 2074 7261 6e73 6163   - type: transac
-00000340: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-00000350: 2064 6573 7469 6e61 7469 6f6e 3a20 3c61   destination: <a
-00000360: 7563 7469 6f6e 3e0a 2020 2020 2020 2020  uction>.        
-00000370: 2020 2020 656e 7472 7970 6f69 6e74 3a20      entrypoint: 
-00000380: 6269 640a 2020 2020 2020 2d20 6361 6c6c  bid.      - call
-00000390: 6261 636b 3a20 6f6e 5f77 6974 6864 7261  back: on_withdra
-000003a0: 770a 2020 2020 2020 2020 7061 7474 6572  w.        patter
-000003b0: 6e3a 0a20 2020 2020 2020 2020 202d 2074  n:.          - t
-000003c0: 7970 653a 2074 7261 6e73 6163 7469 6f6e  ype: transaction
-000003d0: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-000003e0: 7469 6e61 7469 6f6e 3a20 3c61 7563 7469  tination: <aucti
-000003f0: 6f6e 3e0a 2020 2020 2020 2020 2020 2020  on>.            
-00000400: 656e 7472 7970 6f69 6e74 3a20 7769 7468  entrypoint: with
-00000410: 6472 6177 0a20 2020 2066 6972 7374 5f6c  draw.    first_l
-00000420: 6576 656c 3a20 3133 3335 3635 340a 2020  evel: 1335654.  
-00000430: 2020 6c61 7374 5f6c 6576 656c 3a20 3133    last_level: 13
-00000440: 3430 3635 340a 0a69 6e64 6578 6573 3a0a  40654..indexes:.
-00000450: 2020 747a 636f 6c6f 7273 5f61 7563 7469    tzcolors_aucti
-00000460: 6f6e 3a0a 2020 2020 7465 6d70 6c61 7465  on:.    template
-00000470: 3a20 747a 636f 6c6f 7273 5f61 7563 7469  : tzcolors_aucti
-00000480: 6f6e 0a20 2020 2076 616c 7565 733a 0a20  on.    values:. 
-00000490: 2020 2020 2064 6174 6173 6f75 7263 653a       datasource:
-000004a0: 2074 7a6b 740a 2020 2020 2020 6d69 6e74   tzkt.      mint
-000004b0: 6572 3a20 747a 636f 6c6f 7273 5f6d 696e  er: tzcolors_min
-000004c0: 7465 720a 2020 2020 2020 6175 6374 696f  ter.      auctio
-000004d0: 6e3a 2074 7a63 6f6c 6f72 735f 6175 6374  n: tzcolors_auct
-000004e0: 696f 6e0a 0a6c 6f67 6769 6e67 3a20 5741  ion..logging: WA
-000004f0: 524e 0a                                  RN.
+00000020: 6175 6374 696f 6e0a 0a64 6174 6173 6f75  auction..datasou
+00000030: 7263 6573 3a0a 2020 747a 6b74 3a0a 2020  rces:.  tzkt:.  
+00000040: 2020 6b69 6e64 3a20 7465 7a6f 732e 747a    kind: tezos.tz
+00000050: 6b74 0a20 2020 2075 726c 3a20 247b 545a  kt.    url: ${TZ
+00000060: 4b54 5f55 524c 3a2d 6874 7470 733a 2f2f  KT_URL:-https://
+00000070: 6170 692e 747a 6b74 2e69 6f7d 0a20 2020  api.tzkt.io}.   
+00000080: 2068 7474 703a 0a20 2020 2020 2072 6570   http:.      rep
+00000090: 6c61 795f 7061 7468 3a20 247b 4449 5044  lay_path: ${DIPD
+000000a0: 5550 5f52 4550 4c41 595f 5041 5448 3a2d  UP_REPLAY_PATH:-
+000000b0: 7d0a 0a63 6f6e 7472 6163 7473 3a0a 2020  }..contracts:.  
+000000c0: 747a 636f 6c6f 7273 5f6d 696e 7465 723a  tzcolors_minter:
+000000d0: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
+000000e0: 0a20 2020 2061 6464 7265 7373 3a20 4b54  .    address: KT
+000000f0: 3146 7961 4471 694d 5157 6737 4578 6f37  1FyaDqiMQWg7Exo7
+00000100: 5655 6958 4167 5a62 6432 6b43 7a6f 3364  VUiXAgZbd2kCzo3d
+00000110: 3473 0a20 2020 2074 7970 656e 616d 653a  4s.    typename:
+00000120: 2074 7a63 6f6c 6f72 735f 6d69 6e74 6572   tzcolors_minter
+00000130: 0a20 2074 7a63 6f6c 6f72 735f 6175 6374  .  tzcolors_auct
+00000140: 696f 6e3a 0a20 2020 206b 696e 643a 2074  ion:.    kind: t
+00000150: 657a 6f73 0a20 2020 2061 6464 7265 7373  ezos.    address
+00000160: 3a20 4b54 3143 7065 5351 4b64 6b68 5769  : KT1CpeSQKdkhWi
+00000170: 3470 696e 5963 7365 4346 4b6d 4468 7335  4pinYcseCFKmDhs5
+00000180: 4d37 3442 6b55 0a20 2020 2074 7970 656e  M74BkU.    typen
+00000190: 616d 653a 2074 7a63 6f6c 6f72 735f 6175  ame: tzcolors_au
+000001a0: 6374 696f 6e0a 0a0a 7465 6d70 6c61 7465  ction...template
+000001b0: 733a 0a20 2074 7a63 6f6c 6f72 735f 6175  s:.  tzcolors_au
+000001c0: 6374 696f 6e3a 0a20 2020 206b 696e 643a  ction:.    kind:
+000001d0: 2074 657a 6f73 2e74 7a6b 742e 6f70 6572   tezos.tzkt.oper
+000001e0: 6174 696f 6e73 0a20 2020 2064 6174 6173  ations.    datas
+000001f0: 6f75 7263 653a 203c 6461 7461 736f 7572  ource: <datasour
+00000200: 6365 3e0a 2020 2020 636f 6e74 7261 6374  ce>.    contract
+00000210: 733a 0a20 2020 2020 202d 203c 6175 6374  s:.      - <auct
+00000220: 696f 6e3e 0a20 2020 2068 616e 646c 6572  ion>.    handler
+00000230: 733a 0a20 2020 2020 202d 2063 616c 6c62  s:.      - callb
+00000240: 6163 6b3a 206f 6e5f 6372 6561 7465 5f61  ack: on_create_a
+00000250: 7563 7469 6f6e 0a20 2020 2020 2020 2070  uction.        p
+00000260: 6174 7465 726e 3a0a 2020 2020 2020 2020  attern:.        
+00000270: 2020 2d20 7479 7065 3a20 7472 616e 7361    - type: transa
+00000280: 6374 696f 6e0a 2020 2020 2020 2020 2020  ction.          
+00000290: 2020 6465 7374 696e 6174 696f 6e3a 203c    destination: <
+000002a0: 6175 6374 696f 6e3e 0a20 2020 2020 2020  auction>.       
+000002b0: 2020 2020 2065 6e74 7279 706f 696e 743a       entrypoint:
+000002c0: 2063 7265 6174 655f 6175 6374 696f 6e0a   create_auction.
+000002d0: 2020 2020 2020 2d20 6361 6c6c 6261 636b        - callback
+000002e0: 3a20 6f6e 5f62 6964 0a20 2020 2020 2020  : on_bid.       
+000002f0: 2070 6174 7465 726e 3a0a 2020 2020 2020   pattern:.      
+00000300: 2020 2020 2d20 7479 7065 3a20 7472 616e      - type: tran
+00000310: 7361 6374 696f 6e0a 2020 2020 2020 2020  saction.        
+00000320: 2020 2020 6465 7374 696e 6174 696f 6e3a      destination:
+00000330: 203c 6175 6374 696f 6e3e 0a20 2020 2020   <auction>.     
+00000340: 2020 2020 2020 2065 6e74 7279 706f 696e         entrypoin
+00000350: 743a 2062 6964 0a20 2020 2020 202d 2063  t: bid.      - c
+00000360: 616c 6c62 6163 6b3a 206f 6e5f 7769 7468  allback: on_with
+00000370: 6472 6177 0a20 2020 2020 2020 2070 6174  draw.        pat
+00000380: 7465 726e 3a0a 2020 2020 2020 2020 2020  tern:.          
+00000390: 2d20 7479 7065 3a20 7472 616e 7361 6374  - type: transact
+000003a0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+000003b0: 6465 7374 696e 6174 696f 6e3a 203c 6175  destination: <au
+000003c0: 6374 696f 6e3e 0a20 2020 2020 2020 2020  ction>.         
+000003d0: 2020 2065 6e74 7279 706f 696e 743a 2077     entrypoint: w
+000003e0: 6974 6864 7261 770a 2020 2020 6669 7273  ithdraw.    firs
+000003f0: 745f 6c65 7665 6c3a 2031 3333 3536 3534  t_level: 1335654
+00000400: 0a20 2020 206c 6173 745f 6c65 7665 6c3a  .    last_level:
+00000410: 2031 3334 3036 3534 0a0a 696e 6465 7865   1340654..indexe
+00000420: 733a 0a20 2074 7a63 6f6c 6f72 735f 6175  s:.  tzcolors_au
+00000430: 6374 696f 6e3a 0a20 2020 2074 656d 706c  ction:.    templ
+00000440: 6174 653a 2074 7a63 6f6c 6f72 735f 6175  ate: tzcolors_au
+00000450: 6374 696f 6e0a 2020 2020 7661 6c75 6573  ction.    values
+00000460: 3a0a 2020 2020 2020 6461 7461 736f 7572  :.      datasour
+00000470: 6365 3a20 747a 6b74 0a20 2020 2020 206d  ce: tzkt.      m
+00000480: 696e 7465 723a 2074 7a63 6f6c 6f72 735f  inter: tzcolors_
+00000490: 6d69 6e74 6572 0a20 2020 2020 2061 7563  minter.      auc
+000004a0: 7469 6f6e 3a20 747a 636f 6c6f 7273 5f61  tion: tzcolors_a
+000004b0: 7563 7469 6f6e 0a0a 6c6f 6767 696e 673a  uction..logging:
+000004c0: 2057 4152 4e0a                            WARN.
```

### Comparing `dipdup-7.0.0rc1/tests/configs/demo_big_maps.yml` & `dipdup-7.0.0rc2/tests/configs/demo_factories.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
-00000020: 6269 675f 6d61 7073 0a0a 6461 7461 6261  big_maps..databa
-00000030: 7365 3a0a 2020 6b69 6e64 3a20 7371 6c69  se:.  kind: sqli
-00000040: 7465 0a20 2070 6174 683a 2064 622e 7371  te.  path: db.sq
-00000050: 6c69 7465 330a 0a63 6f6e 7472 6163 7473  lite3..contracts
-00000060: 3a0a 2020 6e61 6d65 5f72 6567 6973 7472  :.  name_registr
-00000070: 793a 0a20 2020 206b 696e 643a 2074 657a  y:.    kind: tez
-00000080: 6f73 0a20 2020 2061 6464 7265 7373 3a20  os.    address: 
-00000090: 4b54 3147 425a 6d53 786d 6e4b 4a58 474d  KT1GBZmSxmnKJXGM
-000000a0: 644d 4c62 7567 5066 4c79 5550 6d75 4c53  dMLbugPfLyUPmuLS
-000000b0: 4d77 4b53 0a20 2020 2074 7970 656e 616d  MwKS.    typenam
-000000c0: 653a 206e 616d 655f 7265 6769 7374 7279  e: name_registry
-000000d0: 0a0a 6461 7461 736f 7572 6365 733a 0a20  ..datasources:. 
-000000e0: 2074 7a6b 743a 0a20 2020 206b 696e 643a   tzkt:.    kind:
-000000f0: 2074 657a 6f73 2e74 7a6b 740a 2020 2020   tezos.tzkt.    
-00000100: 7572 6c3a 2024 7b54 5a4b 545f 5552 4c3a  url: ${TZKT_URL:
-00000110: 2d68 7474 7073 3a2f 2f61 7069 2e74 7a6b  -https://api.tzk
-00000120: 742e 696f 7d0a 2020 2020 6874 7470 3a0a  t.io}.    http:.
-00000130: 2020 2020 2020 7265 706c 6179 5f70 6174        replay_pat
-00000140: 683a 2024 7b44 4950 4455 505f 5245 504c  h: ${DIPDUP_REPL
-00000150: 4159 5f50 4154 483a 2d7d 0a0a 7465 6d70  AY_PATH:-}..temp
-00000160: 6c61 7465 733a 0a20 2062 6967 5f6d 6170  lates:.  big_map
-00000170: 733a 0a20 2020 206b 696e 643a 2074 657a  s:.    kind: tez
-00000180: 6f73 2e74 7a6b 742e 6269 675f 6d61 7073  os.tzkt.big_maps
-00000190: 0a20 2020 2064 6174 6173 6f75 7263 653a  .    datasource:
-000001a0: 203c 6461 7461 736f 7572 6365 3e0a 2020   <datasource>.  
-000001b0: 2020 6861 6e64 6c65 7273 3a0a 2020 2020    handlers:.    
-000001c0: 2020 2d20 6361 6c6c 6261 636b 3a20 6f6e    - callback: on
-000001d0: 5f75 7064 6174 655f 7265 636f 7264 730a  _update_records.
-000001e0: 2020 2020 2020 2020 636f 6e74 7261 6374          contract
-000001f0: 3a20 3c6e 616d 655f 7265 6769 7374 7279  : <name_registry
-00000200: 3e0a 2020 2020 2020 2020 7061 7468 3a20  >.        path: 
-00000210: 7374 6f72 652e 7265 636f 7264 730a 2020  store.records.  
-00000220: 2020 2020 2d20 6361 6c6c 6261 636b 3a20      - callback: 
-00000230: 6f6e 5f75 7064 6174 655f 6578 7069 7279  on_update_expiry
-00000240: 5f6d 6170 0a20 2020 2020 2020 2063 6f6e  _map.        con
-00000250: 7472 6163 743a 203c 6e61 6d65 5f72 6567  tract: <name_reg
-00000260: 6973 7472 793e 0a20 2020 2020 2020 2070  istry>.        p
-00000270: 6174 683a 2073 746f 7265 2e65 7870 6972  ath: store.expir
-00000280: 795f 6d61 700a 0a69 6e64 6578 6573 3a0a  y_map..indexes:.
-00000290: 2020 6269 675f 6d61 7073 3a0a 2020 2020    big_maps:.    
-000002a0: 7465 6d70 6c61 7465 3a20 6269 675f 6d61  template: big_ma
-000002b0: 7073 0a20 2020 2066 6972 7374 5f6c 6576  ps.    first_lev
-000002c0: 656c 3a20 3134 3135 3835 320a 2020 2020  el: 1415852.    
-000002d0: 6c61 7374 5f6c 6576 656c 3a20 3134 3138  last_level: 1418
-000002e0: 3830 300a 2020 2020 7661 6c75 6573 3a0a  800.    values:.
-000002f0: 2020 2020 2020 6461 7461 736f 7572 6365        datasource
-00000300: 3a20 747a 6b74 0a20 2020 2020 206e 616d  : tzkt.      nam
-00000310: 655f 7265 6769 7374 7279 3a20 6e61 6d65  e_registry: name
-00000320: 5f72 6567 6973 7472 790a 0a6c 6f67 6769  _registry..loggi
-00000330: 6e67 3a20 5741 524e 0a                   ng: WARN.
+00000020: 6661 6374 6f72 6965 730a 0a63 6f6e 7472  factories..contr
+00000030: 6163 7473 3a0a 2020 7265 6769 7374 7279  acts:.  registry
+00000040: 3a0a 2020 2020 6b69 6e64 3a20 7465 7a6f  :.    kind: tezo
+00000050: 730a 2020 2020 636f 6465 5f68 6173 683a  s.    code_hash:
+00000060: 204b 5431 3943 4633 4b4b 7276 6457 3737   KT19CF3KKrvdW77
+00000070: 7474 466f 6d43 7569 6e32 6b34 7541 566b  ttFomCuin2k4uAVk
+00000080: 7279 5971 680a 2020 2020 7479 7065 6e61  ryYqh.    typena
+00000090: 6d65 3a20 7265 6769 7374 7279 0a0a 6461  me: registry..da
+000000a0: 7461 736f 7572 6365 733a 0a20 2074 7a6b  tasources:.  tzk
+000000b0: 743a 0a20 2020 206b 696e 643a 2074 657a  t:.    kind: tez
+000000c0: 6f73 2e74 7a6b 740a 2020 2020 7572 6c3a  os.tzkt.    url:
+000000d0: 2024 7b54 5a4b 545f 5552 4c3a 2d68 7474   ${TZKT_URL:-htt
+000000e0: 7073 3a2f 2f61 7069 2e74 7a6b 742e 696f  ps://api.tzkt.io
+000000f0: 7d0a 2020 2020 6874 7470 3a0a 2020 2020  }.    http:.    
+00000100: 2020 7265 706c 6179 5f70 6174 683a 2024    replay_path: $
+00000110: 7b44 4950 4455 505f 5245 504c 4159 5f50  {DIPDUP_REPLAY_P
+00000120: 4154 483a 2d7d 0a0a 7465 6d70 6c61 7465  ATH:-}..template
+00000130: 733a 0a0a 2020 7265 6769 7374 7279 5f64  s:..  registry_d
+00000140: 616f 3a0a 2020 2020 6b69 6e64 3a20 7465  ao:.    kind: te
+00000150: 7a6f 732e 747a 6b74 2e6f 7065 7261 7469  zos.tzkt.operati
+00000160: 6f6e 730a 2020 2020 6461 7461 736f 7572  ons.    datasour
+00000170: 6365 3a20 747a 6b74 0a20 2020 2074 7970  ce: tzkt.    typ
+00000180: 6573 3a0a 2020 2020 2020 2d20 7472 616e  es:.      - tran
+00000190: 7361 6374 696f 6e0a 2020 2020 2020 2d20  saction.      - 
+000001a0: 6f72 6967 696e 6174 696f 6e0a 2020 2020  origination.    
+000001b0: 636f 6e74 7261 6374 733a 0a20 2020 2020  contracts:.     
+000001c0: 202d 203c 636f 6e74 7261 6374 3e0a 2020   - <contract>.  
+000001d0: 2020 6861 6e64 6c65 7273 3a0a 2020 2020    handlers:.    
+000001e0: 2020 2d20 6361 6c6c 6261 636b 3a20 6f6e    - callback: on
+000001f0: 5f70 726f 706f 7365 0a20 2020 2020 2020  _propose.       
+00000200: 2070 6174 7465 726e 3a0a 2020 2020 2020   pattern:.      
+00000210: 2020 2020 2d20 7479 7065 3a20 7472 616e      - type: tran
+00000220: 7361 6374 696f 6e0a 2020 2020 2020 2020  saction.        
+00000230: 2020 2020 6465 7374 696e 6174 696f 6e3a      destination:
+00000240: 203c 636f 6e74 7261 6374 3e0a 2020 2020   <contract>.    
+00000250: 2020 2020 2020 2020 656e 7472 7970 6f69          entrypoi
+00000260: 6e74 3a20 7072 6f70 6f73 650a 2020 2020  nt: propose.    
+00000270: 2020 2d20 6361 6c6c 6261 636b 3a20 6f6e    - callback: on
+00000280: 5f6f 7269 6769 6e61 7469 6f6e 0a20 2020  _origination.   
+00000290: 2020 2020 2070 6174 7465 726e 3a0a 2020       pattern:.  
+000002a0: 2020 2020 2020 2020 2d20 7479 7065 3a20          - type: 
+000002b0: 6f72 6967 696e 6174 696f 6e0a 2020 2020  origination.    
+000002c0: 2020 2020 2020 2020 6f72 6967 696e 6174          originat
+000002d0: 6564 5f63 6f6e 7472 6163 743a 203c 636f  ed_contract: <co
+000002e0: 6e74 7261 6374 3e0a 0a69 6e64 6578 6573  ntract>..indexes
+000002f0: 3a0a 2020 7265 6769 7374 7279 3a0a 2020  :.  registry:.  
+00000300: 2020 7465 6d70 6c61 7465 3a20 7265 6769    template: regi
+00000310: 7374 7279 5f64 616f 0a20 2020 2076 616c  stry_dao.    val
+00000320: 7565 733a 0a20 2020 2020 2063 6f6e 7472  ues:.      contr
+00000330: 6163 743a 2072 6567 6973 7472 790a 2020  act: registry.  
+00000340: 2020 6669 7273 745f 6c65 7665 6c3a 2031    first_level: 1
+00000350: 3838 3136 3139 0a20 2020 206c 6173 745f  881619.    last_
+00000360: 6c65 7665 6c3a 2032 3933 3335 3035       level: 2933505
```

### Comparing `dipdup-7.0.0rc1/tests/configs/demo_dao.yml` & `dipdup-7.0.0rc2/src/demo_factories/dipdup.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,41 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
-00000020: 6461 6f0a 0a64 6174 6162 6173 653a 0a20  dao..database:. 
-00000030: 206b 696e 643a 2073 716c 6974 650a 2020   kind: sqlite.  
-00000040: 7061 7468 3a20 6462 2e73 716c 6974 6533  path: db.sqlite3
-00000050: 0a0a 636f 6e74 7261 6374 733a 0a20 2072  ..contracts:.  r
-00000060: 6567 6973 7472 793a 0a20 2020 206b 696e  egistry:.    kin
-00000070: 643a 2074 657a 6f73 0a20 2020 2063 6f64  d: tezos.    cod
-00000080: 655f 6861 7368 3a20 4b54 3139 4346 334b  e_hash: KT19CF3K
-00000090: 4b72 7664 5737 3774 7446 6f6d 4375 696e  KrvdW77ttFomCuin
-000000a0: 326b 3475 4156 6b72 7959 7168 0a20 2020  2k4uAVkryYqh.   
-000000b0: 2074 7970 656e 616d 653a 2072 6567 6973   typename: regis
-000000c0: 7472 790a 0a64 6174 6173 6f75 7263 6573  try..datasources
-000000d0: 3a0a 2020 747a 6b74 3a0a 2020 2020 6b69  :.  tzkt:.    ki
-000000e0: 6e64 3a20 7465 7a6f 732e 747a 6b74 0a20  nd: tezos.tzkt. 
-000000f0: 2020 2075 726c 3a20 247b 545a 4b54 5f55     url: ${TZKT_U
-00000100: 524c 3a2d 6874 7470 733a 2f2f 6170 692e  RL:-https://api.
-00000110: 747a 6b74 2e69 6f7d 0a20 2020 2068 7474  tzkt.io}.    htt
-00000120: 703a 0a20 2020 2020 2072 6570 6c61 795f  p:.      replay_
-00000130: 7061 7468 3a20 247b 4449 5044 5550 5f52  path: ${DIPDUP_R
-00000140: 4550 4c41 595f 5041 5448 3a2d 7d0a 0a69  EPLAY_PATH:-}..i
-00000150: 6e64 6578 6573 3a0a 2020 7265 6769 7374  ndexes:.  regist
-00000160: 7279 5f64 616f 3a0a 2020 2020 6b69 6e64  ry_dao:.    kind
-00000170: 3a20 7465 7a6f 732e 747a 6b74 2e6f 7065  : tezos.tzkt.ope
-00000180: 7261 7469 6f6e 730a 2020 2020 6461 7461  rations.    data
-00000190: 736f 7572 6365 3a20 747a 6b74 0a20 2020  source: tzkt.   
-000001a0: 2074 7970 6573 3a0a 2020 2020 2020 2d20   types:.      - 
-000001b0: 7472 616e 7361 6374 696f 6e0a 2020 2020  transaction.    
-000001c0: 2020 2d20 6f72 6967 696e 6174 696f 6e0a    - origination.
-000001d0: 2020 2020 6861 6e64 6c65 7273 3a0a 2020      handlers:.  
-000001e0: 2020 2020 2d20 6361 6c6c 6261 636b 3a20      - callback: 
-000001f0: 6f6e 5f6f 7269 6769 6e61 7469 6f6e 0a20  on_origination. 
-00000200: 2020 2020 2020 2070 6174 7465 726e 3a0a         pattern:.
-00000210: 2020 2020 2020 2020 2020 2d20 7479 7065            - type
-00000220: 3a20 6f72 6967 696e 6174 696f 6e0a 2020  : origination.  
-00000230: 2020 2020 2020 2020 2020 6f72 6967 696e            origin
-00000240: 6174 6564 5f63 6f6e 7472 6163 743a 2072  ated_contract: r
-00000250: 6567 6973 7472 790a 2020 2020 2020 2d20  egistry.      - 
-00000260: 6361 6c6c 6261 636b 3a20 6f6e 5f70 726f  callback: on_pro
-00000270: 706f 7365 0a20 2020 2020 2020 2070 6174  pose.        pat
-00000280: 7465 726e 3a0a 2020 2020 2020 2020 2020  tern:.          
-00000290: 2d20 7479 7065 3a20 7472 616e 7361 6374  - type: transact
-000002a0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-000002b0: 6465 7374 696e 6174 696f 6e3a 2072 6567  destination: reg
-000002c0: 6973 7472 790a 2020 2020 2020 2020 2020  istry.          
-000002d0: 2020 656e 7472 7970 6f69 6e74 3a20 7072    entrypoint: pr
-000002e0: 6f70 6f73 650a 2020 2020 6669 7273 745f  opose.    first_
-000002f0: 6c65 7665 6c3a 2031 3838 3136 3139 0a20  level: 1881619. 
-00000300: 2020 206c 6173 745f 6c65 7665 6c3a 2032     last_level: 2
-00000310: 3933 3335 3035                           933505
+00000020: 6661 6374 6f72 6965 730a 0a63 6f6e 7472  factories..contr
+00000030: 6163 7473 3a0a 2020 7265 6769 7374 7279  acts:.  registry
+00000040: 3a0a 2020 2020 6b69 6e64 3a20 7465 7a6f  :.    kind: tezo
+00000050: 730a 2020 2020 6164 6472 6573 733a 204b  s.    address: K
+00000060: 5431 3943 4633 4b4b 7276 6457 3737 7474  T19CF3KKrvdW77tt
+00000070: 466f 6d43 7569 6e32 6b34 7541 566b 7279  FomCuin2k4uAVkry
+00000080: 5971 680a 2020 2020 7479 7065 6e61 6d65  Yqh.    typename
+00000090: 3a20 7265 6769 7374 7279 0a0a 6461 7461  : registry..data
+000000a0: 736f 7572 6365 733a 0a20 2074 7a6b 743a  sources:.  tzkt:
+000000b0: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
+000000c0: 2e74 7a6b 740a 2020 2020 7572 6c3a 2024  .tzkt.    url: $
+000000d0: 7b54 5a4b 545f 5552 4c3a 2d68 7474 7073  {TZKT_URL:-https
+000000e0: 3a2f 2f61 7069 2e74 7a6b 742e 696f 7d0a  ://api.tzkt.io}.
+000000f0: 0a69 6e64 6578 6573 3a0a 2020 7265 6769  .indexes:.  regi
+00000100: 7374 7279 5f64 616f 3a0a 2020 2020 6b69  stry_dao:.    ki
+00000110: 6e64 3a20 7465 7a6f 732e 747a 6b74 2e6f  nd: tezos.tzkt.o
+00000120: 7065 7261 7469 6f6e 730a 2020 2020 6461  perations.    da
+00000130: 7461 736f 7572 6365 3a20 747a 6b74 0a20  tasource: tzkt. 
+00000140: 2020 2074 7970 6573 3a0a 2020 2020 2020     types:.      
+00000150: 2d20 7472 616e 7361 6374 696f 6e0a 2020  - transaction.  
+00000160: 2020 2020 2d20 6f72 6967 696e 6174 696f      - originatio
+00000170: 6e0a 2020 2020 6861 6e64 6c65 7273 3a0a  n.    handlers:.
+00000180: 2020 2020 2020 2d20 6361 6c6c 6261 636b        - callback
+00000190: 3a20 6f6e 5f6f 7269 6769 6e61 7469 6f6e  : on_origination
+000001a0: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
+000001b0: 3a0a 2020 2020 2020 2020 2020 2d20 7479  :.          - ty
+000001c0: 7065 3a20 6f72 6967 696e 6174 696f 6e0a  pe: origination.
+000001d0: 2020 2020 2020 2020 2020 2020 6f72 6967              orig
+000001e0: 696e 6174 6564 5f63 6f6e 7472 6163 743a  inated_contract:
+000001f0: 2072 6567 6973 7472 790a 2020 2020 2020   registry.      
+00000200: 2d20 6361 6c6c 6261 636b 3a20 6f6e 5f70  - callback: on_p
+00000210: 726f 706f 7365 0a20 2020 2020 2020 2070  ropose.        p
+00000220: 6174 7465 726e 3a0a 2020 2020 2020 2020  attern:.        
+00000230: 2020 2d20 7479 7065 3a20 7472 616e 7361    - type: transa
+00000240: 6374 696f 6e0a 2020 2020 2020 2020 2020  ction.          
+00000250: 2020 6465 7374 696e 6174 696f 6e3a 2072    destination: r
+00000260: 6567 6973 7472 790a 2020 2020 2020 2020  egistry.        
+00000270: 2020 2020 656e 7472 7970 6f69 6e74 3a20      entrypoint: 
+00000280: 7072 6f70 6f73 65                        propose
```

### Comparing `dipdup-7.0.0rc1/tests/configs/demo_dex.yml` & `dipdup-7.0.0rc2/tests/configs/demo_dex.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,317 +1,314 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
-00000020: 6465 780a 0a64 6174 6162 6173 653a 0a20  dex..database:. 
-00000030: 206b 696e 643a 2073 716c 6974 650a 2020   kind: sqlite.  
-00000040: 7061 7468 3a20 6462 2e73 716c 6974 6533  path: db.sqlite3
-00000050: 0a0a 636f 6e74 7261 6374 733a 0a20 206b  ..contracts:.  k
-00000060: 7573 645f 6465 785f 6d61 696e 6e65 743a  usd_dex_mainnet:
-00000070: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
-00000080: 0a20 2020 2061 6464 7265 7373 3a20 4b54  .    address: KT
-00000090: 314b 3445 7754 7062 7659 4e39 6167 4a64  1K4EwTpbvYN9agJd
-000000a0: 6a70 794a 6d34 5a5a 6468 7055 4e4b 4233  jpyJm4ZZdhpUNKB3
-000000b0: 4636 0a20 2020 2074 7970 656e 616d 653a  F6.    typename:
-000000c0: 2071 7569 7075 5f66 6131 320a 2020 6b75   quipu_fa12.  ku
-000000d0: 7364 5f74 6f6b 656e 5f6d 6169 6e6e 6574  sd_token_mainnet
-000000e0: 3a0a 2020 2020 6b69 6e64 3a20 7465 7a6f  :.    kind: tezo
-000000f0: 730a 2020 2020 6164 6472 6573 733a 204b  s.    address: K
-00000100: 5431 4b39 6743 5267 614c 5246 4b54 4572  T1K9gCRgaLRFKTEr
-00000110: 5974 3177 5678 4133 4672 6239 466a 6173  Yt1wVxA3Frb9Fjas
-00000120: 6a54 560a 2020 2020 7479 7065 6e61 6d65  jTV.    typename
-00000130: 3a20 6661 3132 5f74 6f6b 656e 0a20 2068  : fa12_token.  h
-00000140: 6461 6f5f 6465 785f 6d61 696e 6e65 743a  dao_dex_mainnet:
-00000150: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
-00000160: 0a20 2020 2061 6464 7265 7373 3a20 4b54  .    address: KT
-00000170: 3151 784c 7175 6b79 666f 6850 5635 6b50  1QxLqukyfohPV5kP
-00000180: 6b77 3937 5273 3663 7731 4444 4476 5967  kw97Rs6cw1DDDvYg
-00000190: 6242 0a20 2020 2074 7970 656e 616d 653a  bB.    typename:
-000001a0: 2071 7569 7075 5f66 6132 0a20 2068 6461   quipu_fa2.  hda
-000001b0: 6f5f 746f 6b65 6e5f 6d61 696e 6e65 743a  o_token_mainnet:
-000001c0: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
-000001d0: 0a20 2020 2061 6464 7265 7373 3a20 4b54  .    address: KT
-000001e0: 3141 4641 326d 774e 554d 4e64 3453 7375  1AFA2mwNUMNd4Ssu
-000001f0: 6a45 3159 5970 3239 7664 3842 5a65 6a79  jE1YYp29vd8BZejy
-00000200: 4b57 0a20 2020 2074 7970 656e 616d 653a  KW.    typename:
-00000210: 2066 6132 5f74 6f6b 656e 0a0a 6461 7461   fa2_token..data
-00000220: 736f 7572 6365 733a 0a20 2074 7a6b 745f  sources:.  tzkt_
-00000230: 6d61 696e 6e65 743a 0a20 2020 206b 696e  mainnet:.    kin
-00000240: 643a 2074 657a 6f73 2e74 7a6b 740a 2020  d: tezos.tzkt.  
-00000250: 2020 7572 6c3a 2068 7474 7073 3a2f 2f61    url: https://a
-00000260: 7069 2e74 7a6b 742e 696f 0a20 2020 2068  pi.tzkt.io.    h
-00000270: 7474 703a 0a20 2020 2020 2072 6570 6c61  ttp:.      repla
-00000280: 795f 7061 7468 3a20 247b 4449 5044 5550  y_path: ${DIPDUP
-00000290: 5f52 4550 4c41 595f 5041 5448 3a2d 7d0a  _REPLAY_PATH:-}.
-000002a0: 0a74 656d 706c 6174 6573 3a0a 2020 7175  .templates:.  qu
-000002b0: 6970 7573 7761 705f 6661 3132 3a0a 2020  ipuswap_fa12:.  
-000002c0: 2020 6b69 6e64 3a20 7465 7a6f 732e 747a    kind: tezos.tz
-000002d0: 6b74 2e6f 7065 7261 7469 6f6e 730a 2020  kt.operations.  
-000002e0: 2020 6461 7461 736f 7572 6365 3a20 747a    datasource: tz
-000002f0: 6b74 5f6d 6169 6e6e 6574 0a20 2020 2063  kt_mainnet.    c
-00000300: 6f6e 7472 6163 7473 3a0a 2020 2020 2020  ontracts:.      
-00000310: 2d20 3c64 6578 5f63 6f6e 7472 6163 743e  - <dex_contract>
-00000320: 0a20 2020 2074 7970 6573 3a0a 2020 2020  .    types:.    
-00000330: 2020 2d20 7472 616e 7361 6374 696f 6e0a    - transaction.
-00000340: 2020 2020 2020 2d20 6f72 6967 696e 6174        - originat
-00000350: 696f 6e0a 2020 2020 6861 6e64 6c65 7273  ion.    handlers
-00000360: 3a0a 2020 2020 2020 2d20 6361 6c6c 6261  :.      - callba
-00000370: 636b 3a20 6f6e 5f66 6131 325f 6f72 6967  ck: on_fa12_orig
-00000380: 696e 6174 696f 6e0a 2020 2020 2020 2020  ination.        
-00000390: 7061 7474 6572 6e3a 0a20 2020 2020 2020  pattern:.       
-000003a0: 2020 202d 2074 7970 653a 206f 7269 6769     - type: origi
-000003b0: 6e61 7469 6f6e 0a20 2020 2020 2020 2020  nation.         
-000003c0: 2020 206f 7269 6769 6e61 7465 645f 636f     originated_co
-000003d0: 6e74 7261 6374 3a20 3c64 6578 5f63 6f6e  ntract: <dex_con
-000003e0: 7472 6163 743e 0a20 2020 2020 202d 2063  tract>.      - c
-000003f0: 616c 6c62 6163 6b3a 206f 6e5f 6661 3132  allback: on_fa12
-00000400: 5f74 6f6b 656e 5f74 6f5f 7465 7a0a 2020  _token_to_tez.  
-00000410: 2020 2020 2020 7061 7474 6572 6e3a 0a20        pattern:. 
-00000420: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
-00000430: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
-00000440: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
-00000450: 7469 6f6e 3a20 3c64 6578 5f63 6f6e 7472  tion: <dex_contr
-00000460: 6163 743e 0a20 2020 2020 2020 2020 2020  act>.           
-00000470: 2065 6e74 7279 706f 696e 743a 2074 6f6b   entrypoint: tok
-00000480: 656e 546f 5465 7a50 6179 6d65 6e74 0a20  enToTezPayment. 
-00000490: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
-000004a0: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
-000004b0: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
-000004c0: 7469 6f6e 3a20 3c74 6f6b 656e 5f63 6f6e  tion: <token_con
-000004d0: 7472 6163 743e 0a20 2020 2020 2020 2020  tract>.         
-000004e0: 2020 2065 6e74 7279 706f 696e 743a 2074     entrypoint: t
-000004f0: 7261 6e73 6665 720a 2020 2020 2020 2020  ransfer.        
-00000500: 2020 2d20 7479 7065 3a20 7472 616e 7361    - type: transa
-00000510: 6374 696f 6e0a 2020 2020 2020 2020 2020  ction.          
-00000520: 2020 736f 7572 6365 3a20 3c64 6578 5f63    source: <dex_c
-00000530: 6f6e 7472 6163 743e 0a20 2020 2020 202d  ontract>.      -
-00000540: 2063 616c 6c62 6163 6b3a 206f 6e5f 6661   callback: on_fa
-00000550: 3132 5f74 657a 5f74 6f5f 746f 6b65 6e0a  12_tez_to_token.
-00000560: 2020 2020 2020 2020 7061 7474 6572 6e3a          pattern:
-00000570: 0a20 2020 2020 2020 2020 202d 2074 7970  .          - typ
-00000580: 653a 2074 7261 6e73 6163 7469 6f6e 0a20  e: transaction. 
-00000590: 2020 2020 2020 2020 2020 2064 6573 7469             desti
-000005a0: 6e61 7469 6f6e 3a20 3c64 6578 5f63 6f6e  nation: <dex_con
-000005b0: 7472 6163 743e 0a20 2020 2020 2020 2020  tract>.         
-000005c0: 2020 2065 6e74 7279 706f 696e 743a 2074     entrypoint: t
-000005d0: 657a 546f 546f 6b65 6e50 6179 6d65 6e74  ezToTokenPayment
-000005e0: 0a20 2020 2020 2020 2020 202d 2074 7970  .          - typ
-000005f0: 653a 2074 7261 6e73 6163 7469 6f6e 0a20  e: transaction. 
-00000600: 2020 2020 2020 2020 2020 2064 6573 7469             desti
-00000610: 6e61 7469 6f6e 3a20 3c74 6f6b 656e 5f63  nation: <token_c
-00000620: 6f6e 7472 6163 743e 0a20 2020 2020 2020  ontract>.       
-00000630: 2020 2020 2065 6e74 7279 706f 696e 743a       entrypoint:
-00000640: 2074 7261 6e73 6665 720a 2020 2020 2020   transfer.      
-00000650: 2d20 6361 6c6c 6261 636b 3a20 6f6e 5f66  - callback: on_f
-00000660: 6131 325f 696e 7665 7374 5f6c 6971 7569  a12_invest_liqui
-00000670: 6469 7479 0a20 2020 2020 2020 2070 6174  dity.        pat
-00000680: 7465 726e 3a0a 2020 2020 2020 2020 2020  tern:.          
-00000690: 2d20 7479 7065 3a20 7472 616e 7361 6374  - type: transact
-000006a0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-000006b0: 6465 7374 696e 6174 696f 6e3a 203c 6465  destination: <de
-000006c0: 785f 636f 6e74 7261 6374 3e0a 2020 2020  x_contract>.    
-000006d0: 2020 2020 2020 2020 656e 7472 7970 6f69          entrypoi
-000006e0: 6e74 3a20 696e 7665 7374 4c69 7175 6964  nt: investLiquid
-000006f0: 6974 790a 2020 2020 2020 2020 2020 2d20  ity.          - 
-00000700: 7479 7065 3a20 7472 616e 7361 6374 696f  type: transactio
-00000710: 6e0a 2020 2020 2020 2020 2020 2020 6465  n.            de
-00000720: 7374 696e 6174 696f 6e3a 203c 746f 6b65  stination: <toke
-00000730: 6e5f 636f 6e74 7261 6374 3e0a 2020 2020  n_contract>.    
-00000740: 2020 2020 2020 2020 656e 7472 7970 6f69          entrypoi
-00000750: 6e74 3a20 7472 616e 7366 6572 0a20 2020  nt: transfer.   
-00000760: 2020 202d 2063 616c 6c62 6163 6b3a 206f     - callback: o
-00000770: 6e5f 6661 3132 5f74 7261 6e73 6665 720a  n_fa12_transfer.
-00000780: 2020 2020 2020 2020 7061 7474 6572 6e3a          pattern:
-00000790: 0a20 2020 2020 2020 2020 202d 2074 7970  .          - typ
-000007a0: 653a 2074 7261 6e73 6163 7469 6f6e 0a20  e: transaction. 
-000007b0: 2020 2020 2020 2020 2020 2064 6573 7469             desti
-000007c0: 6e61 7469 6f6e 3a20 3c64 6578 5f63 6f6e  nation: <dex_con
-000007d0: 7472 6163 743e 0a20 2020 2020 2020 2020  tract>.         
-000007e0: 2020 2065 6e74 7279 706f 696e 743a 2074     entrypoint: t
-000007f0: 7261 6e73 6665 720a 2020 2020 2020 2d20  ransfer.      - 
-00000800: 6361 6c6c 6261 636b 3a20 6f6e 5f66 6131  callback: on_fa1
-00000810: 325f 6469 7665 7374 5f6c 6971 7569 6469  2_divest_liquidi
-00000820: 7479 0a20 2020 2020 2020 2070 6174 7465  ty.        patte
-00000830: 726e 3a0a 2020 2020 2020 2020 2020 2d20  rn:.          - 
-00000840: 7479 7065 3a20 7472 616e 7361 6374 696f  type: transactio
-00000850: 6e0a 2020 2020 2020 2020 2020 2020 6465  n.            de
-00000860: 7374 696e 6174 696f 6e3a 203c 6465 785f  stination: <dex_
-00000870: 636f 6e74 7261 6374 3e0a 2020 2020 2020  contract>.      
-00000880: 2020 2020 2020 656e 7472 7970 6f69 6e74        entrypoint
-00000890: 3a20 6469 7665 7374 4c69 7175 6964 6974  : divestLiquidit
-000008a0: 790a 2020 2020 2020 2020 2020 2d20 7479  y.          - ty
-000008b0: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
-000008c0: 2020 2020 2020 2020 2020 2020 6465 7374              dest
-000008d0: 696e 6174 696f 6e3a 203c 746f 6b65 6e5f  ination: <token_
-000008e0: 636f 6e74 7261 6374 3e0a 2020 2020 2020  contract>.      
-000008f0: 2020 2020 2020 656e 7472 7970 6f69 6e74        entrypoint
-00000900: 3a20 7472 616e 7366 6572 0a20 2020 2020  : transfer.     
-00000910: 2020 2020 202d 2074 7970 653a 2074 7261       - type: tra
-00000920: 6e73 6163 7469 6f6e 0a20 2020 2020 2020  nsaction.       
-00000930: 2020 2020 2073 6f75 7263 653a 203c 6465       source: <de
-00000940: 785f 636f 6e74 7261 6374 3e0a 2020 2020  x_contract>.    
-00000950: 2020 2d20 6361 6c6c 6261 636b 3a20 6f6e    - callback: on
-00000960: 5f66 6131 325f 7769 7468 6472 6177 5f70  _fa12_withdraw_p
-00000970: 726f 6669 740a 2020 2020 2020 2020 7061  rofit.        pa
-00000980: 7474 6572 6e3a 0a20 2020 2020 2020 2020  ttern:.         
-00000990: 202d 2074 7970 653a 2074 7261 6e73 6163   - type: transac
-000009a0: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-000009b0: 2064 6573 7469 6e61 7469 6f6e 3a20 3c64   destination: <d
-000009c0: 6578 5f63 6f6e 7472 6163 743e 0a20 2020  ex_contract>.   
-000009d0: 2020 2020 2020 2020 2065 6e74 7279 706f           entrypo
-000009e0: 696e 743a 2077 6974 6864 7261 7750 726f  int: withdrawPro
-000009f0: 6669 740a 2020 2020 2020 2020 2020 2d20  fit.          - 
-00000a00: 7479 7065 3a20 7472 616e 7361 6374 696f  type: transactio
-00000a10: 6e0a 2020 2020 2020 2020 2020 2020 736f  n.            so
-00000a20: 7572 6365 3a20 3c64 6578 5f63 6f6e 7472  urce: <dex_contr
-00000a30: 6163 743e 0a20 2020 2020 2020 2020 2020  act>.           
-00000a40: 206f 7074 696f 6e61 6c3a 2054 7275 650a   optional: True.
-00000a50: 2020 2020 6669 7273 745f 6c65 7665 6c3a      first_level:
-00000a60: 2031 3430 3735 3238 0a20 2020 206c 6173   1407528.    las
-00000a70: 745f 6c65 7665 6c3a 2031 3433 3736 3130  t_level: 1437610
-00000a80: 0a0a 2020 7175 6970 7573 7761 705f 6661  ..  quipuswap_fa
-00000a90: 323a 0a20 2020 206b 696e 643a 2074 657a  2:.    kind: tez
-00000aa0: 6f73 2e74 7a6b 742e 6f70 6572 6174 696f  os.tzkt.operatio
-00000ab0: 6e73 0a20 2020 2064 6174 6173 6f75 7263  ns.    datasourc
-00000ac0: 653a 2074 7a6b 745f 6d61 696e 6e65 740a  e: tzkt_mainnet.
-00000ad0: 2020 2020 636f 6e74 7261 6374 733a 0a20      contracts:. 
-00000ae0: 2020 2020 202d 203c 6465 785f 636f 6e74       - <dex_cont
-00000af0: 7261 6374 3e0a 2020 2020 7479 7065 733a  ract>.    types:
-00000b00: 0a20 2020 2020 202d 2074 7261 6e73 6163  .      - transac
-00000b10: 7469 6f6e 0a20 2020 2020 202d 206f 7269  tion.      - ori
-00000b20: 6769 6e61 7469 6f6e 0a20 2020 2068 616e  gination.    han
-00000b30: 646c 6572 733a 0a20 2020 2020 202d 2063  dlers:.      - c
-00000b40: 616c 6c62 6163 6b3a 206f 6e5f 6661 325f  allback: on_fa2_
-00000b50: 6f72 6967 696e 6174 696f 6e0a 2020 2020  origination.    
-00000b60: 2020 2020 7061 7474 6572 6e3a 0a20 2020      pattern:.   
-00000b70: 2020 2020 2020 202d 2074 7970 653a 206f         - type: o
-00000b80: 7269 6769 6e61 7469 6f6e 0a20 2020 2020  rigination.     
-00000b90: 2020 2020 2020 206f 7269 6769 6e61 7465         originate
-00000ba0: 645f 636f 6e74 7261 6374 3a20 3c64 6578  d_contract: <dex
-00000bb0: 5f63 6f6e 7472 6163 743e 0a20 2020 2020  _contract>.     
-00000bc0: 202d 2063 616c 6c62 6163 6b3a 206f 6e5f   - callback: on_
-00000bd0: 6661 325f 746f 6b65 6e5f 746f 5f74 657a  fa2_token_to_tez
-00000be0: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
-00000bf0: 3a0a 2020 2020 2020 2020 2020 2d20 7479  :.          - ty
-00000c00: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
-00000c10: 2020 2020 2020 2020 2020 2020 6465 7374              dest
-00000c20: 696e 6174 696f 6e3a 203c 6465 785f 636f  ination: <dex_co
-00000c30: 6e74 7261 6374 3e0a 2020 2020 2020 2020  ntract>.        
-00000c40: 2020 2020 656e 7472 7970 6f69 6e74 3a20      entrypoint: 
-00000c50: 746f 6b65 6e54 6f54 657a 5061 796d 656e  tokenToTezPaymen
-00000c60: 740a 2020 2020 2020 2020 2020 2d20 7479  t.          - ty
-00000c70: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
-00000c80: 2020 2020 2020 2020 2020 2020 6465 7374              dest
-00000c90: 696e 6174 696f 6e3a 203c 746f 6b65 6e5f  ination: <token_
-00000ca0: 636f 6e74 7261 6374 3e0a 2020 2020 2020  contract>.      
-00000cb0: 2020 2020 2020 656e 7472 7970 6f69 6e74        entrypoint
-00000cc0: 3a20 7472 616e 7366 6572 0a20 2020 2020  : transfer.     
-00000cd0: 2020 2020 202d 2074 7970 653a 2074 7261       - type: tra
-00000ce0: 6e73 6163 7469 6f6e 0a20 2020 2020 2020  nsaction.       
-00000cf0: 2020 2020 2073 6f75 7263 653a 203c 6465       source: <de
-00000d00: 785f 636f 6e74 7261 6374 3e0a 2020 2020  x_contract>.    
-00000d10: 2020 2d20 6361 6c6c 6261 636b 3a20 6f6e    - callback: on
-00000d20: 5f66 6132 5f74 657a 5f74 6f5f 746f 6b65  _fa2_tez_to_toke
-00000d30: 6e0a 2020 2020 2020 2020 7061 7474 6572  n.        patter
-00000d40: 6e3a 0a20 2020 2020 2020 2020 202d 2074  n:.          - t
-00000d50: 7970 653a 2074 7261 6e73 6163 7469 6f6e  ype: transaction
-00000d60: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-00000d70: 7469 6e61 7469 6f6e 3a20 3c64 6578 5f63  tination: <dex_c
-00000d80: 6f6e 7472 6163 743e 0a20 2020 2020 2020  ontract>.       
-00000d90: 2020 2020 2065 6e74 7279 706f 696e 743a       entrypoint:
-00000da0: 2074 657a 546f 546f 6b65 6e50 6179 6d65   tezToTokenPayme
-00000db0: 6e74 0a20 2020 2020 2020 2020 202d 2074  nt.          - t
-00000dc0: 7970 653a 2074 7261 6e73 6163 7469 6f6e  ype: transaction
-00000dd0: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-00000de0: 7469 6e61 7469 6f6e 3a20 3c74 6f6b 656e  tination: <token
-00000df0: 5f63 6f6e 7472 6163 743e 0a20 2020 2020  _contract>.     
-00000e00: 2020 2020 2020 2065 6e74 7279 706f 696e         entrypoin
-00000e10: 743a 2074 7261 6e73 6665 720a 2020 2020  t: transfer.    
-00000e20: 2020 2d20 6361 6c6c 6261 636b 3a20 6f6e    - callback: on
-00000e30: 5f66 6132 5f69 6e76 6573 745f 6c69 7175  _fa2_invest_liqu
-00000e40: 6964 6974 790a 2020 2020 2020 2020 7061  idity.        pa
-00000e50: 7474 6572 6e3a 0a20 2020 2020 2020 2020  ttern:.         
-00000e60: 202d 2074 7970 653a 2074 7261 6e73 6163   - type: transac
-00000e70: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-00000e80: 2064 6573 7469 6e61 7469 6f6e 3a20 3c64   destination: <d
-00000e90: 6578 5f63 6f6e 7472 6163 743e 0a20 2020  ex_contract>.   
-00000ea0: 2020 2020 2020 2020 2065 6e74 7279 706f           entrypo
-00000eb0: 696e 743a 2069 6e76 6573 744c 6971 7569  int: investLiqui
-00000ec0: 6469 7479 0a20 2020 2020 2020 2020 202d  dity.          -
-00000ed0: 2074 7970 653a 2074 7261 6e73 6163 7469   type: transacti
-00000ee0: 6f6e 0a20 2020 2020 2020 2020 2020 2064  on.            d
-00000ef0: 6573 7469 6e61 7469 6f6e 3a20 3c74 6f6b  estination: <tok
-00000f00: 656e 5f63 6f6e 7472 6163 743e 0a20 2020  en_contract>.   
-00000f10: 2020 2020 2020 2020 2065 6e74 7279 706f           entrypo
-00000f20: 696e 743a 2074 7261 6e73 6665 720a 2020  int: transfer.  
-00000f30: 2020 2020 2d20 6361 6c6c 6261 636b 3a20      - callback: 
-00000f40: 6f6e 5f66 6132 5f74 7261 6e73 6665 720a  on_fa2_transfer.
-00000f50: 2020 2020 2020 2020 7061 7474 6572 6e3a          pattern:
-00000f60: 0a20 2020 2020 2020 2020 202d 2074 7970  .          - typ
-00000f70: 653a 2074 7261 6e73 6163 7469 6f6e 0a20  e: transaction. 
-00000f80: 2020 2020 2020 2020 2020 2064 6573 7469             desti
-00000f90: 6e61 7469 6f6e 3a20 3c64 6578 5f63 6f6e  nation: <dex_con
-00000fa0: 7472 6163 743e 0a20 2020 2020 2020 2020  tract>.         
-00000fb0: 2020 2065 6e74 7279 706f 696e 743a 2074     entrypoint: t
-00000fc0: 7261 6e73 6665 720a 2020 2020 2020 2d20  ransfer.      - 
-00000fd0: 6361 6c6c 6261 636b 3a20 6f6e 5f66 6132  callback: on_fa2
-00000fe0: 5f64 6976 6573 745f 6c69 7175 6964 6974  _divest_liquidit
-00000ff0: 790a 2020 2020 2020 2020 7061 7474 6572  y.        patter
-00001000: 6e3a 0a20 2020 2020 2020 2020 202d 2074  n:.          - t
-00001010: 7970 653a 2074 7261 6e73 6163 7469 6f6e  ype: transaction
-00001020: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-00001030: 7469 6e61 7469 6f6e 3a20 3c64 6578 5f63  tination: <dex_c
-00001040: 6f6e 7472 6163 743e 0a20 2020 2020 2020  ontract>.       
-00001050: 2020 2020 2065 6e74 7279 706f 696e 743a       entrypoint:
-00001060: 2064 6976 6573 744c 6971 7569 6469 7479   divestLiquidity
-00001070: 0a20 2020 2020 2020 2020 202d 2074 7970  .          - typ
-00001080: 653a 2074 7261 6e73 6163 7469 6f6e 0a20  e: transaction. 
-00001090: 2020 2020 2020 2020 2020 2064 6573 7469             desti
-000010a0: 6e61 7469 6f6e 3a20 3c74 6f6b 656e 5f63  nation: <token_c
-000010b0: 6f6e 7472 6163 743e 0a20 2020 2020 2020  ontract>.       
-000010c0: 2020 2020 2065 6e74 7279 706f 696e 743a       entrypoint:
-000010d0: 2074 7261 6e73 6665 720a 2020 2020 2020   transfer.      
-000010e0: 2020 2020 2d20 7479 7065 3a20 7472 616e      - type: tran
-000010f0: 7361 6374 696f 6e0a 2020 2020 2020 2020  saction.        
-00001100: 2020 2020 736f 7572 6365 3a20 3c64 6578      source: <dex
-00001110: 5f63 6f6e 7472 6163 743e 0a20 2020 2020  _contract>.     
-00001120: 202d 2063 616c 6c62 6163 6b3a 206f 6e5f   - callback: on_
-00001130: 6661 325f 7769 7468 6472 6177 5f70 726f  fa2_withdraw_pro
-00001140: 6669 740a 2020 2020 2020 2020 7061 7474  fit.        patt
-00001150: 6572 6e3a 0a20 2020 2020 2020 2020 202d  ern:.          -
-00001160: 2074 7970 653a 2074 7261 6e73 6163 7469   type: transacti
-00001170: 6f6e 0a20 2020 2020 2020 2020 2020 2064  on.            d
-00001180: 6573 7469 6e61 7469 6f6e 3a20 3c64 6578  estination: <dex
-00001190: 5f63 6f6e 7472 6163 743e 0a20 2020 2020  _contract>.     
-000011a0: 2020 2020 2020 2065 6e74 7279 706f 696e         entrypoin
-000011b0: 743a 2077 6974 6864 7261 7750 726f 6669  t: withdrawProfi
-000011c0: 740a 2020 2020 2020 2020 2020 2d20 7479  t.          - ty
-000011d0: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
-000011e0: 2020 2020 2020 2020 2020 2020 736f 7572              sour
-000011f0: 6365 3a20 3c64 6578 5f63 6f6e 7472 6163  ce: <dex_contrac
-00001200: 743e 0a20 2020 2020 2020 2020 2020 206f  t>.            o
-00001210: 7074 696f 6e61 6c3a 2054 7275 650a 2020  ptional: True.  
-00001220: 2020 6669 7273 745f 6c65 7665 6c3a 2031    first_level: 1
-00001230: 3430 3735 3238 0a20 2020 206c 6173 745f  407528.    last_
-00001240: 6c65 7665 6c3a 2031 3434 3431 3333 0a0a  level: 1444133..
-00001250: 696e 6465 7865 733a 0a20 206b 7573 645f  indexes:.  kusd_
-00001260: 6d61 696e 6e65 743a 0a20 2020 2074 656d  mainnet:.    tem
-00001270: 706c 6174 653a 2071 7569 7075 7377 6170  plate: quipuswap
-00001280: 5f66 6131 320a 2020 2020 7661 6c75 6573  _fa12.    values
-00001290: 3a0a 2020 2020 2020 6465 785f 636f 6e74  :.      dex_cont
-000012a0: 7261 6374 3a20 6b75 7364 5f64 6578 5f6d  ract: kusd_dex_m
-000012b0: 6169 6e6e 6574 0a20 2020 2020 2074 6f6b  ainnet.      tok
-000012c0: 656e 5f63 6f6e 7472 6163 743a 206b 7573  en_contract: kus
-000012d0: 645f 746f 6b65 6e5f 6d61 696e 6e65 740a  d_token_mainnet.
-000012e0: 2020 2020 2020 7379 6d62 6f6c 3a20 6b55        symbol: kU
-000012f0: 5344 0a20 2020 2020 2064 6563 696d 616c  SD.      decimal
-00001300: 733a 2031 380a 0a20 2068 6461 6f5f 6d61  s: 18..  hdao_ma
-00001310: 696e 6e65 743a 0a20 2020 2074 656d 706c  innet:.    templ
-00001320: 6174 653a 2071 7569 7075 7377 6170 5f66  ate: quipuswap_f
-00001330: 6132 0a20 2020 2076 616c 7565 733a 0a20  a2.    values:. 
-00001340: 2020 2020 2064 6578 5f63 6f6e 7472 6163       dex_contrac
-00001350: 743a 2068 6461 6f5f 6465 785f 6d61 696e  t: hdao_dex_main
-00001360: 6e65 740a 2020 2020 2020 746f 6b65 6e5f  net.      token_
-00001370: 636f 6e74 7261 6374 3a20 6864 616f 5f74  contract: hdao_t
-00001380: 6f6b 656e 5f6d 6169 6e6e 6574 0a20 2020  oken_mainnet.   
-00001390: 2020 2073 796d 626f 6c3a 2068 4441 4f0a     symbol: hDAO.
-000013a0: 2020 2020 2020 6465 6369 6d61 6c73 3a20        decimals: 
-000013b0: 360a 0a6c 6f67 6769 6e67 3a20 5741 524e  6..logging: WARN
-000013c0: 0a                                       .
+00000020: 6465 780a 0a63 6f6e 7472 6163 7473 3a0a  dex..contracts:.
+00000030: 2020 6b75 7364 5f64 6578 5f6d 6169 6e6e    kusd_dex_mainn
+00000040: 6574 3a0a 2020 2020 6b69 6e64 3a20 7465  et:.    kind: te
+00000050: 7a6f 730a 2020 2020 6164 6472 6573 733a  zos.    address:
+00000060: 204b 5431 4b34 4577 5470 6276 594e 3961   KT1K4EwTpbvYN9a
+00000070: 674a 646a 7079 4a6d 345a 5a64 6870 554e  gJdjpyJm4ZZdhpUN
+00000080: 4b42 3346 360a 2020 2020 7479 7065 6e61  KB3F6.    typena
+00000090: 6d65 3a20 7175 6970 755f 6661 3132 0a20  me: quipu_fa12. 
+000000a0: 206b 7573 645f 746f 6b65 6e5f 6d61 696e   kusd_token_main
+000000b0: 6e65 743a 0a20 2020 206b 696e 643a 2074  net:.    kind: t
+000000c0: 657a 6f73 0a20 2020 2061 6464 7265 7373  ezos.    address
+000000d0: 3a20 4b54 314b 3967 4352 6761 4c52 464b  : KT1K9gCRgaLRFK
+000000e0: 5445 7259 7431 7756 7841 3346 7262 3946  TErYt1wVxA3Frb9F
+000000f0: 6a61 736a 5456 0a20 2020 2074 7970 656e  jasjTV.    typen
+00000100: 616d 653a 2066 6131 325f 746f 6b65 6e0a  ame: fa12_token.
+00000110: 2020 6864 616f 5f64 6578 5f6d 6169 6e6e    hdao_dex_mainn
+00000120: 6574 3a0a 2020 2020 6b69 6e64 3a20 7465  et:.    kind: te
+00000130: 7a6f 730a 2020 2020 6164 6472 6573 733a  zos.    address:
+00000140: 204b 5431 5178 4c71 756b 7966 6f68 5056   KT1QxLqukyfohPV
+00000150: 356b 506b 7739 3752 7336 6377 3144 4444  5kPkw97Rs6cw1DDD
+00000160: 7659 6762 420a 2020 2020 7479 7065 6e61  vYgbB.    typena
+00000170: 6d65 3a20 7175 6970 755f 6661 320a 2020  me: quipu_fa2.  
+00000180: 6864 616f 5f74 6f6b 656e 5f6d 6169 6e6e  hdao_token_mainn
+00000190: 6574 3a0a 2020 2020 6b69 6e64 3a20 7465  et:.    kind: te
+000001a0: 7a6f 730a 2020 2020 6164 6472 6573 733a  zos.    address:
+000001b0: 204b 5431 4146 4132 6d77 4e55 4d4e 6434   KT1AFA2mwNUMNd4
+000001c0: 5373 756a 4531 5959 7032 3976 6438 425a  SsujE1YYp29vd8BZ
+000001d0: 656a 794b 570a 2020 2020 7479 7065 6e61  ejyKW.    typena
+000001e0: 6d65 3a20 6661 325f 746f 6b65 6e0a 0a64  me: fa2_token..d
+000001f0: 6174 6173 6f75 7263 6573 3a0a 2020 747a  atasources:.  tz
+00000200: 6b74 5f6d 6169 6e6e 6574 3a0a 2020 2020  kt_mainnet:.    
+00000210: 6b69 6e64 3a20 7465 7a6f 732e 747a 6b74  kind: tezos.tzkt
+00000220: 0a20 2020 2075 726c 3a20 6874 7470 733a  .    url: https:
+00000230: 2f2f 6170 692e 747a 6b74 2e69 6f0a 2020  //api.tzkt.io.  
+00000240: 2020 6874 7470 3a0a 2020 2020 2020 7265    http:.      re
+00000250: 706c 6179 5f70 6174 683a 2024 7b44 4950  play_path: ${DIP
+00000260: 4455 505f 5245 504c 4159 5f50 4154 483a  DUP_REPLAY_PATH:
+00000270: 2d7d 0a0a 7465 6d70 6c61 7465 733a 0a20  -}..templates:. 
+00000280: 2071 7569 7075 7377 6170 5f66 6131 323a   quipuswap_fa12:
+00000290: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
+000002a0: 2e74 7a6b 742e 6f70 6572 6174 696f 6e73  .tzkt.operations
+000002b0: 0a20 2020 2064 6174 6173 6f75 7263 653a  .    datasource:
+000002c0: 2074 7a6b 745f 6d61 696e 6e65 740a 2020   tzkt_mainnet.  
+000002d0: 2020 636f 6e74 7261 6374 733a 0a20 2020    contracts:.   
+000002e0: 2020 202d 203c 6465 785f 636f 6e74 7261     - <dex_contra
+000002f0: 6374 3e0a 2020 2020 7479 7065 733a 0a20  ct>.    types:. 
+00000300: 2020 2020 202d 2074 7261 6e73 6163 7469       - transacti
+00000310: 6f6e 0a20 2020 2020 202d 206f 7269 6769  on.      - origi
+00000320: 6e61 7469 6f6e 0a20 2020 2068 616e 646c  nation.    handl
+00000330: 6572 733a 0a20 2020 2020 202d 2063 616c  ers:.      - cal
+00000340: 6c62 6163 6b3a 206f 6e5f 6661 3132 5f6f  lback: on_fa12_o
+00000350: 7269 6769 6e61 7469 6f6e 0a20 2020 2020  rigination.     
+00000360: 2020 2070 6174 7465 726e 3a0a 2020 2020     pattern:.    
+00000370: 2020 2020 2020 2d20 7479 7065 3a20 6f72        - type: or
+00000380: 6967 696e 6174 696f 6e0a 2020 2020 2020  igination.      
+00000390: 2020 2020 2020 6f72 6967 696e 6174 6564        originated
+000003a0: 5f63 6f6e 7472 6163 743a 203c 6465 785f  _contract: <dex_
+000003b0: 636f 6e74 7261 6374 3e0a 2020 2020 2020  contract>.      
+000003c0: 2d20 6361 6c6c 6261 636b 3a20 6f6e 5f66  - callback: on_f
+000003d0: 6131 325f 746f 6b65 6e5f 746f 5f74 657a  a12_token_to_tez
+000003e0: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
+000003f0: 3a0a 2020 2020 2020 2020 2020 2d20 7479  :.          - ty
+00000400: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
+00000410: 2020 2020 2020 2020 2020 2020 6465 7374              dest
+00000420: 696e 6174 696f 6e3a 203c 6465 785f 636f  ination: <dex_co
+00000430: 6e74 7261 6374 3e0a 2020 2020 2020 2020  ntract>.        
+00000440: 2020 2020 656e 7472 7970 6f69 6e74 3a20      entrypoint: 
+00000450: 746f 6b65 6e54 6f54 657a 5061 796d 656e  tokenToTezPaymen
+00000460: 740a 2020 2020 2020 2020 2020 2d20 7479  t.          - ty
+00000470: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
+00000480: 2020 2020 2020 2020 2020 2020 6465 7374              dest
+00000490: 696e 6174 696f 6e3a 203c 746f 6b65 6e5f  ination: <token_
+000004a0: 636f 6e74 7261 6374 3e0a 2020 2020 2020  contract>.      
+000004b0: 2020 2020 2020 656e 7472 7970 6f69 6e74        entrypoint
+000004c0: 3a20 7472 616e 7366 6572 0a20 2020 2020  : transfer.     
+000004d0: 2020 2020 202d 2074 7970 653a 2074 7261       - type: tra
+000004e0: 6e73 6163 7469 6f6e 0a20 2020 2020 2020  nsaction.       
+000004f0: 2020 2020 2073 6f75 7263 653a 203c 6465       source: <de
+00000500: 785f 636f 6e74 7261 6374 3e0a 2020 2020  x_contract>.    
+00000510: 2020 2d20 6361 6c6c 6261 636b 3a20 6f6e    - callback: on
+00000520: 5f66 6131 325f 7465 7a5f 746f 5f74 6f6b  _fa12_tez_to_tok
+00000530: 656e 0a20 2020 2020 2020 2070 6174 7465  en.        patte
+00000540: 726e 3a0a 2020 2020 2020 2020 2020 2d20  rn:.          - 
+00000550: 7479 7065 3a20 7472 616e 7361 6374 696f  type: transactio
+00000560: 6e0a 2020 2020 2020 2020 2020 2020 6465  n.            de
+00000570: 7374 696e 6174 696f 6e3a 203c 6465 785f  stination: <dex_
+00000580: 636f 6e74 7261 6374 3e0a 2020 2020 2020  contract>.      
+00000590: 2020 2020 2020 656e 7472 7970 6f69 6e74        entrypoint
+000005a0: 3a20 7465 7a54 6f54 6f6b 656e 5061 796d  : tezToTokenPaym
+000005b0: 656e 740a 2020 2020 2020 2020 2020 2d20  ent.          - 
+000005c0: 7479 7065 3a20 7472 616e 7361 6374 696f  type: transactio
+000005d0: 6e0a 2020 2020 2020 2020 2020 2020 6465  n.            de
+000005e0: 7374 696e 6174 696f 6e3a 203c 746f 6b65  stination: <toke
+000005f0: 6e5f 636f 6e74 7261 6374 3e0a 2020 2020  n_contract>.    
+00000600: 2020 2020 2020 2020 656e 7472 7970 6f69          entrypoi
+00000610: 6e74 3a20 7472 616e 7366 6572 0a20 2020  nt: transfer.   
+00000620: 2020 202d 2063 616c 6c62 6163 6b3a 206f     - callback: o
+00000630: 6e5f 6661 3132 5f69 6e76 6573 745f 6c69  n_fa12_invest_li
+00000640: 7175 6964 6974 790a 2020 2020 2020 2020  quidity.        
+00000650: 7061 7474 6572 6e3a 0a20 2020 2020 2020  pattern:.       
+00000660: 2020 202d 2074 7970 653a 2074 7261 6e73     - type: trans
+00000670: 6163 7469 6f6e 0a20 2020 2020 2020 2020  action.         
+00000680: 2020 2064 6573 7469 6e61 7469 6f6e 3a20     destination: 
+00000690: 3c64 6578 5f63 6f6e 7472 6163 743e 0a20  <dex_contract>. 
+000006a0: 2020 2020 2020 2020 2020 2065 6e74 7279             entry
+000006b0: 706f 696e 743a 2069 6e76 6573 744c 6971  point: investLiq
+000006c0: 7569 6469 7479 0a20 2020 2020 2020 2020  uidity.         
+000006d0: 202d 2074 7970 653a 2074 7261 6e73 6163   - type: transac
+000006e0: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+000006f0: 2064 6573 7469 6e61 7469 6f6e 3a20 3c74   destination: <t
+00000700: 6f6b 656e 5f63 6f6e 7472 6163 743e 0a20  oken_contract>. 
+00000710: 2020 2020 2020 2020 2020 2065 6e74 7279             entry
+00000720: 706f 696e 743a 2074 7261 6e73 6665 720a  point: transfer.
+00000730: 2020 2020 2020 2d20 6361 6c6c 6261 636b        - callback
+00000740: 3a20 6f6e 5f66 6131 325f 7472 616e 7366  : on_fa12_transf
+00000750: 6572 0a20 2020 2020 2020 2070 6174 7465  er.        patte
+00000760: 726e 3a0a 2020 2020 2020 2020 2020 2d20  rn:.          - 
+00000770: 7479 7065 3a20 7472 616e 7361 6374 696f  type: transactio
+00000780: 6e0a 2020 2020 2020 2020 2020 2020 6465  n.            de
+00000790: 7374 696e 6174 696f 6e3a 203c 6465 785f  stination: <dex_
+000007a0: 636f 6e74 7261 6374 3e0a 2020 2020 2020  contract>.      
+000007b0: 2020 2020 2020 656e 7472 7970 6f69 6e74        entrypoint
+000007c0: 3a20 7472 616e 7366 6572 0a20 2020 2020  : transfer.     
+000007d0: 202d 2063 616c 6c62 6163 6b3a 206f 6e5f   - callback: on_
+000007e0: 6661 3132 5f64 6976 6573 745f 6c69 7175  fa12_divest_liqu
+000007f0: 6964 6974 790a 2020 2020 2020 2020 7061  idity.        pa
+00000800: 7474 6572 6e3a 0a20 2020 2020 2020 2020  ttern:.         
+00000810: 202d 2074 7970 653a 2074 7261 6e73 6163   - type: transac
+00000820: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+00000830: 2064 6573 7469 6e61 7469 6f6e 3a20 3c64   destination: <d
+00000840: 6578 5f63 6f6e 7472 6163 743e 0a20 2020  ex_contract>.   
+00000850: 2020 2020 2020 2020 2065 6e74 7279 706f           entrypo
+00000860: 696e 743a 2064 6976 6573 744c 6971 7569  int: divestLiqui
+00000870: 6469 7479 0a20 2020 2020 2020 2020 202d  dity.          -
+00000880: 2074 7970 653a 2074 7261 6e73 6163 7469   type: transacti
+00000890: 6f6e 0a20 2020 2020 2020 2020 2020 2064  on.            d
+000008a0: 6573 7469 6e61 7469 6f6e 3a20 3c74 6f6b  estination: <tok
+000008b0: 656e 5f63 6f6e 7472 6163 743e 0a20 2020  en_contract>.   
+000008c0: 2020 2020 2020 2020 2065 6e74 7279 706f           entrypo
+000008d0: 696e 743a 2074 7261 6e73 6665 720a 2020  int: transfer.  
+000008e0: 2020 2020 2020 2020 2d20 7479 7065 3a20          - type: 
+000008f0: 7472 616e 7361 6374 696f 6e0a 2020 2020  transaction.    
+00000900: 2020 2020 2020 2020 736f 7572 6365 3a20          source: 
+00000910: 3c64 6578 5f63 6f6e 7472 6163 743e 0a20  <dex_contract>. 
+00000920: 2020 2020 202d 2063 616c 6c62 6163 6b3a       - callback:
+00000930: 206f 6e5f 6661 3132 5f77 6974 6864 7261   on_fa12_withdra
+00000940: 775f 7072 6f66 6974 0a20 2020 2020 2020  w_profit.       
+00000950: 2070 6174 7465 726e 3a0a 2020 2020 2020   pattern:.      
+00000960: 2020 2020 2d20 7479 7065 3a20 7472 616e      - type: tran
+00000970: 7361 6374 696f 6e0a 2020 2020 2020 2020  saction.        
+00000980: 2020 2020 6465 7374 696e 6174 696f 6e3a      destination:
+00000990: 203c 6465 785f 636f 6e74 7261 6374 3e0a   <dex_contract>.
+000009a0: 2020 2020 2020 2020 2020 2020 656e 7472              entr
+000009b0: 7970 6f69 6e74 3a20 7769 7468 6472 6177  ypoint: withdraw
+000009c0: 5072 6f66 6974 0a20 2020 2020 2020 2020  Profit.         
+000009d0: 202d 2074 7970 653a 2074 7261 6e73 6163   - type: transac
+000009e0: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+000009f0: 2073 6f75 7263 653a 203c 6465 785f 636f   source: <dex_co
+00000a00: 6e74 7261 6374 3e0a 2020 2020 2020 2020  ntract>.        
+00000a10: 2020 2020 6f70 7469 6f6e 616c 3a20 5472      optional: Tr
+00000a20: 7565 0a20 2020 2066 6972 7374 5f6c 6576  ue.    first_lev
+00000a30: 656c 3a20 3134 3037 3532 380a 2020 2020  el: 1407528.    
+00000a40: 6c61 7374 5f6c 6576 656c 3a20 3134 3337  last_level: 1437
+00000a50: 3631 300a 0a20 2071 7569 7075 7377 6170  610..  quipuswap
+00000a60: 5f66 6132 3a0a 2020 2020 6b69 6e64 3a20  _fa2:.    kind: 
+00000a70: 7465 7a6f 732e 747a 6b74 2e6f 7065 7261  tezos.tzkt.opera
+00000a80: 7469 6f6e 730a 2020 2020 6461 7461 736f  tions.    dataso
+00000a90: 7572 6365 3a20 747a 6b74 5f6d 6169 6e6e  urce: tzkt_mainn
+00000aa0: 6574 0a20 2020 2063 6f6e 7472 6163 7473  et.    contracts
+00000ab0: 3a0a 2020 2020 2020 2d20 3c64 6578 5f63  :.      - <dex_c
+00000ac0: 6f6e 7472 6163 743e 0a20 2020 2074 7970  ontract>.    typ
+00000ad0: 6573 3a0a 2020 2020 2020 2d20 7472 616e  es:.      - tran
+00000ae0: 7361 6374 696f 6e0a 2020 2020 2020 2d20  saction.      - 
+00000af0: 6f72 6967 696e 6174 696f 6e0a 2020 2020  origination.    
+00000b00: 6861 6e64 6c65 7273 3a0a 2020 2020 2020  handlers:.      
+00000b10: 2d20 6361 6c6c 6261 636b 3a20 6f6e 5f66  - callback: on_f
+00000b20: 6132 5f6f 7269 6769 6e61 7469 6f6e 0a20  a2_origination. 
+00000b30: 2020 2020 2020 2070 6174 7465 726e 3a0a         pattern:.
+00000b40: 2020 2020 2020 2020 2020 2d20 7479 7065            - type
+00000b50: 3a20 6f72 6967 696e 6174 696f 6e0a 2020  : origination.  
+00000b60: 2020 2020 2020 2020 2020 6f72 6967 696e            origin
+00000b70: 6174 6564 5f63 6f6e 7472 6163 743a 203c  ated_contract: <
+00000b80: 6465 785f 636f 6e74 7261 6374 3e0a 2020  dex_contract>.  
+00000b90: 2020 2020 2d20 6361 6c6c 6261 636b 3a20      - callback: 
+00000ba0: 6f6e 5f66 6132 5f74 6f6b 656e 5f74 6f5f  on_fa2_token_to_
+00000bb0: 7465 7a0a 2020 2020 2020 2020 7061 7474  tez.        patt
+00000bc0: 6572 6e3a 0a20 2020 2020 2020 2020 202d  ern:.          -
+00000bd0: 2074 7970 653a 2074 7261 6e73 6163 7469   type: transacti
+00000be0: 6f6e 0a20 2020 2020 2020 2020 2020 2064  on.            d
+00000bf0: 6573 7469 6e61 7469 6f6e 3a20 3c64 6578  estination: <dex
+00000c00: 5f63 6f6e 7472 6163 743e 0a20 2020 2020  _contract>.     
+00000c10: 2020 2020 2020 2065 6e74 7279 706f 696e         entrypoin
+00000c20: 743a 2074 6f6b 656e 546f 5465 7a50 6179  t: tokenToTezPay
+00000c30: 6d65 6e74 0a20 2020 2020 2020 2020 202d  ment.          -
+00000c40: 2074 7970 653a 2074 7261 6e73 6163 7469   type: transacti
+00000c50: 6f6e 0a20 2020 2020 2020 2020 2020 2064  on.            d
+00000c60: 6573 7469 6e61 7469 6f6e 3a20 3c74 6f6b  estination: <tok
+00000c70: 656e 5f63 6f6e 7472 6163 743e 0a20 2020  en_contract>.   
+00000c80: 2020 2020 2020 2020 2065 6e74 7279 706f           entrypo
+00000c90: 696e 743a 2074 7261 6e73 6665 720a 2020  int: transfer.  
+00000ca0: 2020 2020 2020 2020 2d20 7479 7065 3a20          - type: 
+00000cb0: 7472 616e 7361 6374 696f 6e0a 2020 2020  transaction.    
+00000cc0: 2020 2020 2020 2020 736f 7572 6365 3a20          source: 
+00000cd0: 3c64 6578 5f63 6f6e 7472 6163 743e 0a20  <dex_contract>. 
+00000ce0: 2020 2020 202d 2063 616c 6c62 6163 6b3a       - callback:
+00000cf0: 206f 6e5f 6661 325f 7465 7a5f 746f 5f74   on_fa2_tez_to_t
+00000d00: 6f6b 656e 0a20 2020 2020 2020 2070 6174  oken.        pat
+00000d10: 7465 726e 3a0a 2020 2020 2020 2020 2020  tern:.          
+00000d20: 2d20 7479 7065 3a20 7472 616e 7361 6374  - type: transact
+00000d30: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+00000d40: 6465 7374 696e 6174 696f 6e3a 203c 6465  destination: <de
+00000d50: 785f 636f 6e74 7261 6374 3e0a 2020 2020  x_contract>.    
+00000d60: 2020 2020 2020 2020 656e 7472 7970 6f69          entrypoi
+00000d70: 6e74 3a20 7465 7a54 6f54 6f6b 656e 5061  nt: tezToTokenPa
+00000d80: 796d 656e 740a 2020 2020 2020 2020 2020  yment.          
+00000d90: 2d20 7479 7065 3a20 7472 616e 7361 6374  - type: transact
+00000da0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+00000db0: 6465 7374 696e 6174 696f 6e3a 203c 746f  destination: <to
+00000dc0: 6b65 6e5f 636f 6e74 7261 6374 3e0a 2020  ken_contract>.  
+00000dd0: 2020 2020 2020 2020 2020 656e 7472 7970            entryp
+00000de0: 6f69 6e74 3a20 7472 616e 7366 6572 0a20  oint: transfer. 
+00000df0: 2020 2020 202d 2063 616c 6c62 6163 6b3a       - callback:
+00000e00: 206f 6e5f 6661 325f 696e 7665 7374 5f6c   on_fa2_invest_l
+00000e10: 6971 7569 6469 7479 0a20 2020 2020 2020  iquidity.       
+00000e20: 2070 6174 7465 726e 3a0a 2020 2020 2020   pattern:.      
+00000e30: 2020 2020 2d20 7479 7065 3a20 7472 616e      - type: tran
+00000e40: 7361 6374 696f 6e0a 2020 2020 2020 2020  saction.        
+00000e50: 2020 2020 6465 7374 696e 6174 696f 6e3a      destination:
+00000e60: 203c 6465 785f 636f 6e74 7261 6374 3e0a   <dex_contract>.
+00000e70: 2020 2020 2020 2020 2020 2020 656e 7472              entr
+00000e80: 7970 6f69 6e74 3a20 696e 7665 7374 4c69  ypoint: investLi
+00000e90: 7175 6964 6974 790a 2020 2020 2020 2020  quidity.        
+00000ea0: 2020 2d20 7479 7065 3a20 7472 616e 7361    - type: transa
+00000eb0: 6374 696f 6e0a 2020 2020 2020 2020 2020  ction.          
+00000ec0: 2020 6465 7374 696e 6174 696f 6e3a 203c    destination: <
+00000ed0: 746f 6b65 6e5f 636f 6e74 7261 6374 3e0a  token_contract>.
+00000ee0: 2020 2020 2020 2020 2020 2020 656e 7472              entr
+00000ef0: 7970 6f69 6e74 3a20 7472 616e 7366 6572  ypoint: transfer
+00000f00: 0a20 2020 2020 202d 2063 616c 6c62 6163  .      - callbac
+00000f10: 6b3a 206f 6e5f 6661 325f 7472 616e 7366  k: on_fa2_transf
+00000f20: 6572 0a20 2020 2020 2020 2070 6174 7465  er.        patte
+00000f30: 726e 3a0a 2020 2020 2020 2020 2020 2d20  rn:.          - 
+00000f40: 7479 7065 3a20 7472 616e 7361 6374 696f  type: transactio
+00000f50: 6e0a 2020 2020 2020 2020 2020 2020 6465  n.            de
+00000f60: 7374 696e 6174 696f 6e3a 203c 6465 785f  stination: <dex_
+00000f70: 636f 6e74 7261 6374 3e0a 2020 2020 2020  contract>.      
+00000f80: 2020 2020 2020 656e 7472 7970 6f69 6e74        entrypoint
+00000f90: 3a20 7472 616e 7366 6572 0a20 2020 2020  : transfer.     
+00000fa0: 202d 2063 616c 6c62 6163 6b3a 206f 6e5f   - callback: on_
+00000fb0: 6661 325f 6469 7665 7374 5f6c 6971 7569  fa2_divest_liqui
+00000fc0: 6469 7479 0a20 2020 2020 2020 2070 6174  dity.        pat
+00000fd0: 7465 726e 3a0a 2020 2020 2020 2020 2020  tern:.          
+00000fe0: 2d20 7479 7065 3a20 7472 616e 7361 6374  - type: transact
+00000ff0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+00001000: 6465 7374 696e 6174 696f 6e3a 203c 6465  destination: <de
+00001010: 785f 636f 6e74 7261 6374 3e0a 2020 2020  x_contract>.    
+00001020: 2020 2020 2020 2020 656e 7472 7970 6f69          entrypoi
+00001030: 6e74 3a20 6469 7665 7374 4c69 7175 6964  nt: divestLiquid
+00001040: 6974 790a 2020 2020 2020 2020 2020 2d20  ity.          - 
+00001050: 7479 7065 3a20 7472 616e 7361 6374 696f  type: transactio
+00001060: 6e0a 2020 2020 2020 2020 2020 2020 6465  n.            de
+00001070: 7374 696e 6174 696f 6e3a 203c 746f 6b65  stination: <toke
+00001080: 6e5f 636f 6e74 7261 6374 3e0a 2020 2020  n_contract>.    
+00001090: 2020 2020 2020 2020 656e 7472 7970 6f69          entrypoi
+000010a0: 6e74 3a20 7472 616e 7366 6572 0a20 2020  nt: transfer.   
+000010b0: 2020 2020 2020 202d 2074 7970 653a 2074         - type: t
+000010c0: 7261 6e73 6163 7469 6f6e 0a20 2020 2020  ransaction.     
+000010d0: 2020 2020 2020 2073 6f75 7263 653a 203c         source: <
+000010e0: 6465 785f 636f 6e74 7261 6374 3e0a 2020  dex_contract>.  
+000010f0: 2020 2020 2d20 6361 6c6c 6261 636b 3a20      - callback: 
+00001100: 6f6e 5f66 6132 5f77 6974 6864 7261 775f  on_fa2_withdraw_
+00001110: 7072 6f66 6974 0a20 2020 2020 2020 2070  profit.        p
+00001120: 6174 7465 726e 3a0a 2020 2020 2020 2020  attern:.        
+00001130: 2020 2d20 7479 7065 3a20 7472 616e 7361    - type: transa
+00001140: 6374 696f 6e0a 2020 2020 2020 2020 2020  ction.          
+00001150: 2020 6465 7374 696e 6174 696f 6e3a 203c    destination: <
+00001160: 6465 785f 636f 6e74 7261 6374 3e0a 2020  dex_contract>.  
+00001170: 2020 2020 2020 2020 2020 656e 7472 7970            entryp
+00001180: 6f69 6e74 3a20 7769 7468 6472 6177 5072  oint: withdrawPr
+00001190: 6f66 6974 0a20 2020 2020 2020 2020 202d  ofit.          -
+000011a0: 2074 7970 653a 2074 7261 6e73 6163 7469   type: transacti
+000011b0: 6f6e 0a20 2020 2020 2020 2020 2020 2073  on.            s
+000011c0: 6f75 7263 653a 203c 6465 785f 636f 6e74  ource: <dex_cont
+000011d0: 7261 6374 3e0a 2020 2020 2020 2020 2020  ract>.          
+000011e0: 2020 6f70 7469 6f6e 616c 3a20 5472 7565    optional: True
+000011f0: 0a20 2020 2066 6972 7374 5f6c 6576 656c  .    first_level
+00001200: 3a20 3134 3037 3532 380a 2020 2020 6c61  : 1407528.    la
+00001210: 7374 5f6c 6576 656c 3a20 3134 3434 3133  st_level: 144413
+00001220: 330a 0a69 6e64 6578 6573 3a0a 2020 6b75  3..indexes:.  ku
+00001230: 7364 5f6d 6169 6e6e 6574 3a0a 2020 2020  sd_mainnet:.    
+00001240: 7465 6d70 6c61 7465 3a20 7175 6970 7573  template: quipus
+00001250: 7761 705f 6661 3132 0a20 2020 2076 616c  wap_fa12.    val
+00001260: 7565 733a 0a20 2020 2020 2064 6578 5f63  ues:.      dex_c
+00001270: 6f6e 7472 6163 743a 206b 7573 645f 6465  ontract: kusd_de
+00001280: 785f 6d61 696e 6e65 740a 2020 2020 2020  x_mainnet.      
+00001290: 746f 6b65 6e5f 636f 6e74 7261 6374 3a20  token_contract: 
+000012a0: 6b75 7364 5f74 6f6b 656e 5f6d 6169 6e6e  kusd_token_mainn
+000012b0: 6574 0a20 2020 2020 2073 796d 626f 6c3a  et.      symbol:
+000012c0: 206b 5553 440a 2020 2020 2020 6465 6369   kUSD.      deci
+000012d0: 6d61 6c73 3a20 3138 0a0a 2020 6864 616f  mals: 18..  hdao
+000012e0: 5f6d 6169 6e6e 6574 3a0a 2020 2020 7465  _mainnet:.    te
+000012f0: 6d70 6c61 7465 3a20 7175 6970 7573 7761  mplate: quipuswa
+00001300: 705f 6661 320a 2020 2020 7661 6c75 6573  p_fa2.    values
+00001310: 3a0a 2020 2020 2020 6465 785f 636f 6e74  :.      dex_cont
+00001320: 7261 6374 3a20 6864 616f 5f64 6578 5f6d  ract: hdao_dex_m
+00001330: 6169 6e6e 6574 0a20 2020 2020 2074 6f6b  ainnet.      tok
+00001340: 656e 5f63 6f6e 7472 6163 743a 2068 6461  en_contract: hda
+00001350: 6f5f 746f 6b65 6e5f 6d61 696e 6e65 740a  o_token_mainnet.
+00001360: 2020 2020 2020 7379 6d62 6f6c 3a20 6844        symbol: hD
+00001370: 414f 0a20 2020 2020 2064 6563 696d 616c  AO.      decimal
+00001380: 733a 2036 0a0a 6c6f 6767 696e 673a 2057  s: 6..logging: W
+00001390: 4152 4e0a                                ARN.
```

### Comparing `dipdup-7.0.0rc1/tests/configs/demo_domains.yml` & `dipdup-7.0.0rc2/tests/configs/demo_domains.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,59 +1,57 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
-00000020: 646f 6d61 696e 730a 0a64 6174 6162 6173  domains..databas
-00000030: 653a 0a20 206b 696e 643a 2073 716c 6974  e:.  kind: sqlit
-00000040: 650a 2020 7061 7468 3a20 6462 2e73 716c  e.  path: db.sql
-00000050: 6974 6533 0a0a 636f 6e74 7261 6374 733a  ite3..contracts:
-00000060: 0a20 206e 616d 655f 7265 6769 7374 7279  .  name_registry
-00000070: 3a0a 2020 2020 6b69 6e64 3a20 7465 7a6f  :.    kind: tezo
-00000080: 730a 2020 2020 6164 6472 6573 733a 204b  s.    address: K
-00000090: 5431 4742 5a6d 5378 6d6e 4b4a 5847 4d64  T1GBZmSxmnKJXGMd
-000000a0: 4d4c 6275 6750 664c 7955 506d 754c 534d  MLbugPfLyUPmuLSM
-000000b0: 774b 530a 2020 2020 7479 7065 6e61 6d65  wKS.    typename
-000000c0: 3a20 6e61 6d65 5f72 6567 6973 7472 790a  : name_registry.
-000000d0: 0a64 6174 6173 6f75 7263 6573 3a0a 2020  .datasources:.  
-000000e0: 747a 6b74 3a0a 2020 2020 6b69 6e64 3a20  tzkt:.    kind: 
-000000f0: 7465 7a6f 732e 747a 6b74 0a20 2020 2075  tezos.tzkt.    u
-00000100: 726c 3a20 247b 545a 4b54 5f55 524c 3a2d  rl: ${TZKT_URL:-
-00000110: 6874 7470 733a 2f2f 6170 692e 747a 6b74  https://api.tzkt
-00000120: 2e69 6f7d 0a20 2020 2068 7474 703a 0a20  .io}.    http:. 
-00000130: 2020 2020 2072 6570 6c61 795f 7061 7468       replay_path
-00000140: 3a20 247b 4449 5044 5550 5f52 4550 4c41  : ${DIPDUP_REPLA
-00000150: 595f 5041 5448 3a2d 7d0a 0a74 656d 706c  Y_PATH:-}..templ
-00000160: 6174 6573 3a0a 2020 646f 6d61 696e 733a  ates:.  domains:
-00000170: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
-00000180: 2e74 7a6b 742e 6f70 6572 6174 696f 6e73  .tzkt.operations
-00000190: 0a20 2020 2064 6174 6173 6f75 7263 653a  .    datasource:
-000001a0: 203c 6461 7461 736f 7572 6365 3e0a 2020   <datasource>.  
-000001b0: 2020 636f 6e74 7261 6374 733a 0a20 2020    contracts:.   
-000001c0: 2020 202d 203c 6e61 6d65 5f72 6567 6973     - <name_regis
-000001d0: 7472 793e 0a20 2020 2068 616e 646c 6572  try>.    handler
-000001e0: 733a 0a20 2020 2020 202d 2063 616c 6c62  s:.      - callb
-000001f0: 6163 6b3a 206f 6e5f 6164 6d69 6e5f 7570  ack: on_admin_up
-00000200: 6461 7465 0a20 2020 2020 2020 2070 6174  date.        pat
-00000210: 7465 726e 3a0a 2020 2020 2020 2020 2020  tern:.          
-00000220: 2d20 7479 7065 3a20 7472 616e 7361 6374  - type: transact
-00000230: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-00000240: 6465 7374 696e 6174 696f 6e3a 203c 6e61  destination: <na
-00000250: 6d65 5f72 6567 6973 7472 793e 0a20 2020  me_registry>.   
-00000260: 2020 2020 2020 2020 2065 6e74 7279 706f           entrypo
-00000270: 696e 743a 2061 646d 696e 5f75 7064 6174  int: admin_updat
-00000280: 650a 2020 2020 2020 2d20 6361 6c6c 6261  e.      - callba
-00000290: 636b 3a20 6f6e 5f65 7865 6375 7465 0a20  ck: on_execute. 
-000002a0: 2020 2020 2020 2070 6174 7465 726e 3a0a         pattern:.
-000002b0: 2020 2020 2020 2020 2020 2d20 7479 7065            - type
-000002c0: 3a20 7472 616e 7361 6374 696f 6e0a 2020  : transaction.  
-000002d0: 2020 2020 2020 2020 2020 6465 7374 696e            destin
-000002e0: 6174 696f 6e3a 203c 6e61 6d65 5f72 6567  ation: <name_reg
-000002f0: 6973 7472 793e 0a20 2020 2020 2020 2020  istry>.         
-00000300: 2020 2065 6e74 7279 706f 696e 743a 2065     entrypoint: e
-00000310: 7865 6375 7465 0a20 2020 206c 6173 745f  xecute.    last_
-00000320: 6c65 7665 6c3a 2031 3435 3038 3532 0a0a  level: 1450852..
-00000330: 696e 6465 7865 733a 0a20 2064 6f6d 6169  indexes:.  domai
-00000340: 6e73 3a0a 2020 2020 7465 6d70 6c61 7465  ns:.    template
-00000350: 3a20 646f 6d61 696e 730a 2020 2020 7661  : domains.    va
-00000360: 6c75 6573 3a0a 2020 2020 2020 6461 7461  lues:.      data
-00000370: 736f 7572 6365 3a20 747a 6b74 0a20 2020  source: tzkt.   
-00000380: 2020 206e 616d 655f 7265 6769 7374 7279     name_registry
-00000390: 3a20 6e61 6d65 5f72 6567 6973 7472 790a  : name_registry.
-000003a0: 0a6c 6f67 6769 6e67 3a20 5741 524e 0a    .logging: WARN.
+00000020: 646f 6d61 696e 730a 0a63 6f6e 7472 6163  domains..contrac
+00000030: 7473 3a0a 2020 6e61 6d65 5f72 6567 6973  ts:.  name_regis
+00000040: 7472 793a 0a20 2020 206b 696e 643a 2074  try:.    kind: t
+00000050: 657a 6f73 0a20 2020 2061 6464 7265 7373  ezos.    address
+00000060: 3a20 4b54 3147 425a 6d53 786d 6e4b 4a58  : KT1GBZmSxmnKJX
+00000070: 474d 644d 4c62 7567 5066 4c79 5550 6d75  GMdMLbugPfLyUPmu
+00000080: 4c53 4d77 4b53 0a20 2020 2074 7970 656e  LSMwKS.    typen
+00000090: 616d 653a 206e 616d 655f 7265 6769 7374  ame: name_regist
+000000a0: 7279 0a0a 6461 7461 736f 7572 6365 733a  ry..datasources:
+000000b0: 0a20 2074 7a6b 743a 0a20 2020 206b 696e  .  tzkt:.    kin
+000000c0: 643a 2074 657a 6f73 2e74 7a6b 740a 2020  d: tezos.tzkt.  
+000000d0: 2020 7572 6c3a 2024 7b54 5a4b 545f 5552    url: ${TZKT_UR
+000000e0: 4c3a 2d68 7474 7073 3a2f 2f61 7069 2e74  L:-https://api.t
+000000f0: 7a6b 742e 696f 7d0a 2020 2020 6874 7470  zkt.io}.    http
+00000100: 3a0a 2020 2020 2020 7265 706c 6179 5f70  :.      replay_p
+00000110: 6174 683a 2024 7b44 4950 4455 505f 5245  ath: ${DIPDUP_RE
+00000120: 504c 4159 5f50 4154 483a 2d7d 0a0a 7465  PLAY_PATH:-}..te
+00000130: 6d70 6c61 7465 733a 0a20 2064 6f6d 6169  mplates:.  domai
+00000140: 6e73 3a0a 2020 2020 6b69 6e64 3a20 7465  ns:.    kind: te
+00000150: 7a6f 732e 747a 6b74 2e6f 7065 7261 7469  zos.tzkt.operati
+00000160: 6f6e 730a 2020 2020 6461 7461 736f 7572  ons.    datasour
+00000170: 6365 3a20 3c64 6174 6173 6f75 7263 653e  ce: <datasource>
+00000180: 0a20 2020 2063 6f6e 7472 6163 7473 3a0a  .    contracts:.
+00000190: 2020 2020 2020 2d20 3c6e 616d 655f 7265        - <name_re
+000001a0: 6769 7374 7279 3e0a 2020 2020 6861 6e64  gistry>.    hand
+000001b0: 6c65 7273 3a0a 2020 2020 2020 2d20 6361  lers:.      - ca
+000001c0: 6c6c 6261 636b 3a20 6f6e 5f61 646d 696e  llback: on_admin
+000001d0: 5f75 7064 6174 650a 2020 2020 2020 2020  _update.        
+000001e0: 7061 7474 6572 6e3a 0a20 2020 2020 2020  pattern:.       
+000001f0: 2020 202d 2074 7970 653a 2074 7261 6e73     - type: trans
+00000200: 6163 7469 6f6e 0a20 2020 2020 2020 2020  action.         
+00000210: 2020 2064 6573 7469 6e61 7469 6f6e 3a20     destination: 
+00000220: 3c6e 616d 655f 7265 6769 7374 7279 3e0a  <name_registry>.
+00000230: 2020 2020 2020 2020 2020 2020 656e 7472              entr
+00000240: 7970 6f69 6e74 3a20 6164 6d69 6e5f 7570  ypoint: admin_up
+00000250: 6461 7465 0a20 2020 2020 202d 2063 616c  date.      - cal
+00000260: 6c62 6163 6b3a 206f 6e5f 6578 6563 7574  lback: on_execut
+00000270: 650a 2020 2020 2020 2020 7061 7474 6572  e.        patter
+00000280: 6e3a 0a20 2020 2020 2020 2020 202d 2074  n:.          - t
+00000290: 7970 653a 2074 7261 6e73 6163 7469 6f6e  ype: transaction
+000002a0: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
+000002b0: 7469 6e61 7469 6f6e 3a20 3c6e 616d 655f  tination: <name_
+000002c0: 7265 6769 7374 7279 3e0a 2020 2020 2020  registry>.      
+000002d0: 2020 2020 2020 656e 7472 7970 6f69 6e74        entrypoint
+000002e0: 3a20 6578 6563 7574 650a 2020 2020 6c61  : execute.    la
+000002f0: 7374 5f6c 6576 656c 3a20 3134 3530 3835  st_level: 145085
+00000300: 320a 0a69 6e64 6578 6573 3a0a 2020 646f  2..indexes:.  do
+00000310: 6d61 696e 733a 0a20 2020 2074 656d 706c  mains:.    templ
+00000320: 6174 653a 2064 6f6d 6169 6e73 0a20 2020  ate: domains.   
+00000330: 2076 616c 7565 733a 0a20 2020 2020 2064   values:.      d
+00000340: 6174 6173 6f75 7263 653a 2074 7a6b 740a  atasource: tzkt.
+00000350: 2020 2020 2020 6e61 6d65 5f72 6567 6973        name_regis
+00000360: 7472 793a 206e 616d 655f 7265 6769 7374  try: name_regist
+00000370: 7279 0a0a 6c6f 6767 696e 673a 2057 4152  ry..logging: WAR
+00000380: 4e0a                                     N.
```

### Comparing `dipdup-7.0.0rc1/tests/configs/demo_factories.yml` & `dipdup-7.0.0rc2/tests/configs/demo_nft_marketplace.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,83 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
-00000020: 6661 6374 6f72 6965 730a 0a64 6174 6162  factories..datab
-00000030: 6173 653a 0a20 206b 696e 643a 2073 716c  ase:.  kind: sql
-00000040: 6974 650a 2020 7061 7468 3a20 6462 2e73  ite.  path: db.s
-00000050: 716c 6974 6533 0a0a 636f 6e74 7261 6374  qlite3..contract
-00000060: 733a 0a20 2072 6567 6973 7472 793a 0a20  s:.  registry:. 
-00000070: 2020 206b 696e 643a 2074 657a 6f73 0a20     kind: tezos. 
-00000080: 2020 2063 6f64 655f 6861 7368 3a20 4b54     code_hash: KT
-00000090: 3139 4346 334b 4b72 7664 5737 3774 7446  19CF3KKrvdW77ttF
-000000a0: 6f6d 4375 696e 326b 3475 4156 6b72 7959  omCuin2k4uAVkryY
-000000b0: 7168 0a20 2020 2074 7970 656e 616d 653a  qh.    typename:
-000000c0: 2072 6567 6973 7472 790a 0a64 6174 6173   registry..datas
-000000d0: 6f75 7263 6573 3a0a 2020 747a 6b74 3a0a  ources:.  tzkt:.
-000000e0: 2020 2020 6b69 6e64 3a20 7465 7a6f 732e      kind: tezos.
-000000f0: 747a 6b74 0a20 2020 2075 726c 3a20 247b  tzkt.    url: ${
-00000100: 545a 4b54 5f55 524c 3a2d 6874 7470 733a  TZKT_URL:-https:
-00000110: 2f2f 6170 692e 747a 6b74 2e69 6f7d 0a20  //api.tzkt.io}. 
-00000120: 2020 2068 7474 703a 0a20 2020 2020 2072     http:.      r
-00000130: 6570 6c61 795f 7061 7468 3a20 247b 4449  eplay_path: ${DI
-00000140: 5044 5550 5f52 4550 4c41 595f 5041 5448  PDUP_REPLAY_PATH
-00000150: 3a2d 7d0a 0a74 656d 706c 6174 6573 3a0a  :-}..templates:.
-00000160: 0a20 2072 6567 6973 7472 795f 6461 6f3a  .  registry_dao:
-00000170: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
-00000180: 2e74 7a6b 742e 6f70 6572 6174 696f 6e73  .tzkt.operations
-00000190: 0a20 2020 2064 6174 6173 6f75 7263 653a  .    datasource:
-000001a0: 2074 7a6b 740a 2020 2020 7479 7065 733a   tzkt.    types:
-000001b0: 0a20 2020 2020 202d 2074 7261 6e73 6163  .      - transac
-000001c0: 7469 6f6e 0a20 2020 2020 202d 206f 7269  tion.      - ori
-000001d0: 6769 6e61 7469 6f6e 0a20 2020 2063 6f6e  gination.    con
-000001e0: 7472 6163 7473 3a0a 2020 2020 2020 2d20  tracts:.      - 
-000001f0: 3c63 6f6e 7472 6163 743e 0a20 2020 2068  <contract>.    h
-00000200: 616e 646c 6572 733a 0a20 2020 2020 202d  andlers:.      -
-00000210: 2063 616c 6c62 6163 6b3a 206f 6e5f 7072   callback: on_pr
-00000220: 6f70 6f73 650a 2020 2020 2020 2020 7061  opose.        pa
-00000230: 7474 6572 6e3a 0a20 2020 2020 2020 2020  ttern:.         
-00000240: 202d 2074 7970 653a 2074 7261 6e73 6163   - type: transac
-00000250: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-00000260: 2064 6573 7469 6e61 7469 6f6e 3a20 3c63   destination: <c
-00000270: 6f6e 7472 6163 743e 0a20 2020 2020 2020  ontract>.       
-00000280: 2020 2020 2065 6e74 7279 706f 696e 743a       entrypoint:
-00000290: 2070 726f 706f 7365 0a20 2020 2020 202d   propose.      -
-000002a0: 2063 616c 6c62 6163 6b3a 206f 6e5f 6f72   callback: on_or
-000002b0: 6967 696e 6174 696f 6e0a 2020 2020 2020  igination.      
-000002c0: 2020 7061 7474 6572 6e3a 0a20 2020 2020    pattern:.     
-000002d0: 2020 2020 202d 2074 7970 653a 206f 7269       - type: ori
-000002e0: 6769 6e61 7469 6f6e 0a20 2020 2020 2020  gination.       
-000002f0: 2020 2020 206f 7269 6769 6e61 7465 645f       originated_
-00000300: 636f 6e74 7261 6374 3a20 3c63 6f6e 7472  contract: <contr
-00000310: 6163 743e 0a0a 696e 6465 7865 733a 0a20  act>..indexes:. 
-00000320: 2072 6567 6973 7472 793a 0a20 2020 2074   registry:.    t
-00000330: 656d 706c 6174 653a 2072 6567 6973 7472  emplate: registr
-00000340: 795f 6461 6f0a 2020 2020 7661 6c75 6573  y_dao.    values
-00000350: 3a0a 2020 2020 2020 636f 6e74 7261 6374  :.      contract
-00000360: 3a20 7265 6769 7374 7279 0a20 2020 2066  : registry.    f
-00000370: 6972 7374 5f6c 6576 656c 3a20 3138 3831  irst_level: 1881
-00000380: 3631 390a 2020 2020 6c61 7374 5f6c 6576  619.    last_lev
-00000390: 656c 3a20 3239 3333 3530 35              el: 2933505
+00000020: 6e66 745f 6d61 726b 6574 706c 6163 650a  nft_marketplace.
+00000030: 0a63 6f6e 7472 6163 7473 3a0a 2020 4845  .contracts:.  HE
+00000040: 4e5f 6f62 6a6b 7473 3a0a 2020 2020 6b69  N_objkts:.    ki
+00000050: 6e64 3a20 7465 7a6f 730a 2020 2020 6164  nd: tezos.    ad
+00000060: 6472 6573 733a 2024 7b48 454e 5f4f 424a  dress: ${HEN_OBJ
+00000070: 4b54 533a 2d4b 5431 524a 3650 626a 4870  KTS:-KT1RJ6PbjHp
+00000080: 7763 334d 3572 7735 7332 4e62 6d65 6677  wc3M5rw5s2Nbmefw
+00000090: 6275 7762 6478 746f 6e7d 0a20 2020 2074  buwbdxton}.    t
+000000a0: 7970 656e 616d 653a 2068 656e 5f6f 626a  ypename: hen_obj
+000000b0: 6b74 730a 2020 4845 4e5f 6d69 6e74 6572  kts.  HEN_minter
+000000c0: 3a0a 2020 2020 6b69 6e64 3a20 7465 7a6f  :.    kind: tezo
+000000d0: 730a 2020 2020 6164 6472 6573 733a 2024  s.    address: $
+000000e0: 7b48 454e 5f4d 494e 5445 523a 2d4b 5431  {HEN_MINTER:-KT1
+000000f0: 486b 6735 7165 4e68 6677 704b 5734 6658  Hkg5qeNhfwpKW4fX
+00000100: 7671 3748 475a 4239 7a32 456e 6d43 4341  vq7HGZB9z2EnmCCA
+00000110: 397d 0a20 2020 2074 7970 656e 616d 653a  9}.    typename:
+00000120: 2068 656e 5f6d 696e 7465 720a 0a64 6174   hen_minter..dat
+00000130: 6173 6f75 7263 6573 3a0a 2020 747a 6b74  asources:.  tzkt
+00000140: 5f6d 6169 6e6e 6574 3a0a 2020 2020 6b69  _mainnet:.    ki
+00000150: 6e64 3a20 7465 7a6f 732e 747a 6b74 0a20  nd: tezos.tzkt. 
+00000160: 2020 2075 726c 3a20 247b 545a 4b54 5f55     url: ${TZKT_U
+00000170: 524c 3a2d 6874 7470 733a 2f2f 6170 692e  RL:-https://api.
+00000180: 747a 6b74 2e69 6f7d 0a20 2020 2068 7474  tzkt.io}.    htt
+00000190: 703a 0a20 2020 2020 2072 6570 6c61 795f  p:.      replay_
+000001a0: 7061 7468 3a20 247b 4449 5044 5550 5f52  path: ${DIPDUP_R
+000001b0: 4550 4c41 595f 5041 5448 3a2d 7d0a 0a69  EPLAY_PATH:-}..i
+000001c0: 6e64 6578 6573 3a0a 2020 6865 6e5f 6d61  ndexes:.  hen_ma
+000001d0: 696e 6e65 743a 0a20 2020 206b 696e 643a  innet:.    kind:
+000001e0: 2074 657a 6f73 2e74 7a6b 742e 6f70 6572   tezos.tzkt.oper
+000001f0: 6174 696f 6e73 0a20 2020 2064 6174 6173  ations.    datas
+00000200: 6f75 7263 653a 2074 7a6b 745f 6d61 696e  ource: tzkt_main
+00000210: 6e65 740a 2020 2020 636f 6e74 7261 6374  net.    contract
+00000220: 733a 0a20 2020 2020 202d 2048 454e 5f6d  s:.      - HEN_m
+00000230: 696e 7465 720a 2020 2020 6861 6e64 6c65  inter.    handle
+00000240: 7273 3a0a 2020 2020 2020 2d20 6361 6c6c  rs:.      - call
+00000250: 6261 636b 3a20 6f6e 5f6d 696e 740a 2020  back: on_mint.  
+00000260: 2020 2020 2020 7061 7474 6572 6e3a 0a20        pattern:. 
+00000270: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
+00000280: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
+00000290: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
+000002a0: 7469 6f6e 3a20 4845 4e5f 6d69 6e74 6572  tion: HEN_minter
+000002b0: 0a20 2020 2020 2020 2020 2020 2065 6e74  .            ent
+000002c0: 7279 706f 696e 743a 206d 696e 745f 4f42  rypoint: mint_OB
+000002d0: 4a4b 540a 2020 2020 2020 2020 2020 2d20  JKT.          - 
+000002e0: 7479 7065 3a20 7472 616e 7361 6374 696f  type: transactio
+000002f0: 6e0a 2020 2020 2020 2020 2020 2020 6465  n.            de
+00000300: 7374 696e 6174 696f 6e3a 2048 454e 5f6f  stination: HEN_o
+00000310: 626a 6b74 730a 2020 2020 2020 2020 2020  bjkts.          
+00000320: 2020 656e 7472 7970 6f69 6e74 3a20 6d69    entrypoint: mi
+00000330: 6e74 0a20 2020 2020 202d 2063 616c 6c62  nt.      - callb
+00000340: 6163 6b3a 206f 6e5f 7377 6170 0a20 2020  ack: on_swap.   
+00000350: 2020 2020 2070 6174 7465 726e 3a0a 2020       pattern:.  
+00000360: 2020 2020 2020 2020 2d20 7479 7065 3a20          - type: 
+00000370: 7472 616e 7361 6374 696f 6e0a 2020 2020  transaction.    
+00000380: 2020 2020 2020 2020 6465 7374 696e 6174          destinat
+00000390: 696f 6e3a 2048 454e 5f6d 696e 7465 720a  ion: HEN_minter.
+000003a0: 2020 2020 2020 2020 2020 2020 656e 7472              entr
+000003b0: 7970 6f69 6e74 3a20 7377 6170 0a20 2020  ypoint: swap.   
+000003c0: 2020 202d 2063 616c 6c62 6163 6b3a 206f     - callback: o
+000003d0: 6e5f 6361 6e63 656c 5f73 7761 700a 2020  n_cancel_swap.  
+000003e0: 2020 2020 2020 7061 7474 6572 6e3a 0a20        pattern:. 
+000003f0: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
+00000400: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
+00000410: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
+00000420: 7469 6f6e 3a20 4845 4e5f 6d69 6e74 6572  tion: HEN_minter
+00000430: 0a20 2020 2020 2020 2020 2020 2065 6e74  .            ent
+00000440: 7279 706f 696e 743a 2063 616e 6365 6c5f  rypoint: cancel_
+00000450: 7377 6170 0a20 2020 2020 202d 2063 616c  swap.      - cal
+00000460: 6c62 6163 6b3a 206f 6e5f 636f 6c6c 6563  lback: on_collec
+00000470: 740a 2020 2020 2020 2020 7061 7474 6572  t.        patter
+00000480: 6e3a 0a20 2020 2020 2020 2020 202d 2074  n:.          - t
+00000490: 7970 653a 2074 7261 6e73 6163 7469 6f6e  ype: transaction
+000004a0: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
+000004b0: 7469 6e61 7469 6f6e 3a20 4845 4e5f 6d69  tination: HEN_mi
+000004c0: 6e74 6572 0a20 2020 2020 2020 2020 2020  nter.           
+000004d0: 2065 6e74 7279 706f 696e 743a 2063 6f6c   entrypoint: col
+000004e0: 6c65 6374 0a20 2020 2066 6972 7374 5f6c  lect.    first_l
+000004f0: 6576 656c 3a20 3133 3635 3030 300a 2020  evel: 1365000.  
+00000500: 2020 6c61 7374 5f6c 6576 656c 3a20 3133    last_level: 13
+00000510: 3636 3030 300a 0a6c 6f67 6769 6e67 3a20  66000..logging: 
+00000520: 5741 524e                                WARN
```

### Comparing `dipdup-7.0.0rc1/tests/configs/demo_nft_marketplace.yml` & `dipdup-7.0.0rc2/tests/configs/dipdup.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,86 +1,79 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
 00000020: 6e66 745f 6d61 726b 6574 706c 6163 650a  nft_marketplace.
-00000030: 0a64 6174 6162 6173 653a 0a20 206b 696e  .database:.  kin
-00000040: 643a 2073 716c 6974 650a 2020 7061 7468  d: sqlite.  path
-00000050: 3a20 6462 2e73 716c 6974 6533 0a0a 636f  : db.sqlite3..co
-00000060: 6e74 7261 6374 733a 0a20 2048 454e 5f6f  ntracts:.  HEN_o
-00000070: 626a 6b74 733a 0a20 2020 206b 696e 643a  bjkts:.    kind:
-00000080: 2074 657a 6f73 0a20 2020 2061 6464 7265   tezos.    addre
-00000090: 7373 3a20 247b 4845 4e5f 4f42 4a4b 5453  ss: ${HEN_OBJKTS
-000000a0: 3a2d 4b54 3152 4a36 5062 6a48 7077 6333  :-KT1RJ6PbjHpwc3
-000000b0: 4d35 7277 3573 324e 626d 6566 7762 7577  M5rw5s2Nbmefwbuw
-000000c0: 6264 7874 6f6e 7d0a 2020 2020 7479 7065  bdxton}.    type
-000000d0: 6e61 6d65 3a20 6865 6e5f 6f62 6a6b 7473  name: hen_objkts
-000000e0: 0a20 2048 454e 5f6d 696e 7465 723a 0a20  .  HEN_minter:. 
-000000f0: 2020 206b 696e 643a 2074 657a 6f73 0a20     kind: tezos. 
-00000100: 2020 2061 6464 7265 7373 3a20 247b 4845     address: ${HE
-00000110: 4e5f 4d49 4e54 4552 3a2d 4b54 3148 6b67  N_MINTER:-KT1Hkg
-00000120: 3571 654e 6866 7770 4b57 3466 5876 7137  5qeNhfwpKW4fXvq7
-00000130: 4847 5a42 397a 3245 6e6d 4343 4139 7d0a  HGZB9z2EnmCCA9}.
-00000140: 2020 2020 7479 7065 6e61 6d65 3a20 6865      typename: he
-00000150: 6e5f 6d69 6e74 6572 0a0a 6461 7461 736f  n_minter..dataso
-00000160: 7572 6365 733a 0a20 2074 7a6b 745f 6d61  urces:.  tzkt_ma
-00000170: 696e 6e65 743a 0a20 2020 206b 696e 643a  innet:.    kind:
-00000180: 2074 657a 6f73 2e74 7a6b 740a 2020 2020   tezos.tzkt.    
-00000190: 7572 6c3a 2024 7b54 5a4b 545f 5552 4c3a  url: ${TZKT_URL:
-000001a0: 2d68 7474 7073 3a2f 2f61 7069 2e74 7a6b  -https://api.tzk
-000001b0: 742e 696f 7d0a 2020 2020 6874 7470 3a0a  t.io}.    http:.
-000001c0: 2020 2020 2020 7265 706c 6179 5f70 6174        replay_pat
-000001d0: 683a 2024 7b44 4950 4455 505f 5245 504c  h: ${DIPDUP_REPL
-000001e0: 4159 5f50 4154 483a 2d7d 0a0a 696e 6465  AY_PATH:-}..inde
-000001f0: 7865 733a 0a20 2068 656e 5f6d 6169 6e6e  xes:.  hen_mainn
-00000200: 6574 3a0a 2020 2020 6b69 6e64 3a20 7465  et:.    kind: te
-00000210: 7a6f 732e 747a 6b74 2e6f 7065 7261 7469  zos.tzkt.operati
-00000220: 6f6e 730a 2020 2020 6461 7461 736f 7572  ons.    datasour
-00000230: 6365 3a20 747a 6b74 5f6d 6169 6e6e 6574  ce: tzkt_mainnet
-00000240: 0a20 2020 2063 6f6e 7472 6163 7473 3a0a  .    contracts:.
-00000250: 2020 2020 2020 2d20 4845 4e5f 6d69 6e74        - HEN_mint
-00000260: 6572 0a20 2020 2068 616e 646c 6572 733a  er.    handlers:
-00000270: 0a20 2020 2020 202d 2063 616c 6c62 6163  .      - callbac
-00000280: 6b3a 206f 6e5f 6d69 6e74 0a20 2020 2020  k: on_mint.     
-00000290: 2020 2070 6174 7465 726e 3a0a 2020 2020     pattern:.    
-000002a0: 2020 2020 2020 2d20 7479 7065 3a20 7472        - type: tr
-000002b0: 616e 7361 6374 696f 6e0a 2020 2020 2020  ansaction.      
-000002c0: 2020 2020 2020 6465 7374 696e 6174 696f        destinatio
-000002d0: 6e3a 2048 454e 5f6d 696e 7465 720a 2020  n: HEN_minter.  
-000002e0: 2020 2020 2020 2020 2020 656e 7472 7970            entryp
-000002f0: 6f69 6e74 3a20 6d69 6e74 5f4f 424a 4b54  oint: mint_OBJKT
-00000300: 0a20 2020 2020 2020 2020 202d 2074 7970  .          - typ
-00000310: 653a 2074 7261 6e73 6163 7469 6f6e 0a20  e: transaction. 
-00000320: 2020 2020 2020 2020 2020 2064 6573 7469             desti
-00000330: 6e61 7469 6f6e 3a20 4845 4e5f 6f62 6a6b  nation: HEN_objk
-00000340: 7473 0a20 2020 2020 2020 2020 2020 2065  ts.            e
-00000350: 6e74 7279 706f 696e 743a 206d 696e 740a  ntrypoint: mint.
-00000360: 2020 2020 2020 2d20 6361 6c6c 6261 636b        - callback
-00000370: 3a20 6f6e 5f73 7761 700a 2020 2020 2020  : on_swap.      
-00000380: 2020 7061 7474 6572 6e3a 0a20 2020 2020    pattern:.     
-00000390: 2020 2020 202d 2074 7970 653a 2074 7261       - type: tra
-000003a0: 6e73 6163 7469 6f6e 0a20 2020 2020 2020  nsaction.       
-000003b0: 2020 2020 2064 6573 7469 6e61 7469 6f6e       destination
-000003c0: 3a20 4845 4e5f 6d69 6e74 6572 0a20 2020  : HEN_minter.   
-000003d0: 2020 2020 2020 2020 2065 6e74 7279 706f           entrypo
-000003e0: 696e 743a 2073 7761 700a 2020 2020 2020  int: swap.      
-000003f0: 2d20 6361 6c6c 6261 636b 3a20 6f6e 5f63  - callback: on_c
-00000400: 616e 6365 6c5f 7377 6170 0a20 2020 2020  ancel_swap.     
-00000410: 2020 2070 6174 7465 726e 3a0a 2020 2020     pattern:.    
-00000420: 2020 2020 2020 2d20 7479 7065 3a20 7472        - type: tr
-00000430: 616e 7361 6374 696f 6e0a 2020 2020 2020  ansaction.      
-00000440: 2020 2020 2020 6465 7374 696e 6174 696f        destinatio
-00000450: 6e3a 2048 454e 5f6d 696e 7465 720a 2020  n: HEN_minter.  
-00000460: 2020 2020 2020 2020 2020 656e 7472 7970            entryp
-00000470: 6f69 6e74 3a20 6361 6e63 656c 5f73 7761  oint: cancel_swa
-00000480: 700a 2020 2020 2020 2d20 6361 6c6c 6261  p.      - callba
-00000490: 636b 3a20 6f6e 5f63 6f6c 6c65 6374 0a20  ck: on_collect. 
-000004a0: 2020 2020 2020 2070 6174 7465 726e 3a0a         pattern:.
-000004b0: 2020 2020 2020 2020 2020 2d20 7479 7065            - type
-000004c0: 3a20 7472 616e 7361 6374 696f 6e0a 2020  : transaction.  
-000004d0: 2020 2020 2020 2020 2020 6465 7374 696e            destin
-000004e0: 6174 696f 6e3a 2048 454e 5f6d 696e 7465  ation: HEN_minte
-000004f0: 720a 2020 2020 2020 2020 2020 2020 656e  r.            en
-00000500: 7472 7970 6f69 6e74 3a20 636f 6c6c 6563  trypoint: collec
-00000510: 740a 2020 2020 6669 7273 745f 6c65 7665  t.    first_leve
-00000520: 6c3a 2031 3336 3530 3030 0a20 2020 206c  l: 1365000.    l
-00000530: 6173 745f 6c65 7665 6c3a 2031 3336 3630  ast_level: 13660
-00000540: 3030 0a0a 6c6f 6767 696e 673a 2057 4152  00..logging: WAR
-00000550: 4e                                       N
+00000030: 0a63 6f6e 7472 6163 7473 3a0a 2020 4845  .contracts:.  HE
+00000040: 4e5f 6f62 6a6b 7473 3a0a 2020 2020 6b69  N_objkts:.    ki
+00000050: 6e64 3a20 7465 7a6f 730a 2020 2020 6164  nd: tezos.    ad
+00000060: 6472 6573 733a 2024 7b48 454e 5f4f 424a  dress: ${HEN_OBJ
+00000070: 4b54 533a 2d4b 5431 524a 3650 626a 4870  KTS:-KT1RJ6PbjHp
+00000080: 7763 334d 3572 7735 7332 4e62 6d65 6677  wc3M5rw5s2Nbmefw
+00000090: 6275 7762 6478 746f 6e7d 0a20 2020 2074  buwbdxton}.    t
+000000a0: 7970 656e 616d 653a 2068 656e 5f6f 626a  ypename: hen_obj
+000000b0: 6b74 730a 2020 4845 4e5f 6d69 6e74 6572  kts.  HEN_minter
+000000c0: 3a0a 2020 2020 6b69 6e64 3a20 7465 7a6f  :.    kind: tezo
+000000d0: 730a 2020 2020 6164 6472 6573 733a 2024  s.    address: $
+000000e0: 7b48 454e 5f4d 494e 5445 523a 2d4b 5431  {HEN_MINTER:-KT1
+000000f0: 486b 6735 7165 4e68 6677 704b 5734 6658  Hkg5qeNhfwpKW4fX
+00000100: 7671 3748 475a 4239 7a32 456e 6d43 4341  vq7HGZB9z2EnmCCA
+00000110: 397d 0a20 2020 2074 7970 656e 616d 653a  9}.    typename:
+00000120: 2068 656e 5f6d 696e 7465 720a 0a64 6174   hen_minter..dat
+00000130: 6173 6f75 7263 6573 3a0a 2020 747a 6b74  asources:.  tzkt
+00000140: 5f6d 6169 6e6e 6574 3a0a 2020 2020 6b69  _mainnet:.    ki
+00000150: 6e64 3a20 7465 7a6f 732e 747a 6b74 0a20  nd: tezos.tzkt. 
+00000160: 2020 2075 726c 3a20 247b 545a 4b54 5f55     url: ${TZKT_U
+00000170: 524c 3a2d 6874 7470 733a 2f2f 6170 692e  RL:-https://api.
+00000180: 747a 6b74 2e69 6f7d 0a20 2020 2068 7474  tzkt.io}.    htt
+00000190: 703a 0a20 2020 2020 2072 6570 6c61 795f  p:.      replay_
+000001a0: 7061 7468 3a20 247b 4449 5044 5550 5f52  path: ${DIPDUP_R
+000001b0: 4550 4c41 595f 5041 5448 3a2d 7d0a 0a69  EPLAY_PATH:-}..i
+000001c0: 6e64 6578 6573 3a0a 2020 6865 6e5f 6d61  ndexes:.  hen_ma
+000001d0: 696e 6e65 743a 0a20 2020 206b 696e 643a  innet:.    kind:
+000001e0: 2074 657a 6f73 2e74 7a6b 742e 6f70 6572   tezos.tzkt.oper
+000001f0: 6174 696f 6e73 0a20 2020 2064 6174 6173  ations.    datas
+00000200: 6f75 7263 653a 2074 7a6b 745f 6d61 696e  ource: tzkt_main
+00000210: 6e65 740a 2020 2020 636f 6e74 7261 6374  net.    contract
+00000220: 733a 0a20 2020 2020 202d 2048 454e 5f6d  s:.      - HEN_m
+00000230: 696e 7465 720a 2020 2020 6861 6e64 6c65  inter.    handle
+00000240: 7273 3a0a 2020 2020 2020 2d20 6361 6c6c  rs:.      - call
+00000250: 6261 636b 3a20 6f6e 5f6d 696e 740a 2020  back: on_mint.  
+00000260: 2020 2020 2020 7061 7474 6572 6e3a 0a20        pattern:. 
+00000270: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
+00000280: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
+00000290: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
+000002a0: 7469 6f6e 3a20 4845 4e5f 6d69 6e74 6572  tion: HEN_minter
+000002b0: 0a20 2020 2020 2020 2020 2020 2065 6e74  .            ent
+000002c0: 7279 706f 696e 743a 206d 696e 745f 4f42  rypoint: mint_OB
+000002d0: 4a4b 540a 2020 2020 2020 2020 2020 2d20  JKT.          - 
+000002e0: 7479 7065 3a20 7472 616e 7361 6374 696f  type: transactio
+000002f0: 6e0a 2020 2020 2020 2020 2020 2020 6465  n.            de
+00000300: 7374 696e 6174 696f 6e3a 2048 454e 5f6f  stination: HEN_o
+00000310: 626a 6b74 730a 2020 2020 2020 2020 2020  bjkts.          
+00000320: 2020 656e 7472 7970 6f69 6e74 3a20 6d69    entrypoint: mi
+00000330: 6e74 0a20 2020 2020 202d 2063 616c 6c62  nt.      - callb
+00000340: 6163 6b3a 206f 6e5f 7377 6170 0a20 2020  ack: on_swap.   
+00000350: 2020 2020 2070 6174 7465 726e 3a0a 2020       pattern:.  
+00000360: 2020 2020 2020 2020 2d20 7479 7065 3a20          - type: 
+00000370: 7472 616e 7361 6374 696f 6e0a 2020 2020  transaction.    
+00000380: 2020 2020 2020 2020 6465 7374 696e 6174          destinat
+00000390: 696f 6e3a 2048 454e 5f6d 696e 7465 720a  ion: HEN_minter.
+000003a0: 2020 2020 2020 2020 2020 2020 656e 7472              entr
+000003b0: 7970 6f69 6e74 3a20 7377 6170 0a20 2020  ypoint: swap.   
+000003c0: 2020 202d 2063 616c 6c62 6163 6b3a 206f     - callback: o
+000003d0: 6e5f 6361 6e63 656c 5f73 7761 700a 2020  n_cancel_swap.  
+000003e0: 2020 2020 2020 7061 7474 6572 6e3a 0a20        pattern:. 
+000003f0: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
+00000400: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
+00000410: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
+00000420: 7469 6f6e 3a20 4845 4e5f 6d69 6e74 6572  tion: HEN_minter
+00000430: 0a20 2020 2020 2020 2020 2020 2065 6e74  .            ent
+00000440: 7279 706f 696e 743a 2063 616e 6365 6c5f  rypoint: cancel_
+00000450: 7377 6170 0a20 2020 2020 202d 2063 616c  swap.      - cal
+00000460: 6c62 6163 6b3a 206f 6e5f 636f 6c6c 6563  lback: on_collec
+00000470: 740a 2020 2020 2020 2020 7061 7474 6572  t.        patter
+00000480: 6e3a 0a20 2020 2020 2020 2020 202d 2074  n:.          - t
+00000490: 7970 653a 2074 7261 6e73 6163 7469 6f6e  ype: transaction
+000004a0: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
+000004b0: 7469 6e61 7469 6f6e 3a20 4845 4e5f 6d69  tination: HEN_mi
+000004c0: 6e74 6572 0a20 2020 2020 2020 2020 2020  nter.           
+000004d0: 2065 6e74 7279 706f 696e 743a 2063 6f6c   entrypoint: col
+000004e0: 6c65 6374                                lect
```

### Comparing `dipdup-7.0.0rc1/tests/configs/demo_raw.yml` & `dipdup-7.0.0rc2/tests/configs/demo_raw.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
-00000020: 7261 770a 0a64 6174 6162 6173 653a 0a20  raw..database:. 
-00000030: 206b 696e 643a 2073 716c 6974 650a 2020   kind: sqlite.  
-00000040: 7061 7468 3a20 6462 2e73 716c 6974 6533  path: db.sqlite3
-00000050: 0a0a 6461 7461 736f 7572 6365 733a 0a20  ..datasources:. 
-00000060: 2074 7a6b 743a 0a20 2020 206b 696e 643a   tzkt:.    kind:
-00000070: 2074 657a 6f73 2e74 7a6b 740a 2020 2020   tezos.tzkt.    
-00000080: 7572 6c3a 2024 7b54 5a4b 545f 5552 4c3a  url: ${TZKT_URL:
-00000090: 2d68 7474 7073 3a2f 2f61 7069 2e74 7a6b  -https://api.tzk
-000000a0: 742e 696f 7d0a 2020 2020 6874 7470 3a0a  t.io}.    http:.
-000000b0: 2020 2020 2020 7265 706c 6179 5f70 6174        replay_pat
-000000c0: 683a 2024 7b44 4950 4455 505f 5245 504c  h: ${DIPDUP_REPL
-000000d0: 4159 5f50 4154 483a 2d7d 0a0a 696e 6465  AY_PATH:-}..inde
-000000e0: 7865 733a 0a20 206d 6169 6e6e 6574 5f6f  xes:.  mainnet_o
-000000f0: 7065 7261 7469 6f6e 733a 0a20 2020 206b  perations:.    k
-00000100: 696e 643a 2074 657a 6f73 2e74 7a6b 742e  ind: tezos.tzkt.
-00000110: 6f70 6572 6174 696f 6e73 5f75 6e66 696c  operations_unfil
-00000120: 7465 7265 640a 2020 2020 6461 7461 736f  tered.    dataso
-00000130: 7572 6365 3a20 747a 6b74 0a20 2020 2074  urce: tzkt.    t
-00000140: 7970 6573 3a0a 2020 2020 2020 2d20 7472  ypes:.      - tr
-00000150: 616e 7361 6374 696f 6e0a 2020 2020 2020  ansaction.      
-00000160: 2d20 6d69 6772 6174 696f 6e0a 2020 2020  - migration.    
-00000170: 6361 6c6c 6261 636b 3a20 6f6e 5f6f 7065  callback: on_ope
-00000180: 7261 7469 6f6e 0a20 2020 2066 6972 7374  ration.    first
-00000190: 5f6c 6576 656c 3a20 3135 3839 3234 360a  _level: 1589246.
-000001a0: 2020 2020 6c61 7374 5f6c 6576 656c 3a20      last_level: 
-000001b0: 3135 3839 3234 370a 0a20 206d 6169 6e6e  1589247..  mainn
-000001c0: 6574 5f6f 7269 6769 6e61 7469 6f6e 733a  et_originations:
-000001d0: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
-000001e0: 2e74 7a6b 742e 6f70 6572 6174 696f 6e73  .tzkt.operations
-000001f0: 5f75 6e66 696c 7465 7265 640a 2020 2020  _unfiltered.    
-00000200: 6461 7461 736f 7572 6365 3a20 747a 6b74  datasource: tzkt
-00000210: 0a20 2020 2074 7970 6573 3a0a 2020 2020  .    types:.    
-00000220: 2020 2d20 6f72 6967 696e 6174 696f 6e0a    - origination.
-00000230: 2020 2020 6361 6c6c 6261 636b 3a20 6f6e      callback: on
-00000240: 5f6f 7065 7261 7469 6f6e 0a20 2020 2066  _operation.    f
-00000250: 6972 7374 5f6c 6576 656c 3a20 3135 3839  irst_level: 1589
-00000260: 3235 350a 2020 2020 6c61 7374 5f6c 6576  255.    last_lev
-00000270: 656c 3a20 3135 3839 3235 35              el: 1589255
+00000020: 7261 770a 0a64 6174 6173 6f75 7263 6573  raw..datasources
+00000030: 3a0a 2020 747a 6b74 3a0a 2020 2020 6b69  :.  tzkt:.    ki
+00000040: 6e64 3a20 7465 7a6f 732e 747a 6b74 0a20  nd: tezos.tzkt. 
+00000050: 2020 2075 726c 3a20 247b 545a 4b54 5f55     url: ${TZKT_U
+00000060: 524c 3a2d 6874 7470 733a 2f2f 6170 692e  RL:-https://api.
+00000070: 747a 6b74 2e69 6f7d 0a20 2020 2068 7474  tzkt.io}.    htt
+00000080: 703a 0a20 2020 2020 2072 6570 6c61 795f  p:.      replay_
+00000090: 7061 7468 3a20 247b 4449 5044 5550 5f52  path: ${DIPDUP_R
+000000a0: 4550 4c41 595f 5041 5448 3a2d 7d0a 0a69  EPLAY_PATH:-}..i
+000000b0: 6e64 6578 6573 3a0a 2020 6d61 696e 6e65  ndexes:.  mainne
+000000c0: 745f 6f70 6572 6174 696f 6e73 3a0a 2020  t_operations:.  
+000000d0: 2020 6b69 6e64 3a20 7465 7a6f 732e 747a    kind: tezos.tz
+000000e0: 6b74 2e6f 7065 7261 7469 6f6e 735f 756e  kt.operations_un
+000000f0: 6669 6c74 6572 6564 0a20 2020 2064 6174  filtered.    dat
+00000100: 6173 6f75 7263 653a 2074 7a6b 740a 2020  asource: tzkt.  
+00000110: 2020 7479 7065 733a 0a20 2020 2020 202d    types:.      -
+00000120: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
+00000130: 2020 202d 206d 6967 7261 7469 6f6e 0a20     - migration. 
+00000140: 2020 2063 616c 6c62 6163 6b3a 206f 6e5f     callback: on_
+00000150: 6f70 6572 6174 696f 6e0a 2020 2020 6669  operation.    fi
+00000160: 7273 745f 6c65 7665 6c3a 2031 3538 3932  rst_level: 15892
+00000170: 3436 0a20 2020 206c 6173 745f 6c65 7665  46.    last_leve
+00000180: 6c3a 2031 3538 3932 3437 0a0a 2020 6d61  l: 1589247..  ma
+00000190: 696e 6e65 745f 6f72 6967 696e 6174 696f  innet_originatio
+000001a0: 6e73 3a0a 2020 2020 6b69 6e64 3a20 7465  ns:.    kind: te
+000001b0: 7a6f 732e 747a 6b74 2e6f 7065 7261 7469  zos.tzkt.operati
+000001c0: 6f6e 735f 756e 6669 6c74 6572 6564 0a20  ons_unfiltered. 
+000001d0: 2020 2064 6174 6173 6f75 7263 653a 2074     datasource: t
+000001e0: 7a6b 740a 2020 2020 7479 7065 733a 0a20  zkt.    types:. 
+000001f0: 2020 2020 202d 206f 7269 6769 6e61 7469       - originati
+00000200: 6f6e 0a20 2020 2063 616c 6c62 6163 6b3a  on.    callback:
+00000210: 206f 6e5f 6f70 6572 6174 696f 6e0a 2020   on_operation.  
+00000220: 2020 6669 7273 745f 6c65 7665 6c3a 2031    first_level: 1
+00000230: 3538 3932 3535 0a20 2020 206c 6173 745f  589255.    last_
+00000240: 6c65 7665 6c3a 2031 3538 3932 3535       level: 1589255
```

### Comparing `dipdup-7.0.0rc1/tests/configs/demo_token.yml` & `dipdup-7.0.0rc2/tests/configs/demo_token_transfers_3.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,33 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
-00000020: 746f 6b65 6e0a 0a64 6174 6162 6173 653a  token..database:
-00000030: 0a20 206b 696e 643a 2073 716c 6974 650a  .  kind: sqlite.
-00000040: 2020 7061 7468 3a20 6462 2e73 716c 6974    path: db.sqlit
-00000050: 6533 0a0a 636f 6e74 7261 6374 733a 0a20  e3..contracts:. 
-00000060: 2074 7a62 7463 5f6d 6169 6e6e 6574 3a0a   tzbtc_mainnet:.
-00000070: 2020 2020 6b69 6e64 3a20 7465 7a6f 730a      kind: tezos.
-00000080: 2020 2020 6164 6472 6573 733a 204b 5431      address: KT1
-00000090: 5057 7832 6d6e 4475 656f 6f64 3766 456d  PWx2mnDueood7fEm
-000000a0: 6662 4244 4b78 3144 3942 416e 6e58 6974  fbBDKx1D9BAnnXit
-000000b0: 6e0a 2020 2020 7479 7065 6e61 6d65 3a20  n.    typename: 
-000000c0: 747a 6274 630a 0a64 6174 6173 6f75 7263  tzbtc..datasourc
-000000d0: 6573 3a0a 2020 747a 6b74 3a0a 2020 2020  es:.  tzkt:.    
-000000e0: 6b69 6e64 3a20 7465 7a6f 732e 747a 6b74  kind: tezos.tzkt
-000000f0: 0a20 2020 2075 726c 3a20 6874 7470 733a  .    url: https:
-00000100: 2f2f 6170 692e 747a 6b74 2e69 6f0a 2020  //api.tzkt.io.  
-00000110: 2020 6874 7470 3a0a 2020 2020 2020 7265    http:.      re
-00000120: 706c 6179 5f70 6174 683a 2024 7b44 4950  play_path: ${DIP
-00000130: 4455 505f 5245 504c 4159 5f50 4154 483a  DUP_REPLAY_PATH:
-00000140: 2d7d 0a0a 696e 6465 7865 733a 0a20 2074  -}..indexes:.  t
-00000150: 7a62 7463 5f68 6f6c 6465 7273 5f6d 6169  zbtc_holders_mai
-00000160: 6e6e 6574 3a0a 2020 2020 6b69 6e64 3a20  nnet:.    kind: 
-00000170: 7465 7a6f 732e 747a 6b74 2e6f 7065 7261  tezos.tzkt.opera
-00000180: 7469 6f6e 730a 2020 2020 6461 7461 736f  tions.    dataso
-00000190: 7572 6365 3a20 747a 6b74 0a20 2020 2063  urce: tzkt.    c
-000001a0: 6f6e 7472 6163 7473 3a0a 2020 2020 2020  ontracts:.      
-000001b0: 2d20 747a 6274 635f 6d61 696e 6e65 740a  - tzbtc_mainnet.
-000001c0: 2020 2020 6861 6e64 6c65 7273 3a0a 2020      handlers:.  
-000001d0: 2020 2020 2d20 6361 6c6c 6261 636b 3a20      - callback: 
-000001e0: 6f6e 5f74 7261 6e73 6665 720a 2020 2020  on_transfer.    
-000001f0: 2020 2020 7061 7474 6572 6e3a 0a20 2020      pattern:.   
-00000200: 2020 2020 2020 202d 2064 6573 7469 6e61         - destina
-00000210: 7469 6f6e 3a20 747a 6274 635f 6d61 696e  tion: tzbtc_main
-00000220: 6e65 740a 2020 2020 2020 2020 2020 2020  net.            
-00000230: 656e 7472 7970 6f69 6e74 3a20 7472 616e  entrypoint: tran
-00000240: 7366 6572 0a20 2020 2020 202d 2063 616c  sfer.      - cal
-00000250: 6c62 6163 6b3a 206f 6e5f 6d69 6e74 0a20  lback: on_mint. 
-00000260: 2020 2020 2020 2070 6174 7465 726e 3a0a         pattern:.
-00000270: 2020 2020 2020 2020 2020 2d20 6465 7374            - dest
-00000280: 696e 6174 696f 6e3a 2074 7a62 7463 5f6d  ination: tzbtc_m
-00000290: 6169 6e6e 6574 0a20 2020 2020 2020 2020  ainnet.         
-000002a0: 2020 2065 6e74 7279 706f 696e 743a 206d     entrypoint: m
-000002b0: 696e 740a 2020 2020 6669 7273 745f 6c65  int.    first_le
-000002c0: 7665 6c3a 2031 3336 3530 3030 0a20 2020  vel: 1365000.   
-000002d0: 206c 6173 745f 6c65 7665 6c3a 2031 3336   last_level: 136
-000002e0: 3630 3030 0a0a 6c6f 6767 696e 673a 2057  6000..logging: W
-000002f0: 4152 4e0a                                ARN.
+00000020: 746f 6b65 6e5f 7472 616e 7366 6572 730a  token_transfers.
+00000030: 0a63 6f6e 7472 6163 7473 3a0a 2020 747a  .contracts:.  tz
+00000040: 6274 635f 6d61 696e 6e65 743a 0a20 2020  btc_mainnet:.   
+00000050: 206b 696e 643a 2074 657a 6f73 0a20 2020   kind: tezos.   
+00000060: 2061 6464 7265 7373 3a20 4b54 3150 5778   address: KT1PWx
+00000070: 326d 6e44 7565 6f6f 6437 6645 6d66 6242  2mnDueood7fEmfbB
+00000080: 444b 7831 4439 4241 6e6e 5869 746e 0a20  DKx1D9BAnnXitn. 
+00000090: 2020 2074 7970 656e 616d 653a 2074 7a62     typename: tzb
+000000a0: 7463 0a0a 6461 7461 736f 7572 6365 733a  tc..datasources:
+000000b0: 0a20 2074 7a6b 743a 0a20 2020 206b 696e  .  tzkt:.    kin
+000000c0: 643a 2074 657a 6f73 2e74 7a6b 740a 2020  d: tezos.tzkt.  
+000000d0: 2020 7572 6c3a 2068 7474 7073 3a2f 2f61    url: https://a
+000000e0: 7069 2e74 7a6b 742e 696f 0a20 2020 2068  pi.tzkt.io.    h
+000000f0: 7474 703a 0a20 2020 2020 2072 6570 6c61  ttp:.      repla
+00000100: 795f 7061 7468 3a20 247b 4449 5044 5550  y_path: ${DIPDUP
+00000110: 5f52 4550 4c41 595f 5041 5448 3a2d 7d0a  _REPLAY_PATH:-}.
+00000120: 0a69 6e64 6578 6573 3a0a 2020 747a 6274  .indexes:.  tzbt
+00000130: 635f 686f 6c64 6572 735f 6d61 696e 6e65  c_holders_mainne
+00000140: 743a 0a20 2020 206b 696e 643a 2074 657a  t:.    kind: tez
+00000150: 6f73 2e74 7a6b 742e 746f 6b65 6e5f 7472  os.tzkt.token_tr
+00000160: 616e 7366 6572 730a 2020 2020 6461 7461  ansfers.    data
+00000170: 736f 7572 6365 3a20 747a 6b74 0a20 2020  source: tzkt.   
+00000180: 2068 616e 646c 6572 733a 0a20 2020 2020   handlers:.     
+00000190: 202d 2063 616c 6c62 6163 6b3a 206f 6e5f   - callback: on_
+000001a0: 746f 6b65 6e5f 7472 616e 7366 6572 0a20  token_transfer. 
+000001b0: 2020 2020 2020 2063 6f6e 7472 6163 743a         contract:
+000001c0: 2074 7a62 7463 5f6d 6169 6e6e 6574 0a20   tzbtc_mainnet. 
+000001d0: 2020 2066 6972 7374 5f6c 6576 656c 3a20     first_level: 
+000001e0: 3233 3135 3030 300a 2020 2020 6c61 7374  2315000.    last
+000001f0: 5f6c 6576 656c 3a20 3233 3135 3130 300a  _level: 2315100.
+00000200: 0a6c 6f67 6769 6e67 3a20 5741 524e 0a    .logging: WARN.
```

### Comparing `dipdup-7.0.0rc1/tests/configs/demo_token_transfers.yml` & `dipdup-7.0.0rc2/tests/configs/demo_token_transfers.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
 00000020: 746f 6b65 6e5f 7472 616e 7366 6572 730a  token_transfers.
-00000030: 0a64 6174 6162 6173 653a 0a20 206b 696e  .database:.  kin
-00000040: 643a 2073 716c 6974 650a 2020 7061 7468  d: sqlite.  path
-00000050: 3a20 6462 2e73 716c 6974 6533 0a0a 636f  : db.sqlite3..co
-00000060: 6e74 7261 6374 733a 0a20 2074 7a62 7463  ntracts:.  tzbtc
-00000070: 5f6d 6169 6e6e 6574 3a0a 2020 2020 6b69  _mainnet:.    ki
-00000080: 6e64 3a20 7465 7a6f 730a 2020 2020 6164  nd: tezos.    ad
-00000090: 6472 6573 733a 204b 5431 5057 7832 6d6e  dress: KT1PWx2mn
-000000a0: 4475 656f 6f64 3766 456d 6662 4244 4b78  Dueood7fEmfbBDKx
-000000b0: 3144 3942 416e 6e58 6974 6e0a 2020 2020  1D9BAnnXitn.    
-000000c0: 7479 7065 6e61 6d65 3a20 747a 6274 630a  typename: tzbtc.
-000000d0: 0a64 6174 6173 6f75 7263 6573 3a0a 2020  .datasources:.  
-000000e0: 747a 6b74 3a0a 2020 2020 6b69 6e64 3a20  tzkt:.    kind: 
-000000f0: 7465 7a6f 732e 747a 6b74 0a20 2020 2075  tezos.tzkt.    u
-00000100: 726c 3a20 6874 7470 733a 2f2f 6170 692e  rl: https://api.
-00000110: 747a 6b74 2e69 6f0a 2020 2020 6874 7470  tzkt.io.    http
-00000120: 3a0a 2020 2020 2020 7265 706c 6179 5f70  :.      replay_p
-00000130: 6174 683a 2024 7b44 4950 4455 505f 5245  ath: ${DIPDUP_RE
-00000140: 504c 4159 5f50 4154 483a 2d7d 0a0a 696e  PLAY_PATH:-}..in
-00000150: 6465 7865 733a 0a20 2074 7a62 7463 5f68  dexes:.  tzbtc_h
-00000160: 6f6c 6465 7273 5f6d 6169 6e6e 6574 3a0a  olders_mainnet:.
-00000170: 2020 2020 6b69 6e64 3a20 7465 7a6f 732e      kind: tezos.
-00000180: 747a 6b74 2e74 6f6b 656e 5f74 7261 6e73  tzkt.token_trans
-00000190: 6665 7273 0a20 2020 2064 6174 6173 6f75  fers.    datasou
-000001a0: 7263 653a 2074 7a6b 740a 2020 2020 6861  rce: tzkt.    ha
-000001b0: 6e64 6c65 7273 3a0a 2020 2020 2020 2d20  ndlers:.      - 
-000001c0: 6361 6c6c 6261 636b 3a20 6f6e 5f74 6f6b  callback: on_tok
-000001d0: 656e 5f74 7261 6e73 6665 720a 2020 2020  en_transfer.    
-000001e0: 2020 2020 636f 6e74 7261 6374 3a20 747a      contract: tz
-000001f0: 6274 635f 6d61 696e 6e65 740a 2020 2020  btc_mainnet.    
-00000200: 6669 7273 745f 6c65 7665 6c3a 2031 3336  first_level: 136
-00000210: 3439 3939 0a20 2020 206c 6173 745f 6c65  4999.    last_le
-00000220: 7665 6c3a 2031 3336 3630 3030 0a0a 6c6f  vel: 1366000..lo
-00000230: 6767 696e 673a 2057 4152 4e0a            gging: WARN.
+00000030: 0a63 6f6e 7472 6163 7473 3a0a 2020 747a  .contracts:.  tz
+00000040: 6274 635f 6d61 696e 6e65 743a 0a20 2020  btc_mainnet:.   
+00000050: 206b 696e 643a 2074 657a 6f73 0a20 2020   kind: tezos.   
+00000060: 2061 6464 7265 7373 3a20 4b54 3150 5778   address: KT1PWx
+00000070: 326d 6e44 7565 6f6f 6437 6645 6d66 6242  2mnDueood7fEmfbB
+00000080: 444b 7831 4439 4241 6e6e 5869 746e 0a20  DKx1D9BAnnXitn. 
+00000090: 2020 2074 7970 656e 616d 653a 2074 7a62     typename: tzb
+000000a0: 7463 0a0a 6461 7461 736f 7572 6365 733a  tc..datasources:
+000000b0: 0a20 2074 7a6b 743a 0a20 2020 206b 696e  .  tzkt:.    kin
+000000c0: 643a 2074 657a 6f73 2e74 7a6b 740a 2020  d: tezos.tzkt.  
+000000d0: 2020 7572 6c3a 2068 7474 7073 3a2f 2f61    url: https://a
+000000e0: 7069 2e74 7a6b 742e 696f 0a20 2020 2068  pi.tzkt.io.    h
+000000f0: 7474 703a 0a20 2020 2020 2072 6570 6c61  ttp:.      repla
+00000100: 795f 7061 7468 3a20 247b 4449 5044 5550  y_path: ${DIPDUP
+00000110: 5f52 4550 4c41 595f 5041 5448 3a2d 7d0a  _REPLAY_PATH:-}.
+00000120: 0a69 6e64 6578 6573 3a0a 2020 747a 6274  .indexes:.  tzbt
+00000130: 635f 686f 6c64 6572 735f 6d61 696e 6e65  c_holders_mainne
+00000140: 743a 0a20 2020 206b 696e 643a 2074 657a  t:.    kind: tez
+00000150: 6f73 2e74 7a6b 742e 746f 6b65 6e5f 7472  os.tzkt.token_tr
+00000160: 616e 7366 6572 730a 2020 2020 6461 7461  ansfers.    data
+00000170: 736f 7572 6365 3a20 747a 6b74 0a20 2020  source: tzkt.   
+00000180: 2068 616e 646c 6572 733a 0a20 2020 2020   handlers:.     
+00000190: 202d 2063 616c 6c62 6163 6b3a 206f 6e5f   - callback: on_
+000001a0: 746f 6b65 6e5f 7472 616e 7366 6572 0a20  token_transfer. 
+000001b0: 2020 2020 2020 2063 6f6e 7472 6163 743a         contract:
+000001c0: 2074 7a62 7463 5f6d 6169 6e6e 6574 0a20   tzbtc_mainnet. 
+000001d0: 2020 2066 6972 7374 5f6c 6576 656c 3a20     first_level: 
+000001e0: 3133 3634 3939 390a 2020 2020 6c61 7374  1364999.    last
+000001f0: 5f6c 6576 656c 3a20 3133 3636 3030 300a  _level: 1366000.
+00000200: 0a6c 6f67 6769 6e67 3a20 5741 524e 0a    .logging: WARN.
```

### Comparing `dipdup-7.0.0rc1/tests/configs/demo_token_transfers_2.yml` & `dipdup-7.0.0rc2/tests/configs/demo_token_transfers_4.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,51 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
 00000020: 746f 6b65 6e5f 7472 616e 7366 6572 730a  token_transfers.
-00000030: 0a64 6174 6162 6173 653a 0a20 206b 696e  .database:.  kin
-00000040: 643a 2073 716c 6974 650a 2020 7061 7468  d: sqlite.  path
-00000050: 3a20 6462 2e73 716c 6974 6533 0a0a 636f  : db.sqlite3..co
-00000060: 6e74 7261 6374 733a 0a20 2074 7a62 7463  ntracts:.  tzbtc
-00000070: 5f6d 6169 6e6e 6574 3a0a 2020 2020 6b69  _mainnet:.    ki
-00000080: 6e64 3a20 7465 7a6f 730a 2020 2020 6164  nd: tezos.    ad
-00000090: 6472 6573 733a 204b 5431 5057 7832 6d6e  dress: KT1PWx2mn
-000000a0: 4475 656f 6f64 3766 456d 6662 4244 4b78  Dueood7fEmfbBDKx
-000000b0: 3144 3942 416e 6e58 6974 6e0a 2020 2020  1D9BAnnXitn.    
-000000c0: 7479 7065 6e61 6d65 3a20 747a 6274 630a  typename: tzbtc.
-000000d0: 0a64 6174 6173 6f75 7263 6573 3a0a 2020  .datasources:.  
-000000e0: 747a 6b74 3a0a 2020 2020 6b69 6e64 3a20  tzkt:.    kind: 
-000000f0: 7465 7a6f 732e 747a 6b74 0a20 2020 2075  tezos.tzkt.    u
-00000100: 726c 3a20 6874 7470 733a 2f2f 6170 692e  rl: https://api.
-00000110: 747a 6b74 2e69 6f0a 2020 2020 6874 7470  tzkt.io.    http
-00000120: 3a0a 2020 2020 2020 7265 706c 6179 5f70  :.      replay_p
-00000130: 6174 683a 2024 7b44 4950 4455 505f 5245  ath: ${DIPDUP_RE
-00000140: 504c 4159 5f50 4154 483a 2d7d 0a0a 696e  PLAY_PATH:-}..in
-00000150: 6465 7865 733a 0a20 2074 7a62 7463 5f68  dexes:.  tzbtc_h
-00000160: 6f6c 6465 7273 5f6d 6169 6e6e 6574 3a0a  olders_mainnet:.
-00000170: 2020 2020 6b69 6e64 3a20 7465 7a6f 732e      kind: tezos.
-00000180: 747a 6b74 2e74 6f6b 656e 5f74 7261 6e73  tzkt.token_trans
-00000190: 6665 7273 0a20 2020 2064 6174 6173 6f75  fers.    datasou
-000001a0: 7263 653a 2074 7a6b 740a 2020 2020 6861  rce: tzkt.    ha
-000001b0: 6e64 6c65 7273 3a0a 2020 2020 2020 2d20  ndlers:.      - 
-000001c0: 6361 6c6c 6261 636b 3a20 6f6e 5f74 6f6b  callback: on_tok
-000001d0: 656e 5f74 7261 6e73 6665 720a 2020 2020  en_transfer.    
-000001e0: 2020 2020 636f 6e74 7261 6374 3a20 747a      contract: tz
-000001f0: 6274 635f 6d61 696e 6e65 740a 2020 2020  btc_mainnet.    
-00000200: 6669 7273 745f 6c65 7665 6c3a 2031 3336  first_level: 136
-00000210: 3638 3234 0a20 2020 206c 6173 745f 6c65  6824.    last_le
-00000220: 7665 6c3a 2031 3336 3639 3939 0a0a 6c6f  vel: 1366999..lo
-00000230: 6767 696e 673a 2057 4152 4e0a            gging: WARN.
+00000030: 0a63 6f6e 7472 6163 7473 3a0a 2020 747a  .contracts:.  tz
+00000040: 6274 635f 6d61 696e 6e65 743a 0a20 2020  btc_mainnet:.   
+00000050: 206b 696e 643a 2074 657a 6f73 0a20 2020   kind: tezos.   
+00000060: 2061 6464 7265 7373 3a20 4b54 3150 5778   address: KT1PWx
+00000070: 326d 6e44 7565 6f6f 6437 6645 6d66 6242  2mnDueood7fEmfbB
+00000080: 444b 7831 4439 4241 6e6e 5869 746e 0a20  DKx1D9BAnnXitn. 
+00000090: 2020 2074 7970 656e 616d 653a 2074 7a62     typename: tzb
+000000a0: 7463 0a20 2074 7a62 7463 5f68 6f6c 6465  tc.  tzbtc_holde
+000000b0: 725f 6d61 696e 6e65 743a 0a20 2020 206b  r_mainnet:.    k
+000000c0: 696e 643a 2074 657a 6f73 0a20 2020 2061  ind: tezos.    a
+000000d0: 6464 7265 7373 3a20 747a 3155 6237 7636  ddress: tz1Ub7v6
+000000e0: 656f 6563 364b 6442 3556 5443 7174 4145  eoec6KdB5VTCqtAE
+000000f0: 5672 5173 6a6a 315a 5446 546b 0a0a 6461  VrQsjj1ZTFTk..da
+00000100: 7461 736f 7572 6365 733a 0a20 2074 7a6b  tasources:.  tzk
+00000110: 743a 0a20 2020 206b 696e 643a 2074 657a  t:.    kind: tez
+00000120: 6f73 2e74 7a6b 740a 2020 2020 7572 6c3a  os.tzkt.    url:
+00000130: 2068 7474 7073 3a2f 2f61 7069 2e74 7a6b   https://api.tzk
+00000140: 742e 696f 0a20 2020 2068 7474 703a 0a20  t.io.    http:. 
+00000150: 2020 2020 2072 6570 6c61 795f 7061 7468       replay_path
+00000160: 3a20 247b 4449 5044 5550 5f52 4550 4c41  : ${DIPDUP_REPLA
+00000170: 595f 5041 5448 3a2d 7d0a 0a69 6e64 6578  Y_PATH:-}..index
+00000180: 6573 3a0a 2020 747a 6274 635f 686f 6c64  es:.  tzbtc_hold
+00000190: 6572 735f 6d61 696e 6e65 743a 0a20 2020  ers_mainnet:.   
+000001a0: 206b 696e 643a 2074 657a 6f73 2e74 7a6b   kind: tezos.tzk
+000001b0: 742e 746f 6b65 6e5f 7472 616e 7366 6572  t.token_transfer
+000001c0: 730a 2020 2020 6461 7461 736f 7572 6365  s.    datasource
+000001d0: 3a20 747a 6b74 0a20 2020 2068 616e 646c  : tzkt.    handl
+000001e0: 6572 733a 0a20 2020 2020 202d 2063 616c  ers:.      - cal
+000001f0: 6c62 6163 6b3a 206f 6e5f 746f 6b65 6e5f  lback: on_token_
+00000200: 7472 616e 7366 6572 0a20 2020 2020 2020  transfer.       
+00000210: 2063 6f6e 7472 6163 743a 2074 7a62 7463   contract: tzbtc
+00000220: 5f6d 6169 6e6e 6574 0a20 2020 2020 202d  _mainnet.      -
+00000230: 2063 616c 6c62 6163 6b3a 206f 6e5f 746f   callback: on_to
+00000240: 6b65 6e5f 7472 616e 7366 6572 0a20 2020  ken_transfer.   
+00000250: 2020 2020 2066 726f 6d3a 2074 7a62 7463       from: tzbtc
+00000260: 5f6d 6169 6e6e 6574 0a20 2020 2020 202d  _mainnet.      -
+00000270: 2063 616c 6c62 6163 6b3a 206f 6e5f 746f   callback: on_to
+00000280: 6b65 6e5f 7472 616e 7366 6572 0a20 2020  ken_transfer.   
+00000290: 2020 2020 2074 6f3a 2074 7a62 7463 5f68       to: tzbtc_h
+000002a0: 6f6c 6465 725f 6d61 696e 6e65 740a 2020  older_mainnet.  
+000002b0: 2020 2320 7365 653a 2068 7474 7073 3a2f    # see: https:/
+000002c0: 2f61 7069 2e74 7a6b 742e 696f 2f76 312f  /api.tzkt.io/v1/
+000002d0: 746f 6b65 6e73 2f74 7261 6e73 6665 7273  tokens/transfers
+000002e0: 3f69 643d 3132 3530 3639 3131 390a 2020  ?id=125069119.  
+000002f0: 2020 6669 7273 745f 6c65 7665 6c3a 2031    first_level: 1
+00000300: 3336 3638 3430 0a20 2020 206c 6173 745f  366840.    last_
+00000310: 6c65 7665 6c3a 2031 3336 3638 3430 0a0a  level: 1366840..
+00000320: 6c6f 6767 696e 673a 2057 4152 4e0a       logging: WARN.
```

### Comparing `dipdup-7.0.0rc1/tests/configs/demo_token_transfers_4.yml` & `dipdup-7.0.0rc2/tests/configs/demo_token_transfers_2.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,33 @@
 00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
 00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
 00000020: 746f 6b65 6e5f 7472 616e 7366 6572 730a  token_transfers.
-00000030: 0a64 6174 6162 6173 653a 0a20 206b 696e  .database:.  kin
-00000040: 643a 2073 716c 6974 650a 2020 7061 7468  d: sqlite.  path
-00000050: 3a20 6462 2e73 716c 6974 6533 0a0a 636f  : db.sqlite3..co
-00000060: 6e74 7261 6374 733a 0a20 2074 7a62 7463  ntracts:.  tzbtc
-00000070: 5f6d 6169 6e6e 6574 3a0a 2020 2020 6b69  _mainnet:.    ki
-00000080: 6e64 3a20 7465 7a6f 730a 2020 2020 6164  nd: tezos.    ad
-00000090: 6472 6573 733a 204b 5431 5057 7832 6d6e  dress: KT1PWx2mn
-000000a0: 4475 656f 6f64 3766 456d 6662 4244 4b78  Dueood7fEmfbBDKx
-000000b0: 3144 3942 416e 6e58 6974 6e0a 2020 2020  1D9BAnnXitn.    
-000000c0: 7479 7065 6e61 6d65 3a20 747a 6274 630a  typename: tzbtc.
-000000d0: 2020 747a 6274 635f 686f 6c64 6572 5f6d    tzbtc_holder_m
-000000e0: 6169 6e6e 6574 3a0a 2020 2020 6b69 6e64  ainnet:.    kind
-000000f0: 3a20 7465 7a6f 730a 2020 2020 6164 6472  : tezos.    addr
-00000100: 6573 733a 2074 7a31 5562 3776 3665 6f65  ess: tz1Ub7v6eoe
-00000110: 6336 4b64 4235 5654 4371 7441 4556 7251  c6KdB5VTCqtAEVrQ
-00000120: 736a 6a31 5a54 4654 6b0a 0a64 6174 6173  sjj1ZTFTk..datas
-00000130: 6f75 7263 6573 3a0a 2020 747a 6b74 3a0a  ources:.  tzkt:.
-00000140: 2020 2020 6b69 6e64 3a20 7465 7a6f 732e      kind: tezos.
-00000150: 747a 6b74 0a20 2020 2075 726c 3a20 6874  tzkt.    url: ht
-00000160: 7470 733a 2f2f 6170 692e 747a 6b74 2e69  tps://api.tzkt.i
-00000170: 6f0a 2020 2020 6874 7470 3a0a 2020 2020  o.    http:.    
-00000180: 2020 7265 706c 6179 5f70 6174 683a 2024    replay_path: $
-00000190: 7b44 4950 4455 505f 5245 504c 4159 5f50  {DIPDUP_REPLAY_P
-000001a0: 4154 483a 2d7d 0a0a 696e 6465 7865 733a  ATH:-}..indexes:
-000001b0: 0a20 2074 7a62 7463 5f68 6f6c 6465 7273  .  tzbtc_holders
-000001c0: 5f6d 6169 6e6e 6574 3a0a 2020 2020 6b69  _mainnet:.    ki
-000001d0: 6e64 3a20 7465 7a6f 732e 747a 6b74 2e74  nd: tezos.tzkt.t
-000001e0: 6f6b 656e 5f74 7261 6e73 6665 7273 0a20  oken_transfers. 
-000001f0: 2020 2064 6174 6173 6f75 7263 653a 2074     datasource: t
-00000200: 7a6b 740a 2020 2020 6861 6e64 6c65 7273  zkt.    handlers
-00000210: 3a0a 2020 2020 2020 2d20 6361 6c6c 6261  :.      - callba
-00000220: 636b 3a20 6f6e 5f74 6f6b 656e 5f74 7261  ck: on_token_tra
-00000230: 6e73 6665 720a 2020 2020 2020 2020 636f  nsfer.        co
-00000240: 6e74 7261 6374 3a20 747a 6274 635f 6d61  ntract: tzbtc_ma
-00000250: 696e 6e65 740a 2020 2020 2020 2d20 6361  innet.      - ca
-00000260: 6c6c 6261 636b 3a20 6f6e 5f74 6f6b 656e  llback: on_token
-00000270: 5f74 7261 6e73 6665 720a 2020 2020 2020  _transfer.      
-00000280: 2020 6672 6f6d 3a20 747a 6274 635f 6d61    from: tzbtc_ma
-00000290: 696e 6e65 740a 2020 2020 2020 2d20 6361  innet.      - ca
-000002a0: 6c6c 6261 636b 3a20 6f6e 5f74 6f6b 656e  llback: on_token
-000002b0: 5f74 7261 6e73 6665 720a 2020 2020 2020  _transfer.      
-000002c0: 2020 746f 3a20 747a 6274 635f 686f 6c64    to: tzbtc_hold
-000002d0: 6572 5f6d 6169 6e6e 6574 0a20 2020 2023  er_mainnet.    #
-000002e0: 2073 6565 3a20 6874 7470 733a 2f2f 6170   see: https://ap
-000002f0: 692e 747a 6b74 2e69 6f2f 7631 2f74 6f6b  i.tzkt.io/v1/tok
-00000300: 656e 732f 7472 616e 7366 6572 733f 6964  ens/transfers?id
-00000310: 3d31 3235 3036 3931 3139 0a20 2020 2066  =125069119.    f
-00000320: 6972 7374 5f6c 6576 656c 3a20 3133 3636  irst_level: 1366
-00000330: 3834 300a 2020 2020 6c61 7374 5f6c 6576  840.    last_lev
-00000340: 656c 3a20 3133 3636 3834 300a 0a6c 6f67  el: 1366840..log
-00000350: 6769 6e67 3a20 5741 524e 0a              ging: WARN.
+00000030: 0a63 6f6e 7472 6163 7473 3a0a 2020 747a  .contracts:.  tz
+00000040: 6274 635f 6d61 696e 6e65 743a 0a20 2020  btc_mainnet:.   
+00000050: 206b 696e 643a 2074 657a 6f73 0a20 2020   kind: tezos.   
+00000060: 2061 6464 7265 7373 3a20 4b54 3150 5778   address: KT1PWx
+00000070: 326d 6e44 7565 6f6f 6437 6645 6d66 6242  2mnDueood7fEmfbB
+00000080: 444b 7831 4439 4241 6e6e 5869 746e 0a20  DKx1D9BAnnXitn. 
+00000090: 2020 2074 7970 656e 616d 653a 2074 7a62     typename: tzb
+000000a0: 7463 0a0a 6461 7461 736f 7572 6365 733a  tc..datasources:
+000000b0: 0a20 2074 7a6b 743a 0a20 2020 206b 696e  .  tzkt:.    kin
+000000c0: 643a 2074 657a 6f73 2e74 7a6b 740a 2020  d: tezos.tzkt.  
+000000d0: 2020 7572 6c3a 2068 7474 7073 3a2f 2f61    url: https://a
+000000e0: 7069 2e74 7a6b 742e 696f 0a20 2020 2068  pi.tzkt.io.    h
+000000f0: 7474 703a 0a20 2020 2020 2072 6570 6c61  ttp:.      repla
+00000100: 795f 7061 7468 3a20 247b 4449 5044 5550  y_path: ${DIPDUP
+00000110: 5f52 4550 4c41 595f 5041 5448 3a2d 7d0a  _REPLAY_PATH:-}.
+00000120: 0a69 6e64 6578 6573 3a0a 2020 747a 6274  .indexes:.  tzbt
+00000130: 635f 686f 6c64 6572 735f 6d61 696e 6e65  c_holders_mainne
+00000140: 743a 0a20 2020 206b 696e 643a 2074 657a  t:.    kind: tez
+00000150: 6f73 2e74 7a6b 742e 746f 6b65 6e5f 7472  os.tzkt.token_tr
+00000160: 616e 7366 6572 730a 2020 2020 6461 7461  ansfers.    data
+00000170: 736f 7572 6365 3a20 747a 6b74 0a20 2020  source: tzkt.   
+00000180: 2068 616e 646c 6572 733a 0a20 2020 2020   handlers:.     
+00000190: 202d 2063 616c 6c62 6163 6b3a 206f 6e5f   - callback: on_
+000001a0: 746f 6b65 6e5f 7472 616e 7366 6572 0a20  token_transfer. 
+000001b0: 2020 2020 2020 2063 6f6e 7472 6163 743a         contract:
+000001c0: 2074 7a62 7463 5f6d 6169 6e6e 6574 0a20   tzbtc_mainnet. 
+000001d0: 2020 2066 6972 7374 5f6c 6576 656c 3a20     first_level: 
+000001e0: 3133 3636 3832 340a 2020 2020 6c61 7374  1366824.    last
+000001f0: 5f6c 6576 656c 3a20 3133 3636 3939 390a  _level: 1366999.
+00000200: 0a6c 6f67 6769 6e67 3a20 5741 524e 0a    .logging: WARN.
```

### Comparing `dipdup-7.0.0rc1/tests/configs/hen_subjkt.yml` & `dipdup-7.0.0rc2/tests/configs/hen_subjkt.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/configs/kolibri_ovens.yml` & `dipdup-7.0.0rc2/tests/configs/kolibri_ovens.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/configs/operation_filters.yml` & `dipdup-7.0.0rc2/tests/configs/operation_filters.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/configs/yupana.yml` & `dipdup-7.0.0rc2/tests/configs/yupana.yml`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/profile_abi_decoding.py` & `dipdup-7.0.0rc2/tests/profile_abi_decoding.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/0535b2dcc93076e6026fa48cc501adaed47b7b060e6483d8312f40c184d7287d` & `dipdup-7.0.0rc2/tests/replays/0535b2dcc93076e6026fa48cc501adaed47b7b060e6483d8312f40c184d7287d`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/064e788d2566d748f516b17c6a43ab34259443cc9537f0dec7c1a5a2bce704b2` & `dipdup-7.0.0rc2/tests/replays/064e788d2566d748f516b17c6a43ab34259443cc9537f0dec7c1a5a2bce704b2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/0eaaba2830dbdd3a80286fbc367084bce6e55c678e21da178a7eb16beef6c997` & `dipdup-7.0.0rc2/tests/replays/0eaaba2830dbdd3a80286fbc367084bce6e55c678e21da178a7eb16beef6c997`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/1228b36594bb93d619170ad49373f1ceec52d10faafdd727b37f3cdeffd663db` & `dipdup-7.0.0rc2/tests/replays/1228b36594bb93d619170ad49373f1ceec52d10faafdd727b37f3cdeffd663db`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/13afdf001ce3d6a0219c0f7f6d372d9b645770e5f4304576f7f7a37b45af96fc` & `dipdup-7.0.0rc2/tests/replays/13afdf001ce3d6a0219c0f7f6d372d9b645770e5f4304576f7f7a37b45af96fc`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/14408f393a3e399b241184f858e70396e3b8313e32ee1a984913d43fb74dcfec` & `dipdup-7.0.0rc2/tests/replays/14408f393a3e399b241184f858e70396e3b8313e32ee1a984913d43fb74dcfec`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/14cba0424c66b1869edc8e18ca3079856083cc3db7e68ef61fce165b6d7e1a6d` & `dipdup-7.0.0rc2/tests/replays/14cba0424c66b1869edc8e18ca3079856083cc3db7e68ef61fce165b6d7e1a6d`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/18d85ceab66daf057861b99b7e223a25067197b3b77edbf060390df58cb65eaa` & `dipdup-7.0.0rc2/tests/replays/18d85ceab66daf057861b99b7e223a25067197b3b77edbf060390df58cb65eaa`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/19441b677ef5fd8ca39c37e6ddd2a7d9bc8cb3ab282b2a91ce4d8430f56f0fa9` & `dipdup-7.0.0rc2/tests/replays/19441b677ef5fd8ca39c37e6ddd2a7d9bc8cb3ab282b2a91ce4d8430f56f0fa9`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/1a43bd7d1397cc3169ad267cd2ef083a5a63eaac7ed5186aadfc01bb53636214` & `dipdup-7.0.0rc2/tests/replays/1a43bd7d1397cc3169ad267cd2ef083a5a63eaac7ed5186aadfc01bb53636214`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/1c07d3d72acc637fb46c59d0a6dc9749f3412a5d527ca2eb0cccc01720fda1c7` & `dipdup-7.0.0rc2/tests/replays/1c07d3d72acc637fb46c59d0a6dc9749f3412a5d527ca2eb0cccc01720fda1c7`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/1c34d1f810ae474395893bf67fb8cfb27b0506ab94eebec42cd4d2d21bf3dfcd` & `dipdup-7.0.0rc2/tests/replays/1c34d1f810ae474395893bf67fb8cfb27b0506ab94eebec42cd4d2d21bf3dfcd`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/252fd058cfef21f9b5b7f4367f730ec7d41647253d7cc7ccfb1e22d42d1f366a` & `dipdup-7.0.0rc2/tests/replays/252fd058cfef21f9b5b7f4367f730ec7d41647253d7cc7ccfb1e22d42d1f366a`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/27373c23411bf37b605c8d0ead9a0e6c6c1f1718ce7863b095b759811e44e155` & `dipdup-7.0.0rc2/tests/replays/27373c23411bf37b605c8d0ead9a0e6c6c1f1718ce7863b095b759811e44e155`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/2a45ec6372b45e46199a6af24272cb93586777a0522cd1203b3eeef213ce4583` & `dipdup-7.0.0rc2/tests/replays/2a45ec6372b45e46199a6af24272cb93586777a0522cd1203b3eeef213ce4583`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/31cc70e13495f58ecde80847bc6c9e08536cc426c03bd2aa8c45c1b2c798e155` & `dipdup-7.0.0rc2/tests/replays/31cc70e13495f58ecde80847bc6c9e08536cc426c03bd2aa8c45c1b2c798e155`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/31dd376b771f347a0d6fe4dd132a1f96f809274429b78ec86dd742e5589fbc23` & `dipdup-7.0.0rc2/tests/replays/31dd376b771f347a0d6fe4dd132a1f96f809274429b78ec86dd742e5589fbc23`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/32e3a13cc470d8720ce28f5eaff327340fb25cbe712e5b5a348af1bc3c92235a` & `dipdup-7.0.0rc2/tests/replays/32e3a13cc470d8720ce28f5eaff327340fb25cbe712e5b5a348af1bc3c92235a`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/36072e13c9ce265bb81142b8816da8c31bd9180e7c663ea4169bd259af107382` & `dipdup-7.0.0rc2/tests/replays/36072e13c9ce265bb81142b8816da8c31bd9180e7c663ea4169bd259af107382`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/377ac31d6316391ed138df44bec374d65202f0577603e80465ced3c09140f78c` & `dipdup-7.0.0rc2/tests/replays/377ac31d6316391ed138df44bec374d65202f0577603e80465ced3c09140f78c`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/383899084f79460e96fd311bb64e4925738c486b39d6281539456c5fcac41620` & `dipdup-7.0.0rc2/tests/replays/383899084f79460e96fd311bb64e4925738c486b39d6281539456c5fcac41620`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/39b8664d1bca5d374ff905c8a3a396b53d19ee469dc37545a8ca6b080bd0e9e0` & `dipdup-7.0.0rc2/tests/replays/39b8664d1bca5d374ff905c8a3a396b53d19ee469dc37545a8ca6b080bd0e9e0`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/3a2bd8b6b72bf18152d2550c106789fa9b8abc98ea9d759a6597b7ebfbab0fc2` & `dipdup-7.0.0rc2/tests/replays/3a2bd8b6b72bf18152d2550c106789fa9b8abc98ea9d759a6597b7ebfbab0fc2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/3c9ad6f98f79e72185ea58c4777115750c658c5defd616664212095bd440c10c` & `dipdup-7.0.0rc2/tests/replays/3c9ad6f98f79e72185ea58c4777115750c658c5defd616664212095bd440c10c`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/42b7bf0da866257ef98e1f7124d2d21fe7d13228c076fffa32331da423f36933` & `dipdup-7.0.0rc2/tests/replays/42b7bf0da866257ef98e1f7124d2d21fe7d13228c076fffa32331da423f36933`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/43cb0ab415d8b8b3f7addc3e82ea27d93b2c66ff55c117e1e0c7c64a0fcfc3f2` & `dipdup-7.0.0rc2/tests/replays/43cb0ab415d8b8b3f7addc3e82ea27d93b2c66ff55c117e1e0c7c64a0fcfc3f2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/440173d32e95111ca7b080ccc4dc09bfab23c8361919b2c113f0ff9ab445eec2` & `dipdup-7.0.0rc2/tests/replays/440173d32e95111ca7b080ccc4dc09bfab23c8361919b2c113f0ff9ab445eec2`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/489233ce9373f7de4f7a9053055c74bc0df999bfe939ed67d98b6d67e676e35a` & `dipdup-7.0.0rc2/tests/replays/489233ce9373f7de4f7a9053055c74bc0df999bfe939ed67d98b6d67e676e35a`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/4a57776d93475adfd9c49b6c3295a7cedfc23b73733a1fb5f0c985ee039dc5dc` & `dipdup-7.0.0rc2/tests/replays/4a57776d93475adfd9c49b6c3295a7cedfc23b73733a1fb5f0c985ee039dc5dc`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/4aa7f9b0657be0c44baf2caed8c7cb08d02097a4095cf6417f78cba3a25e8423` & `dipdup-7.0.0rc2/tests/replays/4aa7f9b0657be0c44baf2caed8c7cb08d02097a4095cf6417f78cba3a25e8423`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/5483a0e11009e0f186bf70c214e2597d267a75a1e19152a9e7ed1ec257ce88ca` & `dipdup-7.0.0rc2/tests/replays/5483a0e11009e0f186bf70c214e2597d267a75a1e19152a9e7ed1ec257ce88ca`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/587613799ebfae42b1884016d1a44a452d68e70e3ed80641d90b8e7657ba8ee5` & `dipdup-7.0.0rc2/tests/replays/587613799ebfae42b1884016d1a44a452d68e70e3ed80641d90b8e7657ba8ee5`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/5b7c31b4b73bc57e8296e6051b3bc7b2302b32588d8fbcafce8a66de3be743df` & `dipdup-7.0.0rc2/tests/replays/5b7c31b4b73bc57e8296e6051b3bc7b2302b32588d8fbcafce8a66de3be743df`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/5b99bc4beb6a9a33f7d2f118426458e4c788e0ab6d9e51949d3ccbf8b4003fc1` & `dipdup-7.0.0rc2/tests/replays/5b99bc4beb6a9a33f7d2f118426458e4c788e0ab6d9e51949d3ccbf8b4003fc1`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/5d21060ba8e78279d2d1edaa2f266ecf36105eaccef5ebed15748441651f76fd` & `dipdup-7.0.0rc2/tests/replays/5d21060ba8e78279d2d1edaa2f266ecf36105eaccef5ebed15748441651f76fd`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/6cc8d741a41b76983cd7e0f63e8f22a4c67cd946888f45a5b7ead8c3bb5ad2f1` & `dipdup-7.0.0rc2/tests/replays/6cc8d741a41b76983cd7e0f63e8f22a4c67cd946888f45a5b7ead8c3bb5ad2f1`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/6cff8d120db8fd3926a45714ce7f1d0560803eb5a7b4a413b64fee1b7fd7a8ff` & `dipdup-7.0.0rc2/tests/replays/6cff8d120db8fd3926a45714ce7f1d0560803eb5a7b4a413b64fee1b7fd7a8ff`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/6d76a3c3f427ff534c551de1793cb1d1dfbd22ccad97f5917a9f9b201a3f9804` & `dipdup-7.0.0rc2/tests/replays/6d76a3c3f427ff534c551de1793cb1d1dfbd22ccad97f5917a9f9b201a3f9804`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/7669ea717d9759748aed86302326b79be5157a1a36d13b39b00f06bcbe22b309` & `dipdup-7.0.0rc2/tests/replays/7669ea717d9759748aed86302326b79be5157a1a36d13b39b00f06bcbe22b309`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/76d49ae3b723376c88ca65a3080a273e098d226932a1a49c38fbc4421e7c2e64` & `dipdup-7.0.0rc2/tests/replays/76d49ae3b723376c88ca65a3080a273e098d226932a1a49c38fbc4421e7c2e64`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/7b6cf9b8c69712bf26ed09059352ec740606969bf20eab0dedda870273f4fde9` & `dipdup-7.0.0rc2/tests/replays/7b6cf9b8c69712bf26ed09059352ec740606969bf20eab0dedda870273f4fde9`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/7b9c78209f98b2c3a6678ed224fa686eee25c3c63dddd7f9af77c734b0dfabb8` & `dipdup-7.0.0rc2/tests/replays/7b9c78209f98b2c3a6678ed224fa686eee25c3c63dddd7f9af77c734b0dfabb8`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/7d4a99edf5845445bbeb894ad34b063c985ca061ffed162093721c0032210e31` & `dipdup-7.0.0rc2/tests/replays/136157c421184c218127595797f5fe0b774e2807f6f4605a1d1944a1738e2d6d`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/803e05a8d0bb9e7cfb49530271d43ea62111b6419e7cded2d221f7e0e0c92ece` & `dipdup-7.0.0rc2/tests/replays/803e05a8d0bb9e7cfb49530271d43ea62111b6419e7cded2d221f7e0e0c92ece`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/80921fd33043def891912a6ad57d76664399564fd813950eb11f4a0e69e3e28f` & `dipdup-7.0.0rc2/tests/replays/80921fd33043def891912a6ad57d76664399564fd813950eb11f4a0e69e3e28f`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/816d08f71c84537ea8df05a40678b1addca15bf3a73c0e927c75d9f9c0f2d418` & `dipdup-7.0.0rc2/tests/replays/816d08f71c84537ea8df05a40678b1addca15bf3a73c0e927c75d9f9c0f2d418`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/84cf46aa9c8dbd3ca6c3d946c749713e6c70a6a20d9cc69b4156235fd099b2e3` & `dipdup-7.0.0rc2/tests/replays/84cf46aa9c8dbd3ca6c3d946c749713e6c70a6a20d9cc69b4156235fd099b2e3`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/93516225810a23a6799f2f9a1dee055ca79a66ee2b8d0f32be820c9c385e936b` & `dipdup-7.0.0rc2/tests/replays/93516225810a23a6799f2f9a1dee055ca79a66ee2b8d0f32be820c9c385e936b`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/9e6e907842da2cd494c558ea5ecc211fd12e56bfc547450978fb7dfe03853e58` & `dipdup-7.0.0rc2/tests/replays/9e6e907842da2cd494c558ea5ecc211fd12e56bfc547450978fb7dfe03853e58`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/a3ce91a1b0d505cc221f0e201781466ba1e2d6dc7b624b9bc75a03ce3dbb0f92` & `dipdup-7.0.0rc2/tests/replays/a3ce91a1b0d505cc221f0e201781466ba1e2d6dc7b624b9bc75a03ce3dbb0f92`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/a795ef429bde71b3ba66b545c0048f57a78ab5d2247772761d8efe86567199b9` & `dipdup-7.0.0rc2/tests/replays/a795ef429bde71b3ba66b545c0048f57a78ab5d2247772761d8efe86567199b9`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/aa8fe6037996b296bf9a3011e45cd9ecb92fb728592a843f91b03b2848cb1fb1` & `dipdup-7.0.0rc2/tests/replays/aa8fe6037996b296bf9a3011e45cd9ecb92fb728592a843f91b03b2848cb1fb1`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/acc952ba1905717315212f952ed689d7b8f683165b31c0a7a25199aed9fda27f` & `dipdup-7.0.0rc2/tests/replays/acc952ba1905717315212f952ed689d7b8f683165b31c0a7a25199aed9fda27f`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/b3af887f7ad8172af75b94a09bedfb9ae1e14f8819a36d6ce9f709721068263b` & `dipdup-7.0.0rc2/tests/replays/b3af887f7ad8172af75b94a09bedfb9ae1e14f8819a36d6ce9f709721068263b`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/b49fb33ee80345b70414ad08806a860e2139c20d98a5150c6ccd1b28a90f311e` & `dipdup-7.0.0rc2/tests/replays/b49fb33ee80345b70414ad08806a860e2139c20d98a5150c6ccd1b28a90f311e`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/bec4433b4206f00c2310a7961cff7f539434b9161b45673793aa5a3b50234313` & `dipdup-7.0.0rc2/tests/replays/bec4433b4206f00c2310a7961cff7f539434b9161b45673793aa5a3b50234313`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/c0202a433296436c27458b3d5ec5c72d5e2d47ff77c939ce399780cc0f3e56bc` & `dipdup-7.0.0rc2/tests/replays/c0202a433296436c27458b3d5ec5c72d5e2d47ff77c939ce399780cc0f3e56bc`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/c369836c15d9ed15477002b850d5cbb96b1ff5ff33e917b812ab9c0905063957` & `dipdup-7.0.0rc2/tests/replays/c369836c15d9ed15477002b850d5cbb96b1ff5ff33e917b812ab9c0905063957`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/c8e8698717ada415bc10405da983c8357165914dd0219f3d09bb9a939705242d` & `dipdup-7.0.0rc2/tests/replays/c8e8698717ada415bc10405da983c8357165914dd0219f3d09bb9a939705242d`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/cc162df04c4990c79f7507dd915601fd4d58c947a248156cbe302a64adfe898a` & `dipdup-7.0.0rc2/tests/replays/cc162df04c4990c79f7507dd915601fd4d58c947a248156cbe302a64adfe898a`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/cc5d3d4a58d5cb6bc7270d38c797b7740b79f913590ef0164abd50e58fba9405` & `dipdup-7.0.0rc2/tests/replays/cc5d3d4a58d5cb6bc7270d38c797b7740b79f913590ef0164abd50e58fba9405`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/d0a594d14bcb3fbf916092ec6707dfd3c9f48f53f0a1ad40a32023e7a87f8ef5` & `dipdup-7.0.0rc2/tests/replays/d0a594d14bcb3fbf916092ec6707dfd3c9f48f53f0a1ad40a32023e7a87f8ef5`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/d62748a927a09395579b5790c8f871cc8653081cf4475abc93173989f950b92b` & `dipdup-7.0.0rc2/tests/replays/d62748a927a09395579b5790c8f871cc8653081cf4475abc93173989f950b92b`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/d94397f6ecec8ce25f87177fe410f6498d7d30a04360506c0cd300d291c167e7` & `dipdup-7.0.0rc2/tests/replays/d94397f6ecec8ce25f87177fe410f6498d7d30a04360506c0cd300d291c167e7`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/dc86d5e346c85e6f7953d7e01298a9db64d778e5ba717ddd07fff8b589081e98` & `dipdup-7.0.0rc2/tests/replays/dc86d5e346c85e6f7953d7e01298a9db64d778e5ba717ddd07fff8b589081e98`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/dca9cf4f9f27623f10975d369444899458ab9ea85c22af2da6ce6ce8c09c2b58` & `dipdup-7.0.0rc2/tests/replays/dca9cf4f9f27623f10975d369444899458ab9ea85c22af2da6ce6ce8c09c2b58`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/df62701276d6dbf4860058cc582c0b4f7b583758f4f5be96c9ee045757c151e3` & `dipdup-7.0.0rc2/tests/replays/df62701276d6dbf4860058cc582c0b4f7b583758f4f5be96c9ee045757c151e3`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/e39ebba701031aa13dfd9eb5dba1effd2938e96682d1030dcbd70172f9f190a9` & `dipdup-7.0.0rc2/tests/replays/e39ebba701031aa13dfd9eb5dba1effd2938e96682d1030dcbd70172f9f190a9`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/e4a563a0b19379a44e9d2dc398131e9fd30d6039ff4ffacf1252db0bf8b433aa` & `dipdup-7.0.0rc2/tests/replays/e4a563a0b19379a44e9d2dc398131e9fd30d6039ff4ffacf1252db0bf8b433aa`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/eb8b6b33cb2e165d1a3a73c09938d3083671a82ad73d4c0cff1fb2a5e5715f76` & `dipdup-7.0.0rc2/tests/replays/eb8b6b33cb2e165d1a3a73c09938d3083671a82ad73d4c0cff1fb2a5e5715f76`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998502994011975%*

 * *Differences: {'76': "{6: {'alias': 'Binance legacy'}}", '77': "{6: {'alias': 'Binance legacy'}}"}*

```diff
@@ -10922,15 +10922,15 @@
         66864850927616,
         1589247,
         "2021-08-06T09:29:54Z",
         "ooYr1ekKJSvNuaaDQybtFSHaLE9gWXA5scpAhPYNwGbj6wNiK3U",
         2334093,
         {
             "address": "tz1SiPXX4MYGNJNDsRc7n8hkvUqFzg8xqF9m",
-            "alias": "Binance"
+            "alias": "Binance legacy"
         },
         null,
         {
             "address": "tz1is7BMbZjgRuufjXs2WsbzegKcZ1LWLatw"
         },
         null,
         1168900000,
@@ -10949,15 +10949,15 @@
         66864851976192,
         1589247,
         "2021-08-06T09:29:54Z",
         "ooYr1ekKJSvNuaaDQybtFSHaLE9gWXA5scpAhPYNwGbj6wNiK3U",
         2334094,
         {
             "address": "tz1SiPXX4MYGNJNDsRc7n8hkvUqFzg8xqF9m",
-            "alias": "Binance"
+            "alias": "Binance legacy"
         },
         null,
         {
             "address": "tz1SiAcRaXib5FjBX3C9Wsa4XVXBqxwy8dBt"
         },
         null,
         17574610,
```

### Comparing `dipdup-7.0.0rc1/tests/replays/eb8e2c3ce2fe7792d2c8e81c61d37821275b64021343103b0c955042ae802189` & `dipdup-7.0.0rc2/tests/replays/eb8e2c3ce2fe7792d2c8e81c61d37821275b64021343103b0c955042ae802189`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/ece1ebe13f9391555230d6b94f33d66a922e2ca71ef5fd39bbd8c2c37ddf54ec` & `dipdup-7.0.0rc2/tests/replays/ece1ebe13f9391555230d6b94f33d66a922e2ca71ef5fd39bbd8c2c37ddf54ec`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/ed3ec9fd9226e9f765b96dc1d5d5a455a7b2505da530961826910b08db693070` & `dipdup-7.0.0rc2/tests/replays/ed3ec9fd9226e9f765b96dc1d5d5a455a7b2505da530961826910b08db693070`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/f3d608f99e6b92e28a064bb9c10c3c605c9c817383c1eebcc68f663d1d23d650` & `dipdup-7.0.0rc2/tests/replays/f3d608f99e6b92e28a064bb9c10c3c605c9c817383c1eebcc68f663d1d23d650`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/f60e794a9be14263cb10e48546ba5610302cc3e7af0a114a593bb50eb85ba5e7` & `dipdup-7.0.0rc2/tests/replays/f60e794a9be14263cb10e48546ba5610302cc3e7af0a114a593bb50eb85ba5e7`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/replays/ff51b3535acc2972090ecd5db3af8f827464c9d92f1aa661630976e5b4ed4cbe` & `dipdup-7.0.0rc2/tests/replays/ff51b3535acc2972090ecd5db3af8f827464c9d92f1aa661630976e5b4ed4cbe`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/responses/asdf.json` & `dipdup-7.0.0rc2/tests/responses/asdf.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/responses/ftzfun.json` & `dipdup-7.0.0rc2/tests/responses/ftzfun.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/responses/hen_subjkt.json` & `dipdup-7.0.0rc2/tests/responses/hen_subjkt.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/responses/hjkl.json` & `dipdup-7.0.0rc2/tests/responses/hjkl.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/responses/kolibri_ovens.json` & `dipdup-7.0.0rc2/tests/responses/kolibri_ovens.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/responses/ooQuCAKBHkmWy2VciDAV9c6CFTywuMLupLzVoKDwS1xvR4EdRng.json` & `dipdup-7.0.0rc2/tests/responses/ooQuCAKBHkmWy2VciDAV9c6CFTywuMLupLzVoKDwS1xvR4EdRng.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/responses/origination_amount.json` & `dipdup-7.0.0rc2/tests/responses/origination_amount.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/responses/qwer.json` & `dipdup-7.0.0rc2/tests/responses/qwer.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/responses/rewq.json` & `dipdup-7.0.0rc2/tests/responses/rewq.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/responses/yupana.json` & `dipdup-7.0.0rc2/tests/responses/yupana.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/responses/zxcv.json` & `dipdup-7.0.0rc2/tests/responses/zxcv.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/schemas/asdf/storage.json` & `dipdup-7.0.0rc2/tests/schemas/asdf/storage.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/schemas/hen_subjkt/storage.json` & `dipdup-7.0.0rc2/tests/schemas/hen_subjkt/storage.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/schemas/hjkl/storage.json` & `dipdup-7.0.0rc2/tests/schemas/hjkl/storage.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/schemas/kolibri_ovens/storage.json` & `dipdup-7.0.0rc2/tests/schemas/kolibri_ovens/storage.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/schemas/qwer/storage.json` & `dipdup-7.0.0rc2/tests/schemas/qwer/storage.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/schemas/rewq/storage.json` & `dipdup-7.0.0rc2/tests/schemas/rewq/storage.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/schemas/yupana/storage.json` & `dipdup-7.0.0rc2/tests/schemas/yupana/storage.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/schemas/zxcv/storage.json` & `dipdup-7.0.0rc2/tests/schemas/zxcv/storage.json`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/test_config/test_callbacks.py` & `dipdup-7.0.0rc2/tests/test_config/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/test_config/test_config.py` & `dipdup-7.0.0rc2/tests/test_config/test_config.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/test_config/test_custom_config.py` & `dipdup-7.0.0rc2/tests/test_config/test_custom_config.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/test_context.py` & `dipdup-7.0.0rc2/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/test_datasources/test_ipfs.py` & `dipdup-7.0.0rc2/tests/test_datasources/test_ipfs.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/test_datasources/test_metadata.py` & `dipdup-7.0.0rc2/tests/test_datasources/test_metadata.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/test_datasources/test_tzkt.py` & `dipdup-7.0.0rc2/tests/test_datasources/test_tzkt.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/test_datasources/test_tzkt_blocks.py` & `dipdup-7.0.0rc2/tests/test_datasources/test_tzkt_blocks.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/test_datasources/test_tzkt_buffer.py` & `dipdup-7.0.0rc2/tests/test_datasources/test_tzkt_buffer.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/test_datasources/test_tzkt_quotes.py` & `dipdup-7.0.0rc2/tests/test_datasources/test_tzkt_quotes.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/test_demos.py` & `dipdup-7.0.0rc2/tests/test_demos.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 
 @asynccontextmanager
 async def run_dipdup_demo(config: str, package: str, cmd: str = 'run') -> AsyncIterator[Path]:
     config_path = CONFIGS_PATH / config
     dipdup_pkg_path = SRC_PATH / 'dipdup'
     demo_pkg_path = SRC_PATH / package
+    sqlite_config_path = Path(__file__).parent / 'configs' / 'sqlite.yaml'
 
     with tempfile.TemporaryDirectory() as tmp_root_path:
         # NOTE: Symlink configs, packages and executables
         tmp_config_path = Path(tmp_root_path) / 'dipdup.yaml'
         os.symlink(config_path, tmp_config_path)
 
         tmp_bin_path = Path(tmp_root_path) / 'bin'
@@ -52,15 +53,15 @@
             **os.environ,
             'PATH': str(tmp_bin_path),
             'PYTHONPATH': str(tmp_root_path),
             'DIPDUP_TEST': '1',
         }
 
         subprocess.run(
-            f'dipdup -c {tmp_config_path} {cmd}',
+            f'dipdup -c {tmp_config_path} -c {sqlite_config_path} {cmd}',
             cwd=tmp_root_path,
             check=True,
             shell=True,
             env=env,
             stderr=subprocess.PIPE,
             stdout=subprocess.PIPE,
         )
```

### Comparing `dipdup-7.0.0rc1/tests/test_dipdup.py` & `dipdup-7.0.0rc2/tests/test_dipdup.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/test_hasura.py` & `dipdup-7.0.0rc2/tests/test_hasura.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/test_index/test_operation.py` & `dipdup-7.0.0rc2/tests/test_index/test_operation.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/test_introspection.py` & `dipdup-7.0.0rc2/tests/test_introspection.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/test_models.py` & `dipdup-7.0.0rc2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/test_rollback.py` & `dipdup-7.0.0rc2/tests/test_rollback.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/test_utils.py` & `dipdup-7.0.0rc2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/types/bazaar/storage.py` & `dipdup-7.0.0rc2/tests/types/bazaar/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/types/ftzfun/storage.py` & `dipdup-7.0.0rc2/tests/types/ftzfun/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/types/hen_subjkt/storage.py` & `dipdup-7.0.0rc2/tests/types/hen_subjkt/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/types/hjkl/storage.py` & `dipdup-7.0.0rc2/tests/types/hjkl/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/types/qwer/storage.py` & `dipdup-7.0.0rc2/tests/types/qwer/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/types/rewq/storage.py` & `dipdup-7.0.0rc2/tests/types/rewq/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/types/tezotop/storage.py` & `dipdup-7.0.0rc2/tests/types/tezotop/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/types/yupana/storage.py` & `dipdup-7.0.0rc2/tests/types/yupana/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/tests/types/zxcv/storage.py` & `dipdup-7.0.0rc2/tests/types/zxcv/storage.py`

 * *Files identical despite different names*

### Comparing `dipdup-7.0.0rc1/PKG-INFO` & `dipdup-7.0.0rc2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dipdup
-Version: 7.0.0rc1
+Version: 7.0.0rc2
 Summary: Modular framework for creating selective indexers and featureful backends for dapps
 Keywords: api backend blockchain crypto cryptocurrencies dapp declarative ethereum evm framework indexer indexers michelson scheduler sdk smart-contracts tezos tzkt
 Author-Email: Lev Gorodetskii <dipdup@drsr.io>, Vladimir Bobrikov <vladimir_bobrikov@pm.me>, Michael Zaikin <mz@baking-bad.org>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Typing :: Typed
 Project-URL: Homepage, https://dipdup.io/
-Project-URL: Documentation, https://docs.dipdup.io
+Project-URL: Documentation, https://dipdup.io/docs
 Project-URL: Repository, https://github.com/dipdup-io/dipdup
 Requires-Python: <3.12,>=3.11
 Requires-Dist: asyncpg~=0.28.0
 Requires-Dist: datamodel-code-generator~=0.21.1
 Requires-Dist: pydantic~=1.10.11
 Requires-Dist: tortoise-orm===0.19.3
 Requires-Dist: aiohttp~=3.8
@@ -56,25 +56,25 @@
 [![GitHub issues](https://img.shields.io/github/issues/dipdup-io/dipdup?color=2c2c2c)](https://github.com/dipdup-io/dipdup/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/dipdup-io/dipdup?color=2c2c2c)](https://github.com/dipdup-io/dipdup/pulls)
 
 <h3 align="center"><img src="https://actual-docs.interface-1bp.pages.dev/_nuxt/logo.9b02ab5e.svg" alt="DipDup logo"></h3>
 
 DipDup is a Python framework for building smart contract indexers. It helps developers focus on business logic instead of writing a boilerplate to store and serve data. DipDup-based indexers are selective, which means only required data is requested. This approach allows to achieve faster indexing times and decreased load on underlying APIs.
 
-* **Ready to build your first indexer?** Head to [Quickstart](https://docs.dipdup.io/quickstart).
+- **Ready to build your first indexer?** Head to [Quickstart](https://dipdup.io/docs/quickstart).
 
-* **Looking for examples?** Check out [Demo Projects](https://docs.dipdup.io/examples/demo-projects) and [Built with DipDup](https://docs.dipdup.io/examples/built-with-dipdup) pages.
+- **Looking for examples?** Check out [Demo Projects](https://dipdup.io/docs/examples/demos) and [Built with DipDup](https://dipdup.io/docs/examples/built-with-dipdup) pages.
 
-* **Want to participate?** Vote for [open issues](https://github.com/dipdup-io/dipdup/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc), join [discussions](https://github.com/dipdup-io/dipdup/discussions) or [become a sponsor](https://github.com/sponsors/dipdup-io).
+- **Want to participate?** Vote for [open issues](https://github.com/dipdup-io/dipdup/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc), join [discussions](https://github.com/dipdup-io/dipdup/discussions) or [become a sponsor](https://github.com/sponsors/dipdup-io).
 
-* **Have a question?** Join our [Discord](https://discord.gg/NbANhqCJHA) or tag @dipdup_io on [Twitter](https://twitter.com/dipdup_io).
+- **Have a question?** Join our [Discord](https://discord.gg/NbANhqCJHA) or tag @dipdup_io on [Twitter](https://twitter.com/dipdup_io).
 
 This project is maintained by the [Baking Bad](https://bakingbad.dev/) team.
 <br>
-Development is supported by [Tezos Foundation](https://tezos.foundation/).
+Development is supported by [Tezos Foundation](https://tezos.foundation/) and [OnlyDust](https://www.onlydust.xyz).
 
 ## Thanks
 
 ### Sponsors
 
 Decentralized web requires decentralized funding. The following people and organizations help the project to be sustainable.
```

