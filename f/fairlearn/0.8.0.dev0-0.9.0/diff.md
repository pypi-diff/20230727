# Comparing `tmp/fairlearn-0.8.0.dev0.tar.gz` & `tmp/fairlearn-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairlearn-0.8.0.dev0.tar", last modified: Fri Oct 28 20:44:31 2022, max compression
+gzip compressed data, was "fairlearn-0.9.0.tar", last modified: Thu Jul 27 16:04:52 2023, max compression
```

## Comparing `fairlearn-0.8.0.dev0.tar` & `fairlearn-0.9.0.tar`

### file list

```diff
@@ -1,188 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.073650 fairlearn-0.8.0.dev0/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1967 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/AUTHORS.md
--rwxr-xr-x   0 runner    (1001) docker     (121)     1168 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6956 2022-10-28 20:44:31.073650 fairlearn-0.8.0.dev0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)     6237 2022-10-28 20:44:30.000000 fairlearn-0.8.0.dev0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.057649 fairlearn-0.8.0.dev0/fairlearn/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1027 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.057649 fairlearn-0.8.0.dev0/fairlearn/adversarial/
--rwxr-xr-x   0 runner    (1001) docker     (121)      333 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/adversarial/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    49677 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/adversarial/_adversarial_mitigation.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8672 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/adversarial/_backend_engine.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2345 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/adversarial/_constants.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10127 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/adversarial/_preprocessor.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8135 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/adversarial/_pytorch_engine.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6175 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/adversarial/_tensorflow_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.057649 fairlearn-0.8.0.dev0/fairlearn/datasets/
--rwxr-xr-x   0 runner    (1001) docker     (121)      570 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/datasets/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      147 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/datasets/_constants.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6498 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/datasets/_fetch_acs_income.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3551 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/datasets/_fetch_adult.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3773 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/datasets/_fetch_bank_marketing.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5989 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/datasets/_fetch_boston.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3575 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/datasets/_fetch_diabetes_hospital.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      240 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.057649 fairlearn-0.8.0.dev0/fairlearn/experimental/
--rwxr-xr-x   0 runner    (1001) docker     (121)      255 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/experimental/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      414 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/experimental/enable_metric_frame_plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.061649 fairlearn-0.8.0.dev0/fairlearn/metrics/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3050 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/metrics/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4154 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/metrics/_annotated_metric_function.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1566 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/metrics/_balanced_root_mean_squared_error.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15224 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/metrics/_disaggregated_result.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6263 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/metrics/_disparities.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8172 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/metrics/_extra_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1551 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/metrics/_generated_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2350 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/metrics/_group_feature.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8301 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/metrics/_group_metric_set.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      926 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/metrics/_input_manipulations.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5745 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/metrics/_make_derived_metric.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2544 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/metrics/_mean_predictions.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    32298 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/metrics/_metric_frame.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9252 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/metrics/_plot_model_comparison.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10045 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/metrics/_plotter.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1344 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/metrics/_selection_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.061649 fairlearn-0.8.0.dev0/fairlearn/postprocessing/
--rwxr-xr-x   0 runner    (1001) docker     (121)      548 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/postprocessing/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1058 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/postprocessing/_constants.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7865 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/postprocessing/_interpolated_thresholder.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4311 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/postprocessing/_plotting.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1792 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/postprocessing/_threshold_operation.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    29605 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/postprocessing/_threshold_optimizer.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12254 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/postprocessing/_tradeoff_curve_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.061649 fairlearn-0.8.0.dev0/fairlearn/preprocessing/
--rwxr-xr-x   0 runner    (1001) docker     (121)      255 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/preprocessing/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5022 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/preprocessing/_correlation_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.061649 fairlearn-0.8.0.dev0/fairlearn/reductions/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1338 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/reductions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.061649 fairlearn-0.8.0.dev0/fairlearn/reductions/_exponentiated_gradient/
--rwxr-xr-x   0 runner    (1001) docker     (121)      260 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/reductions/_exponentiated_gradient/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      557 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/reductions/_exponentiated_gradient/_constants.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10133 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/reductions/_exponentiated_gradient/_lagrangian.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12136 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/reductions/_exponentiated_gradient/exponentiated_gradient.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.061649 fairlearn-0.8.0.dev0/fairlearn/reductions/_grid_search/
--rwxr-xr-x   0 runner    (1001) docker     (121)      209 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/reductions/_grid_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4970 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/reductions/_grid_search/_grid_generator.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9501 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/reductions/_grid_search/grid_search.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.061649 fairlearn-0.8.0.dev0/fairlearn/reductions/_moments/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1006 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/reductions/_moments/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6010 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/reductions/_moments/bounded_group_loss.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3614 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/reductions/_moments/error_rate.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3420 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/reductions/_moments/moment.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    21173 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/reductions/_moments/utility_parity.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1871 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/show_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.061649 fairlearn-0.8.0.dev0/fairlearn/utils/
--rwxr-xr-x   0 runner    (1001) docker     (121)      127 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1923 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/utils/_common.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6691 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/fairlearn/utils/_input_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.057649 fairlearn-0.8.0.dev0/fairlearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6956 2022-10-28 20:44:31.000000 fairlearn-0.8.0.dev0/fairlearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6696 2022-10-28 20:44:31.000000 fairlearn-0.8.0.dev0/fairlearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-28 20:44:31.000000 fairlearn-0.8.0.dev0/fairlearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-28 20:44:10.000000 fairlearn-0.8.0.dev0/fairlearn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-10-28 20:44:31.000000 fairlearn-0.8.0.dev0/fairlearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-10-28 20:44:31.000000 fairlearn-0.8.0.dev0/fairlearn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      506 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (121)      742 2022-10-28 20:44:31.073650 fairlearn-0.8.0.dev0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1551 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.061649 fairlearn-0.8.0.dev0/test/
--rwxr-xr-x   0 runner    (1001) docker     (121)      100 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.061649 fairlearn-0.8.0.dev0/test/notebooks/
--rwxr-xr-x   0 runner    (1001) docker     (121)      100 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/notebooks/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3542 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/notebooks/test_notebooks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.065650 fairlearn-0.8.0.dev0/test/unit/
--rwxr-xr-x   0 runner    (1001) docker     (121)      100 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.065650 fairlearn-0.8.0.dev0/test/unit/adversarial/
--rwxr-xr-x   0 runner    (1001) docker     (121)       74 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/adversarial/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9527 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/adversarial/helper.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    17928 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/adversarial/test_adversarial_mitigation.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2982 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/adversarial/test_preprocessing.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      888 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      258 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.065650 fairlearn-0.8.0.dev0/test/unit/datasets/
--rwxr-xr-x   0 runner    (1001) docker     (121)      100 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/datasets/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2438 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/datasets/test_datasets.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      374 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/fixes.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2591 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/input_convertors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.069650 fairlearn-0.8.0.dev0/test/unit/metrics/
--rwxr-xr-x   0 runner    (1001) docker     (121)      100 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3035 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/data_for_test.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      500 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/sample_loader.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1437 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/test_annotated_metric_function.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1581 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/test_balanced_root_mean_squared_error.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12254 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/test_create_group_metric_set.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2301 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/test_disaggregated_result.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4250 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/test_disparities.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    22344 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/test_extra_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3792 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/test_generated_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2015 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/test_group_feature.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2395 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/test_input_manipulations.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8107 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/test_make_derived_metric.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2392 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/test_mean_predictions.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    76185 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/test_metricframe_aggregates.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5975 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/test_metricframe_by_group.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5152 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/test_metricframe_comprehensive.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3807 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/test_metricframe_deprecate.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5677 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/test_metricframe_missing.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1121 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/test_metricframe_multiclass.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3134 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/test_metricframe_nonscalar.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10149 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/test_metricframe_overall.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6842 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/test_metricframe_process_features.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    14453 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/test_metricframe_smoke.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5899 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/test_plot_metricframe.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7759 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/test_plot_model_comparison.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1357 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/test_selection_rate.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      288 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.069650 fairlearn-0.8.0.dev0/test/unit/postprocessing/
--rwxr-xr-x   0 runner    (1001) docker     (121)      100 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/postprocessing/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6843 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/postprocessing/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8821 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/postprocessing/test_curve_utilities.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2938 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/postprocessing/test_plots.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1723 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/postprocessing/test_smoke.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      852 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/postprocessing/test_threshold_operation.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    36257 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/postprocessing/test_threshold_optimization.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6047 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/postprocessing/test_threshold_optimizer_multiple_sensitive_features.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.069650 fairlearn-0.8.0.dev0/test/unit/preprocessing/
--rwxr-xr-x   0 runner    (1001) docker     (121)      100 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.069650 fairlearn-0.8.0.dev0/test/unit/preprocessing/linear_dep_remover/
--rwxr-xr-x   0 runner    (1001) docker     (121)      100 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/preprocessing/linear_dep_remover/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1654 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/preprocessing/linear_dep_remover/test_sklearn_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.069650 fairlearn-0.8.0.dev0/test/unit/reductions/
--rwxr-xr-x   0 runner    (1001) docker     (121)      100 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/reductions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      384 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/reductions/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      899 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/reductions/data_generators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.069650 fairlearn-0.8.0.dev0/test/unit/reductions/exponentiated_gradient/
--rwxr-xr-x   0 runner    (1001) docker     (121)      100 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/reductions/exponentiated_gradient/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1208 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/reductions/exponentiated_gradient/simple_learners.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5801 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/reductions/exponentiated_gradient/test_control_features.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8203 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/reductions/exponentiated_gradient/test_exponentiatedgradient_arguments.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    34149 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/reductions/exponentiated_gradient/test_exponentiatedgradient_smoke.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9732 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/reductions/exponentiated_gradient/test_lagrangian.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1143 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/reductions/exponentiated_gradient/test_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.069650 fairlearn-0.8.0.dev0/test/unit/reductions/grid_search/
--rwxr-xr-x   0 runner    (1001) docker     (121)      100 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/reductions/grid_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8517 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/reductions/grid_search/test_grid_generator.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    17162 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/reductions/grid_search/test_grid_search_arguments.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8660 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/reductions/grid_search/test_grid_search_demographicparity.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6082 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/reductions/grid_search/test_grid_search_regression.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1542 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/reductions/grid_search/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.069650 fairlearn-0.8.0.dev0/test/unit/reductions/moments/
--rwxr-xr-x   0 runner    (1001) docker     (121)      100 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/reductions/moments/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2336 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/reductions/moments/data_generator.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6034 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/reductions/moments/test_moments_bounded_group_loss.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4628 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/reductions/moments/test_moments_control_features.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5385 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/reductions/moments/test_moments_demographic_parity.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7415 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/reductions/moments/test_moments_equalized_odds.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      651 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/reductions/moments/test_moments_error_rate.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1678 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/reductions/test_smoke.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3121 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/test_random_state.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      584 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/test_show_versions.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      826 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test/unit/utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:44:31.073650 fairlearn-0.8.0.dev0/test_othermlpackages/
--rwxr-xr-x   0 runner    (1001) docker     (121)      100 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test_othermlpackages/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6162 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test_othermlpackages/adversarial_fairness.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6171 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test_othermlpackages/package_test_common.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1253 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test_othermlpackages/test_lightgbm.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4088 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test_othermlpackages/test_pytorch.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1726 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test_othermlpackages/test_tensorflow.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      826 2022-10-28 20:44:04.000000 fairlearn-0.8.0.dev0/test_othermlpackages/test_xgboost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.937425 fairlearn-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-27 16:04:20.000000 fairlearn-0.9.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-27 16:04:20.000000 fairlearn-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-07-27 16:04:52.937425 fairlearn-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-27 16:04:52.000000 fairlearn-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.905424 fairlearn-0.9.0/fairlearn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.909424 fairlearn-0.9.0/fairlearn/adversarial/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/adversarial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49675 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/adversarial/_adversarial_mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/adversarial/_backend_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/adversarial/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/adversarial/_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/adversarial/_pytorch_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/adversarial/_tensorflow_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.909424 fairlearn-0.9.0/fairlearn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/datasets/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/datasets/_fetch_acs_income.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/datasets/_fetch_adult.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/datasets/_fetch_bank_marketing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/datasets/_fetch_boston.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/datasets/_fetch_credit_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/datasets/_fetch_diabetes_hospital.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.909424 fairlearn-0.9.0/fairlearn/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/experimental/enable_metric_frame_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.913424 fairlearn-0.9.0/fairlearn/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/metrics/_annotated_metric_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/metrics/_base_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15313 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/metrics/_disaggregated_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/metrics/_fairness_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/metrics/_generated_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/metrics/_group_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/metrics/_make_derived_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36278 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/metrics/_metric_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9269 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/metrics/_plot_model_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/metrics/_plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.913424 fairlearn-0.9.0/fairlearn/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/postprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/postprocessing/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/postprocessing/_interpolated_thresholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/postprocessing/_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/postprocessing/_threshold_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29836 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/postprocessing/_threshold_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/postprocessing/_tradeoff_curve_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.917424 fairlearn-0.9.0/fairlearn/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/preprocessing/_correlation_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.917424 fairlearn-0.9.0/fairlearn/reductions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/reductions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.917424 fairlearn-0.9.0/fairlearn/reductions/_exponentiated_gradient/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/reductions/_exponentiated_gradient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/reductions/_exponentiated_gradient/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/reductions/_exponentiated_gradient/_lagrangian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/reductions/_exponentiated_gradient/exponentiated_gradient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.917424 fairlearn-0.9.0/fairlearn/reductions/_grid_search/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/reductions/_grid_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/reductions/_grid_search/_grid_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/reductions/_grid_search/grid_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.917424 fairlearn-0.9.0/fairlearn/reductions/_moments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/reductions/_moments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/reductions/_moments/bounded_group_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/reductions/_moments/error_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/reductions/_moments/moment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/reductions/_moments/utility_parity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/show_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.921424 fairlearn-0.9.0/fairlearn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/utils/_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/utils/_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/utils/_input_manipulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-27 16:04:20.000000 fairlearn-0.9.0/fairlearn/utils/_input_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.909424 fairlearn-0.9.0/fairlearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-07-27 16:04:52.000000 fairlearn-0.9.0/fairlearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-07-27 16:04:52.000000 fairlearn-0.9.0/fairlearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 16:04:52.000000 fairlearn-0.9.0/fairlearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 16:04:31.000000 fairlearn-0.9.0/fairlearn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-27 16:04:52.000000 fairlearn-0.9.0/fairlearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-27 16:04:52.000000 fairlearn-0.9.0/fairlearn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-27 16:04:20.000000 fairlearn-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-27 16:04:52.937425 fairlearn-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-27 16:04:20.000000 fairlearn-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.921424 fairlearn-0.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.921424 fairlearn-0.9.0/test/install/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/install/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/install/test_no_matplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/install/test_no_ml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.921424 fairlearn-0.9.0/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.921424 fairlearn-0.9.0/test/unit/adversarial/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/adversarial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/adversarial/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17916 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/adversarial/test_adversarial_mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/adversarial/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.921424 fairlearn-0.9.0/test/unit/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/datasets/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/fixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/input_convertors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.929424 fairlearn-0.9.0/test/unit/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/metrics/data_for_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/metrics/test_annotated_metric_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22343 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/metrics/test_base_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/metrics/test_disaggregated_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/metrics/test_fairness_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/metrics/test_generated_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/metrics/test_group_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/metrics/test_make_derived_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/metrics/test_mean_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76731 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/metrics/test_metricframe_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/metrics/test_metricframe_by_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/metrics/test_metricframe_comprehensive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/metrics/test_metricframe_deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/metrics/test_metricframe_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/metrics/test_metricframe_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/metrics/test_metricframe_nonscalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/metrics/test_metricframe_overall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/metrics/test_metricframe_process_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/metrics/test_metricframe_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/metrics/test_plot_metricframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/metrics/test_plot_model_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/metrics/test_selection_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.929424 fairlearn-0.9.0/test/unit/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/postprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/postprocessing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/postprocessing/test_curve_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/postprocessing/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/postprocessing/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/postprocessing/test_threshold_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36257 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/postprocessing/test_threshold_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/postprocessing/test_threshold_optimizer_multiple_sensitive_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.929424 fairlearn-0.9.0/test/unit/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.929424 fairlearn-0.9.0/test/unit/preprocessing/linear_dep_remover/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/preprocessing/linear_dep_remover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/preprocessing/linear_dep_remover/test_sklearn_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.933425 fairlearn-0.9.0/test/unit/reductions/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/data_generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.933425 fairlearn-0.9.0/test/unit/reductions/exponentiated_gradient/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/exponentiated_gradient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/exponentiated_gradient/simple_learners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/exponentiated_gradient/test_control_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/exponentiated_gradient/test_exponentiatedgradient_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34149 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/exponentiated_gradient/test_exponentiatedgradient_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/exponentiated_gradient/test_lagrangian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/exponentiated_gradient/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/exponentiated_gradient/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.933425 fairlearn-0.9.0/test/unit/reductions/grid_search/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/grid_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/grid_search/test_grid_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/grid_search/test_grid_search_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/grid_search/test_grid_search_demographicparity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/grid_search/test_grid_search_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/grid_search/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/grid_search/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.937425 fairlearn-0.9.0/test/unit/reductions/moments/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/moments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/moments/data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/moments/test_moments_bounded_group_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/moments/test_moments_control_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/moments/test_moments_demographic_parity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/moments/test_moments_equalized_odds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/moments/test_moments_error_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/reductions/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/test_random_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/test_show_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test/unit/utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:04:52.937425 fairlearn-0.9.0/test_othermlpackages/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test_othermlpackages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test_othermlpackages/adversarial_fairness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test_othermlpackages/package_test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test_othermlpackages/test_lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test_othermlpackages/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test_othermlpackages/test_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-27 16:04:20.000000 fairlearn-0.9.0/test_othermlpackages/test_xgboost.py
```

### Comparing `fairlearn-0.8.0.dev0/AUTHORS.md` & `fairlearn-0.9.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/LICENSE` & `fairlearn-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/PKG-INFO` & `fairlearn-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: fairlearn
-Version: 0.8.0.dev0
-Summary: Algorithms for mitigating unfairness in supervised machine learning
+Version: 0.9.0
+Summary: A Python package to assess and improve fairness of machine learning models.
 Home-page: https://github.com/fairlearn/fairlearn
-Author: Miroslav Dudik, Richard Edgar, Brandon Horn, Roman Lutz
-Author-email: fairlearn@microsoft.com
+Author: Miroslav Dudik, Richard Edgar, Adrin Jalali, Roman Lutz, Michael Madaio, Hilde Weerts
+Author-email: fairlearn-internal@python.org
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: customplots
 License-File: LICENSE
 License-File: AUTHORS.md
 
-|Build Status| |MIT license| |PyPI| |Discord| |StackOverflow|
+|MIT license| |PyPI| |Discord| |StackOverflow|
 
 Fairlearn
 =========
 
 Fairlearn is a Python package that empowers developers of artificial
 intelligence (AI) systems to assess their system's fairness and mitigate
 any observed unfairness issues. Fairlearn contains mitigation algorithms
@@ -107,26 +106,26 @@
 Check out our in-depth `guide on the Fairlearn
 metrics <https://fairlearn.org/main/user_guide/assessment>`__.
 
 Fairlearn algorithms
 ~~~~~~~~~~~~~~~~~~~~
 
 For an overview of our algorithms please refer to our
-`website <https://fairlearn.org/main/user_guide/mitigation.html>`__.
+`website <https://fairlearn.org/main/user_guide/mitigation/index.html>`__.
 
 Install Fairlearn
 -----------------
 
 For instructions on how to install Fairlearn check out our `Quickstart
 guide <https://fairlearn.org/main/quickstart.html>`__.
 
 Usage
 -----
 
-For common usage refer to the `Jupyter notebooks <./notebooks>`__ and
+For common usage refer to the `Jupyter notebooks <https://fairlearn.org/main/auto_examples/index.html>`__ and
 our `user guide <https://fairlearn.org/main/user_guide/index.html>`__.
 Please note that our APIs are subject to change, so notebooks downloaded
 from ``main`` may not be compatible with Fairlearn installed with
 ``pip``. In this case, please navigate the tags in the repository (e.g.
 `v0.7.0 <https://github.com/fairlearn/fairlearn/tree/v0.7.0>`__) to
 locate the appropriate version of the notebook.
 
@@ -165,16 +164,14 @@
 
 Reporting security issues
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 To report security issues please send an email to
 ``fairlearn-internal@python.org``.
 
-.. |Build Status| image:: https://dev.azure.com/responsibleai/fairlearn/_apis/build/status/Nightly?branchName=main
-   :target: https://dev.azure.com/responsibleai/fairlearn/_build/latest?definitionId=23&branchName=main
 .. |MIT license| image:: https://img.shields.io/badge/License-MIT-blue.svg
    :target: https://github.com/fairlearn/fairlearn/blob/main/LICENSE
 .. |PyPI| image:: https://img.shields.io/pypi/v/fairlearn?color=blue
    :target: https://pypi.org/project/fairlearn/
 .. |Discord| image:: https://img.shields.io/discord/840099830160031744
    :target: https://discord.gg/R22yCfgsRn
 .. |StackOverflow| image:: https://img.shields.io/badge/StackOverflow-questions-blueviolet
```

### Comparing `fairlearn-0.8.0.dev0/README.rst` & `fairlearn-0.9.0/fairlearn.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,26 @@
-|Build Status| |MIT license| |PyPI| |Discord| |StackOverflow|
+Metadata-Version: 2.1
+Name: fairlearn
+Version: 0.9.0
+Summary: A Python package to assess and improve fairness of machine learning models.
+Home-page: https://github.com/fairlearn/fairlearn
+Author: Miroslav Dudik, Richard Edgar, Adrin Jalali, Roman Lutz, Michael Madaio, Hilde Weerts
+Author-email: fairlearn-internal@python.org
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 3 - Alpha
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+
+|MIT license| |PyPI| |Discord| |StackOverflow|
 
 Fairlearn
 =========
 
 Fairlearn is a Python package that empowers developers of artificial
 intelligence (AI) systems to assess their system's fairness and mitigate
 any observed unfairness issues. Fairlearn contains mitigation algorithms
@@ -88,26 +106,26 @@
 Check out our in-depth `guide on the Fairlearn
 metrics <https://fairlearn.org/main/user_guide/assessment>`__.
 
 Fairlearn algorithms
 ~~~~~~~~~~~~~~~~~~~~
 
 For an overview of our algorithms please refer to our
-`website <https://fairlearn.org/main/user_guide/mitigation.html>`__.
+`website <https://fairlearn.org/main/user_guide/mitigation/index.html>`__.
 
 Install Fairlearn
 -----------------
 
 For instructions on how to install Fairlearn check out our `Quickstart
 guide <https://fairlearn.org/main/quickstart.html>`__.
 
 Usage
 -----
 
-For common usage refer to the `Jupyter notebooks <./notebooks>`__ and
+For common usage refer to the `Jupyter notebooks <https://fairlearn.org/main/auto_examples/index.html>`__ and
 our `user guide <https://fairlearn.org/main/user_guide/index.html>`__.
 Please note that our APIs are subject to change, so notebooks downloaded
 from ``main`` may not be compatible with Fairlearn installed with
 ``pip``. In this case, please navigate the tags in the repository (e.g.
 `v0.7.0 <https://github.com/fairlearn/fairlearn/tree/v0.7.0>`__) to
 locate the appropriate version of the notebook.
 
@@ -146,16 +164,14 @@
 
 Reporting security issues
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 To report security issues please send an email to
 ``fairlearn-internal@python.org``.
 
-.. |Build Status| image:: https://dev.azure.com/responsibleai/fairlearn/_apis/build/status/Nightly?branchName=main
-   :target: https://dev.azure.com/responsibleai/fairlearn/_build/latest?definitionId=23&branchName=main
 .. |MIT license| image:: https://img.shields.io/badge/License-MIT-blue.svg
    :target: https://github.com/fairlearn/fairlearn/blob/main/LICENSE
 .. |PyPI| image:: https://img.shields.io/pypi/v/fairlearn?color=blue
    :target: https://pypi.org/project/fairlearn/
 .. |Discord| image:: https://img.shields.io/discord/840099830160031744
    :target: https://discord.gg/R22yCfgsRn
 .. |StackOverflow| image:: https://img.shields.io/badge/StackOverflow-questions-blueviolet
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/__init__.py` & `fairlearn-0.9.0/fairlearn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import atexit
 import logging
 import os
 
 from .show_versions import show_versions  # noqa: F401
 
 __name__ = "fairlearn"
-__version__ = "0.8.0.dev0"
+__version__ = "0.9.0"
 _base_version = __version__  # To enable the v0.4.6 docs
 
 # Setup logging infrastructure
 # Only log to disk if environment variable FAIRLEARN_LOGS specified
 fairlearn_logs = os.environ.get("FAIRLEARN_LOGS")
 if fairlearn_logs is not None:
     logger = logging.getLogger(__name__)
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/adversarial/_adversarial_mitigation.py` & `fairlearn-0.9.0/fairlearn/adversarial/_adversarial_mitigation.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,15 +378,15 @@
                     expected_dist = "binary"
                 elif kw_or_func in ["square_loss", None]:
                     expected_dist = "continuous"
                 else:
                     raise ValueError(
                         _KWARG_ERROR_MESSAGE.format(
                             kwname,
-                            ("A valid keyword or a callable"),
+                            "A valid keyword or a callable",
                         )
                     )
                 return _get_type(data, expected_dist)
             else:
                 return kw_or_func
 
         self.predictor_loss_ = read_kw(Y, self.predictor_loss, "predictor_loss")
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/adversarial/_backend_engine.py` & `fairlearn-0.9.0/fairlearn/adversarial/_backend_engine.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/fairlearn/adversarial/_constants.py` & `fairlearn-0.9.0/fairlearn/adversarial/_constants.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/fairlearn/adversarial/_preprocessor.py` & `fairlearn-0.9.0/fairlearn/adversarial/_preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) Fairlearn contributors.
 # Licensed under the MIT License.
 
+import fairlearn.utils._compatibility as compat
 from ._constants import (
     _TYPE_COMPLIANCE_ERROR,
     _TYPE_CHECK_ERROR,
     _ARG_ERROR_MESSAGE,
     _TYPE_UNKNOWN_ERROR,
     _INVALID_OHE,
 )
@@ -124,15 +125,17 @@
             self.n_features_in_ = X.shape[0]
             self.n_features_out_ = X.shape[0]
 
             if self.inferred_type_ in ["binary", "multiclass"]:
                 # NOTE: if 'binary' then it could be possible it is already 0/1
                 # encoded. So may want to skip redundant OHE in that case...
                 self.transform_ = OneHotEncoder(
-                    drop="if_binary", sparse=False, handle_unknown="error"
+                    drop="if_binary",
+                    handle_unknown="error",
+                    **compat._SPARSE_OUTPUT_FALSE,
                 )
                 self.transform_.fit(X)
                 self.n_features_out_ = sum(
                     len(cat) if len(cat) != 2 else 1
                     for cat in self.transform_.categories_
                 )
             # elif "multilabel-indicator" needn't be encoded, so we do not create
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/adversarial/_pytorch_engine.py` & `fairlearn-0.9.0/fairlearn/adversarial/_pytorch_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     def get_loss(self, dist_type):
         """Get loss function corresponding to the keyword."""
         if dist_type == "binary":
             # Use sigmoid as last layer
             return torch.nn.BCELoss(reduction="mean")
         elif dist_type == "category":
             # Use logsoftmax as last layer
-            return torch.nn.NLLLoss(reduction="mean")
+            return torch.nn.CrossEntropyLoss(reduction="mean")
         elif dist_type == "continuous":
             return torch.nn.MSELoss(reduction="mean")
         super(PytorchEngine, self).get_loss(dist_type)
 
     def get_model(self, list_nodes):
         """
         Build a model from a list of keywords.
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/adversarial/_tensorflow_engine.py` & `fairlearn-0.9.0/fairlearn/adversarial/_tensorflow_engine.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/fairlearn/datasets/__init__.py` & `fairlearn-0.9.0/fairlearn/datasets/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 
 
 """This module contains datasets that can be used for benchmarking and education."""
 
 
 from ._fetch_acs_income import fetch_acs_income
 from ._fetch_adult import fetch_adult
-from ._fetch_boston import fetch_boston
 from ._fetch_bank_marketing import fetch_bank_marketing
+from ._fetch_boston import fetch_boston
+from ._fetch_credit_card import fetch_credit_card
 from ._fetch_diabetes_hospital import fetch_diabetes_hospital
 
 __all__ = [
     "fetch_acs_income",
     "fetch_adult",
-    "fetch_boston",
     "fetch_bank_marketing",
+    "fetch_boston",
+    "fetch_credit_card",
     "fetch_diabetes_hospital",
 ]
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/datasets/_fetch_acs_income.py` & `fairlearn-0.9.0/fairlearn/datasets/_fetch_acs_income.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 
 import pathlib
 
 import numpy as np
 import pandas as pd
 from sklearn.datasets import fetch_openml
 
+import fairlearn.utils._compatibility as compat
+
 from ._constants import _DOWNLOAD_DIRECTORY_NAME
 
 
 def fetch_acs_income(
     *,
     cache=True,
     data_home=None,
-    as_frame=False,
+    as_frame=True,
     return_X_y=False,
     states=None,
 ):
     """Load the ACS Income dataset (regression).
 
     Download it if necessary.
 
@@ -42,22 +44,25 @@
         Whether to cache downloaded datasets using joblib.
 
     data_home : str, default=None
         Specify another download and cache folder for the datasets.
         By default, all fairlearn data is stored in '~/.fairlearn-data'
         subfolders.
 
-    as_frame : bool, default=False
+    as_frame : bool, default=True
         If True, the data is a pandas DataFrame including columns with
         appropriate dtypes (numeric, string or categorical). The target is
         a pandas DataFrame or Series depending on the number of target_columns.
         The Bunch will contain a ``frame`` attribute with the target and the
         data. If ``return_X_y`` is True, then ``(data, target)`` will be pandas
         DataFrames or Series as describe above.
 
+        .. versionchanged:: 0.9.0
+            Default value changed to True.
+
     return_X_y : bool, default=False
         If True, returns ``(data.data, data.target)`` instead of a Bunch
         object.
 
     states: list, default=None
         List containing two letter (capitalized) state abbreviations.
         If None, data from all 50 US states and Puerto Rico will be returned.
@@ -78,20 +83,25 @@
             A threshold can be applied as a postprocessing step to frame this
             as a binary classification problem.
             If ``as_frame`` is True, ``target`` is a pandas object.
         feature_names : list of length 10
             Array of ordered feature names used in the dataset.
         DESCR : string
             Description of the ACSIncome dataset.
+        categories : dict or None
+            Maps each categorical feature name to a list of values, such that the
+            value encoded as i is ith in the list. If ``as_frame`` is True, this is None.
+        frame : pandas DataFrame
+            Only present when ``as_frame`` is True. DataFrame with ``data`` and ``target``.
 
-    (data, target) : tuple of (numpy.ndarray, numpy.ndarray)
-        if ``return_X_y`` is True and ``as_frame`` is False
+    (data, target) : tuple if ``return_X_y`` is True
 
-    (data, target) : tuple of (pandas.DataFrame, pandas.Series)
-        if ``return_X_y`` is True and ``as_frame`` is True
+    Notes
+    ----------
+    Our API largely follows the API of :func:`sklearn.datasets.fetch_openml`.
 
     References
     ----------
     .. [1] Ding, F., Hardt, M., Miller, J., & Schmidt, L. (2021).
        "Retiring Adult: New Datasets for Fair Machine Learning."
        Advances in Neural Information Processing Systems, 34.
 
@@ -177,14 +187,15 @@
     # fetch data for all 50 US states and Puerto Rico
     data_dict = fetch_openml(
         data_id=43141,
         data_home=data_home,
         cache=cache,
         as_frame=True,
         return_X_y=False,
+        **compat._PARSER_KWARG,
     )
 
     # filter by state
     df_all = data_dict["data"].copy(deep=True)
     df_all["PINCP"] = data_dict["target"]
     cols = df_all.columns
     df = pd.DataFrame(np.zeros((0, len(cols))), columns=cols)
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/datasets/_fetch_adult.py` & `fairlearn-0.9.0/fairlearn/datasets/_fetch_adult.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # Copyright (c) Microsoft Corporation and Fairlearn contributors.
 # Licensed under the MIT License.
 
 import pathlib
 
 from sklearn.datasets import fetch_openml
 
+import fairlearn.utils._compatibility as compat
+
 from ._constants import _DOWNLOAD_DIRECTORY_NAME
 
 
-def fetch_adult(*, cache=True, data_home=None, as_frame=False, return_X_y=False):
+def fetch_adult(*, cache=True, data_home=None, as_frame=True, return_X_y=False):
     """Load the UCI Adult dataset (binary classification).
 
     Read more in the :ref:`User Guide <boston_housing_data>`.
 
     Download it if necessary.
 
     ==============   ====================
@@ -37,22 +39,25 @@
         Whether to cache downloaded datasets using joblib.
 
     data_home : str, default=None
         Specify another download and cache folder for the datasets.
         By default, all fairlearn data is stored in '~/.fairlearn-data'
         subfolders.
 
-    as_frame : bool, default=False
+    as_frame : bool, default=True
         If True, the data is a pandas DataFrame including columns with
         appropriate dtypes (numeric, string or categorical). The target is
         a pandas DataFrame or Series depending on the number of target_columns.
         The Bunch will contain a ``frame`` attribute with the target and the
         data. If ``return_X_y`` is True, then ``(data, target)`` will be pandas
         DataFrames or Series as describe above.
 
+        .. versionchanged:: 0.9.0
+            Default value changed to True.
+
     return_X_y : bool, default=False
         If True, returns ``(data.data, data.target)`` instead of a Bunch
         object.
 
     Returns
     -------
     dataset : :obj:`~sklearn.utils.Bunch`
@@ -65,20 +70,25 @@
             Each value represents whether the person earns more than $50,000
             a year (>50K) or not (<=50K).
             If ``as_frame`` is True, ``target`` is a pandas object.
         feature_names : list of length 14
             Array of ordered feature names used in the dataset.
         DESCR : string
             Description of the UCI Adult dataset.
+        categories : dict or None
+            Maps each categorical feature name to a list of values, such that the
+            value encoded as i is ith in the list. If ``as_frame`` is True, this is None.
+        frame : pandas DataFrame
+            Only present when ``as_frame`` is True. DataFrame with ``data`` and ``target``.
 
-    (data, target) : tuple of (numpy.ndarray, numpy.ndarray)
-        if ``return_X_y`` is True and ``as_frame`` is False
+    (data, target) : tuple if ``return_X_y`` is True
 
-    (data, target) : tuple of (pandas.DataFrame, pandas.Series)
-        if ``return_X_y`` is True and ``as_frame`` is True
+    Notes
+    ----------
+    Our API largely follows the API of :func:`sklearn.datasets.fetch_openml`.
 
     References
     ----------
     .. [1] R. Kohavi and B. Becker, UCI Machine Learning Repository:
        Adult Data Set, 01-May-1996. [Online]. Available:
        https://archive.ics.uci.edu/ml/datasets/adult.
 
@@ -93,8 +103,9 @@
 
     return fetch_openml(
         data_id=1590,
         data_home=data_home,
         cache=cache,
         as_frame=as_frame,
         return_X_y=return_X_y,
+        **compat._PARSER_KWARG,
     )
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/datasets/_fetch_bank_marketing.py` & `fairlearn-0.9.0/fairlearn/datasets/_fetch_bank_marketing.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # Copyright (c) Microsoft Corporation and Fairlearn contributors.
 # Licensed under the MIT License.
 
 import pathlib
 
 from sklearn.datasets import fetch_openml
 
+import fairlearn.utils._compatibility as compat
+
 from ._constants import _DOWNLOAD_DIRECTORY_NAME
 
 
 def fetch_bank_marketing(
-    *, cache=True, data_home=None, as_frame=False, return_X_y=False
+    *, cache=True, data_home=None, as_frame=True, return_X_y=False
 ):
     """Load the UCI bank marketing dataset (binary classification).
 
     Download it if necessary.
 
     ==============   ====================
     Samples total                   45211
-    Dimensionality                     17
+    Dimensionality                     16
     Features         numeric, categorical
     Classes                             2
     ==============   ====================
 
     Source: UCI Repository [3]_ Paper: Moro et al., 2014 [4]_
 
     The data is related with direct marketing campaigns of a Portuguese
@@ -40,49 +42,57 @@
         Whether to cache downloaded datasets using joblib.
 
     data_home : str, default=None
         Specify another download and cache folder for the datasets.
         By default, all fairlearn data is stored in '~/.fairlearn-data'
         subfolders.
 
-    as_frame : bool, default=False
+    as_frame : bool, default=True
         If True, the data is a pandas DataFrame including columns with
         appropriate dtypes (numeric, string or categorical). The target is
         a pandas DataFrame or Series depending on the number of target_columns.
         The Bunch will contain a ``frame`` attribute with the target and the
         data. If ``return_X_y`` is True, then ``(data, target)`` will be pandas
         DataFrames or Series as describe above.
 
+        .. versionchanged:: 0.9.0
+            Default value changed to True.
+
     return_X_y : bool, default=False
         If True, returns ``(data.data, data.target)`` instead of a Bunch
         object.
 
     Returns
     -------
     dataset : :obj:`~sklearn.utils.Bunch`
         Dictionary-like object, with the following attributes.
 
-        data : ndarray, shape (45211, 17)
-            Each row corresponding to the 17 feature values in order.
+        data : ndarray, shape (45211, 16)
+            Each row corresponding to the 16 feature values in order.
             If ``as_frame`` is True, ``data`` is a pandas object.
         target : numpy array of shape (45211,)
             Each value represents whether the client subscribed a
             term deposit which is 'yes' if the client subscribed and 'no'
             otherwise.
             If ``as_frame`` is True, ``target`` is a pandas object.
-        feature_names : list of length 17
+        feature_names : list of length 16
             Array of ordered feature names used in the dataset.
         DESCR : string
             Description of the UCI bank marketing dataset.
+        categories : dict or None
+            Maps each categorical feature name to a list of values, such that the
+            value encoded as i is ith in the list. If ``as_frame`` is True, this is None.
+        frame : pandas DataFrame
+            Only present when ``as_frame`` is True. DataFrame with ``data`` and ``target``.
 
-    (data, target) : tuple of (numpy.ndarray, numpy.ndarray)
-        if ``return_X_y`` is True and ``as_frame`` is False
+    (data, target) : tuple if ``return_X_y`` is True
 
-    (data, target) : tuple of (pandas.DataFrame, pandas.Series)
-        if ``return_X_y`` is True and ``as_frame`` is True
+    Notes
+    ----------
+    Our API largely follows the API of :func:`sklearn.datasets.fetch_openml`.
 
     References
     ----------
     .. [3] S. Moro, P. Cortez, and P. Rita, UCI Machine Learning Repository:
        Bank Marketing Data Set, 14-Feb-2014. [Online]. Available:
        https://archive.ics.uci.edu/ml/datasets/Bank+Marketing.
 
@@ -96,8 +106,9 @@
 
     return fetch_openml(
         data_id=1461,
         data_home=data_home,
         cache=cache,
         as_frame=as_frame,
         return_X_y=return_X_y,
+        **compat._PARSER_KWARG,
     )
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/datasets/_fetch_boston.py` & `fairlearn-0.9.0/fairlearn/datasets/_fetch_boston.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 # Licensed under the MIT License.
 
 import pathlib
 import warnings
 
 from sklearn.datasets import fetch_openml
 
+import fairlearn.utils._compatibility as compat
 from fairlearn.exceptions import DataFairnessWarning
 
 from ._constants import _DOWNLOAD_DIRECTORY_NAME
 
 
 def fetch_boston(
-    *, cache=True, data_home=None, as_frame=False, return_X_y=False, warn=True
+    *, cache=True, data_home=None, as_frame=True, return_X_y=False, warn=True
 ):
     """Load the boston housing dataset (regression).
 
     Download it if necessary.
 
     ==============   ==============
     Samples total               506
@@ -67,22 +68,25 @@
         Whether to cache downloaded datasets using joblib.
 
     data_home : str, default=None
         Specify another download and cache folder for the datasets.
         By default, all fairlearn data is stored in '~/.fairlearn-data'
         subfolders.
 
-    as_frame : bool, default=False
+    as_frame : bool, default=True
         If True, the data is a pandas DataFrame including columns with
         appropriate dtypes (numeric, string or categorical). The target is
         a pandas DataFrame or Series depending on the number of target_columns.
         The Bunch will contain a ``frame`` attribute with the target and the
         data. If ``return_X_y`` is True, then ``(data, target)`` will be pandas
         DataFrames or Series as describe above.
 
+        .. versionchanged:: 0.9.0
+            Default value changed to True.
+
     return_X_y : bool, default=False
         If True, returns ``(data.data, data.target)`` instead of a Bunch
         object.
 
     warn : bool, default=True
         If True, it raises an extra warning to make users aware of the unfairness
         aspect of this dataset.
@@ -100,23 +104,25 @@
             Each value corresponds to the average
             house value in units of 100,000.
             If ``as_frame`` is True, ``target`` is a pandas object.
         feature_names : list of length 13
             Array of ordered feature names used in the dataset.
         DESCR : string
             Description of the Boston housing dataset.
+        categories : dict or None
+            Maps each categorical feature name to a list of values, such that the
+            value encoded as i is ith in the list. If ``as_frame`` is True, this is None.
+        frame : pandas DataFrame
+            Only present when ``as_frame`` is True. DataFrame with ``data`` and ``target``.
 
-    (data, target) : tuple of (numpy.ndarray, numpy.ndarray)
-        if ``return_X_y`` is True and ``as_frame`` is False
-
-    (data, target) : tuple of (pandas.DataFrame, pandas.Series)
-        if ``return_X_y`` is True and ``as_frame`` is True
+    (data, target) : tuple if ``return_X_y`` is True
 
     Notes
     -----
+    Our API largely follows the API of :func:`sklearn.datasets.fetch_openml`.
     This dataset consists of 506 samples and 13 features. It is notorious for the fairness
     issues related to the `B` column. There's more information in the references.
 
     References
     ----------
     .. [5] J. Vanschoren, "boston," OpenML, 29-Sep-2014. [Online]. Available:
        https://www.openml.org/d/531.
@@ -146,8 +152,9 @@
         data_home = pathlib.Path().home() / _DOWNLOAD_DIRECTORY_NAME
     return fetch_openml(
         data_id=531,
         data_home=data_home,
         cache=cache,
         as_frame=as_frame,
         return_X_y=return_X_y,
+        **compat._PARSER_KWARG,
     )
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/datasets/_fetch_diabetes_hospital.py` & `fairlearn-0.9.0/fairlearn/datasets/_fetch_diabetes_hospital.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # Copyright (c) Fairlearn contributors.
 # Licensed under the MIT License.
 
 import pathlib
 
 from sklearn.datasets import fetch_openml
+
+import fairlearn.utils._compatibility as compat
+
 from ._constants import _DOWNLOAD_DIRECTORY_NAME
 
 
 def fetch_diabetes_hospital(
-    *, cache=True, data_home=None, return_X_y=False
+    *, as_frame=True, cache=True, data_home=None, return_X_y=False
 ):
     """Load the preprocessed Diabetes 130-Hospitals dataset (binary classification).
 
     Download it if necessary.
 
     ==============   ============================
     Samples total                          101766
-    Dimensionality                             25
+    Dimensionality                             24
     Features         numeric, categorical, string
     Classes                                     2
     ==============   ============================
 
     Source: UCI Repository :footcite:`strack2014diabetes`
     Paper: Strack et al., 2014 :footcite:`strack2014impact`
 
@@ -38,23 +41,28 @@
     Fairlearn". In this version, the target variable "readmitted" is binarized
     into whether the patient was re-admitted within thirty days. The full
     pre-processing script is available
     `here <https://github.com/fairlearn/talks/blob/main/2021_scipy_tutorial/preprocess.py>`_.
 
     Read more in the :ref:`User Guide <diabetes_hospital_data>`.
 
-    .. note::
-        The dataset is always returned as a pandas object, because string
-        attributes are not supported for array representation, resulting
-        in a `ValueError`.
-
     .. versionadded:: 0.8.0
 
     Parameters
     ----------
+    as_frame : bool, default=True
+        If True, the data is a pandas DataFrame including columns with
+        appropriate dtypes (numeric, string or categorical).
+
+        .. note::
+            If set to False, this will raise an exception because of a type mismatch
+            in the OpenML dataset.
+
+        .. versionadded:: 0.9.0
+
     cache : bool, default=True
         Whether to cache downloaded datasets using joblib.
 
     data_home : str, default=None
         Specify another download and cache folder for the datasets.
         By default, all fairlearn data is stored in '~/.fairlearn-data'
         subfolders.
@@ -62,38 +70,47 @@
     return_X_y : bool, default=False
         If True, returns ``(data.data, data.target)`` instead of a Bunch
         object.
 
     Returns
     -------
     dataset : :obj:`~sklearn.utils.Bunch`
-        Dictionary-like object, with the following attributes.
+        Dictionary-like object, with the following attributes:
 
-        data : ndarray, shape (101766, 25)
-            Each row corresponding to the 25 feature values in order.
+        data : ndarray, shape (101766, 24)
+            Each row corresponding to the 24 feature values in order.
             If ``as_frame`` is True, ``data`` is a pandas object.
         target : numpy array of shape (101766,)
             Each value represents whether readmission of the patient
             occurred within 30 days of the release.
-        feature_names : list of length 25
+        feature_names : list of length 24
             Array of ordered feature names used in the dataset.
         DESCR : string
             Description of the Diabetes 130-Hospitals dataset.
+        categories : dict or None
+            Maps each categorical feature name to a list of values, such that the
+            value encoded as i is ith in the list. If ``as_frame`` is True, this is None.
+        frame : pandas DataFrame
+            Only present when ``as_frame`` is True. DataFrame with ``data`` and ``target``.
+
+    (data, target) : tuple if ``return_X_y`` is True
 
-    (data, target) : tuple of (pandas.DataFrame, pandas.Series)
-        if ``return_X_y`` is True
+    Notes
+    ----------
+    Our API largely follows the API of :func:`sklearn.datasets.fetch_openml`.
 
     References
     ----------
     .. footbibliography::
 
     """
     if not data_home:
         data_home = pathlib.Path().home() / _DOWNLOAD_DIRECTORY_NAME
 
     return fetch_openml(
         data_id=43874,
         data_home=data_home,
         cache=cache,
-        as_frame=True,
+        as_frame=as_frame,
         return_X_y=return_X_y,
+        **compat._PARSER_KWARG,
     )
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/metrics/__init__.py` & `fairlearn-0.9.0/fairlearn/metrics/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,60 +21,54 @@
 subgroups.
 This extends to multiple grouping columns, calculating the metric
 for each combination of subgroups.
 """
 
 import sys as _sys
 
-from ._disparities import demographic_parity_difference  # noqa: F401
-from ._disparities import demographic_parity_ratio  # noqa: F401
-from ._disparities import equalized_odds_difference, equalized_odds_ratio  # noqa: F401
-from ._extra_metrics import _balanced_root_mean_squared_error  # noqa: F401
-from ._extra_metrics import _mean_overprediction  # noqa: F401
-from ._extra_metrics import _mean_underprediction  # noqa: F401
-from ._extra_metrics import count  # noqa: F401
-from ._extra_metrics import false_negative_rate  # noqa: F401
-from ._extra_metrics import false_positive_rate  # noqa: F401
-from ._extra_metrics import mean_prediction  # noqa: F401
-from ._extra_metrics import selection_rate  # noqa: F401
-from ._extra_metrics import true_negative_rate  # noqa: F401
-from ._extra_metrics import true_positive_rate  # noqa: F401; noqa: F401
+from ._base_metrics import count  # noqa: F401
+from ._base_metrics import false_negative_rate  # noqa: F401
+from ._base_metrics import false_positive_rate  # noqa: F401
+from ._base_metrics import mean_prediction  # noqa: F401
+from ._base_metrics import selection_rate  # noqa: F401
+from ._base_metrics import true_negative_rate  # noqa: F401
+from ._base_metrics import true_positive_rate  # noqa: F401; noqa: F401
+from ._fairness_metrics import demographic_parity_difference  # noqa: F401
+from ._fairness_metrics import demographic_parity_ratio  # noqa: F401
+from ._fairness_metrics import equalized_odds_difference  # noqa: F401
+from ._fairness_metrics import equalized_odds_ratio  # noqa: F401
 from ._generated_metrics import _generated_metric_dict  # noqa: F401
 from ._make_derived_metric import make_derived_metric  # noqa: F401
 from ._metric_frame import MetricFrame  # noqa: F401
 from ._plot_model_comparison import plot_model_comparison  # noqa: F401
 
 # Add the generated metrics of the form and
 # `<metric>_{difference,ratio,group_min,group_max`
 _module_obj = _sys.modules[__name__]
 for _name, _func in _generated_metric_dict.items():
     setattr(_module_obj, _name, _func)
 
 # ============================================
 # Build list of items to be listed in the docs
 
-_core = [
-    "MetricFrame",
-    "make_derived_metric",
-    "plot_model_comparison"
-]
+_core = ["MetricFrame", "make_derived_metric", "plot_model_comparison"]
 
-_disparities = [
+_fairness = [
     "demographic_parity_difference",
     "demographic_parity_ratio",
     "equalized_odds_difference",
     "equalized_odds_ratio",
 ]
 
-_extra_metrics = [
+_base_metrics = [
     "true_positive_rate",
     "true_negative_rate",
     "false_positive_rate",
     "false_negative_rate",
     "mean_prediction",
     "selection_rate",
     "count",
 ]
 
 __all__ = (
-    _core + _disparities + _extra_metrics + list(sorted(_generated_metric_dict.keys()))
+    _core + _fairness + _base_metrics + list(sorted(_generated_metric_dict.keys()))
 )
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/metrics/_annotated_metric_function.py` & `fairlearn-0.9.0/fairlearn/metrics/_annotated_metric_function.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/fairlearn/metrics/_disaggregated_result.py` & `fairlearn-0.9.0/fairlearn/metrics/_disaggregated_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,19 @@
     The incoming DataFrame may have been sliced via `groupby()`.
     This function applies each annotated function in turn to the
     supplied DataFrame.
     """
     values = dict()
     for function_name, metric_function in metric_functions.items():
         values[function_name] = metric_function(data)
-    result = pd.Series(data=values.values(), index=values.keys())
+    # correctly handle zero provided metrics
+    if len(values) == 0:
+        result = pd.Series(dtype=float)
+    else:
+        result = pd.Series(values)
     return result
 
 
 class DisaggregatedResult:
     """Pickier version of MetricFrame.
 
     This holds the internal result from a disaggregated metric
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/metrics/_disparities.py` & `fairlearn-0.9.0/fairlearn/metrics/_fairness_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) Microsoft Corporation and Fairlearn contributors.
 # Licensed under the MIT License.
 
-"""Metrics for measuring disparity."""
+"""Metrics for measuring fairness."""
 
-from ._extra_metrics import false_positive_rate, selection_rate, true_positive_rate
+from ._base_metrics import false_positive_rate, selection_rate, true_positive_rate
 from ._metric_frame import MetricFrame
 
 
 def demographic_parity_difference(
     y_true, y_pred, *, sensitive_features, method="between_groups", sample_weight=None
 ) -> float:
     """Calculate the demographic parity difference.
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/metrics/_extra_metrics.py` & `fairlearn-0.9.0/fairlearn/metrics/_base_metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # Copyright (c) Microsoft Corporation and Fairlearn contributors.
 # Licensed under the MIT License.
 
-"""A variety of extra metrics useful for assessing fairness.
+"""A variety of base metrics useful for assessing fairness.
 
 These are metrics which are not part of `scikit-learn`.
 """
 
 import numpy as np
 import sklearn.metrics as skm
+from typing import Any
 
-from ._balanced_root_mean_squared_error import (  # noqa: F401
-    _balanced_root_mean_squared_error,
-)
-from ._mean_predictions import _mean_overprediction  # noqa: F401,E501
-from ._mean_predictions import _mean_underprediction, mean_prediction  # noqa: F401
 from ._metric_frame import check_consistent_length
-from ._selection_rate import selection_rate  # noqa: F401,E501
+from fairlearn.utils._input_manipulations import _convert_to_ndarray_and_squeeze
 
+_EMPTY_INPUT_PREDICTIONS_ERROR_MESSAGE = (
+    "Empty y_pred passed to selection_rate function."
+)
 _TOO_MANY_UNIQUE_Y_VALS = "Must have no more than two unique y values"
 _RESTRICTED_VALS_IF_POS_LABEL_NONE = (
     "If pos_label is not specified, values must be from {0, 1} or {-1, 1}"  # noqa: E501
 )
 _NEED_POS_LABEL_IN_Y_VALS = "Must have pos_label in y values"
 
 
@@ -234,19 +233,14 @@
         sample_weight=sample_weight,
         labels=unique_labels,
         normalize="true",
     ).ravel()
     return fnr
 
 
-def _root_mean_squared_error(y_true, y_pred, **kwargs):
-    r"""Calculate the root mean squared error."""
-    return skm.mean_squared_error(y_true, y_pred, squared=False, **kwargs)
-
-
 def count(y_true, y_pred) -> int:
     r"""Calculate the number of data points in each group when working with `MetricFrame`.
 
     The ``y_true`` argument is used to make this calculation. For consistency with
     other metric functions, the ``y_pred`` argument is required, but ignored.
 
     Read more in the :ref:`User Guide <assessment>`.
@@ -262,7 +256,65 @@
     Returns
     -------
     int
         The number of data points in each group.
     """
     check_consistent_length(y_true, y_pred)
     return len(y_true)
+
+
+def mean_prediction(y_true, y_pred, sample_weight=None) -> float:
+    r"""Calculate the (weighted) mean prediction.
+
+    The true values are ignored, but required as an argument in order
+    to maintain a consistent interface
+
+    Parameters
+    ----------
+    y_true : array_like
+        The true labels (ignored)
+
+    y_pred : array_like
+        The predicted labels
+
+    sample_weight : array_like
+        Optional array of sample weights
+    """
+    y_p = _convert_to_ndarray_and_squeeze(y_pred)
+    s_w = np.ones(len(y_p))
+    if sample_weight is not None:
+        s_w = _convert_to_ndarray_and_squeeze(sample_weight)
+
+    return np.dot(y_p, s_w) / s_w.sum()
+
+
+def selection_rate(y_true, y_pred, *, pos_label: Any = 1, sample_weight=None) -> float:
+    """Calculate the fraction of predicted labels matching the 'good' outcome.
+
+    The argument `pos_label` specifies the 'good' outcome. For consistency with
+    other metric functions, the ``y_true`` argument is required, but ignored.
+
+    Read more in the :ref:`User Guide <custom_fairness_metrics>`.
+
+    Parameters
+    ----------
+    y_true : array_like
+        The true labels (ignored)
+
+    y_pred : array_like
+        The predicted labels
+
+    pos_label : Scalar
+        The label to treat as the 'good' outcome
+
+    sample_weight : array_like
+        Optional array of sample weights
+    """
+    selected = _convert_to_ndarray_and_squeeze(y_pred) == pos_label
+    if len(selected) == 0:
+        raise ValueError(_EMPTY_INPUT_PREDICTIONS_ERROR_MESSAGE)
+
+    s_w = np.ones(len(selected))
+    if sample_weight is not None:
+        s_w = np.squeeze(np.asarray(sample_weight))
+
+    return np.dot(selected, s_w) / s_w.sum()
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/metrics/_generated_metrics.py` & `fairlearn-0.9.0/fairlearn/metrics/_generated_metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Copyright (c) Microsoft Corporation and Fairlearn contributors.
 # Licensed under the MIT License.
 
 import sklearn.metrics as skm
 
-from ._extra_metrics import (
+from ._base_metrics import (
     false_negative_rate,
     false_positive_rate,
     selection_rate,
     true_negative_rate,
     true_positive_rate,
 )
 from ._make_derived_metric import make_derived_metric
 
 METRICS_SPEC = [
-    # base metrics from _extra_metrics
+    # base metrics from _base_metrics
     (true_positive_rate, ["difference", "ratio"]),
     (true_negative_rate, ["difference", "ratio"]),
     (false_positive_rate, ["difference", "ratio"]),
     (false_negative_rate, ["difference", "ratio"]),
     (selection_rate, ["difference", "ratio"]),
     # base metrics from sklearn.metrics
     (skm.accuracy_score, ["difference", "ratio", "group_min"]),
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/metrics/_group_feature.py` & `fairlearn-0.9.0/fairlearn/metrics/_group_feature.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/fairlearn/metrics/_input_manipulations.py` & `fairlearn-0.9.0/fairlearn/utils/_input_manipulations.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 
 import numpy as np
 
 _ARRAY_NOT_1D = "Supplied input array has more than one non-trivial dimension"
 
 
 def _convert_to_ndarray_and_squeeze(target):
-    """Convert input to a `numpy.ndarray` and calls squeeze (to dispose of unit length dimensions).
+    """
+    Convert input to a `numpy.ndarray` and calls squeeze (to dispose of unit length dimensions).
 
+    There is a special case for empty.
     There is a special case to stop single element arrays being converted to scalars.
     """
     result = np.asarray(target)
-
-    if result.size > 1:
+    if result.size == 0:
+        result = result
+    elif result.size > 1:
         result = np.squeeze(result)
     else:
         result = result.reshape(1)
 
     return result
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/metrics/_make_derived_metric.py` & `fairlearn-0.9.0/fairlearn/metrics/_make_derived_metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     def __init__(
         self,
         *,
         metric: Callable[..., Union[float, int]],
         transform: str,
         sample_param_names: List[str],
     ):
-
         if not callable(metric):
             raise ValueError(_METRIC_CALLABLE_ERROR)
         sig = inspect.signature(metric)
 
         for param_name in parameters_for_transforms:
             if param_name in sig.parameters:
                 raise ValueError(_METHOD_ARG_ERROR.format(param_name))
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/metrics/_metric_frame.py` & `fairlearn-0.9.0/fairlearn/metrics/_metric_frame.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,18 +6,22 @@
 from functools import wraps
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import numpy as np
 import pandas as pd
 from sklearn.utils import check_consistent_length
 
-from fairlearn.metrics._input_manipulations import _convert_to_ndarray_and_squeeze
+from fairlearn.utils._input_manipulations import _convert_to_ndarray_and_squeeze
 
 from ._annotated_metric_function import AnnotatedMetricFunction
-from ._disaggregated_result import DisaggregatedResult
+from ._disaggregated_result import (
+    DisaggregatedResult,
+    _VALID_ERROR_STRING,
+    _INVALID_ERRORS_VALUE_ERROR_MESSAGE,
+)
 from ._group_feature import GroupFeature
 
 logger = logging.getLogger(__name__)
 
 _SF_DICT_CONVERSION_FAILURE = (
     "DataFrame.from_dict() failed on sensitive features. "
     "Please ensure each array is strictly 1-D. "
@@ -30,14 +34,17 @@
 _DUPLICATE_FEATURE_NAME = "Detected duplicate feature name: '{0}'"
 _TOO_MANY_FEATURE_DIMS = "Feature array has too many dimensions"
 _SAMPLE_PARAMS_NOT_DICT = "Sample parameters must be a dictionary"
 _SAMPLE_PARAM_KEYS_NOT_IN_FUNC_DICT = (
     "Keys in 'sample_params' do not match those in 'metric'"
 )
 
+_COMPARE_METHODS = ["between_groups", "to_overall"]
+_INVALID_COMPARE_METHOD = "Unrecognised comparison method: {0}"
+
 
 def _deprecate_metric_frame_init(new_metric_frame_init):
     """Issue deprecation warnings for the `MetricFrame` constructor.
 
     Decorator to issue warnings if called with positional arguments
     or with the keyword argument `metric` instead of `metrics`.
 
@@ -64,30 +71,34 @@
                 "were given"
             )
 
         # If 1-3 positional arguments are provided (apart fom self), issue warning.
         if len(args) > 0:
             args_msg = ", ".join([f"'{name}'" for name in positional_dict.keys()])
             warnings.warn(
-                f"You have provided {args_msg} as positional arguments. "
-                "Please pass them as keyword arguments. From version "
-                f"{version} passing them as positional arguments "
-                "will result in an error.",
+                (
+                    f"You have provided {args_msg} as positional arguments. "
+                    "Please pass them as keyword arguments. From version "
+                    f"{version} passing them as positional arguments "
+                    "will result in an error."
+                ),
                 FutureWarning,
             )
 
         # If a keyword argument `metric` is provided, issue warning.
         metric_arg_dict = {}
         if metric is not None:
             metric_arg_dict = {"metrics": metric}
             warnings.warn(
-                "The positional argument 'metric' has been replaced "
-                "by a keyword argument 'metrics'. "
-                f"From version {version} passing it as a positional argument "
-                "or as a keyword argument 'metric' will result in an error",
+                (
+                    "The positional argument 'metric' has been replaced "
+                    "by a keyword argument 'metrics'. "
+                    f"From version {version} passing it as a positional argument "
+                    "or as a keyword argument 'metric' will result in an error"
+                ),
                 FutureWarning,
             )
 
         # Call the new constructor with positional arguments passed as keyword arguments
         # and with the `metric` keyword argument renamed to `metrics`.
         new_metric_frame_init(self, **metric_arg_dict, **positional_dict, **kwargs)
 
@@ -319,22 +330,113 @@
         if self._cf_names:
             namelist = namelist + self._cf_names
         for name in namelist:
             if name in nameset:
                 raise ValueError(_DUPLICATE_FEATURE_NAME.format(name))
             nameset.add(name)
 
-        # Create the 'overall' results
-        self._result = DisaggregatedResult.create(
+        # Create the basic results
+        result = DisaggregatedResult.create(
             data=all_data,
             annotated_functions=annotated_funcs,
             sensitive_feature_names=self._sf_names,
             control_feature_names=self._cf_names,
         )
 
+        # Build into cache
+        self._result_cache = dict()
+        self._populate_results(result)
+
+    def _extract_result(self, underlying_result, no_control_levels: bool):
+        """
+        Change result types for those who dislike consistency.
+
+        The `no_control_levels` parameter determines whether the presence
+        of control levels will affect the result. This is the case for
+        overall, but not the other cases.
+        """
+        if self._user_supplied_callable:
+            if self.control_levels or no_control_levels:
+                return underlying_result.iloc[:, 0]
+            else:
+                return underlying_result.iloc[0]
+        else:
+            return underlying_result
+
+    def _none_to_nan(
+        self, target: Union[pd.Series, pd.DataFrame]
+    ) -> Union[pd.Series, pd.DataFrame]:
+        """Convert Nones to NaNs."""
+        if isinstance(target, pd.Series):
+            result = target.map(lambda x: x if x is not None else np.nan)
+        else:
+            result = target.applymap(lambda x: x if x is not None else np.nan)
+        return result
+
+    def _populate_results(self, raw_result: DisaggregatedResult):
+        """
+        Populate the :code:`_result_cache`.
+
+        We cache all possible results from :class:`~MetricFrame` internally
+        (i.e. all possible calls to :meth:`~MetricFrame.difference()` etc.)
+        and this method is responsible for performing those computations.
+        The :code:`_result_cache` is a nested dictionary, with keys given by
+        the method names and arguments being cached.
+
+        Note that if exceptions are thrown, we cache those, and they are thrown
+        if the user calls the corresponding method (and arguments).
+        """
+        # Start with overall
+        self._result_cache["overall"] = self._extract_result(
+            raw_result.overall, no_control_levels=False
+        )
+
+        # Now do by_group
+        self._result_cache["by_group"] = self._extract_result(
+            raw_result.by_group, no_control_levels=True
+        )
+
+        # Next up, group_min and group_max
+        group_functions = {"group_min": "min", "group_max": "max"}
+        for k, v in group_functions.items():
+            self._result_cache[k] = dict()
+            for err_string in _VALID_ERROR_STRING:
+                try:
+                    self._result_cache[k][err_string] = self._group(
+                        raw_result, v, err_string
+                    )
+                except Exception as e:  # noqa: B902
+                    # Store any exception for later
+                    self._result_cache[k][err_string] = e
+
+        # Differences and ratios
+        for c_t in ["difference", "ratio"]:
+            self._result_cache[c_t] = dict()
+            for c_m in _COMPARE_METHODS:
+                self._result_cache[c_t][c_m] = dict()
+                for err_string in _VALID_ERROR_STRING:
+                    try:
+                        if c_t == "difference":
+                            tmp = raw_result.difference(
+                                self.control_levels, method=c_m, errors=err_string
+                            )
+                        else:
+                            tmp = raw_result.ratio(
+                                self.control_levels, method=c_m, errors=err_string
+                            )
+
+                        result = self._none_to_nan(tmp)
+
+                        self._result_cache[c_t][c_m][err_string] = self._extract_result(
+                            result, no_control_levels=False
+                        )
+                    except Exception as e:  # noqa: B902
+                        # Store any exception for later
+                        self._result_cache[c_t][c_m][err_string] = e
+
     @property
     def overall(self) -> Union[Any, pd.Series, pd.DataFrame]:
         """Return the underlying metrics evaluated on the whole dataset.
 
         Read more in the :ref:`User Guide <assessment_quantify_harms>`.
 
         Returns
@@ -360,21 +462,15 @@
             ======== ================  =================================
 
             The distinction applies even if the dictionary contains a
             single metric function. This is to allow for a consistent
             interface when calling programatically, while also reducing
             typing for those using Fairlearn interactively.
         """
-        if self._user_supplied_callable:
-            if self.control_levels:
-                return self._result.overall.iloc[:, 0]
-            else:
-                return self._result.overall.iloc[0]
-        else:
-            return self._result.overall
+        return self._result_cache["overall"]
 
     @property
     def by_group(self) -> Union[pd.Series, pd.DataFrame]:
         """Return the collection of metrics evaluated for each subgroup.
 
         The collection is defined by the combination of classes in the
         sensitive and control features. The exact type depends on
@@ -395,18 +491,15 @@
             functions, and rows indexed by the combinations of subgroups
             in the sensitive and control features.
 
             If a particular combination of subgroups was not present in the dataset
             (likely to occur as more sensitive and control features
             are specified), then the corresponding entry will be NaN.
         """
-        if self._user_supplied_callable:
-            return self._result.by_group.iloc[:, 0]
-        else:
-            return self._result.by_group
+        return self._result_cache["by_group"]
 
     @property
     def control_levels(self) -> Optional[List[str]]:
         """Return a list of feature names which are produced by control features.
 
         If control features are present, then the rows of the :attr:`.by_group`
         property have a :class:`pandas.MultiIndex` index. This property
@@ -433,45 +526,43 @@
         -------
         List[str]
             List of names, which can be used in calls to
             :meth:`pandas.DataFrame.groupby` etc.
         """
         return self._sf_names
 
-    def __group(
-        self, grouping_function: str, errors: str = "raise"
+    def _group(
+        self,
+        disagg_result: DisaggregatedResult,
+        grouping_function: str,
+        errors: str = "raise",
     ) -> Union[Any, pd.Series, pd.DataFrame]:
         """Return the minimum/maximum value of the metric over the sensitive features.
 
         This is a private method, please use .group_min() or .group_max() instead.
 
         Parameters
         ----------
+        disagg_result: The DisaggregatedResult containing all the metrics
         grouping_function: {'min', 'max'}
         errors: {'raise', 'coerce'}, default 'raise'
         if 'raise', then invalid parsing will raise an exception
         if 'coerce', then invalid parsing will be set as NaN
 
         Returns
         -------
         typing.Any pandas.Series or pandas.DataFrame
             The minimum value over sensitive features. The exact type
             follows the table in :attr:`.MetricFrame.overall`.
         """
-        result = self._result.apply_grouping(
+        result = disagg_result.apply_grouping(
             grouping_function, self.control_levels, errors=errors
         )
 
-        if self._user_supplied_callable:
-            if self.control_levels:
-                return result.iloc[:, 0]
-            else:
-                return result.iloc[0]
-        else:
-            return result
+        return self._extract_result(result, no_control_levels=False)
 
     def group_max(self, errors: str = "raise") -> Union[Any, pd.Series, pd.DataFrame]:
         """Return the maximum value of the metric over the sensitive features.
 
         This method computes the maximum value over all combinations of
         sensitive features for each underlying metric function in the :attr:`.by_group`
         property (it will only succeed if all the underlying metric
@@ -489,15 +580,22 @@
 
         Returns
         -------
         typing.Any or pandas.Series or pandas.DataFrame
             The maximum value over sensitive features. The exact type
             follows the table in :attr:`.MetricFrame.overall`.
         """
-        return self.__group("max", errors)
+        if errors not in _VALID_ERROR_STRING:
+            raise ValueError(_INVALID_ERRORS_VALUE_ERROR_MESSAGE)
+
+        value = self._result_cache["group_max"][errors]
+        if isinstance(value, Exception):
+            raise value
+        else:
+            return value
 
     def group_min(self, errors: str = "raise") -> Union[Any, pd.Series, pd.DataFrame]:
         """Return the maximum value of the metric over the sensitive features.
 
         This method computes the minimum value over all combinations of
         sensitive features for each underlying metric function in the :attr:`.by_group`
         property (it will only succeed if all the underlying metric
@@ -515,15 +613,22 @@
 
         Returns
         -------
         typing.Any or pandas.Series or pandas.DataFrame
             The maximum value over sensitive features. The exact type
             follows the table in :attr:`.MetricFrame.overall`.
         """
-        return self.__group("min", errors)
+        if errors not in _VALID_ERROR_STRING:
+            raise ValueError(_INVALID_ERRORS_VALUE_ERROR_MESSAGE)
+
+        value = self._result_cache["group_min"][errors]
+        if isinstance(value, Exception):
+            raise value
+        else:
+            return value
 
     def difference(
         self, method: str = "between_groups", errors: str = "coerce"
     ) -> Union[Any, pd.Series, pd.DataFrame]:
         """Return the maximum absolute difference between groups for each metric.
 
         This method calculates a scalar value for each underlying metric by
@@ -554,28 +659,25 @@
             if 'coerce', then invalid parsing will be set as NaN
 
         Returns
         -------
         typing.Any or pandas.Series or pandas.DataFrame
             The exact type follows the table in :attr:`.MetricFrame.overall`.
         """
-        tmp = self._result.difference(self.control_levels, method=method, errors=errors)
+        if errors not in _VALID_ERROR_STRING:
+            raise ValueError(_INVALID_ERRORS_VALUE_ERROR_MESSAGE)
 
-        if isinstance(tmp, pd.Series):
-            result = tmp.map(lambda x: x if x is not None else np.nan)
-        else:
-            result = tmp.applymap(lambda x: x if x is not None else np.nan)
+        if method not in _COMPARE_METHODS:
+            raise ValueError(_INVALID_COMPARE_METHOD.format(method))
 
-        if self._user_supplied_callable:
-            if self.control_levels:
-                return result.iloc[:, 0]
-            else:
-                return result.iloc[0]
+        value = self._result_cache["difference"][method][errors]
+        if isinstance(value, Exception):
+            raise value
         else:
-            return result
+            return value
 
     def ratio(
         self, method: str = "between_groups", errors: str = "coerce"
     ) -> Union[Any, pd.Series, pd.DataFrame]:
         """Return the minimum ratio between groups for each metric.
 
         This method calculates a scalar value for each underlying metric by
@@ -608,28 +710,25 @@
             if 'coerce', then invalid parsing will be set as NaN
 
         Returns
         -------
         typing.Any or pandas.Series or pandas.DataFrame
             The exact type follows the table in :attr:`.MetricFrame.overall`.
         """
-        tmp = self._result.ratio(self.control_levels, method=method, errors=errors)
+        if errors not in _VALID_ERROR_STRING:
+            raise ValueError(_INVALID_ERRORS_VALUE_ERROR_MESSAGE)
 
-        if isinstance(tmp, pd.Series):
-            result = tmp.map(lambda x: x if x is not None else np.nan)
-        else:
-            result = tmp.applymap(lambda x: x if x is not None else np.nan)
+        if method not in _COMPARE_METHODS:
+            raise ValueError(_INVALID_COMPARE_METHOD.format(method))
 
-        if self._user_supplied_callable:
-            if self.control_levels:
-                return result.iloc[:, 0]
-            else:
-                return result.iloc[0]
-
-        return result
+        value = self._result_cache["ratio"][method][errors]
+        if isinstance(value, Exception):
+            raise value
+        else:
+            return value
 
     def _process_functions(
         self,
         metric: Union[Callable, Dict[str, Callable]],
         sample_params,
         all_data: pd.DataFrame,
     ) -> Dict[str, AnnotatedMetricFunction]:
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/metrics/_plot_model_comparison.py` & `fairlearn-0.9.0/fairlearn/metrics/_plot_model_comparison.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,28 +141,29 @@
         raise ValueError(
             _INCONSISTENT_ARRAY_LENGTH.format("y_true and the rows of y_preds")
         )
 
     if isinstance(axis_labels, (list, tuple)):
         if len(axis_labels) != 2:
             raise ValueError(
-                "Key word argument axis_labels should be a list or tuple of two strings."
+                "Key word argument axis_labels should be a list or tuple of two"
+                " strings."
             )
     elif isinstance(axis_labels, bool):
         pass
     else:
         raise ValueError(
             _INPUT_DATA_FORMAT_ERROR_MESSAGE.format(
                 axis_labels,
                 "boolean or tuple of two strings",
                 type(axis_labels).__name__,
             )
         )
 
-    for (kwarg, name) in (
+    for kwarg, name in (
         (legend, "legend"),
         (show_plot, "show_plot"),
     ):
         if not isinstance(kwarg, bool):
             raise ValueError(
                 _INPUT_DATA_FORMAT_ERROR_MESSAGE.format(
                     name, "boolean", type(kwarg).__name__
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/metrics/_plotter.py` & `fairlearn-0.9.0/fairlearn/metrics/_plotter.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/fairlearn/postprocessing/__init__.py` & `fairlearn-0.9.0/fairlearn/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/fairlearn/postprocessing/_constants.py` & `fairlearn-0.9.0/fairlearn/postprocessing/_constants.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/fairlearn/postprocessing/_interpolated_thresholder.py` & `fairlearn-0.9.0/fairlearn/postprocessing/_interpolated_thresholder.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,18 +97,20 @@
         Otherwise it is fitted from the provided arguments.
         """
         if self.estimator is None:
             raise ValueError(BASE_ESTIMATOR_NONE_ERROR_MESSAGE)
 
         if self.predict_method == "deprecated":
             warn(
-                "'predict_method' default value is changed from 'predict' to "
-                "'auto'. Explicitly pass `predict_method='predict' to "
-                "replicate the old behavior, or pass `predict_method='auto' "
-                "or other valid values to silence this warning.",
+                (
+                    "'predict_method' default value is changed from 'predict' to "
+                    "'auto'. Explicitly pass `predict_method='predict' to "
+                    "replicate the old behavior, or pass `predict_method='auto' "
+                    "or other valid values to silence this warning."
+                ),
                 FutureWarning,
             )
             self._predict_method = "predict"
         else:
             self._predict_method = self.predict_method
 
         if not self.prefit:
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/postprocessing/_plotting.py` & `fairlearn-0.9.0/fairlearn/postprocessing/_plotting.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/fairlearn/postprocessing/_threshold_operation.py` & `fairlearn-0.9.0/fairlearn/postprocessing/_threshold_operation.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/fairlearn/postprocessing/_threshold_optimizer.py` & `fairlearn-0.9.0/fairlearn/postprocessing/_threshold_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,24 +173,31 @@
 
     predict_method : {'auto', 'predict_proba', 'decision_function', 'predict'\
             }, default='auto'
 
         Defines which method of the ``estimator`` is used to get the output
         values.
 
-        - 'auto': use one of ``predict_proba``, ``decision_function``, or
-          ``predict``, in that order.
-        - 'predict_proba': use the second column from the output of
-          `predict_proba`. It is assumed that the second column represents the
-          positive outcome.
-        - 'decision_function': use the raw values given by the
-          `decision_function`.
-        - 'predict': use the hard values reported by the `predict` method if
-          estimator is a classifier, and the regression values if estimator is
-          a regressor. This is equivalent to what is done in [1]_.
+            'auto'
+                use one of :code:`predict_proba`, :code:`decision_function`, or 
+                :code:`predict`, in that order.
+            
+            'predict_proba'
+                use the second column from the output of :code:`predict_proba`. 
+                It is assumed that the second column represents the positive 
+                outcome.
+            
+            'decision_function'
+                use the raw values given by the :code:`decision_function`.
+            
+            'predict'
+                use the hard values reported by the :code:`predict` method if 
+                estimator is a classifier, and the regression values if 
+                estimator is a regressor. This is equivalent to what 
+                is done in [1]_.
 
         .. versionadded:: 0.7
             In previous versions only the ``predict`` method was used
             implicitly.
 
         .. versionchanged:: 0.7
             From version 0.7, 'predict' is deprecated as the default value and
@@ -279,18 +286,20 @@
                     NOT_SUPPORTED_OBJECTIVES_FOR_EQUALIZED_ODDS_ERROR_MESSAGE
                 )
         else:
             raise ValueError(NOT_SUPPORTED_CONSTRAINTS_ERROR_MESSAGE)
 
         if self.predict_method == "deprecated":
             warn(
-                "'predict_method' default value is changed from 'predict' to "
-                "'auto'. Explicitly pass `predict_method='predict' to "
-                "replicate the old behavior, or pass `predict_method='auto' "
-                "or other valid values to silence this warning.",
+                (
+                    "'predict_method' default value is changed from 'predict' to "
+                    "'auto'. Explicitly pass `predict_method='predict' to "
+                    "replicate the old behavior, or pass `predict_method='auto' "
+                    "or other valid values to silence this warning."
+                ),
                 FutureWarning,
             )
             self._predict_method = "predict"
         else:
             self._predict_method = self.predict_method
 
         if kwargs.get(_KW_CONTROL_FEATURES) is not None:
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/postprocessing/_tradeoff_curve_utilities.py` & `fairlearn-0.9.0/fairlearn/postprocessing/_tradeoff_curve_utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 DEGENERATE_LABELS_ERROR_MESSAGE = "Degenerate labels for sensitive feature value {}"
 
 # Dictionary of metrics based on confusion matrix. Their input must be a Bunch with the fields
 # named n, positives, negatives, predicted_positives, predicted_negatives, true_positives,
 # true_negatives, false_positives, false_negatives. The fields indicate the counts. They can all
 # be numpy arrays of the same length. Metrics are expected to return NaN where undefined.
 METRIC_DICT = {
-    "selection_rate": (lambda x: x.predicted_positives / x.n),
-    "false_positive_rate": (lambda x: x.false_positives / x.negatives),
-    "false_negative_rate": (lambda x: x.false_negatives / x.positives),
-    "true_positive_rate": (lambda x: x.true_positives / x.positives),
-    "true_negative_rate": (lambda x: x.true_negatives / x.negatives),
-    "accuracy_score": (lambda x: (x.true_positives + x.true_negatives) / x.n),
+    "selection_rate": lambda x: x.predicted_positives / x.n,
+    "false_positive_rate": lambda x: x.false_positives / x.negatives,
+    "false_negative_rate": lambda x: x.false_negatives / x.positives,
+    "true_positive_rate": lambda x: x.true_positives / x.positives,
+    "true_negative_rate": lambda x: x.true_negatives / x.negatives,
+    "accuracy_score": lambda x: (x.true_positives + x.true_negatives) / x.n,
     "balanced_accuracy_score": (
         lambda x: 0.5 * x.true_positives / x.positives
         + 0.5 * x.true_negatives / x.negatives
     ),
 }
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/preprocessing/_correlation_remover.py` & `fairlearn-0.9.0/fairlearn/preprocessing/_correlation_remover.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,19 @@
         return X
 
     def fit(self, X, y=None):
         """Learn the projection required to make the dataset uncorrelated with sensitive columns."""  # noqa: E501
         self._create_lookup(X)
         X = self._validate_data(X)
         X_use, X_sensitive = self._split_X(X)
-        self.sensitive_mean_ = X_sensitive.mean()
+        # correctly handle zero provided sensitive features
+        if X_sensitive.shape[1] == 0:
+            self.sensitive_mean_ = np.array([])
+        else:
+            self.sensitive_mean_ = X_sensitive.mean()
         X_s_center = X_sensitive - self.sensitive_mean_
         self.beta_, _, _, _ = np.linalg.lstsq(X_s_center, X_use, rcond=None)
         self.X_shape_ = X.shape
         return self
 
     def transform(self, X):
         """Transform X by applying the correlation remover."""
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/reductions/__init__.py` & `fairlearn-0.9.0/fairlearn/reductions/__init__.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/fairlearn/reductions/_exponentiated_gradient/_constants.py` & `fairlearn-0.9.0/fairlearn/reductions/_exponentiated_gradient/_constants.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/fairlearn/reductions/_exponentiated_gradient/_lagrangian.py` & `fairlearn-0.9.0/fairlearn/reductions/_exponentiated_gradient/_lagrangian.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,22 @@
 
 _MESSAGE_BAD_OBJECTIVE = (
     "Objective needs to be of the same type as constraints. "
     "Objective is {}, constraints are {}."
 )
 
 
+class _PredictorAsCallable:
+    def __init__(self, classifier):
+        self._classifier = classifier
+
+    def __call__(self, X):
+        return self._classifier.predict(X)
+
+
 class _Lagrangian:
     """Operations related to the Lagrangian.
 
     Parameters
     ----------
     X : {numpy.ndarray, pandas.DataFrame}
         the training features
@@ -229,21 +237,15 @@
         """Solve the best-response problem.
 
         Returns the classifier that solves the best-response problem for
         the vector of Lagrange multipliers `lambda_vec`.
         """
         classifier = self._call_oracle(lambda_vec)
 
-        def h(X):
-            pred = classifier.predict(X)
-            # Some estimators return an output of the shape (num_preds, 1) - flatten such
-            # results
-            if getattr(pred, "flatten", None) is not None:
-                pred = pred.flatten()
-            return pred
+        h = _PredictorAsCallable(classifier)
 
         h_error = self.obj.gamma(h)[0]
         h_gamma = self.constraints.gamma(h)
         h_value = h_error + h_gamma.dot(lambda_vec)
 
         if not self.hs.empty:
             values = self.errors + self.gammas.transpose().dot(lambda_vec)
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/reductions/_exponentiated_gradient/exponentiated_gradient.py` & `fairlearn-0.9.0/fairlearn/reductions/_exponentiated_gradient/exponentiated_gradient.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,16 +207,18 @@
                 Qs.append(Q_EG)
                 gaps.append(gap_EG)
             else:
                 Qs.append(Q_LP)
                 gaps.append(gap_LP)
 
             logger.debug(
-                "%seta=%.6f, L_low=%.3f, L=%.3f, L_high=%.3f, gap=%.6f, disp=%.3f, "
-                "err=%.3f, gap_LP=%.6f",
+                (
+                    "%seta=%.6f, L_low=%.3f, L=%.3f, L_high=%.3f, gap=%.6f, disp=%.3f, "
+                    "err=%.3f, gap_LP=%.6f"
+                ),
                 _INDENTATION,
                 eta,
                 result_EG.L_low,
                 result_EG.L,
                 result_EG.L_high,
                 gap_EG,
                 result_EG.gamma.max(),
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/reductions/_grid_search/_grid_generator.py` & `fairlearn-0.9.0/fairlearn/reductions/_grid_search/_grid_generator.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/fairlearn/reductions/_grid_search/grid_search.py` & `fairlearn-0.9.0/fairlearn/reductions/_grid_search/grid_search.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/fairlearn/reductions/_moments/__init__.py` & `fairlearn-0.9.0/fairlearn/reductions/_moments/__init__.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/fairlearn/reductions/_moments/bounded_group_loss.py` & `fairlearn-0.9.0/fairlearn/reductions/_moments/bounded_group_loss.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/fairlearn/reductions/_moments/error_rate.py` & `fairlearn-0.9.0/fairlearn/reductions/_moments/error_rate.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,14 @@
     .. math::
       c_{FP} P[h(X)=1, Y=0] + c_{FN} P[h(X)=0, Y=1]
 
     where :math:`c_{FP}` and :math:`c_{FN}` are the costs of false positive
     and false negative errors respectively. The standard misclassification
     error corresponds to :math:`c_{FP}=c_{FN}=1.0`.
 
-    Read more in the :ref:`User Guide <error_rate_parity>`.
-
     Parameters
     ----------
     costs : dict
         The dictionary with keys :code:`'fp'` and :code:`'fn'` containing the
         costs of false positives and false negatives. If none are provided
         costs of 1.0 are assumed.
     """
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/reductions/_moments/moment.py` & `fairlearn-0.9.0/fairlearn/reductions/_moments/moment.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/fairlearn/reductions/_moments/utility_parity.py` & `fairlearn-0.9.0/fairlearn/reductions/_moments/utility_parity.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 from .error_rate import ErrorRate
 from .moment import (
     _ALL,
     _EVENT,
     _GROUP_ID,
     _LABEL,
-    _PREDICTION,
     _SIGN,
     ClassificationMoment,
 )
 
 _UPPER_BOUND_DIFF = "upper_bound_diff"
 _LOWER_BOUND_DIFF = "lower_bound_diff"
 _MESSAGE_INVALID_BOUNDS = "Only one of difference_bound and ratio_bound can be used."
@@ -149,76 +148,87 @@
             utilities = np.vstack(
                 [
                     np.zeros(y.shape, dtype=np.float64),
                     np.ones(y.shape, dtype=np.float64),
                 ]
             ).T
         self.utilities = utilities
+        self.utility_diff = self.utilities[:, 1] - self.utilities[:, 0]
         self.prob_event = self.tags.groupby(_EVENT).size() / self.total_samples
         self.prob_group_event = (
             self.tags.groupby([_EVENT, _GROUP_ID]).size() / self.total_samples
         )
         signed = pd.concat(
             [self.prob_group_event, self.prob_group_event],
             keys=["+", "-"],
             names=[_SIGN, _EVENT, _GROUP_ID],
         )
         self.index = signed.index
         self.default_objective_lambda_vec = None
 
+        # Fill information about the matrix U, which is used to calculate signed weights
+        # and gamma vector. The matrix has a row corresponding to each example and column
+        # corresponding to each component of lambda, the signed weights and gamma are
+        # calculated as:
+        #
+        # signed_weights = utility_diff * U.dot(lambda_vec)
+        # gamma = -U.T.dot(utilities[y_pred]) / total_samples
+        #
+        # If the i-th example's event and group are "e" and "g" then the entries in the
+        # i-th row of the matrix, indexed by tuples (sign, event, group), are defined as:
+        #
+        # U_i,(+,e',g') =      1[e=e']/P(e) - rho*1[e=e',g=g']/P(g,e)
+        # U_i,(-,e',g') = -rho*1[e=e']/P(e) +     1[e=e',g=g']/P(g,e)
+        #
+        # This corresponds to the expression given right above Theorem 1 of the paper
+        # "A Reductions Approach to Fair Classification" by Agarwal et al. (2018).
+
+        self.U = pd.DataFrame(0, index=self.tags.index, columns=self.index)
+        for e, g in self.prob_group_event.index:
+            event_select = 1 * (self.tags[_EVENT] == e)
+            group_event_select = event_select * (self.tags[_GROUP_ID] == g)
+            self.U["+", e, g] = (
+                event_select / self.prob_event[e]
+                + (-self.ratio) * group_event_select / self.prob_group_event[e, g]
+            )
+            self.U["-", e, g] = (-self.ratio) * event_select / self.prob_event[
+                e
+            ] + group_event_select / self.prob_group_event[e, g]
+
         # fill in the information about the basis
         event_vals = self.tags[_EVENT].dropna().unique()
         group_vals = self.tags[_GROUP_ID].unique()
         # The matrices pos_basis and neg_basis contain a lower-dimensional description of
         # constraints, which is achieved by removing some redundant constraints.
         # Considering fewer constraints is not required for correctness, but it can dramatically
         # speed up GridSearch.
         self.pos_basis = pd.DataFrame()
         self.neg_basis = pd.DataFrame()
         self.neg_basis_present = pd.Series(dtype="float64")
         zero_vec = pd.Series(0.0, self.index)
         i = 0
-        for event_val in event_vals:
+        for e in event_vals:
             # Constraints on the final group are redundant, so they are not included in the basis.
-            for group in group_vals[:-1]:
+            for g in group_vals[:-1]:
                 self.pos_basis[i] = 0 + zero_vec
                 self.neg_basis[i] = 0 + zero_vec
-                self.pos_basis[i]["+", event_val, group] = 1
-                self.neg_basis[i]["-", event_val, group] = 1
+                self.pos_basis[i]["+", e, g] = 1
+                self.neg_basis[i]["-", e, g] = 1
                 self.neg_basis_present.at[i] = True
                 i += 1
 
     def gamma(self, predictor):
         """Calculate the degree to which constraints are currently violated by the predictor."""
-        utility_diff = self.utilities[:, 1] - self.utilities[:, 0]
         predictions = predictor(self.X)
         if isinstance(predictions, np.ndarray):
             # TensorFlow seems to return an (n,1) array instead of an (n) array
             predictions = np.squeeze(predictions)
-        pred = utility_diff.T * predictions + self.utilities[:, 0]
-        self.tags[_PREDICTION] = pred
-        expect_event = self.tags.groupby(_EVENT).mean(numeric_only=True)
-        expect_group_event = self.tags.groupby([_EVENT, _GROUP_ID]).mean()
-        expect_group_event[_UPPER_BOUND_DIFF] = (
-            self.ratio * expect_group_event[_PREDICTION] - expect_event[_PREDICTION]
-        )
-        expect_group_event[_LOWER_BOUND_DIFF] = (
-            -expect_group_event[_PREDICTION] + self.ratio * expect_event[_PREDICTION]
-        )
-        g_signed = pd.concat(
-            [
-                expect_group_event[_UPPER_BOUND_DIFF],
-                expect_group_event[_LOWER_BOUND_DIFF],
-            ],
-            keys=["+", "-"],
-            names=[_SIGN, _EVENT, _GROUP_ID],
-        )
-        self._gamma_descr = str(
-            expect_group_event[[_PREDICTION, _UPPER_BOUND_DIFF, _LOWER_BOUND_DIFF]]
-        )
+        pred = self.utility_diff.T * predictions + self.utilities[:, 0]
+        g_signed = -self.U.T.dot(pred) / self.total_samples
+        self._gamma_descr = str(g_signed)
         return g_signed
 
     def bound(self):
         """Return bound vector.
 
         Returns
         -------
@@ -259,30 +269,15 @@
 
         Parameters
         ----------
         lambda_vec : :class:`pandas:pandas.Series`
             The vector of Lagrange multipliers indexed by `index`
 
         """
-        lambda_event = (lambda_vec["+"] - self.ratio * lambda_vec["-"]).groupby(
-            level=_EVENT
-        ).sum() / self.prob_event
-        lambda_group_event = (
-            self.ratio * lambda_vec["+"] - lambda_vec["-"]
-        ) / self.prob_group_event
-        adjust = lambda_event - lambda_group_event
-        signed_weights = self.tags.apply(
-            lambda row: 0
-            if pd.isna(row[_EVENT])
-            else adjust[row[_EVENT], row[_GROUP_ID]],
-            axis=1,
-        )
-        utility_diff = self.utilities[:, 1] - self.utilities[:, 0]
-        signed_weights = utility_diff.T * signed_weights
-        return signed_weights
+        return self.utility_diff * self.U.dot(lambda_vec)
 
 
 # Ensure that UtilityParity shows up in correct place in documentation
 # when it is used as a base class
 UtilityParity.__module__ = "fairlearn.reductions"
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/show_versions.py` & `fairlearn-0.9.0/fairlearn/show_versions.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 # Licensed under the MIT License.
 
 """Utility methods to print system info for debugging.
 
 Adapted from :py:func:`pandas.show_versions` and :py:func:`sklearn.show_versions`.
 """  # noqa: RST304
 
-import importlib
 import platform
 import sys
 
 
 def _get_sys_info():
     """System information.
 
-    :returns: system and Python version information
-    :rtype: dict
+    Returns
+    -------
+    sys_info : dict
+        system and Python version information
     """
     python = sys.version.replace("\n", " ")
 
     blob = [
         ("python", python),
         ("executable", sys.executable),
         ("machine", platform.platform()),
@@ -27,55 +28,57 @@
 
     return dict(blob)
 
 
 def _get_deps_info():
     """Overview of the installed version of main dependencies.
 
-    :return: version information on relevant Python libraries
-    :rtype: dict
+    This function does not import the modules to collect the version numbers
+    but instead relies on standard Python package metadata.
+
+    Returns
+    -------
+    deps_info: dict
+        version information on relevant Python libraries
     """
     deps = sorted(
         [
             "pip",
             "setuptools",
-            "sklearn",
             "numpy",
             "scipy",
             "Cython",
             "pandas",
             "matplotlib",
-            "tempeh",
+            "sklearn",
+            "lightgbm",
+            "pytorch",
+            "tensorflow",
         ]
     )
 
-    def get_version(module):
-        return module.__version__
+    from fairlearn import __version__
 
-    deps_info = {}
+    deps_info = {"fairlearn": __version__}
+
+    from importlib.metadata import PackageNotFoundError, version
 
     for modname in deps:
         try:
-            if modname in sys.modules:
-                mod = sys.modules[modname]
-            else:
-                mod = importlib.import_module(modname)
-            ver = get_version(mod)
-            deps_info[modname] = ver
-        except ImportError:
+            deps_info[modname] = version(modname)
+        except PackageNotFoundError:
             deps_info[modname] = None
-
     return deps_info
 
 
 def show_versions():
     """Print useful debugging information."""
     sys_info = _get_sys_info()
     deps_info = _get_deps_info()
 
     print("\nSystem:")
     for k, stat in sys_info.items():
         print("{k:>10}: {stat}".format(k=k, stat=stat))
 
     print("\nPython dependencies:")
     for k, stat in deps_info.items():
-        print("{k:>10}: {stat}".format(k=k, stat=stat))
+        print("{k:>13}: {stat}".format(k=k, stat=stat))
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn/utils/_common.py` & `fairlearn-0.9.0/fairlearn/utils/_common.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/fairlearn/utils/_input_validation.py` & `fairlearn-0.9.0/fairlearn/utils/_input_validation.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/fairlearn.egg-info/PKG-INFO` & `fairlearn-0.9.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,8 @@
-Metadata-Version: 2.1
-Name: fairlearn
-Version: 0.8.0.dev0
-Summary: Algorithms for mitigating unfairness in supervised machine learning
-Home-page: https://github.com/fairlearn/fairlearn
-Author: Miroslav Dudik, Richard Edgar, Brandon Horn, Roman Lutz
-Author-email: fairlearn@microsoft.com
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: customplots
-License-File: LICENSE
-License-File: AUTHORS.md
-
-|Build Status| |MIT license| |PyPI| |Discord| |StackOverflow|
+|MIT license| |PyPI| |Discord| |StackOverflow|
 
 Fairlearn
 =========
 
 Fairlearn is a Python package that empowers developers of artificial
 intelligence (AI) systems to assess their system's fairness and mitigate
 any observed unfairness issues. Fairlearn contains mitigation algorithms
@@ -107,26 +88,26 @@
 Check out our in-depth `guide on the Fairlearn
 metrics <https://fairlearn.org/main/user_guide/assessment>`__.
 
 Fairlearn algorithms
 ~~~~~~~~~~~~~~~~~~~~
 
 For an overview of our algorithms please refer to our
-`website <https://fairlearn.org/main/user_guide/mitigation.html>`__.
+`website <https://fairlearn.org/main/user_guide/mitigation/index.html>`__.
 
 Install Fairlearn
 -----------------
 
 For instructions on how to install Fairlearn check out our `Quickstart
 guide <https://fairlearn.org/main/quickstart.html>`__.
 
 Usage
 -----
 
-For common usage refer to the `Jupyter notebooks <./notebooks>`__ and
+For common usage refer to the `Jupyter notebooks <https://fairlearn.org/main/auto_examples/index.html>`__ and
 our `user guide <https://fairlearn.org/main/user_guide/index.html>`__.
 Please note that our APIs are subject to change, so notebooks downloaded
 from ``main`` may not be compatible with Fairlearn installed with
 ``pip``. In this case, please navigate the tags in the repository (e.g.
 `v0.7.0 <https://github.com/fairlearn/fairlearn/tree/v0.7.0>`__) to
 locate the appropriate version of the notebook.
 
@@ -165,16 +146,14 @@
 
 Reporting security issues
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 To report security issues please send an email to
 ``fairlearn-internal@python.org``.
 
-.. |Build Status| image:: https://dev.azure.com/responsibleai/fairlearn/_apis/build/status/Nightly?branchName=main
-   :target: https://dev.azure.com/responsibleai/fairlearn/_build/latest?definitionId=23&branchName=main
 .. |MIT license| image:: https://img.shields.io/badge/License-MIT-blue.svg
    :target: https://github.com/fairlearn/fairlearn/blob/main/LICENSE
 .. |PyPI| image:: https://img.shields.io/pypi/v/fairlearn?color=blue
    :target: https://pypi.org/project/fairlearn/
 .. |Discord| image:: https://img.shields.io/discord/840099830160031744
    :target: https://discord.gg/R22yCfgsRn
 .. |StackOverflow| image:: https://img.shields.io/badge/StackOverflow-questions-blueviolet
```

### Comparing `fairlearn-0.8.0.dev0/fairlearn.egg-info/SOURCES.txt` & `fairlearn-0.9.0/fairlearn.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,33 +22,29 @@
 fairlearn/adversarial/_tensorflow_engine.py
 fairlearn/datasets/__init__.py
 fairlearn/datasets/_constants.py
 fairlearn/datasets/_fetch_acs_income.py
 fairlearn/datasets/_fetch_adult.py
 fairlearn/datasets/_fetch_bank_marketing.py
 fairlearn/datasets/_fetch_boston.py
+fairlearn/datasets/_fetch_credit_card.py
 fairlearn/datasets/_fetch_diabetes_hospital.py
 fairlearn/experimental/__init__.py
 fairlearn/experimental/enable_metric_frame_plotting.py
 fairlearn/metrics/__init__.py
 fairlearn/metrics/_annotated_metric_function.py
-fairlearn/metrics/_balanced_root_mean_squared_error.py
+fairlearn/metrics/_base_metrics.py
 fairlearn/metrics/_disaggregated_result.py
-fairlearn/metrics/_disparities.py
-fairlearn/metrics/_extra_metrics.py
+fairlearn/metrics/_fairness_metrics.py
 fairlearn/metrics/_generated_metrics.py
 fairlearn/metrics/_group_feature.py
-fairlearn/metrics/_group_metric_set.py
-fairlearn/metrics/_input_manipulations.py
 fairlearn/metrics/_make_derived_metric.py
-fairlearn/metrics/_mean_predictions.py
 fairlearn/metrics/_metric_frame.py
 fairlearn/metrics/_plot_model_comparison.py
 fairlearn/metrics/_plotter.py
-fairlearn/metrics/_selection_rate.py
 fairlearn/postprocessing/__init__.py
 fairlearn/postprocessing/_constants.py
 fairlearn/postprocessing/_interpolated_thresholder.py
 fairlearn/postprocessing/_plotting.py
 fairlearn/postprocessing/_threshold_operation.py
 fairlearn/postprocessing/_threshold_optimizer.py
 fairlearn/postprocessing/_tradeoff_curve_utilities.py
@@ -65,18 +61,21 @@
 fairlearn/reductions/_moments/__init__.py
 fairlearn/reductions/_moments/bounded_group_loss.py
 fairlearn/reductions/_moments/error_rate.py
 fairlearn/reductions/_moments/moment.py
 fairlearn/reductions/_moments/utility_parity.py
 fairlearn/utils/__init__.py
 fairlearn/utils/_common.py
+fairlearn/utils/_compatibility.py
+fairlearn/utils/_input_manipulations.py
 fairlearn/utils/_input_validation.py
 test/__init__.py
-test/notebooks/__init__.py
-test/notebooks/test_notebooks.py
+test/install/__init__.py
+test/install/test_no_matplotlib.py
+test/install/test_no_ml.py
 test/unit/__init__.py
 test/unit/conftest.py
 test/unit/constants.py
 test/unit/fixes.py
 test/unit/input_convertors.py
 test/unit/test_random_state.py
 test/unit/test_show_versions.py
@@ -85,24 +84,20 @@
 test/unit/adversarial/helper.py
 test/unit/adversarial/test_adversarial_mitigation.py
 test/unit/adversarial/test_preprocessing.py
 test/unit/datasets/__init__.py
 test/unit/datasets/test_datasets.py
 test/unit/metrics/__init__.py
 test/unit/metrics/data_for_test.py
-test/unit/metrics/sample_loader.py
 test/unit/metrics/test_annotated_metric_function.py
-test/unit/metrics/test_balanced_root_mean_squared_error.py
-test/unit/metrics/test_create_group_metric_set.py
+test/unit/metrics/test_base_metrics.py
 test/unit/metrics/test_disaggregated_result.py
-test/unit/metrics/test_disparities.py
-test/unit/metrics/test_extra_metrics.py
+test/unit/metrics/test_fairness_metrics.py
 test/unit/metrics/test_generated_metrics.py
 test/unit/metrics/test_group_feature.py
-test/unit/metrics/test_input_manipulations.py
 test/unit/metrics/test_make_derived_metric.py
 test/unit/metrics/test_mean_predictions.py
 test/unit/metrics/test_metricframe_aggregates.py
 test/unit/metrics/test_metricframe_by_group.py
 test/unit/metrics/test_metricframe_comprehensive.py
 test/unit/metrics/test_metricframe_deprecate.py
 test/unit/metrics/test_metricframe_missing.py
@@ -132,20 +127,22 @@
 test/unit/reductions/test_smoke.py
 test/unit/reductions/exponentiated_gradient/__init__.py
 test/unit/reductions/exponentiated_gradient/simple_learners.py
 test/unit/reductions/exponentiated_gradient/test_control_features.py
 test/unit/reductions/exponentiated_gradient/test_exponentiatedgradient_arguments.py
 test/unit/reductions/exponentiated_gradient/test_exponentiatedgradient_smoke.py
 test/unit/reductions/exponentiated_gradient/test_lagrangian.py
+test/unit/reductions/exponentiated_gradient/test_pickle.py
 test/unit/reductions/exponentiated_gradient/test_utilities.py
 test/unit/reductions/grid_search/__init__.py
 test/unit/reductions/grid_search/test_grid_generator.py
 test/unit/reductions/grid_search/test_grid_search_arguments.py
 test/unit/reductions/grid_search/test_grid_search_demographicparity.py
 test/unit/reductions/grid_search/test_grid_search_regression.py
+test/unit/reductions/grid_search/test_pickle.py
 test/unit/reductions/grid_search/utilities.py
 test/unit/reductions/moments/__init__.py
 test/unit/reductions/moments/data_generator.py
 test/unit/reductions/moments/test_moments_bounded_group_loss.py
 test/unit/reductions/moments/test_moments_control_features.py
 test/unit/reductions/moments/test_moments_demographic_parity.py
 test/unit/reductions/moments/test_moments_equalized_odds.py
```

### Comparing `fairlearn-0.8.0.dev0/setup.cfg` & `fairlearn-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/setup.py` & `fairlearn-0.9.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,35 +9,31 @@
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 # Use requirements.txt to set the install_requires
 with open("requirements.txt") as f:
     install_requires = [line.strip() for line in f]
 
-# Fetch separate requirements file for each extension
-extras = ["customplots"]
-extras_require = dict()
-for e in extras:
-    req_file = "requirements-{0}.txt".format(e)
-    with open(req_file) as f:
-        extras_require[e] = [line.strip() for line in f]
-
 setuptools.setup(
     name=fairlearn.__name__,
     version=fairlearn.__version__,
-    author="Miroslav Dudik, Richard Edgar, Brandon Horn, Roman Lutz",
-    author_email="fairlearn@microsoft.com",
-    description="Algorithms for mitigating unfairness in supervised machine learning",
+    author=(
+        "Miroslav Dudik, Richard Edgar, Adrin Jalali, Roman Lutz, Michael Madaio, Hilde"
+        " Weerts"
+    ),
+    author_email="fairlearn-internal@python.org",
+    description=(
+        "A Python package to assess and improve fairness of machine learning models."
+    ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fairlearn/fairlearn",
     packages=setuptools.find_packages(),
     python_requires=">=3.8",
     install_requires=install_requires,
-    extras_require=extras_require,
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Development Status :: 3 - Alpha",
```

### Comparing `fairlearn-0.8.0.dev0/test/unit/adversarial/helper.py` & `fairlearn-0.9.0/test/unit/adversarial/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,28 +83,27 @@
             def __call__(self, X):
                 return self.forward(X)
 
             def apply(self, weights):
                 self.w = weights
 
         BCELoss = type("BCELoss", (BCE,), {})
-        NLLLoss = type("NLLLoss", (CCE,), {})
+        CrossEntropyLoss = type("CrossEntropyLoss", (CCE,), {})
         MSELoss = type("MSELoss", (MSE,), {})
 
         class Linear:  # noqa: D106
             def __init__(self, a, b):
                 self.a = a
                 self.b = b
 
-        ReLU = lambda: type("ReLU", (), {"__call__": lambda x: np.max(x, 0)})  # noqa: E731
+        def ReLU():
+            return type("ReLU", (), {"__call__": lambda x: np.max(x, 0)})  # noqa: E731
 
         def LeakyReLU():
-            return type(
-                "LeakyReLU", (), {"__call__": lambda x: np.max(x, 0.1 * x)}
-            )
+            return type("LeakyReLU", (), {"__call__": lambda x: np.max(x, 0.1 * x)})
 
         Sigmoid = lambda: type("Sigmoid", (), {"__call__": lambda x: x})  # noqa: E731
         Softmax = lambda: type("Softmax", (), {"__call__": lambda x: x})  # noqa: E731
 
         class ModuleList:  # noqa: D106
             def __init__(self, layers):
                 self.layers = layers
@@ -214,15 +213,15 @@
     dist_type = [
         Keyword_BINARY,
         Keyword_CATEGORY,
         Keyword_CONTINUOUS,
         Keyword_CONTINUOUS,
     ]
     K = len(datas)
-    total_combinations = K ** 3
+    total_combinations = K**3
     combinations = np.random.choice(total_combinations, size=n).tolist()
     for c in combinations:
         c_orig = c
         X = c % K
         c = (c - X) // K
         Y = c % K
         c = (c - Y) // K
@@ -246,15 +245,15 @@
 
     def evaluate(self, X):
         """Deterministic evaluation function."""
         cols = self.base._y_transform.n_features_out_
         rows = len(X)
         y = []
         for row in range(rows):
-            rng = np.random.default_rng(int(np.round(np.mean(X[row]) * (2 ** 32))))
+            rng = np.random.default_rng(int(np.round(np.mean(X[row]) * (2**32))))
             y.append(rng.random(cols))
         return np.stack(y)
 
     def train_step(self, X, Y, Z):  # noqa: D102
         return (0, 0)
 
     def get_optimizer(self, optimizer, model):  # noqa: D102
```

### Comparing `fairlearn-0.8.0.dev0/test/unit/adversarial/test_adversarial_mitigation.py` & `fairlearn-0.9.0/test/unit/adversarial/test_adversarial_mitigation.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,15 +338,15 @@
     assert isinstance(mitigator.backendEngine_.predictor_loss, MSE)
     assert isinstance(mitigator.backendEngine_.adversary_loss, CCE)
 
 
 @pytest.mark.parametrize("torch3", [True, False])
 def test_fake_models(torch3):
     """Test various data types and see if it is interpreted correctly."""
-    for ((X, Y, Z), (X_type, Y_type, Z_type)) in generate_data_combinations():
+    for (X, Y, Z), (X_type, Y_type, Z_type) in generate_data_combinations():
         mitigator = get_instance(
             fake_training=True, torch=torch3, tensorflow=not torch3
         )
 
         mitigator.fit(X, Y, sensitive_features=Z)
         assert isinstance(
             mitigator.backendEngine_.predictor_loss, KeywordToClass(Y_type)
@@ -354,22 +354,22 @@
         assert isinstance(
             mitigator.backendEngine_.adversary_loss, KeywordToClass(Z_type)
         )
 
 
 def test_fake_models_list_inputs():
     """Test model with lists as input."""
-    for ((X, Y, Z), types) in generate_data_combinations():
+    for (X, Y, Z), types in generate_data_combinations():
         mitigator = get_instance(fake_mixin=True)
         mitigator.fit(X.tolist(), Y.tolist(), sensitive_features=Z.tolist())
 
 
 def test_fake_models_df_inputs():
     """Test model with data frames as input."""
-    for ((X, Y, Z), types) in generate_data_combinations():
+    for (X, Y, Z), types in generate_data_combinations():
         mitigator = get_instance(fake_mixin=True)
         mitigator.fit(
             pd.DataFrame(X), pd.DataFrame(Y), sensitive_features=pd.DataFrame(Z)
         )
 
 
 def check_type_helper(data, actual_type, valid_choices, invalid_choices):
@@ -477,17 +477,17 @@
     check_type_helper(
         notCat,
         Keyword_CONTINUOUS,
         [Keyword_AUTO, Keyword_CONTINUOUS],  # Auto does work here
         [Keyword_BINARY, Keyword_CATEGORY, Keyword_CLASSIFICATION],
     )
     notCat[0, 1] = 0.5
-    notCat[
-        0, 2:
-    ] = 0.0  # Special case because now first row sums to one but is not one-hot
+    notCat[0, 2:] = (
+        0.0  # Special case because now first row sums to one but is not one-hot
+    )
     check_type_helper(
         notCat,
         Keyword_CONTINUOUS,
         [Keyword_AUTO, Keyword_CONTINUOUS],  # Auto does work here
         [Keyword_BINARY, Keyword_CATEGORY, Keyword_CLASSIFICATION],
     )
 
@@ -498,33 +498,33 @@
     assert X.ndim == 2
     assert len(X.shape) == 2
     assert X.dtype == float
 
 
 def test_validate_data():
     """Test if validate_data properly preprocesses datasets to ndarray."""
-    for ((X, Y, Z), types) in generate_data_combinations():
+    for (X, Y, Z), types in generate_data_combinations():
         mitigator = get_instance(fake_mixin=True)
         X, Y, Z = mitigator._validate_input(X, Y, Z)
         for x in (X, Y, Z):
             check_2dnp(x)
 
 
 def test_validate_data_list_inputs():
     """Test if validate_data properly preprocesses list datasets to ndarray."""
-    for ((X, Y, Z), types) in generate_data_combinations():
+    for (X, Y, Z), types in generate_data_combinations():
         mitigator = get_instance(fake_mixin=True)
         X, Y, Z = mitigator._validate_input(X.tolist(), Y.tolist(), Z.tolist())
         for x in (X, Y, Z):
             check_2dnp(x)
 
 
 def test_validate_data_df_inputs():
     """Test if validate_data properly preprocesses dataframes to ndarray."""
-    for ((X, Y, Z), types) in generate_data_combinations():
+    for (X, Y, Z), types in generate_data_combinations():
         mitigator = get_instance(fake_mixin=True)
         X, Y, Z = mitigator._validate_input(
             pd.DataFrame(X), pd.DataFrame(Y), pd.DataFrame(Z)
         )
         for x in (X, Y, Z):
             check_2dnp(x)
 
@@ -547,15 +547,15 @@
     mitigator = get_instance(torch=False, tensorflow=False, backend=backend)
     with pytest.raises(RuntimeError):
         mitigator._validate_backend()
 
 
 def test_validate_data_ambiguous_rows():
     """Test if an ambiguous number of rows are caught."""
-    for ((X, Y, Z), types) in generate_data_combinations():
+    for (X, Y, Z), types in generate_data_combinations():
         X = X[:5, :]
         mitigator = get_instance(fake_mixin=True)
         with pytest.raises(ValueError) as exc:
             mitigator._validate_input(X.tolist(), Y.tolist(), Z.tolist())
             assert str(
                 exc.value
             ) == "Input data has an ambiguous number of rows: {}, {}, {}.".format(
```

### Comparing `fairlearn-0.8.0.dev0/test/unit/adversarial/test_preprocessing.py` & `fairlearn-0.9.0/test/unit/adversarial/test_preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Fairlearn contributors.
 # Licensed under the MIT License.
 
 from fairlearn.adversarial._preprocessor import FloatTransformer
 import pytest
 from pandas import DataFrame, Series
 from numpy import ndarray, asarray, issubdtype
-from sklearn.datasets import fetch_openml
+from fairlearn.datasets import fetch_adult
 
 
 def data_generator():
     """
     Generate datasets with appropriate labellings.
 
     Some data can not be represented by some data types, so then you
@@ -35,15 +35,15 @@
     yield [[0, 0, 1], [0, 1, 0], [0, 0, 1], [1, 0, 0]], "category", [Series]
     yield [1, 2, 6, 2, 1.1], "continuous"
     yield [0.1, 2.0, 0.999999, 100000.1], "continuous"
     yield [[5.5, 12.2], [86.2, 81.1]], "continuous", [Series]
     yield [[0, 1], [1, 0], [0.1, 2]], "continuous", [Series]
 
     # Larger examples.
-    X, y = fetch_openml(data_id=1590, as_frame=True, return_X_y=True)
+    X, y = fetch_adult(return_X_y=True)
     yield y.tolist(), "binary"
     non_NaN_rows = ~X.isna().any(axis=1)
     X = X[non_NaN_rows]
     yield X["native-country"].tolist(), "category"
     yield X["sex"].tolist(), "binary"
     # yield X['capital-loss'], 'continuous' # FIXME: what should this be?
```

### Comparing `fairlearn-0.8.0.dev0/test/unit/conftest.py` & `fairlearn-0.9.0/test/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/datasets/test_datasets.py` & `fairlearn-0.9.0/test/unit/datasets/test_datasets.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,43 +3,40 @@
 
 import pandas as pd
 import numpy as np
 import pytest
 
 from fairlearn.datasets import (
     fetch_adult,
-    fetch_boston,
     fetch_bank_marketing,
+    fetch_boston,
+    fetch_credit_card,
     fetch_diabetes_hospital,
 )
 
 # =============================================
 
 
 class TestFairlearnDataset:
     @pytest.mark.parametrize("as_frame", [True, False])
     @pytest.mark.parametrize(
         "fetch_function",
         [
             fetch_adult,
-            fetch_boston,
             fetch_bank_marketing,
+            fetch_boston,
+            fetch_credit_card,
             fetch_diabetes_hospital,
         ],
     )
     def test_dataset_as_bunch(self, as_frame, fetch_function):
-        if fetch_function == fetch_diabetes_hospital:
-            if as_frame is True:
-                dataset = fetch_function()
-            elif as_frame is False:
-                pytest.skip(
-                    "Skipping the diabetes hospital dataset with as_frame False"
-                )
-        else:
-            dataset = fetch_function(as_frame=as_frame)
+        if as_frame is False and fetch_function is fetch_diabetes_hospital:
+            msg = "fetch_diabetes_hospital will be skipped until dataset is fixed."
+            pytest.skip(msg)
+        dataset = fetch_function(as_frame=as_frame)
         assert dataset is not None
         assert dataset["data"].shape is not None
         assert isinstance(dataset["data"], pd.DataFrame if as_frame else np.ndarray)
         assert dataset["target"].shape is not None
         assert isinstance(dataset["target"], pd.Series if as_frame else np.ndarray)
         assert dataset["feature_names"] is not None
         assert isinstance(dataset["feature_names"], list)
@@ -47,26 +44,30 @@
         assert isinstance(dataset["DESCR"], str)
 
     @pytest.mark.parametrize("as_frame", [True, False])
     @pytest.mark.parametrize(
         "fetch_function",
         [
             fetch_adult,
-            fetch_boston,
             fetch_bank_marketing,
+            fetch_boston,
+            fetch_credit_card,
             fetch_diabetes_hospital,
         ],
     )
     def test_dataset_as_X_y(self, as_frame, fetch_function):
-        if fetch_function == fetch_diabetes_hospital:
-            if as_frame is True:
-                X, y = fetch_function(return_X_y=True)
-            elif as_frame is False:
-                pytest.skip(
-                    "Skipping the diabetes hospital dataset with as_frame False"
-                )
-        else:
-            X, y = fetch_function(as_frame=as_frame, return_X_y=True)
+        if as_frame is False and fetch_function is fetch_diabetes_hospital:
+            msg = "fetch_diabetes_hospital will be skipped until dataset is fixed."
+            pytest.skip(msg)
+        X, y = fetch_function(as_frame=as_frame, return_X_y=True)
         assert X is not None
         assert isinstance(X, pd.DataFrame if as_frame else np.ndarray)
         assert y is not None
         assert isinstance(y, pd.Series if as_frame else np.ndarray)
+
+    def test_fetch_diabetes_hospital_as_ndarray_raises_value_error(self):
+        # Once this test no longer passes, the NOTE in the docstring of
+        # fetch_diabetes_hospital regarding as_frame and the if clauses in
+        # both dataset tests can be removed because the OpenML dataset has
+        # been fixed.
+        with pytest.raises(ValueError):
+            fetch_diabetes_hospital(as_frame=False)
```

### Comparing `fairlearn-0.8.0.dev0/test/unit/input_convertors.py` & `fairlearn-0.9.0/test/unit/input_convertors.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/metrics/data_for_test.py` & `fairlearn-0.9.0/test/unit/metrics/data_for_test.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/metrics/test_annotated_metric_function.py` & `fairlearn-0.9.0/test/unit/metrics/test_annotated_metric_function.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/metrics/test_disaggregated_result.py` & `fairlearn-0.9.0/test/unit/metrics/test_disaggregated_result.py`

 * *Files 14% similar despite different names*

```diff
@@ -47,17 +47,49 @@
             sensitive_feature_names=["g_1"],
             control_feature_names=None,
         )
         with pytest.raises(ValueError) as e0:
             _ = target.difference(control_feature_names=None, method="bad_func")
         assert str(e0.value) == "Unrecognised method 'bad_func' in difference() call"
 
+    def test_bad_difference_errors(self):
+        target = DisaggregatedResult.create(
+            data=basic_data,
+            annotated_functions=metric_dict,
+            sensitive_feature_names=["g_1"],
+            control_feature_names=None,
+        )
+        with pytest.raises(ValueError) as e0:
+            _ = target.difference(
+                control_feature_names=None, method="between_groups", errors="bad_option"
+            )
+        assert (
+            str(e0.value)
+            == "Invalid error value specified. Valid values are ['raise', 'coerce']"
+        )
+
     def test_bad_ratio_method(self):
         target = DisaggregatedResult.create(
             data=basic_data,
             annotated_functions=metric_dict,
             sensitive_feature_names=["g_1"],
             control_feature_names=None,
         )
         with pytest.raises(ValueError) as e0:
             _ = target.ratio(control_feature_names=None, method="bad_func")
         assert str(e0.value) == "Unrecognised method 'bad_func' in ratio() call"
+
+    def test_bad_ratio_errors(self):
+        target = DisaggregatedResult.create(
+            data=basic_data,
+            annotated_functions=metric_dict,
+            sensitive_feature_names=["g_1"],
+            control_feature_names=None,
+        )
+        with pytest.raises(ValueError) as e0:
+            _ = target.ratio(
+                control_feature_names=None, method="between_groups", errors="bad_option"
+            )
+        assert (
+            str(e0.value)
+            == "Invalid error value specified. Valid values are ['raise', 'coerce']"
+        )
```

### Comparing `fairlearn-0.8.0.dev0/test/unit/metrics/test_disparities.py` & `fairlearn-0.9.0/test/unit/metrics/test_fairness_metrics.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/metrics/test_extra_metrics.py` & `fairlearn-0.9.0/test/unit/metrics/test_base_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Licensed under the MIT License.
 
 import numpy as np
 import pytest
 import sklearn.metrics as skm
 
 import fairlearn.metrics as metrics
-from fairlearn.metrics._extra_metrics import _get_labels_for_confusion_matrix
+from fairlearn.metrics._base_metrics import _get_labels_for_confusion_matrix
 
 # =============================================
 
 
 class TestGetLabelsForConfusionMatrix:
     def test_smoke(self):
         r0 = _get_labels_for_confusion_matrix([0, 1], None)
```

### Comparing `fairlearn-0.8.0.dev0/test/unit/metrics/test_generated_metrics.py` & `fairlearn-0.9.0/test/unit/metrics/test_generated_metrics.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,16 +3,27 @@
 
 import pytest
 
 import fairlearn.metrics as metrics
 
 # ======================================================
 
+# Evaluation of log loss with y_true=1 and y_pred=0 (or vice versa)
+# gives mathematically an infinite value. Scikit-learn in this case
+# returns a finite value based on the setting of the keyword parameter
+# eps of log_loss function. In our tests with log loss, we replace 0 with
+# apx0 and 1 with apx1 in y_pred when it disagrees with y_true. This
+# avoids the issue of an infinite log loss.
+
+apx0 = 1e-15
+apx1 = 1 - apx0
+
 y_true = [0, 0, 0, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1]
 y_pred = [1, 0, 1, 0, 1, 0, 0, 1, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1]
+y_pred_log_loss = [apx1, 0, apx1, apx0, 1, apx0, 0, apx1, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1]
 sf_binary = [0, 1, 0, 1, 0, 1, 0, 1, 0, 1, 0, 1, 0, 1, 0, 1, 0, 1]
 
 derived_metric_results = {
     "true_positive_rate_difference": {"method": "to_overall", "expected": 0.25},
     "true_positive_rate_ratio": {"method": "to_overall", "expected": 0.75},
     "true_negative_rate_difference": {
         "method": "between_groups",
@@ -53,17 +64,21 @@
     assert len(metrics._generated_metric_dict) == 25
 
 
 @pytest.mark.parametrize("func_name", derived_metric_results.keys())
 def test_generated_metrics_smoke(func_name):
     func = getattr(metrics, func_name)
     assert callable(func)
+    if func_name.startswith("log_loss"):
+        y_pred_test = y_pred_log_loss
+    else:
+        y_pred_test = y_pred
     result = func(
         y_true,
-        y_pred,
+        y_pred_test,
         sensitive_features=sf_binary,
         method=derived_metric_results[func_name]["method"],
     )
     assert result == pytest.approx(derived_metric_results[func_name]["expected"])
 
 
 @pytest.mark.parametrize("method", ["between_groups", "to_overall"])
```

### Comparing `fairlearn-0.8.0.dev0/test/unit/metrics/test_group_feature.py` & `fairlearn-0.9.0/test/unit/metrics/test_group_feature.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/metrics/test_make_derived_metric.py` & `fairlearn-0.9.0/test/unit/metrics/test_make_derived_metric.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/metrics/test_mean_predictions.py` & `fairlearn-0.9.0/test/unit/metrics/test_mean_predictions.py`

 * *Files 20% similar despite different names*

```diff
@@ -36,83 +36,7 @@
     y_pred = [42]
     y_true = None
     weight = [2]
 
     result = metrics.mean_prediction(y_true, y_pred, weight)
 
     assert result == 42
-
-
-def test_mean_overprediction_unweighted():
-    y_pred = [0, 1, 2, 3, 4]
-    y_true = [1, 1, 5, 0, 2]
-
-    result = metrics._mean_overprediction(y_true, y_pred)
-
-    assert result == 1
-
-
-def test_mean_overprediction_unweighted_single():
-    y_pred = [1]
-    y_true = [0]
-
-    result = metrics._mean_overprediction(y_true, y_pred)
-
-    assert result == 1
-
-
-def test_mean_overprediction_weighted():
-    y_pred = [0, 1, 2, 3, 4]
-    y_true = [1, 1, 5, 0, 2]
-    weight = [3, 1, 7, 1, 2]
-
-    result = metrics._mean_overprediction(y_true, y_pred, weight)
-
-    assert result == 0.5
-
-
-def test_mean_overprediction_weighted_single():
-    y_pred = [1]
-    y_true = [0]
-    weight = [1]
-
-    result = metrics._mean_overprediction(y_true, y_pred, weight)
-
-    assert result == 1
-
-
-def test_mean_underprediction_unweighted():
-    y_pred = [0, 1, 1, 3, 4]
-    y_true = [1, 1, 5, 0, 2]
-
-    result = metrics._mean_underprediction(y_true, y_pred)
-
-    assert result == 1
-
-
-def test_mean_underprediction_unweighted_single():
-    y_pred = [0]
-    y_true = [1]
-
-    result = metrics._mean_underprediction(y_true, y_pred)
-
-    assert result == 1
-
-
-def test_mean_underprediction_weighted():
-    y_pred = [0, 1, 5, 3, 1]
-    y_true = [1, 1, 2, 0, 2]
-    weight = [4, 1, 2, 2, 1]
-
-    result = metrics._mean_underprediction(y_true, y_pred, weight)
-
-    assert result == 0.5
-
-
-def test_mean_underprediction_weighted_single():
-    y_pred = [0]
-    y_true = [42]
-    weight = [2]
-
-    result = metrics._mean_underprediction(y_true, y_pred, weight)
-
-    assert result == 42
```

### Comparing `fairlearn-0.8.0.dev0/test/unit/metrics/test_metricframe_aggregates.py` & `fairlearn-0.9.0/test/unit/metrics/test_metricframe_aggregates.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,14 +132,28 @@
 
         mf = metrics.MetricFrame(
             metrics=my_prec, y_true=[1, 0], y_pred=[1, 0], sensitive_features=["a", "b"]
         )
 
         assert mf.ratio(method="to_overall") == 0
 
+    def test_difference_bad_method(self):
+        self._prepare(skm.accuracy_score)
+
+        with pytest.raises(ValueError) as exc:
+            self.target.difference(method="some_string")
+        assert "Unrecognised comparison method: some_string" == exc.value.args[0]
+
+    def test_ratio_bad_method(self):
+        self._prepare(skm.accuracy_score)
+
+        with pytest.raises(ValueError) as exc:
+            self.target.ratio(method="some_other_string")
+        assert "Unrecognised comparison method: some_other_string" == exc.value.args[0]
+
 
 class Test1m1sf0cfFnDict:
     # Key difference is that the function is supplied as a dict
     def _prepare(self, metric_fn):
         self.mfn = "Random name"
         self.target = metrics.MetricFrame(
             metrics={self.mfn: metric_fn},
```

### Comparing `fairlearn-0.8.0.dev0/test/unit/metrics/test_metricframe_by_group.py` & `fairlearn-0.9.0/test/unit/metrics/test_metricframe_by_group.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/metrics/test_metricframe_comprehensive.py` & `fairlearn-0.9.0/test/unit/metrics/test_metricframe_comprehensive.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/metrics/test_metricframe_deprecate.py` & `fairlearn-0.9.0/test/unit/metrics/test_metricframe_deprecate.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,24 +78,23 @@
         )
 
     assert len(record) == 1
     assert str(record[0].message) == msg
     assert mf.difference() == pytest.approx(accuracy_score_difference)
 
 
-def test_no_warnings():
-    with pytest.warns(None) as record:
-        mf = metrics.MetricFrame(
-            metrics=skm.accuracy_score,
-            y_true=y_true,
-            y_pred=y_pred,
-            sensitive_features=sf,
-        )
+def test_no_warnings(recwarn):
+    mf = metrics.MetricFrame(
+        metrics=skm.accuracy_score,
+        y_true=y_true,
+        y_pred=y_pred,
+        sensitive_features=sf,
+    )
 
-    assert len(record) == 0
+    assert len(recwarn) == 0
     assert mf.difference() == pytest.approx(accuracy_score_difference)
 
 
 def test_metric_and_metrics():
     warn_msg = (
         "The positional argument 'metric' has been replaced by "
         f"a keyword argument 'metrics'. From version {version} passing "
```

### Comparing `fairlearn-0.8.0.dev0/test/unit/metrics/test_metricframe_missing.py` & `fairlearn-0.9.0/test/unit/metrics/test_metricframe_missing.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 n = len(y_t)
 g_A = np.asarray([group_gen(x, int(n / 2), ["aa", "bb"]) for x in range(n)])
 g_B = np.asarray([group_gen(x, 1 + int(n / 3), ["x", "y", "z"]) for x in range(n)])
 
 
 @pytest.mark.parametrize("metric_fn", metric)
 def test_missing_sensitive_feature_combinations(metric_fn):
-
     target = metrics.MetricFrame(
         metrics=metric_fn,
         y_true=y_t,
         y_pred=y_p,
         sensitive_features=np.stack([g_A, g_B], axis=1),
     )
```

### Comparing `fairlearn-0.8.0.dev0/test/unit/metrics/test_metricframe_multiclass.py` & `fairlearn-0.9.0/test/unit/metrics/test_metricframe_multiclass.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/metrics/test_metricframe_nonscalar.py` & `fairlearn-0.9.0/test/unit/metrics/test_metricframe_nonscalar.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/metrics/test_metricframe_overall.py` & `fairlearn-0.9.0/test/unit/metrics/test_metricframe_overall.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/metrics/test_metricframe_process_features.py` & `fairlearn-0.9.0/test/unit/metrics/test_metricframe_process_features.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/metrics/test_metricframe_smoke.py` & `fairlearn-0.9.0/test/unit/metrics/test_metricframe_smoke.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/metrics/test_plot_metricframe.py` & `fairlearn-0.9.0/test/unit/metrics/test_plot_metricframe.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/metrics/test_plot_model_comparison.py` & `fairlearn-0.9.0/test/unit/metrics/test_plot_model_comparison.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,14 @@
 
 
 def random_metric2(yp, yt):
     return np.mean(yp == yt) ** 2
 
 
 def test_named():
-
     ax = plot_model_comparison(
         x_axis_metric=random_metric1,
         y_axis_metric=random_metric2,
         y_true=y_t,
         y_preds=y_p,
         sensitive_features=g_1,
     )
```

### Comparing `fairlearn-0.8.0.dev0/test/unit/postprocessing/conftest.py` & `fairlearn-0.9.0/test/unit/postprocessing/conftest.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/postprocessing/test_curve_utilities.py` & `fairlearn-0.9.0/test/unit/postprocessing/test_curve_utilities.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/postprocessing/test_plots.py` & `fairlearn-0.9.0/test/unit/postprocessing/test_plots.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Microsoft Corporation and Fairlearn contributors.
 # Licensed under the MIT License.
 
-import pkg_resources
+from importlib.metadata import PackageNotFoundError
 import pytest
 
 from fairlearn.postprocessing import ThresholdOptimizer, plot_threshold_optimizer
 
 from .conftest import ExamplePredictor, _data_ex1, _data_ex2, _data_ex3, scores_ex
 
 PYTEST_MPL_NOT_INSTALLED_MSG = (
@@ -39,18 +39,19 @@
     fig, (ax) = plt.subplots(1, 1)
     plot_threshold_optimizer(adjusted_predictor, ax=ax, show_plot=False)
     return fig
 
 
 def is_mpl_installed():
     try:
-        pkg_resources.get_distribution("pytest-mpl")
-        pkg_resources.get_distribution("matplotlib")
+        import pytest_mpl  # noqa: F401
+        import matplotlib.pyplot as plt  # noqa: F401
+
         return True
-    except pkg_resources.DistributionNotFound:
+    except PackageNotFoundError:
         return False
 
 
 @pytest.mark.skipif(not is_mpl_installed(), reason=PYTEST_MPL_NOT_INSTALLED_MSG)
 class TestPlots:
     @pytest.mark.mpl_image_compare(filename="equalized_odds_ex1.png")
     def test_plot_equalized_odds_ex1(self):
```

### Comparing `fairlearn-0.8.0.dev0/test/unit/postprocessing/test_smoke.py` & `fairlearn-0.9.0/test/unit/postprocessing/test_smoke.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/postprocessing/test_threshold_operation.py` & `fairlearn-0.9.0/test/unit/postprocessing/test_threshold_operation.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/postprocessing/test_threshold_optimization.py` & `fairlearn-0.9.0/test/unit/postprocessing/test_threshold_optimization.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/postprocessing/test_threshold_optimizer_multiple_sensitive_features.py` & `fairlearn-0.9.0/test/unit/postprocessing/test_threshold_optimizer_multiple_sensitive_features.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/preprocessing/linear_dep_remover/test_sklearn_compat.py` & `fairlearn-0.9.0/test/unit/preprocessing/linear_dep_remover/test_sklearn_compat.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/reductions/data_generators.py` & `fairlearn-0.9.0/test/unit/reductions/data_generators.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/reductions/exponentiated_gradient/simple_learners.py` & `fairlearn-0.9.0/test/unit/reductions/exponentiated_gradient/simple_learners.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/reductions/exponentiated_gradient/test_control_features.py` & `fairlearn-0.9.0/test/unit/reductions/exponentiated_gradient/test_control_features.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/reductions/exponentiated_gradient/test_exponentiatedgradient_arguments.py` & `fairlearn-0.9.0/test/unit/reductions/exponentiated_gradient/test_exponentiatedgradient_arguments.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/reductions/exponentiated_gradient/test_exponentiatedgradient_smoke.py` & `fairlearn-0.9.0/test/unit/reductions/exponentiated_gradient/test_exponentiatedgradient_smoke.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/reductions/exponentiated_gradient/test_lagrangian.py` & `fairlearn-0.9.0/test/unit/reductions/exponentiated_gradient/test_lagrangian.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/reductions/exponentiated_gradient/test_utilities.py` & `fairlearn-0.9.0/test/unit/reductions/exponentiated_gradient/test_utilities.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/reductions/grid_search/test_grid_generator.py` & `fairlearn-0.9.0/test/unit/reductions/grid_search/test_grid_generator.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/reductions/grid_search/test_grid_search_arguments.py` & `fairlearn-0.9.0/test/unit/reductions/grid_search/test_grid_search_arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,14 @@
         else:
             assert len(log_records) == 0
 
     @pytest.mark.parametrize("transformX", candidate_X_transforms)
     @pytest.mark.parametrize("transformY", candidate_Y_transforms)
     @pytest.mark.parametrize("transformA", candidate_A_transforms)
     def test_custom_grid(self, transformX, transformY, transformA):
-
         # Creating a standard grid with the default parameters
         grid_size = 10
         grid_limit = 2.0
         grid_offset = 0.1
 
         disparity_moment = EqualizedOdds()
         X, y, A = _quick_data(False)
@@ -312,15 +311,14 @@
     # ----------------------------
 
     @pytest.mark.parametrize("transformA", candidate_A_transforms)
     @pytest.mark.parametrize("transformX", candidate_X_transforms)
     @pytest.mark.parametrize("A_two_dim", [False, True])
     @pytest.mark.uncollect_if(func=is_invalid_transformation)
     def test_Y_df_bad_columns(self, transformX, transformA, A_two_dim):
-
         gs = GridSearch(
             self.estimator,
             self.disparity_criterion,
             sample_weight_name=self.sample_weight_name,
         )
         X, Y, A = _quick_data(A_two_dim)
```

### Comparing `fairlearn-0.8.0.dev0/test/unit/reductions/grid_search/test_grid_search_demographicparity.py` & `fairlearn-0.9.0/test/unit/reductions/grid_search/test_grid_search_demographicparity.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     number_a1,
     a0_threshold,
     a1_threshold,
     a0_label,
     a1_label,
     A_two_dim=False,
 ):
-
     a0s = np.full(number_a0, a0_label)
     a1s = np.full(number_a1, a1_label)
 
     a0_scores = np.linspace(0, 1, number_a0)
     a1_scores = np.linspace(0, 1, number_a1)
     score_feature = np.concatenate((a0_scores, a1_scores), axis=None)
 
@@ -36,15 +35,15 @@
     Y_a1 = [x > a1_threshold for x in a1_scores]
 
     Y = np.concatenate((Y_a0, Y_a1), axis=None)
 
     X = pd.DataFrame(
         {
             "actual_feature": score_feature,
-            "sensitive_feature1": A,
+            "sensitive_features": A,
             "constant_ones_feature": np.ones(len(Y)),
         }
     )
 
     if A_two_dim:
         A = np.stack((A, A), -1)
```

### Comparing `fairlearn-0.8.0.dev0/test/unit/reductions/grid_search/test_grid_search_regression.py` & `fairlearn-0.9.0/test/unit/reductions/grid_search/test_grid_search_regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 from fairlearn.reductions import BoundedGroupLoss, GridSearch, SquareLoss, ZeroOneLoss
 
 
 def _simple_regression_data(
     number_a0, number_a1, a0_factor, a1_factor, a0_label, a1_label, A_two_dim=False
 ):
-
     a0s = np.full(number_a0, a0_label)
     a1s = np.full(number_a1, a1_label)
 
     a0_scores = np.linspace(0, 1, number_a0)
     a1_scores = np.linspace(0, 1, number_a1)
     score_feature = np.concatenate((a0_scores, a1_scores), axis=None)
 
@@ -124,15 +123,15 @@
 
     estimator = LinearRegression()
 
     unmitigated_estimator = copy.deepcopy(estimator)
     unmitigated_estimator.fit(X, y)
 
     # Do the grid search with a zero Lagrange multiplier
-    idx = pd.Int64Index(sorted([a0_label, a1_label]))
+    idx = pd.Index(sorted([a0_label, a1_label]))
     lagrange_balanced_series = pd.Series([1.0, 1.0], index=idx)
     grid_df = pd.DataFrame(lagrange_balanced_series)
 
     grid_search = GridSearch(
         estimator, constraints=BoundedGroupLoss(ZeroOneLoss()), grid=grid_df
     )
     grid_search.fit(X, y, sensitive_features=A)
@@ -159,15 +158,15 @@
     X, y, A = _simple_regression_data(
         a0_count, a1_count, a0_factor, a1_factor, a0_label, a1_label, A_two_dim
     )
 
     estimator = LinearRegression()
 
     # Do the grid search with a zero Lagrange multiplier
-    idx = pd.Int64Index(sorted([a0_label, a1_label]))
+    idx = pd.Index(sorted([a0_label, a1_label]))
     l0_series = pd.Series([2.0, 0.0], index=idx)
     l1_series = pd.Series([1.5, 0.5], index=idx)
     l2_series = pd.Series([1.0, 1.0], index=idx)
     l3_series = pd.Series([0.5, 1.5], index=idx)
     l4_series = pd.Series([0.0, 2.0], index=idx)
     grid_df = pd.concat([l0_series, l1_series, l2_series, l3_series, l4_series], axis=1)
```

### Comparing `fairlearn-0.8.0.dev0/test/unit/reductions/grid_search/utilities.py` & `fairlearn-0.9.0/test/unit/reductions/grid_search/utilities.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/reductions/moments/data_generator.py` & `fairlearn-0.9.0/test/unit/reductions/moments/data_generator.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/reductions/moments/test_moments_bounded_group_loss.py` & `fairlearn-0.9.0/test/unit/reductions/moments/test_moments_bounded_group_loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
         self.disparity_criterion.load_data(X, Y, sensitive_features=A)
         bnd = self.disparity_criterion.bound()
         loss_eps = self.disparity_criterion.gamma(predictor) - bnd
         loss = self.disparity_criterion.gamma(predictor)
         assert np.all(np.isclose(loss - eps, loss_eps))
 
     def test_bgl_gpa_data(self):
-
         names = [
             "gender",
             "physics",
             "biology",
             "history",
             "second_language",
             "geography",
```

### Comparing `fairlearn-0.8.0.dev0/test/unit/reductions/moments/test_moments_control_features.py` & `fairlearn-0.9.0/test/unit/reductions/moments/test_moments_control_features.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Copyright (c) Microsoft Corporation and Fairlearn contributors.
 # Licensed under the MIT License.
 
 from test.unit.reductions.data_generators import loan_scenario_generator
 
-import numpy as np
 import pandas as pd
 import pytest
 from sklearn.linear_model import LogisticRegression
 from sklearn.metrics import accuracy_score
 
 from fairlearn.metrics import (
     MetricFrame,
@@ -50,16 +49,16 @@
 
     est = LogisticRegression()
     est.fit(X_dummy, y)
     y_pred = est.predict(X_dummy)
 
     target = moment()
     target.load_data(
-        np.asarray(X_dummy),
-        np.asarray(y),
+        X_dummy,
+        y,
         sensitive_features=X["sens"],
         control_features=X["ctrl"],
     )
 
     # gamma measures the constraint violation relative to the overall value
     results = target.gamma(est.predict)
 
@@ -103,16 +102,16 @@
 
     est = LogisticRegression()
     est.fit(X_dummy, y)
     y_pred = est.predict(X_dummy)
 
     target = moment()
     target.load_data(
-        np.asarray(X_dummy),
-        np.asarray(y),
+        X_dummy,
+        y,
         sensitive_features=X["sens"],
         control_features=X["ctrl"],
     )
 
     # gamma measures the constraint violation relative to the overall value
     results = target.gamma(est.predict)
```

### Comparing `fairlearn-0.8.0.dev0/test/unit/reductions/moments/test_moments_demographic_parity.py` & `fairlearn-0.9.0/test/unit/reductions/moments/test_moments_demographic_parity.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/reductions/moments/test_moments_equalized_odds.py` & `fairlearn-0.9.0/test/unit/reductions/moments/test_moments_equalized_odds.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,9 +208,8 @@
     w_a0_F = np.full(num_a0_F, sw_a0_F)
     w_a0_T = np.full(num_a0_T, sw_a0_T)
     w_a1_F = np.full(num_a1_F, sw_a1_F)
     w_a1_T = np.full(num_a1_T, sw_a1_T)
     expected = np.concatenate((w_a0_F, w_a0_T, w_a1_F, w_a1_T), axis=None)
 
     signed_weights = eqo.signed_weights(lambda_vec)
-    # Be bold and test for equality
-    assert np.array_equal(expected, signed_weights)
+    assert np.allclose(expected, signed_weights)
```

### Comparing `fairlearn-0.8.0.dev0/test/unit/reductions/moments/test_moments_error_rate.py` & `fairlearn-0.9.0/test/unit/reductions/moments/test_moments_error_rate.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/reductions/test_smoke.py` & `fairlearn-0.9.0/test/unit/reductions/test_smoke.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/test_random_state.py` & `fairlearn-0.9.0/test/unit/test_random_state.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Licensed under the MIT License.
 
 import pandas as pd
 from sklearn.datasets import fetch_openml
 from sklearn.linear_model import LogisticRegression
 from sklearn.model_selection import train_test_split
 
+import fairlearn.utils._compatibility as compat
 from fairlearn.postprocessing import ThresholdOptimizer
 from fairlearn.reductions import EqualizedOdds, ExponentiatedGradient
 
 
 def test_random_state_threshold_optimizer():
     """Test that the random_state argument works as expected.
 
@@ -66,15 +67,15 @@
     for _ in range(100):
         assert (y_pred_test == expgrad.predict(X_test, random_state=0)).all()
     assert (y_pred_test != expgrad.predict(X_test, random_state=1)).any()
 
 
 def _get_test_data():
     # fetch data from OpenML
-    data = fetch_openml(data_id=42193)
+    data = fetch_openml(data_id=42193, **compat._PARSER_KWARG)
     X = (
         pd.DataFrame(data["data"], columns=data["feature_names"])
         .drop(columns=["race_Caucasian", "c_charge_degree_F"])
         .astype(float)
     )
     y = data["target"].astype(int)
```

### Comparing `fairlearn-0.8.0.dev0/test/unit/test_show_versions.py` & `fairlearn-0.9.0/test/unit/test_show_versions.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test/unit/utility_functions.py` & `fairlearn-0.9.0/test/unit/utility_functions.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test_othermlpackages/adversarial_fairness.py` & `fairlearn-0.9.0/test_othermlpackages/adversarial_fairness.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 
 from sklearn.compose import make_column_transformer, make_column_selector
 from sklearn.preprocessing import OneHotEncoder, StandardScaler
 from sklearn.impute import SimpleImputer
 from sklearn.pipeline import Pipeline
 import torch
 from numpy import mean, number
-from sklearn.datasets import fetch_openml
 
+import fairlearn.utils._compatibility as compat
+from fairlearn.datasets import fetch_adult
 from fairlearn.metrics import (
     MetricFrame,
     selection_rate,
     demographic_parity_difference,
 )
 from sklearn.metrics import accuracy_score
 
@@ -24,15 +25,15 @@
 # Global variables of test_examples()
 schedulers = []
 step = 1
 
 
 def test_examples():
     # EXAMPLE 1
-    X, y = fetch_openml(data_id=1590, as_frame=True, return_X_y=True)
+    X, y = fetch_adult(return_X_y=True)
     pos_label = y[0]
 
     z = X["sex"]  # In this example, we consider 'sex' the sensitive feature.
 
     ct = make_column_transformer(
         (
             Pipeline(
@@ -43,15 +44,18 @@
             ),
             make_column_selector(dtype_include=number),
         ),
         (
             Pipeline(
                 [
                     ("imputer", SimpleImputer(strategy="most_frequent")),
-                    ("encoder", OneHotEncoder(drop="if_binary", sparse=False)),
+                    (
+                        "encoder",
+                        OneHotEncoder(drop="if_binary", **compat._SPARSE_OUTPUT_FALSE),
+                    ),
                 ]
             ),
             make_column_selector(dtype_include="category"),
         ),
     )
 
     X_train, X_test, Y_train, Y_test, Z_train, Z_test = train_test_split(
@@ -61,15 +65,15 @@
     X_prep_train = ct.fit_transform(X_train)  # Only fit on training data!
     X_prep_test = ct.transform(X_test)
 
     mitigator = AdversarialFairnessClassifier(
         backend="torch",
         predictor_model=[50, "leaky_relu"],
         adversary_model=[3, "leaky_relu"],
-        batch_size=2 ** 8,
+        batch_size=2**8,
         progress_updates=0.5,
         random_state=123,
     )
 
     mitigator.fit(X_prep_train, Y_train, sensitive_features=Z_train)
 
     predictions = mitigator.predict(X_prep_test)
@@ -143,15 +147,15 @@
 
     mitigator = AdversarialFairnessClassifier(
         predictor_model=predictor_model,
         adversary_model=[3, "leaky_relu"],
         predictor_optimizer=optimizer_constructor,
         adversary_optimizer=optimizer_constructor,
         epochs=10,
-        batch_size=2 ** 7,
+        batch_size=2**7,
         shuffle=True,
         callbacks=callbacks,
         random_state=123,
     )
 
     mitigator.fit(X_prep_train, Y_train, sensitive_features=Z_train)
 
@@ -173,15 +177,15 @@
             ("preprocessor", ct),
             (
                 "classifier",
                 AdversarialFairnessClassifier(
                     backend="torch",
                     predictor_model=[50, "leaky_relu"],
                     adversary_model=[3, "leaky_relu"],
-                    batch_size=2 ** 8,
+                    batch_size=2**8,
                     random_state=123,
                 ),
             ),
         ]
     )
 
     pipeline.fit(X_train, Y_train, classifier__sensitive_features=Z_train)
```

### Comparing `fairlearn-0.8.0.dev0/test_othermlpackages/package_test_common.py` & `fairlearn-0.9.0/test_othermlpackages/package_test_common.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,31 +4,32 @@
 """Common testing methods for use with other ML packages."""
 
 import copy
 
 import pandas as pd
 from numpy import mean, random, number
 
-from sklearn.datasets import fetch_openml
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import LabelEncoder, StandardScaler, OneHotEncoder
 from sklearn.compose import make_column_selector, make_column_transformer
 
+import fairlearn.utils._compatibility as compat
+import fairlearn.datasets as fld
 from fairlearn.metrics import demographic_parity_difference
 from fairlearn.postprocessing import ThresholdOptimizer
 from fairlearn.reductions import ExponentiatedGradient, GridSearch
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 def fetch_adult():
     """Grab dataset for testing."""
-    data = fetch_openml(data_id=1590, as_frame=True)
+    data = fld.fetch_adult()
     X = data.data.drop(labels=["sex"], axis=1)
     X = pd.get_dummies(X)
     Y = (data.target == ">50K") * 1
     A = data.data["sex"]
 
     le = LabelEncoder()
     Y = le.fit_transform(Y)
@@ -123,15 +124,15 @@
     assert dp_diff_mitigated <= dp_diff_unmitigated
 
 
 def run_AdversarialFairness_classification(estimator):
     """Run classification test with AdversarialFairness."""
     random.seed(123)
 
-    X, y = fetch_openml(data_id=1590, as_frame=True, return_X_y=True)
+    X, y = fld.fetch_adult(return_X_y=True)
 
     non_NaN_rows = ~X.isna().any(axis=1)
 
     X = X[non_NaN_rows]
     y = y[non_NaN_rows]
 
     sensitive_feature = X["sex"]
@@ -139,30 +140,30 @@
     def preprocess(X):
         if isinstance(X, pd.Series):
             X = X.to_frame()
         """Make the Transformer for a single dataframe."""
         ct = make_column_transformer(
             (StandardScaler(), make_column_selector(dtype_include=number)),
             (
-                OneHotEncoder(drop="if_binary", sparse=False),
+                OneHotEncoder(drop="if_binary", **compat._SPARSE_OUTPUT_FALSE),
                 make_column_selector(dtype_include="category"),
             ),
         )
         return ct.fit_transform(X)
 
     X = preprocess(X)
     y = preprocess(y)
     sensitive_feature = preprocess(sensitive_feature)
 
     X_train, X_test, Y_train, Y_test, A_train, A_test = train_test_split(
         X, y, sensitive_feature, test_size=0.2, random_state=12345, stratify=y
     )
 
     estimator.epochs = 100
-    estimator.batch_size = 2 ** 9
+    estimator.batch_size = 2**10
     estimator.shuffle = True
     estimator.progress_updates = None
 
     estimator.fit(X_train, Y_train, sensitive_features=A_train)
 
     predictions = estimator.predict(X_test)
 
@@ -170,15 +171,14 @@
         Y_test, predictions, sensitive_features=A_test
     )
 
     accuracy = mean(predictions == Y_test)
 
     # This might give problems as it is a bit random (though we set a seed,
     # it may depend on other factors such as version).
-    if not (accuracy > 0.6 and dp_diff < 0.3):
+    if not (accuracy > 0.8 and dp_diff < 0.2):
         logger.warning(
             "Training of AdversarialFairness is worse than usual."  # noqa
             + f"Accuracy {str(accuracy)} with a disparity difference of"  # noqa
             + f"{str(dp_diff)}."  # noqa
         )
-
     assert estimator is not None
```

### Comparing `fairlearn-0.8.0.dev0/test_othermlpackages/test_lightgbm.py` & `fairlearn-0.9.0/test_othermlpackages/test_lightgbm.py`

 * *Files identical despite different names*

### Comparing `fairlearn-0.8.0.dev0/test_othermlpackages/test_pytorch.py` & `fairlearn-0.9.0/test_othermlpackages/test_pytorch.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,18 +29,18 @@
                 nn.Sigmoid(),
             )
 
         def forward(self, X, **kwargs):
             return self.model(X)
 
     class SampleWeightNeuralNet(NeuralNetClassifier):
-        def __init__(self, *args, criterion__reduce=False, **kwargs):
+        def __init__(self, *args, criterion__reduction="none", **kwargs):
             # make sure to set reduce=False in your criterion, since we need the loss
             # for each sample so that it can be weighted
-            super().__init__(*args, criterion__reduce=criterion__reduce, **kwargs)
+            super().__init__(*args, criterion__reduction=criterion__reduction, **kwargs)
 
         def fit(self, X, y, sample_weight=None):
             if isinstance(X, (pd.DataFrame, pd.Series)):
                 X = X.to_numpy().astype("float32")
             if isinstance(y, (pd.DataFrame, pd.Series)):
                 y = y.to_numpy()
             if sample_weight is not None and isinstance(
@@ -54,17 +54,15 @@
             )
             X = {"X": X, "sample_weight": sample_weight}
             return super().fit(X, y)
 
         def predict(self, X):
             if isinstance(X, (pd.DataFrame, pd.Series)):
                 X = X.to_numpy().astype("float32")
-            # The base implementation uses np.argmax which works
-            # for multiclass classification only.
-            return (super().predict_proba(X) > 0.5).astype(float)
+            return super().predict(X).squeeze()
 
         def get_loss(self, y_pred, y_true, X, *args, **kwargs):
             # override get_loss to use the sample_weight from X
             loss_unreduced = super().get_loss(
                 y_pred, y_true.float(), X, *args, **kwargs
             )
             sample_weight = X["sample_weight"]
```

### Comparing `fairlearn-0.8.0.dev0/test_othermlpackages/test_tensorflow.py` & `fairlearn-0.9.0/test_othermlpackages/test_tensorflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,29 +23,29 @@
     model.add(Dense(1, activation="sigmoid"))
     # Compile model
     model.compile(loss="binary_crossentropy", optimizer="adam", metrics=["accuracy"])
     return model
 
 
 def test_expgrad_classification():
-    estimator = KerasClassifier(build_fn=create_model)
+    estimator = KerasClassifier(model=create_model)
     disparity_moment = DemographicParity()
 
     ptc.run_expgrad_classification(estimator, disparity_moment)
 
 
 def test_gridsearch_classification():
-    estimator = KerasClassifier(build_fn=create_model)
+    estimator = KerasClassifier(model=create_model)
     disparity_moment = DemographicParity()
 
     ptc.run_gridsearch_classification(estimator, disparity_moment)
 
 
 def test_thresholdoptimizer_classification():
-    estimator = KerasClassifier(build_fn=create_model)
+    estimator = KerasClassifier(model=create_model)
 
     ptc.run_thresholdoptimizer_classification(estimator)
 
 
 def test_adversarial_classification():
     mitigator = AdversarialFairnessClassifier(
         backend="tensorflow",
```

### Comparing `fairlearn-0.8.0.dev0/test_othermlpackages/test_xgboost.py` & `fairlearn-0.9.0/test_othermlpackages/test_xgboost.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 
 from . import package_test_common as ptc
 
 xgb = pytest.importorskip("xgboost")
 
 
 def test_expgrad_classification():
-    estimator = xgb.XGBClassifier(use_label_encoder=False)
+    estimator = xgb.XGBClassifier()
     disparity_moment = DemographicParity()
 
     ptc.run_expgrad_classification(estimator, disparity_moment)
 
 
 def test_gridsearch_classification():
-    estimator = xgb.XGBClassifier(use_label_encoder=False)
+    estimator = xgb.XGBClassifier()
     disparity_moment = DemographicParity()
 
     ptc.run_gridsearch_classification(estimator, disparity_moment)
 
 
 def test_thresholdoptimizer_classification():
-    estimator = xgb.XGBClassifier(use_label_encoder=False)
+    estimator = xgb.XGBClassifier()
 
     ptc.run_thresholdoptimizer_classification(estimator)
```

