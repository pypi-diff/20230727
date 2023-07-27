# Comparing `tmp/mlpylint-0.0.2.tar.gz` & `tmp/mlpylint-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpylint-0.0.2.tar", last modified: Mon Jul 24 07:43:46 2023, max compression
+gzip compressed data, was "mlpylint-0.0.3.tar", last modified: Thu Jul 27 12:27:33 2023, max compression
```

## Comparing `mlpylint-0.0.2.tar` & `mlpylint-0.0.3.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 07:43:46.121135 mlpylint-0.0.2/
--rw-rw-rw-   0        0        0     1090 2023-07-17 17:13:05.000000 mlpylint-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4368 2023-07-24 07:43:46.121135 mlpylint-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3040 2023-07-24 07:29:37.000000 mlpylint-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 07:43:46.071458 mlpylint-0.0.2/mlpylint.egg-info/
--rw-rw-rw-   0        0        0     4368 2023-07-24 07:43:46.000000 mlpylint-0.0.2/mlpylint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4662 2023-07-24 07:43:46.000000 mlpylint-0.0.2/mlpylint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 07:43:46.000000 mlpylint-0.0.2/mlpylint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-24 07:43:46.000000 mlpylint-0.0.2/mlpylint.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-23 18:52:34.000000 mlpylint-0.0.2/mlpylint.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       89 2023-07-24 07:43:46.000000 mlpylint-0.0.2/mlpylint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-24 07:43:46.000000 mlpylint-0.0.2/mlpylint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       84 2023-07-18 11:00:37.000000 mlpylint-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1548 2023-07-24 07:43:46.122136 mlpylint-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-24 07:43:46.072458 mlpylint-0.0.2/src/
--rw-rw-rw-   0        0        0        0 2023-07-18 09:26:23.000000 mlpylint-0.0.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:43:46.075460 mlpylint-0.0.2/src/analysis/
--rw-rw-rw-   0        0        0        0 2023-04-01 22:11:59.000000 mlpylint-0.0.2/src/analysis/__init__.py
--rw-rw-rw-   0        0        0     6936 2023-07-18 09:30:36.000000 mlpylint-0.0.2/src/analysis/argument.py
--rw-rw-rw-   0        0        0      348 2023-06-22 14:08:30.000000 mlpylint-0.0.2/src/analysis/config.py
--rw-rw-rw-   0        0        0     3482 2023-07-18 09:30:36.000000 mlpylint-0.0.2/src/analysis/result.py
--rw-rw-rw-   0        0        0     5462 2023-07-22 13:10:28.000000 mlpylint-0.0.2/src/analysis/runner.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:43:46.088460 mlpylint-0.0.2/src/checkers/
--rw-rw-rw-   0        0        0        0 2023-04-01 22:14:02.000000 mlpylint-0.0.2/src/checkers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:43:46.092459 mlpylint-0.0.2/src/checkers/advice/
--rw-rw-rw-   0        0        0        0 2023-05-07 15:22:41.000000 mlpylint-0.0.2/src/checkers/advice/__init__.py
--rw-rw-rw-   0        0        0     5023 2023-07-22 13:13:35.000000 mlpylint-0.0.2/src/checkers/advice/advice_checker_4_12_memory_not_freed.py
--rw-rw-rw-   0        0        0     3025 2023-07-21 16:41:28.000000 mlpylint-0.0.2/src/checkers/advice/advice_checker_4_16_broadcasting_feature_not_used.py
--rw-rw-rw-   0        0        0     3628 2023-07-23 07:45:25.000000 mlpylint-0.0.2/src/checkers/advice/advice_checker_4_18_training_evaluation_mode_improper_toggling.py
--rw-rw-rw-   0        0        0     3694 2023-07-21 20:07:07.000000 mlpylint-0.0.2/src/checkers/advice/advice_checker_4_1_unnecessary_iteration.py
--rw-rw-rw-   0        0        0     3430 2023-07-23 08:09:22.000000 mlpylint-0.0.2/src/checkers/advice/advice_checker_4_20_gradients_not_cleared_before_backward_propagation.py
--rw-rw-rw-   0        0        0     4780 2023-07-23 08:34:13.000000 mlpylint-0.0.2/src/checkers/advice/advice_checker_4_21_data_leakage.py
--rw-rw-rw-   0        0        0      558 2023-04-28 15:37:23.000000 mlpylint-0.0.2/src/checkers/base_checker.py
--rw-rw-rw-   0        0        0     3682 2023-07-18 15:02:34.000000 mlpylint-0.0.2/src/checkers/checker_4_11_hyperparameter_not_explicitly_set.py
--rw-rw-rw-   0        0        0     3749 2023-07-18 15:03:16.000000 mlpylint-0.0.2/src/checkers/checker_4_13_deterministic_algorithm_option_not_used.py
--rw-rw-rw-   0        0        0    13736 2023-07-18 15:03:55.000000 mlpylint-0.0.2/src/checkers/checker_4_14_randomness_uncontrolled.py
--rw-rw-rw-   0        0        0     5564 2023-07-18 15:04:37.000000 mlpylint-0.0.2/src/checkers/checker_4_15_missing_the_mask_of_invalid_value.py
--rw-rw-rw-   0        0        0     3585 2023-07-18 15:04:59.000000 mlpylint-0.0.2/src/checkers/checker_4_17_tensorarray_not_used.py
--rw-rw-rw-   0        0        0     3010 2023-07-23 12:30:18.000000 mlpylint-0.0.2/src/checkers/checker_4_19_pytorch_call_method_misused.py
--rw-rw-rw-   0        0        0     5162 2023-07-18 14:58:23.000000 mlpylint-0.0.2/src/checkers/checker_4_2_nan_equivalence_comparison_misused.py
--rw-rw-rw-   0        0        0     3341 2023-07-18 14:58:44.000000 mlpylint-0.0.2/src/checkers/checker_4_3_chain_indexing.py
--rw-rw-rw-   0        0        0     3275 2023-07-18 14:59:10.000000 mlpylint-0.0.2/src/checkers/checker_4_4_columns_and_data_type_not_explicitly_set.py
--rw-rw-rw-   0        0        0    11187 2023-07-18 15:00:03.000000 mlpylint-0.0.2/src/checkers/checker_4_5_empty_column_misinitialization.py
--rw-rw-rw-   0        0        0     3677 2023-07-18 15:00:30.000000 mlpylint-0.0.2/src/checkers/checker_4_6_merge_api_parameter_not_explicitly_set.py
--rw-rw-rw-   0        0        0     4202 2023-07-18 15:00:55.000000 mlpylint-0.0.2/src/checkers/checker_4_7_in_place_apis_misused.py
--rw-rw-rw-   0        0        0     2703 2023-07-18 15:01:39.000000 mlpylint-0.0.2/src/checkers/checker_4_8_dataframe_conversion_api_misused.py
--rw-rw-rw-   0        0        0     5829 2023-07-23 18:48:38.000000 mlpylint-0.0.2/src/checkers/checker_4_9_matrix_multiplication_api_misused.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:43:46.093460 mlpylint-0.0.2/tests/
--rw-rw-rw-   0        0        0        0 2023-04-01 23:33:14.000000 mlpylint-0.0.2/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:43:46.107351 mlpylint-0.0.2/tests/test_checkers/
--rw-rw-rw-   0        0        0        0 2023-04-02 16:23:11.000000 mlpylint-0.0.2/tests/test_checkers/__init__.py
--rw-rw-rw-   0        0        0      717 2023-07-22 12:56:13.000000 mlpylint-0.0.2/tests/test_checkers/test_advice_checker_4_12_memory_not_freed.py
--rw-rw-rw-   0        0        0      780 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_advice_checker_4_16_broadcasting_feature_not_used.py
--rw-rw-rw-   0        0        0      856 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_advice_checker_4_18_training_evaluation_mode_improper_toggling.py
--rw-rw-rw-   0        0        0      741 2023-07-21 20:05:10.000000 mlpylint-0.0.2/tests/test_checkers/test_advice_checker_4_1_unnecessary_iteration.py
--rw-rw-rw-   0        0        0      883 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_advice_checker_4_20_gradients_not_cleared_before_backward_propagation.py
--rw-rw-rw-   0        0        0      633 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_advice_checker_4_21_data_leakage.py
--rw-rw-rw-   0        0        0      720 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_11_hyperparameter_not_explicitly_set.py
--rw-rw-rw-   0        0        0      748 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_13_deterministic_algorithm_option_not_used.py
--rw-rw-rw-   0        0        0      674 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_14_randomness_uncontrolled.py
--rw-rw-rw-   0        0        0      716 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_15_missing_the_mask_of_invalid_value.py
--rw-rw-rw-   0        0        0      657 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_17_tensorarray_not_used.py
--rw-rw-rw-   0        0        0      690 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_19_pytorch_call_method_misused.py
--rw-rw-rw-   0        0        0      736 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_2_nan_equivalence_comparison_misused.py
--rw-rw-rw-   0        0        0      626 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_3_chain_indexing.py
--rw-rw-rw-   0        0        0      741 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_4_columns_and_datatype_not_explicitly_set.py
--rw-rw-rw-   0        0        0      704 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_5_empty_column_misinitialization.py
--rw-rw-rw-   0        0        0      738 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_6_merge_api_parameter_not_explicitly_set.py
--rw-rw-rw-   0        0        0      657 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_7_in_place_apis_misused.py
--rw-rw-rw-   0        0        0      712 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_8_dataframe_conversion_api_misused.py
--rw-rw-rw-   0        0        0      717 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_checkers/test_checker_4_9_matrix_multiplication_api_misused.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:43:46.120135 mlpylint-0.0.2/tests/test_files/
--rw-rw-rw-   0        0        0        0 2023-04-02 16:23:30.000000 mlpylint-0.0.2/tests/test_files/__init__.py
--rw-rw-rw-   0        0        0      291 2023-07-17 12:38:57.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_11_hyperparameter_not_explicitly_set.py
--rw-rw-rw-   0        0        0      941 2023-07-22 12:57:56.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_12_memory_not_freed.py
--rw-rw-rw-   0        0        0     2016 2023-06-15 00:02:04.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_13_deterministic_algorithm_option_not_used.py
--rw-rw-rw-   0        0        0     2454 2023-06-11 19:11:44.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_14_randomness_uncontrolled.py
--rw-rw-rw-   0        0        0      637 2023-06-11 20:09:44.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_15_missing_the_mask_of_invalid_value.py
--rw-rw-rw-   0        0        0      538 2023-07-21 16:12:07.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_16_broadcasting_feature_not_used.py
--rw-rw-rw-   0        0        0      918 2023-05-08 08:32:09.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_17_tensorarray_not_used.py
--rw-rw-rw-   0        0        0     1001 2023-06-05 12:37:31.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_18_training_evaluation_mode_improper_toggling.py
--rw-rw-rw-   0        0        0      603 2023-05-08 09:54:37.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_19_pytorch_call_method_misused.py
--rw-rw-rw-   0        0        0     2274 2023-07-21 19:39:51.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_1_unnecessary_iteration.py
--rw-rw-rw-   0        0        0     1202 2023-07-23 08:09:22.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_20_gradients_not_cleared_before_backward_propagation.py
--rw-rw-rw-   0        0        0     1621 2023-07-23 08:34:26.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_21_data_leakage.py
--rw-rw-rw-   0        0        0      587 2023-06-06 07:43:34.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_2_nan_equivalence_comparison_misused.py
--rw-rw-rw-   0        0        0     1114 2023-06-06 15:36:23.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_3_chain_indexing.py
--rw-rw-rw-   0        0        0     2099 2023-04-29 14:13:44.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_4_columns_and_datatype_not_explicitly_set.py
--rw-rw-rw-   0        0        0     1145 2023-06-14 21:59:24.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_5_empty_column_misinitialization.py
--rw-rw-rw-   0        0        0      956 2023-04-29 18:45:40.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_6_merge_api_parameter_not_explicitly_set.py
--rw-rw-rw-   0        0        0      854 2023-06-11 10:28:02.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_7_in_place_apis_misused.py
--rw-rw-rw-   0        0        0      660 2023-06-11 12:07:03.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_8_dataframe_conversion_api_misused.py
--rw-rw-rw-   0        0        0     2173 2023-06-14 22:51:51.000000 mlpylint-0.0.2/tests/test_files/file_checker_4_9_matrix_multiplication_api_misused.py
--rw-rw-rw-   0        0        0        2 2023-07-18 09:37:54.000000 mlpylint-0.0.2/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 12:27:33.192157 mlpylint-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-07-17 17:13:05.000000 mlpylint-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4688 2023-07-27 12:27:33.192157 mlpylint-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3360 2023-07-24 07:59:08.000000 mlpylint-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 12:27:33.145152 mlpylint-0.0.3/mlpylint.egg-info/
+-rw-rw-rw-   0        0        0     4688 2023-07-27 12:27:33.000000 mlpylint-0.0.3/mlpylint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4658 2023-07-27 12:27:33.000000 mlpylint-0.0.3/mlpylint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 12:27:33.000000 mlpylint-0.0.3/mlpylint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-27 12:27:33.000000 mlpylint-0.0.3/mlpylint.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-26 17:48:48.000000 mlpylint-0.0.3/mlpylint.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       89 2023-07-27 12:27:33.000000 mlpylint-0.0.3/mlpylint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-27 12:27:33.000000 mlpylint-0.0.3/mlpylint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       84 2023-07-18 11:00:37.000000 mlpylint-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1548 2023-07-27 12:27:33.193158 mlpylint-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-27 12:27:33.146161 mlpylint-0.0.3/src/
+-rw-rw-rw-   0        0        0        0 2023-07-18 09:26:23.000000 mlpylint-0.0.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 12:27:33.149157 mlpylint-0.0.3/src/analysis/
+-rw-rw-rw-   0        0        0        0 2023-04-01 22:11:59.000000 mlpylint-0.0.3/src/analysis/__init__.py
+-rw-rw-rw-   0        0        0     6936 2023-07-18 09:30:36.000000 mlpylint-0.0.3/src/analysis/argument.py
+-rw-rw-rw-   0        0        0      348 2023-06-22 14:08:30.000000 mlpylint-0.0.3/src/analysis/config.py
+-rw-rw-rw-   0        0        0     3482 2023-07-18 09:30:36.000000 mlpylint-0.0.3/src/analysis/result.py
+-rw-rw-rw-   0        0        0     5462 2023-07-22 13:10:28.000000 mlpylint-0.0.3/src/analysis/runner.py
+drwxrwxrwx   0        0        0        0 2023-07-27 12:27:33.159149 mlpylint-0.0.3/src/checkers/
+-rw-rw-rw-   0        0        0        0 2023-04-01 22:14:02.000000 mlpylint-0.0.3/src/checkers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 12:27:33.164157 mlpylint-0.0.3/src/checkers/advice/
+-rw-rw-rw-   0        0        0        0 2023-05-07 15:22:41.000000 mlpylint-0.0.3/src/checkers/advice/__init__.py
+-rw-rw-rw-   0        0        0     5023 2023-07-22 13:13:35.000000 mlpylint-0.0.3/src/checkers/advice/advice_checker_4_12_memory_not_freed.py
+-rw-rw-rw-   0        0        0     3025 2023-07-21 16:41:28.000000 mlpylint-0.0.3/src/checkers/advice/advice_checker_4_16_broadcasting_feature_not_used.py
+-rw-rw-rw-   0        0        0     3628 2023-07-23 07:45:25.000000 mlpylint-0.0.3/src/checkers/advice/advice_checker_4_18_training_evaluation_mode_improper_toggling.py
+-rw-rw-rw-   0        0        0     3694 2023-07-21 20:07:07.000000 mlpylint-0.0.3/src/checkers/advice/advice_checker_4_1_unnecessary_iteration.py
+-rw-rw-rw-   0        0        0     3430 2023-07-23 08:09:22.000000 mlpylint-0.0.3/src/checkers/advice/advice_checker_4_20_gradients_not_cleared_before_backward_propagation.py
+-rw-rw-rw-   0        0        0     4780 2023-07-23 08:34:13.000000 mlpylint-0.0.3/src/checkers/advice/advice_checker_4_21_data_leakage.py
+-rw-rw-rw-   0        0        0      558 2023-04-28 15:37:23.000000 mlpylint-0.0.3/src/checkers/base_checker.py
+-rw-rw-rw-   0        0        0     3891 2023-07-26 13:28:02.000000 mlpylint-0.0.3/src/checkers/checker_4_11_hyperparameter_not_explicitly_set.py
+-rw-rw-rw-   0        0        0     3749 2023-07-18 15:03:16.000000 mlpylint-0.0.3/src/checkers/checker_4_13_deterministic_algorithm_option_not_used.py
+-rw-rw-rw-   0        0        0    13446 2023-07-26 08:17:43.000000 mlpylint-0.0.3/src/checkers/checker_4_14_randomness_uncontrolled.py
+-rw-rw-rw-   0        0        0     5564 2023-07-18 15:04:37.000000 mlpylint-0.0.3/src/checkers/checker_4_15_missing_the_mask_of_invalid_value.py
+-rw-rw-rw-   0        0        0     3585 2023-07-18 15:04:59.000000 mlpylint-0.0.3/src/checkers/checker_4_17_tensorarray_not_used.py
+-rw-rw-rw-   0        0        0     3010 2023-07-23 12:30:18.000000 mlpylint-0.0.3/src/checkers/checker_4_19_pytorch_call_method_misused.py
+-rw-rw-rw-   0        0        0     5456 2023-07-26 08:36:25.000000 mlpylint-0.0.3/src/checkers/checker_4_2_nan_equivalence_comparison_misused.py
+-rw-rw-rw-   0        0        0     3365 2023-07-26 08:36:25.000000 mlpylint-0.0.3/src/checkers/checker_4_3_chain_indexing.py
+-rw-rw-rw-   0        0        0     3563 2023-07-26 14:20:26.000000 mlpylint-0.0.3/src/checkers/checker_4_4_columns_and_data_type_not_explicitly_set.py
+-rw-rw-rw-   0        0        0    11271 2023-07-25 12:39:33.000000 mlpylint-0.0.3/src/checkers/checker_4_5_empty_column_misinitialization.py
+-rw-rw-rw-   0        0        0     3552 2023-07-25 12:45:16.000000 mlpylint-0.0.3/src/checkers/checker_4_6_merge_api_parameter_not_explicitly_set.py
+-rw-rw-rw-   0        0        0     4202 2023-07-18 15:00:55.000000 mlpylint-0.0.3/src/checkers/checker_4_7_in_place_apis_misused.py
+-rw-rw-rw-   0        0        0     2703 2023-07-18 15:01:39.000000 mlpylint-0.0.3/src/checkers/checker_4_8_dataframe_conversion_api_misused.py
+-rw-rw-rw-   0        0        0     5829 2023-07-25 12:54:41.000000 mlpylint-0.0.3/src/checkers/checker_4_9_matrix_multiplication_api_misused.py
+drwxrwxrwx   0        0        0        0 2023-07-27 12:27:33.165156 mlpylint-0.0.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-01 23:33:14.000000 mlpylint-0.0.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 12:27:33.178157 mlpylint-0.0.3/tests/test_checkers/
+-rw-rw-rw-   0        0        0        0 2023-04-02 16:23:11.000000 mlpylint-0.0.3/tests/test_checkers/__init__.py
+-rw-rw-rw-   0        0        0      717 2023-07-22 12:56:13.000000 mlpylint-0.0.3/tests/test_checkers/test_advice_checker_4_12_memory_not_freed.py
+-rw-rw-rw-   0        0        0      780 2023-07-18 09:37:54.000000 mlpylint-0.0.3/tests/test_checkers/test_advice_checker_4_16_broadcasting_feature_not_used.py
+-rw-rw-rw-   0        0        0      856 2023-07-18 09:37:54.000000 mlpylint-0.0.3/tests/test_checkers/test_advice_checker_4_18_training_evaluation_mode_improper_toggling.py
+-rw-rw-rw-   0        0        0      741 2023-07-21 20:05:10.000000 mlpylint-0.0.3/tests/test_checkers/test_advice_checker_4_1_unnecessary_iteration.py
+-rw-rw-rw-   0        0        0      883 2023-07-18 09:37:54.000000 mlpylint-0.0.3/tests/test_checkers/test_advice_checker_4_20_gradients_not_cleared_before_backward_propagation.py
+-rw-rw-rw-   0        0        0      633 2023-07-18 09:37:54.000000 mlpylint-0.0.3/tests/test_checkers/test_advice_checker_4_21_data_leakage.py
+-rw-rw-rw-   0        0        0      716 2023-07-26 13:22:38.000000 mlpylint-0.0.3/tests/test_checkers/test_checker_4_11_hyperparameter_not_explicitly_set.py
+-rw-rw-rw-   0        0        0      748 2023-07-18 09:37:54.000000 mlpylint-0.0.3/tests/test_checkers/test_checker_4_13_deterministic_algorithm_option_not_used.py
+-rw-rw-rw-   0        0        0      674 2023-07-18 09:37:54.000000 mlpylint-0.0.3/tests/test_checkers/test_checker_4_14_randomness_uncontrolled.py
+-rw-rw-rw-   0        0        0      716 2023-07-18 09:37:54.000000 mlpylint-0.0.3/tests/test_checkers/test_checker_4_15_missing_the_mask_of_invalid_value.py
+-rw-rw-rw-   0        0        0      657 2023-07-18 09:37:54.000000 mlpylint-0.0.3/tests/test_checkers/test_checker_4_17_tensorarray_not_used.py
+-rw-rw-rw-   0        0        0      690 2023-07-18 09:37:54.000000 mlpylint-0.0.3/tests/test_checkers/test_checker_4_19_pytorch_call_method_misused.py
+-rw-rw-rw-   0        0        0      736 2023-07-25 11:53:10.000000 mlpylint-0.0.3/tests/test_checkers/test_checker_4_2_nan_equivalence_comparison_misused.py
+-rw-rw-rw-   0        0        0      626 2023-07-18 09:37:54.000000 mlpylint-0.0.3/tests/test_checkers/test_checker_4_3_chain_indexing.py
+-rw-rw-rw-   0        0        0      741 2023-07-18 09:37:54.000000 mlpylint-0.0.3/tests/test_checkers/test_checker_4_4_columns_and_datatype_not_explicitly_set.py
+-rw-rw-rw-   0        0        0      704 2023-07-18 09:37:54.000000 mlpylint-0.0.3/tests/test_checkers/test_checker_4_5_empty_column_misinitialization.py
+-rw-rw-rw-   0        0        0      738 2023-07-18 09:37:54.000000 mlpylint-0.0.3/tests/test_checkers/test_checker_4_6_merge_api_parameter_not_explicitly_set.py
+-rw-rw-rw-   0        0        0      657 2023-07-18 09:37:54.000000 mlpylint-0.0.3/tests/test_checkers/test_checker_4_7_in_place_apis_misused.py
+-rw-rw-rw-   0        0        0      712 2023-07-18 09:37:54.000000 mlpylint-0.0.3/tests/test_checkers/test_checker_4_8_dataframe_conversion_api_misused.py
+-rw-rw-rw-   0        0        0      717 2023-07-18 09:37:54.000000 mlpylint-0.0.3/tests/test_checkers/test_checker_4_9_matrix_multiplication_api_misused.py
+drwxrwxrwx   0        0        0        0 2023-07-27 12:27:33.191159 mlpylint-0.0.3/tests/test_files/
+-rw-rw-rw-   0        0        0        0 2023-04-02 16:23:30.000000 mlpylint-0.0.3/tests/test_files/__init__.py
+-rw-rw-rw-   0        0        0      307 2023-07-26 13:27:08.000000 mlpylint-0.0.3/tests/test_files/file_checker_4_11_hyperparam_not_explicitly_set.py
+-rw-rw-rw-   0        0        0      941 2023-07-22 12:57:56.000000 mlpylint-0.0.3/tests/test_files/file_checker_4_12_memory_not_freed.py
+-rw-rw-rw-   0        0        0     2016 2023-07-25 13:39:04.000000 mlpylint-0.0.3/tests/test_files/file_checker_4_13_deterministic_algorithm_option_not_used.py
+-rw-rw-rw-   0        0        0     2454 2023-06-11 19:11:44.000000 mlpylint-0.0.3/tests/test_files/file_checker_4_14_randomness_uncontrolled.py
+-rw-rw-rw-   0        0        0      637 2023-06-11 20:09:44.000000 mlpylint-0.0.3/tests/test_files/file_checker_4_15_missing_the_mask_of_invalid_value.py
+-rw-rw-rw-   0        0        0      538 2023-07-21 16:12:07.000000 mlpylint-0.0.3/tests/test_files/file_checker_4_16_broadcasting_feature_not_used.py
+-rw-rw-rw-   0        0        0      918 2023-05-08 08:32:09.000000 mlpylint-0.0.3/tests/test_files/file_checker_4_17_tensorarray_not_used.py
+-rw-rw-rw-   0        0        0     1001 2023-06-05 12:37:31.000000 mlpylint-0.0.3/tests/test_files/file_checker_4_18_training_evaluation_mode_improper_toggling.py
+-rw-rw-rw-   0        0        0      603 2023-05-08 09:54:37.000000 mlpylint-0.0.3/tests/test_files/file_checker_4_19_pytorch_call_method_misused.py
+-rw-rw-rw-   0        0        0     2274 2023-07-21 19:39:51.000000 mlpylint-0.0.3/tests/test_files/file_checker_4_1_unnecessary_iteration.py
+-rw-rw-rw-   0        0        0     1202 2023-07-23 08:09:22.000000 mlpylint-0.0.3/tests/test_files/file_checker_4_20_gradients_not_cleared_before_backward_propagation.py
+-rw-rw-rw-   0        0        0     1621 2023-07-23 08:34:26.000000 mlpylint-0.0.3/tests/test_files/file_checker_4_21_data_leakage.py
+-rw-rw-rw-   0        0        0     1050 2023-07-25 11:52:49.000000 mlpylint-0.0.3/tests/test_files/file_checker_4_2_nan_equivalence_comparison_misused.py
+-rw-rw-rw-   0        0        0     1114 2023-06-06 15:36:23.000000 mlpylint-0.0.3/tests/test_files/file_checker_4_3_chain_indexing.py
+-rw-rw-rw-   0        0        0     2825 2023-07-26 14:21:59.000000 mlpylint-0.0.3/tests/test_files/file_checker_4_4_columns_and_datatype_not_explicitly_set.py
+-rw-rw-rw-   0        0        0     1145 2023-06-14 21:59:24.000000 mlpylint-0.0.3/tests/test_files/file_checker_4_5_empty_column_misinitialization.py
+-rw-rw-rw-   0        0        0      956 2023-04-29 18:45:40.000000 mlpylint-0.0.3/tests/test_files/file_checker_4_6_merge_api_parameter_not_explicitly_set.py
+-rw-rw-rw-   0        0        0      854 2023-06-11 10:28:02.000000 mlpylint-0.0.3/tests/test_files/file_checker_4_7_in_place_apis_misused.py
+-rw-rw-rw-   0        0        0      660 2023-06-11 12:07:03.000000 mlpylint-0.0.3/tests/test_files/file_checker_4_8_dataframe_conversion_api_misused.py
+-rw-rw-rw-   0        0        0     2173 2023-06-14 22:51:51.000000 mlpylint-0.0.3/tests/test_files/file_checker_4_9_matrix_multiplication_api_misused.py
+-rw-rw-rw-   0        0        0        2 2023-07-18 09:37:54.000000 mlpylint-0.0.3/tests/test_utils.py
```

### Comparing `mlpylint-0.0.2/LICENSE` & `mlpylint-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/PKG-INFO` & `mlpylint-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpylint
-Version: 0.0.2
+Version: 0.0.3
 Summary: MLpylint, a static analysis tool for identifying ML-specific code smells
 Author: Peter Hamfelt
 Author-email: peter.hamfelt@gmail.com
 Keywords: linting,static-analysis,python-linting,python-static-analysis,machine-learning,machine-learning-engineering,ML-model-quality,artificial-intelligence,python,software-quality,technical-debt,software-engineering,maintainability,code-smell
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -53,14 +53,29 @@
 ```
 cd mlpylint
 py -m venv venv
 source venv/Scripts/activate
 pip install -e .[dev]
 ```
 
+## Update PyPI Package
+
+```
+=== Token required from PyPI ===
+Create .pypirc file in C:\Users\<user_name> with pypi token parameters
+
+=== In project root dir ===
+py -m pip install --upgrade pip
+py -m pip install --upgrade build
+py -m build
+py -m pip install --upgrade twine
+py -m twine upload dist/*
+
+```
+
 ## Usage
 
 ```
 $ mlpylint --help                          # View tool options
 $ mlpylint <path>                          # Check for code smells (CS)
 $ mlpylint -a,  --advice <path>            # Check for code smells (CS) and include advisory results (CSA)
 $ mlpylint -ls, --list-smells              # List all available code smells
```

### Comparing `mlpylint-0.0.2/README.md` & `mlpylint-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,29 @@
 ```
 cd mlpylint
 py -m venv venv
 source venv/Scripts/activate
 pip install -e .[dev]
 ```
 
+## Update PyPI Package
+
+```
+=== Token required from PyPI ===
+Create .pypirc file in C:\Users\<user_name> with pypi token parameters
+
+=== In project root dir ===
+py -m pip install --upgrade pip
+py -m pip install --upgrade build
+py -m build
+py -m pip install --upgrade twine
+py -m twine upload dist/*
+
+```
+
 ## Usage
 
 ```
 $ mlpylint --help                          # View tool options
 $ mlpylint <path>                          # Check for code smells (CS)
 $ mlpylint -a,  --advice <path>            # Check for code smells (CS) and include advisory results (CSA)
 $ mlpylint -ls, --list-smells              # List all available code smells
```

### Comparing `mlpylint-0.0.2/mlpylint.egg-info/PKG-INFO` & `mlpylint-0.0.3/mlpylint.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpylint
-Version: 0.0.2
+Version: 0.0.3
 Summary: MLpylint, a static analysis tool for identifying ML-specific code smells
 Author: Peter Hamfelt
 Author-email: peter.hamfelt@gmail.com
 Keywords: linting,static-analysis,python-linting,python-static-analysis,machine-learning,machine-learning-engineering,ML-model-quality,artificial-intelligence,python,software-quality,technical-debt,software-engineering,maintainability,code-smell
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -53,14 +53,29 @@
 ```
 cd mlpylint
 py -m venv venv
 source venv/Scripts/activate
 pip install -e .[dev]
 ```
 
+## Update PyPI Package
+
+```
+=== Token required from PyPI ===
+Create .pypirc file in C:\Users\<user_name> with pypi token parameters
+
+=== In project root dir ===
+py -m pip install --upgrade pip
+py -m pip install --upgrade build
+py -m build
+py -m pip install --upgrade twine
+py -m twine upload dist/*
+
+```
+
 ## Usage
 
 ```
 $ mlpylint --help                          # View tool options
 $ mlpylint <path>                          # Check for code smells (CS)
 $ mlpylint -a,  --advice <path>            # Check for code smells (CS) and include advisory results (CSA)
 $ mlpylint -ls, --list-smells              # List all available code smells
```

### Comparing `mlpylint-0.0.2/mlpylint.egg-info/SOURCES.txt` & `mlpylint-0.0.3/mlpylint.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 tests/test_checkers/test_checker_4_4_columns_and_datatype_not_explicitly_set.py
 tests/test_checkers/test_checker_4_5_empty_column_misinitialization.py
 tests/test_checkers/test_checker_4_6_merge_api_parameter_not_explicitly_set.py
 tests/test_checkers/test_checker_4_7_in_place_apis_misused.py
 tests/test_checkers/test_checker_4_8_dataframe_conversion_api_misused.py
 tests/test_checkers/test_checker_4_9_matrix_multiplication_api_misused.py
 tests/test_files/__init__.py
-tests/test_files/file_checker_4_11_hyperparameter_not_explicitly_set.py
+tests/test_files/file_checker_4_11_hyperparam_not_explicitly_set.py
 tests/test_files/file_checker_4_12_memory_not_freed.py
 tests/test_files/file_checker_4_13_deterministic_algorithm_option_not_used.py
 tests/test_files/file_checker_4_14_randomness_uncontrolled.py
 tests/test_files/file_checker_4_15_missing_the_mask_of_invalid_value.py
 tests/test_files/file_checker_4_16_broadcasting_feature_not_used.py
 tests/test_files/file_checker_4_17_tensorarray_not_used.py
 tests/test_files/file_checker_4_18_training_evaluation_mode_improper_toggling.py
```

### Comparing `mlpylint-0.0.2/setup.cfg` & `mlpylint-0.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6c70 796c 696e 740d 0a76 6572   = mlpylint..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e32 0d0a 6465  sion = 0.0.2..de
+00000020: 7369 6f6e 203d 2030 2e30 2e33 0d0a 6465  sion = 0.0.3..de
 00000030: 7363 7269 7074 696f 6e20 3d20 4d4c 7079  scription = MLpy
 00000040: 6c69 6e74 2c20 6120 7374 6174 6963 2061  lint, a static a
 00000050: 6e61 6c79 7369 7320 746f 6f6c 2066 6f72  nalysis tool for
 00000060: 2069 6465 6e74 6966 7969 6e67 204d 4c2d   identifying ML-
 00000070: 7370 6563 6966 6963 2063 6f64 6520 736d  specific code sm
 00000080: 656c 6c73 0d0a 6c6f 6e67 5f64 6573 6372  ells..long_descr
 00000090: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
```

### Comparing `mlpylint-0.0.2/src/analysis/argument.py` & `mlpylint-0.0.3/src/analysis/argument.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/src/analysis/result.py` & `mlpylint-0.0.3/src/analysis/result.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/src/analysis/runner.py` & `mlpylint-0.0.3/src/analysis/runner.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/src/checkers/advice/advice_checker_4_12_memory_not_freed.py` & `mlpylint-0.0.3/src/checkers/advice/advice_checker_4_12_memory_not_freed.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/src/checkers/advice/advice_checker_4_16_broadcasting_feature_not_used.py` & `mlpylint-0.0.3/src/checkers/advice/advice_checker_4_16_broadcasting_feature_not_used.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/src/checkers/advice/advice_checker_4_18_training_evaluation_mode_improper_toggling.py` & `mlpylint-0.0.3/src/checkers/advice/advice_checker_4_18_training_evaluation_mode_improper_toggling.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/src/checkers/advice/advice_checker_4_1_unnecessary_iteration.py` & `mlpylint-0.0.3/src/checkers/advice/advice_checker_4_1_unnecessary_iteration.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/src/checkers/advice/advice_checker_4_20_gradients_not_cleared_before_backward_propagation.py` & `mlpylint-0.0.3/src/checkers/advice/advice_checker_4_20_gradients_not_cleared_before_backward_propagation.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/src/checkers/advice/advice_checker_4_21_data_leakage.py` & `mlpylint-0.0.3/src/checkers/advice/advice_checker_4_21_data_leakage.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/src/checkers/base_checker.py` & `mlpylint-0.0.3/src/checkers/base_checker.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/src/checkers/checker_4_11_hyperparameter_not_explicitly_set.py` & `mlpylint-0.0.3/src/checkers/checker_4_11_hyperparameter_not_explicitly_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,27 +45,31 @@
         self.check_hyperparam_sgd_torch(node)
 
     def check_hyperparam_kmeans_sklearn(self, node: astroid.Call) -> None:
         inferred_node = safe_infer(node)
         if (
                 inferred_node is not None
                 and isinstance(inferred_node, astroid.Instance)
-                and inferred_node.qname() == "sklearn.cluster._kmeans.KMeans"
+                and inferred_node.pytype() == "sklearn.cluster._kmeans.KMeans"
+                and isinstance(node.func, astroid.Name)
+                and node.func.name == "KMeans"
         ):
             required_args = ['n_clusters', 'random_state']
             provided_args = [keyword.arg for keyword in node.keywords]
             if not all(arg in provided_args for arg in required_args):
                 self.record_finding(node)
 
     def check_hyperparam_sgd_torch(self, node: astroid.Call) -> None:
         inferred_node = safe_infer(node)
         if (
                 inferred_node is not None
                 and isinstance(inferred_node, astroid.Instance)
-                and inferred_node.qname() == "torch.optim.sgd.SGD"
+                and inferred_node.pytype() == "torch.optim.sgd.SGD"
+                and isinstance(node.func, astroid.Name)
+                and node.func.name == "SGD"
         ):
             required_args = ['lr', 'momentum', 'weight_decay']
             provided_args = [keyword.arg for keyword in node.keywords]
             if not all(arg in provided_args for arg in required_args):
                 self.record_finding(node)
 
     def record_finding(self, node: astroid.Call) -> None:
```

### Comparing `mlpylint-0.0.2/src/checkers/checker_4_13_deterministic_algorithm_option_not_used.py` & `mlpylint-0.0.3/src/checkers/checker_4_13_deterministic_algorithm_option_not_used.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/src/checkers/checker_4_14_randomness_uncontrolled.py` & `mlpylint-0.0.3/src/checkers/checker_4_14_randomness_uncontrolled.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 class RandomnessUncontrolled(BaseChecker):
     """
     This class performs an extensive review of the Python file to detect any instances of uncontrolled randomness. It
     takes note of 'Scikit-learn's reliance on 'NumPy's random number generator. It seeks out all invocations of
     'numpy.random', 'torch.rand', and Python's 'random.random' that do not have corresponding seed set calls. In
     addition, it focuses on specific scenarios:
     1. The use of 'Scikit-learn's RandomForestClassifier without setting
-    the 'random_state' parameter and a global 'NumPy' seed.
+    the 'random_state' parameter.
     2. The use of 'PyTorch's DataLoader without setting
     'NumPy's manual seed and the 'worker_init_fn' parameter.
 
 
     Clarification:
-    1. `numpy.random.seed()`: Sets the seed for NumPy's random number generator. Affects any operation relying on NumPy
-    for randomness, including Scikit-learn.
+    1. `numpy.random.seed()`: Sets the seed for NumPy's random number generator. Affects any operation
+    relying on NumPy for randomness, including Scikit-learn.
     2. `random.seed()`: Sets the seed for Python's built-in random module. Affects Python's native random operations.
     3. `torch.manual_seed()`: Sets the seed for PyTorch's random number generator. Affects PyTorch's random operations.
-    4. Scikit-learn relies on NumPy's random number generation. Therefore, setting a seed using `numpy.random.seed()`
-    ensures deterministic behavior in Scikit-learn processes.
+    4. Scikit-learn relies on NumPy's random number generation internal. However, requires setting random_state for
+    RandomForestClassifier
     """
 
     ID = "CS14"
     TITLE = "Set random seed explicitly during the development process whenever a possible random procedure is " \
             "involved in the application. "
     DESCRIPTION = """
     Context:
@@ -162,17 +162,14 @@
                                 self.numpy_node = node
                 except astroid.InferenceError:
                     pass
 
             if isinstance(node.func.expr, astroid.Name):
                 for infer in node.func.expr.inferred():
                     if isinstance(infer, astroid.Module):
-                        # if infer.name == "numpy.random":
-                        #     self.has_call_of_numpy_random = True
-                        #     self.numpy_node = node
                         if infer.name == "random":
                             self.has_call_of_py_random = True
                             self.py_node = node
                         elif infer.name == "torch" and node.func.attrname == 'rand':
                             self.has_call_of_torch_rand = True
                             self.torch_node = node
 
@@ -231,15 +228,14 @@
         4. Code smell - Use of PyTorch's rand without setting seed
         5. Code smell - Use of Python's random without setting seed
         """
         # 1)
         if (
                 self.sklearn_random_forest_alias
                 and not self.has_sklearn_random_forest_parameter_random_state
-                and not self.has_numpy_seed
                 and self.sklearn_random_forest_node is not None
         ):
             self.record_finding(node=self.sklearn_random_forest_node)
 
         # 2)
         if (
                 self.torch_dataloader_alias
```

### Comparing `mlpylint-0.0.2/src/checkers/checker_4_15_missing_the_mask_of_invalid_value.py` & `mlpylint-0.0.3/src/checkers/checker_4_15_missing_the_mask_of_invalid_value.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/src/checkers/checker_4_17_tensorarray_not_used.py` & `mlpylint-0.0.3/src/checkers/checker_4_17_tensorarray_not_used.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/src/checkers/checker_4_19_pytorch_call_method_misused.py` & `mlpylint-0.0.3/src/checkers/checker_4_19_pytorch_call_method_misused.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/src/checkers/checker_4_2_nan_equivalence_comparison_misused.py` & `mlpylint-0.0.3/src/checkers/checker_4_2_nan_equivalence_comparison_misused.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import astroid
+from astroid.helpers import safe_infer
 
 from src.analysis.result import Result, CodeSmell
 from src.checkers.base_checker import BaseChecker
 
-COMPARISON_OP = frozenset(("<", "<=", ">", ">=", "!=", "==", "is", "is not"))  # Note: python 3.10 does not support "<>"
+COMPARISON_OP = frozenset(("<", "<=", ">", ">=", "!=", "==", "is", "is not"))
 
 
 class NaNEquivalenceComparisonMisusedChecker(BaseChecker):
     """
     This class inspects the Python code for the import of "numpy" and stores its alias. It also checks for
     'importfrom' statements related to 'numpy.nan' and keeps track of its alias. Furthermore, it reviews comparisons
     involving 'numpy.nan', utilizing the stored alias and the predicted inferred string.
@@ -55,59 +56,72 @@
                     self.numpy_nan_alias.add(node.names[0][1])
                 else:
                     self.numpy_nan_alias.add(node.names[0][0])
 
             self.has_numpy_import = True
 
     def visit_compare(self, node: astroid.Compare) -> None:
+        if not self.has_numpy_import:
+            return
+
         # Iterate compare object and search for numpy.nan occurrences and valid operator
-        # Check left and check operator
-        if node.ops[0][0] in COMPARISON_OP and self.check_nan_equivalence_misuse(node.left):
+        # Check left
+        if node.ops[0][0] in COMPARISON_OP and self.check_nan_equivalence_misuse(obj=node.left):
             self.record_finding(node=node)
             return
 
-        # Check opt and check operator
+        # Check ops
         for op, obj in node.ops:
-            if op in COMPARISON_OP and self.check_nan_equivalence_misuse(obj):
+            if (
+                op in COMPARISON_OP
+                and self.check_nan_equivalence_misuse(obj=obj)
+            ):
                 self.record_finding(node=node)
                 return
 
+        return
+        # High precision detection of nan comparison
+        # prev_obj = node.left
+        # prev_op = node.ops[0][0]
+        # for op, obj in node.ops:
+        #     if (
+        #         prev_op in COMPARISON_OP
+        #         and self.check_nan_equivalence_misuse(obj=prev_obj)
+        #         and self.check_nan_equivalence_misuse(obj=obj)
+        #     ):
+        #         self.record_finding(node=node)
+        #         return
+        #     else:
+        #         prev_op = op
+        #         prev_obj = obj
+
     def check_nan_equivalence_misuse(self, obj: astroid.NodeNG) -> bool:
         if isinstance(obj, astroid.Attribute):
             if obj.attrname in {"nan", "NaN", "NAN"} and isinstance(obj.expr, astroid.Name):
                 return self.check_attr_name(name=obj.expr)
         elif isinstance(obj, astroid.Name):
             return self.check_name(name=obj)
 
     def check_attr_name(self, name: astroid.Name) -> bool:
-        # Check if inferred value contains numpy
-        for infer in name.inferred():
-            if "numpy" in str(infer):
-                return True
-
+        inferred_node = safe_infer(name)
+        # Check if inferred node is numpy module
+        if inferred_node and inferred_node.root().name == "numpy":
+            return True
         # Check if variable name matches any of the stored numpy alias
-        if name.name in self.numpy_alias:
+        elif name.name in self.numpy_alias:
             return True
 
-    def check_name(self, name: astroid.Name) -> bool:
-        # Check if inferred value contains numpy
-        for infer in name.inferred():
-            if "numpy" in str(infer):
-                return True
+        return False
 
+    def check_name(self, name: astroid.Name) -> bool:
         # Check if variable name matches any of the stored numpy nan aliases
         if name.name in self.numpy_nan_alias:
             return True
 
-    def pylint_check_is_numpy_nan(self) -> None:
-        """
-        Pylint's implementation of detecting numpy.NaN. From version 2.17.2
-        Limited to static numpy alias names: {"numpy", "nmp", "np"} and nan alias {"NaN"}
-        """
-        pass
+        return False
 
     def record_finding(self, node: astroid.Compare) -> None:
         Result.add(CodeSmell(code_smell_id=self.ID,
                              code_smell_title="NaN Equivalence Comparison Misused",
                              file_path=self.filename,
                              line=node.lineno,
                              col_offset=node.col_offset,
```

### Comparing `mlpylint-0.0.2/src/checkers/checker_4_3_chain_indexing.py` & `mlpylint-0.0.3/src/checkers/checker_4_3_chain_indexing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import astroid
+from astroid.helpers import safe_infer
 
 from src.analysis.result import Result, CodeSmell
 from src.checkers.base_checker import BaseChecker
 
-COMPARISON_OP = frozenset(("<", "<=", ">", ">=", "!=", "==", "is", "is not"))  # Note: python 3.10 does not support "<>"
+COMPARISON_OP = frozenset(("<", "<=", ">", ">=", "!=", "==", "is", "is not"))
 
 
 class ChainIndexing(BaseChecker):
     """
     This class verifies the import of "pandas" in Python code and stores its alias. It also examines inferred strings
     associated with 'pandas' for subscript operations and ensures that the parent node is of the same subscript type.
     """
@@ -51,21 +52,22 @@
             self.has_pandas_import = True
 
     def visit_subscript(self, node: astroid.Subscript):
         if not self.has_pandas_import:
             return
 
         if isinstance(node.value, astroid.Name):
-            for inferred in node.value.inferred():
-                if (
-                        "pandas" in str(inferred)
-                        and hasattr(node, "parent")
-                        and isinstance(node.parent, astroid.Subscript)
-                ):
-                    self.record_finding(node=node)
+            inferred_node = safe_infer(node.value)
+            if (
+                    inferred_node
+                    and "pandas" in inferred_node.root().name
+                    and hasattr(node, "parent")
+                    and isinstance(node.parent, astroid.Subscript)
+            ):
+                self.record_finding(node=node)
 
     def record_finding(self, node: astroid.Subscript) -> None:
         Result.add(CodeSmell(code_smell_id=self.ID,
                              code_smell_title="Chain Indexing",
                              file_path=self.filename,
                              line=node.lineno,
                              col_offset=node.col_offset,
```

### Comparing `mlpylint-0.0.2/src/checkers/checker_4_4_columns_and_data_type_not_explicitly_set.py` & `mlpylint-0.0.3/src/checkers/checker_4_4_columns_and_data_type_not_explicitly_set.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 import astroid
+from astroid.helpers import safe_infer
 
 from src.analysis.result import Result, CodeSmell
 from src.checkers.base_checker import BaseChecker
 
+PANDAS_READ_METHODS = frozenset(("read_csv",
+                        "read_table",
+                        "read_sql",
+                        "read_xml",
+                        "read_json",
+                        "read_excel",
+                        "read_sql_query",))
+
 
 class ColumnsAndDataTypeNotExplicitlySet(BaseChecker):
     """
     This class checks function calls for the inferred "pandas" module and the presence of attribute names beginning
     with "read_". It also inspects for the explicit use of keyword arguments "columns" and "dtype" within these
     "read_" method calls.
     """
@@ -32,41 +41,36 @@
     """
 
     def __init__(self, filename):
         super().__init__(filename)
 
     def visit_call(self, node: astroid.nodes.Call):
         has_pandas_module = False
-
         if (
                 isinstance(node.func, astroid.Attribute)
                 and isinstance(node.func.expr, astroid.Name)
-                and node.func.attrname.startswith('read_')
+                and node.func.attrname in PANDAS_READ_METHODS
         ):
-            for inferred in node.func.expr.inferred():
-                if isinstance(inferred, astroid.Module) and "pandas" in inferred.name:
-                    has_pandas_module = True
-                elif "pandas" in str(inferred):
-                    has_pandas_module = True
+            inferred_node = safe_infer(node.func.expr)
+            if inferred_node and "pandas" in inferred_node.root().name:
+                has_pandas_module = True
 
         if has_pandas_module:
             self.check_explicit_columns_and_dtype(node=node)
 
     def check_explicit_columns_and_dtype(self, node: astroid.Call):
-        explicit_columns = False
-        explicit_dtype = False
+        # No check for dtype_backends, according to pandas doc "The dtype_backends are still experimential."
+        # Checking usercols and dtype is redundant. Therefore, only checking dtype keyword is set
+        has_explicit_dtype = False
 
         for keyword in node.keywords:
-            if keyword.arg == 'usecols':
-                explicit_columns = True
-
             if keyword.arg == 'dtype':
-                explicit_dtype = True
+                has_explicit_dtype = True
 
-        if not explicit_columns or not explicit_dtype:
+        if not has_explicit_dtype:
             self.record_finding(node=node)
 
     def record_finding(self, node: astroid.Call) -> None:
         Result.add(CodeSmell(code_smell_id=self.ID,
                              code_smell_title="Columns and DataType Not Explicitly Set",
                              file_path=self.filename,
                              line=node.lineno,
```

### Comparing `mlpylint-0.0.2/src/checkers/checker_4_5_empty_column_misinitialization.py` & `mlpylint-0.0.3/src/checkers/checker_4_5_empty_column_misinitialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import astroid
+from astroid.helpers import safe_infer
 
 from src.analysis.result import Result, CodeSmell
 from src.checkers.base_checker import BaseChecker
 
 
 class EmptyColumnMisinitialization(BaseChecker):
     """
@@ -74,21 +75,22 @@
         if isinstance(node.parent, astroid.Assign):
             func_name = None
 
             if (
                     isinstance(node.func, astroid.Attribute)
                     and isinstance(node.func.expr, astroid.Name)
                     and node.func.attrname == "DataFrame"
-                    and (
-                        node.func.expr.name in self.pandas_alias or
-                        any(isinstance(i, astroid.Module) and i.name == 'pandas' for i in node.func.expr.inferred())
-                    )
             ):
-                # Pandas DataFrame is called by pandas alias, pd.DataFrame()
-                func_name = node.func.attrname
+                inferred_node = safe_infer(node.func.expr)
+                if (
+                        node.func.expr.name in self.pandas_alias or
+                        (inferred_node and "pandas" in inferred_node.root().name)
+                ):
+                    # Pandas DataFrame is called by pandas alias, pd.DataFrame()
+                    func_name = node.func.attrname
             elif (
                     isinstance(node.func, astroid.Name)
                     and (
                             node.func.name in self.pandas_dataframe_alias or
                             any(isinstance(i, astroid.ClassDef) and i.name == 'DataFrame' for i in node.func.inferred())
                     )
             ):
@@ -162,15 +164,15 @@
                     if isinstance(node.value, astroid.Assign):
                         inferred_value = next(node.value.value.infer())
                     else:
                         inferred_value = next(node.value.infer())
                 except astroid.InferenceError:
                     pass
                 else:
-                    if isinstance(inferred_value, astroid.Const) and inferred_value.value in {"", 0}:
+                    if inferred_value and isinstance(inferred_value, astroid.Const) and inferred_value.value in {"", 0}:
                         self.record_finding(node=node)
 
             # Check assign to multiple subscripts
             # df['A'], df['G'], df['C'] = 0, "", ""
             # df['X'] = df['A'] = df['C'] = ""
             if isinstance(assign_target, astroid.Tuple):
                 if isinstance(node.value, astroid.Tuple):
```

### Comparing `mlpylint-0.0.2/src/checkers/checker_4_6_merge_api_parameter_not_explicitly_set.py` & `mlpylint-0.0.3/src/checkers/checker_4_6_merge_api_parameter_not_explicitly_set.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import astroid
+from astroid.helpers import safe_infer
 
 from src.analysis.result import Result, CodeSmell
 from src.checkers.base_checker import BaseChecker
 
 
 class MergeAPIParameterNotExplicitlySet(BaseChecker):
     """
@@ -36,21 +37,17 @@
 
     def __init__(self, filename):
         super().__init__(filename)
 
     def visit_call(self, node: astroid.Call):
         if isinstance(node.func, astroid.Attribute) and node.func.attrname == 'merge':
             # Check inferred object is of type "pandas"
-            if hasattr(node.func.expr, "infer"):
-                for inferred in node.func.expr.inferred():
-                    if (
-                            isinstance(inferred, astroid.Instance)
-                            and inferred.pytype() == "pandas.core.frame.DataFrame"
-                    ):
-                        self.check_merge_call(node)
+            inferred_value = safe_infer(node.func.expr)
+            if inferred_value and inferred_value.pytype() == "pandas.core.frame.DataFrame":
+                self.check_merge_call(node=node)
 
     def check_merge_call(self, node: astroid.Call):
         required_params = {'on', 'how', 'validate'}
 
         # Iterate through keyword arguments of the merge() call
         for kwarg in node.keywords:
             # If the keyword argument name is in the required_params set, remove it
```

### Comparing `mlpylint-0.0.2/src/checkers/checker_4_7_in_place_apis_misused.py` & `mlpylint-0.0.3/src/checkers/checker_4_7_in_place_apis_misused.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/src/checkers/checker_4_8_dataframe_conversion_api_misused.py` & `mlpylint-0.0.3/src/checkers/checker_4_8_dataframe_conversion_api_misused.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/src/checkers/checker_4_9_matrix_multiplication_api_misused.py` & `mlpylint-0.0.3/src/checkers/checker_4_9_matrix_multiplication_api_misused.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_checkers/test_advice_checker_4_12_memory_not_freed.py` & `mlpylint-0.0.3/tests/test_checkers/test_advice_checker_4_12_memory_not_freed.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_checkers/test_advice_checker_4_16_broadcasting_feature_not_used.py` & `mlpylint-0.0.3/tests/test_checkers/test_advice_checker_4_16_broadcasting_feature_not_used.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_checkers/test_advice_checker_4_18_training_evaluation_mode_improper_toggling.py` & `mlpylint-0.0.3/tests/test_checkers/test_advice_checker_4_18_training_evaluation_mode_improper_toggling.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_checkers/test_advice_checker_4_1_unnecessary_iteration.py` & `mlpylint-0.0.3/tests/test_checkers/test_advice_checker_4_1_unnecessary_iteration.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_checkers/test_advice_checker_4_20_gradients_not_cleared_before_backward_propagation.py` & `mlpylint-0.0.3/tests/test_checkers/test_advice_checker_4_20_gradients_not_cleared_before_backward_propagation.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_checkers/test_advice_checker_4_21_data_leakage.py` & `mlpylint-0.0.3/tests/test_checkers/test_advice_checker_4_21_data_leakage.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_checkers/test_checker_4_11_hyperparameter_not_explicitly_set.py` & `mlpylint-0.0.3/tests/test_checkers/test_checker_4_11_hyperparameter_not_explicitly_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 ROOT_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 REGISTERED_CHECKERS = [HyperparameterNotExplicitlySet]
 
 
 def test_checker_4_11_hyperparameter_not_explicitly_set():
     print(" Testing... \n")
 
-    file_path = 'file_checker_4_11_hyperparameter_not_explicitly_set.py'
+    file_path = 'file_checker_4_11_hyperparam_not_explicitly_set.py'
     absolute_file_path = os.path.join(ROOT_DIR, 'test_files', file_path)
 
     runner = Runner(path=absolute_file_path, registered_checkers=REGISTERED_CHECKERS)
     runner.run()
 
     assert len(Result.code_smells) == 2
```

### Comparing `mlpylint-0.0.2/tests/test_checkers/test_checker_4_13_deterministic_algorithm_option_not_used.py` & `mlpylint-0.0.3/tests/test_checkers/test_checker_4_13_deterministic_algorithm_option_not_used.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_checkers/test_checker_4_14_randomness_uncontrolled.py` & `mlpylint-0.0.3/tests/test_checkers/test_checker_4_14_randomness_uncontrolled.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_checkers/test_checker_4_15_missing_the_mask_of_invalid_value.py` & `mlpylint-0.0.3/tests/test_checkers/test_checker_4_15_missing_the_mask_of_invalid_value.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_checkers/test_checker_4_17_tensorarray_not_used.py` & `mlpylint-0.0.3/tests/test_checkers/test_checker_4_17_tensorarray_not_used.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_checkers/test_checker_4_19_pytorch_call_method_misused.py` & `mlpylint-0.0.3/tests/test_checkers/test_checker_4_19_pytorch_call_method_misused.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_checkers/test_checker_4_2_nan_equivalence_comparison_misused.py` & `mlpylint-0.0.3/tests/test_checkers/test_checker_4_2_nan_equivalence_comparison_misused.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_checkers/test_checker_4_3_chain_indexing.py` & `mlpylint-0.0.3/tests/test_checkers/test_checker_4_3_chain_indexing.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_checkers/test_checker_4_4_columns_and_datatype_not_explicitly_set.py` & `mlpylint-0.0.3/tests/test_checkers/test_checker_4_4_columns_and_datatype_not_explicitly_set.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_checkers/test_checker_4_5_empty_column_misinitialization.py` & `mlpylint-0.0.3/tests/test_checkers/test_checker_4_5_empty_column_misinitialization.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_checkers/test_checker_4_6_merge_api_parameter_not_explicitly_set.py` & `mlpylint-0.0.3/tests/test_checkers/test_checker_4_6_merge_api_parameter_not_explicitly_set.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_checkers/test_checker_4_7_in_place_apis_misused.py` & `mlpylint-0.0.3/tests/test_checkers/test_checker_4_7_in_place_apis_misused.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_checkers/test_checker_4_8_dataframe_conversion_api_misused.py` & `mlpylint-0.0.3/tests/test_checkers/test_checker_4_8_dataframe_conversion_api_misused.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_checkers/test_checker_4_9_matrix_multiplication_api_misused.py` & `mlpylint-0.0.3/tests/test_checkers/test_checker_4_9_matrix_multiplication_api_misused.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_files/file_checker_4_12_memory_not_freed.py` & `mlpylint-0.0.3/tests/test_files/file_checker_4_12_memory_not_freed.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_files/file_checker_4_13_deterministic_algorithm_option_not_used.py` & `mlpylint-0.0.3/tests/test_files/file_checker_4_13_deterministic_algorithm_option_not_used.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_files/file_checker_4_14_randomness_uncontrolled.py` & `mlpylint-0.0.3/tests/test_files/file_checker_4_14_randomness_uncontrolled.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_files/file_checker_4_15_missing_the_mask_of_invalid_value.py` & `mlpylint-0.0.3/tests/test_files/file_checker_4_15_missing_the_mask_of_invalid_value.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_files/file_checker_4_16_broadcasting_feature_not_used.py` & `mlpylint-0.0.3/tests/test_files/file_checker_4_16_broadcasting_feature_not_used.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_files/file_checker_4_17_tensorarray_not_used.py` & `mlpylint-0.0.3/tests/test_files/file_checker_4_17_tensorarray_not_used.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_files/file_checker_4_18_training_evaluation_mode_improper_toggling.py` & `mlpylint-0.0.3/tests/test_files/file_checker_4_18_training_evaluation_mode_improper_toggling.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_files/file_checker_4_19_pytorch_call_method_misused.py` & `mlpylint-0.0.3/tests/test_files/file_checker_4_19_pytorch_call_method_misused.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_files/file_checker_4_1_unnecessary_iteration.py` & `mlpylint-0.0.3/tests/test_files/file_checker_4_1_unnecessary_iteration.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_files/file_checker_4_20_gradients_not_cleared_before_backward_propagation.py` & `mlpylint-0.0.3/tests/test_files/file_checker_4_20_gradients_not_cleared_before_backward_propagation.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_files/file_checker_4_21_data_leakage.py` & `mlpylint-0.0.3/tests/test_files/file_checker_4_21_data_leakage.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_files/file_checker_4_3_chain_indexing.py` & `mlpylint-0.0.3/tests/test_files/file_checker_4_3_chain_indexing.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_files/file_checker_4_4_columns_and_datatype_not_explicitly_set.py` & `mlpylint-0.0.3/tests/test_files/file_checker_4_4_columns_and_datatype_not_explicitly_set.py`

 * *Files 25% similar despite different names*

```diff
@@ -53,7 +53,34 @@
 
 # Example 9: Code smell - usecols and dtype not set in a nested function call
 def process_data_without_usecols_dtype(file_path):
     return pd.read_csv(file_path)
 
 
 data9 = process_data_without_usecols_dtype('data9.csv')
+
+# Pandas read_
+# Check the following read methods
+pd.read_csv(dtype=None)
+pd.read_table(dtype=None)
+pd.read_sql(dtype=None)
+pd.read_xml(dtype=None)
+pd.read_json(dtype=None)
+pd.read_excel(dtype=None)
+pd.read_sql_query(dtype=None)
+
+pd.read_sql_query(None)  # Code Smell
+
+# No check for the following read methods (missing dtype keyword)
+# pd.read_orc(dtype_backend=)
+# pd.read_fwf(dtype_backend=)
+# pd.read_html(dtype_backend=)
+# pd.read_parquet(dtype_backend=)
+# pd.read_feather(dtype_backend=)
+# pd.read_gbq()
+# pd.read_clipboard(dtype_backend=)
+# pd.read_sql_table(dtype_backend=)
+# pd.read_sas()
+# pd.read_pickle()
+# pd.read_spss(dtype_backend=)
+# pd.read_stata(preserve_dtypes=)
+# pd.read_hdf()
```

### Comparing `mlpylint-0.0.2/tests/test_files/file_checker_4_5_empty_column_misinitialization.py` & `mlpylint-0.0.3/tests/test_files/file_checker_4_5_empty_column_misinitialization.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_files/file_checker_4_6_merge_api_parameter_not_explicitly_set.py` & `mlpylint-0.0.3/tests/test_files/file_checker_4_6_merge_api_parameter_not_explicitly_set.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_files/file_checker_4_7_in_place_apis_misused.py` & `mlpylint-0.0.3/tests/test_files/file_checker_4_7_in_place_apis_misused.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_files/file_checker_4_8_dataframe_conversion_api_misused.py` & `mlpylint-0.0.3/tests/test_files/file_checker_4_8_dataframe_conversion_api_misused.py`

 * *Files identical despite different names*

### Comparing `mlpylint-0.0.2/tests/test_files/file_checker_4_9_matrix_multiplication_api_misused.py` & `mlpylint-0.0.3/tests/test_files/file_checker_4_9_matrix_multiplication_api_misused.py`

 * *Files identical despite different names*

