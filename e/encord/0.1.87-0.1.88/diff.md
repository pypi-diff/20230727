# Comparing `tmp/encord-0.1.87.tar.gz` & `tmp/encord-0.1.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encord-0.1.87.tar", max compression
+gzip compressed data, was "encord-0.1.88.tar", max compression
```

## Comparing `encord-0.1.87.tar` & `encord-0.1.88.tar`

### file list

```diff
@@ -1,89 +1,92 @@
--rw-r--r--   0        0        0    11330 2023-07-24 15:47:37.430500 encord-0.1.87/LICENSE
--rw-r--r--   0        0        0     2027 2023-07-24 15:47:37.430500 encord-0.1.87/README.md
--rw-r--r--   0        0        0      158 2023-07-24 15:47:37.446500 encord-0.1.87/encord/__init__.py
--rw-r--r--   0        0        0      100 2023-07-24 15:47:37.446500 encord-0.1.87/encord/_version.py
--rw-r--r--   0        0        0    49616 2023-07-24 15:47:37.446500 encord-0.1.87/encord/client.py
--rw-r--r--   0        0        0        0 2023-07-24 15:47:37.446500 encord-0.1.87/encord/common/__init__.py
--rw-r--r--   0        0        0       45 2023-07-24 15:47:37.446500 encord-0.1.87/encord/common/constants.py
--rw-r--r--   0        0        0      508 2023-07-24 15:47:37.446500 encord-0.1.87/encord/common/enum.py
--rw-r--r--   0        0        0    10852 2023-07-24 15:47:37.446500 encord-0.1.87/encord/configs.py
--rw-r--r--   0        0        0        0 2023-07-24 15:47:37.446500 encord-0.1.87/encord/constants/__init__.py
--rw-r--r--   0        0        0      866 2023-07-24 15:47:37.446500 encord-0.1.87/encord/constants/enums.py
--rw-r--r--   0        0        0     3196 2023-07-24 15:47:37.446500 encord-0.1.87/encord/constants/model.py
--rw-r--r--   0        0        0     4522 2023-07-24 15:47:37.446500 encord-0.1.87/encord/constants/model_weights.py
--rw-r--r--   0        0        0     1119 2023-07-24 15:47:37.446500 encord-0.1.87/encord/constants/string_constants.py
--rw-r--r--   0        0        0        0 2023-07-24 15:47:37.446500 encord-0.1.87/encord/constants/test/__init__.py
--rw-r--r--   0        0        0      634 2023-07-24 15:47:37.446500 encord-0.1.87/encord/constants/test/test_enums.py
--rw-r--r--   0        0        0    16021 2023-07-24 15:47:37.446500 encord-0.1.87/encord/dataset.py
--rw-r--r--   0        0        0     6355 2023-07-24 15:47:37.446500 encord-0.1.87/encord/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/__init__.py
--rw-r--r--   0        0        0     5315 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/bundle.py
--rw-r--r--   0        0        0      319 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/common.py
--rw-r--r--   0        0        0      535 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/constants.py
--rw-r--r--   0        0        0     7234 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/error_utils.py
--rw-r--r--   0        0        0      103 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/limits.py
--rw-r--r--   0        0        0     7886 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/querier.py
--rw-r--r--   0        0        0      747 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/query_methods.py
--rw-r--r--   0        0        0     1738 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/request.py
--rw-r--r--   0        0        0     6182 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/utils.py
--rw-r--r--   0        0        0        0 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/v2/__init__.py
--rw-r--r--   0        0        0     3388 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/v2/api_client.py
--rw-r--r--   0        0        0      964 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/v2/error_utils.py
--rw-r--r--   0        0        0      223 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/v2/payloads.py
--rw-r--r--   0        0        0     2249 2023-07-24 15:47:37.446500 encord-0.1.87/encord/http/v2/request_signer.py
--rw-r--r--   0        0        0      340 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/__init__.py
--rw-r--r--   0        0        0     5164 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/bitmask.py
--rw-r--r--   0        0        0      182 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/classification.py
--rw-r--r--   0        0        0    21796 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/common.py
--rw-r--r--   0        0        0      151 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/constants.py
--rw-r--r--   0        0        0     5748 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/coordinates.py
--rw-r--r--   0        0        0     3461 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/frames.py
--rw-r--r--   0        0        0    22033 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/internal_helpers.py
--rw-r--r--   0        0        0   140628 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/ontology_labels_impl.py
--rw-r--r--   0        0        0      174 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/ontology_object.py
--rw-r--r--   0        0        0      185 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/ontology_structure.py
--rw-r--r--   0        0        0      549 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/project.py
--rw-r--r--   0        0        0     1622 2023-07-24 15:47:37.446500 encord-0.1.87/encord/objects/utils.py
--rw-r--r--   0        0        0     3430 2023-07-24 15:47:37.446500 encord-0.1.87/encord/ontology.py
--rw-r--r--   0        0        0        0 2023-07-24 15:47:37.446500 encord-0.1.87/encord/orm/__init__.py
--rw-r--r--   0        0        0      932 2023-07-24 15:47:37.446500 encord-0.1.87/encord/orm/analytics.py
--rw-r--r--   0        0        0      982 2023-07-24 15:47:37.446500 encord-0.1.87/encord/orm/api_key.py
--rw-r--r--   0        0        0      486 2023-07-24 15:47:37.446500 encord-0.1.87/encord/orm/base_dto/__init__.py
--rw-r--r--   0        0        0      337 2023-07-24 15:47:37.446500 encord-0.1.87/encord/orm/base_dto/base_dto_interface.py
--rw-r--r--   0        0        0     1418 2023-07-24 15:47:37.446500 encord-0.1.87/encord/orm/base_dto/base_dto_pydantic_v1.py
--rw-r--r--   0        0        0     1481 2023-07-24 15:47:37.446500 encord-0.1.87/encord/orm/base_dto/base_dto_pydantic_v2.py
--rw-r--r--   0        0        0     5335 2023-07-24 15:47:37.446500 encord-0.1.87/encord/orm/base_orm.py
--rw-r--r--   0        0        0      111 2023-07-24 15:47:37.446500 encord-0.1.87/encord/orm/cloud_integration.py
--rw-r--r--   0        0        0    32993 2023-07-24 15:47:37.446500 encord-0.1.87/encord/orm/dataset.py
--rw-r--r--   0        0        0      829 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/dataset_with_user_role.py
--rw-r--r--   0        0        0      256 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/formatter.py
--rw-r--r--   0        0        0     1241 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/label_log.py
--rw-r--r--   0        0        0    11889 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/label_row.py
--rw-r--r--   0        0        0     1577 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/labeling_algorithm.py
--rw-r--r--   0        0        0     6667 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/model.py
--rw-r--r--   0        0        0      874 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/ontology.py
--rw-r--r--   0        0        0     8658 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/project.py
--rw-r--r--   0        0        0      625 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/project_api_key.py
--rw-r--r--   0        0        0      828 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/project_with_user_role.py
--rw-r--r--   0        0        0        0 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/test/__init__.py
--rw-r--r--   0        0        0      570 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/test/test_dataset.py
--rw-r--r--   0        0        0      314 2023-07-24 15:47:37.450501 encord-0.1.87/encord/orm/workflow.py
--rw-r--r--   0        0        0    41332 2023-07-24 15:47:37.450501 encord-0.1.87/encord/project.py
--rw-r--r--   0        0        0        0 2023-07-24 15:47:37.450501 encord-0.1.87/encord/project_ontology/__init__.py
--rw-r--r--   0        0        0     1316 2023-07-24 15:47:37.450501 encord-0.1.87/encord/project_ontology/classification_attribute.py
--rw-r--r--   0        0        0      525 2023-07-24 15:47:37.450501 encord-0.1.87/encord/project_ontology/classification_option.py
--rw-r--r--   0        0        0      357 2023-07-24 15:47:37.450501 encord-0.1.87/encord/project_ontology/classification_type.py
--rw-r--r--   0        0        0      237 2023-07-24 15:47:37.450501 encord-0.1.87/encord/project_ontology/object_type.py
--rw-r--r--   0        0        0     9676 2023-07-24 15:47:37.450501 encord-0.1.87/encord/project_ontology/ontology.py
--rw-r--r--   0        0        0      630 2023-07-24 15:47:37.450501 encord-0.1.87/encord/project_ontology/ontology_classification.py
--rw-r--r--   0        0        0      683 2023-07-24 15:47:37.450501 encord-0.1.87/encord/project_ontology/ontology_object.py
--rw-r--r--   0        0        0    29036 2023-07-24 15:47:37.450501 encord-0.1.87/encord/user_client.py
--rw-r--r--   0        0        0        0 2023-07-24 15:47:37.450501 encord-0.1.87/encord/utilities/__init__.py
--rw-r--r--   0        0        0     4282 2023-07-24 15:47:37.450501 encord-0.1.87/encord/utilities/client_utilities.py
--rw-r--r--   0        0        0      253 2023-07-24 15:47:37.450501 encord-0.1.87/encord/utilities/common.py
--rw-r--r--   0        0        0     3270 2023-07-24 15:47:37.450501 encord-0.1.87/encord/utilities/label_utilities.py
--rw-r--r--   0        0        0      343 2023-07-24 15:47:37.450501 encord-0.1.87/encord/utilities/ontology_user.py
--rw-r--r--   0        0        0      578 2023-07-24 15:47:37.450501 encord-0.1.87/encord/utilities/project_user.py
--rw-r--r--   0        0        0      467 2023-07-24 15:47:37.450501 encord-0.1.87/encord/utilities/project_utilities.py
--rw-r--r--   0        0        0     1989 2023-07-24 15:47:37.450501 encord-0.1.87/pyproject.toml
--rw-r--r--   0        0        0     3106 1970-01-01 00:00:00.000000 encord-0.1.87/PKG-INFO
+-rw-r--r--   0        0        0    11330 2023-07-27 16:11:34.423414 encord-0.1.88/LICENSE
+-rw-r--r--   0        0        0     2027 2023-07-27 16:11:34.423414 encord-0.1.88/README.md
+-rw-r--r--   0        0        0      158 2023-07-27 16:11:34.439414 encord-0.1.88/encord/__init__.py
+-rw-r--r--   0        0        0      100 2023-07-27 16:11:34.439414 encord-0.1.88/encord/_version.py
+-rw-r--r--   0        0        0    48749 2023-07-27 16:11:34.439414 encord-0.1.88/encord/client.py
+-rw-r--r--   0        0        0        0 2023-07-27 16:11:34.439414 encord-0.1.88/encord/common/__init__.py
+-rw-r--r--   0        0        0       45 2023-07-27 16:11:34.439414 encord-0.1.88/encord/common/constants.py
+-rw-r--r--   0        0        0      508 2023-07-27 16:11:34.439414 encord-0.1.88/encord/common/enum.py
+-rw-r--r--   0        0        0    10852 2023-07-27 16:11:34.439414 encord-0.1.88/encord/configs.py
+-rw-r--r--   0        0        0        0 2023-07-27 16:11:34.439414 encord-0.1.88/encord/constants/__init__.py
+-rw-r--r--   0        0        0      866 2023-07-27 16:11:34.439414 encord-0.1.88/encord/constants/enums.py
+-rw-r--r--   0        0        0     3196 2023-07-27 16:11:34.439414 encord-0.1.88/encord/constants/model.py
+-rw-r--r--   0        0        0     4522 2023-07-27 16:11:34.439414 encord-0.1.88/encord/constants/model_weights.py
+-rw-r--r--   0        0        0     1119 2023-07-27 16:11:34.439414 encord-0.1.88/encord/constants/string_constants.py
+-rw-r--r--   0        0        0        0 2023-07-27 16:11:34.439414 encord-0.1.88/encord/constants/test/__init__.py
+-rw-r--r--   0        0        0      634 2023-07-27 16:11:34.443415 encord-0.1.88/encord/constants/test/test_enums.py
+-rw-r--r--   0        0        0    16021 2023-07-27 16:11:34.443415 encord-0.1.88/encord/dataset.py
+-rw-r--r--   0        0        0     6355 2023-07-27 16:11:34.443415 encord-0.1.88/encord/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-27 16:11:34.443415 encord-0.1.88/encord/http/__init__.py
+-rw-r--r--   0        0        0     5315 2023-07-27 16:11:34.443415 encord-0.1.88/encord/http/bundle.py
+-rw-r--r--   0        0        0      319 2023-07-27 16:11:34.443415 encord-0.1.88/encord/http/common.py
+-rw-r--r--   0        0        0      535 2023-07-27 16:11:34.443415 encord-0.1.88/encord/http/constants.py
+-rw-r--r--   0        0        0     7234 2023-07-27 16:11:34.443415 encord-0.1.88/encord/http/error_utils.py
+-rw-r--r--   0        0        0      103 2023-07-27 16:11:34.443415 encord-0.1.88/encord/http/limits.py
+-rw-r--r--   0        0        0     7886 2023-07-27 16:11:34.443415 encord-0.1.88/encord/http/querier.py
+-rw-r--r--   0        0        0      747 2023-07-27 16:11:34.443415 encord-0.1.88/encord/http/query_methods.py
+-rw-r--r--   0        0        0     1738 2023-07-27 16:11:34.443415 encord-0.1.88/encord/http/request.py
+-rw-r--r--   0        0        0     6182 2023-07-27 16:11:34.443415 encord-0.1.88/encord/http/utils.py
+-rw-r--r--   0        0        0        0 2023-07-27 16:11:34.443415 encord-0.1.88/encord/http/v2/__init__.py
+-rw-r--r--   0        0        0     3388 2023-07-27 16:11:34.443415 encord-0.1.88/encord/http/v2/api_client.py
+-rw-r--r--   0        0        0      964 2023-07-27 16:11:34.443415 encord-0.1.88/encord/http/v2/error_utils.py
+-rw-r--r--   0        0        0      223 2023-07-27 16:11:34.443415 encord-0.1.88/encord/http/v2/payloads.py
+-rw-r--r--   0        0        0     2249 2023-07-27 16:11:34.443415 encord-0.1.88/encord/http/v2/request_signer.py
+-rw-r--r--   0        0        0      491 2023-07-27 16:11:34.443415 encord-0.1.88/encord/objects/__init__.py
+-rw-r--r--   0        0        0     5164 2023-07-27 16:11:34.443415 encord-0.1.88/encord/objects/bitmask.py
+-rw-r--r--   0        0        0     3282 2023-07-27 16:11:34.443415 encord-0.1.88/encord/objects/classification.py
+-rw-r--r--   0        0        0    24224 2023-07-27 16:11:34.443415 encord-0.1.88/encord/objects/classification_instance.py
+-rw-r--r--   0        0        0    17233 2023-07-27 16:11:34.443415 encord-0.1.88/encord/objects/common.py
+-rw-r--r--   0        0        0      151 2023-07-27 16:11:34.443415 encord-0.1.88/encord/objects/constants.py
+-rw-r--r--   0        0        0     5748 2023-07-27 16:11:34.443415 encord-0.1.88/encord/objects/coordinates.py
+-rw-r--r--   0        0        0     3461 2023-07-27 16:11:34.443415 encord-0.1.88/encord/objects/frames.py
+-rw-r--r--   0        0        0    22072 2023-07-27 16:11:34.443415 encord-0.1.88/encord/objects/internal_helpers.py
+-rw-r--r--   0        0        0     5045 2023-07-27 16:11:34.443415 encord-0.1.88/encord/objects/ontology_element.py
+-rw-r--r--   0        0        0    76273 2023-07-27 16:11:34.443415 encord-0.1.88/encord/objects/ontology_labels_impl.py
+-rw-r--r--   0        0        0     3544 2023-07-27 16:11:34.443415 encord-0.1.88/encord/objects/ontology_object.py
+-rw-r--r--   0        0        0    35816 2023-07-27 16:11:34.443415 encord-0.1.88/encord/objects/ontology_object_instance.py
+-rw-r--r--   0        0        0      185 2023-07-27 16:11:34.443415 encord-0.1.88/encord/objects/ontology_structure.py
+-rw-r--r--   0        0        0      549 2023-07-27 16:11:34.443415 encord-0.1.88/encord/objects/project.py
+-rw-r--r--   0        0        0     1622 2023-07-27 16:11:34.443415 encord-0.1.88/encord/objects/utils.py
+-rw-r--r--   0        0        0     3430 2023-07-27 16:11:34.443415 encord-0.1.88/encord/ontology.py
+-rw-r--r--   0        0        0        0 2023-07-27 16:11:34.443415 encord-0.1.88/encord/orm/__init__.py
+-rw-r--r--   0        0        0      932 2023-07-27 16:11:34.443415 encord-0.1.88/encord/orm/analytics.py
+-rw-r--r--   0        0        0      982 2023-07-27 16:11:34.443415 encord-0.1.88/encord/orm/api_key.py
+-rw-r--r--   0        0        0      486 2023-07-27 16:11:34.443415 encord-0.1.88/encord/orm/base_dto/__init__.py
+-rw-r--r--   0        0        0      337 2023-07-27 16:11:34.443415 encord-0.1.88/encord/orm/base_dto/base_dto_interface.py
+-rw-r--r--   0        0        0     1418 2023-07-27 16:11:34.443415 encord-0.1.88/encord/orm/base_dto/base_dto_pydantic_v1.py
+-rw-r--r--   0        0        0     1481 2023-07-27 16:11:34.443415 encord-0.1.88/encord/orm/base_dto/base_dto_pydantic_v2.py
+-rw-r--r--   0        0        0     5335 2023-07-27 16:11:34.443415 encord-0.1.88/encord/orm/base_orm.py
+-rw-r--r--   0        0        0      111 2023-07-27 16:11:34.443415 encord-0.1.88/encord/orm/cloud_integration.py
+-rw-r--r--   0        0        0    32993 2023-07-27 16:11:34.443415 encord-0.1.88/encord/orm/dataset.py
+-rw-r--r--   0        0        0      829 2023-07-27 16:11:34.443415 encord-0.1.88/encord/orm/dataset_with_user_role.py
+-rw-r--r--   0        0        0      256 2023-07-27 16:11:34.443415 encord-0.1.88/encord/orm/formatter.py
+-rw-r--r--   0        0        0     1241 2023-07-27 16:11:34.443415 encord-0.1.88/encord/orm/label_log.py
+-rw-r--r--   0        0        0    11889 2023-07-27 16:11:34.443415 encord-0.1.88/encord/orm/label_row.py
+-rw-r--r--   0        0        0     1577 2023-07-27 16:11:34.443415 encord-0.1.88/encord/orm/labeling_algorithm.py
+-rw-r--r--   0        0        0     6667 2023-07-27 16:11:34.443415 encord-0.1.88/encord/orm/model.py
+-rw-r--r--   0        0        0      874 2023-07-27 16:11:34.443415 encord-0.1.88/encord/orm/ontology.py
+-rw-r--r--   0        0        0     8658 2023-07-27 16:11:34.443415 encord-0.1.88/encord/orm/project.py
+-rw-r--r--   0        0        0      625 2023-07-27 16:11:34.443415 encord-0.1.88/encord/orm/project_api_key.py
+-rw-r--r--   0        0        0      828 2023-07-27 16:11:34.443415 encord-0.1.88/encord/orm/project_with_user_role.py
+-rw-r--r--   0        0        0        0 2023-07-27 16:11:34.443415 encord-0.1.88/encord/orm/test/__init__.py
+-rw-r--r--   0        0        0      570 2023-07-27 16:11:34.443415 encord-0.1.88/encord/orm/test/test_dataset.py
+-rw-r--r--   0        0        0      314 2023-07-27 16:11:34.443415 encord-0.1.88/encord/orm/workflow.py
+-rw-r--r--   0        0        0    41451 2023-07-27 16:11:34.443415 encord-0.1.88/encord/project.py
+-rw-r--r--   0        0        0        0 2023-07-27 16:11:34.443415 encord-0.1.88/encord/project_ontology/__init__.py
+-rw-r--r--   0        0        0     1316 2023-07-27 16:11:34.447414 encord-0.1.88/encord/project_ontology/classification_attribute.py
+-rw-r--r--   0        0        0      525 2023-07-27 16:11:34.447414 encord-0.1.88/encord/project_ontology/classification_option.py
+-rw-r--r--   0        0        0      357 2023-07-27 16:11:34.447414 encord-0.1.88/encord/project_ontology/classification_type.py
+-rw-r--r--   0        0        0      237 2023-07-27 16:11:34.447414 encord-0.1.88/encord/project_ontology/object_type.py
+-rw-r--r--   0        0        0     9676 2023-07-27 16:11:34.447414 encord-0.1.88/encord/project_ontology/ontology.py
+-rw-r--r--   0        0        0      630 2023-07-27 16:11:34.447414 encord-0.1.88/encord/project_ontology/ontology_classification.py
+-rw-r--r--   0        0        0      683 2023-07-27 16:11:34.447414 encord-0.1.88/encord/project_ontology/ontology_object.py
+-rw-r--r--   0        0        0    29036 2023-07-27 16:11:34.447414 encord-0.1.88/encord/user_client.py
+-rw-r--r--   0        0        0        0 2023-07-27 16:11:34.447414 encord-0.1.88/encord/utilities/__init__.py
+-rw-r--r--   0        0        0     4282 2023-07-27 16:11:34.447414 encord-0.1.88/encord/utilities/client_utilities.py
+-rw-r--r--   0        0        0      253 2023-07-27 16:11:34.447414 encord-0.1.88/encord/utilities/common.py
+-rw-r--r--   0        0        0     3270 2023-07-27 16:11:34.447414 encord-0.1.88/encord/utilities/label_utilities.py
+-rw-r--r--   0        0        0      343 2023-07-27 16:11:34.447414 encord-0.1.88/encord/utilities/ontology_user.py
+-rw-r--r--   0        0        0      578 2023-07-27 16:11:34.447414 encord-0.1.88/encord/utilities/project_user.py
+-rw-r--r--   0        0        0      467 2023-07-27 16:11:34.447414 encord-0.1.88/encord/utilities/project_utilities.py
+-rw-r--r--   0        0        0     1989 2023-07-27 16:11:34.447414 encord-0.1.88/pyproject.toml
+-rw-r--r--   0        0        0     3106 1970-01-01 00:00:00.000000 encord-0.1.88/PKG-INFO
```

### Comparing `encord-0.1.87/LICENSE` & `encord-0.1.88/LICENSE`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/README.md` & `encord-0.1.88/README.md`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/client.py` & `encord-0.1.88/encord/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,36 +211,18 @@
             return EncordClientDataset(querier, config)
 
         else:
             raise encord.exceptions.InitialisationError(
                 message=f"API key [{config.api_key}] is not associated with a project or dataset"
             )
 
-    def __getattr__(self, name):
-        """Overriding __getattr__."""
-        value = self.__dict__.get(name)
-        if not value:
-            self_type = type(self).__name__
-            if self_type == "CordClientDataset" and name in EncordClientProject.__dict__.keys():
-                raise encord.exceptions.EncordException(message=f"{name} is implemented in Projects, not Datasets.")
-            elif self_type == "CordClientProject" and name in EncordClientDataset.__dict__.keys():
-                raise encord.exceptions.EncordException(message=f"{name} is implemented in Datasets, not Projects.")
-            elif name == "items":
-                pass
-            else:
-                raise encord.exceptions.EncordException(message=f"{name} is not implemented.")
-        return value
-
     def get_cloud_integrations(self) -> List[CloudIntegration]:
         return self._querier.get_multiple(CloudIntegration)
 
 
-CordClient = EncordClient
-
-
 class EncordClientDataset(EncordClient):
     """
     DEPRECATED - prefer using the :class:`encord.dataset.Dataset` instead
     """
 
     def __init__(
         self,
@@ -703,17 +685,14 @@
         payload = {"image_group_data_hash": image_group_id}
 
         response = self._querier.get_multiple(ImageGroupOCR, payload=payload)
 
         return response
 
 
-CordClientDataset = EncordClientDataset
-
-
 class EncordClientProject(EncordClient):
     """
     DEPRECATED - prefer using the :class:`encord.project.Project` instead
     """
 
     def get_project(self, include_labels_metadata=True) -> OrmProject:
         """
```

### Comparing `encord-0.1.87/encord/configs.py` & `encord-0.1.88/encord/configs.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/constants/enums.py` & `encord-0.1.88/encord/constants/enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/constants/model.py` & `encord-0.1.88/encord/constants/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/constants/model_weights.py` & `encord-0.1.88/encord/constants/model_weights.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/constants/string_constants.py` & `encord-0.1.88/encord/constants/string_constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/constants/test/test_enums.py` & `encord-0.1.88/encord/constants/test/test_enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/dataset.py` & `encord-0.1.88/encord/dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/exceptions.py` & `encord-0.1.88/encord/exceptions.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/http/bundle.py` & `encord-0.1.88/encord/http/bundle.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/http/constants.py` & `encord-0.1.88/encord/http/constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/http/error_utils.py` & `encord-0.1.88/encord/http/error_utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/http/querier.py` & `encord-0.1.88/encord/http/querier.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/http/query_methods.py` & `encord-0.1.88/encord/http/query_methods.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/http/request.py` & `encord-0.1.88/encord/http/request.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/http/utils.py` & `encord-0.1.88/encord/http/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/http/v2/api_client.py` & `encord-0.1.88/encord/http/v2/api_client.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/http/v2/error_utils.py` & `encord-0.1.88/encord/http/v2/error_utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/http/v2/request_signer.py` & `encord-0.1.88/encord/http/v2/request_signer.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/objects/bitmask.py` & `encord-0.1.88/encord/objects/bitmask.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/objects/coordinates.py` & `encord-0.1.88/encord/objects/coordinates.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/objects/frames.py` & `encord-0.1.88/encord/objects/frames.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/objects/internal_helpers.py` & `encord-0.1.88/encord/objects/internal_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,18 +21,18 @@
     Attribute,
     ChecklistAttribute,
     FlatOption,
     NestableOption,
     Option,
     RadioAttribute,
     TextAttribute,
-    _get_element_by_hash,
 )
 from encord.objects.constants import DEFAULT_MANUAL_ANNOTATION
 from encord.objects.frames import Ranges, ranges_to_list
+from encord.objects.ontology_element import _get_element_by_hash
 from encord.objects.utils import _lower_snake_case, short_uuid_str
 
 ValueType = TypeVar("ValueType")
 AttributeType = TypeVar("AttributeType", bound=Attribute)
 
 
 class Answer(ABC, Generic[ValueType, AttributeType]):
```

### Comparing `encord-0.1.87/encord/objects/project.py` & `encord-0.1.88/encord/objects/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/objects/utils.py` & `encord-0.1.88/encord/objects/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/ontology.py` & `encord-0.1.88/encord/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/orm/analytics.py` & `encord-0.1.88/encord/orm/analytics.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/orm/api_key.py` & `encord-0.1.88/encord/orm/api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/orm/base_dto/base_dto_pydantic_v1.py` & `encord-0.1.88/encord/orm/base_dto/base_dto_pydantic_v1.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/orm/base_dto/base_dto_pydantic_v2.py` & `encord-0.1.88/encord/orm/base_dto/base_dto_pydantic_v2.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/orm/base_orm.py` & `encord-0.1.88/encord/orm/base_orm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/orm/dataset.py` & `encord-0.1.88/encord/orm/dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/orm/dataset_with_user_role.py` & `encord-0.1.88/encord/orm/dataset_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/orm/label_log.py` & `encord-0.1.88/encord/orm/label_log.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/orm/label_row.py` & `encord-0.1.88/encord/orm/label_row.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/orm/labeling_algorithm.py` & `encord-0.1.88/encord/orm/labeling_algorithm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/orm/model.py` & `encord-0.1.88/encord/orm/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/orm/ontology.py` & `encord-0.1.88/encord/orm/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/orm/project.py` & `encord-0.1.88/encord/orm/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/orm/project_api_key.py` & `encord-0.1.88/encord/orm/project_api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/orm/project_with_user_role.py` & `encord-0.1.88/encord/orm/project_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/orm/test/test_dataset.py` & `encord-0.1.88/encord/orm/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/project.py` & `encord-0.1.88/encord/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Iterable, List, Optional, Set, Tuple, Union
 
 from encord.client import EncordClientProject
 from encord.constants.model import AutomationModels, Device
 from encord.http.bundle import Bundle
 from encord.http.v2.api_client import ApiClient
 from encord.http.v2.payloads import Page
-from encord.objects import LabelRowV2
+from encord.objects import LabelRowV2, OntologyStructure
 from encord.ontology import Ontology
 from encord.orm.analytics import (
     CollaboratorTimer,
     CollaboratorTimerParams,
     CollaboratorTimersGroupBy,
 )
 from encord.orm.cloud_integration import CloudIntegration
@@ -87,29 +87,34 @@
         return project_instance.last_edited_at
 
     @property
     def ontology(self) -> dict:
         """
         Get the ontology of the project.
 
-        DEPRECATED: Prefer using the :class:`encord.objects.ontology_structure.OntologyStructure` class to work with the data.
-
-        .. code::
-
-            from encord.objects.ontology_structure import OntologyStructure
-
-            project = user_client.get_project("<project_hash>")
-
-            ontology = OntologyStructure.from_dict(project.ontology)
-
+        DEPRECATED: Prefer using the :meth:`encord.Project.ontology_structure` method.
         """
         project_instance = self._get_project_instance()
         return project_instance.editor_ontology
 
     @property
+    def ontology_hash(self) -> str:
+        """
+        Get the ontology hash of the project's ontology.
+        """
+        return self._ontology.ontology_hash
+
+    @property
+    def ontology_structure(self) -> OntologyStructure:
+        """
+        Get the ontology structure of the project's ontology.
+        """
+        return self._ontology.structure
+
+    @property
     def datasets(self) -> list:
         """
         Get the associated datasets.
 
         Prefer using the :meth:`encord.objects.project.ProjectDataset` class to work with the data.
 
         .. code::
```

### Comparing `encord-0.1.87/encord/project_ontology/classification_attribute.py` & `encord-0.1.88/encord/project_ontology/classification_attribute.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/project_ontology/classification_option.py` & `encord-0.1.88/encord/project_ontology/classification_option.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/project_ontology/ontology.py` & `encord-0.1.88/encord/project_ontology/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/project_ontology/ontology_classification.py` & `encord-0.1.88/encord/project_ontology/ontology_classification.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/project_ontology/ontology_object.py` & `encord-0.1.88/encord/project_ontology/ontology_object.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/user_client.py` & `encord-0.1.88/encord/user_client.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/utilities/client_utilities.py` & `encord-0.1.88/encord/utilities/client_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/utilities/label_utilities.py` & `encord-0.1.88/encord/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/encord/utilities/project_user.py` & `encord-0.1.88/encord/utilities/project_user.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.87/pyproject.toml` & `encord-0.1.88/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encord"
-version = "0.1.87"
+version = "0.1.88"
 description = "Encord Python SDK Client"
 authors = ["Cord Technologies Limited <hello@encord.com>"]
 license = "Apache Software License"
 keywords = ["encord"]
 packages = [
     { include = "encord"},
 ]
```

### Comparing `encord-0.1.87/PKG-INFO` & `encord-0.1.88/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encord
-Version: 0.1.87
+Version: 0.1.88
 Summary: Encord Python SDK Client
 Home-page: https://github.com/encord-team/encord-client-python
 License: Apache Software License
 Keywords: encord
 Author: Cord Technologies Limited
 Author-email: hello@encord.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: encord Version: 0.1.87 Summary: Encord Python SDK
+Metadata-Version: 2.1 Name: encord Version: 0.1.88 Summary: Encord Python SDK
 Client Home-page: https://github.com/encord-team/encord-client-python License:
 Apache Software License Keywords: encord Author: Cord Technologies Limited
 Author-email: hello@encord.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: Apache Software License Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

