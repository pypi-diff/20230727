# Comparing `tmp/vectice-23.2.7.1.tar.gz` & `tmp/vectice-23.2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectice-23.2.7.1.tar", last modified: Tue Jul 11 11:53:58 2023, max compression
+gzip compressed data, was "/home/runner/work/sdk-python/sdk-python/dist/.tmp-_fe4i8zn/vectice-23.2.8.0.tar", last modified: Thu Jul 27 12:05:24 2023, max compression
```

## Comparing `vectice-23.2.7.1.tar` & `vectice-23.2.8.0.tar`

### file list

```diff
@@ -1,137 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:53:58.647463 vectice-23.2.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 11:53:45.000000 vectice-23.2.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-11 11:53:58.647463 vectice-23.2.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-11 11:53:45.000000 vectice-23.2.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-11 11:53:45.000000 vectice-23.2.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-11 11:53:58.651463 vectice-23.2.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-11 11:53:45.000000 vectice-23.2.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:53:58.615463 vectice-23.2.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:53:58.619463 vectice-23.2.7.1/src/vectice/
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:53:58.627463 vectice-23.2.7.1/src/vectice/api/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/gql_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/gql_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/gql_code_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/gql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/gql_entity_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/gql_feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/gql_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/gql_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/gql_user_workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/http_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    12727 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/http_error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/iteration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:53:58.635463 vectice-23.2.7.1/src/vectice/api/json/
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/artifact_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/code.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/code_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/dataset_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/dataset_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/entity_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/model_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/model_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/model_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/organization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/paged_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/property.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/public_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/user_and_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/user_declared_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/json_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/api/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    21946 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:53:58.639463 vectice-23.2.7.1/src/vectice/models/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/attachment_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    14390 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/git_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:53:58.639463 vectice-23.2.7.1/src/vectice/models/representation/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/representation/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/representation/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/representation/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/representation/model_version_representation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:53:58.643463 vectice-23.2.7.1/src/vectice/models/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/bigquery_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/databricks_table_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/description.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/gcs_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:53:58.647463 vectice-23.2.7.1/src/vectice/models/resource/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/column_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/dataframe_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/db_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/df_wrapper_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/df_wrapper_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11652 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/df_wrapper_spark_df.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/extra_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/metadata/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/resource/s3_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    29620 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/step_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/step_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/step_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/step_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/step_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/models/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:53:58.647463 vectice-23.2.7.1/src/vectice/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/utils/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/utils/automatic_link_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/utils/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/utils/instance_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/utils/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-11 11:53:45.000000 vectice-23.2.7.1/src/vectice/utils/vectice_ids_regex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:53:58.619463 vectice-23.2.7.1/src/vectice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-11 11:53:58.000000 vectice-23.2.7.1/src/vectice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-11 11:53:58.000000 vectice-23.2.7.1/src/vectice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:53:58.000000 vectice-23.2.7.1/src/vectice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-11 11:53:58.000000 vectice-23.2.7.1/src/vectice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 11:53:58.000000 vectice-23.2.7.1/src/vectice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:05:24.000000 vectice-23.2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 12:05:15.000000 vectice-23.2.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-27 12:05:24.000000 vectice-23.2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-27 12:05:15.000000 vectice-23.2.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-27 12:05:15.000000 vectice-23.2.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-27 12:05:24.000000 vectice-23.2.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-27 12:05:15.000000 vectice-23.2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice/
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19549 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/gql_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/gql_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/gql_code_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/gql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/gql_entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/gql_feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/gql_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/gql_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/gql_user_workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12727 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/http_error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice/api/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/artifact_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/dataset_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/dataset_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/model_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/model_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/model_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/organization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/paged_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/public_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/user_and_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/user_declared_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21946 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/attachment_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14230 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/git_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice/models/representation/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/representation/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/representation/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/representation/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/representation/model_version_representation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice/models/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/bigquery_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11018 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/databricks_table_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/gcs_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/column_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/dataframe_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/db_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/df_wrapper_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/extra_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/s3_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29620 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/step_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/step_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/step_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/step_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/step_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/utils/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/utils/automatic_link_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/utils/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/utils/instance_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/utils/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/utils/vectice_ids_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `vectice-23.2.7.1/LICENSE` & `vectice-23.2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/PKG-INFO` & `vectice-23.2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 23.2.7.1
+Version: 23.2.8.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
```

### Comparing `vectice-23.2.7.1/setup.py` & `vectice-23.2.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,19 +72,21 @@
             "dslr[psycopg2-binary]",
             "mock>=1.0.1",
             "numpy",
             "pytest",
             "pytest-randomly",
             "coverage",
             "pytest-cov",
-            "scikit-learn<=0.24.2",
+            "scikit-learn",
             "testcontainers",
             "testbook",
             "db-dtypes>=1.1.1",
             "pyspark",
+            "Cython<3.0",
+            "pyyaml==5.3.1",
         ],
         "gcs": ["google-cloud-storage>=1.17.0", "google-cloud-bigquery"],
         "s3": ["boto3"],
     },
     classifiers=[
         "Topic :: Internet",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
```

### Comparing `vectice-23.2.7.1/src/vectice/__init__.py` & `vectice-23.2.8.0/src/vectice/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,17 +14,22 @@
 - the [Iteration][vectice.models.Iteration] class
 - the [Step][vectice.models.Step] class
 - the [Model][vectice.Model] class
 """
 
 from __future__ import annotations
 
+import sys
 import warnings
 
 warnings.filterwarnings("ignore", ".*PYARROW_IGNORE_TIMEZONE")
+if sys.version_info < (3, 8):
+    print(
+        "ImportWarning: Python 3.7 is no longer maintained by the community. Upgrade to Python 3.8 or higher to ensure full compatibility with Vectice and access to its complete features."
+    )
 
 from vectice import api, models
 from vectice.__version__ import __version__
 from vectice.connection import Connection
 from vectice.models.dataset import Dataset
 from vectice.models.git_version import CodeSource
 from vectice.models.model import Metric, Model, Property
```

### Comparing `vectice-23.2.7.1/src/vectice/api/__init__.py` & `vectice-23.2.8.0/src/vectice/api/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from __future__ import annotations
 
 from vectice.api import json
 from vectice.api.client import Client
 from vectice.api.http_error_handlers import InvalidReferenceError, MissingReferenceError
 from vectice.api.iteration import IterationApi
-from vectice.api.last_assets import LastAssetApi
 from vectice.api.phase import PhaseApi
 from vectice.api.step import StepApi
 from vectice.api.workspace import WorkspaceApi
 
 __all__ = [
     "MissingReferenceError",
     "InvalidReferenceError",
     "Client",
     "WorkspaceApi",
     "json",
     "PhaseApi",
     "StepApi",
     "IterationApi",
-    "LastAssetApi",
 ]
```

### Comparing `vectice-23.2.7.1/src/vectice/api/_auth.py` & `vectice-23.2.8.0/src/vectice/api/_auth.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/attachment.py` & `vectice-23.2.8.0/src/vectice/api/attachment.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/client.py` & `vectice-23.2.8.0/src/vectice/api/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 from vectice.api.json.dataset_version import DatasetVersionOutput
 from vectice.api.json.dataset_version_representation import DatasetVersionRepresentationOutput
 from vectice.api.json.iteration import IterationStatus
 from vectice.api.json.metric import MetricInput
 from vectice.api.json.model_representation import ModelRepresentationOutput
 from vectice.api.json.model_version_representation import ModelVersionRepresentationOutput
 from vectice.api.json.organization_config import OrgConfigOutput
-from vectice.api.last_assets import LastAssetApi
 from vectice.api.phase import PhaseApi
 from vectice.api.project import ProjectApi
 from vectice.api.step import StepApi
 from vectice.api.version import VersionApi
 from vectice.api.workspace import WorkspaceApi
 from vectice.models.dataset import Dataset
 from vectice.models.representation.dataset_version_representation import DatasetVersionRepresentation
@@ -439,17 +438,14 @@
             framework=model.library,
             codeVersionId=code_version_id,
         )
         return GqlModelApi(self._gql_client, self.auth).register_model(
             model_register_input, project_id, phase_id, iteration_id
         )
 
-    def get_last_assets(self, target_types: list[str], page):
-        return LastAssetApi(self._gql_client, self.auth).get_last_assets(target_types, page)
-
     def get_user_and_default_workspace(self):
         return UserAndDefaultWorkspaceApi(self._gql_client, self.auth).get_user_and_default_workspace()
 
     def create_code_gql(self, project_id: str, code: CodeInput):
         return GqlCodeApi(self._gql_client, self.auth).create_code(project_id, code)
 
     def create_code_version_gql(self, code_id: int, code_version: CodeVersionCreateBody):
```

### Comparing `vectice-23.2.7.1/src/vectice/api/gql_api.py` & `vectice-23.2.8.0/src/vectice/api/gql_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/gql_code.py` & `vectice-23.2.8.0/src/vectice/api/gql_code.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/gql_code_version.py` & `vectice-23.2.8.0/src/vectice/api/gql_code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/gql_dataset.py` & `vectice-23.2.8.0/src/vectice/api/gql_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/gql_entity_file.py` & `vectice-23.2.8.0/src/vectice/api/gql_entity_file.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/gql_feature_flag.py` & `vectice-23.2.8.0/src/vectice/api/gql_feature_flag.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/gql_model.py` & `vectice-23.2.8.0/src/vectice/api/gql_model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/gql_organization.py` & `vectice-23.2.8.0/src/vectice/api/gql_organization.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/gql_user_workspace_api.py` & `vectice-23.2.8.0/src/vectice/api/gql_user_workspace_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/http_error.py` & `vectice-23.2.8.0/src/vectice/api/http_error.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/http_error_handlers.py` & `vectice-23.2.8.0/src/vectice/api/http_error_handlers.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/iteration.py` & `vectice-23.2.8.0/src/vectice/api/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/json/__init__.py` & `vectice-23.2.8.0/src/vectice/api/json/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/json/artifact_version.py` & `vectice-23.2.8.0/src/vectice/api/json/artifact_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/json/code.py` & `vectice-23.2.8.0/src/vectice/api/json/code.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/json/code_version.py` & `vectice-23.2.8.0/src/vectice/api/json/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/json/dataset_register.py` & `vectice-23.2.8.0/src/vectice/api/json/dataset_register.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/json/dataset_representation.py` & `vectice-23.2.8.0/src/vectice/api/json/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/json/dataset_version.py` & `vectice-23.2.8.0/src/vectice/api/json/dataset_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/json/dataset_version_representation.py` & `vectice-23.2.8.0/src/vectice/api/json/dataset_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/json/files_metadata.py` & `vectice-23.2.8.0/src/vectice/api/json/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/json/iteration.py` & `vectice-23.2.8.0/src/vectice/api/json/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/json/last_assets.py` & `vectice-23.2.8.0/src/vectice/api/json/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/json/metric.py` & `vectice-23.2.8.0/src/vectice/api/json/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/json/model.py` & `vectice-23.2.8.0/src/vectice/api/json/model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/json/model_register.py` & `vectice-23.2.8.0/src/vectice/api/json/model_register.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/json/model_representation.py` & `vectice-23.2.8.0/src/vectice/api/json/model_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/json/model_version.py` & `vectice-23.2.8.0/src/vectice/api/json/model_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/json/model_version_representation.py` & `vectice-23.2.8.0/src/vectice/api/json/model_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/json/paged_response.py` & `vectice-23.2.8.0/src/vectice/api/json/paged_response.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/json/phase.py` & `vectice-23.2.8.0/src/vectice/api/json/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/json/project.py` & `vectice-23.2.8.0/src/vectice/api/json/project.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/json/property.py` & `vectice-23.2.8.0/src/vectice/api/json/property.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/json/public_config.py` & `vectice-23.2.8.0/src/vectice/api/json/public_config.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/json/step.py` & `vectice-23.2.8.0/src/vectice/api/json/step.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/json/workspace.py` & `vectice-23.2.8.0/src/vectice/api/json/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/phase.py` & `vectice-23.2.8.0/src/vectice/api/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/project.py` & `vectice-23.2.8.0/src/vectice/api/project.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/rest_api.py` & `vectice-23.2.8.0/src/vectice/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/step.py` & `vectice-23.2.8.0/src/vectice/api/step.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/version.py` & `vectice-23.2.8.0/src/vectice/api/version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/api/workspace.py` & `vectice-23.2.8.0/src/vectice/api/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/connection.py` & `vectice-23.2.8.0/src/vectice/connection.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/__init__.py` & `vectice-23.2.8.0/src/vectice/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/attachment_container.py` & `vectice-23.2.8.0/src/vectice/models/attachment_container.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/dataset.py` & `vectice-23.2.8.0/src/vectice/models/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from vectice.models.property import Property
 from vectice.models.representation.dataset_representation import DatasetRepresentation
 from vectice.models.representation.dataset_version_representation import DatasetVersionRepresentation
 from vectice.models.resource.base import Resource
 from vectice.models.resource.bigquery_resource import BigQueryResource
 from vectice.models.resource.databricks_table_resource import DatabricksTableResource
 from vectice.models.resource.metadata.base import DatasetSourceUsage, DatasetType
+from vectice.utils.common_utils import format_attachments
 
 _logger = logging.getLogger(__name__)
 
 
 TBaseDerivedFrom = Union[str, DatasetRepresentation, DatasetVersionRepresentation]
 
 
@@ -38,15 +39,15 @@
         self._resource = resource
         self._training_resource = training_resource
         self._testing_resource = testing_resource
         self._validation_resource = validation_resource
         self._derived_from = _get_derived_from(derived_from)
         self._latest_version_id: str | None = None
         self._properties = self._format_properties(properties) if properties else None
-        self._attachments = self._format_attachments(attachments) if attachments else None
+        self._attachments = format_attachments(attachments) if attachments else None
 
         if self._type is DatasetType.MODELING:
             if self._training_resource is None or self._testing_resource is None:
                 raise ValueError("You cannot create a modeling dataset without both training and testing sets")
 
             self._training_resource.usage = DatasetSourceUsage.TRAINING
             self._testing_resource.usage = DatasetSourceUsage.TESTING
@@ -309,25 +310,21 @@
     @attachments.setter
     def attachments(self, attachments: list[str] | str):
         """Attach a file or files to the dataset.
 
         Parameters:
             attachments: The filename or filenames of the file or set of files to attach to the dataset.
         """
-        self._attachments = self._format_attachments(attachments)
+        self._attachments = format_attachments(attachments)
 
     @staticmethod
     def _check_key_duplicates(key_list: list[str]):
         if len(key_list) != len(set(key_list)):
             raise ValueError("Duplicate keys are not allowed.")
 
-    @staticmethod
-    def _format_attachments(attachments: str | list[str]) -> list[str]:
-        return [attachment for attachment in set(attachments)] if isinstance(attachments, list) else [attachments]
-
     def _format_properties(self, properties: dict[str, str | int] | list[Property] | Property | None) -> list[Property]:
         if properties is None:
             return []
         if isinstance(properties, Property):
             return [properties]
         if isinstance(properties, list):
             properties = self._remove_incorrect_properties(properties)
```

### Comparing `vectice-23.2.7.1/src/vectice/models/git_version.py` & `vectice-23.2.8.0/src/vectice/models/git_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 from __future__ import annotations
 
 import logging
 import os
-from typing import TYPE_CHECKING, Any
-
-from git import GitError
-from git.repo import Repo
+from typing import TYPE_CHECKING
 
 import vectice
 from vectice.api.json.code import CodeInput
 from vectice.api.json.code_version import CodeVersionCreateBody, GitVersion
 from vectice.utils.common_utils import hide_logs
 
 if TYPE_CHECKING:
     from logging import Logger
 
     from git.diff import Diff
+    from git.repo import Repo
 
     from vectice.api.client import Client
     from vectice.api.json.user_declared_version import UserDeclaredVersion
 
 
 _logger = logging.getLogger(__name__)
 
 
 class CodeSource:
     """Capture the current git commit."""
 
     def __init__(self, repository: Repo, user_declared_version: UserDeclaredVersion | None = None):
-        self._repository: Repo = repository
+        self._repository = repository
         self._git_version: GitVersion | None = _extract_git_version(repository)
         self._user_declared_version: UserDeclaredVersion | None = user_declared_version
 
     @property
-    def repository(self) -> Any:
+    def repository(self) -> Repo:
         return self._repository
 
     @property
     def user_declared_version(self) -> UserDeclaredVersion | None:
         return self._user_declared_version
 
     @property
@@ -110,29 +108,39 @@
             file_names.append(file.a_path)
     if diff_outputs:
         client.create_code_attachments(diff_outputs, code_version_id, project_id)
     if file_names:
         _logger.info(f"Code captured the following changed files; {', '.join(file_names)}")
 
 
-def _look_for_git_repository(repo_path=".") -> Any | None:
+def _look_for_git_repository(repo_path=".") -> Repo | None:
+    def _log_error(error: str):
+        _logger.debug(
+            f"Code capture failed: {error.__class__.__name__}: {error}. "
+            "Make sure the current directory is a valid Git repository (non-bare, non worktree) "
+            "and its permissions allow the current user to access it."
+        )
+
+    try:
+        from git import GitError
+    except ImportError as error:
+        _log_error(str(error))
+        return None
+
     try:
         repo_path = os.path.abspath(repo_path)
     except OSError:
         _logger.debug(f"Code capture failed: the directory '{repo_path}' cannot be accessed by the system")
         return None
     try:
+        from git.repo import Repo
+
         return Repo(repo_path, search_parent_directories=True)
     except GitError as error:
-        error_message = str(error) or repo_path
-        _logger.debug(
-            f"Code capture failed: {error.__class__.__name__}: {error_message}. "
-            "Make sure the current directory is a valid Git repository (non-bare, non worktree) "
-            "and its permissions allow the current user to access it."
-        )
+        _log_error(str(error) or repo_path)
         return None
 
 
 def _check_for_code(client: Client, project_id: str, _logger: Logger) -> int | None:
     code_version_id = None
 
     if vectice.code_capture:
```

### Comparing `vectice-23.2.7.1/src/vectice/models/iteration.py` & `vectice-23.2.8.0/src/vectice/models/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/metric.py` & `vectice-23.2.8.0/src/vectice/models/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/model.py` & `vectice-23.2.8.0/src/vectice/models/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 import pickle  # nosec
 from typing import Any
 
 from vectice.models import Metric, Property
 from vectice.models.dataset import TDerivedFrom, _get_derived_from
+from vectice.utils.common_utils import format_attachments
 
 _logger = logging.getLogger(__name__)
 
 
 class Model:
     """Represent a wrapped model.
 
@@ -46,15 +47,15 @@
             derived_from: List of dataset (or version ids) to link as lineage.
         """
         self._library = library
         self._technique = technique
         self._name = name if name else self._generate_name()
         self._metrics = self._format_metrics(metrics) if metrics else None
         self._properties = self._format_properties(properties) if properties else None
-        self._attachments = self._format_attachments(attachments) if attachments else None
+        self._attachments = format_attachments(attachments) if attachments else None
         self._predictor = pickle.dumps(predictor)  # nosec
         self._derived_from = _get_derived_from(derived_from)
 
     def __repr__(self):
         return (
             f"Model(name='{self.name}', library='{self.library}', technique='{self.technique}', "
             f"metrics={self.metrics}, properties={self.properties}, attachments={self.attachments})"
@@ -66,15 +67,15 @@
 
         Returns:
             The model's name.
         """
         return self._name
 
     @name.setter
-    def name(self, name):
+    def name(self, name: str):
         """Set the model's name.
 
         Parameters:
             name: The name of the model.
         """
         self._name = name
 
@@ -107,15 +108,15 @@
 
         Returns:
             The name of the library used to generate the model.
         """
         return self._library
 
     @library.setter
-    def library(self, library):
+    def library(self, library: str):
         """Set the name of the library used to create the model.
 
         Parameters:
             library: The name of the library used to create the model.
         """
         self._library = library
 
@@ -125,15 +126,15 @@
 
         Returns:
             The name of the modeling technique used to learn the model.
         """
         return self._technique
 
     @technique.setter
-    def technique(self, technique):
+    def technique(self, technique: str):
         """Set the name of the modeling technique used to learn the model.
 
         Parameters:
             technique: The modeling technique used.
         """
         self._technique = technique
 
@@ -187,15 +188,15 @@
     @attachments.setter
     def attachments(self, attachments: list[str] | str):
         """Attach a file or files to the model.
 
         Parameters:
             attachments: The filename or filenames of the file or set of files to attach to the model.
         """
-        self._attachments = self._format_attachments(attachments)
+        self._attachments = format_attachments(attachments)
 
     @property
     def derived_from(self) -> list[str]:
         """The datasets from which this model is derived.
 
         Returns:
             The datasets from which this model is derived.
@@ -229,18 +230,14 @@
     def _remove_incorrect_metrics(metrics: list[Metric]) -> list[Metric]:
         for metric in metrics:
             if not isinstance(metric, Metric):
                 logging.warning(f"Incorrect metric '{metric}'. Please check metric type.")
                 metrics.remove(metric)
         return metrics
 
-    @staticmethod
-    def _format_attachments(attachments: str | list[str]) -> list[str]:
-        return [attachment for attachment in set(attachments)] if isinstance(attachments, list) else [attachments]
-
     def _format_properties(
         self, properties: dict[str, str] | dict[str, int] | list[Property] | Property | None
     ) -> list[Property]:
         if properties is None:
             return []
         if isinstance(properties, Property):
             return [properties]
```

### Comparing `vectice-23.2.7.1/src/vectice/models/phase.py` & `vectice-23.2.8.0/src/vectice/models/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/project.py` & `vectice-23.2.8.0/src/vectice/models/project.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/property.py` & `vectice-23.2.8.0/src/vectice/models/property.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/representation/dataset_representation.py` & `vectice-23.2.8.0/src/vectice/models/representation/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/resource/__init__.py` & `vectice-23.2.8.0/src/vectice/models/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/resource/base.py` & `vectice-23.2.8.0/src/vectice/models/resource/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
             The resource's metadata.
         """
         if self._metadata is None:
             self._metadata = self._build_metadata()
         return self._metadata
 
     @metadata.setter
-    def metadata(self, value):
+    def metadata(self, value: Metadata):
         """Set the resource's metadata.
 
         Parameters:
             value: The metadata to set.
         """
         self._metadata = value
```

### Comparing `vectice-23.2.7.1/src/vectice/models/resource/bigquery_resource.py` & `vectice-23.2.8.0/src/vectice/models/resource/bigquery_resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,57 +75,53 @@
             return self._fetch_dataset_data(index=index, path=path)
 
         raise ValueError(f"Path '{path}' is invalid, please reference either a dataset or a table.")
 
     def _fetch_table_data(self, index: int, path: str) -> dict[str, tuple[Table | None, DataFrameType | None]]:
         from google.api_core.exceptions import Forbidden
 
-        table_name = path.partition(".")[-1]
-
         dataframe = self._dataframes[index] if self._dataframes is not None and len(self._dataframes) > index else None
         if self.bq_client is None:
-            return {table_name: (None, dataframe)}
+            return {path: (None, dataframe)}
 
         tb = None
         try:
             tb = self.bq_client.get_table(table=path)
         except Forbidden:
-            _logger.warning(f"Failed to fetch data information for table {table_name}")
+            _logger.warning(f"Failed to fetch data information for table {path}")
             pass
 
-        return {table_name: (tb, dataframe)}
+        return {path: (tb, dataframe)}
 
     def _fetch_dataset_data(
         self, index: int, path: str
     ) -> tuple[dict[str, tuple[Table | None, DataFrameType | None]], int]:
         from google.api_core.exceptions import Forbidden
 
         df_index = 0
         tables_dict: dict[str, tuple[Table | None, DataFrameType | None]] = {}
-        dataset = path.partition(".")[-1]
         if self.bq_client is None:
             new_index = df_index + index
             dataframe = (
                 self._dataframes[new_index]
                 if self._dataframes is not None and len(self._dataframes) > new_index
                 else None
             )
-            return {dataset: (None, dataframe)}, 1
+            return {path: (None, dataframe)}, 1
         try:
             tables_data: list[Table] = self.bq_client.list_tables(dataset=path)  # type: ignore[assignment]
             tables = sorted(tables_data, key=lambda table: table.table_id.lower())
             for table in tables:
                 new_index = df_index + index
                 dataframe = (
                     self._dataframes[new_index]
                     if self._dataframes is not None and len(self._dataframes) > new_index
                     else None
                 )
-                dataset = path.partition(".")[-1]
-                table_name = f"{dataset}.{table.table_id}"
+                table_name = f"{path}.{table.table_id}"
                 try:
                     tables_dict[table_name] = (
                         self.bq_client.get_table(table=f"{path}.{table.table_id}"),
                         dataframe,
                     )
                 except Exception:
                     _logger.warning(f"Failed to fetch data information for table {table_name}")
@@ -137,15 +133,15 @@
         except Forbidden:
             _logger.warning(f"Failed to list tables for dataset {path}")
             return {}, 0
 
     def _build_metadata(self) -> DBMetadata:
         tables_metadata: dict[str, tuple[Table | None, DataFrameType | None]] = self.data
         dbs: list[MetadataDB] = []
-        for table_name, [table_metadata, dataframe] in tables_metadata.items():
+        for table_path, [table_metadata, dataframe] in tables_metadata.items():
             columns: list[DBColumn] | None = None
             size = None
             rows_number = None
             updated_date = None
             created_date = None
             if table_metadata is not None:
                 columns = []
@@ -165,22 +161,23 @@
                             is_private_key=False,
                             is_foreign_key=False,
                         )
                     )
 
             dbs.append(
                 MetadataDB(
-                    name=table_name,
+                    name=table_path.partition(".")[-1],
                     rows_number=rows_number,
                     size=size,
                     columns=columns,
                     created_date=created_date,
                     updated_date=updated_date,
+                    uri=table_path,
                     dataframe=dataframe,
-                    display_name=table_name.rpartition(".")[-1],
+                    display_name=table_path.rpartition(".")[-1],
                     capture_schema_only=self.capture_schema_only,
                 )
             )
 
         metadata_size = None
         for db in dbs:
             if db.size is not None:
```

### Comparing `vectice-23.2.7.1/src/vectice/models/resource/databricks_table_resource.py` & `vectice-23.2.8.0/src/vectice/models/resource/databricks_table_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,22 +113,21 @@
 
         if schema is None:
             schema = self._get_schema(self._spark_client, has_version, has_at, path, table_path)
 
         table_format = detail["format"]
         extra_metadata: list[ExtraMetadata] = [
             ExtraMetadata(key="format", value=table_format, display_name="Format"),
-            ExtraMetadata(key="path", value=location, display_name="Path"),
         ]
 
         information = self._get_table_information(self._spark_client)
         if "Type" in information:
             extra_metadata.append(ExtraMetadata(key="type", value=information["Type"], display_name="Type"))
         if detail["sizeInBytes"] is None and "Statistics" in information and has_at is None and has_version is None:
-            match_bytes = re.search(r"([0-9]+)( bytes)", information["Statistics"])
+            match_bytes = re.search(r"([0-9]{1,15})( bytes)", information["Statistics"])
             if match_bytes is not None:
                 detail["sizeInBytes"] = int(match_bytes.group(1))
 
         if table_format == "delta":
             extra_metadata.extend(
                 self._get_delta_table_history_extra_metadata(self._spark_client, has_version, has_at, path)
             )
@@ -212,20 +211,22 @@
         dbs: list[MetadataDB] = []
         for table_name, [table_metadata, dataframe] in tables_metadata.items():
             columns: list[DBColumn] | None = None
             size = None
             updated_date = None
             created_date = None
             rows_number = None
+            uri = None
             if table_metadata is not None and self._spark_client is not None:
                 columns = []
                 detail = table_metadata["detail"]
                 created_at = detail["createdAt"]
                 last_modified = detail["lastModified"]
                 size = detail["sizeInBytes"]
+                uri = detail["location"]
                 if "rowsNumber" in detail:
                     rows_number = detail["rowsNumber"]
 
                 def get_iso_format_from_str_or_date(date_time):
                     if date_time is not None:
                         if isinstance(date_time, str):
                             return parser.parse(date_time).isoformat()
@@ -248,14 +249,15 @@
                 MetadataDB(
                     name=table_name,
                     size=size,
                     rows_number=rows_number,
                     columns=columns,
                     created_date=created_date,
                     updated_date=updated_date,
+                    uri=uri,
                     dataframe=dataframe,
                     extra_metadata=table_metadata["extra_metadata"] if table_metadata is not None else None,
                     display_name=table_name.rpartition("/")[-1],
                     capture_schema_only=self.capture_schema_only,
                 )
             )
```

### Comparing `vectice-23.2.7.1/src/vectice/models/resource/description.py` & `vectice-23.2.8.0/src/vectice/models/resource/description.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/resource/file_resource.py` & `vectice-23.2.8.0/src/vectice/models/resource/file_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/resource/gcs_resource.py` & `vectice-23.2.8.0/src/vectice/models/resource/gcs_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/resource/metadata/__init__.py` & `vectice-23.2.8.0/src/vectice/models/resource/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/resource/metadata/base.py` & `vectice-23.2.8.0/src/vectice/models/resource/metadata/base.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/resource/metadata/column_metadata.py` & `vectice-23.2.8.0/src/vectice/models/resource/metadata/column_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/resource/metadata/dataframe_config.py` & `vectice-23.2.8.0/src/vectice/models/resource/metadata/dataframe_config.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/resource/metadata/db_metadata.py` & `vectice-23.2.8.0/src/vectice/models/resource/metadata/db_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,40 +47,43 @@
         self,
         name: str,
         columns: list[DBColumn] | None,
         rows_number: int | None = None,
         size: int | None = None,
         updated_date: str | None = None,
         created_date: str | None = None,
+        uri: str | None = None,
         dataframe: DataFrameType | None = None,
         extra_metadata: list[ExtraMetadata] | None = None,
         display_name: str | None = None,
         capture_schema_only: bool = False,
     ):
         """Initialize a MetadataDB instance.
 
         Parameters:
             name: The name of the table.
             columns: The columns that compose the table.
             rows_number: The number of row of the table.
             size: The size of the table.
             updated_date: The date of last update of the table.
             created_date: The creation date of the table.
+            uri: The uri of the table.
             dataframe (Optional): A dataframe allowing vectice to optionally compute more metadata about this resource such as columns stats, size, rows number and column numbers. (Support Pandas and Spark)
             extra_metadata (Optional): Extra metadata to be captured.
             display_name (Optional): Name that will be shown in the UI.
             capture_schema_only (Optional): A boolean parameter indicating whether to capture only the schema or both the schema and column statistics of the dataframes.
 
         """
         super().__init__(
             name=name,
             size=size,
             columns=list(columns) if columns is not None else None,
             updated_date=updated_date,
             created_date=created_date,
+            uri=uri,
             dataframe=dataframe,
             extra_metadata=extra_metadata,
             display_name=display_name,
             capture_schema_only=capture_schema_only,
         )
         self.rows_number = rows_number
```

### Comparing `vectice-23.2.7.1/src/vectice/models/resource/metadata/df_wrapper_pandas.py` & `vectice-23.2.8.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py` & `vectice-23.2.8.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,20 +56,15 @@
 
         return False
 
     def capture_column_schema(self) -> list[Column]:
         column_cat: ColumnCategoryType | None = None
         list_schema: list[Column] = []
 
-        for idx, (column, column_type) in enumerate(self.dataframe.dtypes.items()):
-            if idx >= MAX_COLUMNS_CAPTURE_STATS:
-                _logger.warning(
-                    f"Statistics are only captured for the first {MAX_COLUMNS_CAPTURE_STATS} columns of your dataframe."
-                )
-                break
+        for column, column_type in self.dataframe.dtypes.items():
             column = str(column)
             if api.types.is_bool_dtype(column_type):
                 column_cat = ColumnCategoryType.BOOLEAN
                 dtype = str(column_type)
             elif api.types.is_numeric_dtype(column_type):
                 column_cat = ColumnCategoryType.NUMERICAL
                 dtype = str(column_type)
@@ -87,31 +82,33 @@
                 Column(
                     name=column,
                     data_type=dtype if dtype != "object" else "string",
                     stats=None,
                     category_type=column_cat,
                 )
             )
-
         return list_schema
 
     def capture_column_statistics(self, list_col_schema: list[Column]) -> list[Column]:
         columns: list[Column] = []
         stat: TextStat | BooleanStat | NumericalStat | DateStat | None = None
-        for col in list_col_schema:
+        for idx, col in enumerate(list_col_schema):
+            if idx == MAX_COLUMNS_CAPTURE_STATS:
+                _logger.warning(
+                    f"Statistics are only captured for the first {MAX_COLUMNS_CAPTURE_STATS} columns of your dataframe."
+                )
             column = self.dataframe[col.name]
             col_type = col.category_type
-            if col_type is not None:
+            if col_type is not None and idx < MAX_COLUMNS_CAPTURE_STATS:
                 stat = self.__capture_pandas_stats__(column, col_type)
             else:
                 stat = None
             col.stats = stat
 
             columns.append(col)
-
         return columns
 
     def __capture_pandas_stats__(
         self, series: Series, col_type: ColumnCategoryType
     ) -> TextStat | BooleanStat | NumericalStat | DateStat | None:
         if col_type.value == "BOOLEAN":
             return self.__compute_boolean_column_statistics__(series)
```

### Comparing `vectice-23.2.7.1/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py` & `vectice-23.2.8.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/resource/metadata/df_wrapper_resource.py` & `vectice-23.2.8.0/src/vectice/models/resource/metadata/df_wrapper_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class DataFrameWrapper(ABC, Generic[T]):
     """Base class for dataframe wrappers.
 
     Use DataFrameWrapper subclasses to assign wrap DataFrames to generate statistics  The
     Vectice library supports a handful of common cases.  Additional
     cases are generally easy to supply by deriving from this base
     class.  In particular, subclasses must override this class'
-    abstact methods (`capture_columns()`, `get_size()`).
+    abstact methods (`capture_column_statistics()`, `capture_column_schema()`, `get_size()`).
     """
 
     def __init__(self, dataframe: T):
         self.dataframe = dataframe
         self.rows: int = 0
 
     @abstractmethod
```

### Comparing `vectice-23.2.7.1/src/vectice/models/resource/metadata/df_wrapper_spark_df.py` & `vectice-23.2.8.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,20 +45,15 @@
 
         return Size(rows=self.rows, columns=self.columns_numbers)
 
     def capture_column_schema(self) -> list[Column]:
         column_cat: ColumnCategoryType | None = None
         list_schema: list[Column] = []
 
-        for idx, (column, column_type) in enumerate(self.dataframe.dtypes):
-            if idx >= MAX_COLUMNS_CAPTURE_STATS:
-                _logger.warning(
-                    f"Statistics are only captured for the first {MAX_COLUMNS_CAPTURE_STATS} columns of your dataframe."
-                )
-                break
+        for column, column_type in self.dataframe.dtypes:
             column = str(column)
             if column_type in ["tinyint", "smallint", "int", "bigint", "float", "double"] or "decimal" in column_type:
                 column_cat = ColumnCategoryType.NUMERICAL
                 dtype = str(column_type)
             elif column_type == "date" or column_type == "timestamp":
                 column_cat = ColumnCategoryType.DATE
                 dtype = str(column_type)
@@ -86,18 +81,21 @@
     def capture_column_statistics(self, list_col_schema: list[Column]) -> list[Column]:
         columns: list[Column] = []
         stat: BooleanStat | NumericalStat | TextStat | DateStat | None = None
         result: Dict[str, BooleanStat | NumericalStat | TextStat | DateStat] = {}
 
         column_split_by_type = self.__get_list_column_split_by_type__(list_col_schema)
         result_numerical, result_str, result_bool, result_date = self.__compute_spark_stats__(column_split_by_type)
-
         result = {**result_numerical, **result_str, **result_bool, **result_date}
-        for col in list_col_schema:
-            if col.name in result:
+        for idx, col in enumerate(list_col_schema):
+            if idx == MAX_COLUMNS_CAPTURE_STATS:
+                _logger.warning(
+                    f"Statistics are only captured for the first {MAX_COLUMNS_CAPTURE_STATS} columns of your dataframe."
+                )
+            if col.name in result and idx < MAX_COLUMNS_CAPTURE_STATS:
                 stat = result[col.name]
             else:
                 stat = None
 
             col.stats = stat
             columns.append(col)
         return columns
@@ -123,15 +121,17 @@
         if len(column_values["date"]) > 0:
             result_date = self.__compute_date_column_statistics__(self.dataframe.select(column_values["date"]))
         return result_numerical, result_str, result_bool, result_date
 
     def __get_list_column_split_by_type__(self, list_col_schema) -> Dict[str, list]:
         column_split_by_type: Dict[str, list] = {"numerical": [], "string": [], "boolean": [], "date": []}
 
-        for col in list_col_schema:
+        for idx, col in enumerate(list_col_schema):
+            if idx >= MAX_COLUMNS_CAPTURE_STATS:
+                break
             column_name = col.name
             if col.category_type == ColumnCategoryType.NUMERICAL:
                 column_split_by_type["numerical"].append(column_name)
             elif col.category_type == ColumnCategoryType.DATE:
                 column_split_by_type["date"].append(column_name)
             elif col.category_type == ColumnCategoryType.BOOLEAN:
                 column_split_by_type["boolean"].append(column_name)
```

### Comparing `vectice-23.2.7.1/src/vectice/models/resource/metadata/files_metadata.py` & `vectice-23.2.8.0/src/vectice/models/resource/metadata/files_metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,25 +79,24 @@
         """
         super().__init__(
             name=name,
             size=size,
             columns=columns,
             created_date=created_date,
             updated_date=updated_date,
+            uri=uri,
             dataframe=dataframe,
             extra_metadata=extra_metadata,
             display_name=display_name,
             capture_schema_only=capture_schema_only,
         )
         self.fingerprint = fingerprint
-        self.uri = uri
         self.content_type = content_type
 
     def asdict(self) -> dict:
         return {
             **super().asdict(),
             "fingerprint": self.fingerprint,
             "createdDate": self.created_date,
-            "uri": self.uri,
             "mimeType": self.content_type,
             "filename": self.display_name,
         }
```

### Comparing `vectice-23.2.7.1/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py` & `vectice-23.2.8.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/resource/metadata/source.py` & `vectice-23.2.8.0/src/vectice/models/resource/metadata/source.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,38 +21,41 @@
     def __init__(
         self,
         name: str,
         size: int | None = None,
         columns: list[Column] | None = None,
         updated_date: str | None = None,
         created_date: str | None = None,
+        uri: str | None = None,
         dataframe: DataFrameType | None = None,
         extra_metadata: list[ExtraMetadata] | None = None,
         display_name: str | None = None,
         capture_schema_only: bool = False,
     ):
         """Initialize a MetadataDB instance.
 
         Parameters:
             name: The name of the source.
             size: The size of the source.
             columns: The columns that compose the source.
             updated_date: The date of last update of the source.
             created_date: The date of creation of the source.
+            uri: The uri of the source.
             dataframe (Optional): A dataframe allowing vectice to optionally compute more metadata about this resource such as columns stats, size, rows number and column numbers. (Support Pandas and Spark)
             extra_metadata (Optional): Extra metadata to be captured.
             capture_schema_only (Optional): A boolean parameter indicating whether to capture only the schema or both the schema and column statistics of the dataframes.
 
         """
         self.name = name
         self.display_name = display_name
         self.size = size
         self.columns = columns
         self.created_date = created_date
         self.updated_date = updated_date
+        self.uri = uri
         self.extra_metadata = extra_metadata
         self._dataframe = dataframe
         self._wrapper: PandasDFWrapper | PysparkPandasDFWrapper | SparkDFWrapper | None = None
         self._settings = MetadataSettings()
         self.capture_schema_only = capture_schema_only
 
         if isinstance(self._dataframe, PandasDF):
@@ -66,15 +69,15 @@
                 from pyspark.pandas.frame import DataFrame as PysparkPandasDF
                 from pyspark.sql.dataframe import DataFrame as SparkDF
 
                 if isinstance(self._dataframe, SparkDF):
                     self._wrapper = SparkDFWrapper(self._dataframe)
                 elif isinstance(self._dataframe, PysparkPandasDF):
                     _logger.warning(
-                        "WARNING: Pandas on spark is not supported yet, pass a Pandas or a Spark DataFrame to get statistics."
+                        "WARNING: Pandas on spark DataFrame is not supported yet, pass a Pandas or a Spark DataFrame to get statistics."
                     )
             except ImportError:
                 pass
 
     def set_settings(self, settings: MetadataSettings):
         self._settings = settings
 
@@ -101,11 +104,12 @@
         exm = self.extra_metadata
         return {
             **size_info,
             "size": self.size,
             "name": self.name,
             "updatedDate": self.updated_date,
             "createdDate": self.created_date,
+            "uri": self.uri,
             "columns": columns_list_dict,
             "skippedStatistics": skipped_statistics,
             "extraMetadata": [metadata.to_dict() for metadata in exm] if exm is not None else None,  # type: ignore[attr-defined]
         }
```

### Comparing `vectice-23.2.7.1/src/vectice/models/resource/s3_resource.py` & `vectice-23.2.8.0/src/vectice/models/resource/s3_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/step.py` & `vectice-23.2.8.0/src/vectice/models/step.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/step_dataset.py` & `vectice-23.2.8.0/src/vectice/models/step_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/step_image.py` & `vectice-23.2.8.0/src/vectice/models/step_image.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/step_model.py` & `vectice-23.2.8.0/src/vectice/models/step_model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/step_number.py` & `vectice-23.2.8.0/src/vectice/models/step_number.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/step_string.py` & `vectice-23.2.8.0/src/vectice/models/step_string.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/models/workspace.py` & `vectice-23.2.8.0/src/vectice/models/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/utils/automatic_link_utils.py` & `vectice-23.2.8.0/src/vectice/utils/automatic_link_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/utils/common_utils.py` & `vectice-23.2.8.0/src/vectice/utils/common_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -163,7 +163,19 @@
     for key, value in input_dict.items():
         camel_case_key = re.sub(r"_([a-z])", lambda match: match.group(1).upper(), key)
         if isinstance(value, dict):
             value = _convert_keys_to_camel_case(value)
         camel_case_dict[camel_case_key] = value
 
     return camel_case_dict
+
+
+def format_attachments(attachments: str | list[str]) -> list[str]:
+    list_attachments = (
+        [attachment for attachment in set(attachments)] if isinstance(attachments, list) else [attachments]
+    )
+    for attachment in list_attachments:
+        if not isinstance(attachment, str):
+            raise ValueError(
+                f"Argument 'attachments' with type '{type(attachment)}' is invalid, only str are supported."
+            )
+    return list_attachments
```

### Comparing `vectice-23.2.7.1/src/vectice/utils/configuration.py` & `vectice-23.2.8.0/src/vectice/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/utils/deprecation.py` & `vectice-23.2.8.0/src/vectice/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/utils/last_assets.py` & `vectice-23.2.8.0/src/vectice/utils/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice/utils/logging_utils.py` & `vectice-23.2.8.0/src/vectice/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.7.1/src/vectice.egg-info/PKG-INFO` & `vectice-23.2.8.0/src/vectice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 23.2.7.1
+Version: 23.2.8.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
```

### Comparing `vectice-23.2.7.1/src/vectice.egg-info/SOURCES.txt` & `vectice-23.2.8.0/src/vectice.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 src/vectice/api/gql_model.py
 src/vectice/api/gql_organization.py
 src/vectice/api/gql_user_workspace_api.py
 src/vectice/api/http_error.py
 src/vectice/api/http_error_handlers.py
 src/vectice/api/iteration.py
 src/vectice/api/json_object.py
-src/vectice/api/last_assets.py
 src/vectice/api/phase.py
 src/vectice/api/project.py
 src/vectice/api/rest_api.py
 src/vectice/api/step.py
 src/vectice/api/version.py
 src/vectice/api/workspace.py
 src/vectice/api/json/__init__.py
```

### Comparing `vectice-23.2.7.1/src/vectice.egg-info/requires.txt` & `vectice-23.2.8.0/src/vectice.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -43,12 +43,14 @@
 dslr[psycopg2-binary]
 mock>=1.0.1
 numpy
 pytest
 pytest-randomly
 coverage
 pytest-cov
-scikit-learn<=0.24.2
+scikit-learn
 testcontainers
 testbook
 db-dtypes>=1.1.1
 pyspark
+Cython<3.0
+pyyaml==5.3.1
```

