# Comparing `tmp/data_diff-0.7.9.tar.gz` & `tmp/data_diff-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_diff-0.7.9.tar", max compression
+gzip compressed data, was "data_diff-0.8.0.tar", max compression
```

## Comparing `data_diff-0.7.9.tar` & `data_diff-0.8.0.tar`

### file list

```diff
@@ -1,73 +1,74 @@
--rw-r--r--   0        0        0     1053 2023-04-03 18:06:26.931220 data_diff-0.7.9/LICENSE
--rw-r--r--   0        0        0     2696 2023-05-11 19:39:43.703801 data_diff-0.7.9/README.md
--rw-r--r--   0        0        0     8710 2023-05-24 18:36:17.565800 data_diff-0.7.9/data_diff/__init__.py
--rw-r--r--   0        0        0    16825 2023-06-14 23:21:12.728962 data_diff-0.7.9/data_diff/__main__.py
--rw-r--r--   0        0        0      126 2023-05-15 21:10:13.082463 data_diff-0.7.9/data_diff/cloud/__init__.py
--rw-r--r--   0        0        0    11568 2023-06-14 23:21:12.729167 data_diff-0.7.9/data_diff/cloud/data_source.py
--rw-r--r--   0        0        0    10067 2023-05-15 21:10:13.082649 data_diff-0.7.9/data_diff/cloud/datafold_api.py
--rw-r--r--   0        0        0     4044 2023-04-03 18:06:26.931568 data_diff-0.7.9/data_diff/config.py
--rw-r--r--   0        0        0      493 2023-04-21 21:58:08.194615 data_diff-0.7.9/data_diff/databases/__init__.py
--rw-r--r--   0        0        0     1353 2023-04-21 21:58:08.194720 data_diff-0.7.9/data_diff/databases/_connect.py
--rw-r--r--   0        0        0      174 2023-04-21 21:58:08.194816 data_diff-0.7.9/data_diff/databases/base.py
--rw-r--r--   0        0        0      257 2023-04-21 21:58:08.195148 data_diff-0.7.9/data_diff/databases/bigquery.py
--rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195281 data_diff-0.7.9/data_diff/databases/clickhouse.py
--rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195390 data_diff-0.7.9/data_diff/databases/databricks.py
--rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195511 data_diff-0.7.9/data_diff/databases/duckdb.py
--rw-r--r--   0        0        0      236 2023-04-21 21:58:08.195617 data_diff-0.7.9/data_diff/databases/mysql.py
--rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195713 data_diff-0.7.9/data_diff/databases/oracle.py
--rw-r--r--   0        0        0      275 2023-04-21 21:58:08.195827 data_diff-0.7.9/data_diff/databases/postgresql.py
--rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195918 data_diff-0.7.9/data_diff/databases/presto.py
--rw-r--r--   0        0        0      257 2023-04-21 21:58:08.196013 data_diff-0.7.9/data_diff/databases/redshift.py
--rw-r--r--   0        0        0      264 2023-04-21 21:58:08.196109 data_diff-0.7.9/data_diff/databases/snowflake.py
--rw-r--r--   0        0        0      236 2023-04-21 21:58:08.196196 data_diff-0.7.9/data_diff/databases/trino.py
--rw-r--r--   0        0        0      250 2023-04-21 21:58:08.196288 data_diff-0.7.9/data_diff/databases/vertica.py
--rw-r--r--   0        0        0    17316 2023-06-14 23:21:12.729369 data_diff-0.7.9/data_diff/dbt.py
--rw-r--r--   0        0        0    20102 2023-06-14 23:21:12.729586 data_diff-0.7.9/data_diff/dbt_parser.py
--rw-r--r--   0        0        0    14376 2023-04-21 21:58:08.196773 data_diff-0.7.9/data_diff/diff_tables.py
--rw-r--r--   0        0        0     1753 2023-06-14 23:21:12.729730 data_diff-0.7.9/data_diff/errors.py
--rw-r--r--   0        0        0     9333 2023-05-05 21:08:17.222755 data_diff-0.7.9/data_diff/hashdiff_tables.py
--rw-r--r--   0        0        0     1477 2023-06-14 16:32:15.976930 data_diff-0.7.9/data_diff/info_tree.py
--rw-r--r--   0        0        0    15337 2023-06-14 16:32:15.977221 data_diff-0.7.9/data_diff/joindiff_tables.py
--rw-r--r--   0        0        0     7557 2023-04-03 18:06:26.932827 data_diff-0.7.9/data_diff/lexicographic_space.py
--rw-r--r--   0        0        0     1783 2023-04-03 18:06:26.932897 data_diff-0.7.9/data_diff/parse_time.py
--rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.197181 data_diff-0.7.9/data_diff/query_utils.py
--rw-r--r--   0        0        0       76 2023-04-21 21:58:08.197422 data_diff-0.7.9/data_diff/sqeleton/__init__.py
--rw-r--r--   0        0        0      279 2023-04-21 21:58:08.197521 data_diff-0.7.9/data_diff/sqeleton/__main__.py
--rw-r--r--   0        0        0      264 2023-05-05 21:08:17.222879 data_diff-0.7.9/data_diff/sqeleton/abcs/__init__.py
--rw-r--r--   0        0        0      409 2023-04-21 21:58:08.197743 data_diff-0.7.9/data_diff/sqeleton/abcs/compiler.py
--rw-r--r--   0        0        0    11118 2023-05-05 21:08:17.223038 data_diff-0.7.9/data_diff/sqeleton/abcs/database_types.py
--rw-r--r--   0        0        0     6989 2023-05-05 21:08:17.223166 data_diff-0.7.9/data_diff/sqeleton/abcs/mixins.py
--rw-r--r--   0        0        0     2425 2023-04-21 21:58:08.198003 data_diff-0.7.9/data_diff/sqeleton/bound_exprs.py
--rw-r--r--   0        0        0      554 2023-04-21 21:58:08.198154 data_diff-0.7.9/data_diff/sqeleton/databases/__init__.py
--rw-r--r--   0        0        0     9245 2023-05-15 21:10:13.083663 data_diff-0.7.9/data_diff/sqeleton/databases/_connect.py
--rw-r--r--   0        0        0    20140 2023-05-11 19:39:43.705453 data_diff-0.7.9/data_diff/sqeleton/databases/base.py
--rw-r--r--   0        0        0    10648 2023-06-14 23:21:12.731092 data_diff-0.7.9/data_diff/sqeleton/databases/bigquery.py
--rw-r--r--   0        0        0     6642 2023-04-21 21:58:08.198608 data_diff-0.7.9/data_diff/sqeleton/databases/clickhouse.py
--rw-r--r--   0        0        0     6959 2023-04-21 21:58:08.198702 data_diff-0.7.9/data_diff/sqeleton/databases/databricks.py
--rw-r--r--   0        0        0     6093 2023-04-21 21:58:08.198787 data_diff-0.7.9/data_diff/sqeleton/databases/duckdb.py
--rw-r--r--   0        0        0      910 2023-04-21 21:58:08.198859 data_diff-0.7.9/data_diff/sqeleton/databases/mssql.py
--rw-r--r--   0        0        0     4438 2023-04-21 21:58:08.198940 data_diff-0.7.9/data_diff/sqeleton/databases/mysql.py
--rw-r--r--   0        0        0     6550 2023-05-05 21:08:17.223666 data_diff-0.7.9/data_diff/sqeleton/databases/oracle.py
--rw-r--r--   0        0        0     5551 2023-05-05 21:08:17.223788 data_diff-0.7.9/data_diff/sqeleton/databases/postgresql.py
--rw-r--r--   0        0        0     6112 2023-04-21 21:58:08.199200 data_diff-0.7.9/data_diff/sqeleton/databases/presto.py
--rw-r--r--   0        0        0     6297 2023-05-24 18:36:17.567499 data_diff-0.7.9/data_diff/sqeleton/databases/redshift.py
--rw-r--r--   0        0        0     7742 2023-04-21 21:58:08.199375 data_diff-0.7.9/data_diff/sqeleton/databases/snowflake.py
--rw-r--r--   0        0        0     1297 2023-04-21 21:58:08.199477 data_diff-0.7.9/data_diff/sqeleton/databases/trino.py
--rw-r--r--   0        0        0     5426 2023-04-21 21:58:08.199590 data_diff-0.7.9/data_diff/sqeleton/databases/vertica.py
--rw-r--r--   0        0        0      464 2023-04-21 21:58:08.199708 data_diff-0.7.9/data_diff/sqeleton/queries/__init__.py
--rw-r--r--   0        0        0     5291 2023-04-21 21:58:08.199788 data_diff-0.7.9/data_diff/sqeleton/queries/api.py
--rw-r--r--   0        0        0    30750 2023-05-05 21:08:17.224381 data_diff-0.7.9/data_diff/sqeleton/queries/ast_classes.py
--rw-r--r--   0        0        0      367 2023-04-21 21:58:08.200018 data_diff-0.7.9/data_diff/sqeleton/queries/base.py
--rw-r--r--   0        0        0     2605 2023-04-21 21:58:08.200096 data_diff-0.7.9/data_diff/sqeleton/queries/compiler.py
--rw-r--r--   0        0        0     1985 2023-04-21 21:58:08.200163 data_diff-0.7.9/data_diff/sqeleton/queries/extras.py
--rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.200227 data_diff-0.7.9/data_diff/sqeleton/query_utils.py
--rw-r--r--   0        0        0     1981 2023-04-21 21:58:08.200332 data_diff-0.7.9/data_diff/sqeleton/repl.py
--rw-r--r--   0        0        0      737 2023-04-21 21:58:08.200391 data_diff-0.7.9/data_diff/sqeleton/schema.py
--rw-r--r--   0        0        0     8907 2023-04-21 21:58:08.200481 data_diff-0.7.9/data_diff/sqeleton/utils.py
--rw-r--r--   0        0        0    10884 2023-04-21 21:58:08.200617 data_diff-0.7.9/data_diff/table_segment.py
--rw-r--r--   0        0        0     2651 2023-04-03 18:06:26.933183 data_diff-0.7.9/data_diff/thread_utils.py
--rw-r--r--   0        0        0     5481 2023-06-14 22:17:36.188033 data_diff-0.7.9/data_diff/tracking.py
--rw-r--r--   0        0        0     6637 2023-06-08 19:44:38.931340 data_diff-0.7.9/data_diff/utils.py
--rw-r--r--   0        0        0       22 2023-06-14 23:23:45.736859 data_diff-0.7.9/data_diff/version.py
--rwxr-xr-x   0        0        0     2851 2023-06-14 23:23:47.177863 data_diff-0.7.9/pyproject.toml
--rw-r--r--   0        0        0     5286 1970-01-01 00:00:00.000000 data_diff-0.7.9/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-04-03 18:06:26.931220 data_diff-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2742 2023-07-27 16:41:55.956926 data_diff-0.8.0/README.md
+-rw-r--r--   0        0        0     8710 2023-05-24 18:36:17.565800 data_diff-0.8.0/data_diff/__init__.py
+-rw-r--r--   0        0        0    18130 2023-07-27 15:17:08.933362 data_diff-0.8.0/data_diff/__main__.py
+-rw-r--r--   0        0        0      126 2023-05-15 21:10:13.082463 data_diff-0.8.0/data_diff/cloud/__init__.py
+-rw-r--r--   0        0        0    11568 2023-06-16 19:57:48.275419 data_diff-0.8.0/data_diff/cloud/data_source.py
+-rw-r--r--   0        0        0    10562 2023-07-25 19:31:06.998411 data_diff-0.8.0/data_diff/cloud/datafold_api.py
+-rw-r--r--   0        0        0     4044 2023-04-03 18:06:26.931568 data_diff-0.8.0/data_diff/config.py
+-rw-r--r--   0        0        0      493 2023-04-21 21:58:08.194615 data_diff-0.8.0/data_diff/databases/__init__.py
+-rw-r--r--   0        0        0     1353 2023-04-21 21:58:08.194720 data_diff-0.8.0/data_diff/databases/_connect.py
+-rw-r--r--   0        0        0      174 2023-04-21 21:58:08.194816 data_diff-0.8.0/data_diff/databases/base.py
+-rw-r--r--   0        0        0      257 2023-04-21 21:58:08.195148 data_diff-0.8.0/data_diff/databases/bigquery.py
+-rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195281 data_diff-0.8.0/data_diff/databases/clickhouse.py
+-rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195390 data_diff-0.8.0/data_diff/databases/databricks.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195511 data_diff-0.8.0/data_diff/databases/duckdb.py
+-rw-r--r--   0        0        0      236 2023-04-21 21:58:08.195617 data_diff-0.8.0/data_diff/databases/mysql.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195713 data_diff-0.8.0/data_diff/databases/oracle.py
+-rw-r--r--   0        0        0      275 2023-04-21 21:58:08.195827 data_diff-0.8.0/data_diff/databases/postgresql.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195918 data_diff-0.8.0/data_diff/databases/presto.py
+-rw-r--r--   0        0        0      257 2023-04-21 21:58:08.196013 data_diff-0.8.0/data_diff/databases/redshift.py
+-rw-r--r--   0        0        0      264 2023-04-21 21:58:08.196109 data_diff-0.8.0/data_diff/databases/snowflake.py
+-rw-r--r--   0        0        0      236 2023-04-21 21:58:08.196196 data_diff-0.8.0/data_diff/databases/trino.py
+-rw-r--r--   0        0        0      250 2023-04-21 21:58:08.196288 data_diff-0.8.0/data_diff/databases/vertica.py
+-rw-r--r--   0        0        0    19863 2023-07-27 15:25:50.449603 data_diff-0.8.0/data_diff/dbt.py
+-rw-r--r--   0        0        0    20292 2023-07-27 15:17:08.934005 data_diff-0.8.0/data_diff/dbt_parser.py
+-rw-r--r--   0        0        0    14471 2023-07-18 16:15:04.405684 data_diff-0.8.0/data_diff/diff_tables.py
+-rw-r--r--   0        0        0     2411 2023-07-25 19:31:06.998680 data_diff-0.8.0/data_diff/errors.py
+-rw-r--r--   0        0        0     9098 2023-07-16 03:33:52.656293 data_diff-0.8.0/data_diff/format.py
+-rw-r--r--   0        0        0     9405 2023-06-27 22:04:20.813975 data_diff-0.8.0/data_diff/hashdiff_tables.py
+-rw-r--r--   0        0        0     1917 2023-06-22 19:56:54.945638 data_diff-0.8.0/data_diff/info_tree.py
+-rw-r--r--   0        0        0    15377 2023-06-22 19:56:54.946004 data_diff-0.8.0/data_diff/joindiff_tables.py
+-rw-r--r--   0        0        0     7557 2023-04-03 18:06:26.932827 data_diff-0.8.0/data_diff/lexicographic_space.py
+-rw-r--r--   0        0        0     1783 2023-04-03 18:06:26.932897 data_diff-0.8.0/data_diff/parse_time.py
+-rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.197181 data_diff-0.8.0/data_diff/query_utils.py
+-rw-r--r--   0        0        0       76 2023-04-21 21:58:08.197422 data_diff-0.8.0/data_diff/sqeleton/__init__.py
+-rw-r--r--   0        0        0      279 2023-04-21 21:58:08.197521 data_diff-0.8.0/data_diff/sqeleton/__main__.py
+-rw-r--r--   0        0        0      264 2023-05-05 21:08:17.222879 data_diff-0.8.0/data_diff/sqeleton/abcs/__init__.py
+-rw-r--r--   0        0        0      409 2023-04-21 21:58:08.197743 data_diff-0.8.0/data_diff/sqeleton/abcs/compiler.py
+-rw-r--r--   0        0        0    11118 2023-05-05 21:08:17.223038 data_diff-0.8.0/data_diff/sqeleton/abcs/database_types.py
+-rw-r--r--   0        0        0     7029 2023-06-27 22:04:20.814299 data_diff-0.8.0/data_diff/sqeleton/abcs/mixins.py
+-rw-r--r--   0        0        0     2425 2023-04-21 21:58:08.198003 data_diff-0.8.0/data_diff/sqeleton/bound_exprs.py
+-rw-r--r--   0        0        0      554 2023-04-21 21:58:08.198154 data_diff-0.8.0/data_diff/sqeleton/databases/__init__.py
+-rw-r--r--   0        0        0     9245 2023-06-20 20:21:00.599502 data_diff-0.8.0/data_diff/sqeleton/databases/_connect.py
+-rw-r--r--   0        0        0    20140 2023-05-11 19:39:43.705453 data_diff-0.8.0/data_diff/sqeleton/databases/base.py
+-rw-r--r--   0        0        0    10648 2023-06-16 19:57:48.277742 data_diff-0.8.0/data_diff/sqeleton/databases/bigquery.py
+-rw-r--r--   0        0        0     6642 2023-04-21 21:58:08.198608 data_diff-0.8.0/data_diff/sqeleton/databases/clickhouse.py
+-rw-r--r--   0        0        0     6959 2023-04-21 21:58:08.198702 data_diff-0.8.0/data_diff/sqeleton/databases/databricks.py
+-rw-r--r--   0        0        0     6093 2023-04-21 21:58:08.198787 data_diff-0.8.0/data_diff/sqeleton/databases/duckdb.py
+-rw-r--r--   0        0        0      910 2023-04-21 21:58:08.198859 data_diff-0.8.0/data_diff/sqeleton/databases/mssql.py
+-rw-r--r--   0        0        0     4438 2023-04-21 21:58:08.198940 data_diff-0.8.0/data_diff/sqeleton/databases/mysql.py
+-rw-r--r--   0        0        0     6550 2023-05-05 21:08:17.223666 data_diff-0.8.0/data_diff/sqeleton/databases/oracle.py
+-rw-r--r--   0        0        0     5550 2023-06-27 22:04:20.814520 data_diff-0.8.0/data_diff/sqeleton/databases/postgresql.py
+-rw-r--r--   0        0        0     6112 2023-04-21 21:58:08.199200 data_diff-0.8.0/data_diff/sqeleton/databases/presto.py
+-rw-r--r--   0        0        0     6295 2023-06-27 22:04:20.814736 data_diff-0.8.0/data_diff/sqeleton/databases/redshift.py
+-rw-r--r--   0        0        0     7742 2023-04-21 21:58:08.199375 data_diff-0.8.0/data_diff/sqeleton/databases/snowflake.py
+-rw-r--r--   0        0        0     1297 2023-04-21 21:58:08.199477 data_diff-0.8.0/data_diff/sqeleton/databases/trino.py
+-rw-r--r--   0        0        0     5426 2023-04-21 21:58:08.199590 data_diff-0.8.0/data_diff/sqeleton/databases/vertica.py
+-rw-r--r--   0        0        0      464 2023-04-21 21:58:08.199708 data_diff-0.8.0/data_diff/sqeleton/queries/__init__.py
+-rw-r--r--   0        0        0     5291 2023-04-21 21:58:08.199788 data_diff-0.8.0/data_diff/sqeleton/queries/api.py
+-rw-r--r--   0        0        0    30750 2023-05-05 21:08:17.224381 data_diff-0.8.0/data_diff/sqeleton/queries/ast_classes.py
+-rw-r--r--   0        0        0      367 2023-04-21 21:58:08.200018 data_diff-0.8.0/data_diff/sqeleton/queries/base.py
+-rw-r--r--   0        0        0     2605 2023-04-21 21:58:08.200096 data_diff-0.8.0/data_diff/sqeleton/queries/compiler.py
+-rw-r--r--   0        0        0     1985 2023-04-21 21:58:08.200163 data_diff-0.8.0/data_diff/sqeleton/queries/extras.py
+-rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.200227 data_diff-0.8.0/data_diff/sqeleton/query_utils.py
+-rw-r--r--   0        0        0     1981 2023-04-21 21:58:08.200332 data_diff-0.8.0/data_diff/sqeleton/repl.py
+-rw-r--r--   0        0        0      737 2023-04-21 21:58:08.200391 data_diff-0.8.0/data_diff/sqeleton/schema.py
+-rw-r--r--   0        0        0     8906 2023-06-27 22:04:20.814972 data_diff-0.8.0/data_diff/sqeleton/utils.py
+-rw-r--r--   0        0        0    10884 2023-04-21 21:58:08.200617 data_diff-0.8.0/data_diff/table_segment.py
+-rw-r--r--   0        0        0     2651 2023-04-03 18:06:26.933183 data_diff-0.8.0/data_diff/thread_utils.py
+-rw-r--r--   0        0        0     5481 2023-06-16 19:57:48.278007 data_diff-0.8.0/data_diff/tracking.py
+-rw-r--r--   0        0        0     7840 2023-06-27 22:04:20.815284 data_diff-0.8.0/data_diff/utils.py
+-rw-r--r--   0        0        0       22 2023-07-27 16:42:35.824003 data_diff-0.8.0/data_diff/version.py
+-rwxr-xr-x   0        0        0     2729 2023-07-27 16:42:16.366305 data_diff-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     5253 1970-01-01 00:00:00.000000 data_diff-0.8.0/PKG-INFO
```

### Comparing `data_diff-0.7.9/LICENSE` & `data_diff-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/__init__.py` & `data_diff-0.8.0/data_diff/__init__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/__main__.py` & `data_diff-0.8.0/data_diff/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,44 +2,64 @@
 from datetime import datetime
 import os
 import sys
 import time
 import json
 import logging
 from itertools import islice
-from typing import Optional
+from typing import Dict, Optional
 
 import rich
+from rich.logging import RichHandler
 import click
 
 from data_diff.sqeleton.schema import create_schema
 from data_diff.sqeleton.queries.api import current_timestamp
 
 from .dbt import dbt_diff
-from .utils import eval_name_template, remove_password_from_url, safezip, match_like
+from .utils import eval_name_template, remove_password_from_url, safezip, match_like, LogStatusHandler
 from .diff_tables import Algorithm
 from .hashdiff_tables import HashDiffer, DEFAULT_BISECTION_THRESHOLD, DEFAULT_BISECTION_FACTOR
 from .joindiff_tables import TABLE_WRITE_LIMIT, JoinDiffer
 from .table_segment import TableSegment
 from .databases import connect
 from .parse_time import parse_time_before, UNITS_STR, ParseError
 from .config import apply_config_from_file
 from .tracking import disable_tracking, set_entrypoint_name
 from .version import __version__
 
 
-LOG_FORMAT = "[%(asctime)s] %(levelname)s - %(message)s"
-DATE_FORMAT = "%H:%M:%S"
-
 COLOR_SCHEME = {
     "+": "green",
     "-": "red",
 }
 
-set_entrypoint_name("CLI")
+set_entrypoint_name(os.getenv("DATAFOLD_TRIGGERED_BY", "CLI"))
+
+
+def _get_log_handlers(is_dbt: Optional[bool] = False) -> Dict[str, logging.Handler]:
+    handlers = {}
+    date_format = "%H:%M:%S"
+    log_format_rich = "%(message)s"
+
+    # limits to 100 characters arbitrarily
+    log_format_status = "%(message).100s"
+    rich_handler = RichHandler(rich_tracebacks=True)
+    rich_handler.setFormatter(logging.Formatter(log_format_rich, datefmt=date_format))
+    rich_handler.setLevel(logging.WARN)
+    handlers["rich_handler"] = rich_handler
+
+    # only use log_status_handler in a terminal
+    if rich_handler.console.is_terminal and is_dbt:
+        log_status_handler = LogStatusHandler()
+        log_status_handler.setFormatter(logging.Formatter(log_format_status, datefmt=date_format))
+        log_status_handler.setLevel(logging.DEBUG)
+        handlers["log_status_handler"] = log_status_handler
+
+    return handlers
 
 
 def _remove_passwords_in_dict(d: dict):
     for k, v in d.items():
         if k == "password":
             d[k] = "*" * len(v)
         elif isinstance(v, dict):
@@ -240,14 +260,15 @@
     "--state",
     "-s",
     default=None,
     metavar="PATH",
     help="Specify manifest to utilize for 'prod' comparison paths instead of using configuration.",
 )
 def main(conf, run, **kw):
+    log_handlers = _get_log_handlers(kw["dbt"])
     if kw["table2"] is None and kw["database2"]:
         # Use the "database table table" form
         kw["table2"] = kw["database2"]
         kw["database2"] = kw["database1"]
 
     if kw["version"]:
         print(f"v{__version__}")
@@ -259,41 +280,48 @@
     if kw["no_tracking"]:
         disable_tracking()
 
     if kw.get("interactive"):
         kw["debug"] = True
 
     if kw["debug"]:
-        logging.basicConfig(level=logging.DEBUG, format=LOG_FORMAT, datefmt=DATE_FORMAT)
+        log_handlers["rich_handler"].setLevel(logging.DEBUG)
+        logging.basicConfig(level=logging.DEBUG, handlers=list(log_handlers.values()))
         if kw.get("__conf__"):
             kw["__conf__"] = deepcopy(kw["__conf__"])
             _remove_passwords_in_dict(kw["__conf__"])
             logging.debug(f"Applied run configuration: {kw['__conf__']}")
     elif kw.get("verbose"):
-        logging.basicConfig(level=logging.INFO, format=LOG_FORMAT, datefmt=DATE_FORMAT)
+        log_handlers["rich_handler"].setLevel(logging.INFO)
+        logging.basicConfig(level=logging.DEBUG, handlers=list(log_handlers.values()))
     else:
-        logging.basicConfig(level=logging.WARNING, format=LOG_FORMAT, datefmt=DATE_FORMAT)
+        log_handlers["rich_handler"].setLevel(logging.WARNING)
+        logging.basicConfig(level=logging.DEBUG, handlers=list(log_handlers.values()))
 
     try:
         state = kw.pop("state", None)
         if state:
             state = os.path.expanduser(state)
         profiles_dir_override = kw.pop("dbt_profiles_dir", None)
         if profiles_dir_override:
             profiles_dir_override = os.path.expanduser(profiles_dir_override)
         project_dir_override = kw.pop("dbt_project_dir", None)
         if project_dir_override:
             project_dir_override = os.path.expanduser(project_dir_override)
         if kw["dbt"]:
             dbt_diff(
+                log_status_handler=log_handlers.get("log_status_handler"),
                 profiles_dir_override=profiles_dir_override,
                 project_dir_override=project_dir_override,
                 is_cloud=kw["cloud"],
                 dbt_selection=kw["select"],
+                json_output=kw["json_output"],
                 state=state,
+                where_flag=kw["where"],
+                columns_flag=kw["columns"],
             )
         else:
             return _data_diff(
                 dbt_project_dir=project_dir_override, dbt_profiles_dir=profiles_dir_override, state=state, **kw
             )
     except Exception as e:
         logging.error(e)
```

### Comparing `data_diff-0.7.9/data_diff/cloud/data_source.py` & `data_diff-0.8.0/data_diff/cloud/data_source.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/cloud/datafold_api.py` & `data_diff-0.8.0/data_diff/cloud/datafold_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import enum
 import time
 from typing import Any, Dict, List, Optional, Type, TypeVar, Tuple
 
 import pydantic
 import requests
 
+from data_diff.errors import DataDiffCloudDiffFailed, DataDiffCloudDiffTimedOut, DataDiffDatasourceIdNotFoundError
+
 from ..utils import getLogger
 
 logger = getLogger(__name__)
 
 Self = TypeVar("Self", bound=pydantic.BaseModel)
 
 
@@ -203,17 +205,23 @@
 
     def get_data_sources(self) -> List[TCloudApiDataSource]:
         rv = self.make_get_request(url="api/v1/data_sources")
         rv.raise_for_status()
         return [TCloudApiDataSource(**item) for item in rv.json()]
 
     def get_data_source(self, data_source_id: int) -> TCloudApiDataSource:
-        rv = self.make_get_request(url=f"api/v1/data_sources/{data_source_id}")
+        rv = self.make_get_request(url=f"api/v1/data_sources")
         rv.raise_for_status()
-        return TCloudApiDataSource(**rv.json())
+        response_json = rv.json()
+        datasource = next((datasource for datasource in response_json if datasource["id"] == data_source_id), None)
+        if not datasource:
+            raise DataDiffDatasourceIdNotFoundError(
+                f"Datasource ID: {data_source_id} was not found in your Datafold account!"
+            )
+        return TCloudApiDataSource(**datasource)
 
     def create_data_source(self, config: TDsConfig) -> TCloudApiDataSource:
         payload = config.dict()
         if config.type == "bigquery":
             json_string = payload["options"]["jsonKeyFile"].encode("utf-8")
             payload["options"]["jsonKeyFile"] = base64.b64encode(json_string).decode("utf-8")
         rv = self.make_post_request(url="api/v1/data_sources", payload=payload)
@@ -236,33 +244,35 @@
     def create_data_diff(self, payload: TCloudApiDataDiff) -> int:
         rv = self.make_post_request(url="api/v1/datadiffs", payload=payload.dict())
         return rv.json()["id"]
 
     def poll_data_diff_results(self, diff_id: int) -> TCloudApiDataDiffSummaryResult:
         summary_results = None
         start_time = time.monotonic()
-        sleep_interval = 5  # starts at 5 sec
-        max_sleep_interval = 30
+        sleep_interval = 3
+        max_sleep_interval = 20
         max_wait_time = 300
 
         diff_url = f"{self.host}/datadiffs/{diff_id}/overview"
         while not summary_results:
-            logger.debug(f"Polling: {diff_url}")
+            logger.debug("Polling Datafold for results...")
             response = self.make_get_request(url=f"api/v1/datadiffs/{diff_id}/summary_results")
             response_json = response.json()
             if response_json["status"] == "success":
                 summary_results = response_json
             elif response_json["status"] == "failed":
-                raise Exception(f"Diff failed: {str(response_json)}")
+                raise DataDiffCloudDiffFailed(f"Diff failed: {str(response_json)}")
 
             if time.monotonic() - start_time > max_wait_time:
-                raise Exception(f"Timed out waiting for diff results. Please, go to the UI for details: {diff_url}")
+                raise DataDiffCloudDiffTimedOut(
+                    f"Timed out waiting for diff results. Please, go to the UI for details: {diff_url}"
+                )
 
             time.sleep(sleep_interval)
-            sleep_interval = min(sleep_interval * 2, max_sleep_interval)
+            sleep_interval = min(sleep_interval + 1, max_sleep_interval)
 
         return TCloudApiDataDiffSummaryResult.from_orm(summary_results)
 
     def test_data_source(self, data_source_id: int) -> int:
         rv = self.make_post_request(f"api/v1/data_sources/{data_source_id}/test", {})
         return rv.json()["job_id"]
```

### Comparing `data_diff-0.7.9/data_diff/config.py` & `data_diff-0.8.0/data_diff/config.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/databases/_connect.py` & `data_diff-0.8.0/data_diff/databases/_connect.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/dbt.py` & `data_diff-0.8.0/data_diff/dbt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,30 @@
+from contextlib import nullcontext
+import json
 import os
 import re
 import time
-import webbrowser
 from typing import List, Optional, Dict, Tuple, Union
 import keyring
 import pydantic
 import rich
-from rich.prompt import Confirm, Prompt
+from rich.prompt import Prompt
 
-from data_diff.errors import DataDiffCustomSchemaNoConfigError, DataDiffDbtProjectVarsNotFoundError
+from data_diff.errors import (
+    DataDiffCustomSchemaNoConfigError,
+    DataDiffDbtProjectVarsNotFoundError,
+    DataDiffNoAPIKeyError,
+    DataDiffNoDatasourceIdError,
+)
 
 from . import connect_to_table, diff_tables, Algorithm
-from .cloud import DatafoldAPI, TCloudApiDataDiff, TCloudApiOrgMeta, get_or_create_data_source
-from .dbt_parser import DbtParser, PROJECT_FILE, TDatadiffConfig
+from .cloud import DatafoldAPI, TCloudApiDataDiff, TCloudApiOrgMeta
+from .dbt_parser import DbtParser, TDatadiffConfig
+from .diff_tables import DiffResultWrapper
+from .format import jsonify, jsonify_error
 from .tracking import (
     bool_ask_for_email,
     create_email_signup_event_json,
     set_entrypoint_name,
     set_dbt_user_id,
     set_dbt_version,
     set_dbt_project_id,
@@ -31,149 +39,167 @@
     columns_added_template,
     columns_removed_template,
     no_differences_template,
     columns_type_changed_template,
     run_as_daemon,
     truncate_error,
     print_version_info,
+    LogStatusHandler,
 )
 
 logger = getLogger(__name__)
+CLOUD_DOC_URL = "https://docs.datafold.com/development_testing/cloud"
 
 
 class TDiffVars(pydantic.BaseModel):
     dev_path: List[str]
     prod_path: List[str]
     primary_keys: List[str]
     connection: Dict[str, Optional[str]]
     threads: Optional[int] = None
     where_filter: Optional[str] = None
     include_columns: List[str]
     exclude_columns: List[str]
+    dbt_model: Optional[str] = None
 
 
 def dbt_diff(
     profiles_dir_override: Optional[str] = None,
     project_dir_override: Optional[str] = None,
     is_cloud: bool = False,
     dbt_selection: Optional[str] = None,
+    json_output: bool = False,
     state: Optional[str] = None,
+    log_status_handler: Optional[LogStatusHandler] = None,
+    where_flag: Optional[str] = None,
+    columns_flag: Optional[Tuple[str]] = None,
 ) -> None:
     print_version_info()
     diff_threads = []
-    set_entrypoint_name("CLI-dbt")
+    set_entrypoint_name(os.getenv("DATAFOLD_TRIGGERED_BY", "CLI-dbt"))
     dbt_parser = DbtParser(profiles_dir_override, project_dir_override, state)
     models = dbt_parser.get_models(dbt_selection)
     config = dbt_parser.get_datadiff_config()
     _initialize_events(dbt_parser.dbt_user_id, dbt_parser.dbt_version, dbt_parser.dbt_project_id)
 
-
     if not state and not (config.prod_database or config.prod_schema):
         doc_url = "https://docs.datafold.com/development_testing/open_source#configure-your-dbt-project"
         raise DataDiffDbtProjectVarsNotFoundError(
             f"""vars: data_diff: section not found in dbt_project.yml.\n\nTo solve this, please configure your dbt project: \n{doc_url}\n\nOr specify a production manifest using the `--state` flag."""
         )
 
     if is_cloud:
         api = _initialize_api()
         # exit so the user can set the key
         if not api:
             return
         org_meta = api.get_org_meta()
-
         if config.datasource_id is None:
             rich.print("[red]Data source ID not found in dbt_project.yml")
-            is_create_data_source = Confirm.ask("Would you like to create a new data source?")
-            if is_create_data_source:
-                config.datasource_id = get_or_create_data_source(api=api, dbt_parser=dbt_parser)
-                rich.print(f'To use the data source in next runs, please, update your "{PROJECT_FILE}" with a block:')
-                rich.print(f"[green]vars:\n  data_diff:\n    datasource_id: {config.datasource_id}\n")
-                rich.print(
-                    "Read more about Datafold vars in docs: "
-                    "https://docs.datafold.com/os_diff/dbt_integration/#configure-a-data-source\n"
-                )
-            else:
-                raise ValueError(
-                    "Datasource ID not found, include it as a dbt variable in the dbt_project.yml. "
-                    "\nvars:\n data_diff:\n   datasource_id: 1234"
-                )
+            raise DataDiffNoDatasourceIdError(
+                f"Datasource ID not found. Please include it as a dbt variable in the dbt_project.yml. \nInstructions: {CLOUD_DOC_URL}\n\nvars:\n data_diff:\n   datasource_id: 1234"
+            )
 
         data_source = api.get_data_source(config.datasource_id)
         dbt_parser.set_casing_policy_for(connection_type=data_source.type)
         rich.print("[green][bold]\nDiffs in progress...[/][/]\n")
 
     else:
         dbt_parser.set_connection()
 
-    for model in models:
-        diff_vars = _get_diff_vars(dbt_parser, config, model)
-
-        # we won't always have a prod path when using state
-        # when the model DNE in prod manifest, skip the model diff
-        if (
-            state and len(diff_vars.prod_path) < 2
-        ):  # < 2 because some providers like databricks can legitimately have *only* 2
-            diff_output_str = _diff_output_base(".".join(diff_vars.dev_path), ".".join(diff_vars.prod_path))
-            diff_output_str += "[green]New model: nothing to diff![/] \n"
-            rich.print(diff_output_str)
-            continue
-
-        if diff_vars.primary_keys:
-            if is_cloud:
-                diff_thread = run_as_daemon(_cloud_diff, diff_vars, config.datasource_id, api, org_meta)
-                diff_threads.append(diff_thread)
+    with log_status_handler.status if log_status_handler else nullcontext():
+        for model in models:
+            if log_status_handler:
+                log_status_handler.set_prefix(f"Diffing {model.alias} \n")
+
+            diff_vars = _get_diff_vars(dbt_parser, config, model, where_flag, columns_flag)
+
+            # we won't always have a prod path when using state
+            # when the model DNE in prod manifest, skip the model diff
+            if (
+                state and len(diff_vars.prod_path) < 2
+            ):  # < 2 because some providers like databricks can legitimately have *only* 2
+                diff_output_str = _diff_output_base(".".join(diff_vars.dev_path), ".".join(diff_vars.prod_path))
+                diff_output_str += "[green]New model: nothing to diff![/] \n"
+                rich.print(diff_output_str)
+                continue
+
+            if diff_vars.primary_keys:
+                if is_cloud:
+                    diff_thread = run_as_daemon(
+                        _cloud_diff, diff_vars, config.datasource_id, api, org_meta, log_status_handler
+                    )
+                    diff_threads.append(diff_thread)
+                else:
+                    _local_diff(diff_vars, json_output)
             else:
-                _local_diff(diff_vars)
-        else:
-            rich.print(
-                _diff_output_base(".".join(diff_vars.dev_path), ".".join(diff_vars.prod_path))
-                + "Skipped due to unknown primary key. Add uniqueness tests, meta, or tags.\n"
-            )
-
-    # wait for all threads
-    if diff_threads:
-        for thread in diff_threads:
-            thread.join()
+                if json_output:
+                    print(
+                        json.dumps(
+                            jsonify_error(
+                                table1=diff_vars.prod_path,
+                                table2=diff_vars.dev_path,
+                                dbt_model=diff_vars.dbt_model,
+                                error="No primary key found. Add uniqueness tests, meta, or tags.",
+                            )
+                        ),
+                        flush=True,
+                    )
+                else:
+                    rich.print(
+                        _diff_output_base(".".join(diff_vars.dev_path), ".".join(diff_vars.prod_path))
+                        + "Skipped due to unknown primary key. Add uniqueness tests, meta, or tags.\n"
+                    )
+
+        # wait for all threads
+        if diff_threads:
+            for thread in diff_threads:
+                thread.join()
 
 
 def _get_diff_vars(
     dbt_parser: "DbtParser",
     config: TDatadiffConfig,
     model,
+    where_flag: Optional[str] = None,
+    columns_flag: Optional[Tuple[str]] = None,
 ) -> TDiffVars:
+    cli_columns = list(columns_flag) if columns_flag else []
     dev_database = model.database
     dev_schema = model.schema_
-
+    dev_alias = prod_alias = model.alias
     primary_keys = dbt_parser.get_pk_from_model(model, dbt_parser.unique_columns, "primary-key")
 
     # prod path is constructed via configuration or the prod manifest via --state
     if dbt_parser.prod_manifest_obj:
-        prod_database, prod_schema = _get_prod_path_from_manifest(model, dbt_parser.prod_manifest_obj)
+        prod_database, prod_schema, prod_alias = _get_prod_path_from_manifest(model, dbt_parser.prod_manifest_obj)
     else:
         prod_database, prod_schema = _get_prod_path_from_config(config, model, dev_database, dev_schema)
 
     if dbt_parser.requires_upper:
-        dev_qualified_list = [x.upper() for x in [dev_database, dev_schema, model.alias] if x]
-        prod_qualified_list = [x.upper() for x in [prod_database, prod_schema, model.alias] if x]
+        dev_qualified_list = [x.upper() for x in [dev_database, dev_schema, dev_alias] if x]
+        prod_qualified_list = [x.upper() for x in [prod_database, prod_schema, prod_alias] if x]
         primary_keys = [x.upper() for x in primary_keys]
     else:
-        dev_qualified_list = [x for x in [dev_database, dev_schema, model.alias] if x]
-        prod_qualified_list = [x for x in [prod_database, prod_schema, model.alias] if x]
+        dev_qualified_list = [x for x in [dev_database, dev_schema, dev_alias] if x]
+        prod_qualified_list = [x for x in [prod_database, prod_schema, prod_alias] if x]
 
     datadiff_model_config = dbt_parser.get_datadiff_model_config(model.meta)
 
     return TDiffVars(
+        dbt_model=model.unique_id,
         dev_path=dev_qualified_list,
         prod_path=prod_qualified_list,
         primary_keys=primary_keys,
         connection=dbt_parser.connection,
         threads=dbt_parser.threads,
-        where_filter=datadiff_model_config.where_filter,
-        include_columns=datadiff_model_config.include_columns,
-        exclude_columns=datadiff_model_config.exclude_columns,
+        # cli flags take precedence over any model level config
+        where_filter=where_flag or datadiff_model_config.where_filter,
+        include_columns=cli_columns or datadiff_model_config.include_columns,
+        exclude_columns=[] if cli_columns else datadiff_model_config.exclude_columns,
     )
 
 
 def _get_prod_path_from_config(config, model, dev_database, dev_schema) -> Tuple[str, str]:
     # "custom" dbt config database
     if model.config.database:
         prod_database = model.config.database
@@ -198,52 +224,55 @@
         else:
             prod_schema = config.prod_schema
     else:
         prod_schema = dev_schema
     return prod_database, prod_schema
 
 
-def _get_prod_path_from_manifest(model, prod_manifest) -> Union[Tuple[str, str], Tuple[None, None]]:
+def _get_prod_path_from_manifest(model, prod_manifest) -> Union[Tuple[str, str, str], Tuple[None, None, None]]:
     prod_database = None
     prod_schema = None
+    prod_alias = None
     prod_model = prod_manifest.nodes.get(model.unique_id, None)
     if prod_model:
         prod_database = prod_model.database
         prod_schema = prod_model.schema_
-    return prod_database, prod_schema
+        prod_alias = prod_model.alias
+    return prod_database, prod_schema, prod_alias
 
 
-def _local_diff(diff_vars: TDiffVars) -> None:
+def _local_diff(diff_vars: TDiffVars, json_output: bool = False) -> None:
     dev_qualified_str = ".".join(diff_vars.dev_path)
     prod_qualified_str = ".".join(diff_vars.prod_path)
     diff_output_str = _diff_output_base(dev_qualified_str, prod_qualified_str)
 
-    table1 = connect_to_table(diff_vars.connection, dev_qualified_str, tuple(diff_vars.primary_keys), diff_vars.threads)
-    table2 = connect_to_table(
+    table1 = connect_to_table(
         diff_vars.connection, prod_qualified_str, tuple(diff_vars.primary_keys), diff_vars.threads
     )
+    table2 = connect_to_table(diff_vars.connection, dev_qualified_str, tuple(diff_vars.primary_keys), diff_vars.threads)
 
-    table1_columns = table1.get_schema()
     try:
-        table2_columns = table2.get_schema()
+        table1_columns = table1.get_schema()
     # Not ideal, but we don't have more specific exceptions yet
     except Exception as ex:
         logger.debug(ex)
         diff_output_str += "[red]New model or no access to prod table.[/] \n"
         rich.print(diff_output_str)
         return
 
+    table2_columns = table2.get_schema()
+
     table1_column_names = set(table1_columns.keys())
     table2_column_names = set(table2_columns.keys())
     column_set = table1_column_names.intersection(table2_column_names)
-    columns_added = table1_column_names.difference(table2_column_names)
-    columns_removed = table2_column_names.difference(table1_column_names)
+    columns_added = table2_column_names.difference(table1_column_names)
+    columns_removed = table1_column_names.difference(table2_column_names)
     # col type is i = 1 in tuple
     columns_type_changed = {
-        k for k, v in table1_columns.items() if k in table2_columns and v[1] != table2_columns[k][1]
+        k for k, v in table2_columns.items() if k in table1_columns and v[1] != table1_columns[k][1]
     }
 
     if columns_added:
         diff_output_str += columns_added_template(columns_added)
 
     if columns_removed:
         diff_output_str += columns_removed_template(columns_removed)
@@ -258,23 +287,62 @@
         column_set = {x for x in column_set if x.upper() in [y.upper() for y in diff_vars.include_columns]}
 
     if diff_vars.exclude_columns:
         column_set = {x for x in column_set if x.upper() not in [y.upper() for y in diff_vars.exclude_columns]}
 
     extra_columns = tuple(column_set)
 
-    diff = diff_tables(
+    diff: DiffResultWrapper = diff_tables(
         table1,
         table2,
         threaded=True,
         algorithm=Algorithm.JOINDIFF,
         extra_columns=extra_columns,
         where=diff_vars.where_filter,
         skip_null_keys=True,
     )
+    if json_output:
+        # drain the iterator to get accumulated stats in diff.info_tree
+        try:
+            list(diff)
+        except Exception as e:
+            print(
+                json.dumps(
+                    jsonify_error(list(table1.table_path), list(table2.table_path), diff_vars.dbt_model, str(e))
+                ),
+                flush=True,
+            )
+            return
+
+        dataset1_columns = [
+            (name, type_, table1.database.dialect.parse_type(table1.table_path, name, type_, *other))
+            for (name, type_, *other) in table1_columns.values()
+        ]
+        dataset2_columns = [
+            (name, type_, table2.database.dialect.parse_type(table2.table_path, name, type_, *other))
+            for (name, type_, *other) in table2_columns.values()
+        ]
+        print(
+            json.dumps(
+                jsonify(
+                    diff,
+                    dbt_model=diff_vars.dbt_model,
+                    dataset1_columns=dataset1_columns,
+                    dataset2_columns=dataset2_columns,
+                    with_summary=True,
+                    columns_diff={
+                        "added": columns_added,
+                        "removed": columns_removed,
+                        "changed": columns_type_changed,
+                    },
+                )
+            ),
+            flush=True,
+        )
+        return
 
     if list(diff):
         diff_output_str += f"{diff.get_stats_string(is_dbt=True)} \n"
         rich.print(diff_output_str)
     else:
         diff_output_str += no_differences_template()
         rich.print(diff_output_str)
@@ -288,34 +356,35 @@
     rich.print(f"Cloud datafold host: {datafold_host}")
 
     api_key = os.environ.get("DATAFOLD_API_KEY")
     if not api_key:
         rich.print("[red]API key not found. Getting from the keyring service")
         api_key = keyring.get_password("data-diff", "DATAFOLD_API_KEY")
         if not api_key:
-            rich.print("[red]API key not found, add it as an environment variable called DATAFOLD_API_KEY.")
-
-            yes_or_no = Confirm.ask("Would you like to generate a new API key?")
-            if yes_or_no:
-                webbrowser.open(f"{datafold_host}/login?next={datafold_host}/users/me")
-                rich.print('After generating, please, perform in the terminal "export DATAFOLD_API_KEY=<key>"')
-                return None
-            else:
-                raise ValueError("Cannot initialize API because the API key is not provided")
-
+            raise DataDiffNoAPIKeyError(
+                f"API key not found. Please follow the steps at {CLOUD_DOC_URL} to use the --cloud flag."
+            )
     rich.print("Saving the API key to the system keyring service")
     try:
         keyring.set_password("data-diff", "DATAFOLD_API_KEY", api_key)
     except Exception as e:
         rich.print(f"[red]Failed when saving the API key to the system keyring service. Reason: {e}")
 
     return DatafoldAPI(api_key=api_key, host=datafold_host)
 
 
-def _cloud_diff(diff_vars: TDiffVars, datasource_id: int, api: DatafoldAPI, org_meta: TCloudApiOrgMeta) -> None:
+def _cloud_diff(
+    diff_vars: TDiffVars,
+    datasource_id: int,
+    api: DatafoldAPI,
+    org_meta: TCloudApiOrgMeta,
+    log_status_handler: Optional[LogStatusHandler] = None,
+) -> None:
+    if log_status_handler:
+        log_status_handler.cloud_diff_started(diff_vars.dev_path[-1])
     diff_output_str = _diff_output_base(".".join(diff_vars.dev_path), ".".join(diff_vars.prod_path))
     payload = TCloudApiDataDiff(
         data_source1_id=datasource_id,
         data_source2_id=datasource_id,
         table1=diff_vars.prod_path,
         table2=diff_vars.dev_path,
         pk_columns=diff_vars.primary_keys,
@@ -376,14 +445,16 @@
             )
             diff_output_str += f"\n{diff_url}\n {diff_output} \n"
             rich.print(diff_output_str)
         else:
             diff_output_str += f"\n{diff_url}\n{no_differences_template()}\n"
             rich.print(diff_output_str)
 
+        if log_status_handler:
+            log_status_handler.cloud_diff_finished(diff_vars.dev_path[-1])
     except BaseException as ex:  # Catch KeyboardInterrupt too
         error = ex
     finally:
         # we don't currently have much of this information
         # but I imagine a future iteration of this _cloud method
         # will poll for results
         if is_tracking_enabled():
@@ -421,15 +492,15 @@
     set_dbt_user_id(dbt_user_id)
     set_dbt_version(dbt_version)
     set_dbt_project_id(dbt_project_id)
     _email_signup()
 
 
 def _email_signup() -> None:
-    email_regex = r'^[\w\.\+-]+@[\w\.-]+\.\w+$'
+    email_regex = r"^[\w\.\+-]+@[\w\.-]+\.\w+$"
     prompt = "\nWould you like to be notified when a new data-diff version is available?\n\nEnter email or leave blank to opt out (we'll only ask once).\n"
 
     if bool_ask_for_email():
         while True:
             email_input = Prompt.ask(
                 prompt=prompt,
                 default="",
```

### Comparing `data_diff-0.7.9/data_diff/dbt_parser.py` & `data_diff-0.8.0/data_diff/dbt_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,14 @@
         self,
         profiles_dir_override: Optional[str] = None,
         project_dir_override: Optional[str] = None,
         state: Optional[str] = None,
     ) -> None:
         try_set_dbt_flags()
         self.dbt_runner = try_get_dbt_runner()
-        self.profiles_dir = Path(profiles_dir_override or default_profiles_dir())
         self.project_dir = Path(project_dir_override or default_project_dir())
         self.connection = {}
         self.project_dict = self.get_project_dict()
         self.dev_manifest_obj = self.get_manifest_obj(self.project_dir / MANIFEST_PATH)
         self.prod_manifest_obj = None
         if state:
             self.prod_manifest_obj = self.get_manifest_obj(Path(state))
@@ -115,14 +114,21 @@
         self.dbt_user_id = self.dev_manifest_obj.metadata.user_id
         self.dbt_version = self.dev_manifest_obj.metadata.dbt_version
         self.dbt_project_id = self.dev_manifest_obj.metadata.project_id
         self.requires_upper = False
         self.threads = None
         self.unique_columns = self.get_unique_columns()
 
+        if profiles_dir_override:
+            self.profiles_dir = Path(profiles_dir_override)
+        elif parse_version(self.dbt_version) < parse_version("1.3.0"):
+            self.profiles_dir = legacy_profiles_dir()
+        else:
+            self.profiles_dir = default_profiles_dir()
+
     def get_datadiff_config(self) -> TDatadiffConfig:
         data_diff_vars = self.project_dict.get("vars", {}).get("data_diff", {})
         prod_database = data_diff_vars.get("prod_database")
         prod_schema = data_diff_vars.get("prod_schema")
         prod_custom_schema = data_diff_vars.get("prod_custom_schema")
         datasource_id = data_diff_vars.get("datasource_id")
         config = TDatadiffConfig(
@@ -207,17 +213,14 @@
         with open(self.project_dir / RUN_RESULTS_PATH) as run_results:
             logger.info(f"Parsing file {RUN_RESULTS_PATH}")
             run_results_dict = json.load(run_results)
             run_results_obj = parse_run_results(run_results=run_results_dict)
 
         dbt_version = parse_version(run_results_obj.metadata.dbt_version)
 
-        if dbt_version < parse_version("1.3.0"):
-            self.profiles_dir = legacy_profiles_dir()
-
         if dbt_version < parse_version(LOWER_DBT_V):
             raise DataDiffDbtRunResultsVersionError(
                 f"Found dbt: v{dbt_version} Expected the dbt project's version to be >= {LOWER_DBT_V}"
             )
         if dbt_version >= parse_version(UPPER_DBT_V):
             logger.warning(
                 f"{dbt_version} is a recent version of dbt and may not be fully tested with data-diff! \nPlease report any issues to https://github.com/datafold/data-diff/issues"
@@ -254,43 +257,46 @@
         dbt_profile_var = self.project_dict.get("profile")
 
         profile = get_from_dict_with_raise(
             profiles,
             dbt_profile_var,
             DataDiffDbtProfileNotFoundError(f"No profile '{dbt_profile_var}' found in '{profiles_path}'."),
         )
-        # values can contain env_vars
-        rendered_profile = ProfileRenderer().render_data(profile)
         profile_target = get_from_dict_with_raise(
-            rendered_profile,
+            profile,
             "target",
             DataDiffDbtProfileNotFoundError(f"No target found in profile '{dbt_profile_var}' in '{profiles_path}'."),
         )
+
+        # some use an env var in target:
+        rendered_profile_target = ProfileRenderer().render_data(profile_target)
+
         outputs = get_from_dict_with_raise(
-            rendered_profile,
+            profile,
             "outputs",
             DataDiffDbtProfileNotFoundError(f"No outputs found in profile '{dbt_profile_var}' in '{profiles_path}'."),
         )
         credentials = get_from_dict_with_raise(
             outputs,
-            profile_target,
+            rendered_profile_target,
             DataDiffDbtProfileNotFoundError(
-                f"No credentials found for target '{profile_target}' in profile '{dbt_profile_var}' in '{profiles_path}'."
+                f"No credentials found for target '{rendered_profile_target}' in profile '{dbt_profile_var}' in '{profiles_path}'."
             ),
         )
         conn_type = get_from_dict_with_raise(
             credentials,
             "type",
             DataDiffDbtProfileNotFoundError(
-                f"No type found for target '{profile_target}' in profile '{dbt_profile_var}' in '{profiles_path}'."
+                f"No type found for target '{rendered_profile_target}' in profile '{dbt_profile_var}' in '{profiles_path}'."
             ),
         )
         conn_type = conn_type.lower()
 
-        return credentials, conn_type
+        # resolve any jinja
+        return ProfileRenderer().render_data(credentials), conn_type
 
     def set_connection(self):
         credentials, conn_type = self.get_connection_creds()
         self.set_casing_policy_for(conn_type)
 
         if conn_type == "snowflake":
             conn_info = {
```

### Comparing `data_diff-0.7.9/data_diff/diff_tables.py` & `data_diff-0.8.0/data_diff/diff_tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,16 +136,16 @@
         return DiffStats(diff_by_sign, table1_count, table2_count, unchanged, diff_percent, extra_column_diffs)
 
     def get_stats_string(self, is_dbt: bool = False):
         diff_stats = self._get_stats(is_dbt)
 
         if is_dbt:
             string_output = dbt_diff_string_template(
-                diff_stats.diff_by_sign["-"],
                 diff_stats.diff_by_sign["+"],
+                diff_stats.diff_by_sign["-"],
                 diff_stats.diff_by_sign["!"],
                 diff_stats.unchanged,
                 diff_stats.extra_column_diffs,
                 "Values Updated:",
             )
 
         else:
@@ -161,27 +161,27 @@
             if self.stats:
                 string_output += "\nExtra-Info:\n"
                 for k, v in sorted(self.stats.items()):
                     string_output += f"  {k} = {v}\n"
 
         return string_output
 
-    def get_stats_dict(self):
-        diff_stats = self._get_stats()
+    def get_stats_dict(self, is_dbt: bool = False):
+        diff_stats = self._get_stats(is_dbt)
         json_output = {
             "rows_A": diff_stats.table1_count,
             "rows_B": diff_stats.table2_count,
             "exclusive_A": diff_stats.diff_by_sign["-"],
             "exclusive_B": diff_stats.diff_by_sign["+"],
             "updated": diff_stats.diff_by_sign["!"],
             "unchanged": diff_stats.unchanged,
             "total": sum(diff_stats.diff_by_sign.values()),
             "stats": self.stats,
         }
-
+        json_output["values"] = diff_stats.extra_column_diffs or {}
         return json_output
 
 
 class TableDiffer(ThreadBase, ABC):
     bisection_factor = 32
     stats: dict = {}
```

### Comparing `data_diff-0.7.9/data_diff/errors.py` & `data_diff-0.8.0/data_diff/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,7 +44,27 @@
 
 class DataDiffDbtSelectVersionTooLowError(Exception):
     "Raised when attempting to use `--select` with a dbt-core version < 1.5."
 
 
 class DataDiffCustomSchemaNoConfigError(Exception):
     "Raised when a model has a custom schema, but there is no prod_custom_schema config. (And not using --state)."
+
+
+class DataDiffNoAPIKeyError(Exception):
+    "Raised when using --cloud but no API key is present in the DATAFOLD_API_KEY env var or keyring"
+
+
+class DataDiffNoDatasourceIdError(Exception):
+    "Raised when using --cloud but no datasource_id was found in dbt_project.yml"
+
+
+class DataDiffDatasourceIdNotFoundError(Exception):
+    "Raised when using --cloud but the datasource_id is not found for a particular org."
+
+
+class DataDiffCloudDiffFailed(Exception):
+    "Raised when using --cloud and the remote diff fails."
+
+
+class DataDiffCloudDiffTimedOut(Exception):
+    "Raised when using --cloud and the diff did not return finish before the timeout value."
```

### Comparing `data_diff-0.7.9/data_diff/hashdiff_tables.py` & `data_diff-0.8.0/data_diff/hashdiff_tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,18 @@
     warned_diff_cols = set()
     for _k, v in sorted(d.items(), key=lambda i: i[0]):
         if json_cols:
             parsed_match, overriden_diff_cols = diffs_are_equiv_jsons(v, json_cols)
             if parsed_match:
                 to_warn = overriden_diff_cols - warned_diff_cols
                 for w in to_warn:
-                    logger.warning(f"Equivalent JSON objects with different string representations detected "
-                                   f"in column '{w}'. These cases are NOT reported as differences.")
+                    logger.warning(
+                        f"Equivalent JSON objects with different string representations detected "
+                        f"in column '{w}'. These cases are NOT reported as differences."
+                    )
                     warned_diff_cols.add(w)
                 continue
         yield from v
 
 
 @dataclass
 class HashDiffer(TableDiffer):
@@ -200,16 +202,19 @@
             max_rows = max_space_size
             info_tree.info.max_rows = max_rows
 
         # If count is below the threshold, just download and compare the columns locally
         # This saves time, as bisection speed is limited by ping and query performance.
         if max_rows < self.bisection_threshold or max_space_size < self.bisection_factor * 2:
             rows1, rows2 = self._threaded_call("get_values", [table1, table2])
-            json_cols = {i: colname for i, colname in enumerate(table1.extra_columns)
-                         if isinstance(table1._schema[colname], JSON)}
+            json_cols = {
+                i: colname
+                for i, colname in enumerate(table1.extra_columns)
+                if isinstance(table1._schema[colname], JSON)
+            }
             diff = list(diff_sets(rows1, rows2, json_cols))
 
             info_tree.info.set_diff(diff)
             info_tree.info.rowcounts = {1: len(rows1), 2: len(rows2)}
 
             logger.info(". " * level + f"Diff found {len(diff)} different rows.")
             self.stats["rows_downloaded"] = self.stats.get("rows_downloaded", 0) + max(len(rows1), len(rows2))
```

### Comparing `data_diff-0.7.9/data_diff/joindiff_tables.py` & `data_diff-0.8.0/data_diff/joindiff_tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,15 +202,15 @@
             )
             if self.materialize_to_table
             else None,
         ):
             assert len(a_cols) == len(b_cols)
             logger.debug("Querying for different rows")
             diff = db.query(diff_rows, list)
-            info_tree.info.set_diff(diff)
+            info_tree.info.set_diff(diff, schema=tuple(diff_rows.schema.items()))
             for is_xa, is_xb, *x in diff:
                 if is_xa and is_xb:
                     # Can't both be exclusive, meaning a pk is NULL
                     # This can happen if the explicit null test didn't finish running yet
                     if self.skip_null_keys:
                         # warning is thrown in explicit null test
                         continue
```

### Comparing `data_diff-0.7.9/data_diff/lexicographic_space.py` & `data_diff-0.8.0/data_diff/lexicographic_space.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/parse_time.py` & `data_diff-0.8.0/data_diff/parse_time.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/query_utils.py` & `data_diff-0.8.0/data_diff/query_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/sqeleton/abcs/database_types.py` & `data_diff-0.8.0/data_diff/sqeleton/abcs/database_types.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/sqeleton/abcs/mixins.py` & `data_diff-0.8.0/data_diff/sqeleton/abcs/mixins.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 from abc import ABC, abstractmethod
-from .database_types import Array, TemporalType, FractionalType, ColType_UUID, Boolean, ColType, String_UUID, JSON, Struct
+from .database_types import (
+    Array,
+    TemporalType,
+    FractionalType,
+    ColType_UUID,
+    Boolean,
+    ColType,
+    String_UUID,
+    JSON,
+    Struct,
+)
 from .compiler import Compilable
 
 
 class AbstractMixin(ABC):
     "A mixin for a database dialect"
 
 
 class AbstractMixin_NormalizeValue(AbstractMixin):
-
     @abstractmethod
     def to_comparable(self, value: str, coltype: ColType) -> str:
         """Ensure that the expression is comparable in ``IS DISTINCT FROM``."""
 
     @abstractmethod
     def normalize_timestamp(self, value: str, coltype: TemporalType) -> str:
         """Creates an SQL expression, that converts 'value' to a normalized timestamp.
```

### Comparing `data_diff-0.7.9/data_diff/sqeleton/bound_exprs.py` & `data_diff-0.8.0/data_diff/sqeleton/bound_exprs.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/sqeleton/databases/__init__.py` & `data_diff-0.8.0/data_diff/sqeleton/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/sqeleton/databases/_connect.py` & `data_diff-0.8.0/data_diff/sqeleton/databases/_connect.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/sqeleton/databases/base.py` & `data_diff-0.8.0/data_diff/sqeleton/databases/base.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/sqeleton/databases/bigquery.py` & `data_diff-0.8.0/data_diff/sqeleton/databases/bigquery.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/sqeleton/databases/clickhouse.py` & `data_diff-0.8.0/data_diff/sqeleton/databases/clickhouse.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/sqeleton/databases/databricks.py` & `data_diff-0.8.0/data_diff/sqeleton/databases/databricks.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/sqeleton/databases/duckdb.py` & `data_diff-0.8.0/data_diff/sqeleton/databases/duckdb.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/sqeleton/databases/mssql.py` & `data_diff-0.8.0/data_diff/sqeleton/databases/mssql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/sqeleton/databases/mysql.py` & `data_diff-0.8.0/data_diff/sqeleton/databases/mysql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/sqeleton/databases/oracle.py` & `data_diff-0.8.0/data_diff/sqeleton/databases/oracle.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/sqeleton/databases/postgresql.py` & `data_diff-0.8.0/data_diff/sqeleton/databases/postgresql.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,14 @@
         "numeric": Decimal,
         "bigint": Integer,
         # Text
         "character": Text,
         "character varying": Text,
         "varchar": Text,
         "text": Text,
-
         "json": JSON,
         "jsonb": JSON,
         "uuid": Native_UUID,
         "boolean": Boolean,
     }
 
     def quote(self, s: str):
```

### Comparing `data_diff-0.7.9/data_diff/sqeleton/databases/presto.py` & `data_diff-0.8.0/data_diff/sqeleton/databases/presto.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/sqeleton/databases/redshift.py` & `data_diff-0.8.0/data_diff/sqeleton/databases/redshift.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             f"RPAD(LEFT({timestamp6}, {TIMESTAMP_PRECISION_POS+coltype.precision}), {TIMESTAMP_PRECISION_POS+6}, '0')"
         )
 
     def normalize_number(self, value: str, coltype: FractionalType) -> str:
         return self.to_string(f"{value}::decimal(38,{coltype.precision})")
 
     def normalize_json(self, value: str, _coltype: JSON) -> str:
-        return f'nvl2({value}, json_serialize({value}), NULL)'
+        return f"nvl2({value}, json_serialize({value}), NULL)"
 
 
 class Dialect(PostgresqlDialect):
     name = "Redshift"
     TYPE_CLASSES = {
         **PostgresqlDialect.TYPE_CLASSES,
         "double": Float,
@@ -119,37 +119,37 @@
         d = {r[0]: r for r in rows}
         assert len(d) == len(rows)
         return d
 
     def select_view_columns(self, path: DbPath) -> str:
         _, schema, table = self._normalize_table_path(path)
 
-        return (
-            """select * from pg_get_cols('{}.{}')
+        return """select * from pg_get_cols('{}.{}')
                 cols(view_schema name, view_name name, col_name name, col_type varchar, col_num int)
-            """.format(schema, table)
+            """.format(
+            schema, table
         )
 
     def query_pg_get_cols(self, path: DbPath) -> Dict[str, tuple]:
         rows = self.query(self.select_view_columns(path), list)
 
         if not rows:
             raise RuntimeError(f"{self.name}: View '{'.'.join(path)}' does not exist, or has no columns")
 
         output = {}
         for r in rows:
             col_name = r[2]
-            type_info = r[3].split('(')
+            type_info = r[3].split("(")
             base_type = type_info[0]
             precision = None
             scale = None
 
             if len(type_info) > 1:
-                if base_type == 'numeric':
-                    precision, scale = type_info[1][:-1].split(',')
+                if base_type == "numeric":
+                    precision, scale = type_info[1][:-1].split(",")
                     precision = int(precision)
                     scale = int(scale)
 
             out = [col_name, base_type, None, precision, scale]
             output[col_name] = tuple(out)
 
         return output
```

### Comparing `data_diff-0.7.9/data_diff/sqeleton/databases/snowflake.py` & `data_diff-0.8.0/data_diff/sqeleton/databases/snowflake.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/sqeleton/databases/trino.py` & `data_diff-0.8.0/data_diff/sqeleton/databases/trino.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/sqeleton/databases/vertica.py` & `data_diff-0.8.0/data_diff/sqeleton/databases/vertica.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/sqeleton/queries/api.py` & `data_diff-0.8.0/data_diff/sqeleton/queries/api.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/sqeleton/queries/ast_classes.py` & `data_diff-0.8.0/data_diff/sqeleton/queries/ast_classes.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/sqeleton/queries/compiler.py` & `data_diff-0.8.0/data_diff/sqeleton/queries/compiler.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/sqeleton/queries/extras.py` & `data_diff-0.8.0/data_diff/sqeleton/queries/extras.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/sqeleton/query_utils.py` & `data_diff-0.8.0/data_diff/sqeleton/query_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/sqeleton/repl.py` & `data_diff-0.8.0/data_diff/sqeleton/repl.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/sqeleton/schema.py` & `data_diff-0.8.0/data_diff/sqeleton/schema.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/sqeleton/utils.py` & `data_diff-0.8.0/data_diff/sqeleton/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,15 +320,14 @@
 def match_like(pattern: str, strs: Sequence[str]) -> Iterable[str]:
     reo = re.compile(pattern.replace("%", ".*").replace("?", ".") + "$")
     for s in strs:
         if reo.match(s):
             yield s
 
 
-
 class UnknownMeta(type):
     def __instancecheck__(self, instance):
         return instance is Unknown
 
     def __repr__(self):
         return "Unknown"
```

### Comparing `data_diff-0.7.9/data_diff/table_segment.py` & `data_diff-0.8.0/data_diff/table_segment.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/thread_utils.py` & `data_diff-0.8.0/data_diff/thread_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/tracking.py` & `data_diff-0.8.0/data_diff/tracking.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.9/data_diff/utils.py` & `data_diff-0.8.0/data_diff/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import operator
 import threading
 from datetime import datetime
 from packaging.version import parse as parse_version
 import requests
 from tabulate import tabulate
 from .version import __version__
+from rich.status import Status
 
 
 def safezip(*args):
     "zip but makes sure all sequences are the same length"
     lens = list(map(len, args))
     if len(set(lens)) != 1:
         raise ValueError(f"Mismatching lengths in arguments to safezip: {lens}")
@@ -207,7 +208,43 @@
     except Exception as ex:
         logger.debug(f"Failed checking version: {ex}")
 
     if latest_version and parse_version(__version__) < parse_version(latest_version):
         print(f"{base_version_string} (Update {latest_version} is available!)")
     else:
         print(base_version_string)
+
+
+class LogStatusHandler(logging.Handler):
+    """
+    This log handler can be used to update a rich.status every time a log is emitted.
+    """
+
+    def __init__(self):
+        super().__init__()
+        self.status = Status("")
+        self.prefix = ""
+        self.cloud_diff_status = {}
+
+    def emit(self, record):
+        log_entry = self.format(record)
+        if self.cloud_diff_status:
+            self._update_cloud_status(log_entry)
+        else:
+            self.status.update(self.prefix + log_entry)
+
+    def set_prefix(self, prefix_string):
+        self.prefix = prefix_string
+
+    def cloud_diff_started(self, model_name):
+        self.cloud_diff_status[model_name] = "[yellow]In Progress[/]"
+        self._update_cloud_status()
+
+    def cloud_diff_finished(self, model_name):
+        self.cloud_diff_status[model_name] = "[green]Finished   [/]"
+        self._update_cloud_status()
+
+    def _update_cloud_status(self, log=None):
+        cloud_status_string = "\n"
+        for model_name, status in self.cloud_diff_status.items():
+            cloud_status_string += f"{status} {model_name}\n"
+        self.status.update(f"{cloud_status_string}{log or ''}")
```

### Comparing `data_diff-0.7.9/pyproject.toml` & `data_diff-0.8.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-diff"
-version = "0.7.9"
+version = "0.8.0"
 description = "Command-line tool and Python library to efficiently diff rows across two different databases."
 authors = ["Datafold <data-diff@datafold.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/datafold/data-diff"
 documentation = ""
 classifiers = [
@@ -21,18 +21,15 @@
     "Typing :: Typed"
 ]
 packages = [{ include = "data_diff" }]
 
 [tool.poetry.dependencies]
 python = "^3.7.2"
 runtype = "^0.2.6"
-dsnparse = [
-    { version = "<0.2.0", markers = "python_version < '3.8.0'" },
-    { version = "*", markers = "python_version >= '3.8.0'" }
-]
+dsnparse = "<0.2.0"
 click = "^8.1"
 rich = "*"
 toml = "^0.10.2"
 mysql-connector-python = {version="8.0.29", optional=true}
 psycopg2 = {version="*", optional=true}
 snowflake-connector-python = {version = ">=3.0.2,<4.0.0", optional=true}
 cryptography = {version="*", optional=true}
```

### Comparing `data_diff-0.7.9/PKG-INFO` & `data_diff-0.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6461 7461  : 2.1.Name: data
 00000020: 2d64 6966 660a 5665 7273 696f 6e3a 2030  -diff.Version: 0
-00000030: 2e37 2e39 0a53 756d 6d61 7279 3a20 436f  .7.9.Summary: Co
+00000030: 2e38 2e30 0a53 756d 6d61 7279 3a20 436f  .8.0.Summary: Co
 00000040: 6d6d 616e 642d 6c69 6e65 2074 6f6f 6c20  mmand-line tool 
 00000050: 616e 6420 5079 7468 6f6e 206c 6962 7261  and Python libra
 00000060: 7279 2074 6f20 6566 6669 6369 656e 746c  ry to efficientl
 00000070: 7920 6469 6666 2072 6f77 7320 6163 726f  y diff rows acro
 00000080: 7373 2074 776f 2064 6966 6665 7265 6e74  ss two different
 00000090: 2064 6174 6162 6173 6573 2e0a 486f 6d65   databases..Home
 000000a0: 2d70 6167 653a 2068 7474 7073 3a2f 2f67  -page: https://g
@@ -100,232 +100,230 @@
 00000630: 7569 7265 732d 4469 7374 3a20 6462 742d  uires-Dist: dbt-
 00000640: 6172 7469 6661 6374 732d 7061 7273 6572  artifacts-parser
 00000650: 2028 3e3d 302e 332e 302c 3c30 2e34 2e30   (>=0.3.0,<0.4.0
 00000660: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
 00000670: 2064 6274 2d63 6f72 6520 283e 3d31 2e30   dbt-core (>=1.0
 00000680: 2e30 2c3c 322e 302e 3029 0a52 6571 7569  .0,<2.0.0).Requi
 00000690: 7265 732d 4469 7374 3a20 6473 6e70 6172  res-Dist: dsnpar
-000006a0: 7365 2028 3c30 2e32 2e30 2920 3b20 7079  se (<0.2.0) ; py
-000006b0: 7468 6f6e 5f76 6572 7369 6f6e 203c 2022  thon_version < "
-000006c0: 332e 382e 3022 0a52 6571 7569 7265 732d  3.8.0".Requires-
-000006d0: 4469 7374 3a20 6473 6e70 6172 7365 203b  Dist: dsnparse ;
-000006e0: 2070 7974 686f 6e5f 7665 7273 696f 6e20   python_version 
-000006f0: 3e3d 2022 332e 382e 3022 0a52 6571 7569  >= "3.8.0".Requi
-00000700: 7265 732d 4469 7374 3a20 6475 636b 6462  res-Dist: duckdb
-00000710: 2028 3e3d 302e 372e 302c 3c30 2e38 2e30   (>=0.7.0,<0.8.0
-00000720: 2920 3b20 6578 7472 6120 3d3d 2022 6475  ) ; extra == "du
-00000730: 636b 6462 220a 5265 7175 6972 6573 2d44  ckdb".Requires-D
-00000740: 6973 743a 206b 6579 7269 6e67 0a52 6571  ist: keyring.Req
-00000750: 7569 7265 732d 4469 7374 3a20 6d79 7371  uires-Dist: mysq
-00000760: 6c2d 636f 6e6e 6563 746f 722d 7079 7468  l-connector-pyth
-00000770: 6f6e 2028 3d3d 382e 302e 3239 2920 3b20  on (==8.0.29) ; 
-00000780: 6578 7472 6120 3d3d 2022 6d79 7371 6c22  extra == "mysql"
-00000790: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000007a0: 7072 6571 6c20 283e 3d30 2e32 2e31 392c  preql (>=0.2.19,
-000007b0: 3c30 2e33 2e30 2920 3b20 6578 7472 6120  <0.3.0) ; extra 
-000007c0: 3d3d 2022 7072 6571 6c22 0a52 6571 7569  == "preql".Requi
-000007d0: 7265 732d 4469 7374 3a20 7072 6573 746f  res-Dist: presto
-000007e0: 2d70 7974 686f 6e2d 636c 6965 6e74 203b  -python-client ;
-000007f0: 2065 7874 7261 203d 3d20 2270 7265 7374   extra == "prest
-00000800: 6f22 0a52 6571 7569 7265 732d 4469 7374  o".Requires-Dist
-00000810: 3a20 7073 7963 6f70 6732 203b 2065 7874  : psycopg2 ; ext
-00000820: 7261 203d 3d20 2270 6f73 7467 7265 7371  ra == "postgresq
-00000830: 6c22 206f 7220 6578 7472 6120 3d3d 2022  l" or extra == "
-00000840: 7265 6473 6869 6674 220a 5265 7175 6972  redshift".Requir
-00000850: 6573 2d44 6973 743a 2072 6963 680a 5265  es-Dist: rich.Re
-00000860: 7175 6972 6573 2d44 6973 743a 2072 756e  quires-Dist: run
-00000870: 7479 7065 2028 3e3d 302e 322e 362c 3c30  type (>=0.2.6,<0
-00000880: 2e33 2e30 290a 5265 7175 6972 6573 2d44  .3.0).Requires-D
-00000890: 6973 743a 2073 6e6f 7766 6c61 6b65 2d63  ist: snowflake-c
-000008a0: 6f6e 6e65 6374 6f72 2d70 7974 686f 6e20  onnector-python 
-000008b0: 283e 3d33 2e30 2e32 2c3c 342e 302e 3029  (>=3.0.2,<4.0.0)
-000008c0: 203b 2065 7874 7261 203d 3d20 2273 6e6f   ; extra == "sno
-000008d0: 7766 6c61 6b65 220a 5265 7175 6972 6573  wflake".Requires
-000008e0: 2d44 6973 743a 2074 6162 756c 6174 6520  -Dist: tabulate 
-000008f0: 283e 3d30 2e39 2e30 2c3c 302e 3130 2e30  (>=0.9.0,<0.10.0
-00000900: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
-00000910: 2074 6f6d 6c20 283e 3d30 2e31 302e 322c   toml (>=0.10.2,
-00000920: 3c30 2e31 312e 3029 0a52 6571 7569 7265  <0.11.0).Require
-00000930: 732d 4469 7374 3a20 7472 696e 6f20 283e  s-Dist: trino (>
-00000940: 3d30 2e33 3134 2e30 2c3c 302e 3331 352e  =0.314.0,<0.315.
-00000950: 3029 203b 2065 7874 7261 203d 3d20 2274  0) ; extra == "t
-00000960: 7269 6e6f 220a 5265 7175 6972 6573 2d44  rino".Requires-D
-00000970: 6973 743a 2075 726c 6c69 6233 2028 3c32  ist: urllib3 (<2
-00000980: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
-00000990: 2076 6572 7469 6361 2d70 7974 686f 6e20   vertica-python 
-000009a0: 3b20 6578 7472 6120 3d3d 2022 7665 7274  ; extra == "vert
-000009b0: 6963 6122 0a50 726f 6a65 6374 2d55 524c  ica".Project-URL
-000009c0: 3a20 5265 706f 7369 746f 7279 2c20 6874  : Repository, ht
-000009d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000009e0: 2f64 6174 6166 6f6c 642f 6461 7461 2d64  /datafold/data-d
-000009f0: 6966 660a 4465 7363 7269 7074 696f 6e2d  iff.Description-
-00000a00: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
-00000a10: 7874 2f6d 6172 6b64 6f77 6e0a 0a3c 7020  xt/markdown..<p 
-00000a20: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
-00000a30: 2020 2020 3c69 6d67 2061 6c74 3d22 4461      <img alt="Da
-00000a40: 7461 666f 6c64 2220 7372 633d 2268 7474  tafold" src="htt
-00000a50: 7073 3a2f 2f75 7365 722d 696d 6167 6573  ps://user-images
-00000a60: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00000a70: 6e74 2e63 6f6d 2f31 3739 3939 3331 2f31  nt.com/1799931/1
-00000a80: 3936 3439 3731 3130 2d64 3364 6531 3131  96497110-d3de111
-00000a90: 332d 6139 3766 2d34 3332 322d 6235 3331  3-a97f-4322-b531
-00000aa0: 2d30 3236 6438 3539 6238 3637 612e 706e  -026d859b867a.pn
-00000ab0: 6722 2077 6964 7468 3d22 3530 2522 202f  g" width="50%" /
-00000ac0: 3e0a 3c2f 703e 0a0a 3c68 3120 616c 6967  >.</p>..<h1 alig
-00000ad0: 6e3d 2263 656e 7465 7222 3e0a 6461 7461  n="center">.data
-00000ae0: 2d64 6966 660a 3c2f 6831 3e0a 0a3c 6832  -diff.</h1>..<h2
-00000af0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
-00000b00: 0a44 6576 656c 6f70 2064 6274 206d 6f64  .Develop dbt mod
-00000b10: 656c 7320 6661 7374 6572 2062 7920 7465  els faster by te
-00000b20: 7374 696e 6720 6173 2079 6f75 2063 6f64  sting as you cod
-00000b30: 652e 0a3c 2f68 323e 0a3c 6834 2061 6c69  e..</h2>.<h4 ali
-00000b40: 676e 3d22 6365 6e74 6572 223e 0a53 6565  gn="center">.See
-00000b50: 2068 6f77 2065 7665 7279 2063 6861 6e67   how every chang
-00000b60: 6520 746f 2064 6274 2063 6f64 6520 6166  e to dbt code af
-00000b70: 6665 6374 7320 7468 6520 6461 7461 2070  fects the data p
-00000b80: 726f 6475 6365 6420 696e 2074 6865 206d  roduced in the m
-00000b90: 6f64 6966 6965 6420 6d6f 6465 6c20 616e  odified model an
-00000ba0: 6420 646f 776e 7374 7265 616d 2e0a 3c2f  d downstream..</
-00000bb0: 6834 3e0a 3c62 723e 0a0a 2323 2057 6861  h4>.<br>..## Wha
-00000bc0: 7420 6973 2060 6461 7461 2d64 6966 6660  t is `data-diff`
-00000bd0: 3f0a 0a64 6174 612d 6469 6666 2069 7320  ?..data-diff is 
-00000be0: 616e 206f 7065 6e20 736f 7572 6365 2070  an open source p
-00000bf0: 6163 6b61 6765 2074 6861 7420 796f 7520  ackage that you 
-00000c00: 6361 6e20 7573 6520 746f 2073 6565 2074  can use to see t
-00000c10: 6865 2069 6d70 6163 7420 6f66 2079 6f75  he impact of you
-00000c20: 7220 6462 7420 636f 6465 2063 6861 6e67  r dbt code chang
-00000c30: 6573 206f 6e20 796f 7572 2064 6274 206d  es on your dbt m
-00000c40: 6f64 656c 7320 6173 2079 6f75 2063 6f64  odels as you cod
-00000c50: 652e 0a0a 3c64 6976 2061 6c69 676e 3d22  e...<div align="
-00000c60: 6365 6e74 6572 223e 0a0a 215b 6465 7665  center">..![deve
-00000c70: 6c6f 706d 656e 745f 7465 7374 696e 675f  lopment_testing_
-00000c80: 6769 665d 2868 7474 7073 3a2f 2f75 7365  gif](https://use
-00000c90: 722d 696d 6167 6573 2e67 6974 6875 6275  r-images.githubu
-00000ca0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f31  sercontent.com/1
-00000cb0: 3739 3939 3331 2f32 3336 3335 3432 3836  799931/236354286
-00000cc0: 2d64 3164 3034 3463 662d 3231 3638 2d34  -d1d044cf-2168-4
-00000cd0: 3132 382d 3861 3231 2d38 6338 6361 3766  128-8a21-8c8ca7f
-00000ce0: 6434 3934 632e 6769 6629 0a0a 3c2f 6469  d494c.gif)..</di
-00000cf0: 763e 0a0a 3c62 723e 0a0a 3a65 7965 733a  v>..<br>..:eyes:
-00000d00: 202a 2a57 6174 6368 2034 2d6d 696e 2064   **Watch 4-min d
-00000d10: 656d 6f20 7669 6465 6f20 5b68 6572 655d  emo video [here]
-00000d20: 2868 7474 7073 3a2f 2f77 7777 2e6c 6f6f  (https://www.loo
-00000d30: 6d2e 636f 6d2f 7368 6172 652f 6164 3364  m.com/share/ad3d
-00000d40: 6639 3639 6261 3662 3432 3938 3933 3965  f969ba6b4298939e
-00000d50: 6662 3266 6263 6331 3463 6465 292a 2a0a  fb2fbcc14cde)**.
-00000d60: 0a23 2320 4765 7474 696e 6720 5374 6172  .## Getting Star
-00000d70: 7465 640a 0a2a 2a49 6e73 7461 6c6c 2060  ted..**Install `
-00000d80: 6461 7461 2d64 6966 6660 2a2a 0a0a 496e  data-diff`**..In
-00000d90: 7374 616c 6c20 6064 6174 612d 6469 6666  stall `data-diff
-00000da0: 6020 7769 7468 2074 6865 2063 6f6d 6d61  ` with the comma
-00000db0: 6e64 2074 6861 7420 6973 2073 7065 6369  nd that is speci
-00000dc0: 6669 6320 746f 2074 6865 2064 6174 6162  fic to the datab
-00000dd0: 6173 6520 796f 7520 7573 6520 7769 7468  ase you use with
-00000de0: 2064 6274 2e0a 0a23 2323 2053 6e6f 7766   dbt...### Snowf
-00000df0: 6c61 6b65 0a60 6060 0a70 6970 2069 6e73  lake.```.pip ins
-00000e00: 7461 6c6c 2064 6174 612d 6469 6666 2027  tall data-diff '
-00000e10: 6461 7461 2d64 6966 665b 736e 6f77 666c  data-diff[snowfl
-00000e20: 616b 652c 6462 745d 2720 2d55 0a60 6060  ake,dbt]' -U.```
-00000e30: 0a0a 2323 2320 4269 6751 7565 7279 0a60  ..### BigQuery.`
-00000e40: 6060 0a70 6970 2069 6e73 7461 6c6c 2064  ``.pip install d
-00000e50: 6174 612d 6469 6666 2027 6461 7461 2d64  ata-diff 'data-d
-00000e60: 6966 665b 6462 745d 2720 676f 6f67 6c65  iff[dbt]' google
-00000e70: 2d63 6c6f 7564 2d62 6967 7175 6572 7920  -cloud-bigquery 
-00000e80: 2d55 0a60 6060 0a0a 2323 2320 5265 6473  -U.```..### Reds
-00000e90: 6869 6674 0a60 6060 0a70 6970 2069 6e73  hift.```.pip ins
-00000ea0: 7461 6c6c 2064 6174 612d 6469 6666 2027  tall data-diff '
-00000eb0: 6461 7461 2d64 6966 665b 7265 6473 6869  data-diff[redshi
-00000ec0: 6674 2c64 6274 5d27 202d 550a 6060 600a  ft,dbt]' -U.```.
-00000ed0: 0a23 2323 2050 6f73 7467 7265 730a 6060  .### Postgres.``
-00000ee0: 600a 7069 7020 696e 7374 616c 6c20 6461  `.pip install da
-00000ef0: 7461 2d64 6966 6620 2764 6174 612d 6469  ta-diff 'data-di
-00000f00: 6666 5b70 6f73 7467 7265 732c 6462 745d  ff[postgres,dbt]
-00000f10: 2720 2d55 0a60 6060 0a0a 2323 2320 4461  ' -U.```..### Da
-00000f20: 7461 6272 6963 6b73 0a60 6060 0a70 6970  tabricks.```.pip
-00000f30: 2069 6e73 7461 6c6c 2064 6174 612d 6469   install data-di
-00000f40: 6666 2027 6461 7461 2d64 6966 665b 6461  ff 'data-diff[da
-00000f50: 7461 6272 6963 6b73 2c64 6274 5d27 202d  tabricks,dbt]' -
-00000f60: 550a 6060 600a 0a23 2323 2044 7563 6b44  U.```..### DuckD
-00000f70: 420a 6060 600a 7069 7020 696e 7374 616c  B.```.pip instal
-00000f80: 6c20 6461 7461 2d64 6966 6620 2764 6174  l data-diff 'dat
-00000f90: 612d 6469 6666 5b64 7563 6b64 622c 6462  a-diff[duckdb,db
-00000fa0: 745d 2720 2d55 0a60 6060 0a0a 2a2a 5570  t]' -U.```..**Up
-00000fb0: 6461 7465 2061 2066 6577 206c 696e 6573  date a few lines
-00000fc0: 2069 6e20 796f 7572 2060 6462 745f 7072   in your `dbt_pr
-00000fd0: 6f6a 6563 742e 796d 6c60 2a2a 2e0a 6060  oject.yml`**..``
-00000fe0: 600a 2364 6274 5f70 726f 6a65 6374 2e79  `.#dbt_project.y
-00000ff0: 6d6c 0a76 6172 733a 0a20 2064 6174 615f  ml.vars:.  data_
-00001000: 6469 6666 3a0a 2020 2020 7072 6f64 5f64  diff:.    prod_d
-00001010: 6174 6162 6173 653a 206d 795f 6461 7461  atabase: my_data
-00001020: 6261 7365 0a20 2020 2070 726f 645f 7363  base.    prod_sc
-00001030: 6865 6d61 3a20 6d79 5f64 6566 6175 6c74  hema: my_default
-00001040: 5f73 6368 656d 610a 6060 600a 0a2a 2a52  _schema.```..**R
-00001050: 756e 2079 6f75 7220 6669 7273 7420 6461  un your first da
-00001060: 7461 2064 6966 6621 2a2a 0a0a 6060 600a  ta diff!**..```.
-00001070: 6462 7420 7275 6e20 2626 2064 6174 612d  dbt run && data-
-00001080: 6469 6666 202d 2d64 6274 0a60 6060 0a0a  diff --dbt.```..
-00001090: 5765 2072 6563 6f6d 6d65 6e64 2079 6f75  We recommend you
-000010a0: 2067 6574 2073 7461 7274 6564 2062 7920   get started by 
-000010b0: 7761 6c6b 696e 6720 7468 726f 7567 6820  walking through 
-000010c0: 5b6f 7572 2073 696d 706c 6520 7365 7475  [our simple setu
-000010d0: 7020 696e 7374 7275 6374 696f 6e73 5d28  p instructions](
-000010e0: 6874 7470 733a 2f2f 646f 6373 2e64 6174  https://docs.dat
-000010f0: 6166 6f6c 642e 636f 6d2f 6465 7665 6c6f  afold.com/develo
-00001100: 706d 656e 745f 7465 7374 696e 672f 6f70  pment_testing/op
-00001110: 656e 5f73 6f75 7263 6529 2077 6869 6368  en_source) which
-00001120: 2063 6f6e 7461 696e 2065 7861 6d70 6c65   contain example
-00001130: 7320 616e 6420 6465 7461 696c 732e 0a0a  s and details...
-00001140: 506c 6561 7365 2072 6561 6368 206f 7574  Please reach out
-00001150: 206f 6e20 7468 6520 6462 7420 536c 6163   on the dbt Slac
-00001160: 6b20 696e 205b 2374 6f6f 6c73 2d64 6174  k in [#tools-dat
-00001170: 6166 6f6c 645d 2868 7474 7073 3a2f 2f67  afold](https://g
-00001180: 6574 6462 742e 736c 6163 6b2e 636f 6d2f  etdbt.slack.com/
-00001190: 6172 6368 6976 6573 2f43 3033 4432 3541  archives/C03D25A
-000011a0: 3932 5555 2920 6966 2079 6f75 2068 6176  92UU) if you hav
-000011b0: 6520 616e 7920 7472 6f75 626c 6520 7768  e any trouble wh
-000011c0: 6174 736f 6576 6572 2067 6574 7469 6e67  atsoever getting
-000011d0: 2073 7461 7274 6564 210a 0a3c 6272 3e3c   started!..<br><
-000011e0: 6272 3e0a 0a23 2323 2044 6966 6669 6e67  br>..### Diffing
-000011f0: 2062 6574 7765 656e 2064 6174 6162 6173   between databas
-00001200: 6573 0a0a 4368 6563 6b20 6f75 7420 6f75  es..Check out ou
-00001210: 7220 5b64 6f63 756d 656e 7461 7469 6f6e  r [documentation
-00001220: 5d28 6874 7470 733a 2f2f 646f 6373 2e64  ](https://docs.d
-00001230: 6174 6166 6f6c 642e 636f 6d2f 7265 6665  atafold.com/refe
-00001240: 7265 6e63 652f 6f70 656e 5f73 6f75 7263  rence/open_sourc
-00001250: 652f 636c 6929 2069 6620 796f 7527 7265  e/cli) if you're
-00001260: 206c 6f6f 6b69 6e67 2074 6f20 636f 6d70   looking to comp
-00001270: 6172 6520 6461 7461 2061 6372 6f73 7320  are data across 
-00001280: 6461 7461 6261 7365 7320 2866 6f72 2065  databases (for e
-00001290: 7861 6d70 6c65 2c20 6265 7477 6565 6e20  xample, between 
-000012a0: 506f 7374 6772 6573 2061 6e64 2053 6e6f  Postgres and Sno
-000012b0: 7766 6c61 6b65 292e 0a0a 3c62 723e 0a0a  wflake)...<br>..
-000012c0: 2323 2043 6f6e 7472 6962 7574 6f72 730a  ## Contributors.
-000012d0: 0a57 6520 7468 616e 6b20 6576 6572 796f  .We thank everyo
-000012e0: 6e65 2077 686f 2063 6f6e 7472 6962 7574  ne who contribut
-000012f0: 6564 2073 6f20 6661 7221 0a0a 3c61 2068  ed so far!..<a h
-00001300: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00001310: 6875 622e 636f 6d2f 6461 7461 666f 6c64  hub.com/datafold
-00001320: 2f64 6174 612d 6469 6666 2f67 7261 7068  /data-diff/graph
-00001330: 732f 636f 6e74 7269 6275 746f 7273 223e  s/contributors">
-00001340: 0a20 203c 696d 6720 7372 633d 2268 7474  .  <img src="htt
-00001350: 7073 3a2f 2f63 6f6e 7472 6962 7574 6f72  ps://contributor
-00001360: 732d 696d 672e 7765 622e 6170 702f 696d  s-img.web.app/im
-00001370: 6167 653f 7265 706f 3d64 6174 6166 6f6c  age?repo=datafol
-00001380: 642f 6461 7461 2d64 6966 6622 202f 3e0a  d/data-diff" />.
-00001390: 3c2f 613e 0a0a 3c62 723e 0a0a 2323 2041  </a>..<br>..## A
-000013a0: 6e61 6c79 7469 6373 0a0a 2a20 5b55 7361  nalytics..* [Usa
-000013b0: 6765 2041 6e61 6c79 7469 6373 2026 2044  ge Analytics & D
-000013c0: 6174 6120 5072 6976 6163 795d 2868 7474  ata Privacy](htt
-000013d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000013e0: 6461 7461 666f 6c64 2f64 6174 612d 6469  datafold/data-di
-000013f0: 6666 2f62 6c6f 622f 6d61 7374 6572 2f64  ff/blob/master/d
-00001400: 6f63 732f 7573 6167 655f 616e 616c 7974  ocs/usage_analyt
-00001410: 6963 732e 6d64 290a 0a3c 6272 3e0a 0a23  ics.md)..<br>..#
-00001420: 2320 4c69 6365 6e73 650a 0a54 6869 7320  # License..This 
-00001430: 7072 6f6a 6563 7420 6973 206c 6963 656e  project is licen
-00001440: 7365 6420 756e 6465 7220 7468 6520 7465  sed under the te
-00001450: 726d 7320 6f66 2074 6865 205b 4d49 5420  rms of the [MIT 
-00001460: 4c69 6365 6e73 655d 2868 7474 7073 3a2f  License](https:/
-00001470: 2f67 6974 6875 622e 636f 6d2f 6461 7461  /github.com/data
-00001480: 666f 6c64 2f64 6174 612d 6469 6666 2f62  fold/data-diff/b
-00001490: 6c6f 622f 6d61 7374 6572 2f4c 4943 454e  lob/master/LICEN
-000014a0: 5345 292e 0a0a                           SE)...
+000006a0: 7365 2028 3c30 2e32 2e30 290a 5265 7175  se (<0.2.0).Requ
+000006b0: 6972 6573 2d44 6973 743a 2064 7563 6b64  ires-Dist: duckd
+000006c0: 6220 283e 3d30 2e37 2e30 2c3c 302e 382e  b (>=0.7.0,<0.8.
+000006d0: 3029 203b 2065 7874 7261 203d 3d20 2264  0) ; extra == "d
+000006e0: 7563 6b64 6222 0a52 6571 7569 7265 732d  uckdb".Requires-
+000006f0: 4469 7374 3a20 6b65 7972 696e 670a 5265  Dist: keyring.Re
+00000700: 7175 6972 6573 2d44 6973 743a 206d 7973  quires-Dist: mys
+00000710: 716c 2d63 6f6e 6e65 6374 6f72 2d70 7974  ql-connector-pyt
+00000720: 686f 6e20 283d 3d38 2e30 2e32 3929 203b  hon (==8.0.29) ;
+00000730: 2065 7874 7261 203d 3d20 226d 7973 716c   extra == "mysql
+00000740: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000750: 2070 7265 716c 2028 3e3d 302e 322e 3139   preql (>=0.2.19
+00000760: 2c3c 302e 332e 3029 203b 2065 7874 7261  ,<0.3.0) ; extra
+00000770: 203d 3d20 2270 7265 716c 220a 5265 7175   == "preql".Requ
+00000780: 6972 6573 2d44 6973 743a 2070 7265 7374  ires-Dist: prest
+00000790: 6f2d 7079 7468 6f6e 2d63 6c69 656e 7420  o-python-client 
+000007a0: 3b20 6578 7472 6120 3d3d 2022 7072 6573  ; extra == "pres
+000007b0: 746f 220a 5265 7175 6972 6573 2d44 6973  to".Requires-Dis
+000007c0: 743a 2070 7379 636f 7067 3220 3b20 6578  t: psycopg2 ; ex
+000007d0: 7472 6120 3d3d 2022 706f 7374 6772 6573  tra == "postgres
+000007e0: 716c 2220 6f72 2065 7874 7261 203d 3d20  ql" or extra == 
+000007f0: 2272 6564 7368 6966 7422 0a52 6571 7569  "redshift".Requi
+00000800: 7265 732d 4469 7374 3a20 7269 6368 0a52  res-Dist: rich.R
+00000810: 6571 7569 7265 732d 4469 7374 3a20 7275  equires-Dist: ru
+00000820: 6e74 7970 6520 283e 3d30 2e32 2e36 2c3c  ntype (>=0.2.6,<
+00000830: 302e 332e 3029 0a52 6571 7569 7265 732d  0.3.0).Requires-
+00000840: 4469 7374 3a20 736e 6f77 666c 616b 652d  Dist: snowflake-
+00000850: 636f 6e6e 6563 746f 722d 7079 7468 6f6e  connector-python
+00000860: 2028 3e3d 332e 302e 322c 3c34 2e30 2e30   (>=3.0.2,<4.0.0
+00000870: 2920 3b20 6578 7472 6120 3d3d 2022 736e  ) ; extra == "sn
+00000880: 6f77 666c 616b 6522 0a52 6571 7569 7265  owflake".Require
+00000890: 732d 4469 7374 3a20 7461 6275 6c61 7465  s-Dist: tabulate
+000008a0: 2028 3e3d 302e 392e 302c 3c30 2e31 302e   (>=0.9.0,<0.10.
+000008b0: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
+000008c0: 3a20 746f 6d6c 2028 3e3d 302e 3130 2e32  : toml (>=0.10.2
+000008d0: 2c3c 302e 3131 2e30 290a 5265 7175 6972  ,<0.11.0).Requir
+000008e0: 6573 2d44 6973 743a 2074 7269 6e6f 2028  es-Dist: trino (
+000008f0: 3e3d 302e 3331 342e 302c 3c30 2e33 3135  >=0.314.0,<0.315
+00000900: 2e30 2920 3b20 6578 7472 6120 3d3d 2022  .0) ; extra == "
+00000910: 7472 696e 6f22 0a52 6571 7569 7265 732d  trino".Requires-
+00000920: 4469 7374 3a20 7572 6c6c 6962 3320 283c  Dist: urllib3 (<
+00000930: 3229 0a52 6571 7569 7265 732d 4469 7374  2).Requires-Dist
+00000940: 3a20 7665 7274 6963 612d 7079 7468 6f6e  : vertica-python
+00000950: 203b 2065 7874 7261 203d 3d20 2276 6572   ; extra == "ver
+00000960: 7469 6361 220a 5072 6f6a 6563 742d 5552  tica".Project-UR
+00000970: 4c3a 2052 6570 6f73 6974 6f72 792c 2068  L: Repository, h
+00000980: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000990: 6d2f 6461 7461 666f 6c64 2f64 6174 612d  m/datafold/data-
+000009a0: 6469 6666 0a44 6573 6372 6970 7469 6f6e  diff.Description
+000009b0: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+000009c0: 6578 742f 6d61 726b 646f 776e 0a0a 3c70  ext/markdown..<p
+000009d0: 2061 6c69 676e 3d22 6c65 6674 223e 0a20   align="left">. 
+000009e0: 2020 203c 696d 6720 616c 743d 2244 6174     <img alt="Dat
+000009f0: 6166 6f6c 6422 2073 7263 3d22 6874 7470  afold" src="http
+00000a00: 733a 2f2f 7573 6572 2d69 6d61 6765 732e  s://user-images.
+00000a10: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00000a20: 742e 636f 6d2f 3137 3939 3933 312f 3139  t.com/1799931/19
+00000a30: 3634 3937 3131 302d 6433 6465 3131 3133  6497110-d3de1113
+00000a40: 2d61 3937 662d 3433 3232 2d62 3533 312d  -a97f-4322-b531-
+00000a50: 3032 3664 3835 3962 3836 3761 2e70 6e67  026d859b867a.png
+00000a60: 2220 7769 6474 683d 2233 3025 2220 2f3e  " width="30%" />
+00000a70: 0a3c 2f70 3e0a 0a3c 6831 2061 6c69 676e  .</p>..<h1 align
+00000a80: 3d22 6c65 6674 223e 0a64 6174 612d 6469  ="left">.data-di
+00000a90: 6666 3a20 636f 6d70 6172 6520 6461 7461  ff: compare data
+00000aa0: 7365 7473 2066 6173 742c 2077 6974 6869  sets fast, withi
+00000ab0: 6e20 6f72 2061 6372 6f73 7320 5351 4c20  n or across SQL 
+00000ac0: 6461 7461 6261 7365 730a 3c2f 6831 3e0a  databases.</h1>.
+00000ad0: 0a3c 6272 3e0a 0a0a 2320 5573 6520 6361  .<br>...# Use ca
+00000ae0: 7365 730a 0a23 2320 4461 7461 204d 6967  ses..## Data Mig
+00000af0: 7261 7469 6f6e 2026 2052 6570 6c69 6361  ration & Replica
+00000b00: 7469 6f6e 2054 6573 7469 6e67 0a43 6f6d  tion Testing.Com
+00000b10: 7061 7265 2073 6f75 7263 6520 746f 2074  pare source to t
+00000b20: 6172 6765 7420 616e 6420 6368 6563 6b20  arget and check 
+00000b30: 666f 7220 6469 7363 7265 7061 6e63 6965  for discrepancie
+00000b40: 7320 7768 656e 206d 6f76 696e 6720 6461  s when moving da
+00000b50: 7461 2062 6574 7765 656e 2073 7973 7465  ta between syste
+00000b60: 6d73 3a0a 2d20 4d69 6772 6174 696e 6720  ms:.- Migrating 
+00000b70: 746f 2061 206e 6577 2064 6174 6120 7761  to a new data wa
+00000b80: 7265 686f 7573 6520 2865 2e67 2e2c 204f  rehouse (e.g., O
+00000b90: 7261 636c 6520 3e20 536e 6f77 666c 616b  racle > Snowflak
+00000ba0: 6529 0a2d 2043 6f6e 7665 7274 696e 6720  e).- Converting 
+00000bb0: 5351 4c20 746f 2061 206e 6577 2074 7261  SQL to a new tra
+00000bc0: 6e73 666f 726d 6174 696f 6e20 6672 616d  nsformation fram
+00000bd0: 6577 6f72 6b20 2865 2e67 2e2c 2073 746f  ework (e.g., sto
+00000be0: 7265 6420 7072 6f63 6564 7572 6573 203e  red procedures >
+00000bf0: 2064 6274 290a 2d20 436f 6e74 696e 756f   dbt).- Continuo
+00000c00: 7573 6c79 2072 6570 6c69 6361 7469 6e67  usly replicating
+00000c10: 2064 6174 6120 6672 6f6d 2061 6e20 4f4c   data from an OL
+00000c20: 5450 2044 4220 746f 204f 4c41 5020 4457  TP DB to OLAP DW
+00000c30: 4820 2865 2e67 2e2c 204d 7953 514c 203e  H (e.g., MySQL >
+00000c40: 2052 6564 7368 6966 7429 0a0a 0a49 6e73   Redshift)...Ins
+00000c50: 7461 6c6c 2060 6461 7461 2d64 6966 6660  tall `data-diff`
+00000c60: 2077 6974 6820 7370 6563 6966 6963 2064   with specific d
+00000c70: 6174 6162 6173 6520 6164 6170 7465 7273  atabase adapters
+00000c80: 2c20 652e 672e 3a0a 0a60 6060 0a70 6970  , e.g.:..```.pip
+00000c90: 2069 6e73 7461 6c6c 2064 6174 612d 6469   install data-di
+00000ca0: 6666 2027 6461 7461 2d64 6966 665b 706f  ff 'data-diff[po
+00000cb0: 7374 6772 6573 716c 2c73 6e6f 7766 6c61  stgresql,snowfla
+00000cc0: 6b65 095d 2720 2d55 0a60 6060 0a52 756e  ke.]' -U.```.Run
+00000cd0: 2060 6461 7461 2d64 6966 6660 2077 6974   `data-diff` wit
+00000ce0: 6820 636f 6e6e 6563 7469 6f6e 2055 5249  h connection URI
+00000cf0: 7320 746f 2063 6f6d 7061 7265 2074 6162  s to compare tab
+00000d00: 6c65 733a 0a60 6060 0a64 6174 612d 6469  les:.```.data-di
+00000d10: 6666 205c 0a20 2070 6f73 7467 7265 7371  ff \.  postgresq
+00000d20: 6c3a 2f2f 3c75 7365 726e 616d 653e 3a27  l://<username>:'
+00000d30: 3c70 6173 7377 6f72 643e 2740 6c6f 6361  <password>'@loca
+00000d40: 6c68 6f73 743a 3534 3332 2f3c 6461 7461  lhost:5432/<data
+00000d50: 6261 7365 3e20 5c0a 2020 3c74 6162 6c65  base> \.  <table
+00000d60: 3e20 5c0a 2020 2273 6e6f 7766 6c61 6b65  > \.  "snowflake
+00000d70: 3a2f 2f3c 7573 6572 6e61 6d65 3e3a 3c70  ://<username>:<p
+00000d80: 6173 7377 6f72 643e 403c 7061 7373 776f  assword>@<passwo
+00000d90: 7264 3e2f 3c44 4154 4142 4153 453e 2f3c  rd>/<DATABASE>/<
+00000da0: 5343 4845 4d41 3e3f 7761 7265 686f 7573  SCHEMA>?warehous
+00000db0: 653d 3c57 4152 4548 4f55 5345 3e26 726f  e=<WAREHOUSE>&ro
+00000dc0: 6c65 3d3c 524f 4c45 3e22 205c 0a20 203c  le=<ROLE>" \.  <
+00000dd0: 5441 424c 453e 205c 0a20 202d 6b20 6163  TABLE> \.  -k ac
+00000de0: 7469 7669 7479 5f69 6420 5c0a 2020 2d63  tivity_id \.  -c
+00000df0: 2061 6374 6976 6974 7920 5c0a 2020 2d77   activity \.  -w
+00000e00: 2022 6576 656e 745f 7469 6d65 7374 616d   "event_timestam
+00000e10: 7020 3c20 2732 3032 322d 3130 2d31 3027  p < '2022-10-10'
+00000e20: 220a 6060 600a 4368 6563 6b20 6f75 7420  ".```.Check out 
+00000e30: 5b64 6f63 756d 656e 7461 7469 6f6e 5d28  [documentation](
+00000e40: 6874 7470 733a 2f2f 646f 6373 2e64 6174  https://docs.dat
+00000e50: 6166 6f6c 642e 636f 6d2f 7265 6665 7265  afold.com/refere
+00000e60: 6e63 652f 6f70 656e 5f73 6f75 7263 652f  nce/open_source/
+00000e70: 636c 6929 2066 6f72 2066 756c 6c20 636f  cli) for full co
+00000e80: 6d6d 616e 6420 7265 6665 7265 6e63 652e  mmand reference.
+00000e90: 0a0a 2323 2044 6174 6120 4465 7665 6c6f  ..## Data Develo
+00000ea0: 706d 656e 7420 5465 7374 696e 670a 5465  pment Testing.Te
+00000eb0: 7374 2053 514c 2063 6f64 6520 616e 6420  st SQL code and 
+00000ec0: 7072 6576 6965 7720 6368 616e 6765 7320  preview changes 
+00000ed0: 6279 2063 6f6d 7061 7269 6e67 2064 6576  by comparing dev
+00000ee0: 656c 6f70 6d65 6e74 2f73 7461 6769 6e67  elopment/staging
+00000ef0: 2065 6e76 6972 6f6e 6d65 6e74 2064 6174   environment dat
+00000f00: 6120 746f 2070 726f 6475 6374 696f 6e3a  a to production:
+00000f10: 0a31 2e20 4d61 6b65 2061 2063 6861 6e67  .1. Make a chang
+00000f20: 6520 746f 2073 6f6d 6520 5351 4c20 636f  e to some SQL co
+00000f30: 6465 0a32 2e20 5275 6e20 7468 6520 5351  de.2. Run the SQ
+00000f40: 4c20 636f 6465 2074 6f20 6372 6561 7465  L code to create
+00000f50: 2061 206e 6577 2064 6174 6173 6574 0a33   a new dataset.3
+00000f60: 2e20 436f 6d70 6172 6520 7468 6520 6461  . Compare the da
+00000f70: 7461 7365 7420 7769 7468 2069 7473 2070  taset with its p
+00000f80: 726f 6475 6374 696f 6e20 7665 7273 696f  roduction versio
+00000f90: 6e20 6f72 2061 6e6f 7468 6572 2069 7465  n or another ite
+00000fa0: 7261 7469 6f6e 0a0a 2020 3c70 2061 6c69  ration..  <p ali
+00000fb0: 676e 3d22 6c65 6674 223e 0a20 203c 696d  gn="left">.  <im
+00000fc0: 6720 616c 743d 2264 6274 2220 7372 633d  g alt="dbt" src=
+00000fd0: 2268 7474 7073 3a2f 2f73 6565 6b6c 6f67  "https://seeklog
+00000fe0: 6f2e 636f 6d2f 696d 6167 6573 2f44 2f64  o.com/images/D/d
+00000ff0: 6274 2d6c 6f67 6f2d 4534 4230 4544 3732  bt-logo-E4B0ED72
+00001000: 4132 2d73 6565 6b6c 6f67 6f2e 636f 6d2e  A2-seeklogo.com.
+00001010: 706e 6722 2077 6964 7468 3d22 3130 2522  png" width="10%"
+00001020: 202f 3e0a 2020 3c2f 703e 0a20 200a 6064   />.  </p>.  .`d
+00001030: 6174 612d 6469 6666 6020 696e 7465 6772  ata-diff` integr
+00001040: 6174 6573 2077 6974 6820 6462 7420 436f  ates with dbt Co
+00001050: 7265 2061 6e64 2064 6274 2043 6c6f 7564  re and dbt Cloud
+00001060: 2074 6f20 7365 616d 6c65 7373 6c79 2063   to seamlessly c
+00001070: 6f6d 7061 7265 206c 6f63 616c 2064 6576  ompare local dev
+00001080: 656c 6f70 6d65 6e74 2074 6f20 7072 6f64  elopment to prod
+00001090: 7563 7469 6f6e 2064 6174 6173 6574 732e  uction datasets.
+000010a0: 200a 0a3a 6579 6573 3a20 2a2a 5761 7463   ..:eyes: **Watc
+000010b0: 6820 5b34 2d6d 696e 2064 656d 6f20 7669  h [4-min demo vi
+000010c0: 6465 6f5d 2868 7474 7073 3a2f 2f77 7777  deo](https://www
+000010d0: 2e6c 6f6f 6d2e 636f 6d2f 7368 6172 652f  .loom.com/share/
+000010e0: 6164 3364 6639 3639 6261 3662 3432 3938  ad3df969ba6b4298
+000010f0: 3933 3965 6662 3266 6263 6331 3463 6465  939efb2fbcc14cde
+00001100: 292a 2a0a 0a2a 2a5b 4765 7420 7374 6172  )**..**[Get star
+00001110: 7465 6420 7769 7468 2064 6174 612d 6469  ted with data-di
+00001120: 6666 2026 2064 6274 5d28 6874 7470 733a  ff & dbt](https:
+00001130: 2f2f 646f 6373 2e64 6174 6166 6f6c 642e  //docs.datafold.
+00001140: 636f 6d2f 6465 7665 6c6f 706d 656e 745f  com/development_
+00001150: 7465 7374 696e 672f 6f70 656e 5f73 6f75  testing/open_sou
+00001160: 7263 6529 2a2a 0a0a 5265 6163 6820 6f75  rce)**..Reach ou
+00001170: 7420 6f6e 2074 6865 2064 6274 2053 6c61  t on the dbt Sla
+00001180: 636b 2069 6e20 5b23 746f 6f6c 732d 6461  ck in [#tools-da
+00001190: 7461 666f 6c64 5d28 6874 7470 733a 2f2f  tafold](https://
+000011a0: 6765 7464 6274 2e73 6c61 636b 2e63 6f6d  getdbt.slack.com
+000011b0: 2f61 7263 6869 7665 732f 4330 3344 3235  /archives/C03D25
+000011c0: 4139 3255 5529 2066 6f72 2061 6476 6963  A92UU) for advic
+000011d0: 6520 616e 6420 7375 7070 6f72 740a 0a23  e and support..#
+000011e0: 2320 5375 7070 6f72 7465 6420 6461 7461  # Supported data
+000011f0: 6261 7365 730a 0a2d 2050 6f73 7467 7265  bases..- Postgre
+00001200: 5351 4c20 3e3d 3130 0a2d 204d 7953 514c  SQL >=10.- MySQL
+00001210: 0a2d 2053 6e6f 7766 6c61 6b65 0a2d 2042  .- Snowflake.- B
+00001220: 6967 5175 6572 790a 2d20 5265 6473 6869  igQuery.- Redshi
+00001230: 6674 0a2d 204f 7261 636c 650a 2d20 5072  ft.- Oracle.- Pr
+00001240: 6573 746f 0a2d 2044 6174 6162 7269 636b  esto.- Databrick
+00001250: 730a 2d20 5472 696e 6f0a 2d20 436c 6963  s.- Trino.- Clic
+00001260: 6b68 6f75 7365 0a2d 2056 6572 7469 6361  khouse.- Vertica
+00001270: 0a2d 2044 7563 6b44 4220 3e3d 302e 360a  .- DuckDB >=0.6.
+00001280: 2d20 5351 4c69 7465 2028 636f 6d69 6e67  - SQLite (coming
+00001290: 2073 6f6f 6e29 0a0a 0a3c 6272 3e0a 0a23   soon)...<br>..#
+000012a0: 2320 436f 6e74 7269 6275 746f 7273 0a0a  # Contributors..
+000012b0: 5765 2074 6861 6e6b 2065 7665 7279 6f6e  We thank everyon
+000012c0: 6520 7768 6f20 636f 6e74 7269 6275 7465  e who contribute
+000012d0: 6420 736f 2066 6172 210a 0a3c 6120 6872  d so far!..<a hr
+000012e0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000012f0: 7562 2e63 6f6d 2f64 6174 6166 6f6c 642f  ub.com/datafold/
+00001300: 6461 7461 2d64 6966 662f 6772 6170 6873  data-diff/graphs
+00001310: 2f63 6f6e 7472 6962 7574 6f72 7322 3e0a  /contributors">.
+00001320: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00001330: 733a 2f2f 636f 6e74 7269 6275 746f 7273  s://contributors
+00001340: 2d69 6d67 2e77 6562 2e61 7070 2f69 6d61  -img.web.app/ima
+00001350: 6765 3f72 6570 6f3d 6461 7461 666f 6c64  ge?repo=datafold
+00001360: 2f64 6174 612d 6469 6666 2220 2f3e 0a3c  /data-diff" />.<
+00001370: 2f61 3e0a 0a3c 6272 3e0a 0a23 2320 416e  /a>..<br>..## An
+00001380: 616c 7974 6963 730a 0a2a 205b 5573 6167  alytics..* [Usag
+00001390: 6520 416e 616c 7974 6963 7320 2620 4461  e Analytics & Da
+000013a0: 7461 2050 7269 7661 6379 5d28 6874 7470  ta Privacy](http
+000013b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+000013c0: 6174 6166 6f6c 642f 6461 7461 2d64 6966  atafold/data-dif
+000013d0: 662f 626c 6f62 2f6d 6173 7465 722f 646f  f/blob/master/do
+000013e0: 6373 2f75 7361 6765 5f61 6e61 6c79 7469  cs/usage_analyti
+000013f0: 6373 2e6d 6429 0a0a 3c62 723e 0a0a 2323  cs.md)..<br>..##
+00001400: 204c 6963 656e 7365 0a0a 5468 6973 2070   License..This p
+00001410: 726f 6a65 6374 2069 7320 6c69 6365 6e73  roject is licens
+00001420: 6564 2075 6e64 6572 2074 6865 2074 6572  ed under the ter
+00001430: 6d73 206f 6620 7468 6520 5b4d 4954 204c  ms of the [MIT L
+00001440: 6963 656e 7365 5d28 6874 7470 733a 2f2f  icense](https://
+00001450: 6769 7468 7562 2e63 6f6d 2f64 6174 6166  github.com/dataf
+00001460: 6f6c 642f 6461 7461 2d64 6966 662f 626c  old/data-diff/bl
+00001470: 6f62 2f6d 6173 7465 722f 4c49 4345 4e53  ob/master/LICENS
+00001480: 4529 2e0a 0a                             E)...
```

