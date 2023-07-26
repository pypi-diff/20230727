# Comparing `tmp/omni-pro-0.1.24.tar.gz` & `tmp/omni-pro-0.1.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omni-pro-0.1.24.tar", last modified: Mon Jul 24 15:50:00 2023, max compression
+gzip compressed data, was "omni-pro-0.1.25.tar", last modified: Wed Jul 26 21:58:32 2023, max compression
```

## Comparing `omni-pro-0.1.24.tar` & `omni-pro-0.1.25.tar`

### file list

```diff
@@ -1,332 +1,341 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:50:00.022239 omni-pro-0.1.24/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-24 15:49:32.000000 omni-pro-0.1.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-24 15:50:00.022239 omni-pro-0.1.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-24 15:49:32.000000 omni-pro-0.1.24/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:59.978238 omni-pro-0.1.24/omni/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:59.982238 omni-pro-0.1.24/omni/pro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/cloudmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:59.982238 omni-pro-0.1.24/omni/pro/data/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/data/models.user.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21329 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:59.982238 omni-pro-0.1.24/omni/pro/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:59.982238 omni-pro-0.1.24/omni/pro/models/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/common/ms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:59.982238 omni-pro-0.1.24/omni/pro/models/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:59.982238 omni-pro-0.1.24/omni/pro/models/sql/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/catalog/category.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:59.982238 omni-pro-0.1.24/omni/pro/models/sql/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/common/country.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:59.986239 omni-pro-0.1.24/omni/pro/models/sql/rules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/rules/calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/rules/delivery_category.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/rules/delivery_category_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/rules/delivery_locality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/rules/delivery_locality_territory_matrix_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/rules/delivery_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/rules/delivery_method_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/rules/delivery_method_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/rules/delivery_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/rules/schedule_warehouse_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/rules/schedule_work.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/rules/schedule_work_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/rules/schedule_work_schedule_work_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/rules/warehouse_hierarchy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:59.986239 omni-pro-0.1.24/omni/pro/models/sql/stock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/stock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:59.986239 omni-pro-0.1.24/omni/pro/models/sql/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/utilities/country.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/utilities/territory_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/sql/utilities/territory_matrix_values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:59.986239 omni-pro-0.1.24/omni/pro/models/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/models/utilities/country.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:59.986239 omni-pro-0.1.24/omni/pro/protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:59.986239 omni-pro-0.1.24/omni/pro/protos/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/common/base_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/common/base_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/common/base_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/grpc_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:59.986239 omni-pro-0.1.24/omni/pro/protos/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:59.986239 omni-pro-0.1.24/omni/pro/protos/v1/catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/catalogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/catalogs/family_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25046 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/catalogs/family_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    29775 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/catalogs/family_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/catalogs/template_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/catalogs/template_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17751 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/catalogs/template_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:59.990239 omni-pro-0.1.24/omni/pro/protos/v1/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/clients/address_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/clients/address_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/clients/address_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/clients/client_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/clients/client_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/clients/client_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:50:00.002239 omni-pro-0.1.24/omni/pro/protos/v1/rules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/calendar_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/calendar_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/calendar_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/category_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/category_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/category_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_category_category_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_category_category_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_category_category_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_category_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_category_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_category_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_locality_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_locality_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_locality_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_price_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_price_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_price_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_schedule_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_schedule_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_schedule_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_shipper_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_shipper_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_shipper_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_time_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_time_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_time_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/location_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/location_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/location_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/schedule_work_line_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/schedule_work_line_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/schedule_work_line_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/schedule_work_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/schedule_work_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/schedule_work_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/rules/warehouse_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:50:00.010239 omni-pro-0.1.24/omni/pro/protos/v1/sales/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/address_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/address_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/address_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/carrier_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/carrier_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/carrier_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/channel_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/channel_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/channel_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/client_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/client_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/client_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/country_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/country_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/country_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/currency_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/currency_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/currency_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/order_line_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/order_line_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/order_line_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/order_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/order_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/order_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/payment_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/payment_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/payment_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/picking_order_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/picking_order_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/picking_order_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/picking_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/picking_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/picking_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/product_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/product_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/product_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/sale_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/sale_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/sale_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/tax_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/tax_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/tax_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/uom_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/uom_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/uom_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/user_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/user_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/sales/warehouse_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:50:00.014239 omni-pro-0.1.24/omni/pro/protos/v1/stock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/attachment_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/attachment_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/attachment_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/carrier_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/carrier_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/carrier_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/country_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/country_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/country_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/location_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/location_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/location_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/picking_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/picking_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/picking_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/picking_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/picking_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/picking_type_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/procurement_group_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/procurement_group_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/procurement_group_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/product_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/product_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/product_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/quant_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/quant_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/quant_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/route_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/route_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/route_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/rule_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/rule_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/rule_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/stock_move_line_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/stock_move_line_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/stock_move_line_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/stock_move_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/stock_move_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/stock_move_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/uom_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/uom_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/uom_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/user_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/user_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/stock/warehouse_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:50:00.018239 omni-pro-0.1.24/omni/pro/protos/v1/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24713 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/users/user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    31841 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/users/user_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    43955 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/users/user_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:50:00.022239 omni-pro-0.1.24/omni/pro/protos/v1/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/country_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/country_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/country_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/currency_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/currency_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/currency_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/document_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/document_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/document_type_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/language_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/language_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/language_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/model_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/payment_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/payment_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/payment_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/tax_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/tax_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/tax_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/territory_matrix_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/territory_matrix_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/territory_matrix_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/territory_matrix_value_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/timezone_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/timezone_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/timezone_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/uom_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/uom_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/protos/v1/utilities/uom_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:50:00.022239 omni-pro-0.1.24/omni/pro/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/user/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-24 15:49:32.000000 omni-pro-0.1.24/omni/pro/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:50:00.022239 omni-pro-0.1.24/omni_pro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-24 15:49:59.000000 omni-pro-0.1.24/omni_pro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13769 2023-07-24 15:49:59.000000 omni-pro-0.1.24/omni_pro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:49:59.000000 omni-pro-0.1.24/omni_pro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-24 15:49:59.000000 omni-pro-0.1.24/omni_pro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-24 15:49:59.000000 omni-pro-0.1.24/omni_pro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 15:50:00.022239 omni-pro-0.1.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-24 15:49:52.000000 omni-pro-0.1.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.718906 omni-pro-0.1.25/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-26 21:58:01.000000 omni-pro-0.1.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-26 21:58:32.718906 omni-pro-0.1.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-26 21:58:01.000000 omni-pro-0.1.25/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.642902 omni-pro-0.1.25/omni/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.646902 omni-pro-0.1.25/omni/pro/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/cloudmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.646902 omni-pro-0.1.25/omni/pro/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/data/models.user.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21990 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.646902 omni-pro-0.1.25/omni/pro/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.646902 omni-pro-0.1.25/omni/pro/models/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/common/ms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.646902 omni-pro-0.1.25/omni/pro/models/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/custom_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/custom_fields/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.646902 omni-pro-0.1.25/omni/pro/models/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.646902 omni-pro-0.1.25/omni/pro/models/sql/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/catalog/category.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.646902 omni-pro-0.1.25/omni/pro/models/sql/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/common/country.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.650902 omni-pro-0.1.25/omni/pro/models/sql/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/rules/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/rules/delivery_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/rules/delivery_category_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/rules/delivery_locality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/rules/delivery_locality_territory_matrix_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/rules/delivery_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/rules/delivery_method_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/rules/delivery_method_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/rules/delivery_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/rules/schedule_warehouse_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/rules/schedule_work.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/rules/schedule_work_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/rules/schedule_work_schedule_work_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/rules/warehouse_hierarchy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.650902 omni-pro-0.1.25/omni/pro/models/sql/stock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/stock/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.650902 omni-pro-0.1.25/omni/pro/models/sql/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/utilities/country.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/utilities/territory_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/sql/utilities/territory_matrix_values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.650902 omni-pro-0.1.25/omni/pro/models/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/models/utilities/country.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.650902 omni-pro-0.1.25/omni/pro/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.650902 omni-pro-0.1.25/omni/pro/protos/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/common/base_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/common/base_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/common/base_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/grpc_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.650902 omni-pro-0.1.25/omni/pro/protos/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.654902 omni-pro-0.1.25/omni/pro/protos/v1/catalogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/catalogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/catalogs/family_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25046 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/catalogs/family_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    29775 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/catalogs/family_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/catalogs/template_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/catalogs/template_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17751 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/catalogs/template_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.654902 omni-pro-0.1.25/omni/pro/protos/v1/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/clients/address_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/clients/address_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/clients/address_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/clients/client_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/clients/client_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/clients/client_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.686904 omni-pro-0.1.25/omni/pro/protos/v1/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/calendar_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/calendar_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/calendar_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/category_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/category_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/category_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_category_category_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_category_category_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_category_category_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_category_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_category_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_category_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_locality_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_locality_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_locality_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_price_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_price_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_price_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_schedule_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_schedule_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_schedule_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_shipper_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_shipper_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_shipper_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_time_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_time_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_time_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/location_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/location_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/location_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/schedule_work_line_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/schedule_work_line_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/schedule_work_line_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/schedule_work_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/schedule_work_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/schedule_work_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/rules/warehouse_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.698905 omni-pro-0.1.25/omni/pro/protos/v1/sales/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/address_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/address_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/address_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/carrier_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/carrier_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/carrier_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/channel_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/channel_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/channel_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/client_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/client_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/client_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/country_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/country_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/country_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/currency_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/currency_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/currency_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/order_line_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/order_line_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/order_line_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/order_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/order_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/order_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/payment_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/payment_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/payment_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/picking_order_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/picking_order_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/picking_order_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/picking_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/picking_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/picking_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/product_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/product_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/product_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/sale_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/sale_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/sale_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/tax_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/tax_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/tax_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/uom_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/uom_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/uom_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/user_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/user_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/sales/warehouse_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.706905 omni-pro-0.1.25/omni/pro/protos/v1/stock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/attachment_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/attachment_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/attachment_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/carrier_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/carrier_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/carrier_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/country_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/country_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/country_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/location_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/location_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/location_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/picking_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/picking_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/picking_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/picking_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/picking_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/picking_type_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/procurement_group_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/procurement_group_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/procurement_group_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/product_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/product_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/product_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/quant_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/quant_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/quant_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/route_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/route_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/route_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/rule_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/rule_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/rule_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/sequence_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/sequence_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/sequence_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/stock_move_line_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/stock_move_line_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/stock_move_line_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/stock_move_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/stock_move_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/stock_move_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/uom_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/uom_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/uom_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/user_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/user_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/stock/warehouse_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.710905 omni-pro-0.1.25/omni/pro/protos/v1/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24713 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/users/user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31841 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/users/user_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    43955 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/users/user_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.714906 omni-pro-0.1.25/omni/pro/protos/v1/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/country_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/country_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/country_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/currency_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/currency_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/currency_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/document_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/document_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/document_type_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/language_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/language_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/language_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/model_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/payment_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/payment_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/payment_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/sequence_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/sequence_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/sequence_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/tax_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/tax_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/tax_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/territory_matrix_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/territory_matrix_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/territory_matrix_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/territory_matrix_value_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/timezone_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/timezone_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/timezone_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/uom_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/uom_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/protos/v1/utilities/uom_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.714906 omni-pro-0.1.25/omni/pro/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/user/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-26 21:58:01.000000 omni-pro-0.1.25/omni/pro/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:58:32.718906 omni-pro-0.1.25/omni_pro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-26 21:58:32.000000 omni-pro-0.1.25/omni_pro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14119 2023-07-26 21:58:32.000000 omni-pro-0.1.25/omni_pro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:58:32.000000 omni-pro-0.1.25/omni_pro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-26 21:58:32.000000 omni-pro-0.1.25/omni_pro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-26 21:58:32.000000 omni-pro-0.1.25/omni_pro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 21:58:32.718906 omni-pro-0.1.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-26 21:58:24.000000 omni-pro-0.1.25/setup.py
```

### Comparing `omni-pro-0.1.24/LICENSE` & `omni-pro-0.1.25/LICENSE`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/PKG-INFO` & `omni-pro-0.1.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omni-pro
-Version: 0.1.24
+Version: 0.1.25
 Summary: Python library designed to be a utility for OMS microservices
 Home-page: https://github.com/Omnipro-Solutions/saas-ms-library
 Author: OMNI.PRO
 Author-email: development@omni.pro
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `omni-pro-0.1.24/README.md` & `omni-pro-0.1.25/README.md`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/aws.py` & `omni-pro-0.1.25/omni/pro/aws.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/cloudmap.py` & `omni-pro-0.1.25/omni/pro/cloudmap.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/config.py` & `omni-pro-0.1.25/omni/pro/config.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/database.py` & `omni-pro-0.1.25/omni/pro/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -383,14 +383,16 @@
             ">": "$gt",
             "<": "$lt",
             ">=": "$gte",
             "<=": "$lte",
             "in": "$in",
             "nin": "$nin",
             "!=": "$ne",
+            "!like": "$not",
+            "like": "$regex",
         }
 
     def is_logical_operator(self, token):
         if not isinstance(token, str):
             return False
         return token in self.operators_logical
 
@@ -410,15 +412,20 @@
             if self.is_logical_operator(token):
                 operator_stack.append(token)
             elif self.is_comparison_operator(token):
                 operator_stack.append(token)
             elif self.is_tuple(token):
                 field, old_operator, value = token
                 if old_operator in self.operators_comparison:
-                    operand_stack.append({field: {self.operators_comparison[old_operator]: value}})
+                    options = {}
+                    if old_operator == "like":
+                        options = {"$options": "i"}
+                    elif old_operator == "!like":
+                        options = {self.operators_comparison[old_operator]: {"$regex": value, "$options": "i"}}
+                    operand_stack.append({field: {self.operators_comparison[old_operator]: value} | options})
                 else:
                     raise ValueError(f"Unexpected operator: {old_operator}")
             else:
                 raise ValueError(f"Unexpected token: {token}")
 
         while operator_stack:
             operator = operator_stack.pop()
@@ -447,14 +454,18 @@
         prepared_statement = {}
         prepared_statement["paginated"] = {"page": paginated.offset, "per_page": paginated.limit or 10}
         if (ft := filter.ListFields()) or id:
             expression = [("_id", "=", cls.generate_object_id(id))]
             if ft:
                 str_filter = filter.filter.replace("true", "True").replace("false", "False")
                 expression = ast.literal_eval(str_filter)
+                # reemplace filter id by _id and convert to ObjectId
+                for idx, exp in enumerate(expression):
+                    if isinstance(exp, tuple) and len(exp) == 3 and exp[0] == "id":
+                        expression[idx] = ("_id", exp[1], cls.generate_object_id(exp[2]))
             filter_custom = PolishNotationToMongoDB(expression=expression).convert()
             prepared_statement["filter"] = filter_custom
         if group_by:
             prepared_statement["group_by"] = [x.name_field for x in group_by]
         if sort_by.ListFields():
             prepared_statement["sort_by"] = [cls.db_trans_sort(sort_by)]
         return prepared_statement
```

### Comparing `omni-pro-0.1.24/omni/pro/decorators.py` & `omni-pro-0.1.25/omni/pro/decorators.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/initial.py` & `omni-pro-0.1.25/omni/pro/initial.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/logger.py` & `omni-pro-0.1.25/omni/pro/logger.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/models/base.py` & `omni-pro-0.1.25/omni/pro/models/base.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/models/sql/common/country.py` & `omni-pro-0.1.25/omni/pro/models/sql/common/country.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/models/sql/rules/delivery_category.py` & `omni-pro-0.1.25/omni/pro/models/sql/rules/delivery_category.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/models/sql/rules/delivery_category_category.py` & `omni-pro-0.1.25/omni/pro/models/sql/rules/delivery_category_category.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/models/sql/rules/delivery_locality.py` & `omni-pro-0.1.25/omni/pro/models/sql/rules/delivery_locality.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/models/sql/rules/delivery_locality_territory_matrix_values.py` & `omni-pro-0.1.25/omni/pro/models/sql/rules/delivery_locality_territory_matrix_values.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/models/sql/rules/delivery_method.py` & `omni-pro-0.1.25/omni/pro/models/sql/rules/delivery_method.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/models/sql/rules/delivery_method_ref.py` & `omni-pro-0.1.25/omni/pro/models/sql/rules/delivery_method_ref.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/models/sql/rules/delivery_method_warehouse.py` & `omni-pro-0.1.25/omni/pro/models/sql/rules/delivery_method_warehouse.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/models/sql/rules/delivery_schedule.py` & `omni-pro-0.1.25/omni/pro/models/sql/rules/delivery_schedule.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/models/sql/rules/schedule_warehouse_hierarchy.py` & `omni-pro-0.1.25/omni/pro/models/sql/rules/schedule_warehouse_hierarchy.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/models/sql/rules/schedule_work.py` & `omni-pro-0.1.25/omni/pro/models/sql/rules/schedule_work.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/models/sql/rules/schedule_work_line.py` & `omni-pro-0.1.25/omni/pro/models/sql/rules/schedule_work_line.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/models/sql/rules/schedule_work_schedule_work_line.py` & `omni-pro-0.1.25/omni/pro/models/sql/rules/schedule_work_schedule_work_line.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/models/sql/rules/warehouse_hierarchy.py` & `omni-pro-0.1.25/omni/pro/models/sql/rules/warehouse_hierarchy.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/models/utilities/country.py` & `omni-pro-0.1.25/omni/pro/models/utilities/country.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/common/base_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/common/base_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/common/base_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/common/base_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/grpc_connector.py` & `omni-pro-0.1.25/omni/pro/protos/grpc_connector.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/response.py` & `omni-pro-0.1.25/omni/pro/protos/response.py`

 * *Files 6% similar despite different names*

```diff
@@ -192,10 +192,13 @@
                 message=msg_success,
                 total=total,
                 count=len(list_docs),
                 id=request.id,
                 paginated=request.paginated,
                 **kwargs_return,
             )
+    except ValueError as e:
+        LoggerTraceback.error("Input request data validation error", e, logger)
+        return message_response.input_validator_response(message=str(e))
     except Exception as e:
         LoggerTraceback.error(msg_exception, e, logger)
         return message_response.internal_response(message=msg_exception)
```

### Comparing `omni-pro-0.1.24/omni/pro/protos/util.py` & `omni-pro-0.1.25/omni/pro/protos/util.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/catalogs/family_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/catalogs/family_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/catalogs/family_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/catalogs/family_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/catalogs/family_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/catalogs/family_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/catalogs/template_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/catalogs/template_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/catalogs/template_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/catalogs/template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/catalogs/template_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/catalogs/template_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/clients/address_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/clients/address_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/clients/address_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/clients/address_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/clients/address_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/clients/address_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/clients/client_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/clients/client_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/clients/client_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/clients/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/clients/client_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/clients/client_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/calendar_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/calendar_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/calendar_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/calendar_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/calendar_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/calendar_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/category_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/category_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/category_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/category_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/category_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/category_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_category_category_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_category_category_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_category_category_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_category_category_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_category_category_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_category_category_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_category_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_category_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_category_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_category_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_category_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_category_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_locality_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_locality_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_locality_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_locality_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_locality_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_locality_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_method_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_method_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_method_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_price_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_price_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_price_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_price_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_price_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_price_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_schedule_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_schedule_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_schedule_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_schedule_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_schedule_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_schedule_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_shipper_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_shipper_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_shipper_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_shipper_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_shipper_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_shipper_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_time_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_time_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_time_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_time_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_time_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_time_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/location_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/location_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/location_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/location_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/location_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/location_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/schedule_work_line_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/schedule_work_line_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/schedule_work_line_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/schedule_work_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/schedule_work_line_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/schedule_work_line_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/schedule_work_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/schedule_work_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/schedule_work_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/schedule_work_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/schedule_work_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/schedule_work_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/warehouse_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/warehouse_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/rules/warehouse_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/rules/warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/address_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/address_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/address_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/address_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/address_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/address_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/carrier_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/carrier_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/carrier_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/carrier_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/carrier_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/carrier_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/channel_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/channel_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/channel_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/channel_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/channel_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/client_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/client_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/client_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/client_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/client_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/country_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/country_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/country_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/country_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/country_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/country_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/currency_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/currency_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/currency_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/currency_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/currency_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/currency_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/delivery_method_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/delivery_method_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/delivery_method_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/order_line_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/order_line_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/order_line_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/order_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/order_line_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/order_line_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/order_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/order_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/order_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/order_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/order_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/order_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/payment_method_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/payment_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/payment_method_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/payment_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/payment_method_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/payment_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/picking_order_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/picking_order_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/picking_order_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/picking_order_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/picking_order_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/picking_order_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/picking_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/picking_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/picking_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/picking_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/picking_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/picking_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/product_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/product_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/product_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/product_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/product_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/product_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/sale_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/sale_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/sale_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/sale_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/sale_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/sale_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/tax_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/tax_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/tax_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/tax_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/tax_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/tax_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/uom_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/uom_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/uom_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/uom_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/uom_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/uom_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/user_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/user_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/user_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/user_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/warehouse_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/warehouse_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/sales/warehouse_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/sales/warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/attachment_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/attachment_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/attachment_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/attachment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/attachment_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/attachment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/carrier_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/carrier_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/carrier_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/carrier_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/carrier_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/carrier_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/country_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/country_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/country_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/country_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/country_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/country_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/location_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/location_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/location_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/location_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/location_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/location_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/picking_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/picking_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/picking_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/picking_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/picking_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/picking_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/picking_type_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/picking_type_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1bv1/stock/picking_type.proto\x12&pro.omni.oms.api.v1.stock.picking.type\x1a\x11\x63ommon/base.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xf1\x03\n\x0bPickingType\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rsequence_code\x18\x03 \x01(\t\x12\x14\n\x0cwarehouse_id\x18\x04 \x01(\x05\x12\x0c\n\x04\x63ode\x18\x05 \x01(\t\x12\x1e\n\x16return_picking_type_id\x18\x06 \x01(\x05\x12\x33\n\x0fshow_operations\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x31\n\rshow_reserved\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x1f\n\x17\x64\x65\x66\x61ult_location_src_id\x18\t \x01(\x05\x12 \n\x18\x64\x65\x66\x61ult_location_dest_id\x18\n \x01(\x05\x12\x0e\n\x06prefix\x18\x0b \x01(\t\x12\x0f\n\x07padding\x18\x0c \x01(\x05\x12\x18\n\x10number_increment\x18\r \x01(\x05\x12\x1a\n\x12number_next_actual\x18\x0e \x01(\x05\x12*\n\x06\x61\x63tive\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x10 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xbd\x03\n\x18PickingTypeCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rsequence_code\x18\x02 \x01(\t\x12\x14\n\x0cwarehouse_id\x18\x03 \x01(\x05\x12\x0c\n\x04\x63ode\x18\x04 \x01(\t\x12\x1e\n\x16return_picking_type_id\x18\x05 \x01(\x05\x12\x33\n\x0fshow_operations\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x31\n\rshow_reserved\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x1f\n\x17\x64\x65\x66\x61ult_location_src_id\x18\x08 \x01(\x05\x12 \n\x18\x64\x65\x66\x61ult_location_dest_id\x18\t \x01(\x05\x12\x0e\n\x06prefix\x18\n \x01(\t\x12\x0f\n\x07padding\x18\x0b \x01(\x05\x12\x18\n\x10number_increment\x18\x0c \x01(\x05\x12\x1a\n\x12number_next_actual\x18\r \x01(\x05\x12\x36\n\x07\x63ontext\x18\x0e \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb1\x01\n\x19PickingTypeCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12I\n\x0cpicking_type\x18\x02 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking.type.PickingType"\xf4\x02\n\x16PickingTypeReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xeb\x01\n\x17PickingTypeReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12J\n\rpicking_types\x18\x03 \x03(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking.type.PickingType"\x9d\x01\n\x18PickingTypeUpdateRequest\x12I\n\x0cpicking_type\x18\x01 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking.type.PickingType\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb1\x01\n\x19PickingTypeUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12I\n\x0cpicking_type\x18\x02 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking.type.PickingType"^\n\x18PickingTypeDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"f\n\x19PickingTypeDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\x82\x05\n\x12PickingTypeService\x12\x9a\x01\n\x11PickingTypeCreate\x12@.pro.omni.oms.api.v1.stock.picking.type.PickingTypeCreateRequest\x1a\x41.pro.omni.oms.api.v1.stock.picking.type.PickingTypeCreateResponse"\x00\x12\x94\x01\n\x0fPickingTypeRead\x12>.pro.omni.oms.api.v1.stock.picking.type.PickingTypeReadRequest\x1a?.pro.omni.oms.api.v1.stock.picking.type.PickingTypeReadResponse"\x00\x12\x9a\x01\n\x11PickingTypeUpdate\x12@.pro.omni.oms.api.v1.stock.picking.type.PickingTypeUpdateRequest\x1a\x41.pro.omni.oms.api.v1.stock.picking.type.PickingTypeUpdateResponse"\x00\x12\x9a\x01\n\x11PickingTypeDelete\x12@.pro.omni.oms.api.v1.stock.picking.type.PickingTypeDeleteRequest\x1a\x41.pro.omni.oms.api.v1.stock.picking.type.PickingTypeDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x1bv1/stock/picking_type.proto\x12&pro.omni.oms.api.v1.stock.picking_type\x1a\x11\x63ommon/base.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xf1\x03\n\x0bPickingType\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rsequence_code\x18\x03 \x01(\t\x12\x14\n\x0cwarehouse_id\x18\x04 \x01(\x05\x12\x0c\n\x04\x63ode\x18\x05 \x01(\t\x12\x1e\n\x16return_picking_type_id\x18\x06 \x01(\x05\x12\x33\n\x0fshow_operations\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x31\n\rshow_reserved\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x1f\n\x17\x64\x65\x66\x61ult_location_src_id\x18\t \x01(\x05\x12 \n\x18\x64\x65\x66\x61ult_location_dest_id\x18\n \x01(\x05\x12\x0e\n\x06prefix\x18\x0b \x01(\t\x12\x0f\n\x07padding\x18\x0c \x01(\x05\x12\x18\n\x10number_increment\x18\r \x01(\x05\x12\x1a\n\x12number_next_actual\x18\x0e \x01(\x05\x12*\n\x06\x61\x63tive\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x10 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xbd\x03\n\x18PickingTypeCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rsequence_code\x18\x02 \x01(\t\x12\x14\n\x0cwarehouse_id\x18\x03 \x01(\x05\x12\x0c\n\x04\x63ode\x18\x04 \x01(\t\x12\x1e\n\x16return_picking_type_id\x18\x05 \x01(\x05\x12\x33\n\x0fshow_operations\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x31\n\rshow_reserved\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x1f\n\x17\x64\x65\x66\x61ult_location_src_id\x18\x08 \x01(\x05\x12 \n\x18\x64\x65\x66\x61ult_location_dest_id\x18\t \x01(\x05\x12\x0e\n\x06prefix\x18\n \x01(\t\x12\x0f\n\x07padding\x18\x0b \x01(\x05\x12\x18\n\x10number_increment\x18\x0c \x01(\x05\x12\x1a\n\x12number_next_actual\x18\r \x01(\x05\x12\x36\n\x07\x63ontext\x18\x0e \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb1\x01\n\x19PickingTypeCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12I\n\x0cpicking_type\x18\x02 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking_type.PickingType"\xf4\x02\n\x16PickingTypeReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xeb\x01\n\x17PickingTypeReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12J\n\rpicking_types\x18\x03 \x03(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking_type.PickingType"\x9d\x01\n\x18PickingTypeUpdateRequest\x12I\n\x0cpicking_type\x18\x01 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking_type.PickingType\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb1\x01\n\x19PickingTypeUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12I\n\x0cpicking_type\x18\x02 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking_type.PickingType"^\n\x18PickingTypeDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"f\n\x19PickingTypeDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\x82\x05\n\x12PickingTypeService\x12\x9a\x01\n\x11PickingTypeCreate\x12@.pro.omni.oms.api.v1.stock.picking_type.PickingTypeCreateRequest\x1a\x41.pro.omni.oms.api.v1.stock.picking_type.PickingTypeCreateResponse"\x00\x12\x94\x01\n\x0fPickingTypeRead\x12>.pro.omni.oms.api.v1.stock.picking_type.PickingTypeReadRequest\x1a?.pro.omni.oms.api.v1.stock.picking_type.PickingTypeReadResponse"\x00\x12\x9a\x01\n\x11PickingTypeUpdate\x12@.pro.omni.oms.api.v1.stock.picking_type.PickingTypeUpdateRequest\x1a\x41.pro.omni.oms.api.v1.stock.picking_type.PickingTypeUpdateResponse"\x00\x12\x9a\x01\n\x11PickingTypeDelete\x12@.pro.omni.oms.api.v1.stock.picking_type.PickingTypeDeleteRequest\x1a\x41.pro.omni.oms.api.v1.stock.picking_type.PickingTypeDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.stock.picking_type_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
```

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/picking_type_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/picking_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/picking_type_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/picking_type_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,30 +10,30 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.PickingTypeCreate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.stock.picking.type.PickingTypeService/PickingTypeCreate",
+            "/pro.omni.oms.api.v1.stock.picking_type.PickingTypeService/PickingTypeCreate",
             request_serializer=v1_dot_stock_dot_picking__type__pb2.PickingTypeCreateRequest.SerializeToString,
             response_deserializer=v1_dot_stock_dot_picking__type__pb2.PickingTypeCreateResponse.FromString,
         )
         self.PickingTypeRead = channel.unary_unary(
-            "/pro.omni.oms.api.v1.stock.picking.type.PickingTypeService/PickingTypeRead",
+            "/pro.omni.oms.api.v1.stock.picking_type.PickingTypeService/PickingTypeRead",
             request_serializer=v1_dot_stock_dot_picking__type__pb2.PickingTypeReadRequest.SerializeToString,
             response_deserializer=v1_dot_stock_dot_picking__type__pb2.PickingTypeReadResponse.FromString,
         )
         self.PickingTypeUpdate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.stock.picking.type.PickingTypeService/PickingTypeUpdate",
+            "/pro.omni.oms.api.v1.stock.picking_type.PickingTypeService/PickingTypeUpdate",
             request_serializer=v1_dot_stock_dot_picking__type__pb2.PickingTypeUpdateRequest.SerializeToString,
             response_deserializer=v1_dot_stock_dot_picking__type__pb2.PickingTypeUpdateResponse.FromString,
         )
         self.PickingTypeDelete = channel.unary_unary(
-            "/pro.omni.oms.api.v1.stock.picking.type.PickingTypeService/PickingTypeDelete",
+            "/pro.omni.oms.api.v1.stock.picking_type.PickingTypeService/PickingTypeDelete",
             request_serializer=v1_dot_stock_dot_picking__type__pb2.PickingTypeDeleteRequest.SerializeToString,
             response_deserializer=v1_dot_stock_dot_picking__type__pb2.PickingTypeDeleteResponse.FromString,
         )
 
 
 class PickingTypeServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
@@ -83,15 +83,15 @@
         "PickingTypeDelete": grpc.unary_unary_rpc_method_handler(
             servicer.PickingTypeDelete,
             request_deserializer=v1_dot_stock_dot_picking__type__pb2.PickingTypeDeleteRequest.FromString,
             response_serializer=v1_dot_stock_dot_picking__type__pb2.PickingTypeDeleteResponse.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "pro.omni.oms.api.v1.stock.picking.type.PickingTypeService", rpc_method_handlers
+        "pro.omni.oms.api.v1.stock.picking_type.PickingTypeService", rpc_method_handlers
     )
     server.add_generic_rpc_handlers((generic_handler,))
 
 
 # This class is part of an EXPERIMENTAL API.
 class PickingTypeService(object):
     """Missing associated documentation comment in .proto file."""
@@ -108,15 +108,15 @@
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.stock.picking.type.PickingTypeService/PickingTypeCreate",
+            "/pro.omni.oms.api.v1.stock.picking_type.PickingTypeService/PickingTypeCreate",
             v1_dot_stock_dot_picking__type__pb2.PickingTypeCreateRequest.SerializeToString,
             v1_dot_stock_dot_picking__type__pb2.PickingTypeCreateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
@@ -137,15 +137,15 @@
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.stock.picking.type.PickingTypeService/PickingTypeRead",
+            "/pro.omni.oms.api.v1.stock.picking_type.PickingTypeService/PickingTypeRead",
             v1_dot_stock_dot_picking__type__pb2.PickingTypeReadRequest.SerializeToString,
             v1_dot_stock_dot_picking__type__pb2.PickingTypeReadResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
@@ -166,15 +166,15 @@
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.stock.picking.type.PickingTypeService/PickingTypeUpdate",
+            "/pro.omni.oms.api.v1.stock.picking_type.PickingTypeService/PickingTypeUpdate",
             v1_dot_stock_dot_picking__type__pb2.PickingTypeUpdateRequest.SerializeToString,
             v1_dot_stock_dot_picking__type__pb2.PickingTypeUpdateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
@@ -195,15 +195,15 @@
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.stock.picking.type.PickingTypeService/PickingTypeDelete",
+            "/pro.omni.oms.api.v1.stock.picking_type.PickingTypeService/PickingTypeDelete",
             v1_dot_stock_dot_picking__type__pb2.PickingTypeDeleteRequest.SerializeToString,
             v1_dot_stock_dot_picking__type__pb2.PickingTypeDeleteResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
```

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/procurement_group_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/procurement_group_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n v1/stock/procurement_group.proto\x12+pro.omni.oms.api.v1.stock.procurement.group\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1fgoogle/protobuf/timestamp.proto"\xac\x01\n\x10ProcurementGroup\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\tmove_type\x18\x03 \x01(\t\x12*\n\x06\x61\x63tive\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"x\n\x1dProcurementGroupCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tmove_type\x18\x02 \x01(\t\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc5\x01\n\x1eProcurementGroupCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12X\n\x11procurement_group\x18\x02 \x01(\x0b\x32=.pro.omni.oms.api.v1.stock.procurement.group.ProcurementGroup"\xf9\x02\n\x1bProcurementGroupReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xff\x01\n\x1cProcurementGroupReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12Y\n\x12procurement_groups\x18\x03 \x03(\x0b\x32=.pro.omni.oms.api.v1.stock.procurement.group.ProcurementGroup"\xb1\x01\n\x1dProcurementGroupUpdateRequest\x12X\n\x11procurement_group\x18\x01 \x01(\x0b\x32=.pro.omni.oms.api.v1.stock.procurement.group.ProcurementGroup\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc5\x01\n\x1eProcurementGroupUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12X\n\x11procurement_group\x18\x02 \x01(\x0b\x32=.pro.omni.oms.api.v1.stock.procurement.group.ProcurementGroup"c\n\x1dProcurementGroupDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"k\n\x1eProcurementGroupDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xeb\x05\n\x17ProcurementGroupService\x12\xb3\x01\n\x16ProcurementGroupCreate\x12J.pro.omni.oms.api.v1.stock.procurement.group.ProcurementGroupCreateRequest\x1aK.pro.omni.oms.api.v1.stock.procurement.group.ProcurementGroupCreateResponse"\x00\x12\xad\x01\n\x14ProcurementGroupRead\x12H.pro.omni.oms.api.v1.stock.procurement.group.ProcurementGroupReadRequest\x1aI.pro.omni.oms.api.v1.stock.procurement.group.ProcurementGroupReadResponse"\x00\x12\xb3\x01\n\x16ProcurementGroupUpdate\x12J.pro.omni.oms.api.v1.stock.procurement.group.ProcurementGroupUpdateRequest\x1aK.pro.omni.oms.api.v1.stock.procurement.group.ProcurementGroupUpdateResponse"\x00\x12\xb3\x01\n\x16ProcurementGroupDelete\x12J.pro.omni.oms.api.v1.stock.procurement.group.ProcurementGroupDeleteRequest\x1aK.pro.omni.oms.api.v1.stock.procurement.group.ProcurementGroupDeleteResponse"\x00\x62\x06proto3'
+    b'\n v1/stock/procurement_group.proto\x12+pro.omni.oms.api.v1.stock.procurement_group\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1fgoogle/protobuf/timestamp.proto"\xac\x01\n\x10ProcurementGroup\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\tmove_type\x18\x03 \x01(\t\x12*\n\x06\x61\x63tive\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"x\n\x1dProcurementGroupCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tmove_type\x18\x02 \x01(\t\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc5\x01\n\x1eProcurementGroupCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12X\n\x11procurement_group\x18\x02 \x01(\x0b\x32=.pro.omni.oms.api.v1.stock.procurement_group.ProcurementGroup"\xf9\x02\n\x1bProcurementGroupReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xff\x01\n\x1cProcurementGroupReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12Y\n\x12procurement_groups\x18\x03 \x03(\x0b\x32=.pro.omni.oms.api.v1.stock.procurement_group.ProcurementGroup"\xb1\x01\n\x1dProcurementGroupUpdateRequest\x12X\n\x11procurement_group\x18\x01 \x01(\x0b\x32=.pro.omni.oms.api.v1.stock.procurement_group.ProcurementGroup\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc5\x01\n\x1eProcurementGroupUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12X\n\x11procurement_group\x18\x02 \x01(\x0b\x32=.pro.omni.oms.api.v1.stock.procurement_group.ProcurementGroup"c\n\x1dProcurementGroupDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"k\n\x1eProcurementGroupDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xeb\x05\n\x17ProcurementGroupService\x12\xb3\x01\n\x16ProcurementGroupCreate\x12J.pro.omni.oms.api.v1.stock.procurement_group.ProcurementGroupCreateRequest\x1aK.pro.omni.oms.api.v1.stock.procurement_group.ProcurementGroupCreateResponse"\x00\x12\xad\x01\n\x14ProcurementGroupRead\x12H.pro.omni.oms.api.v1.stock.procurement_group.ProcurementGroupReadRequest\x1aI.pro.omni.oms.api.v1.stock.procurement_group.ProcurementGroupReadResponse"\x00\x12\xb3\x01\n\x16ProcurementGroupUpdate\x12J.pro.omni.oms.api.v1.stock.procurement_group.ProcurementGroupUpdateRequest\x1aK.pro.omni.oms.api.v1.stock.procurement_group.ProcurementGroupUpdateResponse"\x00\x12\xb3\x01\n\x16ProcurementGroupDelete\x12J.pro.omni.oms.api.v1.stock.procurement_group.ProcurementGroupDeleteRequest\x1aK.pro.omni.oms.api.v1.stock.procurement_group.ProcurementGroupDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.stock.procurement_group_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
```

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/procurement_group_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/procurement_group_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/procurement_group_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/procurement_group_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,30 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.ProcurementGroupCreate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.stock.procurement.group.ProcurementGroupService/ProcurementGroupCreate",
+            "/pro.omni.oms.api.v1.stock.procurement_group.ProcurementGroupService/ProcurementGroupCreate",
             request_serializer=v1_dot_stock_dot_procurement__group__pb2.ProcurementGroupCreateRequest.SerializeToString,
             response_deserializer=v1_dot_stock_dot_procurement__group__pb2.ProcurementGroupCreateResponse.FromString,
         )
         self.ProcurementGroupRead = channel.unary_unary(
-            "/pro.omni.oms.api.v1.stock.procurement.group.ProcurementGroupService/ProcurementGroupRead",
+            "/pro.omni.oms.api.v1.stock.procurement_group.ProcurementGroupService/ProcurementGroupRead",
             request_serializer=v1_dot_stock_dot_procurement__group__pb2.ProcurementGroupReadRequest.SerializeToString,
             response_deserializer=v1_dot_stock_dot_procurement__group__pb2.ProcurementGroupReadResponse.FromString,
         )
         self.ProcurementGroupUpdate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.stock.procurement.group.ProcurementGroupService/ProcurementGroupUpdate",
+            "/pro.omni.oms.api.v1.stock.procurement_group.ProcurementGroupService/ProcurementGroupUpdate",
             request_serializer=v1_dot_stock_dot_procurement__group__pb2.ProcurementGroupUpdateRequest.SerializeToString,
             response_deserializer=v1_dot_stock_dot_procurement__group__pb2.ProcurementGroupUpdateResponse.FromString,
         )
         self.ProcurementGroupDelete = channel.unary_unary(
-            "/pro.omni.oms.api.v1.stock.procurement.group.ProcurementGroupService/ProcurementGroupDelete",
+            "/pro.omni.oms.api.v1.stock.procurement_group.ProcurementGroupService/ProcurementGroupDelete",
             request_serializer=v1_dot_stock_dot_procurement__group__pb2.ProcurementGroupDeleteRequest.SerializeToString,
             response_deserializer=v1_dot_stock_dot_procurement__group__pb2.ProcurementGroupDeleteResponse.FromString,
         )
 
 
 class ProcurementGroupServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
@@ -83,15 +83,15 @@
         "ProcurementGroupDelete": grpc.unary_unary_rpc_method_handler(
             servicer.ProcurementGroupDelete,
             request_deserializer=v1_dot_stock_dot_procurement__group__pb2.ProcurementGroupDeleteRequest.FromString,
             response_serializer=v1_dot_stock_dot_procurement__group__pb2.ProcurementGroupDeleteResponse.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "pro.omni.oms.api.v1.stock.procurement.group.ProcurementGroupService", rpc_method_handlers
+        "pro.omni.oms.api.v1.stock.procurement_group.ProcurementGroupService", rpc_method_handlers
     )
     server.add_generic_rpc_handlers((generic_handler,))
 
 
 # This class is part of an EXPERIMENTAL API.
 class ProcurementGroupService(object):
     """Missing associated documentation comment in .proto file."""
@@ -108,15 +108,15 @@
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.stock.procurement.group.ProcurementGroupService/ProcurementGroupCreate",
+            "/pro.omni.oms.api.v1.stock.procurement_group.ProcurementGroupService/ProcurementGroupCreate",
             v1_dot_stock_dot_procurement__group__pb2.ProcurementGroupCreateRequest.SerializeToString,
             v1_dot_stock_dot_procurement__group__pb2.ProcurementGroupCreateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
@@ -137,15 +137,15 @@
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.stock.procurement.group.ProcurementGroupService/ProcurementGroupRead",
+            "/pro.omni.oms.api.v1.stock.procurement_group.ProcurementGroupService/ProcurementGroupRead",
             v1_dot_stock_dot_procurement__group__pb2.ProcurementGroupReadRequest.SerializeToString,
             v1_dot_stock_dot_procurement__group__pb2.ProcurementGroupReadResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
@@ -166,15 +166,15 @@
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.stock.procurement.group.ProcurementGroupService/ProcurementGroupUpdate",
+            "/pro.omni.oms.api.v1.stock.procurement_group.ProcurementGroupService/ProcurementGroupUpdate",
             v1_dot_stock_dot_procurement__group__pb2.ProcurementGroupUpdateRequest.SerializeToString,
             v1_dot_stock_dot_procurement__group__pb2.ProcurementGroupUpdateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
@@ -195,15 +195,15 @@
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.stock.procurement.group.ProcurementGroupService/ProcurementGroupDelete",
+            "/pro.omni.oms.api.v1.stock.procurement_group.ProcurementGroupService/ProcurementGroupDelete",
             v1_dot_stock_dot_procurement__group__pb2.ProcurementGroupDeleteRequest.SerializeToString,
             v1_dot_stock_dot_procurement__group__pb2.ProcurementGroupDeleteResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
```

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/product_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/product_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/product_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/product_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/product_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/product_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/quant_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/quant_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/quant_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/quant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/quant_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/quant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/route_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/route_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/route_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/route_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/route_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/route_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/rule_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/rule_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/rule_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/rule_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/rule_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/rule_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/stock_move_line_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/stock_move_line_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,36 +13,36 @@
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1ev1/stock/stock_move_line.proto\x12$pro.omni.oms.api.v1.stock.stock.line\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1fgoogle/protobuf/timestamp.proto"\xfd\x02\n\rStockMoveLine\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x15\n\rstock_move_id\x18\x02 \x01(\x05\x12\x12\n\npicking_id\x18\x03 \x01(\x05\x12\x0e\n\x06status\x18\x04 \x01(\t\x12\x11\n\treference\x18\x05 \x01(\t\x12(\n\x04\x64\x61te\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06origin\x18\x07 \x01(\t\x12\x12\n\nproduct_id\x18\x08 \x01(\x05\x12\x13\n\x0blocation_id\x18\t \x01(\x05\x12\x18\n\x10location_dest_id\x18\n \x01(\x05\x12\x10\n\x08qty_done\x18\x0b \x01(\x05\x12\x16\n\x0eproduct_uom_id\x18\x0c \x01(\x05\x12*\n\x06\x61\x63tive\x18\r \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x0e \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xc9\x02\n\x1aStockMoveLineCreateRequest\x12\x15\n\rstock_move_id\x18\x01 \x01(\x05\x12\x12\n\npicking_id\x18\x02 \x01(\x05\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x11\n\treference\x18\x04 \x01(\t\x12(\n\x04\x64\x61te\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06origin\x18\x06 \x01(\t\x12\x12\n\nproduct_id\x18\x07 \x01(\x05\x12\x13\n\x0blocation_id\x18\x08 \x01(\x05\x12\x18\n\x10location_dest_id\x18\t \x01(\x05\x12\x10\n\x08qty_done\x18\n \x01(\x05\x12\x16\n\x0eproduct_uom_id\x18\x0b \x01(\x05\x12\x36\n\x07\x63ontext\x18\x0c \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb6\x01\n\x1bStockMoveLineCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12L\n\x0fstock_move_line\x18\x02 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.stock.line.StockMoveLine"\xf6\x02\n\x18StockMoveLineReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xf0\x01\n\x19StockMoveLineReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12M\n\x10stock_move_lines\x18\x03 \x03(\x0b\x32\x33.pro.omni.oms.api.v1.stock.stock.line.StockMoveLine"\xa2\x01\n\x1aStockMoveLineUpdateRequest\x12L\n\x0fstock_move_line\x18\x01 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.stock.line.StockMoveLine\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb6\x01\n\x1bStockMoveLineUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12L\n\x0fstock_move_line\x18\x02 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.stock.line.StockMoveLine"`\n\x1aStockMoveLineDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"h\n\x1bStockMoveLineDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\x84\x05\n\x14StockMoveLineService\x12\x9a\x01\n\x13StockMoveLineCreate\x12@.pro.omni.oms.api.v1.stock.stock.line.StockMoveLineCreateRequest\x1a\x41.pro.omni.oms.api.v1.stock.stock.line.StockMoveLineCreateResponse\x12\x94\x01\n\x11StockMoveLineRead\x12>.pro.omni.oms.api.v1.stock.stock.line.StockMoveLineReadRequest\x1a?.pro.omni.oms.api.v1.stock.stock.line.StockMoveLineReadResponse\x12\x9a\x01\n\x13StockMoveLineUpdate\x12@.pro.omni.oms.api.v1.stock.stock.line.StockMoveLineUpdateRequest\x1a\x41.pro.omni.oms.api.v1.stock.stock.line.StockMoveLineUpdateResponse\x12\x9a\x01\n\x13StockMoveLineDelete\x12@.pro.omni.oms.api.v1.stock.stock.line.StockMoveLineDeleteRequest\x1a\x41.pro.omni.oms.api.v1.stock.stock.line.StockMoveLineDeleteResponseb\x06proto3'
+    b'\n\x1ev1/stock/stock_move_line.proto\x12)pro.omni.oms.api.v1.stock.stock_move_line\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1fgoogle/protobuf/timestamp.proto"\xfd\x02\n\rStockMoveLine\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x15\n\rstock_move_id\x18\x02 \x01(\x05\x12\x12\n\npicking_id\x18\x03 \x01(\x05\x12\x0e\n\x06status\x18\x04 \x01(\t\x12\x11\n\treference\x18\x05 \x01(\t\x12(\n\x04\x64\x61te\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06origin\x18\x07 \x01(\t\x12\x12\n\nproduct_id\x18\x08 \x01(\x05\x12\x13\n\x0blocation_id\x18\t \x01(\x05\x12\x18\n\x10location_dest_id\x18\n \x01(\x05\x12\x10\n\x08qty_done\x18\x0b \x01(\x05\x12\x16\n\x0eproduct_uom_id\x18\x0c \x01(\x05\x12*\n\x06\x61\x63tive\x18\r \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x0e \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xc9\x02\n\x1aStockMoveLineCreateRequest\x12\x15\n\rstock_move_id\x18\x01 \x01(\x05\x12\x12\n\npicking_id\x18\x02 \x01(\x05\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x11\n\treference\x18\x04 \x01(\t\x12(\n\x04\x64\x61te\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06origin\x18\x06 \x01(\t\x12\x12\n\nproduct_id\x18\x07 \x01(\x05\x12\x13\n\x0blocation_id\x18\x08 \x01(\x05\x12\x18\n\x10location_dest_id\x18\t \x01(\x05\x12\x10\n\x08qty_done\x18\n \x01(\x05\x12\x16\n\x0eproduct_uom_id\x18\x0b \x01(\x05\x12\x36\n\x07\x63ontext\x18\x0c \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xbb\x01\n\x1bStockMoveLineCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12Q\n\x0fstock_move_line\x18\x02 \x01(\x0b\x32\x38.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLine"\xf6\x02\n\x18StockMoveLineReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xf5\x01\n\x19StockMoveLineReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12R\n\x10stock_move_lines\x18\x03 \x03(\x0b\x32\x38.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLine"\xa7\x01\n\x1aStockMoveLineUpdateRequest\x12Q\n\x0fstock_move_line\x18\x01 \x01(\x0b\x32\x38.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLine\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xbb\x01\n\x1bStockMoveLineUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12Q\n\x0fstock_move_line\x18\x02 \x01(\x0b\x32\x38.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLine"`\n\x1aStockMoveLineDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"h\n\x1bStockMoveLineDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xac\x05\n\x14StockMoveLineService\x12\xa4\x01\n\x13StockMoveLineCreate\x12\x45.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineCreateRequest\x1a\x46.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineCreateResponse\x12\x9e\x01\n\x11StockMoveLineRead\x12\x43.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineReadRequest\x1a\x44.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineReadResponse\x12\xa4\x01\n\x13StockMoveLineUpdate\x12\x45.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineUpdateRequest\x1a\x46.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineUpdateResponse\x12\xa4\x01\n\x13StockMoveLineDelete\x12\x45.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineDeleteRequest\x1a\x46.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineDeleteResponseb\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.stock.stock_move_line_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_STOCKMOVELINE"]._serialized_start = 157
-    _globals["_STOCKMOVELINE"]._serialized_end = 538
-    _globals["_STOCKMOVELINECREATEREQUEST"]._serialized_start = 541
-    _globals["_STOCKMOVELINECREATEREQUEST"]._serialized_end = 870
-    _globals["_STOCKMOVELINECREATERESPONSE"]._serialized_start = 873
-    _globals["_STOCKMOVELINECREATERESPONSE"]._serialized_end = 1055
-    _globals["_STOCKMOVELINEREADREQUEST"]._serialized_start = 1058
-    _globals["_STOCKMOVELINEREADREQUEST"]._serialized_end = 1432
-    _globals["_STOCKMOVELINEREADRESPONSE"]._serialized_start = 1435
-    _globals["_STOCKMOVELINEREADRESPONSE"]._serialized_end = 1675
-    _globals["_STOCKMOVELINEUPDATEREQUEST"]._serialized_start = 1678
-    _globals["_STOCKMOVELINEUPDATEREQUEST"]._serialized_end = 1840
-    _globals["_STOCKMOVELINEUPDATERESPONSE"]._serialized_start = 1843
-    _globals["_STOCKMOVELINEUPDATERESPONSE"]._serialized_end = 2025
-    _globals["_STOCKMOVELINEDELETEREQUEST"]._serialized_start = 2027
-    _globals["_STOCKMOVELINEDELETEREQUEST"]._serialized_end = 2123
-    _globals["_STOCKMOVELINEDELETERESPONSE"]._serialized_start = 2125
-    _globals["_STOCKMOVELINEDELETERESPONSE"]._serialized_end = 2229
-    _globals["_STOCKMOVELINESERVICE"]._serialized_start = 2232
-    _globals["_STOCKMOVELINESERVICE"]._serialized_end = 2876
+    _globals["_STOCKMOVELINE"]._serialized_start = 162
+    _globals["_STOCKMOVELINE"]._serialized_end = 543
+    _globals["_STOCKMOVELINECREATEREQUEST"]._serialized_start = 546
+    _globals["_STOCKMOVELINECREATEREQUEST"]._serialized_end = 875
+    _globals["_STOCKMOVELINECREATERESPONSE"]._serialized_start = 878
+    _globals["_STOCKMOVELINECREATERESPONSE"]._serialized_end = 1065
+    _globals["_STOCKMOVELINEREADREQUEST"]._serialized_start = 1068
+    _globals["_STOCKMOVELINEREADREQUEST"]._serialized_end = 1442
+    _globals["_STOCKMOVELINEREADRESPONSE"]._serialized_start = 1445
+    _globals["_STOCKMOVELINEREADRESPONSE"]._serialized_end = 1690
+    _globals["_STOCKMOVELINEUPDATEREQUEST"]._serialized_start = 1693
+    _globals["_STOCKMOVELINEUPDATEREQUEST"]._serialized_end = 1860
+    _globals["_STOCKMOVELINEUPDATERESPONSE"]._serialized_start = 1863
+    _globals["_STOCKMOVELINEUPDATERESPONSE"]._serialized_end = 2050
+    _globals["_STOCKMOVELINEDELETEREQUEST"]._serialized_start = 2052
+    _globals["_STOCKMOVELINEDELETEREQUEST"]._serialized_end = 2148
+    _globals["_STOCKMOVELINEDELETERESPONSE"]._serialized_start = 2150
+    _globals["_STOCKMOVELINEDELETERESPONSE"]._serialized_end = 2254
+    _globals["_STOCKMOVELINESERVICE"]._serialized_start = 2257
+    _globals["_STOCKMOVELINESERVICE"]._serialized_end = 2941
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/stock_move_line_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/stock_move_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/stock_move_line_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/stock_move_line_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,30 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.StockMoveLineCreate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.stock.stock.line.StockMoveLineService/StockMoveLineCreate",
+            "/pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineService/StockMoveLineCreate",
             request_serializer=v1_dot_stock_dot_stock__move__line__pb2.StockMoveLineCreateRequest.SerializeToString,
             response_deserializer=v1_dot_stock_dot_stock__move__line__pb2.StockMoveLineCreateResponse.FromString,
         )
         self.StockMoveLineRead = channel.unary_unary(
-            "/pro.omni.oms.api.v1.stock.stock.line.StockMoveLineService/StockMoveLineRead",
+            "/pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineService/StockMoveLineRead",
             request_serializer=v1_dot_stock_dot_stock__move__line__pb2.StockMoveLineReadRequest.SerializeToString,
             response_deserializer=v1_dot_stock_dot_stock__move__line__pb2.StockMoveLineReadResponse.FromString,
         )
         self.StockMoveLineUpdate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.stock.stock.line.StockMoveLineService/StockMoveLineUpdate",
+            "/pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineService/StockMoveLineUpdate",
             request_serializer=v1_dot_stock_dot_stock__move__line__pb2.StockMoveLineUpdateRequest.SerializeToString,
             response_deserializer=v1_dot_stock_dot_stock__move__line__pb2.StockMoveLineUpdateResponse.FromString,
         )
         self.StockMoveLineDelete = channel.unary_unary(
-            "/pro.omni.oms.api.v1.stock.stock.line.StockMoveLineService/StockMoveLineDelete",
+            "/pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineService/StockMoveLineDelete",
             request_serializer=v1_dot_stock_dot_stock__move__line__pb2.StockMoveLineDeleteRequest.SerializeToString,
             response_deserializer=v1_dot_stock_dot_stock__move__line__pb2.StockMoveLineDeleteResponse.FromString,
         )
 
 
 class StockMoveLineServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
@@ -83,15 +83,15 @@
         "StockMoveLineDelete": grpc.unary_unary_rpc_method_handler(
             servicer.StockMoveLineDelete,
             request_deserializer=v1_dot_stock_dot_stock__move__line__pb2.StockMoveLineDeleteRequest.FromString,
             response_serializer=v1_dot_stock_dot_stock__move__line__pb2.StockMoveLineDeleteResponse.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "pro.omni.oms.api.v1.stock.stock.line.StockMoveLineService", rpc_method_handlers
+        "pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineService", rpc_method_handlers
     )
     server.add_generic_rpc_handlers((generic_handler,))
 
 
 # This class is part of an EXPERIMENTAL API.
 class StockMoveLineService(object):
     """Missing associated documentation comment in .proto file."""
@@ -108,15 +108,15 @@
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.stock.stock.line.StockMoveLineService/StockMoveLineCreate",
+            "/pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineService/StockMoveLineCreate",
             v1_dot_stock_dot_stock__move__line__pb2.StockMoveLineCreateRequest.SerializeToString,
             v1_dot_stock_dot_stock__move__line__pb2.StockMoveLineCreateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
@@ -137,15 +137,15 @@
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.stock.stock.line.StockMoveLineService/StockMoveLineRead",
+            "/pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineService/StockMoveLineRead",
             v1_dot_stock_dot_stock__move__line__pb2.StockMoveLineReadRequest.SerializeToString,
             v1_dot_stock_dot_stock__move__line__pb2.StockMoveLineReadResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
@@ -166,15 +166,15 @@
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.stock.stock.line.StockMoveLineService/StockMoveLineUpdate",
+            "/pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineService/StockMoveLineUpdate",
             v1_dot_stock_dot_stock__move__line__pb2.StockMoveLineUpdateRequest.SerializeToString,
             v1_dot_stock_dot_stock__move__line__pb2.StockMoveLineUpdateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
@@ -195,15 +195,15 @@
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.stock.stock.line.StockMoveLineService/StockMoveLineDelete",
+            "/pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineService/StockMoveLineDelete",
             v1_dot_stock_dot_stock__move__line__pb2.StockMoveLineDeleteRequest.SerializeToString,
             v1_dot_stock_dot_stock__move__line__pb2.StockMoveLineDeleteResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
```

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/stock_move_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/stock_move_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x19v1/stock/stock_move.proto\x12$pro.omni.oms.api.v1.stock.stock.move\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xa0\x02\n\tStockMove\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x12\n\npicking_id\x18\x02 \x01(\x05\x12\r\n\x05state\x18\x03 \x01(\t\x12\x12\n\nproduct_id\x18\x04 \x01(\x05\x12\x17\n\x0fproduct_uom_qty\x18\x05 \x01(\x02\x12\x15\n\rquantity_done\x18\x06 \x01(\x02\x12\x16\n\x0eproduct_uom_id\x18\x07 \x01(\x05\x12\x1b\n\x13\x64\x65scription_picking\x18\x08 \x01(\t\x12*\n\x06\x61\x63tive\x18\t \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\n \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xec\x01\n\x16StockMoveCreateRequest\x12\x12\n\npicking_id\x18\x01 \x01(\x05\x12\r\n\x05state\x18\x02 \x01(\t\x12\x12\n\nproduct_id\x18\x03 \x01(\x05\x12\x17\n\x0fproduct_uom_qty\x18\x04 \x01(\x02\x12\x15\n\rquantity_done\x18\x05 \x01(\x02\x12\x16\n\x0eproduct_uom_id\x18\x06 \x01(\x05\x12\x1b\n\x13\x64\x65scription_picking\x18\x07 \x01(\t\x12\x36\n\x07\x63ontext\x18\x08 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa9\x01\n\x17StockMoveCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x43\n\nstock_move\x18\x02 \x01(\x0b\x32/.pro.omni.oms.api.v1.stock.stock.move.StockMove"\xf2\x02\n\x14StockMoveReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xe3\x01\n\x15StockMoveReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x44\n\x0bstock_moves\x18\x03 \x03(\x0b\x32/.pro.omni.oms.api.v1.stock.stock.move.StockMove"\x95\x01\n\x16StockMoveUpdateRequest\x12\x43\n\nstock_move\x18\x01 \x01(\x0b\x32/.pro.omni.oms.api.v1.stock.stock.move.StockMove\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa9\x01\n\x17StockMoveUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x43\n\nstock_move\x18\x02 \x01(\x0b\x32/.pro.omni.oms.api.v1.stock.stock.move.StockMove"\\\n\x16StockMoveDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"d\n\x17StockMoveDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xd8\x04\n\x10StockMoveService\x12\x90\x01\n\x0fStockMoveCreate\x12<.pro.omni.oms.api.v1.stock.stock.move.StockMoveCreateRequest\x1a=.pro.omni.oms.api.v1.stock.stock.move.StockMoveCreateResponse"\x00\x12\x8a\x01\n\rStockMoveRead\x12:.pro.omni.oms.api.v1.stock.stock.move.StockMoveReadRequest\x1a;.pro.omni.oms.api.v1.stock.stock.move.StockMoveReadResponse"\x00\x12\x90\x01\n\x0fStockMoveUpdate\x12<.pro.omni.oms.api.v1.stock.stock.move.StockMoveUpdateRequest\x1a=.pro.omni.oms.api.v1.stock.stock.move.StockMoveUpdateResponse"\x00\x12\x90\x01\n\x0fStockMoveDelete\x12<.pro.omni.oms.api.v1.stock.stock.move.StockMoveDeleteRequest\x1a=.pro.omni.oms.api.v1.stock.stock.move.StockMoveDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x19v1/stock/stock_move.proto\x12$pro.omni.oms.api.v1.stock.stock_move\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xa0\x02\n\tStockMove\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x12\n\npicking_id\x18\x02 \x01(\x05\x12\r\n\x05state\x18\x03 \x01(\t\x12\x12\n\nproduct_id\x18\x04 \x01(\x05\x12\x17\n\x0fproduct_uom_qty\x18\x05 \x01(\x02\x12\x15\n\rquantity_done\x18\x06 \x01(\x02\x12\x16\n\x0eproduct_uom_id\x18\x07 \x01(\x05\x12\x1b\n\x13\x64\x65scription_picking\x18\x08 \x01(\t\x12*\n\x06\x61\x63tive\x18\t \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\n \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xec\x01\n\x16StockMoveCreateRequest\x12\x12\n\npicking_id\x18\x01 \x01(\x05\x12\r\n\x05state\x18\x02 \x01(\t\x12\x12\n\nproduct_id\x18\x03 \x01(\x05\x12\x17\n\x0fproduct_uom_qty\x18\x04 \x01(\x02\x12\x15\n\rquantity_done\x18\x05 \x01(\x02\x12\x16\n\x0eproduct_uom_id\x18\x06 \x01(\x05\x12\x1b\n\x13\x64\x65scription_picking\x18\x07 \x01(\t\x12\x36\n\x07\x63ontext\x18\x08 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa9\x01\n\x17StockMoveCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x43\n\nstock_move\x18\x02 \x01(\x0b\x32/.pro.omni.oms.api.v1.stock.stock_move.StockMove"\xf2\x02\n\x14StockMoveReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xe3\x01\n\x15StockMoveReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x44\n\x0bstock_moves\x18\x03 \x03(\x0b\x32/.pro.omni.oms.api.v1.stock.stock_move.StockMove"\x95\x01\n\x16StockMoveUpdateRequest\x12\x43\n\nstock_move\x18\x01 \x01(\x0b\x32/.pro.omni.oms.api.v1.stock.stock_move.StockMove\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa9\x01\n\x17StockMoveUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x43\n\nstock_move\x18\x02 \x01(\x0b\x32/.pro.omni.oms.api.v1.stock.stock_move.StockMove"\\\n\x16StockMoveDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"d\n\x17StockMoveDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xd8\x04\n\x10StockMoveService\x12\x90\x01\n\x0fStockMoveCreate\x12<.pro.omni.oms.api.v1.stock.stock_move.StockMoveCreateRequest\x1a=.pro.omni.oms.api.v1.stock.stock_move.StockMoveCreateResponse"\x00\x12\x8a\x01\n\rStockMoveRead\x12:.pro.omni.oms.api.v1.stock.stock_move.StockMoveReadRequest\x1a;.pro.omni.oms.api.v1.stock.stock_move.StockMoveReadResponse"\x00\x12\x90\x01\n\x0fStockMoveUpdate\x12<.pro.omni.oms.api.v1.stock.stock_move.StockMoveUpdateRequest\x1a=.pro.omni.oms.api.v1.stock.stock_move.StockMoveUpdateResponse"\x00\x12\x90\x01\n\x0fStockMoveDelete\x12<.pro.omni.oms.api.v1.stock.stock_move.StockMoveDeleteRequest\x1a=.pro.omni.oms.api.v1.stock.stock_move.StockMoveDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.stock.stock_move_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
```

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/stock_move_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/stock_move_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/stock_move_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/stock_move_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,30 +10,30 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.StockMoveCreate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.stock.stock.move.StockMoveService/StockMoveCreate",
+            "/pro.omni.oms.api.v1.stock.stock_move.StockMoveService/StockMoveCreate",
             request_serializer=v1_dot_stock_dot_stock__move__pb2.StockMoveCreateRequest.SerializeToString,
             response_deserializer=v1_dot_stock_dot_stock__move__pb2.StockMoveCreateResponse.FromString,
         )
         self.StockMoveRead = channel.unary_unary(
-            "/pro.omni.oms.api.v1.stock.stock.move.StockMoveService/StockMoveRead",
+            "/pro.omni.oms.api.v1.stock.stock_move.StockMoveService/StockMoveRead",
             request_serializer=v1_dot_stock_dot_stock__move__pb2.StockMoveReadRequest.SerializeToString,
             response_deserializer=v1_dot_stock_dot_stock__move__pb2.StockMoveReadResponse.FromString,
         )
         self.StockMoveUpdate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.stock.stock.move.StockMoveService/StockMoveUpdate",
+            "/pro.omni.oms.api.v1.stock.stock_move.StockMoveService/StockMoveUpdate",
             request_serializer=v1_dot_stock_dot_stock__move__pb2.StockMoveUpdateRequest.SerializeToString,
             response_deserializer=v1_dot_stock_dot_stock__move__pb2.StockMoveUpdateResponse.FromString,
         )
         self.StockMoveDelete = channel.unary_unary(
-            "/pro.omni.oms.api.v1.stock.stock.move.StockMoveService/StockMoveDelete",
+            "/pro.omni.oms.api.v1.stock.stock_move.StockMoveService/StockMoveDelete",
             request_serializer=v1_dot_stock_dot_stock__move__pb2.StockMoveDeleteRequest.SerializeToString,
             response_deserializer=v1_dot_stock_dot_stock__move__pb2.StockMoveDeleteResponse.FromString,
         )
 
 
 class StockMoveServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
@@ -83,15 +83,15 @@
         "StockMoveDelete": grpc.unary_unary_rpc_method_handler(
             servicer.StockMoveDelete,
             request_deserializer=v1_dot_stock_dot_stock__move__pb2.StockMoveDeleteRequest.FromString,
             response_serializer=v1_dot_stock_dot_stock__move__pb2.StockMoveDeleteResponse.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "pro.omni.oms.api.v1.stock.stock.move.StockMoveService", rpc_method_handlers
+        "pro.omni.oms.api.v1.stock.stock_move.StockMoveService", rpc_method_handlers
     )
     server.add_generic_rpc_handlers((generic_handler,))
 
 
 # This class is part of an EXPERIMENTAL API.
 class StockMoveService(object):
     """Missing associated documentation comment in .proto file."""
@@ -108,15 +108,15 @@
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.stock.stock.move.StockMoveService/StockMoveCreate",
+            "/pro.omni.oms.api.v1.stock.stock_move.StockMoveService/StockMoveCreate",
             v1_dot_stock_dot_stock__move__pb2.StockMoveCreateRequest.SerializeToString,
             v1_dot_stock_dot_stock__move__pb2.StockMoveCreateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
@@ -137,15 +137,15 @@
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.stock.stock.move.StockMoveService/StockMoveRead",
+            "/pro.omni.oms.api.v1.stock.stock_move.StockMoveService/StockMoveRead",
             v1_dot_stock_dot_stock__move__pb2.StockMoveReadRequest.SerializeToString,
             v1_dot_stock_dot_stock__move__pb2.StockMoveReadResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
@@ -166,15 +166,15 @@
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.stock.stock.move.StockMoveService/StockMoveUpdate",
+            "/pro.omni.oms.api.v1.stock.stock_move.StockMoveService/StockMoveUpdate",
             v1_dot_stock_dot_stock__move__pb2.StockMoveUpdateRequest.SerializeToString,
             v1_dot_stock_dot_stock__move__pb2.StockMoveUpdateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
@@ -195,15 +195,15 @@
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.stock.stock.move.StockMoveService/StockMoveDelete",
+            "/pro.omni.oms.api.v1.stock.stock_move.StockMoveService/StockMoveDelete",
             v1_dot_stock_dot_stock__move__pb2.StockMoveDeleteRequest.SerializeToString,
             v1_dot_stock_dot_stock__move__pb2.StockMoveDeleteResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
```

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/uom_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/uom_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/uom_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/uom_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/uom_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/uom_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/user_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/user_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/user_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/user_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/warehouse_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/country_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/stock/warehouse.proto
+# source: v1/utilities/country.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
@@ -13,36 +13,36 @@
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x18v1/stock/warehouse.proto\x12#pro.omni.oms.api.v1.stock.warehouse\x1a\x11\x63ommon/base.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1egoogle/protobuf/wrappers.proto"\x92\x02\n\tWarehouse\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x12\n\ncountry_id\x18\x04 \x01(\x05\x12\x37\n\x16territory_matrix_value\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07\x61\x64\x64ress\x18\x06 \x01(\t\x12\x12\n\ncomplement\x18\x07 \x01(\t\x12*\n\x06\x61\x63tive\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\t \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xde\x01\n\x16WarehouseCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x12\n\ncountry_id\x18\x03 \x01(\x05\x12\x37\n\x16territory_matrix_value\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07\x61\x64\x64ress\x18\x05 \x01(\t\x12\x12\n\ncomplement\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa7\x01\n\x17WarehouseCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x41\n\twarehouse\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.v1.stock.warehouse.Warehouse"\xf2\x02\n\x14WarehouseReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xe1\x01\n\x15WarehouseReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x42\n\nwarehouses\x18\x03 \x03(\x0b\x32..pro.omni.oms.api.v1.stock.warehouse.Warehouse"\x93\x01\n\x16WarehouseUpdateRequest\x12\x41\n\twarehouse\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.v1.stock.warehouse.Warehouse\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa7\x01\n\x17WarehouseUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x41\n\twarehouse\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.v1.stock.warehouse.Warehouse"\\\n\x16WarehouseDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"d\n\x17WarehouseDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xd0\x04\n\x10WarehouseService\x12\x8e\x01\n\x0fWarehouseCreate\x12;.pro.omni.oms.api.v1.stock.warehouse.WarehouseCreateRequest\x1a<.pro.omni.oms.api.v1.stock.warehouse.WarehouseCreateResponse"\x00\x12\x88\x01\n\rWarehouseRead\x12\x39.pro.omni.oms.api.v1.stock.warehouse.WarehouseReadRequest\x1a:.pro.omni.oms.api.v1.stock.warehouse.WarehouseReadResponse"\x00\x12\x8e\x01\n\x0fWarehouseUpdate\x12;.pro.omni.oms.api.v1.stock.warehouse.WarehouseUpdateRequest\x1a<.pro.omni.oms.api.v1.stock.warehouse.WarehouseUpdateResponse"\x00\x12\x8e\x01\n\x0fWarehouseDelete\x12;.pro.omni.oms.api.v1.stock.warehouse.WarehouseDeleteRequest\x1a<.pro.omni.oms.api.v1.stock.warehouse.WarehouseDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x1av1/utilities/country.proto\x12%pro.omni.oms.api.v1.utilities.country\x1a\x11\x63ommon/base.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xbd\x04\n\x07\x43ountry\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x19\n\x11phone_number_size\x18\x04 \x01(\x05\x12\x14\n\x0cphone_prefix\x18\x05 \x01(\t\x12\x33\n\x0frequire_zipcode\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12.\n\ncurrencies\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x32\n\x0e\x64ocument_types\x18\t \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x36\n\x12territory_matrixes\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12*\n\tmeta_data\x18\x0c \x01(\x0b\x32\x17.google.protobuf.Struct\x12-\n\ttimezones\x18\r \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12-\n\tlanguages\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x11\n\tlow_level\x18\x0f \x01(\t\x12*\n\x06\x61\x63tive\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x11 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x9d\x04\n\x14\x43ountryCreateRequest\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x19\n\x11phone_number_size\x18\x03 \x01(\x05\x12\x14\n\x0cphone_prefix\x18\x04 \x01(\t\x12\x33\n\x0frequire_zipcode\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x32\n\x0e\x63urrencies_ids\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x36\n\x12\x64ocument_types_ids\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12:\n\x16territory_matrixes_ids\x18\n \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12*\n\tmeta_data\x18\x0b \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x31\n\rtimezones_ids\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x31\n\rlanguages_ids\x18\r \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x11\n\tlow_level\x18\x0e \x01(\t\x12\x36\n\x07\x63ontext\x18\x0f \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x15\x43ountryCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12?\n\x07\x63ountry\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.v1.utilities.country.Country"\xf0\x02\n\x12\x43ountryReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xde\x01\n\x13\x43ountryReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x41\n\tcountries\x18\x03 \x03(\x0b\x32..pro.omni.oms.api.v1.utilities.country.Country"\x8f\x01\n\x14\x43ountryUpdateRequest\x12?\n\x07\x63ountry\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.v1.utilities.country.Country\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x15\x43ountryUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12?\n\x07\x63ountry\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.v1.utilities.country.Country"Z\n\x14\x43ountryDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"b\n\x15\x43ountryDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xc6\x04\n\x0e\x43ountryService\x12\x8c\x01\n\rCountryCreate\x12;.pro.omni.oms.api.v1.utilities.country.CountryCreateRequest\x1a<.pro.omni.oms.api.v1.utilities.country.CountryCreateResponse"\x00\x12\x86\x01\n\x0b\x43ountryRead\x12\x39.pro.omni.oms.api.v1.utilities.country.CountryReadRequest\x1a:.pro.omni.oms.api.v1.utilities.country.CountryReadResponse"\x00\x12\x8c\x01\n\rCountryUpdate\x12;.pro.omni.oms.api.v1.utilities.country.CountryUpdateRequest\x1a<.pro.omni.oms.api.v1.utilities.country.CountryUpdateResponse"\x00\x12\x8c\x01\n\rCountryDelete\x12;.pro.omni.oms.api.v1.utilities.country.CountryDeleteRequest\x1a<.pro.omni.oms.api.v1.utilities.country.CountryDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.stock.warehouse_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.utilities.country_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_WAREHOUSE"]._serialized_start = 147
-    _globals["_WAREHOUSE"]._serialized_end = 421
-    _globals["_WAREHOUSECREATEREQUEST"]._serialized_start = 424
-    _globals["_WAREHOUSECREATEREQUEST"]._serialized_end = 646
-    _globals["_WAREHOUSECREATERESPONSE"]._serialized_start = 649
-    _globals["_WAREHOUSECREATERESPONSE"]._serialized_end = 816
-    _globals["_WAREHOUSEREADREQUEST"]._serialized_start = 819
-    _globals["_WAREHOUSEREADREQUEST"]._serialized_end = 1189
-    _globals["_WAREHOUSEREADRESPONSE"]._serialized_start = 1192
-    _globals["_WAREHOUSEREADRESPONSE"]._serialized_end = 1417
-    _globals["_WAREHOUSEUPDATEREQUEST"]._serialized_start = 1420
-    _globals["_WAREHOUSEUPDATEREQUEST"]._serialized_end = 1567
-    _globals["_WAREHOUSEUPDATERESPONSE"]._serialized_start = 1570
-    _globals["_WAREHOUSEUPDATERESPONSE"]._serialized_end = 1737
-    _globals["_WAREHOUSEDELETEREQUEST"]._serialized_start = 1739
-    _globals["_WAREHOUSEDELETEREQUEST"]._serialized_end = 1831
-    _globals["_WAREHOUSEDELETERESPONSE"]._serialized_start = 1833
-    _globals["_WAREHOUSEDELETERESPONSE"]._serialized_end = 1933
-    _globals["_WAREHOUSESERVICE"]._serialized_start = 1936
-    _globals["_WAREHOUSESERVICE"]._serialized_end = 2528
+    _globals["_COUNTRY"]._serialized_start = 151
+    _globals["_COUNTRY"]._serialized_end = 724
+    _globals["_COUNTRYCREATEREQUEST"]._serialized_start = 727
+    _globals["_COUNTRYCREATEREQUEST"]._serialized_end = 1268
+    _globals["_COUNTRYCREATERESPONSE"]._serialized_start = 1271
+    _globals["_COUNTRYCREATERESPONSE"]._serialized_end = 1434
+    _globals["_COUNTRYREADREQUEST"]._serialized_start = 1437
+    _globals["_COUNTRYREADREQUEST"]._serialized_end = 1805
+    _globals["_COUNTRYREADRESPONSE"]._serialized_start = 1808
+    _globals["_COUNTRYREADRESPONSE"]._serialized_end = 2030
+    _globals["_COUNTRYUPDATEREQUEST"]._serialized_start = 2033
+    _globals["_COUNTRYUPDATEREQUEST"]._serialized_end = 2176
+    _globals["_COUNTRYUPDATERESPONSE"]._serialized_start = 2179
+    _globals["_COUNTRYUPDATERESPONSE"]._serialized_end = 2342
+    _globals["_COUNTRYDELETEREQUEST"]._serialized_start = 2344
+    _globals["_COUNTRYDELETEREQUEST"]._serialized_end = 2434
+    _globals["_COUNTRYDELETERESPONSE"]._serialized_start = 2436
+    _globals["_COUNTRYDELETERESPONSE"]._serialized_end = 2534
+    _globals["_COUNTRYSERVICE"]._serialized_start = 2537
+    _globals["_COUNTRYSERVICE"]._serialized_end = 3119
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/warehouse_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/sequence_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -2,104 +2,127 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from google.protobuf import struct_pb2 as _struct_pb2
 from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Warehouse(_message.Message):
+class Sequence(_message.Message):
     __slots__ = [
         "id",
         "name",
         "code",
-        "country_id",
-        "territory_matrix_value",
-        "address",
-        "complement",
+        "implementation",
+        "prefix",
+        "suffix",
+        "padding",
+        "number_increment",
+        "number_next_actual",
         "active",
         "object_audit",
     ]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    COUNTRY_ID_FIELD_NUMBER: _ClassVar[int]
-    TERRITORY_MATRIX_VALUE_FIELD_NUMBER: _ClassVar[int]
-    ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    COMPLEMENT_FIELD_NUMBER: _ClassVar[int]
+    IMPLEMENTATION_FIELD_NUMBER: _ClassVar[int]
+    PREFIX_FIELD_NUMBER: _ClassVar[int]
+    SUFFIX_FIELD_NUMBER: _ClassVar[int]
+    PADDING_FIELD_NUMBER: _ClassVar[int]
+    NUMBER_INCREMENT_FIELD_NUMBER: _ClassVar[int]
+    NUMBER_NEXT_ACTUAL_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
-    id: int
+    id: str
     name: str
     code: str
-    country_id: int
-    territory_matrix_value: _struct_pb2.Struct
-    address: str
-    complement: str
+    implementation: str
+    prefix: str
+    suffix: str
+    padding: float
+    number_increment: int
+    number_next_actual: int
     active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
-        id: _Optional[int] = ...,
+        id: _Optional[str] = ...,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        country_id: _Optional[int] = ...,
-        territory_matrix_value: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ...,
-        address: _Optional[str] = ...,
-        complement: _Optional[str] = ...,
+        implementation: _Optional[str] = ...,
+        prefix: _Optional[str] = ...,
+        suffix: _Optional[str] = ...,
+        padding: _Optional[float] = ...,
+        number_increment: _Optional[int] = ...,
+        number_next_actual: _Optional[int] = ...,
         active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseCreateRequest(_message.Message):
-    __slots__ = ["name", "code", "country_id", "territory_matrix_value", "address", "complement", "context"]
+class SequenceCreateRequest(_message.Message):
+    __slots__ = [
+        "name",
+        "code",
+        "implementation",
+        "prefix",
+        "suffix",
+        "padding",
+        "number_increment",
+        "number_next_actual",
+        "context",
+    ]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    COUNTRY_ID_FIELD_NUMBER: _ClassVar[int]
-    TERRITORY_MATRIX_VALUE_FIELD_NUMBER: _ClassVar[int]
-    ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    COMPLEMENT_FIELD_NUMBER: _ClassVar[int]
+    IMPLEMENTATION_FIELD_NUMBER: _ClassVar[int]
+    PREFIX_FIELD_NUMBER: _ClassVar[int]
+    SUFFIX_FIELD_NUMBER: _ClassVar[int]
+    PADDING_FIELD_NUMBER: _ClassVar[int]
+    NUMBER_INCREMENT_FIELD_NUMBER: _ClassVar[int]
+    NUMBER_NEXT_ACTUAL_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     name: str
     code: str
-    country_id: int
-    territory_matrix_value: _struct_pb2.Struct
-    address: str
-    complement: str
+    implementation: str
+    prefix: str
+    suffix: str
+    padding: float
+    number_increment: int
+    number_next_actual: int
     context: _base_pb2.Context
     def __init__(
         self,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        country_id: _Optional[int] = ...,
-        territory_matrix_value: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ...,
-        address: _Optional[str] = ...,
-        complement: _Optional[str] = ...,
+        implementation: _Optional[str] = ...,
+        prefix: _Optional[str] = ...,
+        suffix: _Optional[str] = ...,
+        padding: _Optional[float] = ...,
+        number_increment: _Optional[int] = ...,
+        number_next_actual: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseCreateResponse(_message.Message):
-    __slots__ = ["response_standard", "warehouse"]
+class SequenceCreateResponse(_message.Message):
+    __slots__ = ["response_standard", "sequence"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
+    SEQUENCE_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    warehouse: Warehouse
+    sequence: Sequence
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        warehouse: _Optional[_Union[Warehouse, _Mapping]] = ...,
+        sequence: _Optional[_Union[Sequence, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseReadRequest(_message.Message):
+class SequenceReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
@@ -118,61 +141,61 @@
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
         id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseReadResponse(_message.Message):
-    __slots__ = ["response_standard", "meta_data", "warehouses"]
+class SequenceReadResponse(_message.Message):
+    __slots__ = ["response_standard", "meta_data", "sequences"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
-    WAREHOUSES_FIELD_NUMBER: _ClassVar[int]
+    SEQUENCES_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     meta_data: _base_pb2.MetaData
-    warehouses: _containers.RepeatedCompositeFieldContainer[Warehouse]
+    sequences: _containers.RepeatedCompositeFieldContainer[Sequence]
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
-        warehouses: _Optional[_Iterable[_Union[Warehouse, _Mapping]]] = ...,
+        sequences: _Optional[_Iterable[_Union[Sequence, _Mapping]]] = ...,
     ) -> None: ...
 
-class WarehouseUpdateRequest(_message.Message):
-    __slots__ = ["warehouse", "context"]
-    WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
+class SequenceUpdateRequest(_message.Message):
+    __slots__ = ["sequence", "context"]
+    SEQUENCE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    warehouse: Warehouse
+    sequence: Sequence
     context: _base_pb2.Context
     def __init__(
         self,
-        warehouse: _Optional[_Union[Warehouse, _Mapping]] = ...,
+        sequence: _Optional[_Union[Sequence, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseUpdateResponse(_message.Message):
-    __slots__ = ["response_standard", "warehouse"]
+class SequenceUpdateResponse(_message.Message):
+    __slots__ = ["response_standard", "sequence"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
+    SEQUENCE_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    warehouse: Warehouse
+    sequence: Sequence
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        warehouse: _Optional[_Union[Warehouse, _Mapping]] = ...,
+        sequence: _Optional[_Union[Sequence, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseDeleteRequest(_message.Message):
+class SequenceDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: int
     context: _base_pb2.Context
     def __init__(
         self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class WarehouseDeleteResponse(_message.Message):
+class SequenceDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/stock/warehouse_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/users/user_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/users/user_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/users/user_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/users/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/country_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/tax_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/utilities/country.proto
+# source: v1/utilities/tax.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1av1/utilities/country.proto\x12%pro.omni.oms.api.v1.utilities.country\x1a\x11\x63ommon/base.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xbd\x04\n\x07\x43ountry\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x19\n\x11phone_number_size\x18\x04 \x01(\x05\x12\x14\n\x0cphone_prefix\x18\x05 \x01(\t\x12\x33\n\x0frequire_zipcode\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12.\n\ncurrencies\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x32\n\x0e\x64ocument_types\x18\t \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x36\n\x12territory_matrixes\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12*\n\tmeta_data\x18\x0c \x01(\x0b\x32\x17.google.protobuf.Struct\x12-\n\ttimezones\x18\r \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12-\n\tlanguages\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x11\n\tlow_level\x18\x0f \x01(\t\x12*\n\x06\x61\x63tive\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x11 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x9d\x04\n\x14\x43ountryCreateRequest\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x19\n\x11phone_number_size\x18\x03 \x01(\x05\x12\x14\n\x0cphone_prefix\x18\x04 \x01(\t\x12\x33\n\x0frequire_zipcode\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x32\n\x0e\x63urrencies_ids\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x36\n\x12\x64ocument_types_ids\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12:\n\x16territory_matrixes_ids\x18\n \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12*\n\tmeta_data\x18\x0b \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x31\n\rtimezones_ids\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x31\n\rlanguages_ids\x18\r \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x11\n\tlow_level\x18\x0e \x01(\t\x12\x36\n\x07\x63ontext\x18\x0f \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x15\x43ountryCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12?\n\x07\x63ountry\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.v1.utilities.country.Country"\xf0\x02\n\x12\x43ountryReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xde\x01\n\x13\x43ountryReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x41\n\tcountries\x18\x03 \x03(\x0b\x32..pro.omni.oms.api.v1.utilities.country.Country"\x8f\x01\n\x14\x43ountryUpdateRequest\x12?\n\x07\x63ountry\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.v1.utilities.country.Country\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x15\x43ountryUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12?\n\x07\x63ountry\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.v1.utilities.country.Country"Z\n\x14\x43ountryDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"b\n\x15\x43ountryDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xc6\x04\n\x0e\x43ountryService\x12\x8c\x01\n\rCountryCreate\x12;.pro.omni.oms.api.v1.utilities.country.CountryCreateRequest\x1a<.pro.omni.oms.api.v1.utilities.country.CountryCreateResponse"\x00\x12\x86\x01\n\x0b\x43ountryRead\x12\x39.pro.omni.oms.api.v1.utilities.country.CountryReadRequest\x1a:.pro.omni.oms.api.v1.utilities.country.CountryReadResponse"\x00\x12\x8c\x01\n\rCountryUpdate\x12;.pro.omni.oms.api.v1.utilities.country.CountryUpdateRequest\x1a<.pro.omni.oms.api.v1.utilities.country.CountryUpdateResponse"\x00\x12\x8c\x01\n\rCountryDelete\x12;.pro.omni.oms.api.v1.utilities.country.CountryDeleteRequest\x1a<.pro.omni.oms.api.v1.utilities.country.CountryDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x16v1/utilities/tax.proto\x12!pro.omni.oms.api.v1.utilities.tax\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xe4\x01\n\x03Tax\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0c\n\x04rate\x18\x04 \x01(\x02\x12\x10\n\x08rounding\x18\x05 \x01(\x01\x12\x16\n\x0e\x64\x65\x63imal_places\x18\x06 \x01(\x05\x12\x10\n\x08position\x18\x07 \x01(\t\x12*\n\x06\x61\x63tive\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\t \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xad\x01\n\rTaxAddRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0c\n\x04rate\x18\x03 \x01(\x02\x12\x10\n\x08rounding\x18\x04 \x01(\x01\x12\x16\n\x0e\x64\x65\x63imal_places\x18\x05 \x01(\x05\x12\x10\n\x08position\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x90\x01\n\x0eTaxAddResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x33\n\x03tax\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.tax.Tax"\xec\x02\n\x0eTaxReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xce\x01\n\x0fTaxReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x35\n\x05taxes\x18\x03 \x03(\x0b\x32&.pro.omni.oms.api.v1.utilities.tax.Tax"\x7f\n\x10TaxUpdateRequest\x12\x33\n\x03tax\x18\x01 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.tax.Tax\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x93\x01\n\x11TaxUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x33\n\x03tax\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.tax.Tax"V\n\x10TaxDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"^\n\x11TaxDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xe5\x03\n\nTaxService\x12o\n\x06TaxAdd\x12\x30.pro.omni.oms.api.v1.utilities.tax.TaxAddRequest\x1a\x31.pro.omni.oms.api.v1.utilities.tax.TaxAddResponse"\x00\x12r\n\x07TaxRead\x12\x31.pro.omni.oms.api.v1.utilities.tax.TaxReadRequest\x1a\x32.pro.omni.oms.api.v1.utilities.tax.TaxReadResponse"\x00\x12x\n\tTaxUpdate\x12\x33.pro.omni.oms.api.v1.utilities.tax.TaxUpdateRequest\x1a\x34.pro.omni.oms.api.v1.utilities.tax.TaxUpdateResponse"\x00\x12x\n\tTaxDelete\x12\x33.pro.omni.oms.api.v1.utilities.tax.TaxDeleteRequest\x1a\x34.pro.omni.oms.api.v1.utilities.tax.TaxDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.utilities.country_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.utilities.tax_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_COUNTRY"]._serialized_start = 151
-    _globals["_COUNTRY"]._serialized_end = 724
-    _globals["_COUNTRYCREATEREQUEST"]._serialized_start = 727
-    _globals["_COUNTRYCREATEREQUEST"]._serialized_end = 1268
-    _globals["_COUNTRYCREATERESPONSE"]._serialized_start = 1271
-    _globals["_COUNTRYCREATERESPONSE"]._serialized_end = 1434
-    _globals["_COUNTRYREADREQUEST"]._serialized_start = 1437
-    _globals["_COUNTRYREADREQUEST"]._serialized_end = 1805
-    _globals["_COUNTRYREADRESPONSE"]._serialized_start = 1808
-    _globals["_COUNTRYREADRESPONSE"]._serialized_end = 2030
-    _globals["_COUNTRYUPDATEREQUEST"]._serialized_start = 2033
-    _globals["_COUNTRYUPDATEREQUEST"]._serialized_end = 2176
-    _globals["_COUNTRYUPDATERESPONSE"]._serialized_start = 2179
-    _globals["_COUNTRYUPDATERESPONSE"]._serialized_end = 2342
-    _globals["_COUNTRYDELETEREQUEST"]._serialized_start = 2344
-    _globals["_COUNTRYDELETEREQUEST"]._serialized_end = 2434
-    _globals["_COUNTRYDELETERESPONSE"]._serialized_start = 2436
-    _globals["_COUNTRYDELETERESPONSE"]._serialized_end = 2534
-    _globals["_COUNTRYSERVICE"]._serialized_start = 2537
-    _globals["_COUNTRYSERVICE"]._serialized_end = 3119
+    _globals["_TAX"]._serialized_start = 113
+    _globals["_TAX"]._serialized_end = 341
+    _globals["_TAXADDREQUEST"]._serialized_start = 344
+    _globals["_TAXADDREQUEST"]._serialized_end = 517
+    _globals["_TAXADDRESPONSE"]._serialized_start = 520
+    _globals["_TAXADDRESPONSE"]._serialized_end = 664
+    _globals["_TAXREADREQUEST"]._serialized_start = 667
+    _globals["_TAXREADREQUEST"]._serialized_end = 1031
+    _globals["_TAXREADRESPONSE"]._serialized_start = 1034
+    _globals["_TAXREADRESPONSE"]._serialized_end = 1240
+    _globals["_TAXUPDATEREQUEST"]._serialized_start = 1242
+    _globals["_TAXUPDATEREQUEST"]._serialized_end = 1369
+    _globals["_TAXUPDATERESPONSE"]._serialized_start = 1372
+    _globals["_TAXUPDATERESPONSE"]._serialized_end = 1519
+    _globals["_TAXDELETEREQUEST"]._serialized_start = 1521
+    _globals["_TAXDELETEREQUEST"]._serialized_end = 1607
+    _globals["_TAXDELETERESPONSE"]._serialized_start = 1609
+    _globals["_TAXDELETERESPONSE"]._serialized_end = 1703
+    _globals["_TAXSERVICE"]._serialized_start = 1706
+    _globals["_TAXSERVICE"]._serialized_end = 2191
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/country_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/country_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/country_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/country_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/currency_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/currency_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/currency_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/currency_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/currency_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/currency_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/document_type_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/document_type_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/document_type_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/document_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/document_type_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/document_type_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/language_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/language_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/language_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/language_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/language_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/language_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/model_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/model_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/model_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/model_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/model_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/payment_method_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/payment_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/payment_method_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/payment_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/payment_method_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/payment_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/tax_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/uom_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/utilities/tax.proto
+# source: v1/utilities/uom.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
@@ -12,36 +12,36 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x16v1/utilities/tax.proto\x12!pro.omni.oms.api.v1.utilities.tax\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xe4\x01\n\x03Tax\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0c\n\x04rate\x18\x04 \x01(\x02\x12\x10\n\x08rounding\x18\x05 \x01(\x01\x12\x16\n\x0e\x64\x65\x63imal_places\x18\x06 \x01(\x05\x12\x10\n\x08position\x18\x07 \x01(\t\x12*\n\x06\x61\x63tive\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\t \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xad\x01\n\rTaxAddRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0c\n\x04rate\x18\x03 \x01(\x02\x12\x10\n\x08rounding\x18\x04 \x01(\x01\x12\x16\n\x0e\x64\x65\x63imal_places\x18\x05 \x01(\x05\x12\x10\n\x08position\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x90\x01\n\x0eTaxAddResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x33\n\x03tax\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.tax.Tax"\xec\x02\n\x0eTaxReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xce\x01\n\x0fTaxReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x35\n\x05taxes\x18\x03 \x03(\x0b\x32&.pro.omni.oms.api.v1.utilities.tax.Tax"\x7f\n\x10TaxUpdateRequest\x12\x33\n\x03tax\x18\x01 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.tax.Tax\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x93\x01\n\x11TaxUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x33\n\x03tax\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.tax.Tax"V\n\x10TaxDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"^\n\x11TaxDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xe5\x03\n\nTaxService\x12o\n\x06TaxAdd\x12\x30.pro.omni.oms.api.v1.utilities.tax.TaxAddRequest\x1a\x31.pro.omni.oms.api.v1.utilities.tax.TaxAddResponse"\x00\x12r\n\x07TaxRead\x12\x31.pro.omni.oms.api.v1.utilities.tax.TaxReadRequest\x1a\x32.pro.omni.oms.api.v1.utilities.tax.TaxReadResponse"\x00\x12x\n\tTaxUpdate\x12\x33.pro.omni.oms.api.v1.utilities.tax.TaxUpdateRequest\x1a\x34.pro.omni.oms.api.v1.utilities.tax.TaxUpdateResponse"\x00\x12x\n\tTaxDelete\x12\x33.pro.omni.oms.api.v1.utilities.tax.TaxDeleteRequest\x1a\x34.pro.omni.oms.api.v1.utilities.tax.TaxDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x16v1/utilities/uom.proto\x12!pro.omni.oms.api.v1.utilities.uom\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xcc\x01\n\x03Uom\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08\x63\x61tegory\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\x10\n\x08rounding\x18\x06 \x01(\x01\x12*\n\x06\x61\x63tive\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x08 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x98\x01\n\x10UomCreateRequest\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\t\x12\x10\n\x08rounding\x18\x05 \x01(\x01\x12\x36\n\x07\x63ontext\x18\x06 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x93\x01\n\x11UomCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x33\n\x03uom\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.uom.Uom"\xec\x02\n\x0eUomReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xcd\x01\n\x0fUomReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x34\n\x04uoms\x18\x03 \x03(\x0b\x32&.pro.omni.oms.api.v1.utilities.uom.Uom"\x7f\n\x10UomUpdateRequest\x12\x33\n\x03uom\x18\x01 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.uom.Uom\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x93\x01\n\x11UomUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x33\n\x03uom\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.uom.Uom"V\n\x10UomDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"^\n\x11UomDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xee\x03\n\nUomService\x12x\n\tUomCreate\x12\x33.pro.omni.oms.api.v1.utilities.uom.UomCreateRequest\x1a\x34.pro.omni.oms.api.v1.utilities.uom.UomCreateResponse"\x00\x12r\n\x07UomRead\x12\x31.pro.omni.oms.api.v1.utilities.uom.UomReadRequest\x1a\x32.pro.omni.oms.api.v1.utilities.uom.UomReadResponse"\x00\x12x\n\tUomUpdate\x12\x33.pro.omni.oms.api.v1.utilities.uom.UomUpdateRequest\x1a\x34.pro.omni.oms.api.v1.utilities.uom.UomUpdateResponse"\x00\x12x\n\tUomDelete\x12\x33.pro.omni.oms.api.v1.utilities.uom.UomDeleteRequest\x1a\x34.pro.omni.oms.api.v1.utilities.uom.UomDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.utilities.tax_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.utilities.uom_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_TAX"]._serialized_start = 113
-    _globals["_TAX"]._serialized_end = 341
-    _globals["_TAXADDREQUEST"]._serialized_start = 344
-    _globals["_TAXADDREQUEST"]._serialized_end = 517
-    _globals["_TAXADDRESPONSE"]._serialized_start = 520
-    _globals["_TAXADDRESPONSE"]._serialized_end = 664
-    _globals["_TAXREADREQUEST"]._serialized_start = 667
-    _globals["_TAXREADREQUEST"]._serialized_end = 1031
-    _globals["_TAXREADRESPONSE"]._serialized_start = 1034
-    _globals["_TAXREADRESPONSE"]._serialized_end = 1240
-    _globals["_TAXUPDATEREQUEST"]._serialized_start = 1242
-    _globals["_TAXUPDATEREQUEST"]._serialized_end = 1369
-    _globals["_TAXUPDATERESPONSE"]._serialized_start = 1372
-    _globals["_TAXUPDATERESPONSE"]._serialized_end = 1519
-    _globals["_TAXDELETEREQUEST"]._serialized_start = 1521
-    _globals["_TAXDELETEREQUEST"]._serialized_end = 1607
-    _globals["_TAXDELETERESPONSE"]._serialized_start = 1609
-    _globals["_TAXDELETERESPONSE"]._serialized_end = 1703
-    _globals["_TAXSERVICE"]._serialized_start = 1706
-    _globals["_TAXSERVICE"]._serialized_end = 2191
+    _globals["_UOM"]._serialized_start = 113
+    _globals["_UOM"]._serialized_end = 317
+    _globals["_UOMCREATEREQUEST"]._serialized_start = 320
+    _globals["_UOMCREATEREQUEST"]._serialized_end = 472
+    _globals["_UOMCREATERESPONSE"]._serialized_start = 475
+    _globals["_UOMCREATERESPONSE"]._serialized_end = 622
+    _globals["_UOMREADREQUEST"]._serialized_start = 625
+    _globals["_UOMREADREQUEST"]._serialized_end = 989
+    _globals["_UOMREADRESPONSE"]._serialized_start = 992
+    _globals["_UOMREADRESPONSE"]._serialized_end = 1197
+    _globals["_UOMUPDATEREQUEST"]._serialized_start = 1199
+    _globals["_UOMUPDATEREQUEST"]._serialized_end = 1326
+    _globals["_UOMUPDATERESPONSE"]._serialized_start = 1329
+    _globals["_UOMUPDATERESPONSE"]._serialized_end = 1476
+    _globals["_UOMDELETEREQUEST"]._serialized_start = 1478
+    _globals["_UOMDELETEREQUEST"]._serialized_end = 1564
+    _globals["_UOMDELETERESPONSE"]._serialized_start = 1566
+    _globals["_UOMDELETERESPONSE"]._serialized_end = 1660
+    _globals["_UOMSERVICE"]._serialized_start = 1663
+    _globals["_UOMSERVICE"]._serialized_end = 2157
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/tax_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/tax_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/tax_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/tax_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/territory_matrix_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/territory_matrix_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/territory_matrix_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/territory_matrix_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/territory_matrix_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/territory_matrix_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/territory_matrix_value_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/territory_matrix_value_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/timezone_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/timezone_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/timezone_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/timezone_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/timezone_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/timezone_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/uom_pb2.py` & `omni-pro-0.1.25/omni/pro/protos/v1/stock/sequence_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/utilities/uom.proto
+# source: v1/stock/sequence.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
@@ -12,36 +12,36 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x16v1/utilities/uom.proto\x12!pro.omni.oms.api.v1.utilities.uom\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xcc\x01\n\x03Uom\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08\x63\x61tegory\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\x10\n\x08rounding\x18\x06 \x01(\x01\x12*\n\x06\x61\x63tive\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x08 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x98\x01\n\x10UomCreateRequest\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\t\x12\x10\n\x08rounding\x18\x05 \x01(\x01\x12\x36\n\x07\x63ontext\x18\x06 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x93\x01\n\x11UomCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x33\n\x03uom\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.uom.Uom"\xec\x02\n\x0eUomReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xcd\x01\n\x0fUomReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x34\n\x04uoms\x18\x03 \x03(\x0b\x32&.pro.omni.oms.api.v1.utilities.uom.Uom"\x7f\n\x10UomUpdateRequest\x12\x33\n\x03uom\x18\x01 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.uom.Uom\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x93\x01\n\x11UomUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x33\n\x03uom\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.uom.Uom"V\n\x10UomDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"^\n\x11UomDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xee\x03\n\nUomService\x12x\n\tUomCreate\x12\x33.pro.omni.oms.api.v1.utilities.uom.UomCreateRequest\x1a\x34.pro.omni.oms.api.v1.utilities.uom.UomCreateResponse"\x00\x12r\n\x07UomRead\x12\x31.pro.omni.oms.api.v1.utilities.uom.UomReadRequest\x1a\x32.pro.omni.oms.api.v1.utilities.uom.UomReadResponse"\x00\x12x\n\tUomUpdate\x12\x33.pro.omni.oms.api.v1.utilities.uom.UomUpdateRequest\x1a\x34.pro.omni.oms.api.v1.utilities.uom.UomUpdateResponse"\x00\x12x\n\tUomDelete\x12\x33.pro.omni.oms.api.v1.utilities.uom.UomDeleteRequest\x1a\x34.pro.omni.oms.api.v1.utilities.uom.UomDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x17v1/stock/sequence.proto\x12"pro.omni.oms.api.v1.stock.sequence\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xb8\x01\n\x08Sequence\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x17\n\x0fsequence_doc_id\x18\x04 \x01(\t\x12*\n\x06\x61\x63tive\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x84\x01\n\x15SequenceCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x17\n\x0fsequence_doc_id\x18\x03 \x01(\t\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x16SequenceCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12>\n\x08sequence\x18\x02 \x01(\x0b\x32,.pro.omni.oms.api.v1.stock.sequence.Sequence"\xf1\x02\n\x13SequenceReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xdd\x01\n\x14SequenceReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12?\n\tsequences\x18\x03 \x03(\x0b\x32,.pro.omni.oms.api.v1.stock.sequence.Sequence"\x8f\x01\n\x15SequenceUpdateRequest\x12>\n\x08sequence\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.stock.sequence.Sequence\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x16SequenceUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12>\n\x08sequence\x18\x02 \x01(\x0b\x32,.pro.omni.oms.api.v1.stock.sequence.Sequence"[\n\x15SequenceDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"c\n\x16SequenceDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xbb\x04\n\x0fSequenceService\x12\x89\x01\n\x0eSequenceCreate\x12\x39.pro.omni.oms.api.v1.stock.sequence.SequenceCreateRequest\x1a:.pro.omni.oms.api.v1.stock.sequence.SequenceCreateResponse"\x00\x12\x83\x01\n\x0cSequenceRead\x12\x37.pro.omni.oms.api.v1.stock.sequence.SequenceReadRequest\x1a\x38.pro.omni.oms.api.v1.stock.sequence.SequenceReadResponse"\x00\x12\x89\x01\n\x0eSequenceUpdate\x12\x39.pro.omni.oms.api.v1.stock.sequence.SequenceUpdateRequest\x1a:.pro.omni.oms.api.v1.stock.sequence.SequenceUpdateResponse"\x00\x12\x89\x01\n\x0eSequenceDelete\x12\x39.pro.omni.oms.api.v1.stock.sequence.SequenceDeleteRequest\x1a:.pro.omni.oms.api.v1.stock.sequence.SequenceDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.utilities.uom_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.stock.sequence_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_UOM"]._serialized_start = 113
-    _globals["_UOM"]._serialized_end = 317
-    _globals["_UOMCREATEREQUEST"]._serialized_start = 320
-    _globals["_UOMCREATEREQUEST"]._serialized_end = 472
-    _globals["_UOMCREATERESPONSE"]._serialized_start = 475
-    _globals["_UOMCREATERESPONSE"]._serialized_end = 622
-    _globals["_UOMREADREQUEST"]._serialized_start = 625
-    _globals["_UOMREADREQUEST"]._serialized_end = 989
-    _globals["_UOMREADRESPONSE"]._serialized_start = 992
-    _globals["_UOMREADRESPONSE"]._serialized_end = 1197
-    _globals["_UOMUPDATEREQUEST"]._serialized_start = 1199
-    _globals["_UOMUPDATEREQUEST"]._serialized_end = 1326
-    _globals["_UOMUPDATERESPONSE"]._serialized_start = 1329
-    _globals["_UOMUPDATERESPONSE"]._serialized_end = 1476
-    _globals["_UOMDELETEREQUEST"]._serialized_start = 1478
-    _globals["_UOMDELETEREQUEST"]._serialized_end = 1564
-    _globals["_UOMDELETERESPONSE"]._serialized_start = 1566
-    _globals["_UOMDELETERESPONSE"]._serialized_end = 1660
-    _globals["_UOMSERVICE"]._serialized_start = 1663
-    _globals["_UOMSERVICE"]._serialized_end = 2157
+    _globals["_SEQUENCE"]._serialized_start = 115
+    _globals["_SEQUENCE"]._serialized_end = 299
+    _globals["_SEQUENCECREATEREQUEST"]._serialized_start = 302
+    _globals["_SEQUENCECREATEREQUEST"]._serialized_end = 434
+    _globals["_SEQUENCECREATERESPONSE"]._serialized_start = 437
+    _globals["_SEQUENCECREATERESPONSE"]._serialized_end = 600
+    _globals["_SEQUENCEREADREQUEST"]._serialized_start = 603
+    _globals["_SEQUENCEREADREQUEST"]._serialized_end = 972
+    _globals["_SEQUENCEREADRESPONSE"]._serialized_start = 975
+    _globals["_SEQUENCEREADRESPONSE"]._serialized_end = 1196
+    _globals["_SEQUENCEUPDATEREQUEST"]._serialized_start = 1199
+    _globals["_SEQUENCEUPDATEREQUEST"]._serialized_end = 1342
+    _globals["_SEQUENCEUPDATERESPONSE"]._serialized_start = 1345
+    _globals["_SEQUENCEUPDATERESPONSE"]._serialized_end = 1508
+    _globals["_SEQUENCEDELETEREQUEST"]._serialized_start = 1510
+    _globals["_SEQUENCEDELETEREQUEST"]._serialized_end = 1601
+    _globals["_SEQUENCEDELETERESPONSE"]._serialized_start = 1603
+    _globals["_SEQUENCEDELETERESPONSE"]._serialized_end = 1702
+    _globals["_SEQUENCESERVICE"]._serialized_start = 1705
+    _globals["_SEQUENCESERVICE"]._serialized_end = 2276
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/uom_pb2.pyi` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/uom_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -142,18 +142,18 @@
         uom: _Optional[_Union[Uom, _Mapping]] = ...,
     ) -> None: ...
 
 class UomDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    id: int
+    id: str
     context: _base_pb2.Context
     def __init__(
-        self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
+        self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
 class UomDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.24/omni/pro/protos/v1/utilities/uom_pb2_grpc.py` & `omni-pro-0.1.25/omni/pro/protos/v1/utilities/uom_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/stack.py` & `omni-pro-0.1.25/omni/pro/stack.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/user/access.py` & `omni-pro-0.1.25/omni/pro/user/access.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/util.py` & `omni-pro-0.1.25/omni/pro/util.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni/pro/validators.py` & `omni-pro-0.1.25/omni/pro/validators.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.24/omni_pro.egg-info/PKG-INFO` & `omni-pro-0.1.25/omni_pro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omni-pro
-Version: 0.1.24
+Version: 0.1.25
 Summary: Python library designed to be a utility for OMS microservices
 Home-page: https://github.com/Omnipro-Solutions/saas-ms-library
 Author: OMNI.PRO
 Author-email: development@omni.pro
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `omni-pro-0.1.24/omni_pro.egg-info/SOURCES.txt` & `omni-pro-0.1.25/omni_pro.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 omni/pro/util.py
 omni/pro/validators.py
 omni/pro/data/models.user.csv
 omni/pro/models/__init__.py
 omni/pro/models/base.py
 omni/pro/models/common/__init__.py
 omni/pro/models/common/ms.py
+omni/pro/models/custom_fields/__init__.py
+omni/pro/models/custom_fields/enum.py
 omni/pro/models/sql/__init__.py
 omni/pro/models/sql/catalog/__init__.py
 omni/pro/models/sql/catalog/category.py
 omni/pro/models/sql/common/__init__.py
 omni/pro/models/sql/common/country.py
 omni/pro/models/sql/rules/__init__.py
 omni/pro/models/sql/rules/calendar.py
@@ -239,14 +241,17 @@
 omni/pro/protos/v1/stock/quant_pb2_grpc.py
 omni/pro/protos/v1/stock/route_pb2.py
 omni/pro/protos/v1/stock/route_pb2.pyi
 omni/pro/protos/v1/stock/route_pb2_grpc.py
 omni/pro/protos/v1/stock/rule_pb2.py
 omni/pro/protos/v1/stock/rule_pb2.pyi
 omni/pro/protos/v1/stock/rule_pb2_grpc.py
+omni/pro/protos/v1/stock/sequence_pb2.py
+omni/pro/protos/v1/stock/sequence_pb2.pyi
+omni/pro/protos/v1/stock/sequence_pb2_grpc.py
 omni/pro/protos/v1/stock/stock_move_line_pb2.py
 omni/pro/protos/v1/stock/stock_move_line_pb2.pyi
 omni/pro/protos/v1/stock/stock_move_line_pb2_grpc.py
 omni/pro/protos/v1/stock/stock_move_pb2.py
 omni/pro/protos/v1/stock/stock_move_pb2.pyi
 omni/pro/protos/v1/stock/stock_move_pb2_grpc.py
 omni/pro/protos/v1/stock/uom_pb2.py
@@ -277,14 +282,17 @@
 omni/pro/protos/v1/utilities/language_pb2_grpc.py
 omni/pro/protos/v1/utilities/model_pb2.py
 omni/pro/protos/v1/utilities/model_pb2.pyi
 omni/pro/protos/v1/utilities/model_pb2_grpc.py
 omni/pro/protos/v1/utilities/payment_method_pb2.py
 omni/pro/protos/v1/utilities/payment_method_pb2.pyi
 omni/pro/protos/v1/utilities/payment_method_pb2_grpc.py
+omni/pro/protos/v1/utilities/sequence_pb2.py
+omni/pro/protos/v1/utilities/sequence_pb2.pyi
+omni/pro/protos/v1/utilities/sequence_pb2_grpc.py
 omni/pro/protos/v1/utilities/tax_pb2.py
 omni/pro/protos/v1/utilities/tax_pb2.pyi
 omni/pro/protos/v1/utilities/tax_pb2_grpc.py
 omni/pro/protos/v1/utilities/territory_matrix_pb2.py
 omni/pro/protos/v1/utilities/territory_matrix_pb2.pyi
 omni/pro/protos/v1/utilities/territory_matrix_pb2_grpc.py
 omni/pro/protos/v1/utilities/territory_matrix_value_pb2.py
```

### Comparing `omni-pro-0.1.24/setup.py` & `omni-pro-0.1.25/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # The directory containing this file
 HERE = Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 DESCRIPTION = "Python library designed to be a utility for OMS microservices"
-VERSION = "0.1.24"
+VERSION = "0.1.25"
 PACKAGE_NAME = "omni-pro"
 AUTHOR = "OMNI.PRO"
 AUTHOR_EMAIL = "development@omni.pro"
 URL = "https://github.com/Omnipro-Solutions/saas-ms-library"
 
 INSTALL_REQUIRES = [
     "protobuf==4.23.4",
```

