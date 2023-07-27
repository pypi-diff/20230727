# Comparing `tmp/morningstar_data-1.3.3.tar.gz` & `tmp/morningstar_data-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morningstar_data-1.3.3.tar", max compression
+gzip compressed data, was "morningstar_data-1.4.0.tar", max compression
```

## Comparing `morningstar_data-1.3.3.tar` & `morningstar_data-1.4.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0      558 2023-07-20 19:16:43.881025 morningstar_data-1.3.3/LICENSE
--rw-r--r--   0        0        0    11417 2023-07-20 19:16:43.881025 morningstar_data-1.3.3/README.md
--rw-r--r--   0        0        0      207 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/__init__.py
--rw-r--r--   0        0        0      599 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/_base.py
--rw-r--r--   0        0        0     3056 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/_utils.py
--rw-r--r--   0        0        0       82 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/_version.py
--rw-r--r--   0        0        0       61 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/datalake/__init__.py
--rw-r--r--   0        0        0       62 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/datalake/_data_objects/__init__.py
--rw-r--r--   0        0        0      556 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/datalake/_data_objects/_file.py
--rw-r--r--   0        0        0      762 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/datalake/_data_objects/_table.py
--rw-r--r--   0        0        0      996 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/datalake/_data_objects/csvfile.py
--rw-r--r--   0        0        0     2163 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/datalake/_data_objects/temptable.py
--rw-r--r--   0        0        0      552 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/datalake/_error_messages.py
--rw-r--r--   0        0        0      936 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/datalake/_exceptions.py
--rw-r--r--   0        0        0     5620 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/datalake/base.py
--rw-r--r--   0        0        0      939 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/__init__.py
--rw-r--r--   0        0        0     2433 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_api.py
--rw-r--r--   0        0        0      179 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_backend_apis/__init__.py
--rw-r--r--   0        0        0     1845 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_backend_apis/_delivery_backend.py
--rw-r--r--   0        0        0     4801 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_backend_apis/_holdings_backend.py
--rw-r--r--   0        0        0     3361 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_backend_apis/_signed_url_backend.py
--rw-r--r--   0        0        0     3762 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_base_api.py
--rw-r--r--   0        0        0     4947 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_config.py
--rw-r--r--   0        0        0     1999 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_config_key.py
--rw-r--r--   0        0        0     7583 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_core_api.py
--rw-r--r--   0        0        0      197 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_data_objects/__init__.py
--rw-r--r--   0        0        0     2298 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_data_objects/_custom_data_points_types.py
--rw-r--r--   0        0        0    26357 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_data_objects/_data_points_object.py
--rw-r--r--   0        0        0     7532 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_data_objects/_investments_object.py
--rw-r--r--   0        0        0     2572 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_data_point.py
--rw-r--r--   0        0        0     1051 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_data_type.py
--rw-r--r--   0        0        0     1593 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_decorator.py
--rw-r--r--   0        0        0    13892 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_error_messages.py
--rw-r--r--   0        0        0     3463 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_exceptions.py
--rw-r--r--   0        0        0        0 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_investment/__init__.py
--rw-r--r--   0        0        0     4288 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_investment/_asset_flow_data.py
--rw-r--r--   0        0        0     1546 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_investment/_common.py
--rw-r--r--   0        0        0     6085 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_investment/_data.py
--rw-r--r--   0        0        0     8369 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_investment/_normal_data.py
--rw-r--r--   0        0        0     5023 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_investment/_peer_group_data.py
--rw-r--r--   0        0        0      162 2023-07-20 19:16:43.889025 morningstar_data-1.3.3/morningstar_data/direct/_portfolio/__init__.py
--rw-r--r--   0        0        0     1272 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/direct/_portfolio/_common.py
--rw-r--r--   0        0        0     7859 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py
--rw-r--r--   0        0        0     7913 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/direct/_portfolio/_portfolio_settings.py
--rw-r--r--   0        0        0      955 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/direct/_portfolio/_portfolio_type.py
--rw-r--r--   0        0        0    10975 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/direct/_portfolio_data_set.py
--rw-r--r--   0        0        0     3357 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/direct/_utils.py
--rw-r--r--   0        0        0    13061 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/direct/asset_flow.py
--rw-r--r--   0        0        0    16274 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/direct/custom_database.py
--rw-r--r--   0        0        0     1236 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/direct/data_type.py
--rw-r--r--   0        0        0    42539 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/direct/holdings.py
--rw-r--r--   0        0        0    13577 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/direct/investment.py
--rw-r--r--   0        0        0    32223 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/direct/lookup.py
--rw-r--r--   0        0        0     6040 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/direct/peer_group.py
--rw-r--r--   0        0        0    19389 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/direct/performance_report.py
--rw-r--r--   0        0        0    37181 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/direct/portfolio.py
--rw-r--r--   0        0        0    12562 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/direct/returns.py
--rw-r--r--   0        0        0      413 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/direct/user_items/__init__.py
--rw-r--r--   0        0        0      742 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/direct/user_items/_utils.py
--rw-r--r--   0        0        0     7888 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/direct/user_items/data_set.py
--rw-r--r--   0        0        0    12981 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/direct/user_items/investment_lists.py
--rw-r--r--   0        0        0    11145 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/direct/user_items/portfolio.py
--rw-r--r--   0        0        0    10308 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/direct/user_items/search_criteria.py
--rw-r--r--   0        0        0     4752 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/lookup.py
--rw-r--r--   0        0        0      157 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/utils/__init__.py
--rw-r--r--   0        0        0     6359 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/utils/_delivery_config.py
--rw-r--r--   0        0        0     7752 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/utils/_helpers.py
--rw-r--r--   0        0        0    10435 2023-07-20 19:16:43.893025 morningstar_data-1.3.3/morningstar_data/utils/delivery.py
--rw-r--r--   0        0        0     2530 2023-07-20 19:18:06.356974 morningstar_data-1.3.3/pyproject.toml
--rw-r--r--   0        0        0    12526 1970-01-01 00:00:00.000000 morningstar_data-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0      558 2023-07-26 23:58:11.764858 morningstar_data-1.4.0/LICENSE
+-rw-r--r--   0        0        0    11417 2023-07-26 23:58:11.768858 morningstar_data-1.4.0/README.md
+-rw-r--r--   0        0        0      207 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/__init__.py
+-rw-r--r--   0        0        0      599 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/_base.py
+-rw-r--r--   0        0        0     3056 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/_utils.py
+-rw-r--r--   0        0        0       82 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/_version.py
+-rw-r--r--   0        0        0       61 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/datalake/__init__.py
+-rw-r--r--   0        0        0       62 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/datalake/_data_objects/__init__.py
+-rw-r--r--   0        0        0      556 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/datalake/_data_objects/_file.py
+-rw-r--r--   0        0        0      762 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/datalake/_data_objects/_table.py
+-rw-r--r--   0        0        0      996 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/datalake/_data_objects/csvfile.py
+-rw-r--r--   0        0        0     2163 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/datalake/_data_objects/temptable.py
+-rw-r--r--   0        0        0      552 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/datalake/_error_messages.py
+-rw-r--r--   0        0        0      936 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/datalake/_exceptions.py
+-rw-r--r--   0        0        0     5620 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/datalake/base.py
+-rw-r--r--   0        0        0      939 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/__init__.py
+-rw-r--r--   0        0        0     2433 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_api.py
+-rw-r--r--   0        0        0      179 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_backend_apis/__init__.py
+-rw-r--r--   0        0        0     1845 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_backend_apis/_delivery_backend.py
+-rw-r--r--   0        0        0     4801 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_backend_apis/_holdings_backend.py
+-rw-r--r--   0        0        0     3361 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_backend_apis/_signed_url_backend.py
+-rw-r--r--   0        0        0     3762 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_base_api.py
+-rw-r--r--   0        0        0     4947 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_config.py
+-rw-r--r--   0        0        0     1999 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_config_key.py
+-rw-r--r--   0        0        0     7583 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_core_api.py
+-rw-r--r--   0        0        0      197 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_data_objects/__init__.py
+-rw-r--r--   0        0        0     2298 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_data_objects/_custom_data_points_types.py
+-rw-r--r--   0        0        0    26357 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_data_objects/_data_points_object.py
+-rw-r--r--   0        0        0     7532 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_data_objects/_investments_object.py
+-rw-r--r--   0        0        0     2572 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_data_point.py
+-rw-r--r--   0        0        0     1051 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_data_type.py
+-rw-r--r--   0        0        0     1593 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_decorator.py
+-rw-r--r--   0        0        0    13886 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_error_messages.py
+-rw-r--r--   0        0        0     3463 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_investment/__init__.py
+-rw-r--r--   0        0        0     4288 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_investment/_asset_flow_data.py
+-rw-r--r--   0        0        0     1546 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_investment/_common.py
+-rw-r--r--   0        0        0     6085 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_investment/_data.py
+-rw-r--r--   0        0        0     8369 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_investment/_normal_data.py
+-rw-r--r--   0        0        0     5023 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_investment/_peer_group_data.py
+-rw-r--r--   0        0        0      162 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_portfolio/__init__.py
+-rw-r--r--   0        0        0     1272 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_portfolio/_common.py
+-rw-r--r--   0        0        0     7859 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py
+-rw-r--r--   0        0        0     7913 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_portfolio/_portfolio_settings.py
+-rw-r--r--   0        0        0      955 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_portfolio/_portfolio_type.py
+-rw-r--r--   0        0        0    10975 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_portfolio_data_set.py
+-rw-r--r--   0        0        0     3357 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/_utils.py
+-rw-r--r--   0        0        0    13061 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/asset_flow.py
+-rw-r--r--   0        0        0    16274 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/custom_database.py
+-rw-r--r--   0        0        0     1236 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/data_type.py
+-rw-r--r--   0        0        0    44384 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/holdings.py
+-rw-r--r--   0        0        0    13577 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/investment.py
+-rw-r--r--   0        0        0    32223 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/lookup.py
+-rw-r--r--   0        0        0     6040 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/peer_group.py
+-rw-r--r--   0        0        0    19389 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/performance_report.py
+-rw-r--r--   0        0        0    37181 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/portfolio.py
+-rw-r--r--   0        0        0    12562 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/returns.py
+-rw-r--r--   0        0        0      413 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/user_items/__init__.py
+-rw-r--r--   0        0        0      742 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/user_items/_utils.py
+-rw-r--r--   0        0        0     7888 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/user_items/data_set.py
+-rw-r--r--   0        0        0    12981 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/user_items/investment_lists.py
+-rw-r--r--   0        0        0    11145 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/user_items/portfolio.py
+-rw-r--r--   0        0        0    10308 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/direct/user_items/search_criteria.py
+-rw-r--r--   0        0        0     4752 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/lookup.py
+-rw-r--r--   0        0        0      157 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/utils/__init__.py
+-rw-r--r--   0        0        0     6359 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/utils/_delivery_config.py
+-rw-r--r--   0        0        0     7752 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/utils/_helpers.py
+-rw-r--r--   0        0        0    10435 2023-07-26 23:58:11.776858 morningstar_data-1.4.0/morningstar_data/utils/delivery.py
+-rw-r--r--   0        0        0     2530 2023-07-26 23:59:22.842222 morningstar_data-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    12526 1970-01-01 00:00:00.000000 morningstar_data-1.4.0/PKG-INFO
```

### Comparing `morningstar_data-1.3.3/LICENSE` & `morningstar_data-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/README.md` & `morningstar_data-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/_base.py` & `morningstar_data-1.4.0/morningstar_data/_base.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/_utils.py` & `morningstar_data-1.4.0/morningstar_data/_utils.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/datalake/_data_objects/_file.py` & `morningstar_data-1.4.0/morningstar_data/datalake/_data_objects/_file.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/datalake/_data_objects/_table.py` & `morningstar_data-1.4.0/morningstar_data/datalake/_data_objects/_table.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/datalake/_data_objects/csvfile.py` & `morningstar_data-1.4.0/morningstar_data/datalake/_data_objects/csvfile.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/datalake/_data_objects/temptable.py` & `morningstar_data-1.4.0/morningstar_data/datalake/_data_objects/temptable.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/datalake/_error_messages.py` & `morningstar_data-1.4.0/morningstar_data/datalake/_error_messages.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/datalake/_exceptions.py` & `morningstar_data-1.4.0/morningstar_data/datalake/_exceptions.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/datalake/base.py` & `morningstar_data-1.4.0/morningstar_data/datalake/base.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/__init__.py` & `morningstar_data-1.4.0/morningstar_data/direct/__init__.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_api.py` & `morningstar_data-1.4.0/morningstar_data/direct/_api.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_backend_apis/_delivery_backend.py` & `morningstar_data-1.4.0/morningstar_data/direct/_backend_apis/_delivery_backend.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_backend_apis/_holdings_backend.py` & `morningstar_data-1.4.0/morningstar_data/direct/_backend_apis/_holdings_backend.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_backend_apis/_signed_url_backend.py` & `morningstar_data-1.4.0/morningstar_data/direct/_backend_apis/_signed_url_backend.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_base_api.py` & `morningstar_data-1.4.0/morningstar_data/direct/_base_api.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_config.py` & `morningstar_data-1.4.0/morningstar_data/direct/_config.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_config_key.py` & `morningstar_data-1.4.0/morningstar_data/direct/_config_key.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_core_api.py` & `morningstar_data-1.4.0/morningstar_data/direct/_core_api.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_data_objects/_custom_data_points_types.py` & `morningstar_data-1.4.0/morningstar_data/direct/_data_objects/_custom_data_points_types.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_data_objects/_data_points_object.py` & `morningstar_data-1.4.0/morningstar_data/direct/_data_objects/_data_points_object.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_data_objects/_investments_object.py` & `morningstar_data-1.4.0/morningstar_data/direct/_data_objects/_investments_object.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_data_point.py` & `morningstar_data-1.4.0/morningstar_data/direct/_data_point.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_data_type.py` & `morningstar_data-1.4.0/morningstar_data/direct/_data_type.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_decorator.py` & `morningstar_data-1.4.0/morningstar_data/direct/_decorator.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_error_messages.py` & `morningstar_data-1.4.0/morningstar_data/direct/_error_messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 
 # Add custom bad request error messages here
 BAD_REQUEST_ERROR_NO_START_AND_END_DATE = "Specify `start_date` and `end_date` to proceed with your query."
 BAD_REQUEST_ERROR_NO_END_DATE = "Specify the `end_date` to proceed with your query."
 BAD_REQUEST_ERROR_NO_START_DATE = "Specify the `start_date` to proceed with your query."
 BAD_REQUEST_ERROR_INCLUDE_ALL_DATE = "Specify either date or both start date and end date to proceed with your query."
 BAD_REQUEST_ERROR_INVALID_DATE_FORMAT = "Specify date in the format yyyy-MM-dd to proceed with your query."
-BAD_REQUEST_ERROR_NO_INVESTMENT_IDS = "Specify the `investment_ids` to proceed with your query."
+BAD_REQUEST_ERROR_NO_INVESTMENT_IDS = "Specify the `investments` to proceed with your query."
 BAD_REQUEST_ERROR_NO_PORTFOLIO_DATA = "No matching portfolio data for the given date or date range."
-BAD_REQUEST_ERROR_INVALID_INVESTMENT_ID = "One or more ID's, in the provided list of `investment_ids`, are invalid!"
+BAD_REQUEST_ERROR_INVALID_INVESTMENT_ID = "One or more ID's, in the provided list of `investments`, are invalid!"
 BAD_REQUEST_ERROR_INVALID_INVESTMENT_LIST_ID = "Specify the valid `list_id` to proceed with your query. A `list_id` is a global unique identifier i.e. uuid."
 BAD_REQUEST_ERROR_INVALID_PORTFOLIO_ID = "Specify the valid `portfolio_id` to proceed with your query. A `portfolio_id` is a global unique identifier i.e. uuid."
 BAD_REQUEST_ERROR_INVALID_LOOKTHROUGH_HOLDING_TYPE = "Indexes are not supported as a valid Look-Through holding."
 BAD_REQUEST_ERROR_NO_START_AND_END_DATE = "Please specify `start_date` and `end_date` to proceed with your query."
 BAD_REQUEST_ERROR_NO_END_DATE = "Please specify the `end_date` to proceed with your query."
 BAD_REQUEST_ERROR_DATA_SET = "Please enter a valid format for `data_set_id`. To retrieve your data sets, execute `md.direct.user_items.get_data_sets()` and select a valid `data_set_id`. To retrieve morningstar data sets, execute `md.direct.lookup.get_morningstar_data_sets()` "
 BAD_REQUEST_ERROR_INVALID_DELIVER_CONFIG = "Delivery config is not valid. Check the docs for examples of accepted inputs."
```

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_exceptions.py` & `morningstar_data-1.4.0/morningstar_data/direct/_exceptions.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_investment/_asset_flow_data.py` & `morningstar_data-1.4.0/morningstar_data/direct/_investment/_asset_flow_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_investment/_common.py` & `morningstar_data-1.4.0/morningstar_data/direct/_investment/_common.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_investment/_data.py` & `morningstar_data-1.4.0/morningstar_data/direct/_investment/_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_investment/_normal_data.py` & `morningstar_data-1.4.0/morningstar_data/direct/_investment/_normal_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_investment/_peer_group_data.py` & `morningstar_data-1.4.0/morningstar_data/direct/_investment/_peer_group_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_portfolio/_common.py` & `morningstar_data-1.4.0/morningstar_data/direct/_portfolio/_common.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py` & `morningstar_data-1.4.0/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_portfolio/_portfolio_settings.py` & `morningstar_data-1.4.0/morningstar_data/direct/_portfolio/_portfolio_settings.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_portfolio/_portfolio_type.py` & `morningstar_data-1.4.0/morningstar_data/direct/_portfolio/_portfolio_type.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_portfolio_data_set.py` & `morningstar_data-1.4.0/morningstar_data/direct/_portfolio_data_set.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/_utils.py` & `morningstar_data-1.4.0/morningstar_data/direct/_utils.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/asset_flow.py` & `morningstar_data-1.4.0/morningstar_data/direct/asset_flow.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/custom_database.py` & `morningstar_data-1.4.0/morningstar_data/direct/custom_database.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/data_type.py` & `morningstar_data-1.4.0/morningstar_data/direct/data_type.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/holdings.py` & `morningstar_data-1.4.0/morningstar_data/direct/holdings.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,17 @@
     BAD_REQUEST_ERROR_INVALID_INVESTMENT_ID,
     BAD_REQUEST_ERROR_NO_INVESTMENT_IDS,
     BAD_REQUEST_ERROR_NO_PORTFOLIO_DATA,
     BAD_REQUEST_ERROR_NO_START_DATE,
     BAD_REQUEST_ERROR_INVALID_LOOKTHROUGH_HOLDING_TYPE,
     BAD_REQUEST_ERROR_INVALID_PORTFOLIO_ID,
 )
-from ._exceptions import BadRequestException, NetworkExceptionError
+from ._exceptions import BadRequestException, ValueErrorException
 from ._backend_apis._holdings_backend import HoldingAPIBackend, FoFAPIBackend, AMSAPIBackend
+from ._data_objects import Investments
 
 _config = _Config()
 
 _holding_api_request = HoldingAPIBackend()
 _fof_api_request = FoFAPIBackend()
 _ams_api_request = AMSAPIBackend()
 
@@ -56,32 +57,40 @@
         stacklevel=2,
     )
     return get_holdings(investment_ids, date, start_date, end_date)
 
 
 @_decorator.typechecked
 def get_holdings(
-    investment_ids: List[str],
+    investments: Optional[Union[List[str], str, Dict[str, Any]]] = None,  # Make it required once investment_ids get removed,
     date: Optional[str] = None,
     start_date: Optional[str] = None,
     end_date: Optional[str] = None,
+    investment_ids: Optional[List[str]] = None,
 ) -> DataFrame:
     """Returns holdings for the specified investments and date or date range. If the date is not specified, the function uses the latest portfolio date by default.
 
     Args:
-        investment_ids (:obj:`list`): A list of investment IDs. The investment ID format is SecId;Universe or just SecId.
-            For example: ["F00000YOOK;FO","FOUSA00CFV;FO"] or ["F00000YOOK","FOUSA00CFV"].
+        investments (:obj:`Union`, `required`): Defines the investments to fetch. Input can be:
+
+                * Investment IDs (:obj:`list`, `optional`): Investment identifiers, in the format of SecId;Universe or just SecId. E.g., ["F00000YOOK;FO","FOUSA00CFV;FO"] or ["F00000YOOK","FOUSA00CFV"]. Use the `investments <./lookup.html#morningstar_data.direct.investments>`_ function to discover identifiers.
+                * Investment List ID (:obj:`str`, `optional`): Saved investment list in Morningstar Direct. Currently, this function does not support lists that combine investments and user-created portfolios. Use the `get_investment_lists <./lists.html#morningstar_data.direct.user_items.get_investment_lists>`_ function to discover saved lists.
+                * Search Criteria  ID (:obj:`str`, `optional`): Saved search criteria in Morningstar Direct. Use the `get_search_criteria <./search_criteria.html#morningstar_data.direct.user_items.get_search_criteria>`_ function to discover saved search criteria.
+                * Search Criteria Condition (:obj:`dict`, `optional`): Search criteria definition. See details in the Reference section below or use the `get_search_criteria_conditions <./search_criteria.html#morningstar_data.direct.user_items.get_search_criteria_conditions>`_ function to discover the definition of a saved search criteria.
+
         date (:obj:`str`, `optional`): The portfolio date for which to retrieve data. The format is YYYY-MM-DD.
             For example, "2020-01-01". If a date is provided, then the `start_date` and `end_date` parameters are ignored.
             An exception is thrown if `start_date` or `end_date` is provided along with `date`.
         start_date (:obj:`str`, `optional`): The start date for retrieving data. The format is
             YYYY-MM-DD. For example, "2020-01-01". An exception is thrown if `date` is provided along with `start_date`.
         end_date (:obj:`str`, `optional`): The end date for retrieving data. If no value is provided for
             `end_date`, current date will be used. The format is YYYY-MM-DD. For example, "2020-01-01". An exception is
             thrown if `date` is provided along with `end_date`.
+        investment_ids (:obj:`list`): DEPRECATED, A list of investment IDs. The investment ID format is SecId;Universe or just SecId.
+            For example: ["F00000YOOK;FO","FOUSA00CFV;FO"] or ["F00000YOOK","FOUSA00CFV"].
 
     Returns:
         DataFrame: A DataFrame object with holdings data. DataFrame columns include:
 
         * investmentId
         * masterPortfolioId
         * portfolioDate
@@ -96,40 +105,55 @@
         * marketValue
         * sharesChanged
         * currency
         * ticker
         * detailHoldingType
 
     Raises:
-        ValueErrorException: Raised when the `investment_ids` parameter is invalid.
+        ValueErrorException: Raised when the `investments` parameter is invalid.
 
     Examples:
         Retrieve holdings for investment "FOUSA00KZH" on "2020-12-31".
 
     ::
 
         import morningstar_data as md
 
-        df = md.direct.get_holdings(investment_ids=["FOUSA00KZH"], date="2020-12-31")
+        df = md.direct.get_holdings(investments=["FOUSA00KZH"], date="2020-12-31")
         df
 
     :Output:
         =============  =================  ===  ======  =================
         investmentId   masterPortfolioId  ...  ticker  detailHoldingType
         =============  =================  ===  ======  =================
         FOUSA00KZH     6079               ...  CBRE    EQUITY
         FOUSA00KZH     6079               ...  GOOGL   EQUITY
         ...
         =============  =================  ===  ======  =================
 
     """
-    _validate_investment_ids(investment_ids)
+    if investment_ids is not None:
+        warnings.warn(
+            "The investment_ids argument is deprecated and will be removed in the next major version. Use investments instead",
+            FutureWarning,
+            stacklevel=2,
+        )
+
+    if not investment_ids and not investments:
+        raise BadRequestException(BAD_REQUEST_ERROR_NO_INVESTMENT_IDS) from None
+
+    investment_param = Investments(investments or investment_ids)
+    investment_id_list = investment_param.get_investment_ids()
+
+    if [x for x in investment_id_list if len(x.split(";")[0]) != 10]:
+        raise BadRequestException(BAD_REQUEST_ERROR_INVALID_INVESTMENT_ID) from None
+
     _validate_date(date, start_date, end_date)
 
-    investment_date_info = _get_dates(investment_ids, date, start_date, end_date)
+    investment_date_info = _get_dates(investment_id_list, date, start_date, end_date)
     params = []
     master_portfolio_id_investment_id_dict = defaultdict(list)
     for sec_id, date_info in investment_date_info.items():
         if date_info not in params:
             params.append(date_info)
         master_portfolio_id_investment_id_dict[date_info.get("masterPortfolioId", "")].append(sec_id)
 
@@ -346,21 +370,14 @@
             investment_date_info[sec_id] = {
                 "masterPortfolioId": master_portfolio_id,
                 "portfolioDates": date_list,
             }
     return investment_date_info
 
 
-def _validate_investment_ids(investment_ids: List[str]) -> None:
-    if not investment_ids:
-        raise BadRequestException(BAD_REQUEST_ERROR_NO_INVESTMENT_IDS) from None
-    elif [x for x in investment_ids if len(x.split(";")[0]) != 10]:
-        raise BadRequestException(BAD_REQUEST_ERROR_INVALID_INVESTMENT_ID) from None
-
-
 def _get_ids_from_lake_house(df_lookthrough: pd.DataFrame) -> pd.DataFrame:
     sql = """SELECT distinct
             a.investment_id
             ,a.isin
             ,a.cusip
             ,a.weight
             ,a.marketValue as market_value
```

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/investment.py` & `morningstar_data-1.4.0/morningstar_data/direct/investment.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/lookup.py` & `morningstar_data-1.4.0/morningstar_data/direct/lookup.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/peer_group.py` & `morningstar_data-1.4.0/morningstar_data/direct/peer_group.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/performance_report.py` & `morningstar_data-1.4.0/morningstar_data/direct/performance_report.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/portfolio.py` & `morningstar_data-1.4.0/morningstar_data/direct/portfolio.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/returns.py` & `morningstar_data-1.4.0/morningstar_data/direct/returns.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/user_items/_utils.py` & `morningstar_data-1.4.0/morningstar_data/direct/user_items/_utils.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/user_items/data_set.py` & `morningstar_data-1.4.0/morningstar_data/direct/user_items/data_set.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/user_items/investment_lists.py` & `morningstar_data-1.4.0/morningstar_data/direct/user_items/investment_lists.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/user_items/portfolio.py` & `morningstar_data-1.4.0/morningstar_data/direct/user_items/portfolio.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/direct/user_items/search_criteria.py` & `morningstar_data-1.4.0/morningstar_data/direct/user_items/search_criteria.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/lookup.py` & `morningstar_data-1.4.0/morningstar_data/lookup.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/utils/_delivery_config.py` & `morningstar_data-1.4.0/morningstar_data/utils/_delivery_config.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/utils/_helpers.py` & `morningstar_data-1.4.0/morningstar_data/utils/_helpers.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/morningstar_data/utils/delivery.py` & `morningstar_data-1.4.0/morningstar_data/utils/delivery.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.3/pyproject.toml` & `morningstar_data-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "morningstar_data"
-version = "1.3.3"
+version = "1.4.0"
 description = "Morningstar Data"
 authors = ["Morningstar, Inc."]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://www.morningstar.com/products/md-python-package"
 documentation = "https://docs-analyticslab.morningstar.com/latest/index.html"
```

### Comparing `morningstar_data-1.3.3/PKG-INFO` & `morningstar_data-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morningstar-data
-Version: 1.3.3
+Version: 1.4.0
 Summary: Morningstar Data
 Home-page: https://www.morningstar.com/products/md-python-package
 License: Apache-2.0
 Author: Morningstar, Inc.
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

