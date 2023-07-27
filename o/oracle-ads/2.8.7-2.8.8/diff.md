# Comparing `tmp/oracle_ads-2.8.7.tar.gz` & `tmp/oracle_ads-2.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oracle_ads-2.8.7.tar", last modified: Fri Jun 23 00:13:08 2023, max compression
+gzip compressed data, was "oracle_ads-2.8.8.tar", last modified: Thu Jul 27 19:57:02 2023, max compression
```

## Comparing `oracle_ads-2.8.7.tar` & `oracle_ads-2.8.8.tar`

### file list

```diff
@@ -1,532 +1,536 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.688820 oracle_ads-2.8.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-06-23 00:13:08.688820 oracle_ads-2.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    50466 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/THIRD_PARTY_LICENSES.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.624813 oracle_ads-2.8.7/ads/
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/ads_version.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.624813 oracle_ads-2.8.7/ads/automl/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/automl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/automl/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    35984 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/automl/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.624813 oracle_ads-2.8.7/ads/bds/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/bds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/bds/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/bds/big_data_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.624813 oracle_ads-2.8.7/ads/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60039 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/catalog/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16462 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/catalog/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)    16091 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/catalog/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/catalog/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.628814 oracle_ads-2.8.7/ads/common/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.628814 oracle_ads-2.8.7/ads/common/artifact/
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/artifact/.model-ignore
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/artifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45326 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/card_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    20253 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.628814 oracle_ads-2.8.7/ads/common/decorator/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/decorator/argument_to_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/decorator/deprecate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/decorator/runtime_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/decorator/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/dsc_file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/extended_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.628814 oracle_ads-2.8.7/ads/common/function/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/function/fn_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/function/func_conf.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/ipython.py
--rw-r--r--   0 runner    (1001) docker     (123)    27269 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    72294 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/model_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/model_artifact_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    26571 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/model_export_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/model_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/object_storage_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/oci_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/oci_datascience.py
--rw-r--r--   0 runner    (1001) docker     (123)    42155 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/oci_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    37213 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/oci_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/oci_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    16565 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)    46073 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22306 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/common/word_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.628814 oracle_ads-2.8.7/ads/data_labeling/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/boundingbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/data_labeling_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.632814 oracle_ads-2.8.7/ads/data_labeling/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/interface/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/interface/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/interface/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.632814 oracle_ads-2.8.7/ads/data_labeling/loader/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/loader/file_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.632814 oracle_ads-2.8.7/ads/data_labeling/mixin/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/mixin/data_labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/ner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.632814 oracle_ads-2.8.7/ads/data_labeling/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/parser/dls_record_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/parser/export_metadata_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    17416 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/parser/export_record_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.632814 oracle_ads-2.8.7/ads/data_labeling/reader/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22145 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/reader/dataset_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/reader/dls_record_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/reader/export_record_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/reader/jsonl_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/reader/metadata_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/reader/record_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.632814 oracle_ads-2.8.7/ads/data_labeling/visualizer/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/visualizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15880 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/visualizer/image_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/data_labeling/visualizer/text_visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.632814 oracle_ads-2.8.7/ads/database/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/database/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.636814 oracle_ads-2.8.7/ads/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/classification_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17306 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/correlation_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/dask_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/dataframe_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    72309 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11935 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/dataset_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)    38574 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/dataset_with_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    37220 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/feature_engineering_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/forecasting_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/label_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.636814 oracle_ads-2.8.7/ads/dataset/mixin/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/mixin/dataset_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    26056 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)    12909 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/recommendation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22168 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/recommendation_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/regression_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    39503 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/sampled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/target.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dataset/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.636814 oracle_ads-2.8.7/ads/dbmixin/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dbmixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/dbmixin/db_pandas_accessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.636814 oracle_ads-2.8.7/ads/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/environment/ml_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.636814 oracle_ads-2.8.7/ads/evaluations/
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/evaluations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39617 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/evaluations/evaluation_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    53173 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/evaluations/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21279 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/evaluations/statistical_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.636814 oracle_ads-2.8.7/ads/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/experiments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.636814 oracle_ads-2.8.7/ads/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/explanations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/explanations/base_explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/explanations/explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    41704 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/explanations/mlx_global_explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/explanations/mlx_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/explanations/mlx_local_explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/explanations/mlx_whatif_explainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.640815 oracle_ads-2.8.7/ads/feature_engineering/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.640815 oracle_ads-2.8.7/ads/feature_engineering/accessor/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/accessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18403 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/accessor/dataframe_accessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.640815 oracle_ads-2.8.7/ads/feature_engineering/accessor/mixin/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/accessor/mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/accessor/mixin/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/accessor/mixin/eda_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/accessor/mixin/eda_mixin_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/accessor/mixin/feature_types_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/accessor/mixin/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/accessor/series_accessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.640815 oracle_ads-2.8.7/ads/feature_engineering/adsimage/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/adsimage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/adsimage/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/adsimage/image_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.640815 oracle_ads-2.8.7/ads/feature_engineering/adsimage/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/adsimage/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/adsimage/interface/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.640815 oracle_ads-2.8.7/ads/feature_engineering/adsstring/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/adsstring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.640815 oracle_ads-2.8.7/ads/feature_engineering/adsstring/oci_language/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/adsstring/oci_language/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.640815 oracle_ads-2.8.7/ads/feature_engineering/adsstring/string/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/adsstring/string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/data_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.640815 oracle_ads-2.8.7/ads/feature_engineering/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1600358 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/dataset/zip_code_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.652816 oracle_ads-2.8.7/ads/feature_engineering/feature_type/
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/address.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.652816 oracle_ads-2.8.7/ads/feature_engineering/feature_type/adsstring/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/adsstring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/adsstring/common_regex_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/adsstring/oci_language.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.652816 oracle_ads-2.8.7/ads/feature_engineering/feature_type/adsstring/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/adsstring/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/adsstring/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/adsstring/parsers/nltk_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/adsstring/parsers/spacy_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/adsstring/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/category.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/creditcard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/gis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.652816 oracle_ads-2.8.7/ads/feature_engineering/feature_type/handler/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17237 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/handler/feature_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/handler/feature_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/handler/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/ip_address_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/ip_address_v6.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/lat_long.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/ordinal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/unknown.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type/zip_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/feature_type_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    24398 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/feature_engineering/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.656817 oracle_ads-2.8.7/ads/hpo/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/hpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/hpo/_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    15276 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/hpo/ads_search_space.py
--rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/hpo/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/hpo/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)    57469 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/hpo/search_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/hpo/stopping_criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)    16546 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/hpo/tuner_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/hpo/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/hpo/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.660817 oracle_ads-2.8.7/ads/hpo/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/hpo/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/hpo/visualization/_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/hpo/visualization/_edf.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/hpo/visualization/_intermediate_values.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/hpo/visualization/_optimization_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/hpo/visualization/_parallel_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/hpo/visualization/_param_importances.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.660817 oracle_ads-2.8.7/ads/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19427 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/ads_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.660817 oracle_ads-2.8.7/ads/jobs/builders/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/builders/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.660817 oracle_ads-2.8.7/ads/jobs/builders/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/builders/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/builders/infrastructure/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    39289 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/builders/infrastructure/dataflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    59743 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/builders/infrastructure/dsc_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    40623 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/builders/infrastructure/dsc_job_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/builders/infrastructure/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.660817 oracle_ads-2.8.7/ads/jobs/builders/runtimes/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/builders/runtimes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/builders/runtimes/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/builders/runtimes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/builders/runtimes/container_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)    35145 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/builders/runtimes/python_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/env_var_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.660817 oracle_ads-2.8.7/ads/jobs/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/schema/infrastructure_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/schema/job_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/schema/runtime_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/schema/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.664817 oracle_ads-2.8.7/ads/jobs/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/templates/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/templates/driver_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17947 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/templates/driver_oci.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/templates/driver_python.py
--rw-r--r--   0 runner    (1001) docker     (123)    17935 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/templates/driver_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/jobs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.664817 oracle_ads-2.8.7/ads/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20100 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/artifact_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/artifact_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/base_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.664817 oracle_ads-2.8.7/ads/model/common/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/common/.model-ignore
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    37764 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/datascience_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.664817 oracle_ads-2.8.7/ads/model/deployment/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/deployment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.664817 oracle_ads-2.8.7/ads/model/deployment/common/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/deployment/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/deployment/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/deployment/model_deployer.py
--rw-r--r--   0 runner    (1001) docker     (123)    64556 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/deployment/model_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19761 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/deployment/model_deployment_infrastructure.py
--rw-r--r--   0 runner    (1001) docker     (123)    18205 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/deployment/model_deployment_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    26461 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/deployment/model_deployment_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.668818 oracle_ads-2.8.7/ads/model/extractor/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/extractor/automl_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/extractor/huggingface_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/extractor/keras_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/extractor/lightgbm_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/extractor/model_info_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/extractor/model_info_extractor_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/extractor/pytorch_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/extractor/sklearn_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/extractor/spark_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/extractor/tensorflow_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/extractor/xgboost_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.668818 oracle_ads-2.8.7/ads/model/framework/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/framework/automl_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/framework/huggingface_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/framework/lightgbm_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/framework/pytorch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/framework/sklearn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/framework/spark_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/framework/tensorflow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/framework/xgboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   131973 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/generic_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.668818 oracle_ads-2.8.7/ads/model/model_artifact_boilerplate/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/model_artifact_boilerplate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.668818 oracle_ads-2.8.7/ads/model/model_artifact_boilerplate/artifact_introspection_test/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/model_artifact_boilerplate/artifact_introspection_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17101 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/model_artifact_boilerplate/artifact_introspection_test/model_artifact_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/model_artifact_boilerplate/score.py
--rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/model_introspect.py
--rw-r--r--   0 runner    (1001) docker     (123)    54236 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/model_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    16898 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/model_metadata_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/model_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/model_version_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.668818 oracle_ads-2.8.7/ads/model/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/runtime/env_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/runtime/model_deployment_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/runtime/model_provenance_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/runtime/runtime_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.668818 oracle_ads-2.8.7/ads/model/runtime/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/runtime/schemas/inference_env_info_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/runtime/schemas/model_provenance_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/runtime/schemas/training_env_info_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/runtime/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.672818 oracle_ads-2.8.7/ads/model/serde/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/serde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/serde/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    18577 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/serde/model_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    43205 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/serde/model_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.672818 oracle_ads-2.8.7/ads/model/service/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21157 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/service/oci_datascience_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/service/oci_datascience_model_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/service/oci_datascience_model_version_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.672818 oracle_ads-2.8.7/ads/model/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/model/transformer/onnx_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.672818 oracle_ads-2.8.7/ads/mysqldb/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/mysqldb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/mysqldb/mysql_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.672818 oracle_ads-2.8.7/ads/opctl/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.672818 oracle_ads-2.8.7/ads/opctl/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/backend/ads_dataflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    22718 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/backend/ads_ml_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/backend/ads_ml_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/backend/ads_model_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/backend/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    33222 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/backend/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    19152 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    28311 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/cmds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.672818 oracle_ads-2.8.7/ads/opctl/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/conda/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    22027 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/conda/cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/conda/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/conda/manifest_template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/conda/multipart_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/conda/pack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.676818 oracle_ads-2.8.7/ads/opctl/config/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/config/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.676818 oracle_ads-2.8.7/ads/opctl/config/diagnostics/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/config/diagnostics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.676818 oracle_ads-2.8.7/ads/opctl/config/diagnostics/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/config/diagnostics/distributed/default_requirements_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/config/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12714 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/config/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/config/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/config/versioner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.676818 oracle_ads-2.8.7/ads/opctl/config/yaml_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/config/yaml_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/config/yaml_parsers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.676818 oracle_ads-2.8.7/ads/opctl/config/yaml_parsers/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/config/yaml_parsers/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/config/yaml_parsers/distributed/yaml_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.676818 oracle_ads-2.8.7/ads/opctl/decorator/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/decorator/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.676818 oracle_ads-2.8.7/ads/opctl/diagnostics/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/diagnostics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/diagnostics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/diagnostics/check_distributed_job_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/diagnostics/check_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/diagnostics/requirement_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.676818 oracle_ads-2.8.7/ads/opctl/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/distributed/certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/distributed/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    18772 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/distributed/cmds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.676818 oracle_ads-2.8.7/ads/opctl/distributed/common/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/distributed/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/distributed/common/abstract_cluster_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/distributed/common/abstract_framework_spec_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/distributed/common/cluster_config_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/distributed/common/cluster_provider_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/distributed/common/cluster_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/distributed/common/framework_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.676818 oracle_ads-2.8.7/ads/opctl/docker/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/docker/Dockerfile.gpu
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/docker/Dockerfile.job
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/docker/Dockerfile.job.gpu
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/docker/cuda.repo
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/docker/merge_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/index.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.680819 oracle_ads-2.8.7/ads/opctl/model/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/model/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/model/cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.680819 oracle_ads-2.8.7/ads/opctl/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/spark/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/spark/cmds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.680819 oracle_ads-2.8.7/ads/opctl/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/templates/diagnostic_report_template.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    11985 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/opctl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.680819 oracle_ads-2.8.7/ads/oracledb/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/oracledb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/oracledb/oracle_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.680819 oracle_ads-2.8.7/ads/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    84848 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/pipeline/ads_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    28006 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/pipeline/ads_pipeline_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/pipeline/ads_pipeline_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.680819 oracle_ads-2.8.7/ads/pipeline/builders/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/pipeline/builders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.680819 oracle_ads-2.8.7/ads/pipeline/builders/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/pipeline/builders/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/pipeline/builders/infrastructure/custom_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/pipeline/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/pipeline/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.680819 oracle_ads-2.8.7/ads/pipeline/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/pipeline/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.680819 oracle_ads-2.8.7/ads/pipeline/visualizer/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/pipeline/visualizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15563 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/pipeline/visualizer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/pipeline/visualizer/graph_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/pipeline/visualizer/text_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.680819 oracle_ads-2.8.7/ads/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15817 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/secrets/adb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/secrets/auth_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    13926 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/secrets/big_data_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/secrets/mysqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/secrets/oracledb.py
--rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/secrets/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.680819 oracle_ads-2.8.7/ads/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/telemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/telemetry/telemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.684819 oracle_ads-2.8.7/ads/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/templates/dataflow_pyspark.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/templates/dataflow_sparksql.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/templates/func.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/templates/score-pkl.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/templates/score.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/templates/score_generic.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/templates/score_huggingface_pipeline.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/templates/score_lightgbm.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/templates/score_onnx.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    15835 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/templates/score_onnx_new.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/templates/score_oracle_automl.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/templates/score_pyspark.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/templates/score_pytorch.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/templates/score_scikit-learn.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/templates/score_tensorflow.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/templates/score_xgboost.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.684819 oracle_ads-2.8.7/ads/text_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/text_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/text_dataset/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/text_dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/text_dataset/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/text_dataset/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/text_dataset/udfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/text_dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.688820 oracle_ads-2.8.7/ads/type_discovery/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/type_discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/type_discovery/abstract_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/type_discovery/constant_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/type_discovery/continuous_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/type_discovery/credit_card_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/type_discovery/datetime_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/type_discovery/discrete_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/type_discovery/document_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/type_discovery/ip_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/type_discovery/latlon_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/type_discovery/phone_number_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/type_discovery/type_discovery_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    20105 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/type_discovery/typed_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/type_discovery/unknown_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/type_discovery/zipcode_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.688820 oracle_ads-2.8.7/ads/vault/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-06-23 00:13:04.000000 oracle_ads-2.8.7/ads/vault/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:13:08.688820 oracle_ads-2.8.7/oracle_ads.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-06-23 00:13:08.000000 oracle_ads-2.8.7/oracle_ads.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15898 2023-06-23 00:13:08.000000 oracle_ads-2.8.7/oracle_ads.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 00:13:08.000000 oracle_ads-2.8.7/oracle_ads.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-23 00:13:08.000000 oracle_ads-2.8.7/oracle_ads.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-23 00:13:08.000000 oracle_ads-2.8.7/oracle_ads.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 00:13:08.000000 oracle_ads-2.8.7/oracle_ads.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-23 00:13:08.688820 oracle_ads-2.8.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-23 00:13:05.000000 oracle_ads-2.8.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.345330 oracle_ads-2.8.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-07-27 19:57:02.345330 oracle_ads-2.8.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    50466 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/THIRD_PARTY_LICENSES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.265330 oracle_ads-2.8.8/ads/
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/ads_version.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.265330 oracle_ads-2.8.8/ads/automl/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/automl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/automl/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35984 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/automl/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.265330 oracle_ads-2.8.8/ads/bds/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/bds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/bds/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/bds/big_data_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.265330 oracle_ads-2.8.8/ads/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60039 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/catalog/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16462 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/catalog/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16091 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/catalog/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/catalog/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.273330 oracle_ads-2.8.8/ads/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.273330 oracle_ads-2.8.8/ads/common/artifact/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/artifact/.model-ignore
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/artifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45326 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/card_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20253 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.273330 oracle_ads-2.8.8/ads/common/decorator/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/decorator/argument_to_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/decorator/deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/decorator/runtime_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/decorator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/dsc_file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/extended_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.273330 oracle_ads-2.8.8/ads/common/function/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/function/fn_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/function/func_conf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27269 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72294 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/model_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/model_artifact_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26571 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/model_export_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/model_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/object_storage_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/oci_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/oci_datascience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42155 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/oci_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37239 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/oci_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/oci_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16915 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46073 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22306 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/common/word_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.273330 oracle_ads-2.8.8/ads/data_labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/boundingbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/data_labeling_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.273330 oracle_ads-2.8.8/ads/data_labeling/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/interface/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/interface/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/interface/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.273330 oracle_ads-2.8.8/ads/data_labeling/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/loader/file_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.277330 oracle_ads-2.8.8/ads/data_labeling/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/mixin/data_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/ner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.277330 oracle_ads-2.8.8/ads/data_labeling/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/parser/dls_record_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/parser/export_metadata_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17416 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/parser/export_record_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.277330 oracle_ads-2.8.8/ads/data_labeling/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22145 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/reader/dataset_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/reader/dls_record_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/reader/export_record_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/reader/jsonl_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/reader/metadata_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/reader/record_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.277330 oracle_ads-2.8.8/ads/data_labeling/visualizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/visualizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15880 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/visualizer/image_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/data_labeling/visualizer/text_visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.277330 oracle_ads-2.8.8/ads/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/database/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.281330 oracle_ads-2.8.8/ads/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/classification_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17306 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/correlation_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/dask_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/dataframe_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73481 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/dataset_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38574 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/dataset_with_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37594 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/feature_engineering_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/forecasting_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50067 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/label_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.281330 oracle_ads-2.8.8/ads/dataset/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/mixin/dataset_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26056 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12909 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22168 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/recommendation_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/regression_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39503 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/sampled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dataset/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.281330 oracle_ads-2.8.8/ads/dbmixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dbmixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/dbmixin/db_pandas_accessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.285330 oracle_ads-2.8.8/ads/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/environment/ml_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.285330 oracle_ads-2.8.8/ads/evaluations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/evaluations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39617 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/evaluations/evaluation_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53173 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/evaluations/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21279 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/evaluations/statistical_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.285330 oracle_ads-2.8.8/ads/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.285330 oracle_ads-2.8.8/ads/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/explanations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/explanations/base_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/explanations/explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41704 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/explanations/mlx_global_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/explanations/mlx_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/explanations/mlx_local_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/explanations/mlx_whatif_explainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.285330 oracle_ads-2.8.8/ads/feature_engineering/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.285330 oracle_ads-2.8.8/ads/feature_engineering/accessor/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/accessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18403 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/accessor/dataframe_accessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.289330 oracle_ads-2.8.8/ads/feature_engineering/accessor/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/accessor/mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/accessor/mixin/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/accessor/mixin/eda_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/accessor/mixin/eda_mixin_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/accessor/mixin/feature_types_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/accessor/mixin/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/accessor/series_accessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.289330 oracle_ads-2.8.8/ads/feature_engineering/adsimage/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/adsimage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/adsimage/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/adsimage/image_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.289330 oracle_ads-2.8.8/ads/feature_engineering/adsimage/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/adsimage/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/adsimage/interface/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.289330 oracle_ads-2.8.8/ads/feature_engineering/adsstring/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/adsstring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.289330 oracle_ads-2.8.8/ads/feature_engineering/adsstring/oci_language/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/adsstring/oci_language/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.289330 oracle_ads-2.8.8/ads/feature_engineering/adsstring/string/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/adsstring/string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/data_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.289330 oracle_ads-2.8.8/ads/feature_engineering/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1600358 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/dataset/zip_code_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.297330 oracle_ads-2.8.8/ads/feature_engineering/feature_type/
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/address.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.297330 oracle_ads-2.8.8/ads/feature_engineering/feature_type/adsstring/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/adsstring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/adsstring/common_regex_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/adsstring/oci_language.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.297330 oracle_ads-2.8.8/ads/feature_engineering/feature_type/adsstring/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/adsstring/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/adsstring/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/adsstring/parsers/nltk_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/adsstring/parsers/spacy_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/adsstring/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/creditcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/gis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.297330 oracle_ads-2.8.8/ads/feature_engineering/feature_type/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17237 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/handler/feature_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/handler/feature_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/handler/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/ip_address_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/ip_address_v6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/lat_long.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/ordinal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/unknown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type/zip_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/feature_type_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24398 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/feature_engineering/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.301330 oracle_ads-2.8.8/ads/hpo/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/hpo/_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15276 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/hpo/ads_search_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/hpo/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/hpo/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57469 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/hpo/search_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/hpo/stopping_criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16546 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/hpo/tuner_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/hpo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/hpo/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.301330 oracle_ads-2.8.8/ads/hpo/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/hpo/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/hpo/visualization/_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/hpo/visualization/_edf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/hpo/visualization/_intermediate_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/hpo/visualization/_optimization_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/hpo/visualization/_parallel_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/hpo/visualization/_param_importances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.301330 oracle_ads-2.8.8/ads/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19547 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/ads_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.301330 oracle_ads-2.8.8/ads/jobs/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/builders/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.301330 oracle_ads-2.8.8/ads/jobs/builders/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/builders/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/builders/infrastructure/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39289 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/builders/infrastructure/dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60186 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/builders/infrastructure/dsc_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45101 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/builders/infrastructure/dsc_job_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/builders/infrastructure/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.305330 oracle_ads-2.8.8/ads/jobs/builders/runtimes/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/builders/runtimes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/builders/runtimes/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/builders/runtimes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/builders/runtimes/container_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35143 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/builders/runtimes/python_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/builders/runtimes/pytorch_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/env_var_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.305330 oracle_ads-2.8.8/ads/jobs/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/schema/infrastructure_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/schema/job_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/schema/runtime_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/schema/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.305330 oracle_ads-2.8.8/ads/jobs/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/templates/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/templates/driver_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17936 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/templates/driver_oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/templates/driver_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29686 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/templates/driver_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21419 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/templates/driver_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/templates/oci_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/jobs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.309330 oracle_ads-2.8.8/ads/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20100 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/artifact_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/artifact_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/base_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.309330 oracle_ads-2.8.8/ads/model/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/common/.model-ignore
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37764 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/datascience_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.313330 oracle_ads-2.8.8/ads/model/deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/deployment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.313330 oracle_ads-2.8.8/ads/model/deployment/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/deployment/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/deployment/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/deployment/model_deployer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64390 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/deployment/model_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/deployment/model_deployment_infrastructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18205 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/deployment/model_deployment_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26461 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/deployment/model_deployment_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.313330 oracle_ads-2.8.8/ads/model/extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/extractor/automl_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/extractor/huggingface_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/extractor/keras_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/extractor/lightgbm_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/extractor/model_info_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/extractor/model_info_extractor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/extractor/pytorch_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/extractor/sklearn_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/extractor/spark_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/extractor/tensorflow_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/extractor/xgboost_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.317330 oracle_ads-2.8.8/ads/model/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/framework/automl_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/framework/huggingface_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/framework/lightgbm_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/framework/pytorch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/framework/sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/framework/spark_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/framework/tensorflow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/framework/xgboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132405 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/generic_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.317330 oracle_ads-2.8.8/ads/model/model_artifact_boilerplate/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/model_artifact_boilerplate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.317330 oracle_ads-2.8.8/ads/model/model_artifact_boilerplate/artifact_introspection_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/model_artifact_boilerplate/artifact_introspection_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17101 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/model_artifact_boilerplate/artifact_introspection_test/model_artifact_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/model_artifact_boilerplate/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/model_introspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54236 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/model_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16898 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/model_metadata_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/model_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/model_version_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.317330 oracle_ads-2.8.8/ads/model/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/runtime/env_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/runtime/model_deployment_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/runtime/model_provenance_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/runtime/runtime_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.317330 oracle_ads-2.8.8/ads/model/runtime/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/runtime/schemas/inference_env_info_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/runtime/schemas/model_provenance_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/runtime/schemas/training_env_info_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/runtime/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.317330 oracle_ads-2.8.8/ads/model/serde/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/serde/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18577 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/serde/model_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43205 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/serde/model_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.317330 oracle_ads-2.8.8/ads/model/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21157 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/service/oci_datascience_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/service/oci_datascience_model_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/service/oci_datascience_model_version_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.321330 oracle_ads-2.8.8/ads/model/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/model/transformer/onnx_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.321330 oracle_ads-2.8.8/ads/mysqldb/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/mysqldb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/mysqldb/mysql_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.321330 oracle_ads-2.8.8/ads/opctl/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.321330 oracle_ads-2.8.8/ads/opctl/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/backend/ads_dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22718 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/backend/ads_ml_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/backend/ads_ml_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/backend/ads_model_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/backend/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33222 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/backend/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21179 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28780 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/cmds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.325330 oracle_ads-2.8.8/ads/opctl/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/conda/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22027 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/conda/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/conda/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/conda/manifest_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/conda/multipart_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/conda/pack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.325330 oracle_ads-2.8.8/ads/opctl/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/config/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.325330 oracle_ads-2.8.8/ads/opctl/config/diagnostics/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/config/diagnostics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.325330 oracle_ads-2.8.8/ads/opctl/config/diagnostics/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/config/diagnostics/distributed/default_requirements_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/config/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12714 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/config/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/config/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/config/versioner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.325330 oracle_ads-2.8.8/ads/opctl/config/yaml_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/config/yaml_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/config/yaml_parsers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.325330 oracle_ads-2.8.8/ads/opctl/config/yaml_parsers/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/config/yaml_parsers/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/config/yaml_parsers/distributed/yaml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.325330 oracle_ads-2.8.8/ads/opctl/decorator/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/decorator/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.325330 oracle_ads-2.8.8/ads/opctl/diagnostics/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/diagnostics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/diagnostics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/diagnostics/check_distributed_job_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/diagnostics/check_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/diagnostics/requirement_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.329330 oracle_ads-2.8.8/ads/opctl/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/distributed/certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/distributed/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18772 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/distributed/cmds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.329330 oracle_ads-2.8.8/ads/opctl/distributed/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/distributed/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/distributed/common/abstract_cluster_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/distributed/common/abstract_framework_spec_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/distributed/common/cluster_config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/distributed/common/cluster_provider_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/distributed/common/cluster_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/distributed/common/framework_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.329330 oracle_ads-2.8.8/ads/opctl/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/docker/Dockerfile.gpu
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/docker/Dockerfile.job
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/docker/Dockerfile.job.gpu
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/docker/base-env.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/docker/cuda.repo
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/docker/merge_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/index.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.329330 oracle_ads-2.8.8/ads/opctl/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/model/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/model/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.329330 oracle_ads-2.8.8/ads/opctl/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/spark/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/spark/cmds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.329330 oracle_ads-2.8.8/ads/opctl/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/templates/diagnostic_report_template.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    11985 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/opctl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.329330 oracle_ads-2.8.8/ads/oracledb/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/oracledb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/oracledb/oracle_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.333330 oracle_ads-2.8.8/ads/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84872 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/pipeline/ads_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28006 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/pipeline/ads_pipeline_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/pipeline/ads_pipeline_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.333330 oracle_ads-2.8.8/ads/pipeline/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/pipeline/builders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.333330 oracle_ads-2.8.8/ads/pipeline/builders/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/pipeline/builders/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/pipeline/builders/infrastructure/custom_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/pipeline/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/pipeline/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.333330 oracle_ads-2.8.8/ads/pipeline/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/pipeline/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.333330 oracle_ads-2.8.8/ads/pipeline/visualizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/pipeline/visualizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15563 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/pipeline/visualizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/pipeline/visualizer/graph_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/pipeline/visualizer/text_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.337330 oracle_ads-2.8.8/ads/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15817 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/secrets/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/secrets/auth_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13926 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/secrets/big_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/secrets/mysqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/secrets/oracledb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15254 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/secrets/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.337330 oracle_ads-2.8.8/ads/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/telemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/telemetry/telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.337330 oracle_ads-2.8.8/ads/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/templates/dataflow_pyspark.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/templates/dataflow_sparksql.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/templates/func.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/templates/score-pkl.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/templates/score.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/templates/score_generic.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/templates/score_huggingface_pipeline.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/templates/score_lightgbm.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/templates/score_onnx.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    15835 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/templates/score_onnx_new.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/templates/score_oracle_automl.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/templates/score_pyspark.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/templates/score_pytorch.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/templates/score_scikit-learn.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/templates/score_tensorflow.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/templates/score_xgboost.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.341330 oracle_ads-2.8.8/ads/text_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/text_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/text_dataset/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/text_dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/text_dataset/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/text_dataset/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/text_dataset/udfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/text_dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.341330 oracle_ads-2.8.8/ads/type_discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/type_discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/type_discovery/abstract_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/type_discovery/constant_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/type_discovery/continuous_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/type_discovery/credit_card_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/type_discovery/datetime_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/type_discovery/discrete_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/type_discovery/document_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/type_discovery/ip_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/type_discovery/latlon_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/type_discovery/phone_number_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/type_discovery/type_discovery_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20105 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/type_discovery/typed_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/type_discovery/unknown_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/type_discovery/zipcode_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.341330 oracle_ads-2.8.8/ads/vault/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-07-27 19:56:57.000000 oracle_ads-2.8.8/ads/vault/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:57:02.345330 oracle_ads-2.8.8/oracle_ads.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-07-27 19:57:02.000000 oracle_ads-2.8.8/oracle_ads.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16046 2023-07-27 19:57:02.000000 oracle_ads-2.8.8/oracle_ads.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:57:02.000000 oracle_ads-2.8.8/oracle_ads.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-27 19:57:02.000000 oracle_ads-2.8.8/oracle_ads.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-27 19:57:02.000000 oracle_ads-2.8.8/oracle_ads.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-27 19:57:02.000000 oracle_ads-2.8.8/oracle_ads.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-27 19:57:02.345330 oracle_ads-2.8.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-27 19:56:58.000000 oracle_ads-2.8.8/setup.py
```

### Comparing `oracle_ads-2.8.7/LICENSE.txt` & `oracle_ads-2.8.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/MANIFEST.in` & `oracle_ads-2.8.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/PKG-INFO` & `oracle_ads-2.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oracle_ads
-Version: 2.8.7
+Version: 2.8.8
 Summary: Oracle Accelerated Data Science SDK
 Home-page: https://docs.oracle.com/en-us/iaas/tools/ads-sdk/latest/index.html
 Author: Oracle Data Science
 License: Universal Permissive License 1.0
 Project-URL: Github, https://github.com/oracle/accelerated-data-science
 Project-URL: Documentation, https://accelerated-data-science.readthedocs.io/en/latest/index.html
 Keywords: Oracle Cloud Infrastructure,OCI,Machine Learning,ML,Artificial Intelligence,AI,Data Science,Cloud,Oracle
```

### Comparing `oracle_ads-2.8.7/README.md` & `oracle_ads-2.8.8/README.md`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/THIRD_PARTY_LICENSES.txt` & `oracle_ads-2.8.8/THIRD_PARTY_LICENSES.txt`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/__init__.py` & `oracle_ads-2.8.8/ads/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/automl/driver.py` & `oracle_ads-2.8.8/ads/automl/driver.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/automl/provider.py` & `oracle_ads-2.8.8/ads/automl/provider.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/bds/auth.py` & `oracle_ads-2.8.8/ads/bds/auth.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/bds/big_data_service.py` & `oracle_ads-2.8.8/ads/bds/big_data_service.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/catalog/model.py` & `oracle_ads-2.8.8/ads/catalog/model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/catalog/notebook.py` & `oracle_ads-2.8.8/ads/catalog/notebook.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/catalog/project.py` & `oracle_ads-2.8.8/ads/catalog/project.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/catalog/summary.py` & `oracle_ads-2.8.8/ads/catalog/summary.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/cli.py` & `oracle_ads-2.8.8/ads/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/analyzer.py` & `oracle_ads-2.8.8/ads/common/analyzer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/artifact/.model-ignore` & `oracle_ads-2.8.8/ads/common/artifact/.model-ignore`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/auth.py` & `oracle_ads-2.8.8/ads/common/auth.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/card_identifier.py` & `oracle_ads-2.8.8/ads/common/card_identifier.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/config.py` & `oracle_ads-2.8.8/ads/common/config.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/data.py` & `oracle_ads-2.8.8/ads/common/data.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/decorator/argument_to_case.py` & `oracle_ads-2.8.8/ads/common/decorator/argument_to_case.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/decorator/deprecate.py` & `oracle_ads-2.8.8/ads/common/decorator/deprecate.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/decorator/runtime_dependency.py` & `oracle_ads-2.8.8/ads/common/decorator/runtime_dependency.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/decorator/utils.py` & `oracle_ads-2.8.8/ads/common/decorator/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/dsc_file_system.py` & `oracle_ads-2.8.8/ads/common/dsc_file_system.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/error.py` & `oracle_ads-2.8.8/ads/common/error.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/extended_enum.py` & `oracle_ads-2.8.8/ads/common/extended_enum.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/function/fn_util.py` & `oracle_ads-2.8.8/ads/common/function/fn_util.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/function/func_conf.yaml` & `oracle_ads-2.8.8/ads/common/function/func_conf.yaml`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/ipython.py` & `oracle_ads-2.8.8/ads/common/ipython.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/model.py` & `oracle_ads-2.8.8/ads/common/model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/model_artifact.py` & `oracle_ads-2.8.8/ads/common/model_artifact.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/model_artifact_schema.json` & `oracle_ads-2.8.8/ads/common/model_artifact_schema.json`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/model_export_util.py` & `oracle_ads-2.8.8/ads/common/model_export_util.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/model_metadata.py` & `oracle_ads-2.8.8/ads/common/model_metadata.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/object_storage_details.py` & `oracle_ads-2.8.8/ads/common/object_storage_details.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/oci_client.py` & `oracle_ads-2.8.8/ads/common/oci_client.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/oci_datascience.py` & `oracle_ads-2.8.8/ads/common/oci_datascience.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/oci_logging.py` & `oracle_ads-2.8.8/ads/common/oci_logging.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/oci_mixin.py` & `oracle_ads-2.8.8/ads/common/oci_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
             if key in attribute_map:
                 parsed_kwargs[attribute_map[key]] = val
             else:
                 parsed_kwargs[key] = val
 
         return parsed_kwargs
 
-    @classmethod
+    @class_or_instance_method
     def deserialize(cls, data, to_cls):
         """De-serialize data from dictionary to an OCI model"""
         if cls.type_mappings is None:
             cls.type_mappings = cls.init_client().base_client.type_mappings
 
         if data is None:
             return None
@@ -545,15 +545,15 @@
         ----------
         data : dict
             A dictionary containing the properties to initialize the class.
 
         """
         return cls.create_instance(**data)
 
-    @classmethod
+    @class_or_instance_method
     def deserialize(cls, data: dict, to_cls: str = None):
         """Deserialize data
 
         Parameters
         ----------
         data : dict
             A dictionary containing the data to be deserialized.
```

### Comparing `oracle_ads-2.8.7/ads/common/oci_resource.py` & `oracle_ads-2.8.8/ads/common/oci_resource.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/serializer.py` & `oracle_ads-2.8.8/ads/common/serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from typing import Dict, Optional, Union
 from urllib.parse import urlparse
 
 import fsspec
 import yaml
 
 from ads.common import logger
+from ads.common.auth import default_signer
 
 try:
     from yaml import CSafeDumper as dumper
     from yaml import CSafeLoader as loader
 except:
     from yaml import SafeDumper as dumper
     from yaml import SafeLoader as loader
@@ -130,14 +131,22 @@
             keyword arguments to be passed into fsspec.open().
             For OCI object storage, this can be config="path/to/.oci/config".
 
         Returns
         -------
         string: Contents in file specified by URI
         """
+        # Add default signer if the uri is an object storage uri, and
+        # the user does not specify config or signer.
+        if (
+            uri.startswith("oci://")
+            and "config" not in kwargs
+            and "signer" not in kwargs
+        ):
+            kwargs.update(default_signer())
         with fsspec.open(uri, "r", **kwargs) as f:
             return f.read()
 
     def to_json(
         self, uri: str = None, encoder: callable = json.JSONEncoder, **kwargs
     ) -> str:
         """Returns object serialized as a JSON string
```

### Comparing `oracle_ads-2.8.7/ads/common/utils.py` & `oracle_ads-2.8.8/ads/common/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/common/word_lists.py` & `oracle_ads-2.8.8/ads/common/word_lists.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/config.py` & `oracle_ads-2.8.8/ads/config.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/data_labeling/__init__.py` & `oracle_ads-2.8.8/ads/data_labeling/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/data_labeling/boundingbox.py` & `oracle_ads-2.8.8/ads/data_labeling/boundingbox.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/data_labeling/constants.py` & `oracle_ads-2.8.8/ads/data_labeling/constants.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/data_labeling/data_labeling_service.py` & `oracle_ads-2.8.8/ads/data_labeling/data_labeling_service.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/data_labeling/interface/reader.py` & `oracle_ads-2.8.8/ads/data_labeling/interface/reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/data_labeling/loader/file_loader.py` & `oracle_ads-2.8.8/ads/data_labeling/loader/file_loader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/data_labeling/metadata.py` & `oracle_ads-2.8.8/ads/data_labeling/metadata.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/data_labeling/mixin/data_labeling.py` & `oracle_ads-2.8.8/ads/data_labeling/mixin/data_labeling.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/data_labeling/ner.py` & `oracle_ads-2.8.8/ads/data_labeling/ner.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/data_labeling/parser/dls_record_parser.py` & `oracle_ads-2.8.8/ads/data_labeling/parser/dls_record_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/data_labeling/parser/export_metadata_parser.py` & `oracle_ads-2.8.8/ads/data_labeling/parser/export_metadata_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/data_labeling/parser/export_record_parser.py` & `oracle_ads-2.8.8/ads/data_labeling/parser/export_record_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/data_labeling/reader/dataset_reader.py` & `oracle_ads-2.8.8/ads/data_labeling/reader/dataset_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/data_labeling/reader/dls_record_reader.py` & `oracle_ads-2.8.8/ads/data_labeling/reader/dls_record_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/data_labeling/reader/export_record_reader.py` & `oracle_ads-2.8.8/ads/data_labeling/reader/export_record_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/data_labeling/reader/jsonl_reader.py` & `oracle_ads-2.8.8/ads/data_labeling/reader/jsonl_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/data_labeling/reader/metadata_reader.py` & `oracle_ads-2.8.8/ads/data_labeling/reader/metadata_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/data_labeling/reader/record_reader.py` & `oracle_ads-2.8.8/ads/data_labeling/reader/record_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/data_labeling/record.py` & `oracle_ads-2.8.8/ads/data_labeling/record.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/data_labeling/visualizer/image_visualizer.py` & `oracle_ads-2.8.8/ads/data_labeling/visualizer/image_visualizer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/data_labeling/visualizer/text_visualizer.py` & `oracle_ads-2.8.8/ads/data_labeling/visualizer/text_visualizer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/database/connection.py` & `oracle_ads-2.8.8/ads/database/connection.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/dataset/classification_dataset.py` & `oracle_ads-2.8.8/ads/dataset/classification_dataset.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/dataset/correlation.py` & `oracle_ads-2.8.8/ads/dataset/correlation.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/dataset/correlation_plot.py` & `oracle_ads-2.8.8/ads/dataset/correlation_plot.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/dataset/dask_series.py` & `oracle_ads-2.8.8/ads/dataset/dask_series.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/dataset/dataframe_transformer.py` & `oracle_ads-2.8.8/ads/dataset/dataframe_transformer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/dataset/dataset.py` & `oracle_ads-2.8.8/ads/dataset/dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 from ads.dataset.helper import (
     convert_columns,
     fix_column_names,
     generate_sample,
     DatasetDefaults,
     deprecate_default_value,
     deprecate_variable,
+    get_dataset,
+    infer_target_type,
 )
 from ads.dataset.label_encoder import DataFrameLabelEncoder
 from ads.dataset.pipeline import TransformerPipeline
 from ads.dataset.progress import DummyProgressBar
 from ads.dataset.sampled_dataset import PandasDataset
 from ads.type_discovery.type_discovery_driver import TypeDiscoveryDriver
 from ads.dataset.helper import get_feature_type
@@ -219,15 +221,16 @@
         Returns
         -------
         dataset_head : pandas.DataFrame
             The first `n` rows of the dataset
 
         Examples
         --------
-        >>> ds = DatasetFactory.open("classfication_data.csv")
+        >>> import pandas as pd
+        >>> ds = ADSDataset.from_dataframe(pd.read_csv("classfication_data.csv"))
         >>> ds.head()
         * displays the first 5 rows of the dataset, just as the traditional head() function would *
         """
         df = self.df.head(n=n)
 
         #
         # we could just return the above but, jupyterlab doesn't render these well
@@ -294,15 +297,16 @@
         Returns
         -------
         func: function
             a plotting function that contains `*args` and `**kwargs`
 
         Examples
         --------
-        >>> ds = DatasetFactory.open("classfication_data.csv")
+        >>> import pandas as pd
+        >>> ds = ADSDataset.from_dataframe(pd.read_csv("classfication_data.csv"))
         >>> def f1(df):
         ...  return(sum(df), axis=0)
         >>> sum_ds = ds.call(f1)
         """
 
         data = "df"
         if isinstance(func, tuple):
@@ -336,28 +340,27 @@
         Returns
         -------
         ds: ADSDataset
             tagged according to the type of the target column.
 
         Examples
         --------
-        >>> ds = DatasetFactory.open("classfication_data.csv")
+        >>> import pandas as pd
+        >>> ds = ADSDataset.from_dataframe(pd.read_csv("classfication_data.csv"))
         >>> ds_with_target= ds.set_target("target_class")
         """
-        from ads.dataset.factory import DatasetFactory
-
         if target_type:
             target_series = self.sampled_df[target].astype(target_type)
         else:
             target_series = self.sampled_df[target]
-        return DatasetFactory._get_dataset(
+        return get_dataset(
             self.df,
             self.sampled_df,
             target,
-            DatasetFactory.infer_target_type(target, target_series, type_discovery),
+            infer_target_type(target, target_series, type_discovery),
             self.shape,
             **self.init_kwargs,
         )
 
     @deprecated("2.5.2", details="Instead use `to_pandas`.")
     def to_pandas_dataframe(
         self, filter=None, frac=None, include_transformer_pipeline=False
@@ -392,15 +395,16 @@
         dataframe : pandas.DataFrame
             if include_transformer_pipeline is False.
         (data, transformer_pipeline): tuple of pandas.DataFrame and dataset.pipeline.TransformerPipeline
             if include_transformer_pipeline is True.
 
         Examples
         --------
-        >>> ds = DatasetFactory.open("data.csv")
+        >>> import pandas as pd
+        >>> ds = ADSDataset.from_dataframe(pd.read_csv("data.csv"))
         >>> ds_as_df = ds.to_pandas()
 
         Notes
         -----
         See also https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html#sklearn.pipeline.Pipeline
         """
         df = self.df.query(filter) if filter is not None else self.df.copy()
@@ -458,15 +462,16 @@
         dataframe : dask.dataframe.core.DataFrame
             if include_transformer_pipeline is False.
         (data, transformer_pipeline): tuple of dask.dataframe.core.DataFrame and dataset.pipeline.TransformerPipeline
             if include_transformer_pipeline is True.
 
         Examples
         --------
-        >>> ds = DatasetFactory.open("data.csv")
+        >>> import pandas as pd
+        >>> ds = ADSDataset.from_dataframe(pd.read_csv("data.csv"))
         >>> ds_dask = ds.to_dask()
 
         Notes
         -----
         See also http://docs.dask.org/en/latest/dataframe-api.html#dataframe and
         https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html#sklearn.pipeline.Pipeline
 
@@ -517,15 +522,16 @@
         dataframe : h2o.H2OFrame
             if include_transformer_pipeline is False.
         (data, transformer_pipeline): tuple of  h2o.H2OFrame and dataset.pipeline.TransformerPipeline
             if include_transformer_pipeline is True.
 
         Examples
         --------
-        >>> ds = DatasetFactory.open("data.csv")
+        >>> import pandas as pd
+        >>> ds = ADSDataset.from_dataframe(pd.read_csv("data.csv"))
         >>> ds_as_h2o = ds.to_h2o()
 
         Notes
         -----
         See also https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html#sklearn.pipeline.Pipeline
         """
         res = self.to_pandas(
@@ -574,15 +580,16 @@
         dataframe : xgboost.DMatrix
             if include_transformer_pipeline is False.
         (data, transformer_pipeline): tuple of xgboost.DMatrix and dataset.pipeline.TransformerPipeline
             if include_transformer_pipeline is True.
 
         Examples
         --------
-        >>> ds = DatasetFactory.open("data.csv")
+        >>> import pandas as pd
+        >>> ds = ADSDataset.from_dataframe(pd.read_csv("data.csv"))
         >>> xgb_dmat = ds.to_xgb()
 
         Notes
         -----
         See also https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html#sklearn.pipeline.Pipeline
         """
         res = self.to_pandas(
@@ -613,15 +620,16 @@
         Returns
         -------
         sampled_dataset: ADSDataset
             An ADSDataset which was randomly sampled.
 
         Examples
         --------
-        >>> ds = DatasetFactory.open("data.csv")
+        >>> import pandas as pd
+        >>> ds = ADSDataset.from_dataframe(pd.read_csv("data.csv"))
         >>> ds_sample = ds.sample()
         """
         df = self.df.sample(frac=frac, random_state=random_state)
         return self._build_new_dataset(df)
 
     def drop_columns(self, columns):
         """
@@ -640,15 +648,16 @@
         Raises
         ------
         ValidationError
             If any of the feature names is not found in the dataset.
 
         Examples
         --------
-        >>> ds = DatasetFactory.open("data.csv")
+        >>> import pandas as pd
+        >>> ds = ADSDataset.from_dataframe(pd.read_csv("data.csv"))
         >>> ds_smaller = ds.drop_columns(['col1', 'col2'])
         """
         self._validate_feature(columns)
         return self.drop(columns, axis=1)
 
     def assign_column(self, column, arg):
         """
@@ -667,15 +676,16 @@
         Returns
         -------
         dataset: same type as the caller
             a dataset with the specified column assigned.
 
         Examples
         --------
-        >>> ds = DatasetFactory.open("data.csv")
+        >>> import pandas as pd
+        >>> ds = ADSDataset.from_dataframe(pd.read_csv("data.csv"))
         >>> ds_same_size = ds.assign_column('target',lambda x:  x>15 if x not None)
         >>> ds_bigger = ds.assign_column('new_col', np.arange(ds.shape[0]))
         """
         target_name = (
             self.target.name if not utils.is_same_class(self, ADSDataset) else None
         )
         if isinstance(arg, Iterable) or isinstance(arg, ADSDataset):
@@ -742,15 +752,16 @@
         Returns
         -------
         dataset: same type as the caller
             A dataset with specified columns renamed.
 
         Examples
         --------
-        >>> ds = DatasetFactory.open("data.csv")
+        >>> import pandas as pd
+        >>> ds = ADSDataset.from_dataframe(pd.read_csv("data.csv"))
         >>> ds_renamed = ds.rename_columns({'col1': 'target'})
         """
         if isinstance(columns, list):
             assert len(columns) == len(
                 self.columns.values
             ), "columns length do not match the dataset"
             columns = dict(zip(self.columns.values, columns))
@@ -766,15 +777,16 @@
         Parameters
         ----------
         name: str
             Name of the dataset.
 
         Examples
         --------
-        >>> ds = DatasetFactory.open("data1.csv")
+        >>> import pandas as pd
+        >>> ds = ADSDataset.from_dataframe(pd.read_csv("data1.csv"))
         >>> ds_renamed = ds.set_name("dataset1")
         """
         self.name = name
 
     def set_description(self, description):
         """
         Sets description for the dataset.
@@ -784,15 +796,16 @@
         Parameters
         ----------
         description: str
             Description of the dataset.
 
         Examples
         --------
-        >>> ds = DatasetFactory.open("data1.csv")
+        >>> import pandas as pd
+        >>> ds = ADSDataset.from_dataframe(pd.read_csv("data1.csv"))
         >>> ds_renamed = ds.set_description("dataset1 is from "data1.csv"")
         """
         self.description = description
 
     def snapshot(self, snapshot_dir=None, name="", storage_options=None):
         """
         Snapshot the dataset with modifications made so far.
@@ -817,15 +830,16 @@
         Returns
         -------
         p_str: str
             the URI to access the snapshotted dataset.
 
         Examples
         --------
-        >>> ds = DatasetFactory.open("data.csv")
+        >>> import pandas as pd
+        >>> ds = ADSDataset.from_dataframe(pd.read_csv("data.csv"))
         >>> ds_uri = ds.snapshot()
         """
         if snapshot_dir is None:
             import ads.dataset.factory as factory
 
             snapshot_dir = factory.default_snapshots_dir
             if snapshot_dir is None:
@@ -869,15 +883,16 @@
         storage_options: dict, optional
              Parameters passed on to the backend filesystem class.
              Defaults to storage_options set using DatasetFactory.set_default_storage().
         kwargs: dict, optional
 
         Examples
         --------
-        >>> ds = DatasetFactory.open("data.csv")
+        >>> import pandas as pd
+        >>> ds = ADSDataset.from_dataframe(pd.read_csv("data.csv"))
         >>> [ds_link] = ds.to_csv("my/path.csv")
         """
         if storage_options is None:
             import ads.dataset.factory as factory
 
             storage_options = factory.default_storage_options
             logger.info("Using default storage options")
@@ -896,15 +911,16 @@
         storage_options: dict, optional
              Parameters passed on to the backend filesystem class.
              Defaults to storage_options set using DatasetFactory.set_default_storage().
         kwargs: dict, optional
 
         Examples
         --------
-        >>> ds = DatasetFactory.open("data.csv")
+        >>> import pandas as pd
+        >>> ds = ADSDataset.from_dataframe(pd.read_csv("data.csv"))
         >>> ds.to_parquet("my/path")
         """
         if storage_options is None:
             import ads.dataset.factory as factory
 
             storage_options = factory.default_storage_options
             logger.info("Using default storage options")
@@ -923,15 +939,16 @@
         storage_options: dict, optional
             Parameters passed on to the backend filesystem class.
             Defaults to storage_options set using DatasetFactory.set_default_storage().
         kwargs: dict, optional
 
         Examples
         --------
-        >>> ds = DatasetFactory.open("data.csv")
+        >>> import pandas as pd
+        >>> ds = ADSDataset.from_dataframe(pd.read_csv("data.csv"))
         >>> ds.to_json("my/path.json")
         """
         if storage_options is None:
             import ads.dataset.factory as factory
 
             storage_options = factory.default_storage_options
             logger.info("Using default storage options")
@@ -958,15 +975,16 @@
         Returns
         -------
         str
             The filename of the HDF5 file created.
 
         Examples
         --------
-        >>> ds = DatasetFactory.open("data.csv")
+        >>> import pandas as pd
+        >>> ds = ADSDataset.from_dataframe(pd.read_csv("data.csv"))
         >>> ds.to_hdf(path="my/path.h5", key="df")
         """
         if storage_options is None:
             import ads.dataset.factory as factory
 
             storage_options = factory.default_storage_options
             logger.info("Using default storage options")
@@ -1031,15 +1049,21 @@
         descriptors; "type" must always be "record". The list of fields should
         have an entry for every key of the input records, and the types are
         like the primitive, complex or logical types of the Avro spec
         (https://avro.apache.org/docs/1.8.2/spec.html).
 
         Examples
         --------
-        >>> ds = DatasetFactory.open("data.avro")
+        >>> import pandas
+        >>> import fastavro
+        >>> with open("data.avro", "rb") as fp:
+        >>>     reader = fastavro.reader(fp)
+        >>>     records = [r for r in reader]
+        >>>     df = pandas.DataFrame.from_records(records)
+        >>> ds = ADSDataset.from_dataframe(df)
         >>> ds.to_avro("my/path.avro")
         """
         # Get the row by row formatting
         data_row_by_row = []
         for i, row in self.df.iterrows():
             data_row_by_row.append(row.to_dict())
         # Try to auto-generate schema
@@ -1097,15 +1121,16 @@
         Returns
         -------
         updated_dataset: `ADSDataset`
             an ADSDataset with new data types
 
         Examples
         --------
-        >>> ds = DatasetFactory.open("data.csv")
+        >>> import pandas as pd
+        >>> ds = ADSDataset.from_dataframe(pd.read_csv("data.csv"))
         >>> ds_reformatted = ds.astype({"target": "categorical"})
         """
         return self.__getattr__("astype")(helper.map_types(types))
 
     def merge(self, data, **kwargs):
         """
         Merges this dataset with another ADSDataset or pandas dataframe.
@@ -1115,16 +1140,18 @@
         data : Union[ADSDataset, pandas.DataFrame]
             Data to merge.
         kwargs : dict, optional
             additional keyword arguments that would be passed to underlying dataframe's merge API.
 
         Examples
         --------
-        >>> ds1 = DatasetFactory.open("data1.csv")
-        >>> ds2 = DatasetFactory.open("data2.csv")
+        >>> import pandas as pd
+        >>> df1 = pd.read_csv("data1.csv")
+        >>> df2 = pd.read_csv("data2.csv")
+        >>> ds = ADSDataset.from_dataframe(df1.merge(df2))
         >>> ds_12 = ds1.merge(ds2)
         """
         assert isinstance(data, pd.DataFrame) or isinstance(
             data, ADSDataset
         ), "Can only merge datasets if they are of the types pandas or ads"
         df = self.df.merge(data.df if isinstance(data, ADSDataset) else data, **kwargs)
         return self._build_new_dataset(df, progress=utils.get_progress_bar(3))
@@ -1271,17 +1298,16 @@
         set_documentation_mode(prev_doc_mode)
 
         # return a  ADSDataset object if the target has been removed from the dataframe
         if target in sampled_df.columns:
             if progress:
                 progress.update("Building new dataset")
             target_type = self.target.type if target_type is None else target_type
-            from ads.dataset.factory import DatasetFactory
 
-            new_ds = DatasetFactory._get_dataset(
+            new_ds = get_dataset(
                 df,
                 sampled_df,
                 target,
                 target_type,
                 shape,
                 progress=progress,
                 **init_kwargs,
```

### Comparing `oracle_ads-2.8.7/ads/dataset/dataset_browser.py` & `oracle_ads-2.8.8/ads/dataset/dataset_browser.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from typing import List, Set, Tuple, Dict
 
 import requests
 
 import pandas as pd
 import sklearn.datasets as sk_datasets
 
-from ads.dataset.factory import DatasetFactory
+from ads.dataset import helper
 from ads.common.utils import inject_and_copy_kwargs
 from ads.common.decorator.runtime_dependency import (
     runtime_dependency,
     OptionalDependency,
 )
 
 
@@ -166,15 +166,15 @@
     def open(self, name: str, **kwargs):
         #
         # lookup the name
         #
 
         for obj in self._generate_filelist():
             if obj["name"] == name:
-                return DatasetFactory.open(
+                return helper.open(
                     **inject_and_copy_kwargs(
                         kwargs,
                         **{
                             "source": obj["url"],
                             "format": obj["format"],
                             "name": obj["name"],
                             "description": obj["description"],
@@ -198,15 +198,15 @@
     def open(self, name: str, **kwargs):
         #
         # lookup the name
         #
 
         for obj in self._generate_filelist():
             if obj["name"] == name:
-                return DatasetFactory.open(
+                return helper.open(
                     **inject_and_copy_kwargs(
                         kwargs,
                         **{
                             "source": obj["path"],
                             "format": obj["format"],
                             "name": obj["name"],
                             "description": obj["description"],
@@ -282,15 +282,15 @@
 
     def open(self, name: str, **kwargs):
         #
         # lookup the name
         #
         for obj in self.listing:
             if obj["name"] == name:
-                return DatasetFactory.open(
+                return helper.open(
                     obj["url"],
                     format=obj["format"],
                     name=obj["name"],
                     description=obj["description"],
                 )
         raise ValueError(f"dataset [{name}] does not exist, use .list() to display all")
 
@@ -303,15 +303,15 @@
 
     def list(self, filter_pattern: str = ".*") -> List[str]:
         return super().filter_list(self.dataset_names, filter_pattern)
 
     @runtime_dependency(module="seaborn", install_from=OptionalDependency.VIZ)
     def open(self, name: str, **kwargs):
         if name in self.dataset_names:
-            return DatasetFactory.open(
+            return helper.open(
                 seaborn.load_dataset(name), name=name, description="from seaborn"
             )
         else:
             raise ValueError(
                 "dataset [{name}] does not exist, use .list() to display all"
             )
 
@@ -346,15 +346,15 @@
                 df["target"] = pd.Series(
                     [data.target_names[x] for x in data.target]
                 ).astype("category")
             else:
                 df = pd.DataFrame(data.data, columns=data.feature_names)
                 df["target"] = pd.Series(data.target)
 
-            return DatasetFactory.open(
+            return helper.open(
                 df, target="target", name=name, description=description
             )
 
         else:
             raise ValueError(
                 f"dataset [{name}] does not exist, use .list() to display all"
             )
```

### Comparing `oracle_ads-2.8.7/ads/dataset/dataset_with_target.py` & `oracle_ads-2.8.8/ads/dataset/dataset_with_target.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/dataset/exception.py` & `oracle_ads-2.8.8/ads/dataset/exception.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/dataset/factory.py` & `oracle_ads-2.8.8/ads/dataset/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,25 @@
 from ads.common.decorator.deprecate import deprecated
 
 default_snapshots_dir = None
 default_storage_options = None
 mindate = datetime.date(datetime.MINYEAR, 1, 1)
 
 
+warnings.warn(
+    (
+        "The `ads.dataset.factory` is deprecated in `oracle-ads 2.8.8` and will be removed in `oracle-ads 3.0`."
+        "Use Pandas to read from local files or object storage directly. "
+        "Check https://accelerated-data-science.readthedocs.io/en/latest/user_guide/loading_data/connect.html."
+    ),
+    DeprecationWarning,
+    stacklevel=2,
+)
+
+
 class DatasetFactory:
     @staticmethod
     @deprecated(
         "2.6.6",
         details="Deprecated in favor of using Pandas. Pandas supports reading from object storage directly. Check https://accelerated-data-science.readthedocs.io/en/latest/user_guide/loading_data/connect.html",
     )
     def open(
```

### Comparing `oracle_ads-2.8.7/ads/dataset/feature_engineering_transformer.py` & `oracle_ads-2.8.8/ads/dataset/feature_engineering_transformer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/dataset/feature_selection.py` & `oracle_ads-2.8.8/ads/dataset/feature_selection.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/dataset/forecasting_dataset.py` & `oracle_ads-2.8.8/ads/dataset/forecasting_dataset.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/dataset/label_encoder.py` & `oracle_ads-2.8.8/ads/dataset/label_encoder.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/dataset/mixin/dataset_accessor.py` & `oracle_ads-2.8.8/ads/dataset/mixin/dataset_accessor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/dataset/pipeline.py` & `oracle_ads-2.8.8/ads/dataset/pipeline.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/dataset/plot.py` & `oracle_ads-2.8.8/ads/dataset/plot.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/dataset/progress.py` & `oracle_ads-2.8.8/ads/dataset/progress.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/dataset/recommendation.py` & `oracle_ads-2.8.8/ads/dataset/recommendation.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/dataset/recommendation_transformer.py` & `oracle_ads-2.8.8/ads/dataset/recommendation_transformer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/dataset/regression_dataset.py` & `oracle_ads-2.8.8/ads/dataset/regression_dataset.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/dataset/sampled_dataset.py` & `oracle_ads-2.8.8/ads/dataset/sampled_dataset.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/dataset/target.py` & `oracle_ads-2.8.8/ads/dataset/target.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/dataset/timeseries.py` & `oracle_ads-2.8.8/ads/dataset/timeseries.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/dbmixin/db_pandas_accessor.py` & `oracle_ads-2.8.8/ads/dbmixin/db_pandas_accessor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/environment/ml_runtime.py` & `oracle_ads-2.8.8/ads/environment/ml_runtime.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/evaluations/__init__.py` & `oracle_ads-2.8.8/ads/evaluations/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/evaluations/evaluation_plot.py` & `oracle_ads-2.8.8/ads/evaluations/evaluation_plot.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/evaluations/evaluator.py` & `oracle_ads-2.8.8/ads/evaluations/evaluator.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/evaluations/statistical_metrics.py` & `oracle_ads-2.8.8/ads/evaluations/statistical_metrics.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/explanations/base_explainer.py` & `oracle_ads-2.8.8/ads/explanations/base_explainer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/explanations/explainer.py` & `oracle_ads-2.8.8/ads/explanations/explainer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/explanations/mlx_global_explainer.py` & `oracle_ads-2.8.8/ads/explanations/mlx_global_explainer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/explanations/mlx_interface.py` & `oracle_ads-2.8.8/ads/explanations/mlx_interface.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/explanations/mlx_local_explainer.py` & `oracle_ads-2.8.8/ads/explanations/mlx_local_explainer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/explanations/mlx_whatif_explainer.py` & `oracle_ads-2.8.8/ads/explanations/mlx_whatif_explainer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/__init__.py` & `oracle_ads-2.8.8/ads/feature_engineering/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/accessor/dataframe_accessor.py` & `oracle_ads-2.8.8/ads/feature_engineering/accessor/dataframe_accessor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/accessor/mixin/correlation.py` & `oracle_ads-2.8.8/ads/feature_engineering/accessor/mixin/correlation.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/accessor/mixin/eda_mixin.py` & `oracle_ads-2.8.8/ads/feature_engineering/accessor/mixin/eda_mixin.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/accessor/mixin/eda_mixin_series.py` & `oracle_ads-2.8.8/ads/feature_engineering/accessor/mixin/eda_mixin_series.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/accessor/mixin/feature_types_mixin.py` & `oracle_ads-2.8.8/ads/feature_engineering/accessor/mixin/feature_types_mixin.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/accessor/mixin/utils.py` & `oracle_ads-2.8.8/ads/feature_engineering/accessor/mixin/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/accessor/series_accessor.py` & `oracle_ads-2.8.8/ads/feature_engineering/accessor/series_accessor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/adsimage/image.py` & `oracle_ads-2.8.8/ads/feature_engineering/adsimage/image.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/adsimage/image_reader.py` & `oracle_ads-2.8.8/ads/feature_engineering/adsimage/image_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/data_schema.json` & `oracle_ads-2.8.8/ads/feature_engineering/data_schema.json`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/dataset/zip_code_data.py` & `oracle_ads-2.8.8/ads/feature_engineering/dataset/zip_code_data.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/exceptions.py` & `oracle_ads-2.8.8/ads/feature_engineering/exceptions.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/__init__.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/address.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/address.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/adsstring/common_regex_mixin.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/adsstring/common_regex_mixin.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/adsstring/oci_language.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/adsstring/oci_language.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/adsstring/parsers/base.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/adsstring/parsers/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/adsstring/parsers/nltk_parser.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/adsstring/parsers/nltk_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/adsstring/parsers/spacy_parser.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/adsstring/parsers/spacy_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/adsstring/string.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/adsstring/string.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/base.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/boolean.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/boolean.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/category.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/category.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/constant.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/constant.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/continuous.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/continuous.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/creditcard.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/creditcard.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/datetime.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/datetime.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/discrete.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/discrete.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/document.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/document.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/gis.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/gis.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/handler/feature_validator.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/handler/feature_validator.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/handler/feature_warning.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/handler/feature_warning.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/handler/warnings.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/handler/warnings.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/integer.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/integer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/ip_address.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/ip_address.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/ip_address_v4.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/ip_address_v4.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/ip_address_v6.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/ip_address_v6.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/lat_long.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/lat_long.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/object.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/object.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/ordinal.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/ordinal.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/phone_number.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/phone_number.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/string.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/string.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/text.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/text.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/unknown.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/unknown.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type/zip_code.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type/zip_code.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/feature_type_manager.py` & `oracle_ads-2.8.8/ads/feature_engineering/feature_type_manager.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/schema.py` & `oracle_ads-2.8.8/ads/feature_engineering/schema.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/feature_engineering/utils.py` & `oracle_ads-2.8.8/ads/feature_engineering/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/hpo/_imports.py` & `oracle_ads-2.8.8/ads/hpo/_imports.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/hpo/ads_search_space.py` & `oracle_ads-2.8.8/ads/hpo/ads_search_space.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/hpo/distributions.py` & `oracle_ads-2.8.8/ads/hpo/distributions.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/hpo/objective.py` & `oracle_ads-2.8.8/ads/hpo/objective.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/hpo/search_cv.py` & `oracle_ads-2.8.8/ads/hpo/search_cv.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/hpo/stopping_criterion.py` & `oracle_ads-2.8.8/ads/hpo/stopping_criterion.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/hpo/tuner_artifact.py` & `oracle_ads-2.8.8/ads/hpo/tuner_artifact.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/hpo/utils.py` & `oracle_ads-2.8.8/ads/hpo/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/hpo/validation.py` & `oracle_ads-2.8.8/ads/hpo/validation.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/hpo/visualization/_contour.py` & `oracle_ads-2.8.8/ads/hpo/visualization/_contour.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/hpo/visualization/_edf.py` & `oracle_ads-2.8.8/ads/hpo/visualization/_edf.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/hpo/visualization/_intermediate_values.py` & `oracle_ads-2.8.8/ads/hpo/visualization/_intermediate_values.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/hpo/visualization/_optimization_history.py` & `oracle_ads-2.8.8/ads/hpo/visualization/_optimization_history.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/hpo/visualization/_parallel_coordinate.py` & `oracle_ads-2.8.8/ads/hpo/visualization/_parallel_coordinate.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/hpo/visualization/_param_importances.py` & `oracle_ads-2.8.8/ads/hpo/visualization/_param_importances.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/jobs/__init__.py` & `oracle_ads-2.8.8/ads/jobs/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8; -*-
 
-# Copyright (c) 2021, 2022 Oracle and/or its affiliates.
+# Copyright (c) 2021, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 
 import logging
 
 logger = logging.getLogger(__name__)
 try:
@@ -13,14 +13,15 @@
         PythonRuntime,
         GitPythonRuntime,
         NotebookRuntime,
         ScriptRuntime,
         DataFlowRuntime,
         DataFlowNotebookRuntime,
     )
+    from ads.jobs.builders.runtimes.pytorch_runtime import PyTorchDistributedRuntime
     from ads.jobs.builders.runtimes.container_runtime import ContainerRuntime
     from ads.jobs.ads_job import Job
     from ads.jobs.builders import infrastructure
     from ads.jobs.builders.infrastructure.dsc_job import (
         DataScienceJob,
         DataScienceJobRun,
     )
@@ -40,12 +41,13 @@
     "DataScienceJob",
     "DataScienceJobRun",
     "PythonRuntime",
     "GitPythonRuntime",
     "NotebookRuntime",
     "ScriptRuntime",
     "ContainerRuntime",
+    "PyTorchDistributedRuntime",
     "DataFlow",
     "DataFlowRun",
     "DataFlowRuntime",
     "DataFlowNotebookRuntime",
 ]
```

### Comparing `oracle_ads-2.8.7/ads/jobs/ads_job.py` & `oracle_ads-2.8.8/ads/jobs/ads_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from urllib.parse import urlparse
 
 import fsspec
 from ads.common.auth import default_signer
 from ads.jobs.builders.base import Builder
 from ads.jobs.builders.infrastructure.dataflow import DataFlow, DataFlowRun
 from ads.jobs.builders.infrastructure.dsc_job import DataScienceJob, DataScienceJobRun
+from ads.jobs.builders.runtimes.pytorch_runtime import PyTorchDistributedRuntime
 from ads.jobs.builders.runtimes.container_runtime import ContainerRuntime
 from ads.jobs.builders.runtimes.python_runtime import (
     DataFlowRuntime,
     GitPythonRuntime,
     NotebookRuntime,
     PythonRuntime,
     Runtime,
@@ -127,14 +128,15 @@
         item().type: item
         for item in [
             PythonRuntime,
             GitPythonRuntime,
             ContainerRuntime,
             ScriptRuntime,
             NotebookRuntime,
+            PyTorchDistributedRuntime,
             DataFlowRuntime,
         ]
     }
 
     @staticmethod
     def from_datascience_job(job_id) -> "Job":
         """Loads a data science job from OCI.
```

### Comparing `oracle_ads-2.8.7/ads/jobs/builders/base.py` & `oracle_ads-2.8.8/ads/jobs/builders/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/jobs/builders/infrastructure/base.py` & `oracle_ads-2.8.8/ads/jobs/builders/infrastructure/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/jobs/builders/infrastructure/dataflow.py` & `oracle_ads-2.8.8/ads/jobs/builders/infrastructure/dataflow.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/jobs/builders/infrastructure/dsc_job.py` & `oracle_ads-2.8.8/ads/jobs/builders/infrastructure/dsc_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,19 @@
     DataScienceJobRuntimeManager,
 )
 from ads.jobs.builders.infrastructure.utils import get_value
 from ads.jobs.builders.runtimes.artifact import Artifact
 from ads.jobs.builders.runtimes.container_runtime import ContainerRuntime
 from ads.jobs.builders.runtimes.python_runtime import GitPythonRuntime
 
-from ads.common.dsc_file_system import OCIFileStorage, DSCFileSystemManager, OCIObjectStorage
+from ads.common.dsc_file_system import (
+    OCIFileStorage,
+    DSCFileSystemManager,
+    OCIObjectStorage,
+)
 
 logger = logging.getLogger(__name__)
 
 SLEEP_INTERVAL = 3
 WAIT_SECONDS_AFTER_FINISHED = 90
 MAXIMUM_MOUNT_COUNT = 5
 FILE_STORAGE_TYPE = "FILE_STORAGE"
@@ -258,18 +262,17 @@
                 logger.debug("Failed to load config from notebook.")
                 logger.debug(traceback.format_exc())
                 # If there is an error loading the notebook infra configurations.
                 # Ignore it by setting nb_session to None
                 # This will skip loading the default configure.
                 nb_session = None
             if nb_session:
-                nb_config = getattr(
-                    nb_session,
-                    "notebook_session_config_details",
-                    getattr(nb_session, "notebook_session_configuration_details", None),
+                nb_config = (
+                    getattr(nb_session, "notebook_session_config_details", None)
+                    or getattr(nb_session, "notebook_session_configuration_details", None)
                 )
 
                 if nb_config:
                     self._load_infra_from_notebook(nb_config)
                 if self.project_id is None:
                     self.project_id = nb_session.project_id
         super().load_properties_from_env()
@@ -1450,19 +1453,22 @@
             dsc_job.job_infrastructure_configuration_details = {}
 
         for snake_attr, camel_attr in attr_map.items():
             value = self.get_spec(snake_attr)
             if value:
                 dsc_job.job_infrastructure_configuration_details[camel_attr] = value
 
-        if (
-            not dsc_job.job_infrastructure_configuration_details.get("shapeName", "").endswith("Flex")
-            and dsc_job.job_infrastructure_configuration_details.get("jobShapeConfigDetails")
+        if not dsc_job.job_infrastructure_configuration_details.get(
+            "shapeName", ""
+        ).endswith("Flex") and dsc_job.job_infrastructure_configuration_details.get(
+            "jobShapeConfigDetails"
         ):
-            raise ValueError("Shape config is not required for non flex shape from user end.")
+            raise ValueError(
+                "Shape config is not required for non flex shape from user end."
+            )
 
         if dsc_job.job_infrastructure_configuration_details.get("subnetId"):
             dsc_job.job_infrastructure_configuration_details[
                 "jobInfrastructureType"
             ] = JobInfrastructureConfigurationDetails.JOB_INFRASTRUCTURE_TYPE_STANDALONE
 
         if self.storage_mount:
@@ -1491,15 +1497,18 @@
         DataScienceJob
             The DataScienceJob instance (self)
         """
         return (
             self.build()
             .with_compartment_id(self.compartment_id or "{Provide a compartment OCID}")
             .with_project_id(self.project_id or "{Provide a project OCID}")
-            .with_subnet_id(self.subnet_id or "{Provide a subnet OCID or remove this field if you use a default networking}")
+            .with_subnet_id(
+                self.subnet_id
+                or "{Provide a subnet OCID or remove this field if you use a default networking}"
+            )
         )
 
     def create(self, runtime, **kwargs) -> DataScienceJob:
         """Creates a job with runtime.
 
         Parameters
         ----------
@@ -1548,15 +1557,15 @@
         self,
         name=None,
         args=None,
         env_var=None,
         freeform_tags=None,
         defined_tags=None,
         wait=False,
-        **kwargs
+        **kwargs,
     ) -> DataScienceJobRun:
         """Runs a job on OCI Data Science job
 
         Parameters
         ----------
         name : str, optional
             The name of the job run, by default None.
@@ -1599,23 +1608,29 @@
 
         if name:
             envs = self.runtime.envs
             if env_var:
                 envs.update(env_var)
             name = Template(name).safe_substitute(envs)
 
-        return self.dsc_job.run(
+        kwargs = dict(
             display_name=name,
             command_line_arguments=args,
             environment_variables=env_var,
             freeform_tags=freeform_tags,
             defined_tags=defined_tags,
             wait=wait,
-            **kwargs
+            **kwargs,
         )
+        # A Runtime class may define customized run() method.
+        # Use the customized method if the run() method is defined by the runtime.
+        # Otherwise, use the default run() method defined in this class.
+        if hasattr(self.runtime, "run"):
+            return self.runtime.run(self.dsc_job, **kwargs)
+        return self.dsc_job.run(**kwargs)
 
     def delete(self) -> None:
         """Deletes a job"""
         self.dsc_job.delete()
 
     def run_list(self, **kwargs) -> List[DataScienceJobRun]:
         """Gets a list of job runs.
```

### Comparing `oracle_ads-2.8.7/ads/jobs/builders/infrastructure/dsc_job_runtime.py` & `oracle_ads-2.8.8/ads/jobs/builders/infrastructure/dsc_job_runtime.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,21 +25,27 @@
     CondaRuntime,
     ScriptRuntime,
     PythonRuntime,
     NotebookRuntime,
     GitPythonRuntime,
 )
 from ads.jobs.builders.runtimes.container_runtime import ContainerRuntime
+from ads.jobs.builders.runtimes.pytorch_runtime import (
+    PyTorchDistributedRuntime,
+    PyTorchDistributedArtifact,
+)
 from ads.jobs.builders.runtimes.artifact import (
     ScriptArtifact,
     NotebookArtifact,
     PythonArtifact,
     GitPythonArtifact,
 )
+from ads.opctl.distributed.common import cluster_config_helper
 from ads.jobs.builders.infrastructure.utils import get_value
+from ads.jobs.templates import driver_utils
 
 
 class IncompatibleRuntime(Exception):  # pragma: no cover
     """Represents an exception when runtime is not compatible with the OCI data science job configuration.
     This exception is designed to be raised during the extraction of a runtime from OCI data science job.
     The data science job does not explicitly contain information of the type of the ADS runtime.
     Each runtime handler should determine if the configuration of the job can be converted to the runtime.
@@ -180,15 +186,15 @@
             ] = runtime.maximum_runtime_in_minutes
         job_configuration_details["environment_variables"] = self._translate_env(
             runtime
         )
         if runtime.args:
             # shlex.join() is not available until python 3.8
             job_configuration_details["command_line_arguments"] = " ".join(
-                shlex.quote(arg) for arg in runtime.get_spec(runtime.CONST_ARGS)
+                shlex.quote(str(arg)) for arg in runtime.get_spec(runtime.CONST_ARGS)
             )
         return job_configuration_details
 
     @staticmethod
     def _translate_specs(
         runtime: Runtime, spec_mappings: dict, delimiter: Optional[str] = None
     ) -> dict:
@@ -649,15 +655,15 @@
         envs = super()._translate_env(runtime)
         envs.update(
             self._translate_specs(runtime, self.SPEC_MAPPINGS, self.PATH_DELIMITER)
         )
 
         if runtime.entrypoint:
             envs[self.CONST_CODE_ENTRYPOINT] = runtime.entrypoint
-        else:
+        elif runtime.script_uri:
             envs[self.CONST_CODE_ENTRYPOINT] = os.path.basename(runtime.script_uri)
 
         envs[self.CONST_JOB_ENTRYPOINT] = PythonArtifact.CONST_DRIVER_SCRIPT
         return envs
 
     def _extract_envs(self, dsc_job) -> dict:
         """Extract the runtime specification from environment variables.
@@ -670,17 +676,21 @@
         Returns
         -------
         dict
             A runtime specification dictionary for initializing a runtime.
         """
         spec = super()._extract_envs(dsc_job)
         envs = spec.pop(PythonRuntime.CONST_ENV_VAR, {})
-        if self.CONST_CODE_ENTRYPOINT not in envs:
+        if (
+            self.__class__ == PythonRuntimeHandler
+            and self.CONST_CODE_ENTRYPOINT not in envs
+        ):
             raise IncompatibleRuntime()
-        envs.pop(PythonRuntimeHandler.CONST_JOB_ENTRYPOINT)
+        # PyTorchDistributedRuntime does not require entrypoint.
+        envs.pop(PythonRuntimeHandler.CONST_JOB_ENTRYPOINT, None)
         spec.update(self._extract_specs(envs, self.SPEC_MAPPINGS))
         if PythonRuntime.CONST_PYTHON_PATH in spec:
             spec[PythonRuntime.CONST_PYTHON_PATH] = spec[
                 PythonRuntime.CONST_PYTHON_PATH
             ].split(self.PATH_DELIMITER)
         if envs:
             spec[PythonRuntime.CONST_ENV_VAR] = envs
@@ -1031,25 +1041,118 @@
         if entrypoint:
             spec[ContainerRuntime.CONST_ENTRYPOINT] = entrypoint
         if envs:
             spec[ContainerRuntime.CONST_ENV_VAR] = envs
         return spec
 
 
+class PyTorchDistributedRuntimeHandler(PythonRuntimeHandler):
+    RUNTIME_CLASS = PyTorchDistributedRuntime
+    CONST_WORKER_COUNT = "OCI__WORKER_COUNT"
+    CONST_COMMAND = "OCI__LAUNCH_CMD"
+    CONST_DEEPSPEED = "OCI__DEEPSPEED"
+
+    GIT_SPEC_MAPPINGS = {
+        cluster_config_helper.OCI__RUNTIME_URI: GitPythonRuntime.CONST_GIT_URL,
+        cluster_config_helper.OCI__RUNTIME_GIT_BRANCH: GitPythonRuntime.CONST_BRANCH,
+        cluster_config_helper.OCI__RUNTIME_GIT_COMMIT: GitPythonRuntime.CONST_COMMIT,
+        cluster_config_helper.OCI__RUNTIME_GIT_SECRET_ID: GitPythonRuntime.CONST_GIT_SSH_SECRET_ID,
+    }
+
+    SPEC_MAPPINGS = PythonRuntimeHandler.SPEC_MAPPINGS
+    SPEC_MAPPINGS.update(
+        {
+            PyTorchDistributedRuntime.CONST_COMMAND: CONST_COMMAND,
+        }
+    )
+
+    def _translate_artifact(self, runtime: PyTorchDistributedRuntime):
+        return PyTorchDistributedArtifact(runtime.source_uri, runtime)
+
+    def _translate_env(self, runtime: PyTorchDistributedRuntime) -> dict:
+        envs = super()._translate_env(runtime)
+        replica = runtime.replica if runtime.replica else 1
+        # WORKER_COUNT = REPLICA - 1 so that it will be same as distributed training
+        envs[self.CONST_WORKER_COUNT] = str(replica - 1)
+        envs[self.CONST_JOB_ENTRYPOINT] = PyTorchDistributedArtifact.CONST_DRIVER_SCRIPT
+        if runtime.inputs:
+            envs[driver_utils.CONST_ENV_INPUT_MAPPINGS] = json.dumps(runtime.inputs)
+        if runtime.git:
+            for env_key, spec_key in self.GIT_SPEC_MAPPINGS.items():
+                if not runtime.git.get(spec_key):
+                    continue
+                envs[env_key] = runtime.git[spec_key]
+        if runtime.dependencies:
+            if PyTorchDistributedRuntime.CONST_PIP_PKG in runtime.dependencies:
+                envs[driver_utils.CONST_ENV_PIP_PKG] = runtime.dependencies[
+                    PyTorchDistributedRuntime.CONST_PIP_PKG
+                ]
+            if PyTorchDistributedRuntime.CONST_PIP_REQ in runtime.dependencies:
+                envs[driver_utils.CONST_ENV_PIP_REQ] = runtime.dependencies[
+                    PyTorchDistributedRuntime.CONST_PIP_REQ
+                ]
+        if runtime.use_deepspeed:
+            envs[self.CONST_DEEPSPEED] = "1"
+        return envs
+
+    def _extract_envs(self, dsc_job) -> dict:
+        spec = super()._extract_envs(dsc_job)
+        envs = spec.pop(PythonRuntime.CONST_ENV_VAR, {})
+        if self.CONST_WORKER_COUNT not in envs:
+            raise IncompatibleRuntime()
+        # Replicas
+        spec[PyTorchDistributedRuntime.CONST_REPLICA] = (
+            int(envs.pop(self.CONST_WORKER_COUNT)) + 1
+        )
+        # Git
+        if cluster_config_helper.OCI__RUNTIME_URI in envs:
+            git_spec = {}
+            for env_key, spec_key in self.GIT_SPEC_MAPPINGS.items():
+                if env_key in envs:
+                    git_spec[spec_key] = envs.pop(env_key)
+            spec[PyTorchDistributedRuntime.CONST_GIT] = git_spec
+        # Inputs
+        input_mappings = envs.pop(driver_utils.CONST_ENV_INPUT_MAPPINGS, None)
+        if input_mappings:
+            try:
+                spec[PyTorchDistributedRuntime.CONST_INPUT] = json.loads(input_mappings)
+            except ValueError:
+                spec[PyTorchDistributedRuntime.CONST_INPUT] = input_mappings
+        # Dependencies
+        dep = {}
+        if driver_utils.CONST_ENV_PIP_PKG in envs:
+            dep[PyTorchDistributedRuntime.CONST_PIP_PKG] = envs.pop(
+                driver_utils.CONST_ENV_PIP_PKG
+            )
+        if driver_utils.CONST_ENV_PIP_REQ in envs:
+            dep[PyTorchDistributedRuntime.CONST_PIP_REQ] = envs.pop(
+                driver_utils.CONST_ENV_PIP_REQ
+            )
+        if dep:
+            spec[PyTorchDistributedRuntime.CONST_DEP] = dep
+        if envs.pop(self.CONST_DEEPSPEED, None):
+            spec[PyTorchDistributedRuntime.CONST_DEEPSPEED] = True
+        # Envs
+        if envs:
+            spec[PythonRuntime.CONST_ENV_VAR] = envs
+        return spec
+
+
 class DataScienceJobRuntimeManager(RuntimeHandler):
     """This class is used by the DataScienceJob infrastructure to handle the runtime conversion.
     The translate() method determines the actual runtime handler by matching the RUNTIME_CLASS.
     The extract() method determines the actual runtime handler by checking if the runtime can be extracted.
     The order in runtime_handlers is used for extraction until a runtime is extracted.
     RuntimeHandler on the top of the list will have higher priority.
     If a runtime is a specify case of another runtime, the handler should be placed with higher priority.
     """
 
     runtime_handlers = [
         ContainerRuntimeHandler,
+        PyTorchDistributedRuntimeHandler,
         GitPythonRuntimeHandler,
         NotebookRuntimeHandler,
         PythonRuntimeHandler,
         ScriptRuntimeHandler,
     ]
 
     def translate(self, runtime) -> dict:
```

### Comparing `oracle_ads-2.8.7/ads/jobs/builders/infrastructure/utils.py` & `oracle_ads-2.8.8/ads/jobs/builders/infrastructure/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/jobs/builders/runtimes/artifact.py` & `oracle_ads-2.8.8/ads/jobs/builders/runtimes/artifact.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 # Copyright (c) 2021, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 import contextlib
 import logging
 import os
 import shutil
 import tempfile
-import zipfile
 from io import DEFAULT_BUFFER_SIZE
 from urllib import request
 from urllib.parse import urlparse
 
 import fsspec
 from ads.common.auth import default_signer
 
@@ -37,15 +36,15 @@
     """
 
     CONST_DRIVER_UTILS = "driver_utils.py"
     CONST_DRIVER_NOTEBOOK = "driver_notebook.py"
 
     def __init__(self, source, runtime=None) -> None:
         # Get the full path of source file if it is local file.
-        if not urlparse(source).scheme:
+        if source and not urlparse(source).scheme:
             self.source = os.path.abspath(os.path.expanduser(source))
         else:
             self.source = source
         self.path = None
         self.temp_dir = None
         self.runtime = runtime
 
@@ -199,29 +198,35 @@
         self.path = source
 
 
 class PythonArtifact(Artifact):
     """Represents a PythonRuntime job artifact"""
 
     CONST_DRIVER_SCRIPT = "driver_python.py"
+    DEFAULT_BASENAME = "artifact"
     # The directory to store user code
     # This directory must match the USER_CODE_DIR in driver_python.py
     USER_CODE_DIR = "code"
 
     def __init__(self, source, runtime=None) -> None:
         super().__init__(source, runtime)
         self.basename = None
         self.artifact_dir = None
         self.code_dir = None
 
     def _copy_artifacts(self, drivers=None):
         """Copies the drivers and artifacts to the temp artifact dir."""
         # The basename of the job artifact,
         # this will be the name of the zip file uploading to OCI
-        self.basename = os.path.basename(str(self.source).rstrip("/")).split(".", 1)[0]
+        if self.source:
+            self.basename = os.path.basename(str(self.source).rstrip("/")).split(
+                ".", 1
+            )[0]
+        else:
+            self.basename = self.DEFAULT_BASENAME
         # The temp dir path for storing the artifacts, including drivers and user code
         self.artifact_dir = os.path.join(self.temp_dir.name, self.basename)
         # The temp dir path for storing the user code
         self.code_dir = os.path.join(self.artifact_dir, self.USER_CODE_DIR)
         os.makedirs(self.artifact_dir, exist_ok=True)
 
         if not drivers:
@@ -232,16 +237,17 @@
             file_path = os.path.join(
                 os.path.dirname(__file__), "../../templates", filename
             )
 
             shutil.copy(file_path, os.path.join(self.artifact_dir, filename))
 
         # Copy user code
-        os.makedirs(self.code_dir, exist_ok=True)
-        Artifact.copy_from_uri(self.source, self.code_dir, unpack=True)
+        if self.source:
+            os.makedirs(self.code_dir, exist_ok=True)
+            Artifact.copy_from_uri(self.source, self.code_dir, unpack=True)
 
     def _zip_artifacts(self):
         """Create a zip file from the temp artifact dir."""
         output = os.path.join(self.temp_dir.name, self.basename)
         shutil.make_archive(output, "zip", self.artifact_dir, base_dir="./")
         return output + ".zip"
 
@@ -308,15 +314,14 @@
                     + "the notebook path is relative to the root of the source."
                 )
         # Zip the job artifact
         self.path = self._zip_artifacts()
 
 
 class GitPythonArtifact(Artifact):
-
     CONST_DRIVER_SCRIPT = "driver_oci.py"
 
     def __init__(self) -> None:
         super().__init__("", runtime=None)
 
     def build(self):
         """Prepares job artifact for GitPythonRuntime."""
```

### Comparing `oracle_ads-2.8.7/ads/jobs/builders/runtimes/base.py` & `oracle_ads-2.8.8/ads/jobs/builders/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/jobs/builders/runtimes/container_runtime.py` & `oracle_ads-2.8.8/ads/jobs/builders/runtimes/container_runtime.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/jobs/builders/runtimes/python_runtime.py` & `oracle_ads-2.8.8/ads/jobs/builders/runtimes/python_runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
             # Specify the service conda environment by slug name.
             .with_service_conda("pytorch110_p38_cpu_v1")
             # The job artifact can be a single Python script, a directory or a zip file.
             .with_source("local/path/to/code_dir")
             # Environment variable
             .with_environment_variable(NAME="Welcome to OCI Data Science.")
             # Command line argument
-            .with_argument("100 linux \"hi there\"")
+            .with_argument("100 linux 'hi there'")
             # The entrypoint is applicable only to directory or zip file as source
             # The entrypoint should be a path relative to the working dir.
             # Here my_script.sh is a file in the code_dir/my_package directory
             .with_entrypoint("my_package/my_script.sh")
         )
```

### Comparing `oracle_ads-2.8.7/ads/jobs/cli.py` & `oracle_ads-2.8.8/ads/jobs/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/jobs/env_var_parser.py` & `oracle_ads-2.8.8/ads/jobs/env_var_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/jobs/extension.py` & `oracle_ads-2.8.8/ads/jobs/extension.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/jobs/schema/infrastructure_schema.json` & `oracle_ads-2.8.8/ads/jobs/schema/infrastructure_schema.json`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/jobs/schema/job_schema.json` & `oracle_ads-2.8.8/ads/jobs/schema/job_schema.json`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/jobs/schema/runtime_schema.json` & `oracle_ads-2.8.8/ads/jobs/schema/runtime_schema.json`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/jobs/schema/validator.py` & `oracle_ads-2.8.8/ads/jobs/schema/validator.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/jobs/serializer.py` & `oracle_ads-2.8.8/ads/jobs/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import json
 from abc import ABC, abstractmethod
 from typing import Type, TypeVar, Union, Dict
 from urllib.parse import urlparse
 
 import fsspec
 import yaml
+from ads.common.auth import default_signer
 
 Self = TypeVar("Self", bound="Serializable")
 """Special type to represent the current enclosed class.
 
 This type is used by factory class method or when a method returns ``self``.
 """
 
@@ -84,14 +85,22 @@
             The URI of the file.
 
         Returns
         -------
         str
             The content of the file as a string.
         """
+        # Add default signer if the uri is an object storage uri, and
+        # the user does not specify config or signer.
+        if (
+            uri.startswith("oci://")
+            and "config" not in kwargs
+            and "signer" not in kwargs
+        ):
+            kwargs.update(default_signer())
         with fsspec.open(uri, "r", **kwargs) as f:
             return f.read()
 
     def to_json(
         self, uri: str = None, encoder: callable = json.JSONEncoder, **kwargs
     ) -> str:
         """Returns the object serialized as a JSON string
@@ -123,15 +132,15 @@
 
     @classmethod
     def from_json(
         cls: Type[Self],
         json_string: str = None,
         uri: str = None,
         decoder: callable = json.JSONDecoder,
-        **kwargs
+        **kwargs,
     ) -> Self:
         """Creates an object from JSON string provided or from URI location containing JSON string
 
         Args:
             json_string (string, optional): JSON string. Defaults to None.
             uri (string, optional): URI location of file containing JSON string. Defaults to None.
             decoder (callable, optional): Custom decoder. Defaults to simple JSON decoder.
@@ -212,15 +221,15 @@
 
     @classmethod
     def from_yaml(
         cls: Type[Self],
         yaml_string: str = None,
         uri: str = None,
         loader: callable = yaml.SafeLoader,
-        **kwargs
+        **kwargs,
     ) -> Self:
         """Initializes an object from YAML string or URI location containing the YAML
 
         Parameters
         ----------
         yaml_string : str, optional
             YAML string, by default None
@@ -248,15 +257,15 @@
 
     @classmethod
     def from_string(
         cls: Type[Self],
         obj_string: str = None,
         uri: str = None,
         loader: callable = yaml.SafeLoader,
-        **kwargs
+        **kwargs,
     ) -> Self:
         """Initializes an object from YAML/JSON string or URI location containing the YAML/JSON
 
         Parameters
         ----------
         obj_string : str, optional
             YAML/JSON string, by default None
```

### Comparing `oracle_ads-2.8.7/ads/jobs/templates/driver_notebook.py` & `oracle_ads-2.8.8/ads/jobs/templates/driver_notebook.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/jobs/templates/driver_oci.py` & `oracle_ads-2.8.8/ads/jobs/templates/driver_oci.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,14 @@
 """
 import base64
 import logging
 import os
 import random
 import shutil
 import string
-import sys
 import traceback
 import uuid
 from time import sleep, time
 from typing import Optional
 from urllib.parse import urlparse
 from urllib.request import getproxies
```

### Comparing `oracle_ads-2.8.7/ads/jobs/templates/driver_python.py` & `oracle_ads-2.8.8/ads/jobs/templates/driver_python.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/jobs/templates/driver_utils.py` & `oracle_ads-2.8.8/ads/jobs/templates/driver_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 #!/usr/bin/env python
 # -*- coding: utf-8; -*-
 
 # Copyright (c) 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
+import contextlib
 import importlib
 import json
 import logging
 import os
 import runpy
 import shlex
 import stat
 import subprocess
 import sys
 import time
 import traceback
-from typing import List, Optional, Any
+from io import DEFAULT_BUFFER_SIZE
+from typing import List, Optional
+from urllib import request
 from urllib.parse import urlparse
 
 
 import oci
 
 
 CONST_ENV_LOG_LEVEL = "OCI_LOG_LEVEL"
@@ -28,14 +31,17 @@
 CONST_ENV_PYTHON_PATH = "PYTHON_PATH"
 CONST_ENV_ENTRYPOINT = "CODE_ENTRYPOINT"
 CONST_ENV_ENTRY_FUNC = "ENTRY_FUNCTION"
 CONST_ENV_OUTPUT_DIR = "OUTPUT_DIR"
 CONST_ENV_OUTPUT_URI = "OUTPUT_URI"
 CONST_ENV_OCI_RP = "OCI_RESOURCE_PRINCIPAL_VERSION"
 CONST_ENV_ADS_IAM = "OCI_IAM_TYPE"
+CONST_ENV_INPUT_MAPPINGS = "OCI__INPUT_MAPPINGS"
+CONST_ENV_PIP_REQ = "OCI__PIP_REQUIREMENTS"
+CONST_ENV_PIP_PKG = "OCI__PIP_PKG"
 CONST_API_KEY = "api_key"
 
 
 DEFAULT_CODE_DIR = os.path.join(
     os.path.dirname(os.path.abspath(__file__)),
     os.environ.get(CONST_ENV_CODE_DIR, "code"),
 )
@@ -229,14 +235,70 @@
             return
 
         prefix = parsed.path
         return OCIHelper.copy_to_oci_object_storage(
             output_dir, namespace, bucket, prefix
         )
 
+    @staticmethod
+    def _download_with_urlopen(src, dest):
+        url_response = request.urlopen(src)
+        with contextlib.closing(url_response) as f:
+            logger.debug("Downloading from %s", src)
+            with open(dest, "wb") as out_file:
+                block_size = DEFAULT_BUFFER_SIZE * 8
+                while True:
+                    block = f.read(block_size)
+                    if not block:
+                        break
+                    out_file.write(block)
+
+    @staticmethod
+    def _download_with_fsspec(src, dest):
+        import fsspec
+
+        scheme = urlparse(src).scheme
+        fs = fsspec.filesystem(scheme)
+        fs.get(
+            src,
+            dest,
+            recursive=True,
+            callback=fsspec.callbacks.TqdmCallback(),
+        )
+
+    @staticmethod
+    def copy_inputs(mappings: dict = None):
+        if not mappings and CONST_ENV_INPUT_MAPPINGS in os.environ:
+            mappings = json.loads(os.environ[CONST_ENV_INPUT_MAPPINGS])
+            logger.debug("Inputs specified from ENV: %s", mappings)
+
+        if not mappings:
+            logger.debug("No inputs specified.")
+            return
+
+        for src, dest in mappings.items():
+            logger.debug("Copying %s to %s", src, dest)
+            # Create the dest dir if one does not exist.
+            if str(dest).endswith("/"):
+                dest_dir = dest
+            else:
+                dest_dir = os.path.dirname(dest)
+
+            # Do not make dirs if user is using cwd.
+            if dest_dir:
+                os.makedirs(dest_dir, exist_ok=True)
+
+            # Use native Python to download http/ftp.
+            scheme = urlparse(src).scheme
+            if scheme in ["http", "https", "ftp"]:
+                OCIHelper._download_with_urlopen(src, dest)
+            else:
+                OCIHelper._download_with_fsspec(src, dest)
+        return
+
 
 class ArgumentParser:
     """Contains methods for parsing arguments for entry function."""
 
     def __init__(self, argument_list: list) -> None:
         """Initialize the parser with a list of arguments
 
@@ -283,43 +345,46 @@
         Parameters
         ----------
         code_dir : str
             The path to the directory containing the user code.
         """
         logger.info("Job Run ID is: %s", os.environ.get(CONST_ENV_JOB_RUN_OCID))
         self.code_dir = code_dir
+        self.conda_prefix = sys.executable.split("/bin/python", 1)[0]
 
     @staticmethod
     def run_command(
-        command: str, activate_conda: bool = False, level: Optional[int] = None
+        command: str, conda_prefix: str = None, level: Optional[int] = None, check=False
     ) -> int:
         """Runs a shell command and logs the outputs with specific log level.
 
         Parameters
         ----------
         command : str
             The shell command
-        activate_conda : bool, optional
-            Indicate if conda environment should be activated for running the command, by default False
+        conda_prefix : str, optional
+            Prefix of the conda environment for running the command.
+            Defaults to None.
         level : int, optional
             Logging level for the command outputs, by default None.
             If this is set to a log level from logging, e.g. logging.DEBUG,
             the command outputs will be logged with the level.
             If this is None, the command outputs will be printed.
 
         Returns
         -------
         int
             The return code of the command.
         """
-        logger.debug(">>> %s", command)
-        if activate_conda:
+        # Add a small time delay so the existing outputs will not intersect with the command outputs.
+        time.sleep(0.05)
+        logger.info(">>> %s", command)
+        if conda_prefix:
             # Conda activate
             # https://docs.conda.io/projects/conda/en/latest/release-notes.html#id241
-            conda_prefix = sys.executable.split("/bin/python", 1)[0]
             cmd = (
                 "CONDA_BASE=$(conda info --base) && "
                 + "source $CONDA_BASE/etc/profile.d/conda.sh && "
                 + f"conda activate {conda_prefix}; "
                 + command
             )
         else:
@@ -339,25 +404,53 @@
             if output:
                 msg = output.decode()
                 if level is None:
                     # output already contains the line break
                     print(msg, flush=True, end="")
                 else:
                     # logging will flush outputs by default
+                    # logging will add line break
+                    msg = msg.rstrip("\n")
                     logger.log(level=level, msg=msg)
             # Add a small delay so that
             # outputs from the subsequent code will have different timestamp for oci logging
             time.sleep(0.05)
+        if check and process.returncode != 0:
+            # If there is an error, exit the main process with the same return code.
+            sys.exit(process.returncode)
         return process.returncode
 
     def conda_unpack(self):
         if self.run_command("conda-unpack", level=logging.DEBUG):
             logger.info("conda-unpack exits with non-zero return code.")
         return self
 
+    def install_pip_requirements(self, req_path: str = None):
+        if not req_path:
+            req_path = os.environ.get(CONST_ENV_PIP_REQ)
+        if not req_path:
+            return self
+        self.run_command(
+            f"pip install -r {req_path}", conda_prefix=self.conda_prefix, check=True
+        )
+        return self
+
+    def install_pip_packages(self, packages: str = None):
+        if not packages:
+            packages = os.environ.get(CONST_ENV_PIP_PKG)
+        if not packages:
+            return self
+        self.run_command(
+            f"pip install {packages}", conda_prefix=self.conda_prefix, check=True
+        )
+        return self
+
+    def install_dependencies(self):
+        return self.install_pip_requirements().install_pip_packages()
+
     def set_working_dir(self, working_dir: str = os.environ.get(CONST_ENV_WORKING_DIR)):
         """Sets the working directory for the job run.
 
         Parameters
         ----------
         working_dir : str, optional
             Working directory, by default os.environ.get("WORKING_DIR")
@@ -366,17 +459,19 @@
 
         """
         if working_dir:
             working_dir = os.path.join(self.code_dir, working_dir)
         else:
             working_dir = self.code_dir
         os.chdir(working_dir)
+        logger.debug("Working directory set to %s", working_dir)
         # Add working dir to sys.path
         if working_dir not in sys.path:
             sys.path.append(working_dir)
+            logger.debug("Added %s to sys.path", working_dir)
         return self
 
     def setup_python_path(
         self, python_path: str = os.environ.get(CONST_ENV_PYTHON_PATH, "")
     ):
         """Adds additional python paths.
         Relative paths are expanded based on the current working directory.
@@ -394,14 +489,15 @@
             return self
         path_list = python_path.split(os.pathsep)
         path_list.append(self.code_dir)
         for path in path_list:
             abs_path = os.path.abspath(os.path.expanduser(path))
             if abs_path not in sys.path:
                 sys.path.append(abs_path)
+                logger.debug("Added %s to sys.path", abs_path)
         logger.debug("Python Path: %s", sys.path)
         return self
 
     def _run_function(self, module_path: str, entry_function: str, argv: list):
         """Runs the entry function in module specified by module path.
 
         Parameters
@@ -451,15 +547,15 @@
                     os.chmod(entrypoint, st.st_mode | stat.S_IEXEC)
                 except Exception:
                     # Ignore any error here and continue to try to run the script.
                     # Show the exception for debugging
                     logger.debug(traceback.format_exc())
             # Run the entrypoint as shell command with conda activated
             cmd = shlex.join([entrypoint] + sys.argv[1:])
-            return_code = self.run_command(cmd, activate_conda=True)
+            return_code = self.run_command(cmd, conda_prefix=self.conda_prefix)
             # Exit the job run with the same return code if it is non-zero.
             if return_code:
                 logger.error("CMD exited with return code %s.", return_code)
                 sys.exit(return_code)
 
     def run(
         self,
@@ -495,12 +591,14 @@
             logger.info("Running notebook: %s", entrypoint)
             # Exclude tags
             tags = os.environ.get("NOTEBOOK_EXCLUDE_TAGS")
             if tags:
                 tags = json.loads(tags)
                 logger.info("Excluding cells with any of the following tags: %s", tags)
             # Pass in the absolute path to make sure the working dir is notebook directory
-            run_notebook(os.path.abspath(os.path.expanduser(entrypoint)), exclude_tags=tags)
+            run_notebook(
+                os.path.abspath(os.path.expanduser(entrypoint)), exclude_tags=tags
+            )
         else:
             self._run_script(entrypoint_abs_path)
         logger.info("Job run completed.")
         return self
```

### Comparing `oracle_ads-2.8.7/ads/jobs/utils.py` & `oracle_ads-2.8.8/ads/jobs/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/__init__.py` & `oracle_ads-2.8.8/ads/model/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/artifact.py` & `oracle_ads-2.8.8/ads/model/artifact.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/artifact_downloader.py` & `oracle_ads-2.8.8/ads/model/artifact_downloader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/artifact_uploader.py` & `oracle_ads-2.8.8/ads/model/artifact_uploader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/base_properties.py` & `oracle_ads-2.8.8/ads/model/base_properties.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/common/.model-ignore` & `oracle_ads-2.8.8/ads/model/common/.model-ignore`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/common/utils.py` & `oracle_ads-2.8.8/ads/model/common/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/datascience_model.py` & `oracle_ads-2.8.8/ads/model/datascience_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/deployment/__init__.py` & `oracle_ads-2.8.8/ads/model/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/deployment/common/utils.py` & `oracle_ads-2.8.8/ads/model/deployment/common/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/deployment/model_deployer.py` & `oracle_ads-2.8.8/ads/model/deployment/model_deployer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/deployment/model_deployment.py` & `oracle_ads-2.8.8/ads/model/deployment/model_deployment.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,19 @@
 )
 from ads.config import COMPARTMENT_OCID, PROJECT_OCID
 from ads.jobs.builders.base import Builder
 from ads.jobs.builders.infrastructure.utils import get_value
 from ads.model.common.utils import _is_json_serializable
 from ads.model.deployment.common.utils import send_request
 from ads.model.deployment.model_deployment_infrastructure import (
+    DEFAULT_BANDWIDTH_MBPS,
+    DEFAULT_REPLICA,
+    DEFAULT_SHAPE_NAME,
+    DEFAULT_OCPUS,
+    DEFAULT_MEMORY_IN_GBS,
     MODEL_DEPLOYMENT_INFRASTRUCTURE_TYPE,
     ModelDeploymentInfrastructure,
 )
 from ads.model.deployment.model_deployment_runtime import (
     ModelDeploymentCondaRuntime,
     ModelDeploymentContainerRuntime,
     ModelDeploymentRuntime,
@@ -60,20 +65,14 @@
 DEFAULT_RETRYING_REQUEST_ATTEMPTS = 3
 TERMINAL_STATES = [State.ACTIVE, State.FAILED, State.DELETED, State.INACTIVE]
 
 MODEL_DEPLOYMENT_KIND = "deployment"
 MODEL_DEPLOYMENT_TYPE = "modelDeployment"
 MODEL_DEPLOYMENT_INFERENCE_SERVER_TRITON = "TRITON"
 
-MODEL_DEPLOYMENT_INSTANCE_SHAPE = "VM.Standard.E4.Flex"
-MODEL_DEPLOYMENT_INSTANCE_OCPUS = 1
-MODEL_DEPLOYMENT_INSTANCE_MEMORY_IN_GBS = 16
-MODEL_DEPLOYMENT_INSTANCE_COUNT = 1
-MODEL_DEPLOYMENT_BANDWIDTH_MBPS = 10
-
 MODEL_DEPLOYMENT_RUNTIMES = {
     ModelDeploymentRuntimeType.CONDA: ModelDeploymentCondaRuntime,
     ModelDeploymentRuntimeType.CONTAINER: ModelDeploymentContainerRuntime,
 }
 
 
 class ModelDeploymentLogType:
@@ -1597,43 +1596,43 @@
             Dict contains model deployment configuration details.
         """
         infrastructure = self.infrastructure
         runtime = self.runtime
 
         instance_configuration = {
             infrastructure.CONST_INSTANCE_SHAPE_NAME: infrastructure.shape_name
-            or MODEL_DEPLOYMENT_INSTANCE_SHAPE,
+            or DEFAULT_SHAPE_NAME,
         }
 
         if instance_configuration[infrastructure.CONST_INSTANCE_SHAPE_NAME].endswith(
             "Flex"
         ):
             instance_configuration[
                 infrastructure.CONST_MODEL_DEPLOYMENT_INSTANCE_SHAPE_CONFIG_DETAILS
             ] = {
                 infrastructure.CONST_OCPUS: infrastructure.shape_config_details.get(
                     "ocpus", None
                 )
-                or MODEL_DEPLOYMENT_INSTANCE_OCPUS,
+                or DEFAULT_OCPUS,
                 infrastructure.CONST_MEMORY_IN_GBS: infrastructure.shape_config_details.get(
                     "memory_in_gbs", None
                 )
                 or infrastructure.shape_config_details.get(
                     "memoryInGBs", None
                 )
-                or MODEL_DEPLOYMENT_INSTANCE_MEMORY_IN_GBS,
+                or DEFAULT_MEMORY_IN_GBS,
             }
 
         if infrastructure.subnet_id:
             instance_configuration[infrastructure.CONST_SUBNET_ID] = infrastructure.subnet_id
 
         scaling_policy = {
             infrastructure.CONST_POLICY_TYPE: "FIXED_SIZE",
             infrastructure.CONST_INSTANCE_COUNT: infrastructure.replica
-            or MODEL_DEPLOYMENT_INSTANCE_COUNT,
+            or DEFAULT_REPLICA,
         }
 
         if not runtime.model_uri:
             raise ValueError(
                 "Missing parameter model uri. Try reruning it after model uri is configured."
             )
 
@@ -1656,15 +1655,15 @@
                 remove_existing_artifact=runtime.remove_existing_artifact,
                 timeout=runtime.timeout
             )
             model_id = dsc_model.id
 
         model_configuration_details = {
             infrastructure.CONST_BANDWIDTH_MBPS: infrastructure.bandwidth_mbps
-            or MODEL_DEPLOYMENT_BANDWIDTH_MBPS,
+            or DEFAULT_BANDWIDTH_MBPS,
             infrastructure.CONST_INSTANCE_CONFIG: instance_configuration,
             runtime.CONST_MODEL_ID: model_id,
             infrastructure.CONST_SCALING_POLICY: scaling_policy,
         }
 
         if runtime.env:
             if not hasattr(
```

### Comparing `oracle_ads-2.8.7/ads/model/deployment/model_deployment_infrastructure.py` & `oracle_ads-2.8.8/ads/model/deployment/model_deployment_infrastructure.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 
 MODEL_DEPLOYMENT_INFRASTRUCTURE_TYPE = "datascienceModelDeployment"
 MODEL_DEPLOYMENT_INFRASTRUCTURE_KIND = "infrastructure"
 
 DEFAULT_BANDWIDTH_MBPS = 10
 DEFAULT_WEB_CONCURRENCY = 10
 DEFAULT_REPLICA = 1
-DEFAULT_SHAPE_NAME = "VM.Standard.E2.4"
+DEFAULT_SHAPE_NAME = "VM.Standard.E4.Flex"
+DEFAULT_OCPUS = 1
+DEFAULT_MEMORY_IN_GBS = 16
 
 logger = logging.getLogger(__name__)
 
 
 class ModelDeploymentInfrastructure(Builder):
     """A class used to represent a Model Deployment Infrastructure.
 
@@ -219,32 +221,36 @@
         defaults[self.CONST_BANDWIDTH_MBPS] = DEFAULT_BANDWIDTH_MBPS
         defaults[self.CONST_WEB_CONCURRENCY] = DEFAULT_WEB_CONCURRENCY
         defaults[self.CONST_REPLICA] = DEFAULT_REPLICA
 
         if NB_SESSION_OCID:
             try:
                 nb_session = DSCNotebookSession.from_ocid(NB_SESSION_OCID)
-                nb_config = nb_session.notebook_session_configuration_details
+            except Exception as e:
+                logger.warning(
+                    f"Error fetching details about Notebook "
+                    f"session: {NB_SESSION_OCID}. {e}"
+                )
+                logger.debug(traceback.format_exc())
+
+            nb_config = (
+                getattr(nb_session, "notebook_session_config_details", None)
+                or getattr(nb_session, "notebook_session_configuration_details", None)
+            )
+            if nb_config:
                 defaults[self.CONST_SHAPE_NAME] = nb_config.shape
 
                 if nb_config.notebook_session_shape_config_details:
                     notebook_shape_config_details = oci_util.to_dict(
                         nb_config.notebook_session_shape_config_details
                     )
                     defaults[self.CONST_SHAPE_CONFIG_DETAILS] = copy.deepcopy(
                         notebook_shape_config_details
                     )
 
-            except Exception as e:
-                logger.warning(
-                    f"Error fetching details about Notebook "
-                    f"session: {NB_SESSION_OCID}. {e}"
-                )
-                logger.debug(traceback.format_exc())
-
         return defaults
 
     @property
     def kind(self) -> str:
         """The kind of the object as showing in YAML.
 
         Returns
@@ -621,8 +627,12 @@
             self.build()
             .with_compartment_id(self.compartment_id or "{Provide a compartment OCID}")
             .with_project_id(self.project_id or "{Provide a project OCID}")
             .with_bandwidth_mbps(self.bandwidth_mbps or DEFAULT_BANDWIDTH_MBPS)
             .with_web_concurrency(self.web_concurrency or DEFAULT_WEB_CONCURRENCY)
             .with_replica(self.replica or DEFAULT_REPLICA)
             .with_shape_name(self.shape_name or DEFAULT_SHAPE_NAME)
+            .with_shape_config_details(
+                ocpus=self.shape_config_details.get(self.CONST_OCPUS, DEFAULT_OCPUS),
+                memory_in_gbs=self.shape_config_details.get(self.CONST_MEMORY_IN_GBS, DEFAULT_MEMORY_IN_GBS)
+            )
         )
```

### Comparing `oracle_ads-2.8.7/ads/model/deployment/model_deployment_properties.py` & `oracle_ads-2.8.8/ads/model/deployment/model_deployment_properties.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/deployment/model_deployment_runtime.py` & `oracle_ads-2.8.8/ads/model/deployment/model_deployment_runtime.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/extractor/automl_extractor.py` & `oracle_ads-2.8.8/ads/model/extractor/automl_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/extractor/huggingface_extractor.py` & `oracle_ads-2.8.8/ads/model/extractor/huggingface_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/extractor/keras_extractor.py` & `oracle_ads-2.8.8/ads/model/extractor/keras_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/extractor/lightgbm_extractor.py` & `oracle_ads-2.8.8/ads/model/extractor/lightgbm_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/extractor/model_info_extractor.py` & `oracle_ads-2.8.8/ads/model/extractor/model_info_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/extractor/model_info_extractor_factory.py` & `oracle_ads-2.8.8/ads/model/extractor/model_info_extractor_factory.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/extractor/pytorch_extractor.py` & `oracle_ads-2.8.8/ads/model/extractor/pytorch_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/extractor/sklearn_extractor.py` & `oracle_ads-2.8.8/ads/model/extractor/sklearn_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/extractor/spark_extractor.py` & `oracle_ads-2.8.8/ads/model/extractor/spark_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/extractor/tensorflow_extractor.py` & `oracle_ads-2.8.8/ads/model/extractor/tensorflow_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/extractor/xgboost_extractor.py` & `oracle_ads-2.8.8/ads/model/extractor/xgboost_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/framework/automl_model.py` & `oracle_ads-2.8.8/ads/model/framework/automl_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/framework/huggingface_model.py` & `oracle_ads-2.8.8/ads/model/framework/huggingface_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/framework/lightgbm_model.py` & `oracle_ads-2.8.8/ads/model/framework/lightgbm_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/framework/pytorch_model.py` & `oracle_ads-2.8.8/ads/model/framework/pytorch_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,15 @@
                 "In future the models will be saved in TorchScript format by default. Currently saving it using torch.save method."
                 "Set `use_torch_script` as `True` to serialize the model as a TorchScript program by `torch.jit.save()` "
                 "and loaded using `torch.jit.load()` in score.py. "
                 "You don't need to modify `load_model()` in score.py to load the model."
                 "Check https://pytorch.org/tutorials/beginner/saving_loading_models.html#export-load-model-in-torchscript-format for more details."
                 "Set `use_torch_script` as `False` to save only the model parameters."
                 "The model class instance must be constructed before "
-                "loading parameters in the perdict function of score.py."
+                "loading parameters in the predict function of score.py."
                 "Check https://pytorch.org/tutorials/beginner/saving_loading_models.html#save-load-state-dict-recommended for more details."
             )
             use_torch_script = False
 
         if as_onnx and use_torch_script:
             raise ValueError("You can only save Pytorch model into one format.")
```

### Comparing `oracle_ads-2.8.7/ads/model/framework/sklearn_model.py` & `oracle_ads-2.8.8/ads/model/framework/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/framework/spark_model.py` & `oracle_ads-2.8.8/ads/model/framework/spark_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/framework/tensorflow_model.py` & `oracle_ads-2.8.8/ads/model/framework/tensorflow_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/framework/xgboost_model.py` & `oracle_ads-2.8.8/ads/model/framework/xgboost_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/generic_model.py` & `oracle_ads-2.8.8/ads/model/generic_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -2097,36 +2097,72 @@
         ValueError
             If `model_id` is not specified.
         """
         # Set default display_name if not specified - randomly generated easy to remember name generated
         if not display_name:
             display_name = utils.get_random_name_for_resource()
         # populates properties from args and kwargs. Empty values will be ignored.
-        self.properties.with_dict(_extract_locals(locals()))
+        override_properties = _extract_locals(locals())
         # clears out project_id and compartment_id from kwargs, to prevent passing
         # these params to the deployment via kwargs.
         kwargs.pop("project_id", None)
         kwargs.pop("compartment_id", None)
 
         max_wait_time = kwargs.pop("max_wait_time", DEFAULT_WAIT_TIME)
         poll_interval = kwargs.pop("poll_interval", DEFAULT_POLL_INTERVAL)
 
-        self.properties.compartment_id = (
-            self.properties.compartment_id or _COMPARTMENT_OCID
-        )
-        self.properties.project_id = self.properties.project_id or PROJECT_OCID
-        self.properties.deployment_instance_shape = (
-            self.properties.deployment_instance_shape or MODEL_DEPLOYMENT_INSTANCE_SHAPE
-        )
-        self.properties.deployment_instance_count = (
-            self.properties.deployment_instance_count or MODEL_DEPLOYMENT_INSTANCE_COUNT
-        )
-        self.properties.deployment_bandwidth_mbps = (
-            self.properties.deployment_bandwidth_mbps or MODEL_DEPLOYMENT_BANDWIDTH_MBPS
-        )
+        # GenericModel itself has a ModelDeployment instance. When calling deploy(),
+        # if there are parameters passed in they will override this ModelDeployment instance,
+        # otherwise the properties of the ModelDeployment instance will be applied for deployment.
+        existing_infrastructure = self.model_deployment.infrastructure
+        existing_runtime = self.model_deployment.runtime
+        property_dict = ModelProperties(
+            compartment_id = existing_infrastructure.compartment_id
+            or self.properties.compartment_id
+            or _COMPARTMENT_OCID,
+            project_id = existing_infrastructure.project_id
+            or self.properties.project_id
+            or PROJECT_OCID,
+            deployment_instance_shape = existing_infrastructure.shape_name
+            or self.properties.deployment_instance_shape
+            or MODEL_DEPLOYMENT_INSTANCE_SHAPE,
+            deployment_instance_count = existing_infrastructure.replica
+            or self.properties.deployment_instance_count
+            or MODEL_DEPLOYMENT_INSTANCE_COUNT,
+            deployment_bandwidth_mbps = existing_infrastructure.bandwidth_mbps
+            or self.properties.deployment_bandwidth_mbps
+            or MODEL_DEPLOYMENT_BANDWIDTH_MBPS,
+            deployment_ocpus = existing_infrastructure.shape_config_details.get(
+                "ocpus", None
+            )
+            or self.properties.deployment_ocpus
+            or MODEL_DEPLOYMENT_INSTANCE_OCPUS,
+            deployment_memory_in_gbs = existing_infrastructure.shape_config_details.get(
+                "memoryInGBs", None
+            )
+            or self.properties.deployment_memory_in_gbs
+            or MODEL_DEPLOYMENT_INSTANCE_MEMORY_IN_GBS,
+            deployment_log_group_id = existing_infrastructure.log_group_id
+            or self.properties.deployment_log_group_id,
+            deployment_access_log_id = existing_infrastructure.access_log.get(
+                "log_id", None
+            )
+            or self.properties.deployment_access_log_id,
+            deployment_predict_log_id = existing_infrastructure.predict_log.get(
+                "log_id", None
+            )
+            or self.properties.deployment_predict_log_id,
+            deployment_image = existing_runtime.image
+            or self.properties.deployment_image,
+            deployment_instance_subnet_id = existing_infrastructure.subnet_id
+            or self.properties.deployment_instance_subnet_id
+        ).to_dict()
+
+        property_dict.update(override_properties)
+        self.properties.with_dict(property_dict)
 
         if not self.model_id:
             raise ValueError(
                 "The model needs to be saved to the Model Catalog "
                 "before it can be deployed."
             )
 
@@ -2136,127 +2172,81 @@
         ) and not self.properties.deployment_log_group_id:
             raise ValueError(
                 "`deployment_log_group_id` needs to be specified. "
                 "`deployment_access_log_id` and `deployment_predict_log_id` "
                 "cannot be used without `deployment_log_group_id`."
             )
 
-        existing_infrastructure = self.model_deployment.infrastructure
-        existing_runtime = self.model_deployment.runtime
-
-        web_concurrency = (
-            kwargs.pop("web_concurrency", None)
-            or existing_infrastructure.web_concurrency
-        )
-        if not (
-            self.properties.compartment_id or existing_infrastructure.compartment_id
-        ):
+        if not self.properties.compartment_id:
             raise ValueError("`compartment_id` has to be provided.")
-        if not (self.properties.project_id or existing_infrastructure.project_id):
+        if not self.properties.project_id:
             raise ValueError("`project_id` has to be provided.")
         infrastructure = (
             ModelDeploymentInfrastructure()
-            .with_compartment_id(
-                self.properties.compartment_id or existing_infrastructure.compartment_id
-            )
-            .with_project_id(
-                self.properties.project_id or existing_infrastructure.project_id
-            )
-            .with_bandwidth_mbps(
-                self.properties.deployment_bandwidth_mbps
-                or existing_infrastructure.bandwidth_mbps
-            )
-            .with_shape_name(
-                self.properties.deployment_instance_shape
-                or existing_infrastructure.shape_name
-            )
-            .with_subnet_id(
-                self.properties.deployment_instance_subnet_id
-                or existing_infrastructure.subnet_id
-            )
-            .with_replica(
-                self.properties.deployment_instance_count
-                or existing_infrastructure.replica
-            )
-            .with_web_concurrency(web_concurrency)
+            .with_compartment_id(self.properties.compartment_id)
+            .with_project_id(self.properties.project_id)
+            .with_bandwidth_mbps(self.properties.deployment_bandwidth_mbps)
+            .with_shape_name(self.properties.deployment_instance_shape)
+            .with_replica(self.properties.deployment_instance_count)
+            .with_subnet_id(self.properties.deployment_instance_subnet_id)
         )
 
-        ocpus = (
-            self.properties.deployment_ocpus
-            or existing_infrastructure.shape_config_details.get("ocpus")
-        )
-        memory_in_gbs = (
-            self.properties.deployment_memory_in_gbs
-            or existing_infrastructure.shape_config_details.get("memory_in_gbs")
+        web_concurrency = (
+            kwargs.pop("web_concurrency", None)
+            or existing_infrastructure.web_concurrency
         )
+        if web_concurrency:
+            infrastructure.with_web_concurrency(web_concurrency)
 
         if infrastructure.shape_name.endswith("Flex"):
             infrastructure.with_shape_config_details(
-                ocpus=ocpus or MODEL_DEPLOYMENT_INSTANCE_OCPUS,
-                memory_in_gbs=memory_in_gbs or MODEL_DEPLOYMENT_INSTANCE_MEMORY_IN_GBS,
+                ocpus=self.properties.deployment_ocpus,
+                memory_in_gbs=self.properties.deployment_memory_in_gbs,
             )
 
-        access_log_id = (
-            self.properties.deployment_access_log_id
-            or existing_infrastructure.access_log.get("log_id")
-        )
-        access_log_group_id = (
-            self.properties.deployment_log_group_id
-            or existing_infrastructure.access_log.get("log_group_id")
-        )
-
         # specifies the access log id
-        if access_log_id:
+        if self.properties.deployment_access_log_id:
             infrastructure.with_access_log(
-                log_group_id=access_log_group_id,
-                log_id=access_log_id,
+                log_group_id=self.properties.deployment_log_group_id,
+                log_id=self.properties.deployment_access_log_id,
             )
 
-        predict_log_id = (
-            self.properties.deployment_predict_log_id
-            or existing_infrastructure.predict_log.get("log_id")
-        )
-        predict_log_group_id = (
-            self.properties.deployment_log_group_id
-            or existing_infrastructure.predict_log.get("log_group_id")
-        )
-
         # specifies the predict log id
-        if predict_log_id:
+        if self.properties.deployment_predict_log_id:
             infrastructure.with_predict_log(
-                log_group_id=predict_log_group_id,
-                log_id=predict_log_id,
+                log_group_id=self.properties.deployment_log_group_id,
+                log_id=self.properties.deployment_predict_log_id,
             )
 
         environment_variables = (
             kwargs.pop("environment_variables", {}) or existing_runtime.env
         )
         deployment_mode = (
-            kwargs.pop("deployment_mode", ModelDeploymentMode.HTTPS)
+            kwargs.pop("deployment_mode", None)
             or existing_runtime.deployment_mode
+            or ModelDeploymentMode.HTTPS
         )
 
         runtime = None
-        image = self.properties.deployment_image or existing_runtime.image
-        if image:
+        if self.properties.deployment_image:
             image_digest = (
                 kwargs.pop("image_digest", None) or existing_runtime.image_digest
             )
             cmd = kwargs.pop("cmd", []) or existing_runtime.cmd
             entrypoint = kwargs.pop("entrypoint", []) or existing_runtime.entrypoint
             server_port = (
                 kwargs.pop("server_port", None) or existing_runtime.server_port
             )
             health_check_port = (
                 kwargs.pop("health_check_port", None)
                 or existing_runtime.health_check_port
             )
             runtime = (
                 ModelDeploymentContainerRuntime()
-                .with_image(image)
+                .with_image(self.properties.deployment_image)
                 .with_image_digest(image_digest)
                 .with_cmd(cmd)
                 .with_entrypoint(entrypoint)
                 .with_server_port(server_port)
                 .with_health_check_port(health_check_port)
                 .with_deployment_mode(deployment_mode)
                 .with_model_uri(self.model_id)
```

### Comparing `oracle_ads-2.8.7/ads/model/model_artifact_boilerplate/artifact_introspection_test/model_artifact_validate.py` & `oracle_ads-2.8.8/ads/model/model_artifact_boilerplate/artifact_introspection_test/model_artifact_validate.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/model_artifact_boilerplate/score.py` & `oracle_ads-2.8.8/ads/model/model_artifact_boilerplate/score.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/model_introspect.py` & `oracle_ads-2.8.8/ads/model/model_introspect.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/model_metadata.py` & `oracle_ads-2.8.8/ads/model/model_metadata.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/model_metadata_mixin.py` & `oracle_ads-2.8.8/ads/model/model_metadata_mixin.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/model_properties.py` & `oracle_ads-2.8.8/ads/model/model_properties.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/model_version_set.py` & `oracle_ads-2.8.8/ads/model/model_version_set.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/runtime/env_info.py` & `oracle_ads-2.8.8/ads/model/runtime/env_info.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/runtime/model_deployment_details.py` & `oracle_ads-2.8.8/ads/model/runtime/model_deployment_details.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/runtime/model_provenance_details.py` & `oracle_ads-2.8.8/ads/model/runtime/model_provenance_details.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/runtime/runtime_info.py` & `oracle_ads-2.8.8/ads/model/runtime/runtime_info.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/runtime/schemas/model_provenance_schema.yaml` & `oracle_ads-2.8.8/ads/model/runtime/schemas/model_provenance_schema.yaml`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/runtime/utils.py` & `oracle_ads-2.8.8/ads/model/runtime/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/serde/common.py` & `oracle_ads-2.8.8/ads/model/serde/common.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/serde/model_input.py` & `oracle_ads-2.8.8/ads/model/serde/model_input.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/serde/model_serializer.py` & `oracle_ads-2.8.8/ads/model/serde/model_serializer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/service/oci_datascience_model.py` & `oracle_ads-2.8.8/ads/model/service/oci_datascience_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/service/oci_datascience_model_deployment.py` & `oracle_ads-2.8.8/ads/model/service/oci_datascience_model_deployment.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/service/oci_datascience_model_version_set.py` & `oracle_ads-2.8.8/ads/model/service/oci_datascience_model_version_set.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/model/transformer/onnx_transformer.py` & `oracle_ads-2.8.8/ads/model/transformer/onnx_transformer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/mysqldb/mysql_db.py` & `oracle_ads-2.8.8/ads/mysqldb/mysql_db.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/backend/ads_dataflow.py` & `oracle_ads-2.8.8/ads/opctl/backend/ads_dataflow.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/backend/ads_ml_job.py` & `oracle_ads-2.8.8/ads/opctl/backend/ads_ml_job.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/backend/ads_ml_pipeline.py` & `oracle_ads-2.8.8/ads/opctl/backend/ads_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/backend/ads_model_deployment.py` & `oracle_ads-2.8.8/ads/opctl/backend/ads_model_deployment.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/backend/base.py` & `oracle_ads-2.8.8/ads/opctl/backend/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/backend/local.py` & `oracle_ads-2.8.8/ads/opctl/backend/local.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/cli.py` & `oracle_ads-2.8.8/ads/opctl/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -384,29 +384,28 @@
 )
 def run(file, **kwargs):
     """
     Runs the workload on the targeted backend. When run `distributed` yaml spec, the backend is always OCI Data Science
     Jobs
     """
     debug = kwargs["debug"]
+    config = {}
     if file:
         if os.path.exists(file):
             auth = {}
             if kwargs["auth"]:
                 auth = authutil.create_signer(kwargs["auth"])
             else:
                 auth = authutil.default_signer()
 
             with fsspec.open(file, "r", **auth) as f:
                 config = suppress_traceback(debug)(yaml.safe_load)(f.read())
         else:
             raise FileNotFoundError(f"{file} is not found")
-    else:
-        # If no yaml is provided, we assume there's cmdline args to define a job.
-        config = {"kind": "job"}
+
     suppress_traceback(debug)(run_cmd)(config, **kwargs)
 
 
 @commands.command()
 @add_options(_options)
 @click.option(
     "--dry-run",
@@ -448,21 +447,59 @@
 def init_operator(**kwargs):
     suppress_traceback(kwargs["debug"])(init_operator_cmd)(**kwargs)
 
 
 @commands.command()
 @click.argument("ocid", nargs=1)
 @add_options(_model_deployment_options)
+@click.option(
+    "--conda-pack-folder",
+    required=False,
+    default=None,
+    help="folder where conda packs are saved",
+)
+@click.option(
+    "--auth",
+    "-a",
+    help="authentication method",
+    type=click.Choice(AuthType.values()),
+    default=None,
+)
+@click.option(
+    "--oci-profile",
+    help="oci profile",
+    default=None,
+)
+@click.option("--debug", "-d", help="set debug mode", is_flag=True, default=False)
 def delete(**kwargs):
     suppress_traceback(kwargs["debug"])(delete_cmd)(**kwargs)
 
 
 @commands.command()
 @click.argument("ocid", nargs=1)
 @add_options(_model_deployment_options)
+@click.option(
+    "--conda-pack-folder",
+    required=False,
+    default=None,
+    help="folder where conda packs are saved",
+)
+@click.option(
+    "--auth",
+    "-a",
+    help="authentication method",
+    type=click.Choice(AuthType.values()),
+    default=None,
+)
+@click.option(
+    "--oci-profile",
+    help="oci profile",
+    default=None,
+)
+@click.option("--debug", "-d", help="set debug mode", is_flag=True, default=False)
 def cancel(**kwargs):
     suppress_traceback(kwargs["debug"])(cancel_cmd)(**kwargs)
 
 
 @commands.command()
 @click.argument("ocid", nargs=1)
 @click.option(
@@ -487,35 +524,92 @@
 @click.option(
     "--wait",
     help="time in seconds to keep updating the logs after the job run finished for job.",
     type=int,
     required=False,
     default=90
 )
+@click.option(
+    "--conda-pack-folder",
+    required=False,
+    default=None,
+    help="folder where conda packs are saved",
+)
+@click.option(
+    "--auth",
+    "-a",
+    help="authentication method",
+    type=click.Choice(AuthType.values()),
+    default=None,
+)
+@click.option(
+    "--oci-profile",
+    help="oci profile",
+    default=None,
+)
+@click.option("--debug", "-d", help="set debug mode", is_flag=True, default=False)
 def watch(**kwargs):
     """
     ``tail`` logs form a job run, dataflow run or pipeline run.
     Connects to the logging service that was configured with the JobRun, Application Run or Pipeline Run and streams the logs.
     """
     suppress_traceback(kwargs["debug"])(watch_cmd)(**kwargs)
 
 
 @commands.command()
 @click.argument("ocid", nargs=1)
 @add_options(_model_deployment_options)
+@click.option(
+    "--conda-pack-folder",
+    required=False,
+    default=None,
+    help="folder where conda packs are saved",
+)
+@click.option(
+    "--auth",
+    "-a",
+    help="authentication method",
+    type=click.Choice(AuthType.values()),
+    default=None,
+)
+@click.option(
+    "--oci-profile",
+    help="oci profile",
+    default=None,
+)
+@click.option("--debug", "-d", help="set debug mode", is_flag=True, default=False)
 def activate(**kwargs):
     """
     Activates a data science service.
     """
     suppress_traceback(kwargs["debug"])(activate_cmd)(**kwargs)
 
 
 @commands.command()
 @click.argument("ocid", nargs=1)
 @add_options(_model_deployment_options)
+@click.option(
+    "--conda-pack-folder",
+    required=False,
+    default=None,
+    help="folder where conda packs are saved",
+)
+@click.option(
+    "--auth",
+    "-a",
+    help="authentication method",
+    type=click.Choice(AuthType.values()),
+    default=None,
+)
+@click.option(
+    "--oci-profile",
+    help="oci profile",
+    default=None,
+)
+@click.option("--debug", "-d", help="set debug mode", is_flag=True, default=False)
 def deactivate(**kwargs):
     """
     Deactivates a data science service.
     """
     suppress_traceback(kwargs["debug"])(deactivate_cmd)(**kwargs)
```

### Comparing `oracle_ads-2.8.7/ads/opctl/cmds.py` & `oracle_ads-2.8.8/ads/opctl/cmds.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
             and self._backend not in self.BACKENDS_MAP
         ):
             raise NotImplementedError(f"backend {self._backend} is not implemented.")
 
     @property
     def backend(self):
         if self._backend == BACKEND_NAME.LOCAL.value:
-            kind = self.config.get("kind")
+            kind = self.config.get("kind") or self.config["execution"].get("kind")
             if kind not in self.LOCAL_BACKENDS_MAP:
                 options = [backend for backend in self.LOCAL_BACKENDS_MAP.keys()]
                 # Special case local backend option not supported by this factory.
                 options.append("distributed")
                 raise RuntimeError(
                     f"kind {kind} not supported by local backend. Please choose from: "
                     f"[{str.join('|', options)}]"
@@ -150,15 +150,14 @@
             )
             if overwrite not in ["y", "Y"]:
                 return
         with open(yaml_path, "w", encoding="utf-8") as f:
             f.write(yaml_content)
         print(f"Job run info saved to {yaml_path}")
 
-
 def run(config: Dict, **kwargs) -> Dict:
     """
     Run a job given configuration and command line args passed in (kwargs).
 
     Parameters
     ----------
     config: dict
@@ -167,15 +166,23 @@
         keyword arguments, stores configuration from command line args
 
     Returns
     -------
     Dict
         dictionary of job id and run id in case of ML Job run, else empty if running locally
     """
-    p = ConfigProcessor(config).step(ConfigMerger, **kwargs)
+    if config:
+        p = ConfigProcessor(config).step(ConfigMerger, **kwargs)
+        if p.config["kind"] != BACKEND_NAME.LOCAL.value and p.config["kind"] != "distributed":
+            p.config["execution"]["backend"] = p.config["kind"]
+            return _BackendFactory(p.config).backend.apply()
+    else:
+        # If no yaml is provided and config is empty, we assume there's cmdline args to define a job.
+        config = {"kind": "job"}
+        p = ConfigProcessor(config).step(ConfigMerger, **kwargs)
     if config.get("kind") == "distributed":  # TODO: add kind factory
         print(
             "......................... Initializing the process ..................................."
         )
         ini = update_ini(
             kwargs["tag"],
             kwargs["registry"],
@@ -239,22 +246,14 @@
                     "# \u2b50 To stream the logs of the main job run:\n"
                     + f"# \u0024 ads opctl watch {list(cluster_run['mainJobRunId'].values())[0]}"
                 )
                 print(yamlContent)
                 _save_yaml(yamlContent, **kwargs)
             return cluster_run_info
     else:
-        if (
-            "kind" in p.config
-            and p.config["execution"].get("backend", None) != BACKEND_NAME.LOCAL.value
-            and "ocid" not in p.config["execution"]
-        ):
-            p.config["execution"]["backend"] = p.config["kind"]
-            return _BackendFactory(p.config).backend.apply()
-
         if "ocid" in p.config["execution"]:
             resource_to_backend = {
                 DataScienceResource.JOB: BACKEND_NAME.JOB,
                 DataScienceResource.DATAFLOW: BACKEND_NAME.DATAFLOW,
                 DataScienceResource.PIPELINE: BACKEND_NAME.PIPELINE,
             }
             for r, b in resource_to_backend.items():
@@ -589,14 +588,16 @@
         ]
 
         optional_fields = [
             ("log_group_id", ""),
             ("log_id", ""),
             ("docker_registry", ""),
             ("conda_pack_os_prefix", "in the format oci://<bucket>@<namespace>/<path>"),
+            ("memory_in_gbs", ""),
+            ("ocpus", "")
         ]
         _set_service_configurations(
             ADS_JOBS_CONFIG_FILE_NAME,
             required_fields,
             optional_fields,
             folder,
             oci_config_path,
@@ -615,14 +616,18 @@
             ("script_bucket", "in the format oci://<bucket>@<namespace>/<path>"),
         ]
 
         optional_fields = [
             ("num_executors", ""),
             ("spark_version", ""),
             ("archive_bucket", "in the format oci://<bucket>@<namespace>/<path>"),
+            ("driver_shape_memory_in_gbs", ""),
+            ("driver_shape_ocpus", ""),
+            ("executor_shape_memory_in_gbs", ""),
+            ("executor_shape_ocpus", "")
         ]
         _set_service_configurations(
             ADS_DATAFLOW_CONFIG_FILE_NAME,
             required_fields,
             optional_fields,
             folder,
             oci_config_path,
@@ -664,14 +669,16 @@
 
         optional_fields = [
             ("log_group_id", ""),
             ("log_id", ""),
             ("bandwidth_mbps", ""),
             ("replica", ""),
             ("web_concurrency", ""),
+            ("memory_in_gbs", ""),
+            ("ocpus", "")
         ]
 
         _set_service_configurations(
             ADS_MODEL_DEPLOYMENT_CONFIG_FILE_NAME,
             required_fields,
             optional_fields,
             folder,
```

### Comparing `oracle_ads-2.8.7/ads/opctl/conda/cli.py` & `oracle_ads-2.8.8/ads/opctl/conda/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/conda/cmds.py` & `oracle_ads-2.8.8/ads/opctl/conda/cmds.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/conda/config.yaml` & `oracle_ads-2.8.8/ads/opctl/conda/config.yaml`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/conda/multipart_uploader.py` & `oracle_ads-2.8.8/ads/opctl/conda/multipart_uploader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/conda/pack.py` & `oracle_ads-2.8.8/ads/opctl/conda/pack.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/config/base.py` & `oracle_ads-2.8.8/ads/opctl/config/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/config/diagnostics/distributed/default_requirements_config.yaml` & `oracle_ads-2.8.8/ads/opctl/config/diagnostics/distributed/default_requirements_config.yaml`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/config/merger.py` & `oracle_ads-2.8.8/ads/opctl/config/merger.py`

 * *Files 26% similar despite different names*

```diff
@@ -55,14 +55,16 @@
             os.path.expanduser(
                 self.config["execution"].pop("ads_config", DEFAULT_ADS_CONFIG_FOLDER)
             )
         )
         # 3. fill in values from default files under ~/.ads_ops
         self._fill_config_with_defaults(ads_config_path)
 
+        self._config_flex_shape_details()
+
         logger.debug(f"Config: {self.config}")
         return self
 
     def _merge_config_with_cmd_args(self, cmd_args: Dict) -> None:
         # overwrite config with command line args
         # if a command line arg value is None or empty collection, then it is ignored
         def _overwrite(cfg, args):
@@ -192,7 +194,51 @@
             if oci_profile in parser:
                 return parser[oci_profile]
         else:
             logger.info(
                 f"{os.path.join(ads_config_folder, config_file)} does not exist. No config loaded."
             )
         return {}
+
+    def _config_flex_shape_details(self):
+        infrastructure = self.config["infrastructure"]
+        backend = self.config["execution"].get("backend", None)
+        if backend == BACKEND_NAME.JOB.value or backend == BACKEND_NAME.MODEL_DEPLOYMENT.value:
+            shape_name = infrastructure.get("shape_name", "")
+            if shape_name.endswith(".Flex"):
+                if (
+                    "ocpus" not in infrastructure or 
+                    "memory_in_gbs" not in infrastructure
+                ):
+                    raise ValueError(
+                        "Parameters `ocpus` and `memory_in_gbs` must be provided for using flex shape. "
+                        "Call `ads opctl config` to specify."
+                    )
+                infrastructure["shape_config_details"] = {
+                    "ocpus": infrastructure.pop("ocpus"),
+                    "memory_in_gbs": infrastructure.pop("memory_in_gbs")
+                }
+        elif backend == BACKEND_NAME.DATAFLOW.value:
+            executor_shape = infrastructure.get("executor_shape", "")
+            driver_shape = infrastructure.get("driver_shape", "")
+            data_flow_shape_config_details = [
+                "driver_shape_memory_in_gbs",
+                "driver_shape_ocpus",
+                "executor_shape_memory_in_gbs",
+                "executor_shape_ocpus"
+            ]
+            # executor_shape and driver_shape must be the same shape family
+            if executor_shape.endswith(".Flex") or driver_shape.endswith(".Flex"):
+                for parameter in data_flow_shape_config_details:
+                    if parameter not in infrastructure:
+                        raise ValueError(
+                            f"Parameters {parameter} must be provided for using flex shape. "
+                            "Call `ads opctl config` to specify."
+                        )
+                infrastructure["driver_shape_config"] = {
+                    "ocpus": infrastructure.pop("driver_shape_ocpus"),
+                    "memory_in_gbs": infrastructure.pop("driver_shape_memory_in_gbs")
+                }
+                infrastructure["executor_shape_config"] = {
+                    "ocpus": infrastructure.pop("executor_shape_ocpus"),
+                    "memory_in_gbs": infrastructure.pop("executor_shape_memory_in_gbs")
+                }
```

### Comparing `oracle_ads-2.8.7/ads/opctl/config/resolver.py` & `oracle_ads-2.8.8/ads/opctl/config/resolver.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/config/utils.py` & `oracle_ads-2.8.8/ads/opctl/config/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/config/validator.py` & `oracle_ads-2.8.8/ads/opctl/config/validator.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/config/versioner.py` & `oracle_ads-2.8.8/ads/opctl/config/versioner.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/config/yaml_parsers/base.py` & `oracle_ads-2.8.8/ads/opctl/config/yaml_parsers/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/config/yaml_parsers/distributed/yaml_parser.py` & `oracle_ads-2.8.8/ads/opctl/config/yaml_parsers/distributed/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/constants.py` & `oracle_ads-2.8.8/ads/opctl/constants.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/decorator/common.py` & `oracle_ads-2.8.8/ads/opctl/decorator/common.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/diagnostics/__main__.py` & `oracle_ads-2.8.8/ads/opctl/diagnostics/__main__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/diagnostics/check_distributed_job_requirements.py` & `oracle_ads-2.8.8/ads/opctl/diagnostics/check_distributed_job_requirements.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/diagnostics/check_requirements.py` & `oracle_ads-2.8.8/ads/opctl/diagnostics/check_requirements.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/distributed/certificates.py` & `oracle_ads-2.8.8/ads/opctl/distributed/certificates.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/distributed/cli.py` & `oracle_ads-2.8.8/ads/opctl/distributed/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/distributed/cmds.py` & `oracle_ads-2.8.8/ads/opctl/distributed/cmds.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/distributed/common/abstract_cluster_provider.py` & `oracle_ads-2.8.8/ads/opctl/distributed/common/abstract_cluster_provider.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/distributed/common/abstract_framework_spec_builder.py` & `oracle_ads-2.8.8/ads/opctl/distributed/common/abstract_framework_spec_builder.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/distributed/common/cluster_config_helper.py` & `oracle_ads-2.8.8/ads/opctl/distributed/common/cluster_config_helper.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/distributed/common/cluster_provider_factory.py` & `oracle_ads-2.8.8/ads/opctl/distributed/common/cluster_provider_factory.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/distributed/common/cluster_runner.py` & `oracle_ads-2.8.8/ads/opctl/distributed/common/cluster_runner.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/distributed/common/framework_factory.py` & `oracle_ads-2.8.8/ads/opctl/distributed/common/framework_factory.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/docker/Dockerfile` & `oracle_ads-2.8.8/ads/opctl/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/docker/Dockerfile.gpu` & `oracle_ads-2.8.8/ads/opctl/docker/Dockerfile.gpu`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/docker/Dockerfile.job` & `oracle_ads-2.8.8/ads/opctl/docker/Dockerfile.job`

 * *Files 11% similar despite different names*

```diff
@@ -1,116 +1,108 @@
-# Copyright (c) 2021 Oracle and/or its affiliates.
+# Copyright (c) 2021, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
-FROM  --platform=linux/amd64 ghcr.io/oracle/oraclelinux:7-slim
+FROM ghcr.io/oracle/oraclelinux:7-slim
 
 # Configure environment
 ENV DATASCIENCE_USER datascience
 ENV DATASCIENCE_UID 1000
 ENV HOME /home/$DATASCIENCE_USER
 ENV DATASCIENCE_INSTALL_DIR /etc/datascience
 ENV LOGS_DIRECTORY /logs
 
+ARG release=19
+ARG update=13
+
 RUN \
-    yum -y -q install oracle-release-el7 deltarpm && \
+    yum -y -q install oracle-release-el7 && \
     yum-config-manager --add-repo http://yum.oracle.com/repo/OracleLinux/OL7/developer_EPEL/x86_64 && \
     yum-config-manager --enable ol7_optional_latest --enable ol7_addons --enable ol7_software_collections --enable ol7_oracle_instantclient > /dev/null && \
-    yum install -y -q \
-    build-essential \
+    yum groupinstall -y -q 'Development Tools' && \
+    yum update -y && \
+    yum install -y --setopt=skip_missing_names_on_install=False \
     bzip2 \
     curl \
     git \
-    gfortran \
+    gcc-gfortran \
     libcurl-devel \
     libxml2-devel \
     oracle-instantclient${release}.${update}-basic \
     oracle-instantclient${release}.${update}-sqlplus \
     openssl \
     openssl-devel \
     patch \
     sudo \
     unzip \
     zip \
-    g++ \
+    gcc-c++ \
     wget \
     gcc \
-    vim \
-    yum groupinstall -y -q development tools \
     && yum clean all \
     && rm -rf /var/cache/yum/*
 
-
 # setup user
 RUN \
   mkdir -p /home/$DATASCIENCE_USER && \
   useradd -m -s /bin/bash -N -u $DATASCIENCE_UID $DATASCIENCE_USER && \
   chown -R $DATASCIENCE_USER /home/$DATASCIENCE_USER && \
   chown -R $DATASCIENCE_USER:users /usr/local/ && \
   touch /etc/sudoers.d/$DATASCIENCE_USER && echo "$DATASCIENCE_USER ALL=(ALL:ALL) NOPASSWD: ALL" >> /etc/sudoers.d/$DATASCIENCE_USER && \
   mkdir -p $DATASCIENCE_INSTALL_DIR && chown $DATASCIENCE_USER $DATASCIENCE_INSTALL_DIR && \
   mkdir -p $LOGS_DIRECTORY && chown -R $DATASCIENCE_USER:users $LOGS_DIRECTORY && \
   mkdir -p $LOGS_DIRECTORY/harness && chown -R $DATASCIENCE_USER:users $LOGS_DIRECTORY/harness
-#   mkdir -p /home/$DATASCIENCE_USER/condapack
-
 
 RUN mkdir -p /etc/datascience/build
 RUN mkdir -p $DATASCIENCE_INSTALL_DIR/{pre-build-ds,post-build-ds,pre-run-ds,pre-run-user}
 
 #conda
 # set a default language for localization.  necessary for oci cli
 ARG LANG=en_US.utf8
 ENV LANG=$LANG
 ENV SHELL=/bin/bash
 
 # set /opt folder permissions for $DATASCIENCE_USER. Conda is going to live in this folder.
-RUN chown $DATASCIENCE_USER /opt
+RUN chown -R $DATASCIENCE_USER /opt
 
 USER $DATASCIENCE_USER
 WORKDIR /home/datascience
-RUN curl -L https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh >> /home/datascience/miniconda.sh \
+RUN wget -nv https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O /home/datascience/miniconda.sh \
     && /bin/bash /home/datascience/miniconda.sh -f -b -p /opt/conda \
     && rm /home/datascience/miniconda.sh \
-    && ls  /opt/**/* \
-    && /opt/conda/bin/conda install python=3.8 anaconda \
     && /opt/conda/bin/conda clean -yaf
 
 WORKDIR /
 USER root
 RUN printf "#!/bin/bash\nsource /opt/conda/bin/activate\n" > /etc/profile.d/enableconda.sh \
     && chmod +x /etc/profile.d/enableconda.sh
 
 USER $DATASCIENCE_USER
 ENV PATH="/opt/conda/bin:${PATH}"
 WORKDIR /home/datascience
 
-
-#COPY base-env.yaml /opt/base-env.yaml
-#RUN conda env update -q -n root -f /opt/base-env.yaml && conda clean -yaf && rm -rf /home/datascience/.cache/pip
-
+COPY docker/base-env.yaml /opt/base-env.yaml
+RUN conda env update -q -n root -f /opt/base-env.yaml && conda clean -yaf && rm -rf /home/datascience/.cache/pip
 
 USER $DATASCIENCE_USER
 
 ####### WRAP UP ###############################
 RUN python -c 'import sys; assert(sys.version_info[:2]) == (3, 8), "Python 3.8 is not detected"'
 WORKDIR /
 
 RUN conda list
 
 USER root
 
+ARG PIP_INDEX_URL
+
 ############# Setup Conda environment tools ###########################
 ARG RAND=1
 
-RUN pip install conda_pack oci-cli
-
 ARG RUN_WORKING_DIR="/home/datascience"
 WORKDIR $RUN_WORKING_DIR
 
 # clean tmp folder
 RUN rm -rf /tmp/*
 
-#COPY harness.py /etc/datascience/harness.py
 RUN mkdir -p /etc/datascience/operators
-# Temporarily removing operators related components
-# COPY operators/run.py /etc/datascience/operators/run.py
 
 USER datascience
```

### Comparing `oracle_ads-2.8.7/ads/opctl/docker/merge_dependencies.py` & `oracle_ads-2.8.8/ads/opctl/docker/merge_dependencies.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/model/cli.py` & `oracle_ads-2.8.8/ads/opctl/model/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/model/cmds.py` & `oracle_ads-2.8.8/ads/opctl/model/cmds.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/script.py` & `oracle_ads-2.8.8/ads/opctl/script.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/spark/cli.py` & `oracle_ads-2.8.8/ads/opctl/spark/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/spark/cmds.py` & `oracle_ads-2.8.8/ads/opctl/spark/cmds.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/templates/diagnostic_report_template.jinja2` & `oracle_ads-2.8.8/ads/opctl/templates/diagnostic_report_template.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/opctl/utils.py` & `oracle_ads-2.8.8/ads/opctl/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/oracledb/oracle_db.py` & `oracle_ads-2.8.8/ads/oracledb/oracle_db.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/pipeline/__init__.py` & `oracle_ads-2.8.8/ads/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/pipeline/ads_pipeline.py` & `oracle_ads-2.8.8/ads/pipeline/ads_pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -1900,15 +1900,15 @@
 
     #     ml_step_schema = {}
     #     with open(
     #         os.path.join(schema_path, "ml_step_schema.json")
     #     ) as ml_step_schema_file:
     #         ml_step_schema = json.load(ml_step_schema_file)
 
-    #     yaml_dict = yaml.load(Pipeline._read_from_file(uri=uri))
+    #     yaml_dict = yaml.load(Pipeline._read_from_file(uri=uri), Loader=yaml.FullLoader)
 
     #     pipeline_validator = Validator(pipeline_schema)
     #     if not pipeline_validator.validate(yaml_dict):
     #         raise ValueError(pipeline_validator.errors)
 
     #     step_details = yaml_dict["spec"]["stepDetails"]
     #     if len(step_details) == 0:
@@ -1992,15 +1992,14 @@
         return (
             self.build()
             .with_compartment_id(self.compartment_id or "{Provide a compartment OCID}")
             .with_project_id(self.project_id or "{Provide a project OCID}")
         )
 
 
-
 class DataSciencePipeline(OCIDataScienceMixin, oci.data_science.models.Pipeline):
     @classmethod
     def from_ocid(cls, ocid: str) -> "DataSciencePipeline":
         """Gets a datascience pipeline by OCID.
 
         Parameters
         ----------
@@ -2273,8 +2272,8 @@
             wait_for_states=[
                 oci.data_science.models.WorkRequest.STATUS_SUCCEEDED,
                 oci.data_science.models.WorkRequest.STATUS_FAILED,
             ],
             operation_kwargs=operation_kwargs,
             waiter_kwargs=waiter_kwargs,
         )
-        return self.sync()
+        return self.sync()
```

### Comparing `oracle_ads-2.8.7/ads/pipeline/ads_pipeline_run.py` & `oracle_ads-2.8.8/ads/pipeline/ads_pipeline_run.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/pipeline/ads_pipeline_step.py` & `oracle_ads-2.8.8/ads/pipeline/ads_pipeline_step.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/pipeline/builders/infrastructure/custom_script.py` & `oracle_ads-2.8.8/ads/pipeline/builders/infrastructure/custom_script.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/pipeline/cli.py` & `oracle_ads-2.8.8/ads/pipeline/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/pipeline/extension.py` & `oracle_ads-2.8.8/ads/pipeline/extension.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/pipeline/visualizer/base.py` & `oracle_ads-2.8.8/ads/pipeline/visualizer/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/pipeline/visualizer/graph_renderer.py` & `oracle_ads-2.8.8/ads/pipeline/visualizer/graph_renderer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/pipeline/visualizer/text_renderer.py` & `oracle_ads-2.8.8/ads/pipeline/visualizer/text_renderer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/secrets/adb.py` & `oracle_ads-2.8.8/ads/secrets/adb.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/secrets/auth_token.py` & `oracle_ads-2.8.8/ads/secrets/auth_token.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/secrets/big_data_service.py` & `oracle_ads-2.8.8/ads/secrets/big_data_service.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/secrets/mysqldb.py` & `oracle_ads-2.8.8/ads/secrets/mysqldb.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/secrets/oracledb.py` & `oracle_ads-2.8.8/ads/secrets/oracledb.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/secrets/secrets.py` & `oracle_ads-2.8.8/ads/secrets/secrets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
-# Copyright (c) 2021, 2022 Oracle and/or its affiliates.
+# Copyright (c) 2021, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 import ads
 from ads.vault import Vault
 from base64 import b64encode, b64decode
 import os
 import json
@@ -269,15 +269,15 @@
         else:
             vault_info = {}
             uri = source
             with fsspec.open(uri, storage_options=storage_options) as vf:
                 if format.lower() == "json":
                     vault_info = json.load(vf)
                 elif format.lower() in ["yaml", "yml"]:
-                    vault_info = yaml.load(vf)
+                    vault_info = yaml.load(vf, Loader=yaml.FullLoader)
                 if not cls._validate_required_vault_attributes(vault_info):
                     logger.error(
                         f"Missing required Attributes in file {uri}: {cls.required_keys}"
                     )
                     raise ValueError(
                         f"The file: {uri} does not contain all the required attributes - {','.join(cls.required_keys)}."
                     )
```

### Comparing `oracle_ads-2.8.7/ads/telemetry/telemetry.py` & `oracle_ads-2.8.8/ads/telemetry/telemetry.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/templates/score-pkl.jinja2` & `oracle_ads-2.8.8/ads/templates/score-pkl.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/templates/score.jinja2` & `oracle_ads-2.8.8/ads/templates/score.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/templates/score_generic.jinja2` & `oracle_ads-2.8.8/ads/templates/score_generic.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/templates/score_huggingface_pipeline.jinja2` & `oracle_ads-2.8.8/ads/templates/score_huggingface_pipeline.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/templates/score_lightgbm.jinja2` & `oracle_ads-2.8.8/ads/templates/score_lightgbm.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/templates/score_onnx.jinja2` & `oracle_ads-2.8.8/ads/templates/score_onnx.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/templates/score_onnx_new.jinja2` & `oracle_ads-2.8.8/ads/templates/score_onnx_new.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/templates/score_oracle_automl.jinja2` & `oracle_ads-2.8.8/ads/templates/score_oracle_automl.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/templates/score_pyspark.jinja2` & `oracle_ads-2.8.8/ads/templates/score_pyspark.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/templates/score_pytorch.jinja2` & `oracle_ads-2.8.8/ads/templates/score_pytorch.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/templates/score_scikit-learn.jinja2` & `oracle_ads-2.8.8/ads/templates/score_scikit-learn.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/templates/score_tensorflow.jinja2` & `oracle_ads-2.8.8/ads/templates/score_tensorflow.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/templates/score_xgboost.jinja2` & `oracle_ads-2.8.8/ads/templates/score_xgboost.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/text_dataset/backends.py` & `oracle_ads-2.8.8/ads/text_dataset/backends.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/text_dataset/dataset.py` & `oracle_ads-2.8.8/ads/text_dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/text_dataset/extractor.py` & `oracle_ads-2.8.8/ads/text_dataset/extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/text_dataset/options.py` & `oracle_ads-2.8.8/ads/text_dataset/options.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/text_dataset/udfs.py` & `oracle_ads-2.8.8/ads/text_dataset/udfs.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/text_dataset/utils.py` & `oracle_ads-2.8.8/ads/text_dataset/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/type_discovery/abstract_detector.py` & `oracle_ads-2.8.8/ads/type_discovery/abstract_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/type_discovery/constant_detector.py` & `oracle_ads-2.8.8/ads/type_discovery/constant_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/type_discovery/continuous_detector.py` & `oracle_ads-2.8.8/ads/type_discovery/continuous_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/type_discovery/credit_card_detector.py` & `oracle_ads-2.8.8/ads/type_discovery/credit_card_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/type_discovery/datetime_detector.py` & `oracle_ads-2.8.8/ads/type_discovery/datetime_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/type_discovery/discrete_detector.py` & `oracle_ads-2.8.8/ads/type_discovery/discrete_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/type_discovery/document_detector.py` & `oracle_ads-2.8.8/ads/type_discovery/document_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/type_discovery/ip_detector.py` & `oracle_ads-2.8.8/ads/type_discovery/ip_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/type_discovery/latlon_detector.py` & `oracle_ads-2.8.8/ads/type_discovery/latlon_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/type_discovery/phone_number_detector.py` & `oracle_ads-2.8.8/ads/type_discovery/phone_number_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/type_discovery/type_discovery_driver.py` & `oracle_ads-2.8.8/ads/type_discovery/type_discovery_driver.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/type_discovery/typed_feature.py` & `oracle_ads-2.8.8/ads/type_discovery/typed_feature.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/type_discovery/unknown_detector.py` & `oracle_ads-2.8.8/ads/type_discovery/unknown_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/type_discovery/zipcode_detector.py` & `oracle_ads-2.8.8/ads/type_discovery/zipcode_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/ads/vault/vault.py` & `oracle_ads-2.8.8/ads/vault/vault.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.7/oracle_ads.egg-info/PKG-INFO` & `oracle_ads-2.8.8/oracle_ads.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oracle-ads
-Version: 2.8.7
+Version: 2.8.8
 Summary: Oracle Accelerated Data Science SDK
 Home-page: https://docs.oracle.com/en-us/iaas/tools/ads-sdk/latest/index.html
 Author: Oracle Data Science
 License: Universal Permissive License 1.0
 Project-URL: Github, https://github.com/oracle/accelerated-data-science
 Project-URL: Documentation, https://accelerated-data-science.readthedocs.io/en/latest/index.html
 Keywords: Oracle Cloud Infrastructure,OCI,Machine Learning,ML,Artificial Intelligence,AI,Data Science,Cloud,Oracle
```

### Comparing `oracle_ads-2.8.7/oracle_ads.egg-info/SOURCES.txt` & `oracle_ads-2.8.8/oracle_ads.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -221,25 +221,28 @@
 ads/jobs/builders/infrastructure/dsc_job_runtime.py
 ads/jobs/builders/infrastructure/utils.py
 ads/jobs/builders/runtimes/__init__.py
 ads/jobs/builders/runtimes/artifact.py
 ads/jobs/builders/runtimes/base.py
 ads/jobs/builders/runtimes/container_runtime.py
 ads/jobs/builders/runtimes/python_runtime.py
+ads/jobs/builders/runtimes/pytorch_runtime.py
 ads/jobs/schema/__init__.py
 ads/jobs/schema/infrastructure_schema.json
 ads/jobs/schema/job_schema.json
 ads/jobs/schema/runtime_schema.json
 ads/jobs/schema/validator.py
 ads/jobs/templates/__init__.py
 ads/jobs/templates/container.py
 ads/jobs/templates/driver_notebook.py
 ads/jobs/templates/driver_oci.py
 ads/jobs/templates/driver_python.py
+ads/jobs/templates/driver_pytorch.py
 ads/jobs/templates/driver_utils.py
+ads/jobs/templates/oci_metrics.py
 ads/model/__init__.py
 ads/model/artifact.py
 ads/model/artifact_downloader.py
 ads/model/artifact_uploader.py
 ads/model/base_properties.py
 ads/model/datascience_model.py
 ads/model/generic_model.py
@@ -357,14 +360,15 @@
 ads/opctl/distributed/common/cluster_provider_factory.py
 ads/opctl/distributed/common/cluster_runner.py
 ads/opctl/distributed/common/framework_factory.py
 ads/opctl/docker/Dockerfile
 ads/opctl/docker/Dockerfile.gpu
 ads/opctl/docker/Dockerfile.job
 ads/opctl/docker/Dockerfile.job.gpu
+ads/opctl/docker/base-env.yaml
 ads/opctl/docker/cuda.repo
 ads/opctl/docker/merge_dependencies.py
 ads/opctl/model/__init__.py
 ads/opctl/model/cli.py
 ads/opctl/model/cmds.py
 ads/opctl/spark/__init__.py
 ads/opctl/spark/cli.py
```

### Comparing `oracle_ads-2.8.7/oracle_ads.egg-info/requires.txt` & `oracle_ads-2.8.8/oracle_ads.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 gitpython>=3.1.2
 matplotlib>=3.1.3
 numpy>=1.19.2
 oci>=2.104.3
 ocifs>=1.1.3
 pandas<1.6,>1.2.1
 python_jsonschema_objects>=0.3.13
-PyYAML<6,>=5.4
+PyYAML>=6
 requests
 scikit-learn<1.2,>=0.23.2
 tabulate>=0.8.9
 tqdm>=4.59.0
 psutil>=5.7.2
 
 [all-optional]
```

### Comparing `oracle_ads-2.8.7/setup.py` & `oracle_ads-2.8.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "gitpython>=3.1.2",
     "matplotlib>=3.1.3",
     "numpy>=1.19.2",
     "oci>=2.104.3",
     "ocifs>=1.1.3",
     "pandas>1.2.1,<1.6",
     "python_jsonschema_objects>=0.3.13",
-    "PyYAML>=5.4,<6",
+    "PyYAML>=6",  # pyyaml 5.4 is broken with cython 3
     "requests",
     "scikit-learn>=0.23.2,<1.2",
     "tabulate>=0.8.9",
     "tqdm>=4.59.0",
     "psutil>=5.7.2",
 ]
```

