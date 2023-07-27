# Comparing `tmp/morningstar_data-1.4.0.tar.gz` & `tmp/morningstar_data-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morningstar_data-1.4.0.tar", max compression
+gzip compressed data, was "morningstar_data-1.5.0.tar", max compression
```

## Comparing `morningstar_data-1.4.0.tar` & `morningstar_data-1.5.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0      558 2023-07-26 23:58:11.764858 morningstar_data-1.4.0/LICENSE
--rw-r--r--   0        0        0    11417 2023-07-26 23:58:11.768858 morningstar_data-1.4.0/README.md
--rw-r--r--   0        0        0      207 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/__init__.py
--rw-r--r--   0        0        0      599 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/_base.py
--rw-r--r--   0        0        0     3056 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/_utils.py
--rw-r--r--   0        0        0       82 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/_version.py
--rw-r--r--   0        0        0       61 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/datalake/__init__.py
--rw-r--r--   0        0        0       62 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/datalake/_data_objects/__init__.py
--rw-r--r--   0        0        0      556 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/datalake/_data_objects/_file.py
--rw-r--r--   0        0        0      762 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/datalake/_data_objects/_table.py
--rw-r--r--   0        0        0      996 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/datalake/_data_objects/csvfile.py
--rw-r--r--   0        0        0     2163 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/datalake/_data_objects/temptable.py
--rw-r--r--   0        0        0      552 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/datalake/_error_messages.py
--rw-r--r--   0        0        0      936 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/datalake/_exceptions.py
--rw-r--r--   0        0        0     5620 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/datalake/base.py
--rw-r--r--   0        0        0      939 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/__init__.py
--rw-r--r--   0        0        0     2433 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_api.py
--rw-r--r--   0        0        0      179 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_backend_apis/__init__.py
--rw-r--r--   0        0        0     1845 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_backend_apis/_delivery_backend.py
--rw-r--r--   0        0        0     4801 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_backend_apis/_holdings_backend.py
--rw-r--r--   0        0        0     3361 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_backend_apis/_signed_url_backend.py
--rw-r--r--   0        0        0     3762 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_base_api.py
--rw-r--r--   0        0        0     4947 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_config.py
--rw-r--r--   0        0        0     1999 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_config_key.py
--rw-r--r--   0        0        0     7583 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_core_api.py
--rw-r--r--   0        0        0      197 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_data_objects/__init__.py
--rw-r--r--   0        0        0     2298 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_data_objects/_custom_data_points_types.py
--rw-r--r--   0        0        0    26357 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_data_objects/_data_points_object.py
--rw-r--r--   0        0        0     7532 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_data_objects/_investments_object.py
--rw-r--r--   0        0        0     2572 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_data_point.py
--rw-r--r--   0        0        0     1051 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_data_type.py
--rw-r--r--   0        0        0     1593 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_decorator.py
--rw-r--r--   0        0        0    13886 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_error_messages.py
--rw-r--r--   0        0        0     3463 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_exceptions.py
--rw-r--r--   0        0        0        0 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_investment/__init__.py
--rw-r--r--   0        0        0     4288 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_investment/_asset_flow_data.py
--rw-r--r--   0        0        0     1546 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_investment/_common.py
--rw-r--r--   0        0        0     6085 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_investment/_data.py
--rw-r--r--   0        0        0     8369 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_investment/_normal_data.py
--rw-r--r--   0        0        0     5023 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_investment/_peer_group_data.py
--rw-r--r--   0        0        0      162 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_portfolio/__init__.py
--rw-r--r--   0        0        0     1272 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_portfolio/_common.py
--rw-r--r--   0        0        0     7859 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py
--rw-r--r--   0        0        0     7913 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_portfolio/_portfolio_settings.py
--rw-r--r--   0        0        0      955 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_portfolio/_portfolio_type.py
--rw-r--r--   0        0        0    10975 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_portfolio_data_set.py
--rw-r--r--   0        0        0     3357 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_utils.py
--rw-r--r--   0        0        0    13061 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/asset_flow.py
--rw-r--r--   0        0        0    16274 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/custom_database.py
--rw-r--r--   0        0        0     1236 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/data_type.py
--rw-r--r--   0        0        0    44384 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/holdings.py
--rw-r--r--   0        0        0    13577 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/investment.py
--rw-r--r--   0        0        0    32223 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/lookup.py
--rw-r--r--   0        0        0     6040 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/peer_group.py
--rw-r--r--   0        0        0    19389 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/performance_report.py
--rw-r--r--   0        0        0    37181 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/portfolio.py
--rw-r--r--   0        0        0    12562 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/returns.py
--rw-r--r--   0        0        0      413 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/user_items/__init__.py
--rw-r--r--   0        0        0      742 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/user_items/_utils.py
--rw-r--r--   0        0        0     7888 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/user_items/data_set.py
--rw-r--r--   0        0        0    12981 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/user_items/investment_lists.py
--rw-r--r--   0        0        0    11145 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/user_items/portfolio.py
--rw-r--r--   0        0        0    10308 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/user_items/search_criteria.py
--rw-r--r--   0        0        0     4752 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/lookup.py
--rw-r--r--   0        0        0      157 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/utils/__init__.py
--rw-r--r--   0        0        0     6359 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/utils/_delivery_config.py
--rw-r--r--   0        0        0     7752 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/utils/_helpers.py
--rw-r--r--   0        0        0    10435 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/utils/delivery.py
--rw-r--r--   0        0        0     2530 2023-07-26 23:59:22.842222 morningstar_data-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    12526 1970-01-01 00:00:00.000000 morningstar_data-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      558 2023-07-27 00:18:46.620526 morningstar_data-1.5.0/LICENSE
+-rw-r--r--   0        0        0    11417 2023-07-27 00:18:46.620526 morningstar_data-1.5.0/README.md
+-rw-r--r--   0        0        0      207 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/__init__.py
+-rw-r--r--   0        0        0      599 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/_base.py
+-rw-r--r--   0        0        0     3765 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/_utils.py
+-rw-r--r--   0        0        0       82 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/_version.py
+-rw-r--r--   0        0        0       61 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/datalake/__init__.py
+-rw-r--r--   0        0        0       62 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/datalake/_data_objects/__init__.py
+-rw-r--r--   0        0        0      556 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/datalake/_data_objects/_file.py
+-rw-r--r--   0        0        0      762 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/datalake/_data_objects/_table.py
+-rw-r--r--   0        0        0      996 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/datalake/_data_objects/csvfile.py
+-rw-r--r--   0        0        0     2163 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/datalake/_data_objects/temptable.py
+-rw-r--r--   0        0        0      552 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/datalake/_error_messages.py
+-rw-r--r--   0        0        0      936 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/datalake/_exceptions.py
+-rw-r--r--   0        0        0     5620 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/datalake/base.py
+-rw-r--r--   0        0        0      939 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/__init__.py
+-rw-r--r--   0        0        0     2433 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_api.py
+-rw-r--r--   0        0        0      179 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_backend_apis/__init__.py
+-rw-r--r--   0        0        0     1845 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_backend_apis/_delivery_backend.py
+-rw-r--r--   0        0        0     4801 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_backend_apis/_holdings_backend.py
+-rw-r--r--   0        0        0     3361 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_backend_apis/_signed_url_backend.py
+-rw-r--r--   0        0        0     3762 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_base_api.py
+-rw-r--r--   0        0        0     4947 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_config.py
+-rw-r--r--   0        0        0     1999 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_config_key.py
+-rw-r--r--   0        0        0     7583 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_core_api.py
+-rw-r--r--   0        0        0      197 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_data_objects/__init__.py
+-rw-r--r--   0        0        0     2298 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_data_objects/_custom_data_points_types.py
+-rw-r--r--   0        0        0    26542 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_data_objects/_data_points_object.py
+-rw-r--r--   0        0        0     7532 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_data_objects/_investments_object.py
+-rw-r--r--   0        0        0     2559 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_data_point.py
+-rw-r--r--   0        0        0     1597 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_data_type.py
+-rw-r--r--   0        0        0     1593 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_decorator.py
+-rw-r--r--   0        0        0    13886 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_error_messages.py
+-rw-r--r--   0        0        0     3463 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_investment/__init__.py
+-rw-r--r--   0        0        0     4288 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_investment/_asset_flow_data.py
+-rw-r--r--   0        0        0     1546 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_investment/_common.py
+-rw-r--r--   0        0        0     6085 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_investment/_data.py
+-rw-r--r--   0        0        0     8369 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_investment/_normal_data.py
+-rw-r--r--   0        0        0     5023 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_investment/_peer_group_data.py
+-rw-r--r--   0        0        0      162 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_portfolio/__init__.py
+-rw-r--r--   0        0        0     1272 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_portfolio/_common.py
+-rw-r--r--   0        0        0     7859 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py
+-rw-r--r--   0        0        0     7913 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_portfolio/_portfolio_settings.py
+-rw-r--r--   0        0        0      955 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_portfolio/_portfolio_type.py
+-rw-r--r--   0        0        0    10975 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_portfolio_data_set.py
+-rw-r--r--   0        0        0     3357 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/_utils.py
+-rw-r--r--   0        0        0    14301 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/asset_flow.py
+-rw-r--r--   0        0        0    16274 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/custom_database.py
+-rw-r--r--   0        0        0     1236 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/data_type.py
+-rw-r--r--   0        0        0    44384 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/holdings.py
+-rw-r--r--   0        0        0    15186 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/investment.py
+-rw-r--r--   0        0        0    32223 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/lookup.py
+-rw-r--r--   0        0        0     6040 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/peer_group.py
+-rw-r--r--   0        0        0    19389 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/performance_report.py
+-rw-r--r--   0        0        0    37181 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/portfolio.py
+-rw-r--r--   0        0        0    12562 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/returns.py
+-rw-r--r--   0        0        0      413 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/user_items/__init__.py
+-rw-r--r--   0        0        0      742 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/user_items/_utils.py
+-rw-r--r--   0        0        0     7888 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/user_items/data_set.py
+-rw-r--r--   0        0        0    12981 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/user_items/investment_lists.py
+-rw-r--r--   0        0        0    11145 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/user_items/portfolio.py
+-rw-r--r--   0        0        0    10308 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/direct/user_items/search_criteria.py
+-rw-r--r--   0        0        0     4752 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/lookup.py
+-rw-r--r--   0        0        0      157 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/utils/__init__.py
+-rw-r--r--   0        0        0     6359 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/utils/_delivery_config.py
+-rw-r--r--   0        0        0     7752 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/utils/_helpers.py
+-rw-r--r--   0        0        0    10435 2023-07-27 00:18:46.624526 morningstar_data-1.5.0/morningstar_data/utils/delivery.py
+-rw-r--r--   0        0        0     2530 2023-07-27 00:19:56.785870 morningstar_data-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0    12526 1970-01-01 00:00:00.000000 morningstar_data-1.5.0/PKG-INFO
```

### Comparing `morningstar_data-1.4.0/LICENSE` & `morningstar_data-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/README.md` & `morningstar_data-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/_base.py` & `morningstar_data-1.5.0/morningstar_data/_base.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/_utils.py` & `morningstar_data-1.5.0/morningstar_data/_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import logging
 import requests
 import inspect
 
 
 from typing import Optional, Union, List, Any, Dict, Callable
 from .direct._config import _Config
+from .direct._api import _direct_api_request
 
 
 _config = _Config()
 _logger = logging.getLogger(__name__)
 
 
 def get_parameter(key: str) -> Optional[Any]:
@@ -93,7 +94,20 @@
         elif stk.function not in ["get_log_flag", "wrapper"] or stk.function.startswith("_"):
             log_flag = False
             return log_flag
         else:
             continue
 
     return log_flag
+
+
+def _get_user_cells_quota() -> Dict:
+    url = f"{_config.asset_service_url()}/auto/analyticslab/log"
+    response_json = _direct_api_request("get", url)
+    user_cells_quota = {"daily_cell_limit": response_json["max"], "daily_cell_remaining": response_json["remains"]}
+    return user_cells_quota
+
+def _get_data_points_total_columns(data_point_details: list) -> int:
+    url = f"{_config.data_point_service_url()}v1/datapoints/columns"
+    columns_response_json: List[Any] = _direct_api_request("POST", url, json.dumps(data_point_details, ignore_nan=True))
+    total_columns = sum(item.get("columns") for item in columns_response_json)
+    return total_columns
```

### Comparing `morningstar_data-1.4.0/morningstar_data/datalake/_data_objects/_file.py` & `morningstar_data-1.5.0/morningstar_data/datalake/_data_objects/_file.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/datalake/_data_objects/_table.py` & `morningstar_data-1.5.0/morningstar_data/datalake/_data_objects/_table.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/datalake/_data_objects/csvfile.py` & `morningstar_data-1.5.0/morningstar_data/datalake/_data_objects/csvfile.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/datalake/_data_objects/temptable.py` & `morningstar_data-1.5.0/morningstar_data/datalake/_data_objects/temptable.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/datalake/_error_messages.py` & `morningstar_data-1.5.0/morningstar_data/datalake/_error_messages.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/datalake/_exceptions.py` & `morningstar_data-1.5.0/morningstar_data/datalake/_exceptions.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/datalake/base.py` & `morningstar_data-1.5.0/morningstar_data/datalake/base.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/__init__.py` & `morningstar_data-1.5.0/morningstar_data/direct/__init__.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_api.py` & `morningstar_data-1.5.0/morningstar_data/direct/_api.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_backend_apis/_delivery_backend.py` & `morningstar_data-1.5.0/morningstar_data/direct/_backend_apis/_delivery_backend.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_backend_apis/_holdings_backend.py` & `morningstar_data-1.5.0/morningstar_data/direct/_backend_apis/_holdings_backend.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_backend_apis/_signed_url_backend.py` & `morningstar_data-1.5.0/morningstar_data/direct/_backend_apis/_signed_url_backend.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_base_api.py` & `morningstar_data-1.5.0/morningstar_data/direct/_base_api.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_config.py` & `morningstar_data-1.5.0/morningstar_data/direct/_config.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_config_key.py` & `morningstar_data-1.5.0/morningstar_data/direct/_config_key.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_core_api.py` & `morningstar_data-1.5.0/morningstar_data/direct/_core_api.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_data_objects/_custom_data_points_types.py` & `morningstar_data-1.5.0/morningstar_data/direct/_data_objects/_custom_data_points_types.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_data_objects/_data_points_object.py` & `morningstar_data-1.5.0/morningstar_data/direct/_data_objects/_data_points_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,14 +235,17 @@
         if "isTsdp" not in settings_data_frame.columns:
             settings_data_frame["isTsdp"] = None
         settings_data_frame = settings_data_frame.where(settings_data_frame.notnull(), None)
         default_settings = _get_data_point_details(settings_data_frame[["datapointId", "isTsdp"]].to_dict(orient="records"))
         if default_settings and isinstance(default_settings, list):
             settings = self._replace_value(default_settings, settings_data_frame)
             request_builder = _data_point_request_builder(settings)
+            for data_point in request_builder:
+                if data_point.get("isTsdp") == True and "frequency" not in data_point:
+                    data_point["frequency"] = "m"
         return request_builder
 
     def _handle_special_data_point_columns(self, settings_data_frame: pd.DataFrame) -> None:
         """
         For values in the columns "windowType", "windowSize", "stepSize" in the settings dataframe, replace empty values with None
         """
         convert_columns = ["windowType", "windowSize", "stepSize"]
@@ -258,15 +261,14 @@
 
         settings_data_frame = settings_data_frame.apply(self._set_alias, axis=1)
         settings_data_frame = settings_data_frame.where(settings_data_frame.notnull(), None)
 
         # separate data points
         asset_flow_data_points = settings_data_frame[settings_data_frame["datapointId"].isin(ALL_ASSET_FLOW_DATA_POINTS)].reset_index().drop(["index"], axis=1)
         normal_data_points = settings_data_frame[~settings_data_frame["datapointId"].isin(ALL_ASSET_FLOW_DATA_POINTS)].reset_index().drop(["index"], axis=1)
-
         alias_data_point_dict = dict()
         if not asset_flow_data_points.empty:
             default_settings = _get_asset_flow_data_points_by_ids(asset_flow_data_points["datapointId"].tolist())
             if default_settings:
                 asset_flow_list = self._replace_asset_flow_settings(default_settings, asset_flow_data_points)
                 alias_data_point_dict.update({x.get("alias"): x for x in asset_flow_list})
```

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_data_objects/_investments_object.py` & `morningstar_data-1.5.0/morningstar_data/direct/_data_objects/_investments_object.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_data_point.py` & `morningstar_data-1.5.0/morningstar_data/direct/_data_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 
 def _data_point_request_builder(data_point_details: list) -> List[Any]:
     if not data_point_details:
         raise ValueErrorException("No datapoint available.")
     url = f"{_config.data_point_service_url()}v1/datapoints/datapointrequestbuilder"
     response_json: List[Any] = _direct_api_request("POST", url, json.dumps(data_point_details, ignore_nan=True))
+
     return response_json
 
 
 def _request_asset_flow_data_points() -> List[Any]:
     url = f"{_config.securitydata_service_url()}v1/assetflow/datapoints"
     response_json: List[Any] = _direct_api_request("GET", url)
     return response_json
@@ -46,17 +47,15 @@
     url = f"{_config.data_point_service_url()}v1/datapoints/detail"
     response_json: List[Dict[Any, Any]] = _direct_api_request("POST", url, json.dumps(params, ignore_nan=True))
     data_point_id_list = [
         "OS010",
         "OS01Z",
         "OS245",
     ]  # This is a temporary list of faulty data points. These datapoints will be removed in the future after which we wont have to specifically check for these data points.
-    filtered_json_response: List[Dict[Any, Any]] = list(
-        filter(lambda x: x.get("canBeAddedToDataset", False) or x["datapointId"] in data_point_id_list, response_json)
-    )
+    filtered_json_response: List[Dict[Any, Any]] = list(filter(lambda x: x.get("canBeAddedToDataset", False) or x["datapointId"] in data_point_id_list, response_json))
     return filtered_json_response
 
 
 @_decorator.error_handler
 def _get_all_universes() -> DataFrame:
     url = f"{_config.data_point_service_url()}v1/universes"
     response_json = _direct_api_request("GET", url)
```

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_decorator.py` & `morningstar_data-1.5.0/morningstar_data/direct/_decorator.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_error_messages.py` & `morningstar_data-1.5.0/morningstar_data/direct/_error_messages.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_exceptions.py` & `morningstar_data-1.5.0/morningstar_data/direct/_exceptions.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_investment/_asset_flow_data.py` & `morningstar_data-1.5.0/morningstar_data/direct/_investment/_asset_flow_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_investment/_common.py` & `morningstar_data-1.5.0/morningstar_data/direct/_investment/_common.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_investment/_data.py` & `morningstar_data-1.5.0/morningstar_data/direct/_investment/_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_investment/_normal_data.py` & `morningstar_data-1.5.0/morningstar_data/direct/_investment/_normal_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_investment/_peer_group_data.py` & `morningstar_data-1.5.0/morningstar_data/direct/_investment/_peer_group_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_portfolio/_common.py` & `morningstar_data-1.5.0/morningstar_data/direct/_portfolio/_common.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py` & `morningstar_data-1.5.0/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_portfolio/_portfolio_settings.py` & `morningstar_data-1.5.0/morningstar_data/direct/_portfolio/_portfolio_settings.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_portfolio/_portfolio_type.py` & `morningstar_data-1.5.0/morningstar_data/direct/_portfolio/_portfolio_type.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_portfolio_data_set.py` & `morningstar_data-1.5.0/morningstar_data/direct/_portfolio_data_set.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/_utils.py` & `morningstar_data-1.5.0/morningstar_data/direct/_utils.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/asset_flow.py` & `morningstar_data-1.5.0/morningstar_data/direct/asset_flow.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 from . import _decorator, _utils, _error_messages
 from .._base import _logger
 from ._config import _Config
 from ._data_objects import Investments
 from ._data_point import _request_asset_flow_data_points
 from ._exceptions import BadRequestException, QueryLimitException, ResourceNotFoundError
 from ._base_api import APIBackend
+from .._utils import _get_user_cells_quota, _get_data_points_total_columns
+from ._data_type import DryRunResults
+
 
 _config = _Config()
 
 
 class AssetFlowAPIBackend(APIBackend):
     """
     Subclass to call the Asset Flow Data API and handle any HTTP errors that occur.
@@ -160,32 +163,44 @@
 
 
 @_decorator.typechecked
 def get_asset_flow(
     market_id: str,
     data_point_settings: DataFrame,
     investments: Optional[Union[List[str], str, Dict[str, Any]]] = None,
-) -> DataFrame:
+    dry_run: Optional[bool] = False,
+) -> Union[DataFrame, DryRunResults]:
     """Get asset flow data for a market of investments or specific investments within a market.
 
     Args:
-        investments (:obj:`Union`, `required`): Defines the investments to fetch. Input can be:
+        market_id(:obj:`str`): A numeric code representing a broad market of investments. For example, the code for "US Open-end & ETF ex MM ex FoF" is "5". Use the `get_asset_flow_markets <./assetflow.html#morningstar_data.direct.get_asset_flow_markets>`_ function to retrieve a full list of codes.
+
+        data_point_settings(:obj:`DataFrame`): A DataFrame of data points with defined settings. Each row represents a data point. Each column is a configurable setting. This DataFrame can be obtained by `retrieving asset flow data points <./assetflow.html#morningstar_data.direct.get_asset_flow_data_points>`_, or by `retrieving data point settings <./lookup.html#morningstar_data.direct.get_data_point_settings>`_.
+
+        investments(:obj:`Union`, `required`): Defines the investments to fetch. Input can be:
 
             * Investment IDs (:obj:`list`, `optional`): Investment identifiers, in the format of SecId;Universe or just SecId. E.g., ["F00000YOOK;FO","FOUSA00CFV;FO"] or ["F00000YOOK","FOUSA00CFV"]. Use the `investments <./lookup.html#morningstar_data.direct.investments>`_ function to discover identifiers.
             * Investment List ID (:obj:`str`, `optional`): Saved investment list in Morningstar Direct. Use the `get_investment_lists <./lists.html#morningstar_data.direct.user_items.get_investment_lists>`_ function to discover saved lists.
             * Search Criteria  ID (:obj:`str`, `optional`): Saved search criteria in Morningstar Direct. Use the `get_search_criteria <./search_criteria.html#morningstar_data.direct.user_items.get_search_criteria>`_ function to discover saved search criteria.
             * Search Criteria Condition (:obj:`dict`, `optional`): Search criteria definition. See details in the Reference section of `get_investment_data <./investment.html#morningstar_data.direct.get_investment_data>`_ or use the `get_search_criteria_conditions <./search_criteria.html#morningstar_data.direct.user_items.get_search_criteria_conditions>`_ function to discover the definition of a saved search criteria.
 
-        market_id(:obj:`str`): A numeric code representing a broad market of investments. For example, the code for "US Open-end & ETF ex MM ex FoF" is "5". Use the `get_asset_flow_markets <./assetflow.html#morningstar_data.direct.get_asset_flow_markets>`_ function to retrieve a full list of codes.
-        data_point_settings(:obj:`DataFrame`): A DataFrame of data points with defined settings. Each row represents a data point. Each column is a configurable setting. This DataFrame can be obtained by `retrieving asset flow data points <./assetflow.html#morningstar_data.direct.get_asset_flow_data_points>`_, or by `retrieving data point settings <./lookup.html#morningstar_data.direct.get_data_point_settings>`_.
+        dry_run(:obj:`bool`, `optional`): When True, the query will not be executed. Instead, a DryRunResults object will be returned with details about the query's impact on daily cell limit usage.
 
     Returns:
         DataFrame: A DataFrame object with asset flow data. DataFrame columns include `investmentId` and data point names, as
         provided in `data_point_settings`.
 
+        or
+
+        DryRunResults: Returned if dry_run=True is passed
+          estimated_cells_used: Number of cells by this query
+          daily_cells_remaining_before: How many cells are remaining in your daily cell limit before running this query
+          daily_cells_remaining_after: How many cells would be remaining in your daily cell limit after running this query
+          daily_cell_limit: Your total daily cell limit
+
     :Examples:
 
     ::
 
         import morningstar_data as md
         import pandas
 
@@ -225,23 +240,31 @@
         NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
 
         ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
 
     """
     if data_point_settings.empty:
         raise BadRequestException("data_point_settings is required.")
-
     investment_id_list: List[Any] = []
 
     if investments is not None:
         investment_object = Investments(investments)
         investment_id_list = investment_object.get_investment_ids()
 
     data_point_settings = data_point_settings.where(data_point_settings.notnull(), None)
     data_point_list = data_point_settings.to_dict(orient="records")
+
+    if dry_run:
+        estimated_cells_used = _get_data_points_total_columns(data_point_list) * len(investment_id_list)
+        user_cells_quota = _get_user_cells_quota()
+        dry_run_results = DryRunResults(
+            estimated_cells_used=estimated_cells_used, daily_cells_remaining_before=user_cells_quota["daily_cell_remaining"], daily_cell_limit=user_cells_quota["daily_cell_limit"]
+        )
+        return dry_run_results
+
     postbody = {"marketId": market_id, "datapoints": data_point_list}
     if investment_id_list is not None:
         postbody["investments"] = list(map(lambda x: {"id": _remove_univ(x)}, investment_id_list))
     return _get_data(postbody)
 
 
 def _get_data(data: dict) -> DataFrame:
```

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/custom_database.py` & `morningstar_data-1.5.0/morningstar_data/direct/custom_database.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/data_type.py` & `morningstar_data-1.5.0/morningstar_data/direct/data_type.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/holdings.py` & `morningstar_data-1.5.0/morningstar_data/direct/holdings.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/investment.py` & `morningstar_data-1.5.0/morningstar_data/direct/investment.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from .._base import _logger
 from ._data_objects import Investments, InvestmentType, DataPoints, DataPointsType
 
 from ._investment._asset_flow_data import AssetFlowProvider
 from ._investment._normal_data import NormalDataProvider
 from ._investment._common import _get_data_points, _get_data_point_col_names
 
+from .._utils import _get_user_cells_quota, _get_data_points_total_columns
+from ._data_type import DryRunResults
+
 
 @_decorator.typechecked
 def investment_data(
     investments: Union[List[str], str, Dict[str, Any]],
     datapoints: Union[List[Dict[str, Any]], str, DataFrame],
 ) -> DataFrame:
     warnings.warn(
@@ -36,15 +39,16 @@
 # exception handling so that we don't have these types of special cases where error_handler is only allowed on some
 # methods but not others.
 @_decorator.typechecked
 def get_investment_data(
     investments: Union[List[str], str, Dict[str, Any]],
     data_points: Optional[Union[List[Dict[str, Any]], str, DataFrame, List[Any]]] = None,
     display_name: bool = False,
-) -> DataFrame:
+    dry_run: Optional[bool] = False,
+) -> Union[DataFrame, DryRunResults]:
     """Retrieve data for the specified investments and data points.
 
     Args:
         investments (:obj:`Union`, `required`): Defines the investments to fetch. Input can be:
 
             * Investment IDs (:obj:`list`, `optional`): Investment identifiers, in the format of SecId;Universe or just SecId. E.g., ["F00000YOOK;FO","FOUSA00CFV;FO"] or ["F00000YOOK","FOUSA00CFV"]. Use the `investments <./lookup.html#morningstar_data.direct.investments>`_ function to discover identifiers.
             * Investment List ID (:obj:`str`, `optional`): Saved investment list in Morningstar Direct. Currently, this function does not support lists that combine investments and user-created portfolios. Use the `get_investment_lists <./lists.html#morningstar_data.direct.user_items.get_investment_lists>`_ function to discover saved lists.
@@ -55,16 +59,26 @@
 
             * Data Point IDs (:obj:`List[Dict]`, `optional`): A list of dictionaries, each defining a data point and its (optional) associated settings.
             * Data Set ID (:obj:`str`, `optional`): Morningstar data set or user-created data set saved in Morningstar Direct. Use the `get_data_sets <./data_set.html#morningstar_data.direct.user_items.get_data_sets>`_ or `get_morningstar_data_sets <./data_set.html#morningstar_data.direct.get_morningstar_data_sets>`_ functions to discover saved data sets.
             * Data Point Settings (:obj:`DataFrame`, `optional`): A DataFrame of data point identifiers and their associated settings. Use the `get_data_set_details <./data_set.html#morningstar_data.direct.user_items.get_data_set_details>`_ function to discover data point settings from a saved data set.
 
         display_name (:obj:`bool`, `optional`): When true, the returned column names will match display names saved in the data set. Default is false.
 
+        dry_run(:obj:`bool`, `optional`): When True, the query will not be executed. Instead, a DryRunResults object will be returned with details about the query's impact on daily cell limit usage.
+
     Returns:
-        DataFrame: A DataFrame object with investment data.
+        DataFrame: A DataFrame object with investment data
+
+        or
+
+        DryRunResults: Returned if dry_run=True is passed
+          estimated_cells_used: Number of cells by this query
+          daily_cells_remaining_before: How many cells are remaining in your daily cell limit before running this query
+          daily_cells_remaining_after: How many cells would be remaining in your daily cell limit after running this query
+          daily_cell_limit: Your total daily cell limit
 
     :Reference:
 
         Constructing a Search Criteria Condition dictionary:
 
         For example::
 
@@ -221,22 +235,35 @@
         1  FOUSA06UWL;CZ    Columbia Trust Stable Income Fund      88.8333                        ...  90.7781
         =  ===============  =====================================  =============================  ===  =============================
 
 
 
 
     """
-    result = _get_investment_data(investments=investments, data_points=data_points, display_name=display_name)
+
+    result = _get_investment_data(investments=investments, data_points=data_points, display_name=display_name, dry_run=dry_run)
     return result
 
 
-def _get_investment_data(investments: InvestmentType, data_points: DataPointsType, display_name: bool = False) -> DataFrame:
+def _get_investment_data(investments: InvestmentType, data_points: DataPointsType, display_name: bool = False, dry_run: Optional[bool] = False) -> Union[DataFrame, DryRunResults]:
     investment_param = Investments(investments)
     data_point_param = DataPoints(data_points)
 
+    if dry_run:
+        investment_id_list = investment_param.get_investment_ids()
+        data_point_settings = data_point_param.get_data_points()
+        data_point_settings = data_point_settings.where(data_point_settings.notnull(), None)
+        data_point_list = data_point_settings.to_dict(orient="records")
+        estimated_cells_used = _get_data_points_total_columns(data_point_list) * len(investment_id_list)
+        user_cells_quota = _get_user_cells_quota()
+        dry_run_results = DryRunResults(
+            estimated_cells_used=estimated_cells_used, daily_cells_remaining_before=user_cells_quota["daily_cell_remaining"], daily_cell_limit=user_cells_quota["daily_cell_limit"]
+        )
+        return dry_run_results
+
     # Get asset flow data
     asset_flow_req = AssetFlowProvider.build_request(investment_param, data_point_param, display_name)
     asset_flow_result = AssetFlowProvider.run_request(asset_flow_req)
 
     # Get normal data
     normal_data_req = NormalDataProvider.build_request(investment_param, data_point_param, display_name)
     normal_data_result = NormalDataProvider.run_request(normal_data_req)
```

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/lookup.py` & `morningstar_data-1.5.0/morningstar_data/direct/lookup.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/peer_group.py` & `morningstar_data-1.5.0/morningstar_data/direct/peer_group.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/performance_report.py` & `morningstar_data-1.5.0/morningstar_data/direct/performance_report.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/portfolio.py` & `morningstar_data-1.5.0/morningstar_data/direct/portfolio.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/returns.py` & `morningstar_data-1.5.0/morningstar_data/direct/returns.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/user_items/_utils.py` & `morningstar_data-1.5.0/morningstar_data/direct/user_items/_utils.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/user_items/data_set.py` & `morningstar_data-1.5.0/morningstar_data/direct/user_items/data_set.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/user_items/investment_lists.py` & `morningstar_data-1.5.0/morningstar_data/direct/user_items/investment_lists.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/user_items/portfolio.py` & `morningstar_data-1.5.0/morningstar_data/direct/user_items/portfolio.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/direct/user_items/search_criteria.py` & `morningstar_data-1.5.0/morningstar_data/direct/user_items/search_criteria.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/lookup.py` & `morningstar_data-1.5.0/morningstar_data/lookup.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/utils/_delivery_config.py` & `morningstar_data-1.5.0/morningstar_data/utils/_delivery_config.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/utils/_helpers.py` & `morningstar_data-1.5.0/morningstar_data/utils/_helpers.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/morningstar_data/utils/delivery.py` & `morningstar_data-1.5.0/morningstar_data/utils/delivery.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.4.0/pyproject.toml` & `morningstar_data-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "morningstar_data"
-version = "1.4.0"
+version = "1.5.0"
 description = "Morningstar Data"
 authors = ["Morningstar, Inc."]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://www.morningstar.com/products/md-python-package"
 documentation = "https://docs-analyticslab.morningstar.com/latest/index.html"
```

### Comparing `morningstar_data-1.4.0/PKG-INFO` & `morningstar_data-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morningstar-data
-Version: 1.4.0
+Version: 1.5.0
 Summary: Morningstar Data
 Home-page: https://www.morningstar.com/products/md-python-package
 License: Apache-2.0
 Author: Morningstar, Inc.
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

