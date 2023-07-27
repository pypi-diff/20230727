# Comparing `tmp/mindsdb_sql-0.6.6.tar.gz` & `tmp/mindsdb_sql-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mindsdb_sql-0.6.6.tar", last modified: Thu Jul 20 12:23:05 2023, max compression
+gzip compressed data, was "dist\mindsdb_sql-0.6.7.tar", last modified: Thu Jul 27 14:13:03 2023, max compression
```

## Comparing `mindsdb_sql-0.6.6.tar` & `mindsdb_sql-0.6.7.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/
--rw-rw-rw-   0        0        0      535 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/PKG-INFO
--rw-rw-rw-   0        0        0     7245 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql/
--rw-rw-rw-   0        0        0      365 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/__about__.py
--rw-rw-rw-   0        0        0     1195 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/__init__.py
--rw-rw-rw-   0        0        0      170 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/
--rw-rw-rw-   0        0        0        0 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/
--rw-rw-rw-   0        0        0      537 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/__init__.py
--rw-rw-rw-   0        0        0      842 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/alter_table.py
--rw-rw-rw-   0        0        0     1343 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/base.py
--rw-rw-rw-   0        0        0      460 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/commit_transaction.py
--rw-rw-rw-   0        0        0     2287 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/create.py
--rw-rw-rw-   0        0        0      994 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/delete.py
--rw-rw-rw-   0        0        0      942 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/describe.py
--rw-rw-rw-   0        0        0     3056 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/drop.py
--rw-rw-rw-   0        0        0      659 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/explain.py
--rw-rw-rw-   0        0        0     3260 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/insert.py
--rw-rw-rw-   0        0        0      466 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/rollback_transaction.py
-drwxrwxrwx   0        0        0        0 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/
--rw-rw-rw-   0        0        0      591 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/__init__.py
--rw-rw-rw-   0        0        0     1482 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/case.py
--rw-rw-rw-   0        0        0     1113 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/common_table_expression.py
--rw-rw-rw-   0        0        0     1593 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/constant.py
--rw-rw-rw-   0        0        0      503 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/data.py
--rw-rw-rw-   0        0        0     3196 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/identifier.py
--rw-rw-rw-   0        0        0     1381 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/join.py
--rw-rw-rw-   0        0        0      662 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/native_query.py
--rw-rw-rw-   0        0        0     5949 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/operation.py
--rw-rw-rw-   0        0        0      806 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/order_by.py
--rw-rw-rw-   0        0        0      464 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/parameter.py
--rw-rw-rw-   0        0        0     5904 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/select.py
--rw-rw-rw-   0        0        0      504 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/star.py
--rw-rw-rw-   0        0        0      648 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/tuple.py
--rw-rw-rw-   0        0        0      774 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/type_cast.py
--rw-rw-rw-   0        0        0     1178 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/union.py
--rw-rw-rw-   0        0        0     3296 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/set.py
--rw-rw-rw-   0        0        0     2979 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/show.py
--rw-rw-rw-   0        0        0      469 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/start_transaction.py
--rw-rw-rw-   0        0        0     3154 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/update.py
--rw-rw-rw-   0        0        0      639 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/use.py
-drwxrwxrwx   0        0        0        0 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/
--rw-rw-rw-   0        0        0        0 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/
--rw-rw-rw-   0        0        0      833 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/__init__.py
--rw-rw-rw-   0        0        0     2569 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/chatbot.py
--rw-rw-rw-   0        0        0     1595 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/create_database.py
--rw-rw-rw-   0        0        0      953 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/create_file.py
--rw-rw-rw-   0        0        0     2078 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/create_job.py
--rw-rw-rw-   0        0        0     1201 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py
--rw-rw-rw-   0        0        0     5361 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py
--rw-rw-rw-   0        0        0     1534 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/create_view.py
--rw-rw-rw-   0        0        0      704 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py
--rw-rw-rw-   0        0        0      713 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py
--rw-rw-rw-   0        0        0      737 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py
--rw-rw-rw-   0        0        0      692 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/drop_job.py
--rw-rw-rw-   0        0        0      708 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py
--rw-rw-rw-   0        0        0      906 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py
--rw-rw-rw-   0        0        0     1313 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/evaluate.py
--rw-rw-rw-   0        0        0      223 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/finetune_predictor.py
--rw-rw-rw-   0        0        0      359 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/latest.py
--rw-rw-rw-   0        0        0     8179 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/lexer.py
--rw-rw-rw-   0        0        0    46067 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/parser.py
--rw-rw-rw-   0        0        0      311 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/retrain_predictor.py
--rw-rw-rw-   0        0        0     1757 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/trigger.py
-drwxrwxrwx   0        0        0        0 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mysql/
--rw-rw-rw-   0        0        0       67 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mysql/__init__.py
--rw-rw-rw-   0        0        0     1046 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mysql/lexer.py
--rw-rw-rw-   0        0        0    29491 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mysql/parser.py
--rw-rw-rw-   0        0        0      904 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mysql/show_index.py
--rw-rw-rw-   0        0        0      686 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mysql/variable.py
--rw-rw-rw-   0        0        0     6226 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/lexer.py
--rw-rw-rw-   0        0        0      751 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/logger.py
--rw-rw-rw-   0        0        0    21382 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/parser.py
--rw-rw-rw-   0        0        0     2497 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql/planner/
--rw-rw-rw-   0        0        0      150 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/planner/__init__.py
--rw-rw-rw-   0        0        0      878 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/planner/query_plan.py
--rw-rw-rw-   0        0        0    54044 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/planner/query_planner.py
--rw-rw-rw-   0        0        0    21394 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/planner/query_prepare.py
--rw-rw-rw-   0        0        0      536 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/planner/step_result.py
--rw-rw-rw-   0        0        0     8739 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/planner/steps.py
--rw-rw-rw-   0        0        0     2981 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/planner/ts_utils.py
--rw-rw-rw-   0        0        0    13228 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/planner/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql/render/
--rw-rw-rw-   0        0        0        0 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/render/__init__.py
--rw-rw-rw-   0        0        0    20561 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/render/sqlalchemy_render.py
-drwxrwxrwx   0        0        0        0 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql.egg-info/
--rw-rw-rw-   0        0        0      535 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3380 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/setup.cfg
--rw-rw-rw-   0        0        0      862 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/sly/
--rw-rw-rw-   0        0        0      109 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/sly/__init__.py
--rw-rw-rw-   0        0        0      777 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/sly/ast.py
--rw-rw-rw-   0        0        0    16707 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/sly/lex.py
--rw-rw-rw-   0        0        0    89289 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/sly/yacc.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/
+-rw-rw-rw-   0        0        0      535 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/PKG-INFO
+-rw-rw-rw-   0        0        0     7245 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql/
+-rw-rw-rw-   0        0        0      365 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/__about__.py
+-rw-rw-rw-   0        0        0     1195 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/__init__.py
+-rw-rw-rw-   0        0        0      170 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/
+-rw-rw-rw-   0        0        0        0 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/
+-rw-rw-rw-   0        0        0      537 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/alter_table.py
+-rw-rw-rw-   0        0        0     1343 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/base.py
+-rw-rw-rw-   0        0        0      460 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/commit_transaction.py
+-rw-rw-rw-   0        0        0     2287 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/create.py
+-rw-rw-rw-   0        0        0      994 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/delete.py
+-rw-rw-rw-   0        0        0      942 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/describe.py
+-rw-rw-rw-   0        0        0     3056 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/drop.py
+-rw-rw-rw-   0        0        0      659 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/explain.py
+-rw-rw-rw-   0        0        0     3260 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/insert.py
+-rw-rw-rw-   0        0        0      466 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/rollback_transaction.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/
+-rw-rw-rw-   0        0        0      591 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/__init__.py
+-rw-rw-rw-   0        0        0     1482 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/case.py
+-rw-rw-rw-   0        0        0     1113 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/common_table_expression.py
+-rw-rw-rw-   0        0        0     1593 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/constant.py
+-rw-rw-rw-   0        0        0      503 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/data.py
+-rw-rw-rw-   0        0        0     3196 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/identifier.py
+-rw-rw-rw-   0        0        0     1381 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/join.py
+-rw-rw-rw-   0        0        0      662 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/native_query.py
+-rw-rw-rw-   0        0        0     5949 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/operation.py
+-rw-rw-rw-   0        0        0      806 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/order_by.py
+-rw-rw-rw-   0        0        0      464 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/parameter.py
+-rw-rw-rw-   0        0        0     5904 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/select.py
+-rw-rw-rw-   0        0        0      504 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/star.py
+-rw-rw-rw-   0        0        0      648 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/tuple.py
+-rw-rw-rw-   0        0        0      774 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/type_cast.py
+-rw-rw-rw-   0        0        0     1178 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/union.py
+-rw-rw-rw-   0        0        0     3296 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/set.py
+-rw-rw-rw-   0        0        0     2979 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/show.py
+-rw-rw-rw-   0        0        0      469 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/start_transaction.py
+-rw-rw-rw-   0        0        0     3154 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/update.py
+-rw-rw-rw-   0        0        0      639 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/use.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/
+-rw-rw-rw-   0        0        0        0 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/
+-rw-rw-rw-   0        0        0      833 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/__init__.py
+-rw-rw-rw-   0        0        0     2569 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/chatbot.py
+-rw-rw-rw-   0        0        0     1595 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/create_database.py
+-rw-rw-rw-   0        0        0      953 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/create_file.py
+-rw-rw-rw-   0        0        0     2078 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/create_job.py
+-rw-rw-rw-   0        0        0     1201 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py
+-rw-rw-rw-   0        0        0     5361 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py
+-rw-rw-rw-   0        0        0     1534 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/create_view.py
+-rw-rw-rw-   0        0        0      704 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py
+-rw-rw-rw-   0        0        0      713 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py
+-rw-rw-rw-   0        0        0      737 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py
+-rw-rw-rw-   0        0        0      692 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/drop_job.py
+-rw-rw-rw-   0        0        0      708 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py
+-rw-rw-rw-   0        0        0      906 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py
+-rw-rw-rw-   0        0        0     1313 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/evaluate.py
+-rw-rw-rw-   0        0        0      223 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/finetune_predictor.py
+-rw-rw-rw-   0        0        0      359 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/latest.py
+-rw-rw-rw-   0        0        0     8179 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/lexer.py
+-rw-rw-rw-   0        0        0    46322 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/parser.py
+-rw-rw-rw-   0        0        0      311 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/retrain_predictor.py
+-rw-rw-rw-   0        0        0     2246 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/trigger.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mysql/
+-rw-rw-rw-   0        0        0       67 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mysql/__init__.py
+-rw-rw-rw-   0        0        0     1046 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mysql/lexer.py
+-rw-rw-rw-   0        0        0    29491 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mysql/parser.py
+-rw-rw-rw-   0        0        0      904 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mysql/show_index.py
+-rw-rw-rw-   0        0        0      686 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mysql/variable.py
+-rw-rw-rw-   0        0        0     6226 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/lexer.py
+-rw-rw-rw-   0        0        0      751 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/logger.py
+-rw-rw-rw-   0        0        0    21382 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/parser.py
+-rw-rw-rw-   0        0        0     2497 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql/planner/
+-rw-rw-rw-   0        0        0      150 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/planner/__init__.py
+-rw-rw-rw-   0        0        0      878 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/planner/query_plan.py
+-rw-rw-rw-   0        0        0    54291 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/planner/query_planner.py
+-rw-rw-rw-   0        0        0    21394 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/planner/query_prepare.py
+-rw-rw-rw-   0        0        0      536 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/planner/step_result.py
+-rw-rw-rw-   0        0        0     8739 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/planner/steps.py
+-rw-rw-rw-   0        0        0     2981 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/planner/ts_utils.py
+-rw-rw-rw-   0        0        0    13439 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/planner/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql/render/
+-rw-rw-rw-   0        0        0        0 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/render/__init__.py
+-rw-rw-rw-   0        0        0    20561 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/render/sqlalchemy_render.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql.egg-info/
+-rw-rw-rw-   0        0        0      535 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3380 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/setup.cfg
+-rw-rw-rw-   0        0        0      862 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/sly/
+-rw-rw-rw-   0        0        0      109 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/sly/__init__.py
+-rw-rw-rw-   0        0        0      777 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/sly/ast.py
+-rw-rw-rw-   0        0        0    16752 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/sly/lex.py
+-rw-rw-rw-   0        0        0    89289 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/sly/yacc.py
```

### Comparing `mindsdb_sql-0.6.6/PKG-INFO` & `mindsdb_sql-0.6.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mindsdb_sql
-Version: 0.6.6
+Version: 0.6.7
 Summary: Pure python SQL parser
 Home-page: https://github.com/mindsdb/mindsdb_sql
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb_sql
 Description: UNKNOWN
```

### Comparing `mindsdb_sql-0.6.6/README.md` & `mindsdb_sql-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/__init__.py` & `mindsdb_sql-0.6.7/mindsdb_sql/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/__init__.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/alter_table.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/alter_table.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/base.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/base.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/create.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/create.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/delete.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/delete.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/describe.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/describe.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/drop.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/drop.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/explain.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/explain.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/insert.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/insert.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/__init__.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/case.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/case.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/common_table_expression.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/common_table_expression.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/constant.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/constant.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/identifier.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/identifier.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/join.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/join.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/native_query.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/native_query.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/operation.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/operation.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/order_by.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/order_by.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/select.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/select.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/tuple.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/tuple.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/type_cast.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/type_cast.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/union.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/union.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/set.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/set.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/show.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/show.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/update.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/update.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/use.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/use.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/__init__.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/chatbot.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/chatbot.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/create_database.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/create_database.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/create_file.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/create_file.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/create_job.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/create_job.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/create_view.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/create_view.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/drop_job.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/drop_job.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/evaluate.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/evaluate.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/lexer.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/parser.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,21 +104,27 @@
 
     @_('DROP CHATBOT identifier')
     def drop_chat_bot(self, p):
         return DropChatBot(name=p.identifier)
 
     # -- triggers --
     @_('CREATE TRIGGER identifier ON identifier LPAREN raw_query RPAREN')
+    @_('CREATE TRIGGER identifier ON identifier COLUMNS ordering_terms LPAREN raw_query RPAREN')
     def create_trigger(self, p):
         query_str = tokens_to_string(p.raw_query)
 
+        columns = None
+        if hasattr(p, 'ordering_terms'):
+            columns = [i.field for i in p.ordering_terms]
+
         return CreateTrigger(
             name=p.identifier0,
             table=p.identifier1,
-            query_str=query_str
+            query_str=query_str,
+            columns=columns
         )
 
     @_('DROP TRIGGER identifier')
     def drop_trigger(self, p):
         return DropTrigger(name=p.identifier)
```

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/trigger.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/trigger.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,39 +5,51 @@
 
 
 class CreateTrigger(ASTNode):
     def __init__(self,
                  name,
                  table,
                  query_str,
+                 columns=None,
                  *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.name = name
         self.table = table
         self.query_str = query_str
+        self.columns = columns
 
     def to_tree(self, *args, level=0, **kwargs):
         ind = indent(level)
         ind1 = indent(level+1)
         name_str = f'\n{ind1}name={self.name.to_string()},'
 
         table_str = f'\n{ind1}table={self.table.to_string()},'
 
         query_str = f'\n{ind1}query_str={repr(self.query_str)},'
 
+        columns_str = ''
+        if self.columns:
+            columns_str = ', '.join([k.to_string() for k in self.columns])
+            columns_str = f'\n{ind1}columns=[{columns_str}],'
+
         out_str = f'{ind}CreateTrigger(' \
                   f'{name_str}' \
                   f'{table_str}' \
+                  f'{columns_str}' \
                   f'{query_str}' \
                   f'\n{ind})'
         return out_str
 
     def get_string(self, *args, **kwargs):
+        columns_str = ''
+        if self.columns:
+            columns_str = ', '.join([k.to_string() for k in self.columns])
+            columns_str = f' columns {columns_str}'
 
-        out_str = f'CREATE TRIGGER {self.name.to_string()} ON {self.table.to_string()} ({self.query_str})'
+        out_str = f'CREATE TRIGGER {self.name.to_string()} ON {self.table.to_string()}{columns_str} ({self.query_str})'
         return out_str
 
 
 class DropTrigger(Drop):
     def __init__(self,
                  name,
                  *args, **kwargs):
```

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mysql/lexer.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mysql/lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mysql/parser.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mysql/parser.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mysql/show_index.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mysql/show_index.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mysql/variable.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mysql/variable.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/lexer.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/logger.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/logger.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/parser.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/parser.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/parser/utils.py` & `mindsdb_sql-0.6.7/mindsdb_sql/parser/utils.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/planner/query_plan.py` & `mindsdb_sql-0.6.7/mindsdb_sql/planner/query_plan.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/planner/query_planner.py` & `mindsdb_sql-0.6.7/mindsdb_sql/planner/query_planner.py`

 * *Files 0% similar despite different names*

```diff
@@ -694,15 +694,15 @@
             integration = self.default_namespace
             if len(table.parts) > 0:
                 if table.parts[0] in self.databases:
                     integration = table.parts.pop(0)
                 else:
                     integration = self.default_namespace
 
-            if integration is None:
+            if integration is None and not hasattr(table, 'sub_select'):
                 raise PlanningException(f'Integration not found for: {table}')
 
             sub_select = getattr(table, 'sub_select', None)
 
             return dict(
                 integration=integration,
                 table=table,
@@ -833,14 +833,15 @@
                     if predictor_info.get('timeseries'):
                         raise NotImplementedError("TS predictor is not supported here yet")
                     data_step = step_stack[-1]
                     predictor_step = self.plan.add_step(ApplyPredictorStep(
                         namespace=item['integration'],
                         dataframe=data_step.result,
                         predictor=table_name,
+                        params=query.using
                     ))
                     step_stack.append(predictor_step)
                 else:
                     # is table
 
                     query2 = Select(from_table=table_name, targets=[Star()])
                     # parts = tuple(map(str.lower, table_name.parts))
@@ -921,84 +922,95 @@
         # get aliases from select target
         aliased_fields = {}
         for target in targets:
             if target.alias is not None:
                 aliased_fields[target.alias.to_string()] = target
         return aliased_fields
 
-    def plan_join(self, query, integration=None):
+    def adapt_dbt_query(self, query, integration):
         orig_query = query
 
         join = query.from_table
         join_left = join.left
-        join_right = join.right
-
-        if isinstance(join_left, Select) and isinstance(join_left.from_table, Identifier):
-            # dbt query.
 
-            # move latest into subquery
-            moved_conditions = []
+        # dbt query.
 
-            def move_latest(node, **kwargs):
-                if isinstance(node, BinaryOperation):
-                    if Latest() in node.args:
-                        for arg in node.args:
-                            if isinstance(arg, Identifier):
-                                # remove table alias
-                                arg.parts = [arg.parts[-1]]
-                        moved_conditions.append(node)
+        # move latest into subquery
+        moved_conditions = []
 
-            query_traversal(query.where, move_latest)
-
-            # TODO make project step from query.target
+        def move_latest(node, **kwargs):
+            if isinstance(node, BinaryOperation):
+                if Latest() in node.args:
+                    for arg in node.args:
+                        if isinstance(arg, Identifier):
+                            # remove table alias
+                            arg.parts = [arg.parts[-1]]
+                    moved_conditions.append(node)
+
+        query_traversal(query.where, move_latest)
+
+        # TODO make project step from query.target
+
+        # TODO support complex query. Only one table is supported at the moment.
+        # if not isinstance(join_left.from_table, Identifier):
+        #     raise PlanningException(f'Statement not supported: {query.to_string()}')
+
+        # move properties to upper query
+        query = join_left
+
+        if query.from_table.alias is not None:
+            table_alias = [query.from_table.alias.parts[0]]
+        else:
+            table_alias = query.from_table.parts
+
+        # add latest to query.where
+        for cond in moved_conditions:
+            if query.where is not None:
+                query.where = BinaryOperation('and', args=[query.where, cond])
+            else:
+                query.where = cond
 
-            # TODO support complex query. Only one table is supported at the moment.
-            # if not isinstance(join_left.from_table, Identifier):
-            #     raise PlanningException(f'Statement not supported: {query.to_string()}')
+        def add_aliases(node, is_table, **kwargs):
+            if not is_table and isinstance(node, Identifier):
+                if len(node.parts) == 1:
+                    # add table alias to field
+                    node.parts = table_alias + node.parts
+
+        query_traversal(query.where, add_aliases)
+
+        if isinstance(query.from_table, Identifier):
+            # DBT workaround: allow use tables without integration.
+            #   if table.part[0] not in integration - take integration name from create table command
+            if (
+                integration is not None
+                and query.from_table.parts[0] not in self.databases
+            ):
+                # add integration name to table
+                query.from_table.parts.insert(0, integration)
+
+        join_left = join_left.from_table
+
+        if orig_query.limit is not None:
+            if query.limit is None or query.limit.value > orig_query.limit.value:
+                query.limit = orig_query.limit
+        query.parentheses = False
+        query.alias = None
 
-            # move properties to upper query
-            query = join_left
+        return query, join_left
 
-            if query.from_table.alias is not None:
-                table_alias = [query.from_table.alias.parts[0]]
-            else:
-                table_alias = query.from_table.parts
+    def plan_join(self, query, integration=None):
+        orig_query = query
 
-            # add latest to query.where
-            for cond in moved_conditions:
-                if query.where is not None:
-                    query.where = BinaryOperation('and', args=[query.where, cond])
-                else:
-                    query.where = cond
+        join = query.from_table
+        join_left = join.left
+        join_right = join.right
 
-            def add_aliases(node, is_table, **kwargs):
-                if not is_table and isinstance(node, Identifier):
-                    if len(node.parts) == 1:
-                        # add table alias to field
-                        node.parts = table_alias + node.parts
-
-            query_traversal(query.where, add_aliases)
-
-            if isinstance(query.from_table, Identifier):
-                # DBT workaround: allow use tables without integration.
-                #   if table.part[0] not in integration - take integration name from create table command
-                if (
-                    integration is not None
-                    and query.from_table.parts[0] not in self.databases
-                ):
-                    # add integration name to table
-                    query.from_table.parts.insert(0, integration)
-
-            join_left = join_left.from_table
-
-            if orig_query.limit is not None:
-                if query.limit is None or query.limit.value > orig_query.limit.value:
-                    query.limit = orig_query.limit
-            query.parentheses = False
-            query.alias = None
+        if isinstance(join_left, Select) and isinstance(join_left.from_table, Identifier):
+            if self.is_predictor(join_right) and self.get_predictor(join_right).get('timeseries'):
+                query, join_left = self.adapt_dbt_query(query, integration)
 
         aliased_fields = self.get_aliased_fields(query.targets)
 
         recursively_check_join_identifiers_for_ambiguity(query.where)
         recursively_check_join_identifiers_for_ambiguity(query.group_by, aliased_fields=aliased_fields)
         recursively_check_join_identifiers_for_ambiguity(query.having)
         recursively_check_join_identifiers_for_ambiguity(query.order_by, aliased_fields=aliased_fields)
```

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/planner/query_prepare.py` & `mindsdb_sql-0.6.7/mindsdb_sql/planner/query_prepare.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/planner/step_result.py` & `mindsdb_sql-0.6.7/mindsdb_sql/planner/step_result.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/planner/steps.py` & `mindsdb_sql-0.6.7/mindsdb_sql/planner/steps.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/planner/ts_utils.py` & `mindsdb_sql-0.6.7/mindsdb_sql/planner/ts_utils.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/planner/utils.py` & `mindsdb_sql-0.6.7/mindsdb_sql/planner/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import copy
 
 from mindsdb_sql.exceptions import PlanningException
 from mindsdb_sql.parser.ast import (Identifier, Operation, Star, Select, BinaryOperation, Constant,
-                                    OrderBy, BetweenOperation, NullConstant, TypeCast, Parameter)
+                                    OrderBy, UnaryOperation, NullConstant, TypeCast, Parameter)
 from mindsdb_sql.parser import ast
 
 
 def get_integration_path_from_identifier(identifier):
     parts = identifier.parts
     integration_name = parts[0]
     new_parts = parts[1:]
@@ -40,14 +40,21 @@
     return new_identifier
 
 def recursively_extract_column_values(op, row_dict, predictor):
     if isinstance(op, BinaryOperation) and op.op == '=':
         id = op.args[0]
         value = op.args[1]
 
+        if (
+            isinstance(value, UnaryOperation)
+            and value.op == '-'
+            and isinstance(value.args[0], Constant)
+        ):
+            value = Constant(-value.args[0].value)
+
         if not (
                 isinstance(id, Identifier)
                 and
                 (isinstance(value, Constant) or isinstance(value, Parameter))
         ):
             raise PlanningException(f'The WHERE clause for selecting from a predictor'
                                     f' must contain pairs \'Identifier(...) = Constant(...)\','
```

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql/render/sqlalchemy_render.py` & `mindsdb_sql-0.6.7/mindsdb_sql/render/sqlalchemy_render.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/mindsdb_sql.egg-info/SOURCES.txt` & `mindsdb_sql-0.6.7/mindsdb_sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/setup.py` & `mindsdb_sql-0.6.7/setup.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/sly/ast.py` & `mindsdb_sql-0.6.7/sly/ast.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.6/sly/lex.py` & `mindsdb_sql-0.6.7/sly/lex.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,14 +298,16 @@
 
             if isinstance(value, str):
                 pattern = value
 
             elif callable(value):
                 cls._token_funcs[tokname] = value
                 pattern = getattr(value, 'pattern')
+            else:
+                continue
 
             # Form the regular expression component
             part = f'(?P<{tokname}>{pattern})'
 
             # Make sure the individual regex compiles properly
             try:
                 cpat = cls.regex_module.compile(part, cls.reflags)
```

### Comparing `mindsdb_sql-0.6.6/sly/yacc.py` & `mindsdb_sql-0.6.7/sly/yacc.py`

 * *Files identical despite different names*

