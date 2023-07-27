# Comparing `tmp/fiddler-client-2.0.0.dev6.tar.gz` & `tmp/fiddler-client-2.0.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiddler-client-2.0.0.dev6.tar", last modified: Thu Jun 29 07:27:03 2023, max compression
+gzip compressed data, was "fiddler-client-2.0.0.dev7.tar", last modified: Thu Jul 27 12:35:18 2023, max compression
```

## Comparing `fiddler-client-2.0.0.dev6.tar` & `fiddler-client-2.0.0.dev7.tar`

### file list

```diff
@@ -1,89 +1,123 @@
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.125202 fiddler-client-2.0.0.dev6/
--rw-r--r--   0 runner    (1000) docker    (1001)       18 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/MANIFEST.in
--rw-r--r--   0 runner    (1000) docker    (1001)    20044 2023-06-29 07:27:03.125202 fiddler-client-2.0.0.dev6/PKG-INFO
--rw-r--r--   0 runner    (1000) docker    (1001)    16360 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/PUBLIC.md
--rw-r--r--   0 runner    (1000) docker    (1001)     2018 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/README.md
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.121202 fiddler-client-2.0.0.dev6/fiddler/
--rw-r--r--   0 runner    (1000) docker    (1001)     2019 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)       27 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/_version.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.121202 fiddler-client-2.0.0.dev6/fiddler/assets/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/assets/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     8200 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/assets/pg_reserved_words.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5105 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/client.py
--rw-r--r--   0 runner    (1000) docker    (1001)    21393 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/connection.py
--rw-r--r--   0 runner    (1000) docker    (1001)      354 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/constants.py
--rw-r--r--   0 runner    (1000) docker    (1001)   127839 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/core_objects.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4721 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/dataset.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2786 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/exceptions.py
--rw-r--r--   0 runner    (1000) docker    (1001)    26077 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/fiddler_api.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.121202 fiddler-client-2.0.0.dev6/fiddler/libs/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/libs/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     6455 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/libs/http_client.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5056 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/model.py
--rw-r--r--   0 runner    (1000) docker    (1001)    17897 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/monitoring_validator.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.121202 fiddler-client-2.0.0.dev6/fiddler/packtools/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/packtools/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4167 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/packtools/gem.py
--rw-r--r--   0 runner    (1000) docker    (1001)     7442 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/packtools/keras_ig_helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)    14619 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/packtools/project_attributions_helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     9500 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/packtools/template_model.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1808 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/project.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.121202 fiddler-client-2.0.0.dev6/fiddler/utils/
--rw-r--r--   0 runner    (1000) docker    (1001)     4370 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/utils/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1006 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/utils/exceptions.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3213 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/utils/formatting.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3084 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/utils/general_checks.py
--rw-r--r--   0 runner    (1000) docker    (1001)      782 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/utils/helper.py
--rw-r--r--   0 runner    (1000) docker    (1001)      188 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/utils/logging.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5010 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/utils/pandas.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.121202 fiddler-client-2.0.0.dev6/fiddler/v2/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/__init__.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.125202 fiddler-client-2.0.0.dev6/fiddler/v2/api/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)    14561 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/alert_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2603 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/api.py
--rw-r--r--   0 runner    (1000) docker    (1001)     6602 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/baseline_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    15923 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/dataset_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    14948 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/events_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    15328 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/explainability_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4725 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4502 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/job_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     8265 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/model_artifact_deploy.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3066 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/model_deployment_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    16989 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/model_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2937 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/api/project_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1241 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/constants.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.125202 fiddler-client-2.0.0.dev6/fiddler/v2/schema/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/schema/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4635 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/schema/alert.py
--rw-r--r--   0 runner    (1000) docker    (1001)      346 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/schema/base.py
--rw-r--r--   0 runner    (1000) docker    (1001)      490 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/schema/baseline.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3071 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/schema/dataset.py
--rw-r--r--   0 runner    (1000) docker    (1001)      885 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/schema/events.py
--rw-r--r--   0 runner    (1000) docker    (1001)      157 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/schema/job.py
--rw-r--r--   0 runner    (1000) docker    (1001)      453 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/schema/model.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1107 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/schema/model_deployment.py
--rw-r--r--   0 runner    (1000) docker    (1001)      124 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/schema/project.py
--rw-r--r--   0 runner    (1000) docker    (1001)      364 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/schema/server_info.py
--rw-r--r--   0 runner    (1000) docker    (1001)      109 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/schema/user.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.125202 fiddler-client-2.0.0.dev6/fiddler/v2/utils/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/utils/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3144 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/utils/decorators.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2306 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/utils/helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1835 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/utils/response_handler.py
--rw-r--r--   0 runner    (1000) docker    (1001)      362 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/utils/validations.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.125202 fiddler-client-2.0.0.dev6/fiddler/v2/validators/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/validators/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1498 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/v2/validators/dataset_validator.py
--rw-r--r--   0 runner    (1000) docker    (1001)    13986 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/fiddler/validator.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.125202 fiddler-client-2.0.0.dev6/fiddler_client.egg-info/
--rw-r--r--   0 runner    (1000) docker    (1001)    20044 2023-06-29 07:27:03.000000 fiddler-client-2.0.0.dev6/fiddler_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) docker    (1001)     2073 2023-06-29 07:27:03.000000 fiddler-client-2.0.0.dev6/fiddler_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) docker    (1001)        1 2023-06-29 07:27:03.000000 fiddler-client-2.0.0.dev6/fiddler_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) docker    (1001)      203 2023-06-29 07:27:03.000000 fiddler-client-2.0.0.dev6/fiddler_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) docker    (1001)       14 2023-06-29 07:27:03.000000 fiddler-client-2.0.0.dev6/fiddler_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) docker    (1001)       38 2023-06-29 07:27:03.125202 fiddler-client-2.0.0.dev6/setup.cfg
--rw-r--r--   0 runner    (1000) docker    (1001)     1375 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/setup.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-29 07:27:03.125202 fiddler-client-2.0.0.dev6/tests/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/tests/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2080 2023-06-29 07:26:58.000000 fiddler-client-2.0.0.dev6/tests/test_fiddler_api.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.737257 fiddler-client-2.0.0.dev7/
+-rw-r--r--   0 runner    (1000) docker    (1001)       18 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/MANIFEST.in
+-rw-r--r--   0 runner    (1000) docker    (1001)    20648 2023-07-27 12:35:18.737257 fiddler-client-2.0.0.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1000) docker    (1001)    16868 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/PUBLIC.md
+-rw-r--r--   0 runner    (1000) docker    (1001)     2018 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/README.md
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.729257 fiddler-client-2.0.0.dev7/fiddler/
+-rw-r--r--   0 runner    (1000) docker    (1001)     1725 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)       27 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/_version.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.729257 fiddler-client-2.0.0.dev7/fiddler/assets/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/assets/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     8200 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/assets/pg_reserved_words.py
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/connection.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1822 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/constants.py
+-rw-r--r--   0 runner    (1000) docker    (1001)   112950 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/core_objects.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2490 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/exceptions.py
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/fiddler_api.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.729257 fiddler-client-2.0.0.dev7/fiddler/libs/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/libs/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     6439 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/libs/http_client.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.729257 fiddler-client-2.0.0.dev7/fiddler/packtools/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/packtools/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4167 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/packtools/gem.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     7442 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/packtools/keras_ig_helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    14619 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/packtools/project_attributions_helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     9500 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/packtools/template_model.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.729257 fiddler-client-2.0.0.dev7/fiddler/schemas/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/schemas/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1535 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/schemas/custom_features.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1124 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/schemas/model_schema.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      642 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/schemas/model_spec.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      679 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/schemas/model_task_params.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      313 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/schemas/xai_params.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.729257 fiddler-client-2.0.0.dev7/fiddler/utils/
+-rw-r--r--   0 runner    (1000) docker    (1001)     4399 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/utils/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1006 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/utils/exceptions.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3213 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/utils/formatting.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3084 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/utils/general_checks.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      782 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/utils/helper.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      189 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/utils/logger.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5493 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/utils/pandas_helper.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    13986 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/utils/validator.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.729257 fiddler-client-2.0.0.dev7/fiddler/v2/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/__init__.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.733257 fiddler-client-2.0.0.dev7/fiddler/v2/api/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    16477 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/alert_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4254 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/api.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     9825 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/baseline_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1316 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/compatibility_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    17012 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/dataset_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    22117 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/events_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    15338 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/explainability_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4725 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     9611 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/infer_schema_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4538 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/job_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     8271 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/model_artifact_deploy.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4160 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/model_deployment_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    24244 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/model_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3210 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/api/project_mixin.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.733257 fiddler-client-2.0.0.dev7/fiddler/v2/schema/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/schema/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4630 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/schema/alert.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      346 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/schema/base.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      490 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/schema/baseline.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3048 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/schema/dataset.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      882 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/schema/events.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      157 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/schema/job.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      504 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/schema/model.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1107 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/schema/model_deployment.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      124 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/schema/project.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      364 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/schema/server_info.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      109 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/schema/user.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.733257 fiddler-client-2.0.0.dev7/fiddler/v2/utils/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/utils/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4230 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/utils/compatibility_helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3616 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/utils/decorators.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2564 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/utils/helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1818 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/utils/response_handler.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      362 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/utils/validations.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.733257 fiddler-client-2.0.0.dev7/fiddler/v2/validators/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/validators/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1936 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/fiddler/v2/validators/dataset_validator.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.733257 fiddler-client-2.0.0.dev7/fiddler_client.egg-info/
+-rw-r--r--   0 runner    (1000) docker    (1001)    20648 2023-07-27 12:35:18.000000 fiddler-client-2.0.0.dev7/fiddler_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) docker    (1001)     3036 2023-07-27 12:35:18.000000 fiddler-client-2.0.0.dev7/fiddler_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)        1 2023-07-27 12:35:18.000000 fiddler-client-2.0.0.dev7/fiddler_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)      157 2023-07-27 12:35:18.000000 fiddler-client-2.0.0.dev7/fiddler_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)       14 2023-07-27 12:35:18.000000 fiddler-client-2.0.0.dev7/fiddler_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)       38 2023-07-27 12:35:18.737257 fiddler-client-2.0.0.dev7/setup.cfg
+-rw-r--r--   0 runner    (1000) docker    (1001)     1274 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/setup.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.733257 fiddler-client-2.0.0.dev7/tests/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/__init__.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.733257 fiddler-client-2.0.0.dev7/tests/fiddler/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/fiddler/__init__.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.733257 fiddler-client-2.0.0.dev7/tests/fiddler/utils/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/fiddler/utils/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1473 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/fiddler/utils/test_general_checks.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     8079 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/fiddler/utils/test_pandas.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1800 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/fiddler/utils/tests_utils.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3252 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/test_infer_model_schema.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5346 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/test_object_inference.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      280 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/utils.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:18.737257 fiddler-client-2.0.0.dev7/tests/v2/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1421 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/base.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1785 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/helper.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3793 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_add_model.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    32093 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_alert.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    10273 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_baseline.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      912 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_check_version_decorator.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3028 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_custom_features.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     6301 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_dataset_api.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     7654 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_events_api.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2804 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_exceptions.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    15104 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_explainability_apis.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     7556 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_file_upload.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      826 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4606 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_job.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     7390 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_model.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     6546 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_project.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2964 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_response_handler.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    13744 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_upload_dataset.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      584 2023-07-27 12:35:13.000000 fiddler-client-2.0.0.dev7/tests/v2/test_validations.py
```

### Comparing `fiddler-client-2.0.0.dev6/PKG-INFO` & `fiddler-client-2.0.0.dev7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 2.0.0.dev6
+Version: 2.0.0.dev7
 Summary: Python client for Fiddler Service
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 License: UNKNOWN
 Description: Fiddler Client
         =============
         
@@ -42,15 +42,27 @@
               - unshare_project
               - share_project
               - process_avro
               - process_csv
           - #### **New Features**
             - Add `monitor_components` as an attribute of `CustomFeature`. Default to `False`
             - Remove `column` as a parameter in `add_alert_rule` and `get_alert_rules` functions
-            
+        
+        ### 1.8.2
+          - #### **Modifications**
+            - Fixed a bug where `min` and `max` for columns of type `float` in `dataset_info` are cast into `int` after uploaded
+        
+        ### 1.8.1
+          - #### **Modifications**
+            - Fixed a bug wherein null string was going in request body if body wasn't specified.
+            - Fix `categorical_target_class_details` when passed as an array
+            - Fix a bug where `fdl.ModelInputType.TEXT` were not being accepted properly
+            - Fix `categorical_target_class_details` when passed as an empty list
+        
+        
         ### 1.8.0
           - #### **Modifications**
             - Add new alert type -  `statistic` for setting alerts
             - Add `target_class_order` as a required field of `ModelInfo` object when `model_task` is `MULTICLASS_CLASSIFICATION`,
               `RANKING` or `BINARY_CLASSIFICATION`. Only applies for `BINARY_CLASSIFICATION` when target column is of type `CATEGORY`
             - Add `columns` as a parameter in `add_alert_rule` and `get_alert_rules` functions
             - Add deprecation warning for `column` as a parameter in `add_alert_rule` and `get_alert_rules` functions
```

### Comparing `fiddler-client-2.0.0.dev6/PUBLIC.md` & `fiddler-client-2.0.0.dev7/PUBLIC.md`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,27 @@
       - unshare_project
       - share_project
       - process_avro
       - process_csv
   - #### **New Features**
     - Add `monitor_components` as an attribute of `CustomFeature`. Default to `False`
     - Remove `column` as a parameter in `add_alert_rule` and `get_alert_rules` functions
-    
+
+### 1.8.2
+  - #### **Modifications**
+    - Fixed a bug where `min` and `max` for columns of type `float` in `dataset_info` are cast into `int` after uploaded
+
+### 1.8.1
+  - #### **Modifications**
+    - Fixed a bug wherein null string was going in request body if body wasn't specified.
+    - Fix `categorical_target_class_details` when passed as an array
+    - Fix a bug where `fdl.ModelInputType.TEXT` were not being accepted properly
+    - Fix `categorical_target_class_details` when passed as an empty list
+
+
 ### 1.8.0
   - #### **Modifications**
     - Add new alert type -  `statistic` for setting alerts
     - Add `target_class_order` as a required field of `ModelInfo` object when `model_task` is `MULTICLASS_CLASSIFICATION`,
       `RANKING` or `BINARY_CLASSIFICATION`. Only applies for `BINARY_CLASSIFICATION` when target column is of type `CATEGORY`
     - Add `columns` as a parameter in `add_alert_rule` and `get_alert_rules` functions
     - Add deprecation warning for `column` as a parameter in `add_alert_rule` and `get_alert_rules` functions
```

### Comparing `fiddler-client-2.0.0.dev6/README.md` & `fiddler-client-2.0.0.dev7/README.md`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev6/fiddler/__init__.py` & `fiddler-client-2.0.0.dev7/fiddler/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,86 +5,81 @@
 A Python client for Fiddler service.
 
 TODO: Add Licence.
 """
 
 from fiddler import utils
 from fiddler._version import __version__
-from fiddler.client import Fiddler, PredictionEventBundle
+from fiddler.constants import CSV_EXTENSION
 from fiddler.core_objects import (
     ArtifactStatus,
     BaselineType,
     BatchPublishType,
     Column,
-    CustomFeature,
     DatasetInfo,
     DataType,
     DeploymentType,
     ExplanationMethod,
     FiddlerPublishSchema,
     FiddlerTimestamp,
     ModelInfo,
     ModelInputType,
     ModelTask,
     WeightingParams,
     WindowSize,
 )
-from fiddler.exceptions import NotSupported
-from fiddler.fiddler_api import FiddlerApi as FiddlerApiV1
 from fiddler.packtools import gem
-from fiddler.utils import ColorLogger
-from fiddler.v2.api.api import FiddlerClient
+from fiddler.schemas.custom_features import Multivariate, TextEmbedding
+from fiddler.utils import logger
+from fiddler.utils.validator import (
+    PackageValidator,
+    ValidationChainSettings,
+    ValidationModule,
+)
+from fiddler.v2.api.api import FiddlerApi, FiddlerClient
 from fiddler.v2.api.explainability_mixin import (
     DatasetDataSource,
     RowDataSource,
     SqlSliceQueryDataSource,
 )
-from fiddler.v2.constants import CSV_EXTENSION, FileType
 from fiddler.v2.schema.alert import (
     AlertCondition,
     AlertType,
     BinSize,
     ComparePeriod,
     CompareTo,
     Metric,
     Priority,
 )
-from fiddler.v2.schema.job import JobStatus
-from fiddler.v2.schema.model_deployment import DeploymentParams, ModelDeployment
-from fiddler.v2.utils.helpers import match_semver, raise_not_supported
-from fiddler.validator import (
-    PackageValidator,
-    ValidationChainSettings,
-    ValidationModule,
-)
 
-logger = utils.logging.getLogger(__name__)
+logger = logger.get_logger(__name__)
 
 SUPPORTED_API_VERSIONS = ['v2']
 
 
 __all__ = [
     '__version__',
     'BatchPublishType',
     'Column',
-    'CustomFeature',
+    'Multivariate',
+    'TextEmbedding',
+    'ImageEmbedding',
     'ColorLogger',
     'DatasetInfo',
     'DataType',
-    'Fiddler',
     'FiddlerClient',
+    'FiddlerApi',
     'FiddlerTimestamp',
     'FiddlerPublishSchema',
     'gem',
     'ModelInfo',
     'ModelInputType',
     'ModelTask',
     'WeightingParams',
     'ExplanationMethod',
-    'PredictionEventBundle',
     'PackageValidator',
     'ValidationChainSettings',
     'ValidationModule',
     'utils',
     # Exposing constants
     'CSV_EXTENSION',
 ]
```

### Comparing `fiddler-client-2.0.0.dev6/fiddler/assets/pg_reserved_words.py` & `fiddler-client-2.0.0.dev7/fiddler/assets/pg_reserved_words.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev6/fiddler/core_objects.py` & `fiddler-client-2.0.0.dev7/fiddler/core_objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # TODO: Add License
 
 import copy
 import enum
 import functools
 import json
-import logging
 import textwrap
 import warnings
 from dataclasses import asdict, dataclass
 from typing import (
     Any,
     Dict,
     Iterable,
@@ -21,38 +20,35 @@
     cast,
 )
 
 import numpy as np
 import pandas as pd
 import pandas.api.types
 
-from fiddler._version import __version__
-from fiddler.utils.exceptions import MalformedSchemaException
+from fiddler.schemas.custom_features import CustomFeature
 from fiddler.utils.formatting import prettyprint_number, validate_sanitized_names
-from fiddler.utils.general_checks import type_enforce
-from fiddler.utils.pandas import is_datetime
+from fiddler.utils.logger import get_logger
+from fiddler.utils.pandas_helper import is_datetime, is_list, is_vector_value
 
-MAX_VECTOR_DIMENSION = 1024
-MAX_NUMBER_OF_CLUSTERS = 100
-MAX_NUMBER_OF_CUSTOM_FEATURES = 100
 DEFAULT_MAX_INFERRED_CARDINALITY = 100
+PD_TYPE_VECTOR = 'vector'
 
 # default for DatasetInfo.data_type_version and ModelInfo.data_type_version
 # Introduced to bypass certain data type conversion functions
 # from both client and server.
 # More details https://fiddlerlabs.atlassian.net/wiki/spaces/FL/pages/1973617158/Introducing+Version+in+DatasetInfo+and+ModelInfo
 
 # v0 means variable is just defined, no change in any logic.
 # v0 is launched in python-client release 1.7.0
 
 # v1 ignores typecasting of possible_values of categorical data type
 # v1 is launched in python-client release 2.0.0
 CURRENT_DATA_TYPE_VERSION: str = 'v1'
 
-LOG = logging.getLogger(__name__)
+LOG = get_logger(__name__)
 
 
 class IntegrityViolationStatus(NamedTuple):
     is_nullable_violation: bool
     is_type_violation: bool
     is_range_violation: bool
 
@@ -154,34 +150,27 @@
 
     FLOAT = 'float'
     INTEGER = 'int'
     BOOLEAN = 'bool'
     STRING = 'str'
     CATEGORY = 'category'
     TIMESTAMP = 'timestamp'
+    VECTOR = 'vector'
 
     def is_numeric(self):
         return self.value in (DataType.INTEGER.value, DataType.FLOAT.value)
 
     def is_bool_or_cat(self):
         return self.value in (DataType.BOOLEAN.value, DataType.CATEGORY.value)
 
     def is_valid_target(self):
         return self.value != DataType.STRING.value
 
-
-@enum.unique
-class CustomFeatureType(str, enum.Enum):
-    """The types of custom features based on how they are created."""
-
-    FROM_COLUMNS = 'FROM_COLUMNS'
-    # The following types will be added in later versions
-    # FROM_TEXT = 'FROM_TEXT'
-    # FROM_VECTOR = 'FROM_VECTOR'
-    # FROM_DICTIONARY = 'FROM_DICTIONARY'
+    def is_vector(self):
+        return self.value == DataType.VECTOR.value
 
 
 @enum.unique
 class ArtifactStatus(enum.Enum):
     """Artifact Status, default to USER_UPLOADED"""
 
     NO_MODEL = 'no_model'
@@ -338,153 +327,14 @@
             explanations={
                 label_class: AttributionExplanation.from_dict(explanation_dict)
                 for label_class, explanation_dict in deserialized_json.items()
             },
         )
 
 
-@dataclass
-class CustomFeature:
-    """A class used to define custom features such as complex/vector features
-
-    :param name: The name of the custom feature as it will appear in the monitoring tab.
-    :param columns: The name of the data column(s) that constitute the custom feature.
-    :param transformation: The transformation method applied on the original data.
-    :param n_clusters: The number of clusters used for creating clustering-based histograms.
-                       If not specified a preprocessing step will run to choose the number of clusters automatically.
-    :param monitor: A boolean variable that specifies whether this custom feature will
-        be monitored using the clustering-based histogram binning.
-    :param monitor_components: A boolean variable that specifies whether each individual
-        component of this custom feature will be monitored. Default to False
-    """
-
-    name: str
-    columns: Union[str, List[str]]
-    type: CustomFeatureType
-    transformation: Optional[str] = None
-    n_clusters: Optional[int] = None
-    monitor: bool = True
-    monitor_components: bool = False
-
-    def __post_init__(self):
-        if self.n_clusters is not None and not isinstance(self.n_clusters, int):
-            raise TypeError(
-                f'n_clusters argument must be of type int but received {type(self.n_clusters)}.'
-            )
-
-    def to_dict(self) -> Dict[str, Any]:
-        """Converts this object to a more JSON-friendly form."""
-        res = {
-            'name': self.name,
-            'columns': self.columns,
-            'type': self.type.value,
-            'transformation': self.transformation,
-            'n_clusters': self.n_clusters,
-            'monitor': self.monitor,
-            'monitor_components': getattr(self, 'monitor_components', False),
-        }
-        return res
-
-    @classmethod
-    def from_dict(cls, desrialized_json: dict):
-        """Creates a CustomFeature object from deserialized JSON"""
-        return cls(
-            name=desrialized_json['name'],
-            columns=desrialized_json['columns'],
-            type=CustomFeatureType(desrialized_json['type']),
-            transformation=desrialized_json['transformation'],
-            n_clusters=desrialized_json['n_clusters'],
-            monitor=desrialized_json['monitor'],
-            monitor_components=bool(desrialized_json.get('monitor_components', False)),
-        )
-
-    @classmethod
-    def from_columns(
-        cls,
-        cols: List[str],
-        custom_name: str,
-        transformation: Optional[str] = None,
-        n_clusters: Optional[int] = 10,
-        monitor: bool = True,
-        monitor_components: bool = False,
-    ):
-        """Creates a custom feature from multiple numerical columns.
-        :param cols: A list of column names that define this custom feature.
-        :param custom_name: The name of this custom feature as it will appear in the monitoring tab.
-        :param transformation: [Optional] An optional transformation step (eg, dimensionality reduction via SVD).
-        :param n_clusters: [Optional] Number of clusters for clustering-based monitoring.
-        :param monitor:A boolean variable that specifies whether this custom feature will be monitored using the
-                            clustering-based histogram binning.
-        :param monitor_components: A boolean variable that specifies whether each
-        individual component of this custom feature will be monitored. Default to False
-        """
-        if not isinstance(custom_name, str):
-            raise TypeError(
-                f'custom_name argument must be of type str but received {type(custom_name)}'
-            )
-
-        if not (isinstance(cols, list) and all(isinstance(col, str) for col in cols)):
-            raise TypeError(
-                f'cols argument accepts a list of column names, passed {cols}.'
-            )
-
-        if len(cols) > MAX_VECTOR_DIMENSION:
-            raise ValueError(
-                f'The maximum acceptable dimension for a custom feature is {MAX_VECTOR_DIMENSION}, {len(cols)} columns are passed to cols.'
-            )
-
-        if n_clusters and n_clusters > MAX_NUMBER_OF_CLUSTERS:
-            raise ValueError(
-                f'The number of clusters should not exceed {MAX_NUMBER_OF_CLUSTERS}.'
-            )
-
-        return cls(
-            name=custom_name,
-            columns=cols,
-            type=CustomFeatureType.FROM_COLUMNS,
-            transformation=transformation,
-            n_clusters=n_clusters,
-            monitor=monitor,
-            monitor_components=monitor_components,
-        )
-
-    # ToDo: This class method will be added later. For the first version we only use from_columns constructor
-    # @classmethod
-    # def from_text(cls,
-    #               text_col: str,
-    #               transformation: str,
-    #               custom_name: Optional[str] = None,
-    #               n_clusters: Optional[int] = None,
-    #               monitor: bool = True,
-    #               monitor_components = False,
-    #               ):
-    #     """Creates a custom feature from a single text column.
-    #     :param text_col: The name of the dataset column that contains text data.
-    #     :param transformation: The transformation used to convert text data to numerical vectors.
-    #     :param custom_name: [Optional] A new name assigned to this custom feature. If not specified, the name of the text column will be used.
-    #     :param n_clusters: [Optional] Number of clusters for clustering-based monitoring.
-    #     :param monitor:A boolean variable that specifies whether this custom feature will be monitored using the
-    #                         clustering-based histogram binning.
-    #     """
-    #     if not isinstance(text_col, str):
-    #         raise TypeError(f"The first argument specifies the column that contains text data."
-    #                         f" It accepts a string but received {type(text_col)}.")
-    #     if custom_name and not isinstance(custom_name, str):
-    #         raise TypeError(f"custom_name argument must be of type 'str' but received {type(custom_name)}")
-    #
-    #     custom_feature_name = custom_name if custom_name else text_col
-    #     return cls(name=custom_feature_name,
-    #                columns=text_col,
-    #                type=CustomFeatureType.FROM_TEXT,
-    #                transformation=transformation,
-    #                n_clusters=n_clusters,
-    #                monitor=monitor,
-    #                monitor_components=monitor_components)
-
-
 class Column:
     """Represents a single column of a dataset or model input/output.
 
     :param name: The name of the column (corresponds to the header row of a
         CSV file)
     :param data_type: The best encoding type for this column's data.
     :param possible_values: If data_type is CATEGORY, then an exhaustive list
@@ -501,21 +351,24 @@
         self,
         name: str,
         data_type: DataType,
         possible_values: Optional[List[Any]] = None,
         is_nullable: Optional[bool] = None,
         value_range_min: Optional[Union[int, float]] = None,
         value_range_max: Optional[Union[int, float]] = None,
+        n_dimensions: Optional[int] = None,
     ):
         self.name = name
         self.data_type = data_type
-        self.possible_values = possible_values
         self.is_nullable = is_nullable
+
+        self.possible_values = possible_values
         self.value_range_min = value_range_min
         self.value_range_max = value_range_max
+        self.n_dimensions = n_dimensions
 
         inappropriate_value_range = not self.data_type.is_numeric() and not (
             self.value_range_min is None and self.value_range_max is None
         )
         if inappropriate_value_range:
             raise ValueError(
                 f'Do not pass `value_range` for '
@@ -528,14 +381,15 @@
         return cls(
             name=desrialized_json['column-name'],
             data_type=DataType(desrialized_json['data-type']),
             possible_values=desrialized_json.get('possible-values', None),
             is_nullable=desrialized_json.get('is-nullable', None),
             value_range_min=desrialized_json.get('value-range-min', None),
             value_range_max=desrialized_json.get('value-range-max', None),
+            n_dimensions=desrialized_json.get('n-dimensions', None),
         )
 
     def copy(self):
         return copy.deepcopy(self)
 
     def __repr__(self):
         res = (
@@ -545,14 +399,16 @@
         if self.is_nullable is not None:
             res += f', is_nullable={self.is_nullable}'
         if self.value_range_min is not None or self.value_range_max is not None:
             res += (
                 f', value_range_min={self.value_range_min}'
                 f', value_range_max={self.value_range_max}'
             )
+        if self.n_dimensions is not None:
+            res += f', n_dimensions={self.n_dimensions}'
         res += ')'
         return res
 
     def _raise_on_bad_categorical(self):
         """Raises a ValueError if data_type=CATEGORY without possible_values"""
         if (
             self.data_type.value == DataType.CATEGORY.value
@@ -586,17 +442,18 @@
             res['possible-values'] = [val for val in self.possible_values]
         if self.is_nullable is not None:
             res['is-nullable'] = self.is_nullable
         if self.value_range_min is not None:
             res['value-range-min'] = self.value_range_min
         if self.value_range_max is not None:
             res['value-range-max'] = self.value_range_max
+        if self.n_dimensions is not None:
+            res['n-dimensions'] = self.n_dimensions
         return res
 
-
     @staticmethod
     def _value_is_na_or_none(value):
         if value is None:
             return True
         # This needs to be added because when we add `pandas._libs.missing.NAType` type in rabbitmq.
         # When we read the message, it converts the value to the "<NA>".
         if isinstance(value, str):
@@ -741,14 +598,16 @@
             return DataType.FLOAT
         if pd.api.types.is_integer_dtype(pd_dtype):
             return DataType.INTEGER
         if pd.api.types.is_bool_dtype(pd_dtype):
             return DataType.BOOLEAN
         if pd.api.types.is_categorical_dtype(pd_dtype):
             return DataType.CATEGORY
+        if pd_dtype == PD_TYPE_VECTOR:
+            return DataType.VECTOR
 
         return DataType.STRING
 
     @classmethod
     def update_stats_for_existing_schema(
         cls, dataset: dict, info, max_inferred_cardinality: Optional[int] = None
     ):
@@ -856,47 +715,60 @@
             df = df.reset_index(inplace=False)
         name_series_iter = df.items()
         for column_name, column_series in name_series_iter:
             column_info = cls._calculate_stats_for_col(
                 column_name,
                 column_series,
                 max_inferred_cardinality,
-                data_type_version=CURRENT_DATA_TYPE_VERSION
+                data_type_version=CURRENT_DATA_TYPE_VERSION,
             )
             columns.append(column_info)
         return cls(
             display_name,
             columns,
             dataset_id=dataset_id,
             data_type_version=CURRENT_DATA_TYPE_VERSION,
         )
 
     @staticmethod
     def _calculate_stats_for_col(
         column_name,
         column_series,
         max_inferred_cardinality,
-        data_type_version:Optional[str]='v0'):
+        data_type_version: Optional[str] = 'v0',
+    ):
         # @TODO Automatically drop the empty column with warning and proceed instead of aborting the upload
         if column_series.isna().all():
             raise ValueError(
                 f'Column {column_name} is empty. '
                 f'Please remove it and re-upload the dataset.'
             )
 
         # if we infer string or categorical, ensure that the underlying data
         # is also string by casting it.
 
         # FDL-10905: dropna is needed to take care of cases where having None changes
         # data type of int, float, bool to category. dropna() won't change
         # is_nullable detection as column_series.dropna() returns a new instance.
+
         column_series_dropped_na = column_series.dropna()
-        column_dtype = DatasetInfo.datatype_from_pandas_dtype(
-            column_series_dropped_na.infer_objects().dtype
-        )
+        pd_column_dtype = column_series_dropped_na.infer_objects().dtype
+        if pd.api.types.is_object_dtype(pd_column_dtype):
+            row_count = column_series_dropped_na.shape[0]
+            if row_count > 0 and is_vector_value(column_series_dropped_na[0]):
+                iteration_count = min(row_count, 100)
+
+                for i in range(iteration_count):
+                    if not is_vector_value(column_series_dropped_na[i]):
+                        break
+
+                if i == iteration_count - 1:
+                    pd_column_dtype = PD_TYPE_VECTOR
+
+        column_dtype = DatasetInfo.datatype_from_pandas_dtype(pd_column_dtype)
         # get nullability before any datatype modifications like 'astype'
         # which distorts None values.
         is_nullable = bool(column_series.isna().any())
 
         if column_dtype in [DataType.CATEGORY, DataType.STRING]:
             if 'mixed' in pd.api.types.infer_dtype(column_series):
                 LOG.warning(
@@ -907,24 +779,27 @@
                 )
 
         # infer categorical if configured to do so
         if (
             max_inferred_cardinality
             and column_dtype.value == DataType.STRING.value
             and not is_datetime(column_series)
+            and not is_list(column_series)
             and column_series_dropped_na.nunique() <= max_inferred_cardinality
         ):
             column_dtype = DataType.CATEGORY
 
         # get possible values for categorical type
         if column_dtype.is_bool_or_cat():
             # Only when data_type_version is 'v0',
             # categorical column values undergo int/bool -> float -> string conversion.
             if data_type_version == 'v0':
-                possible_values = np.sort(column_series_dropped_na.astype(str).unique()).tolist()
+                possible_values = np.sort(
+                    column_series_dropped_na.astype(str).unique()
+                ).tolist()
                 possible_values_floats = None
                 if column_dtype.value == DataType.CATEGORY.value:
                     try:
                         possible_values_floats = [
                             str(float(raw_val)) for raw_val in possible_values
                         ]
                     except ValueError:
@@ -943,21 +818,30 @@
             if np.isnan(value_min):
                 value_min = None
             if np.isnan(value_max):
                 value_max = None
         else:
             value_min, value_max = None, None
 
+        # get n_dimensions for vector dtype
+        if column_dtype == DataType.VECTOR:
+
+            # pick the most common length of the vector
+            n_dimensions = int(column_series_dropped_na.apply(len).mode()[0])
+        else:
+            n_dimensions = None
+
         return Column(
             name=column_name,
             data_type=column_dtype,
             possible_values=possible_values,
             is_nullable=is_nullable,
             value_range_min=value_min,
             value_range_max=value_max,
+            n_dimensions=n_dimensions,
         )
 
     def to_dict(self) -> Dict[str, Any]:
         """Converts this object to a more JSON-friendly form."""
         res = {
             'name': self.display_name,
             'data_type_version': self.data_type_version,
@@ -1172,15 +1056,15 @@
      to be group by with for performance metrics computation. This have to be given for Ranking for MAP
       and NDCG computations. For ranking models, it represents the query/session id column.
     :param missing_value_encodings(fall_back): [Optional] A dictionary of list representing the values that should be
            replaced with null for each columns. Key is the column name.
     :param tree_shap_enabled: [Optional] Boolean value indicating if Tree SHAP should be enabled for this model.
            If set to True, Tree SHAP will become the default explanation method unless you specify another
            preferred explanation method.
-    :param custom_features: [Optional] A list of custom features that are instances of CustomFeature class.
+    :param custom_features: [Optional] A list of custom features.
     :param data_type_version: [Optional] a String indicating 'v0', 'v1' etc. Used mainly to apply data type conversion rules.
     :param **kwargs: Additional information about the model to store as `misc`.
     """
 
     def __init__(
         self,
         display_name: str,
@@ -1234,15 +1118,16 @@
         self.data_type_version = data_type_version
 
         self.is_binary_ranking_model = is_binary_ranking_model
 
         self._validate_columns()
 
         self.target_class_order = self.get_target_class_order(
-            self.target_class_order, self.model_task, self.targets[0])
+            self.target_class_order, self.model_task, self.targets[0]
+        )
 
         if model_task == ModelTask.RANKING:
             if group_by is None:
                 raise ValueError(
                     'The argument group_by cannot be empty for Ranking models'
                 )
             self.is_binary_ranking_model = len(self.target_class_order) == 2
@@ -1330,29 +1215,30 @@
         self.fall_back = self.missing_value_encodings  # backward compatability
 
         if self.custom_features is not None:
             if not isinstance(self.custom_features, List):
                 raise ValueError(
                     'The custom_features argument only accepts a list of CustomFeature objects.'
                 )
-            if len(self.custom_features) > MAX_NUMBER_OF_CUSTOM_FEATURES:
-                raise ValueError(
-                    f'The maximum number of custom features in a project cannot exceed {MAX_NUMBER_OF_CUSTOM_FEATURES}. {len(self.custom_features)} custom features are defined.'
-                )
 
             available_cols = (
-                self.get_input_names() + self.get_target_names() + self.get_metadata_names()
+                self.get_input_names()
+                + self.get_target_names()
+                + self.get_metadata_names()
             )
             numeric_cols = self.get_input_pandas_dtypes()
             if self.metadata:
                 numeric_cols.update(self.get_metadata_pandas_dtypes())
             if self.targets:
                 numeric_cols.update(self.get_target_pandas_dtypes())
-            valid_col_names = [k for k, v in numeric_cols.items() if
-                               v in (DataType.INTEGER.value, DataType.FLOAT.value)]
+            valid_col_names = [
+                k
+                for k, v in numeric_cols.items()
+                if v in (DataType.INTEGER.value, DataType.FLOAT.value)
+            ]
 
             unique_cf_names = []
             for feature in self.custom_features:
 
                 if not isinstance(feature, CustomFeature):
                     raise ValueError(
                         'The custom_features argument only accepts a list of CustomFeature objects.'
@@ -1393,15 +1279,15 @@
         res = {
             'name': self.display_name,
             'input-type': self.input_type.value,
             'model-task': self.model_task.value,
             'inputs': [c.to_dict() for c in self.inputs],
             'outputs': [c.to_dict() for c in self.outputs],
             'datasets': self.datasets or [],
-            'targets': [target_col.to_dict() for target_col in self.targets]
+            'targets': [target_col.to_dict() for target_col in self.targets],
         }
         if self.target_class_order is not None:
             res['target-class-order'] = self.target_class_order
         if self.metadata:
             res['metadata'] = [metadata_col.to_dict() for metadata_col in self.metadata]
         if self.decisions:
             res['decisions'] = [
@@ -1892,16 +1778,16 @@
         :param custom_features: [Optional] A list of custom features that are instances of CustomFeature class.
 
         :returns A ModelInfo object.
         """
         if categorical_target_class_details is not None:
             warnings.warn(
                 'WARNING: categorical_target_class_details is deprecated in 1.7 and '
-                'will be removed from 2.0.0 version. As a replacement, use target_class'
-                '_order while constructing ModelInfo.',
+                'will be removed from 2.0.0 version. categorical_target_class_details '
+                'will be replaced by target_class_order in 2.0.0',
                 DeprecationWarning,
             )
 
         if custom_explanation_names is None:
             custom_explanation_names = []
 
         if not isinstance(dataset_info, DatasetInfo):
@@ -1959,21 +1845,14 @@
         cls.validate_model_task(
             model_task=model_task,
             target_column=target_column,
             output_names=output_names,
         )
 
         target_class_order = None
-        if categorical_target_class_details is not None:
-            warnings.warn(
-                'WARNING: categorical_target_class_details is deprecated in 1.7 and '
-                'will be removed from 2.0.0 version. As a replacement, use target_class'
-                '_order while constructing ModelInfo.',
-                DeprecationWarning,
-            )
         if target_column:
             target_class_order = cls.get_target_class_order(
                 model_task=model_task,
                 target_column=target_column,
                 target_class_order=categorical_target_class_details,
             )
 
@@ -2152,24 +2031,24 @@
                 for class_name in target_class_order
             ]
         # For regression and ranking
         return [f'predicted_{target_column.name}']
 
     @classmethod
     def check_input_type(cls, input_type: ModelInputType, inputs: List[Column]) -> None:
-        if input_type.value == ModelInputType.TEXT.value:
+        if input_type == ModelInputType.TEXT:
             if len(inputs) != 1:
                 raise ValueError(
                     f'Text models may only contain a single feature column containing '
                     f'text data. Please remove any other non-text features from the '
                     f'features argument if you wish to add a text model. You can add '
                     f'other columns as metadata columns. If your model has multiple '
                     f'inputs please specify the input_type to {ModelInputType.TABULAR}.'
                 )
-            if inputs[0].data_type.value != DataType.STRING:
+            if inputs[0].data_type != DataType.STRING:
                 raise ValueError(
                     'Text features must be of type STRING. Please double check the '
                     'data type of the feature column passed into the '
                     'features argument.'
                 )
 
     @classmethod
@@ -2230,15 +2109,15 @@
         dataset_info: DatasetInfo,
         features: Optional[List[str]],
         metadata_cols: Optional[List[str]],
         decision_cols: Optional[List[str]],
         additional_cols: List[str],
         target: str,
         outputs: Optional[Union[List[str], Dict[str, Union[int, float]]]],
-    ) -> (List[Column], Optional[List[Column]], Optional[List[Column]]):
+    ) -> Tuple[List[Column], Optional[List[Column]], Optional[List[Column]]]:
 
         inputs: List[Column] = []
         metadata: Optional[List[Column]] = None
         decisions: Optional[List[Column]] = None
 
         if metadata_cols:
             metadata = []
@@ -2275,15 +2154,14 @@
             return None
 
         output_columns = []
         ds_info_names_columns = {}
         for ds_column in dataset_info.columns:
             ds_info_names_columns[ds_column.name] = ds_column
 
-
         if model_task.is_classification():
             if isinstance(output_names, dict):
                 output_names = list(output_names.keys())
             for name in output_names:
                 if name in ds_info_names_columns:
                     output_columns.append(ds_info_names_columns[name])
                 else:
@@ -2305,15 +2183,18 @@
                     raise ValueError(
                         f'If outputs is a dictionary, the values should '
                         f'be a tuple of 2 values. Currently passing: '
                         f'{values} for output {name}. Please correct.'
                     )
                 if name in ds_info_names_columns:
                     column = ds_info_names_columns[name]
-                    if not (column.data_type == DataType.FLOAT or column.data_type == DataType.INTEGER):
+                    if not (
+                        column.data_type == DataType.FLOAT
+                        or column.data_type == DataType.INTEGER
+                    ):
                         raise ValueError(
                             f'Column {name} with type {column.data_type} can not be specified as output.'
                             f'Output column type has to be either INTEGER or FLOAT.'
                             f'Please correct.'
                         )
                     column.value_range_min = min(values)
                     column.value_range_max = max(values)
@@ -2339,15 +2220,18 @@
                         col = target_column.name
                     else:
                         raise ValueError(
                             f'Output {name} is not present in the dataset. '
                             f'Please provide a dictionary with the range: '
                             f'{name}: (min_value, max_value).'
                         )
-                if dataset_info[col].value_range_min is None or dataset_info[col].value_range_max is None:
+                if (
+                    dataset_info[col].value_range_min is None
+                    or dataset_info[col].value_range_max is None
+                ):
                     raise ValueError(
                         f'Column {name} with value_range_min or value_range_max as None can not be specified as output.'
                         f'Please correct.'
                     )
                 output_columns.append(
                     Column(
                         name=name,
@@ -2364,15 +2248,15 @@
     @classmethod
     def get_model_parameters(
         cls,
         model_task: ModelTask,
         target_column: Optional[Column],
         ranking_top_k: Optional[int],
         binary_classification_threshold: Optional[float],
-    ) -> (Optional[bool], Optional[int], Optional[float]):
+    ) -> Tuple[Optional[bool], Optional[int], Optional[float]]:
 
         is_binary_ranking_model = None
         top_k = None
         bin_class_threshold = None
 
         if model_task.value == ModelTask.RANKING.value:
             if ranking_top_k and not isinstance(ranking_top_k, int):
@@ -2517,25 +2401,29 @@
         model_task: ModelTask,
         target_column: Column,
     ) -> Optional[List[Union[str, bool, float, int]]]:
 
         if model_task.value == ModelTask.REGRESSION.value:
             return None
 
-        if not target_class_order:
-            return cls._infer_target_class_order(target_column, model_task)
-
         if isinstance(target_class_order, (str, int, float, bool)):
             target_class_order = [target_class_order]
 
-        if not isinstance(target_class_order, list):
+        if isinstance(target_class_order, np.ndarray):
+            target_class_order = target_class_order.tolist()
+
+        if target_class_order and not isinstance(target_class_order, list):
             raise ValueError(
                 'Target-class-order(categorical_target_class_details) cannot be of type '
                 f'{type(target_class_order)}'
             )
+
+        if not target_class_order:
+            return cls._infer_target_class_order(target_column, model_task)
+
         for value in target_class_order:
             if not isinstance(value, (str, int, float, bool)):
                 raise ValueError(
                     'Value in Target-class-order(categorical_target_class_details) '
                     f'cannot be of type {type(value)}. Please input strings, floats, '
                     f'integers, or booleans. '
                 )
@@ -2781,236 +2669,14 @@
 
 CURRENT_SCHEMA_VERSION = 0.1
 DEFUNCT_MODELINFO_SCHEMA_VERSION = '0.0'
 CURRENT_MODELINFO_SCHEMA_VERSION = '1.2'
 VALID_OPERATORS = ['==', '>=', '<=', '>', '<']
 
 
-class SegmentInfo:
-    def __init__(
-        self,
-        project_id,
-        model_id,
-        segment_id,
-        filter=None,
-        subsegments=None,
-        metrics=None,
-        description='',
-    ):
-        """
-        schema-version 0.1
-        """
-        type_enforce('project_id', project_id, str)
-        type_enforce('model_id', model_id, str)
-        type_enforce('segment_id', segment_id, str)
-        self.schema_version = CURRENT_SCHEMA_VERSION
-        self.creator_version = f'FIDDLER-CLIENT-v{__version__}'
-        self.project = project_id
-        self.model = model_id
-        # self.dataset = ''
-        self.segment_id = segment_id
-        self.description = description
-        if filter is None:
-            self.filter = ''
-        else:
-            self.filter = filter
-        if subsegments is None:
-            self.subsegments = {}
-        else:
-            self.subsegments = subsegments
-        if metrics is None:
-            self.metrics = []
-        else:
-            raise MalformedSchemaException(
-                f'Segment specific metrics have not yet been implemented (schema-version {CURRENT_SCHEMA_VERSION}).'
-            )
-            self.metrics = metrics
-
-    def get_filter(self):
-        """
-        schema-version 0.1
-        """
-        # by default, every event should pass through the filter:
-        result = 'True'
-        for feature, operator, value in self.filter:
-            if operator == '==':
-                result += f' & (Eq({feature}, {value}))'
-            else:
-                result += f' & ({feature} {operator} {value})'
-        return result
-
-    def get_subsegments(self):
-        """
-        schema-version 0.1
-        """
-        return self.subsegments
-
-    def get_metrics(self):
-        """
-        schema-version 0.1
-        """
-        return self.metrics
-
-    def to_dict(self) -> Dict:
-        """
-        Serialize object to a JSON-friendly dict.
-
-        This implementation works for schema-version 0.1
-        """
-        return self.__dict__
-        # TODO: bulletproofing
-
-    @classmethod
-    def from_dict(cls, deserialized_json: dict):
-        """
-        Transform deserialized JSON-friendly dict into a SegmentInfo object.
-
-        This implementation works for schema-version 0.1
-        """
-        seg_info = cls(
-            project_id=deserialized_json['project'],
-            model_id=deserialized_json['model'],
-            segment_id=deserialized_json['segment_id'],
-            filter=deserialized_json['filter'],
-            subsegments=deserialized_json['subsegments'],
-            description=deserialized_json['description'],
-        )
-        seg_info.schema_version = deserialized_json['schema_version']
-        seg_info.creator_version = deserialized_json['creator_version']
-        seg_info.metrics = deserialized_json['metrics']
-        return seg_info
-        # TODO: bulletproofing to check additional keys don't exist
-
-    def validate(self, model_info):
-        """
-        Ensure that filters, subsegments, metrics, etc conform to schema-version 0.1.
-        """
-        result = True
-        if len(self.filter) == 0 and len(self.subsegments) == 0:
-            raise MalformedSchemaException(
-                'Both filter and subsegments are missing from SegmentInfo - please specify at least one.'
-            )
-        result = result and self._validate_filter_format(model_info)
-        result = result and self._validate_subsegments_format(model_info)
-        result = result and self._validate_metrics_format(model_info)
-        return result
-
-    def _validate_filter_format(self, model_info):
-        """
-        Validate filters according to schema-version 0.1.
-        """
-        for filter in self.filter:
-            if len(filter) != 3:
-                raise MalformedSchemaException(
-                    f'Could not parse filters, is {filter} a 3-tuple?'
-                )
-            feature, operator, value = filter
-            if operator not in VALID_OPERATORS:
-                raise MalformedSchemaException(
-                    f'Could not parse operator in {filter}, please ensure the middle element is from {VALID_OPERATORS}.'
-                )
-            col = model_info.get_col(feature)
-            if col in model_info.targets:  # disallow targets
-                raise MalformedSchemaException(
-                    f'Cannot include target {col.name} in segment definition.'
-                )
-            if col is None:
-                raise MalformedSchemaException(
-                    f'Could not find column {feature} in the ModelInfo.'
-                )
-            if col.possible_values is not None:
-                if operator != '==':
-                    raise MalformedSchemaException(
-                        f'Only == operation is supported ({operator} is unsupported) for non-numeric features like {feature}.'
-                    )
-                if value not in col.possible_values:
-                    raise MalformedSchemaException(
-                        f'Feature {feature} can never take value {value} according to the ModelInfo.'
-                    )
-            else:
-                if value < col.value_range_min or value > col.value_range_max:
-                    raise MalformedSchemaException(
-                        f'Segment value {value} is defined beyond the permitted value range for feature {feature}: [{col.value_range_min}, {col.value_range_max}].'
-                    )
-        return True
-
-    def _validate_subsegments_format(self, model_info):
-        """
-        Validate subsegments according to schema-version 0.1.
-        """
-        for feature in self.subsegments:
-            col = model_info.get_col(feature)
-            if col in model_info.targets:  # disallow targets
-                raise MalformedSchemaException(
-                    f'Cannot include target {col.name} in segment definition.'
-                )
-            if col is None:
-                raise MalformedSchemaException(
-                    f'Could not find column {feature} in the ModelInfo.'
-                )
-            if col.possible_values is not None:
-                for value in self.subsegments[feature]:
-                    if value not in col.possible_values:
-                        raise MalformedSchemaException(
-                            f'Could not find group-by value {value} in {feature}.possible_values'
-                        )
-            else:
-                min, max = float('inf'), float('-inf')
-                curr = self.subsegments[feature][0] - 1
-                for value in self.subsegments[feature]:
-                    if value <= curr:
-                        raise MalformedSchemaException(
-                            f'Group-by for {feature} should be monotonically non-decreasing.'
-                        )
-                    if value < min:
-                        min = value
-                    if value > max:
-                        max = value
-                    curr = value
-                if min < col.value_range_min:
-                    raise MalformedSchemaException(
-                        f'Group-by for {feature} has min value < min value from ModelInfo.'
-                    )
-                if max > col.value_range_max:
-                    raise MalformedSchemaException(
-                        f'Group-by for {feature} has max value < max value from ModelInfo.'
-                    )
-        return True
-
-    def _validate_metrics_format(self, model_info):
-        """
-        Validate metrics according to schema-version 0.1.
-        """
-        if len(self.metrics) != 0:
-            raise MalformedSchemaException(
-                f'SegmentInfo cannot yet specify metrics (schema-version {CURRENT_SCHEMA_VERSION}).'
-            )
-        else:
-            return True
-        # TODO: allow generic metrics like traffic count, etc
-        valid_metrics = []
-        # ToDo: add ranking
-        if model_info.model_task == ModelTask.BINARY_CLASSIFICATION:
-            valid_metrics += [m.value for m in BuiltInMetrics.get_binary()]
-        elif model_info.model_task == ModelTask.MULTICLASS_CLASSIFICATION:
-            valid_metrics += [m.value for m in BuiltInMetrics.get_multiclass()]
-        elif model_info.model_task == ModelTask.REGRESSION:
-            valid_metrics += [m.value for m in BuiltInMetrics.get_regression()]
-        else:
-            raise MalformedSchemaException(
-                f'ModelInfo has an invalid model_task: {model_info.model_task}, for which there is no segment support.'
-            )
-        for metric in self.metrics:
-            if metric not in valid_metrics:
-                raise MalformedSchemaException(
-                    f'Unknown metric {metric} for specified model_task {model_info.model_task}.'
-                )
-        return True
-
-
 def _summary_dataframe_for_columns(
     columns: Sequence[Column], placeholder=''
 ) -> pd.DataFrame:
     """
         Example:
                  column     dtype count(possible_values) is_nullable            value_range
     0       CreditScore   INTEGER                              False        376 - 850
@@ -3085,40 +2751,38 @@
     1   F2      ['col_name2','col_name3']   FROM_COLUMNS        None            4           True        False
     2   F3      'col_name4'                 FROM_VECTOR         None            auto        True        False
     3   F4      'col_name5'                 FROM_DICTIONARY     None            auto        True        False
     """  # noqa E501
     names = []
     columns = []
     types = []
-    transformations = []
     clusters = []
-    monitors = []
-    monitor_components = []
+    source_columns = []
+    embeddings = []
 
     for feature in custom_features:
         names.append(feature.name)
-        columns.append(feature.columns)
         types.append(feature.type.name)
-        transformations.append(feature.transformation)
+        columns.append(feature.column)
+        source_columns.append(feature.source_column)
+        embeddings.append(feature.column)
+
         if feature.n_clusters is not None:
             clusters.append(feature.n_clusters)
         else:
             clusters.append('auto')
-        monitors.append(feature.monitor)
-        monitor_components.append(feature.monitor_components)
 
     return pd.DataFrame(
         {
             'name': names,
-            'column': columns,
             'type': types,
-            'transformation': transformations,
+            'column': columns,
+            'source': source_columns,
+            'embeddings': embeddings,
             'n_clusters': clusters,
-            'monitor': monitors,
-            'monitor_components': monitor_components,
         }
     )
 
 
 @enum.unique
 class BaselineType(str, enum.Enum):
     PRE_PRODUCTION = 'PRE_PRODUCTION'
```

### Comparing `fiddler-client-2.0.0.dev6/fiddler/exceptions.py` & `fiddler-client-2.0.0.dev7/fiddler/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 
 try:
     from simplejson import JSONDecodeError
 except ImportError:
     from json import JSONDecodeError
 
 from requests.exceptions import HTTPError
+from fiddler.utils.logger import get_logger
 
-from fiddler.utils import logging
-
-logger = logging.getLogger(__name__)
+logger = get_logger(__name__)
 
 
 class NotSupported(Exception):
     pass
 
 
 class AsyncJobFailed(Exception):
@@ -30,15 +29,15 @@
         )
 
     def get_error_details(self) -> NamedTuple:
         status_code = self.response.status_code
         try:
             error_details = self.response.json().get('error', {})
         except JSONDecodeError:
-            raise FiddlerAPIHTTPException(
+            raise HttpException(
                 status_code=self.response.status_code,
                 error_code=self.response.status_code,
                 message=f'Invalid response content-type. {self.response.status_code}:{self.response.content}',
                 errors=[],
             )
         error_code = error_details.get('code')
         message = error_details.get('message')
@@ -46,27 +45,21 @@
         return self.ErrorResponse(status_code, error_code, message, errors)
 
 
 class FiddlerBaseException(Exception):
     pass
 
 
-class FiddlerException(FiddlerBaseException):
-    '''
-    Exception class to handle non API response exceptions
-    '''
-
-
-class FiddlerAPICallException(FiddlerBaseException):
+class ApiException(FiddlerBaseException):
     def __init__(self, message: str) -> None:
         self.message = message
         super().__init__(self.message)
 
 
-class FiddlerAPIHTTPException(FiddlerBaseException):
+class HttpException(FiddlerBaseException):
     '''
     Exception class to specifically handle Fiddler's API error responses structure.
     This is a generic API response exception class
     '''
 
     # @TODO: Handle standard API error response.
     # How to surface error messages coming form the server. Server responds error messages in a list. Which error to surface?
@@ -76,26 +69,26 @@
         self.status_code = status_code
         self.error_code = error_code
         self.message = message
         self.errors = errors
         super().__init__(self.message)
 
 
-class FiddlerAPIBadRequestException(FiddlerAPIHTTPException):
+class BadRequest(HttpException):
     pass
 
 
-class FiddlerAPINotFoundException(FiddlerAPIHTTPException):
+class NotFound(HttpException):
     pass
 
 
-class FiddlerAPIConflictException(FiddlerAPIHTTPException):
+class Conflict(HttpException):
     pass
 
 
-class FiddlerAPIForbiddenException(FiddlerAPIHTTPException):
+class Forbidden(HttpException):
     pass
 
 
-class FiddlerAPIInternalServerErrorException(FiddlerAPIHTTPException):
+class InternalServerError(HttpException):
     pass
```

### Comparing `fiddler-client-2.0.0.dev6/fiddler/libs/http_client.py` & `fiddler-client-2.0.0.dev7/fiddler/libs/http_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import json
 from copy import deepcopy
 from typing import Dict, Optional
 from urllib.parse import urljoin
 
 import requests
+import simplejson
 from requests.adapters import HTTPAdapter
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 
-from fiddler.exceptions import FiddlerAPICallException
-from fiddler.utils import logging
+from fiddler.exceptions import ApiException
+from fiddler.utils import logger
 
 APP_JSON_CONTENT_TYPE = 'application/json'
 
 
-logger = logging.getLogger(__name__)
+logger = logger.get_logger(__name__)
 
 
 class RequestClient:
     def __init__(
         self, base_url: str, headers: Dict[str, str], verify: bool = True
     ) -> None:
         self.base_url = base_url
@@ -57,15 +57,15 @@
         # override/update headers coming from the calling method
         if headers:
             request_headers = deepcopy(self.headers)
             request_headers.update(headers)
 
         content_type = request_headers.get('Content-Type')
         if data and content_type == APP_JSON_CONTENT_TYPE:
-            data = json.dumps(data)
+            data = simplejson.dumps(data, ignore_nan=True)
 
         kwargs.setdefault('allow_redirects', True)
         # requests is not able to pass the value of self.session.verify to the
         # verify param in kwargs when REQUESTS_CA_BUNDLE is set.
         # So setting that as default here
         kwargs.setdefault('verify', self.session.verify)
         try:
@@ -91,24 +91,24 @@
                     headers=request_headers,
                     timeout=timeout,
                     **kwargs,
                 )
         except requests.exceptions.Timeout:
             logger.error(f'{method} call failed with Timeout error for URL {url}')
             message = f'Request timed out while trying to reach endpoint {url}'
-            raise FiddlerAPICallException(message=message)
+            raise ApiException(message=message)
         except requests.exceptions.ConnectionError:
             logger.error(f'{method} call failed with ConnectionError for URL {url}')
             message = f'Unable to reach endpoint {url}'
-            raise FiddlerAPICallException(message=message)
+            raise ApiException(message=message)
         except requests.exceptions.RequestException:
             # catastrophic error.
             logger.error(f'{method} call failed with RequestException for URL {url}')
             message = f'Failed to reach endpoint {url}'
-            raise FiddlerAPICallException(message=message)
+            raise ApiException(message=message)
 
         response.raise_for_status()
         return response
 
     def get(
         self,
         *,
```

### Comparing `fiddler-client-2.0.0.dev6/fiddler/packtools/gem.py` & `fiddler-client-2.0.0.dev7/fiddler/packtools/gem.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev6/fiddler/packtools/keras_ig_helpers.py` & `fiddler-client-2.0.0.dev7/fiddler/packtools/keras_ig_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev6/fiddler/packtools/project_attributions_helpers.py` & `fiddler-client-2.0.0.dev7/fiddler/packtools/project_attributions_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev6/fiddler/packtools/template_model.py` & `fiddler-client-2.0.0.dev7/fiddler/packtools/template_model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev6/fiddler/utils/__init__.py` & `fiddler-client-2.0.0.dev7/fiddler/utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import copy
-import logging
 from typing import List
 
 import pandas as pd
 
 from fiddler import constants
 from fiddler.core_objects import Column, DatasetInfo, DataType, ModelInfo
-from fiddler.utils.pandas import is_datetime, try_series_retype
+from fiddler.utils.logger import get_logger
+from fiddler.utils.pandas_helper import is_datetime, try_series_retype
 
-LOG = logging.getLogger(__name__)
+LOG = get_logger(__name__)
 pd.set_option('mode.chained_assignment', None)
 
 
 def df_from_json_rows(
     dataset_rows_json: List[dict],
     dataset_info: DatasetInfo,
     include_fiddler_id: bool = False,
```

### Comparing `fiddler-client-2.0.0.dev6/fiddler/utils/exceptions.py` & `fiddler-client-2.0.0.dev7/fiddler/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev6/fiddler/utils/formatting.py` & `fiddler-client-2.0.0.dev7/fiddler/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev6/fiddler/utils/general_checks.py` & `fiddler-client-2.0.0.dev7/fiddler/utils/general_checks.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev6/fiddler/utils/helper.py` & `fiddler-client-2.0.0.dev7/fiddler/utils/helper.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev6/fiddler/utils/pandas.py` & `fiddler-client-2.0.0.dev7/fiddler/utils/pandas_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import logging
 from datetime import datetime
 from typing import Dict, Optional, Union
 
 import numpy as np
 import pandas as pd
 
 from fiddler import constants
+from fiddler.utils.logger import get_logger
 
-LOG = logging.getLogger(__name__)
+LOG = get_logger(__name__)
 TIMESTAMP = 'TIMESTAMP'
 
 
 def is_datetime(pandas_series):
     """
     Return true if Series contains all valid dates.
     """
@@ -20,14 +20,32 @@
     try:
         pd.to_datetime(pandas_series, format=constants.TIMESTAMP_FORMAT, errors='raise')
         return True
     except Exception:
         return False
 
 
+def is_list(pandas_series):
+    """
+    Return true if Series contains all valid lists.
+    """
+    try:
+        return pd.Series(pandas_series).apply(lambda x: isinstance(x, list)).all()
+    except Exception:
+        return False
+
+
+def is_vector_value(x: Union[list, np.ndarray]) -> bool:
+    """check if the input is a vector"""
+    if isinstance(x, list):
+        x = np.array(x)
+
+    return isinstance(x, np.ndarray) and np.issubdtype(x.dtype, np.number)
+
+
 def clean_df_types(df):
     """
     Cleans the dataframe types into serializable formats where needed. Currently
     works to:
     - Convert datetime to string
 
     TODO: Expand to all other datatypes
```

### Comparing `fiddler-client-2.0.0.dev6/fiddler/v2/api/alert_mixin.py` & `fiddler-client-2.0.0.dev7/fiddler/v2/api/alert_mixin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,68 +1,73 @@
 import json
 from datetime import datetime, timedelta
-import warnings
 from typing import Any, Dict, List, Optional
 
 from pydantic import parse_obj_as
 
 from fiddler.libs.http_client import RequestClient
-from fiddler.utils import logging
+from fiddler.utils.logger import get_logger
 from fiddler.v2.schema.alert import (
     AlertCondition,
     AlertRule,
     AlertRulePayload,
     AlertType,
     BinSize,
     ComparePeriod,
     CompareTo,
     Metric,
     Priority,
     TriggeredAlerts,
 )
+from fiddler.v2.utils.compatibility_helpers import project_id_compat, model_id_compat
 from fiddler.v2.utils.decorators import handle_api_error_response
 from fiddler.v2.utils.helpers import match_semver
 from fiddler.v2.utils.response_handler import (
     APIResponseHandler,
     PaginatedResponseHandler,
 )
 
-logger = logging.getLogger(__name__)
+logger = get_logger(__name__)
 
 
 class AlertMixin:
     FILTER_ALERT_RULES_API_VERSION = '>=23.1.0'
     GROUP_OF_COLUMNS_API_VERSION = '>=23.3.0'
 
     client: RequestClient
     organization_name: str
 
     @handle_api_error_response
     def add_alert_rule(
         self,
         name: str,
-        project_id: str,
-        model_id: str,
-        alert_type: AlertType,
-        metric: Metric,
-        compare_to: CompareTo,
-        priority: Priority,
-        critical_threshold: float,
-        condition: AlertCondition,
+        project_id: str = None,
+        model_id: str = None,
+        alert_type: AlertType = None,
+        metric: Metric = None,
+        compare_to: CompareTo = None,
+        priority: Priority = None,
+        critical_threshold: float = None,
+        condition: AlertCondition = None,
         bin_size: BinSize = BinSize.ONE_DAY,
-        baseline_id: Optional[str] = None,
+        baseline_name: Optional[str] = None,
         compare_period: Optional[ComparePeriod] = None,
         columns: Optional[List[str]] = None,
         warning_threshold: Optional[float] = None,
-        notifications_config: Optional[Dict[str, Dict[str, Any]]] = None,
+        project_name: str = None,
+        model_name: str = None,
+        notifications_config: Optional[Dict[str, Any]] = None,
     ) -> AlertRule:
         """
         To add an alert rule
+
         :param project_id: Unique project name for which the alert rule is created
         :param model_id: Unique model name for which the alert rule is created
+        :param project_name: Unique project name for which the alert rule is created
+        :param model_name: Unique model name for which the alert rule is created
         :param name: Name of the Alert rule
         :param alert_type: Selects one of the four metric types:
                 1) AlertType.PERFORMANCE
                 2) AlertType.DATA_DRIFT
                 3) AlertType.DATA_INTEGRITY
                 4) AlertType.SERVICE_METRICS
 
@@ -111,51 +116,77 @@
         :param warning_threshold: Threshold value to crossing which a warning level severity alert will be triggered
         :param critical_threshold: Threshold value to crossing which a critical level severity alert will be triggered
         :param condition: Select from:
                 1) AlertCondition.LESSER
                 2) AlertCondition.GREATER
         :param columns: List of column names on which alert rule is to be created. It can take ['__ANY__'] to check for all columns
         :param notifications_config: notifications config object created using helper method build_notifications_config()
-        :param baseline_id: Name of the baselne, whose histogram is compared against the same derived from current data.
+        :param baseline_name: Name of the baselne, whose histogram is compared against the same derived from current data.
                             Used only when alert type is AlertType.DATA_DRIFT.
         :return: created alert rule object
         """
-        if columns and not match_semver(self.server_info.server_version, self.GROUP_OF_COLUMNS_API_VERSION):
-            raise ValueError(f'columns parameter works with server version {self.GROUP_OF_COLUMNS_API_VERSION}')
+        required_params = [
+            'alert_type',
+            'metric',
+            'compare_to',
+            'priority',
+            'critical_threshold',
+            'condition',
+        ]
+        if any(param is None for param in required_params):
+            raise TypeError(
+                f'Please make sure {", ".join(required_params)} params are passed'
+            )
+
+        if columns and not match_semver(
+            self.server_info.server_version, self.GROUP_OF_COLUMNS_API_VERSION
+        ):
+            raise ValueError(
+                f'columns parameter works with server version {self.GROUP_OF_COLUMNS_API_VERSION}'
+            )
+
+        project_name = project_id_compat(
+            project_id=project_id, project_name=project_name
+        )
+
+        model_name = model_id_compat(
+            model_id=model_id,
+            model_name=model_name,
+        )
 
         if not notifications_config:
             notifications_config = self.build_notifications_config()
 
         if bin_size not in BinSize.keys():
             raise ValueError(f'bin_size: {bin_size} should be one of: {BinSize.keys()}')
         if compare_to == CompareTo.TIME_PERIOD and not compare_period:
             raise ValueError(
                 f'compare_period is required when compare_to is {CompareTo.TIME_PERIOD}'
             )
         if compare_period and compare_period not in ComparePeriod.keys():
             raise ValueError(f'compare_period should be one of{ComparePeriod.keys()}')
 
         request_body = AlertRulePayload(
-                organization_name=self.organization_name,
-                project_name=project_id,
-                model_name=model_id,
-                name=name,
-                alert_type=alert_type,
-                metric=metric,
-                compare_to=compare_to,
-                compare_period=compare_period,
-                priority=priority,
-                baseline_name=baseline_id,
-                feature_names=columns,
-                warning_threshold=warning_threshold,
-                critical_threshold=critical_threshold,
-                condition=condition,
-                time_bucket=bin_size,
-                notifications=notifications_config,
-            ).dict()
+            organization_name=self.organization_name,
+            project_name=project_name,
+            model_name=model_name,
+            name=name,
+            alert_type=alert_type,
+            metric=metric,
+            compare_to=compare_to,
+            compare_period=compare_period,
+            priority=priority,
+            baseline_name=baseline_name,
+            feature_names=columns,
+            warning_threshold=warning_threshold,
+            critical_threshold=critical_threshold,
+            condition=condition,
+            time_bucket=bin_size,
+            notifications=notifications_config,
+        ).dict()
         response = self.client.post(
             url='alert-configs',
             data=request_body,
         )
         response_data = APIResponseHandler(response)
         alert_rule_id = response_data.get_data().get('uuid')
 
@@ -180,23 +211,28 @@
     def get_alert_rules(
         self,
         project_id: Optional[str] = None,
         model_id: Optional[str] = None,
         alert_type: Optional[AlertType] = None,
         metric: Optional[Metric] = None,
         columns: Optional[List[str]] = None,
-        baseline_id: Optional[str] = None,
+        baseline_name: Optional[str] = None,
         ordering: Optional[List[str]] = None,
         offset: int = 0,
         limit: int = 20,
+        project_name: Optional[str] = None,
+        model_name: Optional[str] = None,
     ) -> List[AlertRule]:
         """
         Get a list of alert rules with respect to the filtering parameters
-        :param project_id: unique project name
-        :param model_id: unique model name
+
+        :param project_id: Unique project name for which the alert rule is created
+        :param model_id: Unique model name for which the alert rule is created
+        :param project_name: unique project name
+        :param model_name: unique model name
         :param alert_type: Selects one of the four metric types:
                 1) AlertType.PERFORMANCE
                 2) AlertType.DATA_DRIFT
                 3) AlertType.DATA_INTEGRITY
                 4) AlertType.SERVICE_METRICS
 
 
@@ -227,73 +263,92 @@
         :param limit: Number of records to be retrieved per page, also referred as page_size
         :param offset: Pointer to the starting of the page index. offset of the first page is 0
                         and it increments by limit for each page, for e.g., 5th pages offset when
                         limit=100 will be (5 - 1) * 100 = 400. This means 5th page will contain
                         records from index 400 to 499.
         :return: paginated list of alert rules for the set filters
         """
-        if columns and not match_semver(self.server_info.server_version, self.GROUP_OF_COLUMNS_API_VERSION):
-            raise ValueError(f'columns parameter works with server version {self.GROUP_OF_COLUMNS_API_VERSION}')
+        if columns and not match_semver(
+            self.server_info.server_version, self.GROUP_OF_COLUMNS_API_VERSION
+        ):
+            raise ValueError(
+                f'columns parameter works with server version {self.GROUP_OF_COLUMNS_API_VERSION}'
+            )
+
+        project_name = project_id_compat(
+            project_id=project_id, project_name=project_name
+        )
+
+        model_name = model_id_compat(
+            model_id=model_id,
+            model_name=model_name,
+        )
 
         alert_params = {
             'organization_name': self.organization_name,
             'offset': offset,
             'limit': limit,
         }
 
         if match_semver(
             self.server_info.server_version, self.FILTER_ALERT_RULES_API_VERSION
         ):
             filter_by_rules = []
-            if project_id:
+            if project_name:
                 filter_by_rules.append(
-                    {'field': 'project_name', 'operator': 'equal', 'value': project_id}
+                    {
+                        'field': 'project_name',
+                        'operator': 'equal',
+                        'value': project_name,
+                    }
                 )
 
-            if model_id:
+            if model_name:
                 filter_by_rules.append(
-                    {'field': 'model_name', 'operator': 'equal', 'value': model_id}
+                    {'field': 'model_name', 'operator': 'equal', 'value': model_name}
                 )
 
             if alert_type:
                 filter_by_rules.append(
                     {'field': 'alert_type', 'operator': 'equal', 'value': alert_type}
                 )
 
             if metric:
                 filter_by_rules.append(
                     {'field': 'metric', 'operator': 'equal', 'value': metric}
                 )
 
             if columns:
-                filter_by_rules.append({'field': 'feature_names', 'operator': 'contains', 'value': columns})
-            
-            if baseline_id:
+                filter_by_rules.append(
+                    {'field': 'feature_names', 'operator': 'contains', 'value': columns}
+                )
+
+            if baseline_name:
                 filter_by_rules.append(
                     {
                         'field': 'baseline_name',
                         'operator': 'equal',
-                        'value': baseline_id,
+                        'value': baseline_name,
                     }
                 )
 
             if ordering:
                 alert_params.update({'ordering': ','.join(ordering)})
 
             alert_params.update(
                 {'filter': json.dumps({'condition': 'AND', 'rules': filter_by_rules})}
             )
         else:
             alert_params.update(
                 {
-                    'project_name': project_id,
-                    'model_name': model_id,
+                    'project_name': project_name,
+                    'model_name': model_name,
                     'alert_type': alert_type,
                     'metric': metric,
-                    'baseline_name': baseline_id,
+                    'baseline_name': baseline_name,
                     'ordering': ordering,
                 }
             )
 
         response = self.client.get(
             url='alert-configs',
             params=alert_params,
@@ -339,24 +394,31 @@
         return parse_obj_as(List[TriggeredAlerts], items)
 
     def build_notifications_config(
         self,
         emails: str = '',
         pagerduty_services: str = '',
         pagerduty_severity: str = '',
-    ) -> Dict[str, Dict[str, Any]]:
+        webhooks: list[str] = [],
+    ) -> Dict[str, Any]:
         """
         To get the notifications value to be set for alert rule
         :param emails: Comma separated emails list
         :param pagerduty_services: Comma separated pagerduty services list
         :param pagerduty severity: Severity for the alerts triggered by pagerduty
+        :param webhooks: List of webhook uuids, on which we need notification
         :return: dict with emails and pagerduty dict. If left unused, will store empty string for these values
         """
+        webhooks_dict: list[dict[str, str]] = []
+        for webhook_uuid in webhooks:
+            webhooks_dict.append({'uuid': webhook_uuid})
+
         return {
             'emails': {
                 'email': emails,
             },
             'pagerduty': {
                 'service': pagerduty_services,
                 'severity': pagerduty_severity,
             },
+            'webhooks': webhooks_dict,
         }
```

### Comparing `fiddler-client-2.0.0.dev6/fiddler/v2/api/api.py` & `fiddler-client-2.0.0.dev7/fiddler/v2/api/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,123 @@
+import warnings
+from typing import Optional
 from urllib.parse import urljoin
 
 from fiddler._version import __version__
+from fiddler.constants import (
+    CURRENT_API_VERSION,
+    FIDDLER_CLIENT_VERSION_HEADER,
+    MIN_SERVER_VERSION,
+)
 from fiddler.libs.http_client import RequestClient
-from fiddler.utils import logging
+from fiddler.utils.logger import get_logger
 from fiddler.v2.api.alert_mixin import AlertMixin
 from fiddler.v2.api.baseline_mixin import BaselineMixin
 # @todo: This is v1 implementation needs to have a proper v2 approach
+from fiddler.v2.api.compatibility_mixin import CompatibilityMixin
 from fiddler.v2.api.dataset_mixin import DatasetMixin
 from fiddler.v2.api.events_mixin import EventsMixin
 from fiddler.v2.api.explainability_mixin import ExplainabilityMixin
+from fiddler.v2.api.infer_schema_mixin import InferModelSchemaMixin
 from fiddler.v2.api.job_mixin import JobMixin
 from fiddler.v2.api.model_deployment_mixin import ModelDeploymentMixin
 from fiddler.v2.api.model_mixin import ModelMixin
 from fiddler.v2.api.project_mixin import ProjectMixin
-from fiddler.v2.constants import CURRENT_API_VERSION, FIDDLER_CLIENT_VERSION_HEADER
 from fiddler.v2.schema.server_info import ServerInfo
 from fiddler.v2.utils.helpers import match_semver, raise_not_supported
+from fiddler.v2.utils.decorators import handle_api_error_response
 
-logger = logging.getLogger(__name__)
+logger = get_logger(__name__)
 
 
 class FiddlerClient(
     ModelMixin,
+    CompatibilityMixin,
     DatasetMixin,
     ProjectMixin,
     EventsMixin,
     JobMixin,
     BaselineMixin,
     AlertMixin,
     ExplainabilityMixin,
     ModelDeploymentMixin,
+    InferModelSchemaMixin,
 ):
     def __init__(
         self,
-        url: str,
-        organization_name: str,
-        auth_token: str,
-        timeout: int = None,
+        url: Optional[str] = None,
+        org_id: Optional[str] = None,
+        auth_token: Optional[str] = None,
+        proxies: Optional[dict] = None,
+        verbose: Optional[bool] = False,
+        timeout: int = 1200,  # sec
+        version: int = 2,
         verify: bool = True,
+        organization_name: Optional[str] = None,
     ) -> None:
         self.url = (
             url
             if url.endswith(CURRENT_API_VERSION)
             else urljoin(url, CURRENT_API_VERSION)
         )
         self.auth_token = auth_token
-        self.organization_name = organization_name
         self.request_headers = {'Authorization': f'Bearer {auth_token}'}
         self.request_headers.update({FIDDLER_CLIENT_VERSION_HEADER: f'{__version__}'})
         self.timeout = timeout
         self.client = RequestClient(
             base_url=self.url, headers=self.request_headers, verify=verify
         )
 
+        # Check for duplicate params
+        duplicated_params = [org_id, organization_name]
+        if all(value is not None for value in duplicated_params):
+            raise ValueError('Pass either org_id or organization_name')
+        if all(value is None for value in duplicated_params):
+            raise ValueError('Pass either org_id or organization_name')
+        self.organization_name = organization_name
+        if org_id:
+            warnings.warn(
+                f'WARNING: org_id is deprecated and will be removed from future \
+                        versions. Please use organization_name',
+                FutureWarning,
+            )
+
+            self.organization_name = org_id
+
         self.server_info: ServerInfo = self._get_server_info()
         self._check_server_version()
+        
+        # Checks client's version compatibility with server
+        self._check_version_compatibility()
 
     def _get_server_info(self) -> ServerInfo:
         response = self.client.get(
             url='server-info',
             params={'organization_name': self.organization_name},
         )
 
         return ServerInfo(**response.json().get('data'))
 
-    def _check_server_version(self) -> bool:
-        if match_semver(
-            self.server_info.server_version,
-            '<23.2.0',
-        ):
-            raise_not_supported(
-                compatible_client_version='1.8',
-                client_version=__version__,
-                server_version=self.server_info.server_version,
-            )
+    @handle_api_error_response
+    def _check_version_compatibility(self) -> None:
+        params = {
+            'client_version': __version__,
+            'client_name': 'python-sdk',
+        }
+        self.client.get(
+            url='version-compatibility',
+            params=params,
+        )
+        
+    def _check_server_version(self) -> None:
+        if match_semver(self.server_info.server_version, f'>={MIN_SERVER_VERSION}'):
+            return
+
+        raise_not_supported(
+            compatible_client_version='1.8',
+            client_version=__version__,
+            server_version=self.server_info.server_version,
+        )
+
+
+# Alias FiddlerClient as FiddlerApi
+FiddlerApi = FiddlerClient
```

### Comparing `fiddler-client-2.0.0.dev6/fiddler/v2/api/events_mixin.py` & `fiddler-client-2.0.0.dev7/fiddler/v2/api/events_mixin.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,46 +3,52 @@
 from http import HTTPStatus
 from pathlib import Path
 from typing import Any, Dict, Optional, Union
 
 import pandas as pd
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 
+from fiddler.constants import FiddlerTimestamp, FileType, UploadType
 from fiddler.core_objects import BatchPublishType
-from fiddler.exceptions import FiddlerAPIHTTPException
+from fiddler.exceptions import HttpException
 from fiddler.libs.http_client import RequestClient
-from fiddler.utils import logging
+from fiddler.utils import get_logger
+from fiddler.utils import logger
 from fiddler.v2.api.helpers import multipart_upload
-from fiddler.v2.constants import FiddlerTimestamp, FileType, UploadType
 from fiddler.v2.schema.events import EventIngest, EventsIngest
+from fiddler.v2.utils.compatibility_helpers import (
+    project_id_compat,
+    model_id_compat,
+    update_event_compat,
+)
 from fiddler.v2.utils.decorators import handle_api_error_response
 from fiddler.v2.utils.response_handler import APIResponseHandler
 
-logger = logging.getLogger(__name__)
+logger = get_logger(__name__)
 
 
 class EventsMixin:
     client: RequestClient
     organization_name: str
 
     @handle_api_error_response
-    def publish_events_batch(
+    def _publish_events_batch_from_file(
         self,
         project_name: str,
         model_name: str,
         events_path: Path,
         batch_id: Optional[str] = None,
         events_schema: Optional[str] = None,
         id_field: Optional[str] = None,
         is_update: Optional[bool] = None,
         timestamp_field: Optional[str] = None,
         timestamp_format: Optional[FiddlerTimestamp] = None,
         group_by: Optional[str] = None,
         file_type: Optional[FileType] = None,
-        is_sync: Optional[bool] = False,
+        wait: Optional[bool] = False,
     ) -> Dict[str, str]:
         """
         Publishes a batch events object to Fiddler Service.
 
         :param project_name: The project to which the model whose events are being published belongs.
         :param model_name: The model whose events are being published.
         :param events_path: pathlib.Path pointing to the events file to be uploaded
@@ -60,18 +66,19 @@
         :param group_by: Column to group events together for Model Performance metrics. For example,
                         in ranking models that column should be query_id or session_id, used to
                         compute NDCG and MAP. Be aware that the batch_source file/dataset provided should have
                         events belonging to the SAME query_id/session_id TOGETHER and cannot be mixed
                         in the file. For example, having a file with rows belonging to query_id 31,31,31,2,2,31,31,31
                         would not work. Please sort the file by group_by group first to have rows with
                         the following order: query_id 31,31,31,31,31,31,2,2.
-        :param file_type: FileType which specifices the filetype csv etc.
-        :param is_sync: A boolean value which determines if the upload method works in synchronous mode or async mode
+        :param file_type: FileType which specifies the filetype csv etc.
+        :param wait: A boolean value which determines if the upload method works in synchronous mode or async mode
         :returns: Dictionary containing details of the job used to publish events incase of 202 response from the server.
         """
+
         file_name = events_path.name
         response = multipart_upload(
             client=self.client,
             organization_name=self.organization_name,
             project_name=project_name,
             identifier=model_name,
             upload_type=UploadType.EVENT.value,
@@ -93,15 +100,15 @@
         response = self.client.post(
             url=f'events/{self.organization_name}:{project_name}:{model_name}/ingest',
             data=request_body,
         )
         # @TODO: Handle invalid file path exception
         if response.status_code == HTTPStatus.ACCEPTED:
             resp = APIResponseHandler(response).get_data()
-            if is_sync:
+            if wait:
                 job_uuid = resp['job_uuid']
                 job_name = f'Model[{project_name}/{model_name}] - Publish events batch'
                 logger.info(
                     'Model[%s/%s] - Submitted job (%s) for publish events batch',
                     project_name,
                     model_name,
                     job_uuid,
@@ -109,50 +116,192 @@
 
                 job = self.wait_for_job(uuid=job_uuid, job_name=job_name).get_data()
                 job.pop('extras', None)
                 return job
             else:
                 return resp
         else:
-            # raising a generic FiddlerAPIHTTPException
+            # raising a generic HttpException
             logger.error('Failed to publish events')
-            raise FiddlerAPIHTTPException(
+            raise HttpException(
                 response.status_code,
                 error_code=response.status_code,
                 message=response.content,
                 errors=[],
             )
 
     @handle_api_error_response
+    def publish_events_batch(
+        self,
+        project_id: str = None,
+        model_id: str = None,
+        batch_source: Union[pd.DataFrame, str] = None,
+        id_field: Optional[str] = None,
+        update_event: Optional[bool] = False,
+        timestamp_field: Optional[str] = None,
+        timestamp_format: Optional[FiddlerTimestamp] = None,
+        data_source: Optional[BatchPublishType] = None,
+        casting_type: Optional[bool] = False,
+        credentials: Optional[dict] = None,
+        group_by: Optional[str] = None,
+        project_name: str = None,
+        model_name: str = None,
+        events_path: Path = None,
+        batch_id: Optional[str] = None,
+        events_schema: Optional[str] = None,
+        is_update: Optional[bool] = None,
+        file_type: Optional[FileType] = None,
+        wait: Optional[bool] = False,
+    ) -> Dict[str, str]:
+        """
+        Publishes a batch events object to Fiddler Service.
+
+        :param project_id: The project to which the model whose events are being published belongs.
+        :param model_id: The model whose events are being published.
+        :param batch_source: Deprecated
+        :param update_event: Deprecated
+        :param data_source: Deprecated
+        :param casting_type: Deprecated
+        :param credentials: Deprecated
+        :param project_name: The project to which the model whose events are being published belongs.
+        :param model_name: The model whose events are being published.
+        :param events_path: pathlib.Path pointing to the events file to be uploaded
+        :param batch_id: <TBD>
+        :param events_schema: <TBD>
+        :param id_field: Column to extract id value from.
+        :param is_update: Bool indicating if the events are updates to previously published rows
+        :param timestamp_field: Column to extract timestamp value from.
+                                Timestamp must match the specified format in `timestamp_format`.
+        :param timestamp_format:Format of timestamp within batch object. Can be one of:
+                                - FiddlerTimestamp.INFER
+                                - FiddlerTimestamp.EPOCH_MILLISECONDS
+                                - FiddlerTimestamp.EPOCH_SECONDS
+                                - FiddlerTimestamp.ISO_8601
+        :param group_by: Column to group events together for Model Performance metrics. For example,
+                        in ranking models that column should be query_id or session_id, used to
+                        compute NDCG and MAP. Be aware that the batch_source file/dataset provided should have
+                        events belonging to the SAME query_id/session_id TOGETHER and cannot be mixed
+                        in the file. For example, having a file with rows belonging to query_id 31,31,31,2,2,31,31,31
+                        would not work. Please sort the file by group_by group first to have rows with
+                        the following order: query_id 31,31,31,31,31,31,2,2.
+        :param file_type: FileType which specifices the filetype csv etc.
+        :param wait: A boolean value which determines if the upload method works in synchronous mode or async mode
+        :returns: Dictionary containing details of the job used to publish events incase of 202 response from the server.
+        """
+
+        project_name = project_id_compat(
+            project_id=project_id, project_name=project_name
+        )
+        model_name = model_id_compat(
+            model_id=model_id,
+            model_name=model_name,
+        )
+        is_update = update_event_compat(update_event=update_event, is_update=is_update)
+        # Either batch_source or events_path can be given for _publish_events_batch_from_file
+        if batch_source is None and events_path is None:
+            raise ValueError(f'`batch_source` parameter is required.')
+
+        if timestamp_format:
+            if type(timestamp_format) is not FiddlerTimestamp:
+                raise ValueError(
+                    f'timestamp_format format is not of type FiddlerTimestamp'
+                )
+            timestamp_format = FiddlerTimestamp(timestamp_format.value)
+        if type(batch_source) == pd.DataFrame and (
+            data_source is None or BatchPublishType.DATAFRAME == data_source
+        ):
+            if batch_source.empty:
+                raise ValueError(
+                    'The batch provided is empty. Please retry with at least one row of data.'
+                )
+            return self._publish_events_batch_dataframe(
+                project_name=project_name,
+                model_name=model_name,
+                events_df=batch_source,
+                id_field=id_field,
+                is_update=is_update,
+                timestamp_field=timestamp_field,
+                timestamp_format=timestamp_format,
+                group_by=group_by,
+                wait=wait,
+            )
+        elif (events_path or type(batch_source) == str) and (
+            data_source is None or BatchPublishType.LOCAL_DISK == data_source
+        ):
+            return self._publish_events_batch_from_file(
+                project_name=project_name,
+                model_name=model_name,
+                events_path=events_path or Path(batch_source),
+                id_field=id_field,
+                is_update=update_event,
+                timestamp_field=timestamp_field,
+                timestamp_format=timestamp_format,
+                group_by=group_by,
+                file_type=FileType.CSV,
+                wait=wait,
+            )
+        else:
+            raise NotImplementedError(
+                'Batch source other than dataframe and csv is not implemented now'
+            )
+
+    @handle_api_error_response
     def publish_event(
         self,
-        project_name: str,
-        model_name: str,
-        event: dict,
+        project_id: str = None,
+        model_id: str = None,
+        event: dict = None,
         event_id: Optional[str] = None,
+        update_event: Optional[bool] = None,
+        event_timestamp: Optional[int] = None,
+        timestamp_format: FiddlerTimestamp = None,
+        casting_type: Optional[bool] = False,
+        dry_run: Optional[bool] = False,
+        project_name: str = None,
+        model_name: str = None,
         id_field: Optional[str] = None,
         is_update: Optional[bool] = None,
-        event_timestamp: Optional[str] = None,
-        timestamp_format: Optional[str] = None,
     ) -> Optional[str]:
         """
         Publishes an event to Fiddler Service.
 
+        :param project_id: The project to which the model whose events are being published belongs.
+        :param model_id: The model whose events are being published.
+        :param casting_type: Deprecated
+        :param update_event: Deprecated
+        :param dry_run: Deprecated
         :param project_name: The project to which the model whose events are being published belongs
         :param model_name: The model whose events are being published
         :param dict event: Dictionary of event details, such as features and predictions.
         :param event_id: Unique str event id for the event
         :param event_timestamp: The UTC timestamp of the event in epoch milliseconds (e.g. 1609462800000)
         :param timestamp_format: Format of timestamp within batch object. Can be one of:
                                 - FiddlerTimestamp.INFER
                                 - FiddlerTimestamp.EPOCH_MILLISECONDS
                                 - FiddlerTimestamp.EPOCH_SECONDS
                                 - FiddlerTimestamp.ISO_8601
         :returns: Unique event id incase of successful submitted request.
         """
+        project_name = project_id_compat(
+            project_id=project_id, project_name=project_name
+        )
+        model_name = model_id_compat(
+            model_id=model_id,
+            model_name=model_name,
+        )
+        if event is None:
+            raise ValueError('`event` parameter is required.')
+        is_update = update_event_compat(update_event=update_event, is_update=is_update)
+        if timestamp_format:
+            if type(timestamp_format) is not FiddlerTimestamp:
+                raise ValueError(
+                    f'timestamp_format format is not of type FiddlerTimestamp'
+                )
+            timestamp_format = FiddlerTimestamp(timestamp_format.value)
+
         request_body = EventIngest(
             event=event,
             event_id=event_id,
             id_field=id_field,
             is_update=is_update,
             event_timestamp=event_timestamp,
             timestamp_format=timestamp_format,
@@ -162,36 +311,36 @@
             data=request_body,
         )
         if response.status_code == HTTPStatus.ACCEPTED:
             response_dict = APIResponseHandler(response).get_data()
             logger.info(response_dict.get('message'))
             return response_dict.get('__fiddler_id')
         else:
-            # raising a generic FiddlerAPIHTTPException
+            # raising a generic HttpException
             logger.error('Failed to publish events')
-            raise FiddlerAPIHTTPException(
+            raise HttpException(
                 response.status_code,
                 error_code=response.status_code,
                 message=response.content,
                 errors=[],
             )
 
     @handle_api_error_response
-    def publish_events_batch_dataframe(
+    def _publish_events_batch_dataframe(
         self,
         project_name: str,
         model_name: str,
         events_df: pd.DataFrame,
         batch_id: Optional[str] = None,
         id_field: Optional[str] = None,
         is_update: Optional[bool] = None,
         timestamp_field: Optional[str] = None,
         timestamp_format: Optional[FiddlerTimestamp] = None,
         group_by: Optional[str] = None,
-        is_sync: Optional[bool] = False,
+        wait: Optional[bool] = False,
     ) -> Dict[str, str]:
         """
         Publishes a batch events object to Fiddler Service.
 
         :param project_name: The project to which the model whose events are being published belongs.
         :param model_name: The model whose events are being published.
         :param events_df: pd.DataFrame object having the events
@@ -208,15 +357,15 @@
         :param group_by: Column to group events together for Model Performance metrics. For example,
                         in ranking models that column should be query_id or session_id, used to
                         compute NDCG and MAP. Be aware that the batch_source file/dataset provided should have
                         events belonging to the SAME query_id/session_id TOGETHER and cannot be mixed
                         in the file. For example, having a file with rows belonging to query_id 31,31,31,2,2,31,31,31
                         would not work. Please sort the file by group_by group first to have rows with
                         the following order: query_id 31,31,31,31,31,31,2,2.
-        :param is_sync: A boolean value which determines if the upload method works in synchronous mode or async mode
+        :param wait: A boolean value which determines if the upload method works in synchronous mode or async mode
         :returns: Dictionary containing details of the job used to publish events incase of 202 response from the server.
         """
         if events_df is None or events_df.empty:
             raise ValueError(
                 'The batch provided is empty. Please retry with at least one row of data.'
             )
 
@@ -230,31 +379,36 @@
                 events_path=events_path,
                 batch_id=batch_id,
                 id_field=id_field,
                 is_update=is_update,
                 timestamp_field=timestamp_field,
                 timestamp_format=timestamp_format,
                 group_by=group_by,
-                is_sync=is_sync,
+                wait=wait,
             )
 
     @handle_api_error_response
     def publish_events_batch_schema(  # noqa
         self,
         batch_source: Union[Path, str],
         publish_schema: Dict[str, Any],
         data_source: Optional[BatchPublishType] = None,
-        is_sync: Optional[bool] = False,
+        credentials: Optional[dict] = None,
+        group_by: Optional[str] = None,
+        wait: Optional[bool] = False,
     ) -> Dict[str, str]:
         """
         Publishes a batch events object to Fiddler Service.
+
         :param batch_source: pathlib.Path pointing to the events file to be uploaded
         :param publish_schema: Dict object specifying layout of data.
         :param data_source: path of the source file of type BatchPublishType
-        :param is_sync: A boolean value which determines if the upload method works in
+        :param credentials: Deprecated
+        :param group_by: Deprecated
+        :param wait: A boolean value which determines if the upload method works in
                         synchronous mode or async mode
         :returns: Dictionary containing details of the job used to publish events incase
                   of 202 response from the server.
         """
         request_body_json = {}
         request_body_json['schema'] = publish_schema
         if data_source == BatchPublishType.AWS_S3 and isinstance(batch_source, str):
@@ -291,15 +445,15 @@
                 url=f'events/{self.organization_name}/ingest/schema',
                 headers={'Content-Type': content_type_header},
                 data=request_body,
             )
         # @TODO: Handle invalid file path exception
         if response.status_code == HTTPStatus.ACCEPTED:
             resp = APIResponseHandler(response).get_data()
-            if is_sync:
+            if wait:
                 job_uuid = resp['job_uuid']
                 project_name = publish_schema.get('__static', {}).get('__project')
                 model_name = publish_schema.get('__static', {}).get('__model')
                 job_name = (
                     f'Model[{project_name}/{model_name}] - Publish events batch schema',
                 )
 
@@ -312,15 +466,15 @@
                 job = self.wait_for_job(uuid=job_uuid, job_name=job_name).get_data()
                 job.pop('extras', None)
                 return job
             else:
                 return resp
 
         else:
-            # raising a generic FiddlerAPIHTTPException
+            # raising a generic HttpException
             logger.error('Failed to upload events schema.')
-            raise FiddlerAPIHTTPException(
+            raise HttpException(
                 response.status_code,
                 error_code=response.status_code,
                 message=response.content,
                 errors=[],
             )
```

### Comparing `fiddler-client-2.0.0.dev6/fiddler/v2/api/explainability_mixin.py` & `fiddler-client-2.0.0.dev7/fiddler/v2/api/explainability_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from collections import namedtuple
 from typing import Dict, List, NamedTuple, Optional, Union
 
 import pandas as pd
 from pydantic import BaseModel
 
 from fiddler.libs.http_client import RequestClient
-from fiddler.utils import logging
-from fiddler.utils.pandas import try_series_retype
+from fiddler.utils.logger import get_logger
+from fiddler.utils.pandas_helper import try_series_retype
 from fiddler.v2.utils.decorators import handle_api_error_response
 from fiddler.v2.utils.response_handler import APIResponseHandler
 
-logger = logging.getLogger(__name__)
+logger = get_logger(__name__)
 
 
 class DatasetDataSource(BaseModel):
     source_type = 'DATASET'
     dataset_name: str
     source: Optional[str]
     num_samples: Optional[int]
```

### Comparing `fiddler-client-2.0.0.dev6/fiddler/v2/api/helpers.py` & `fiddler-client-2.0.0.dev7/fiddler/v2/api/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import math
 import os
 from typing import Dict, Optional
 from urllib.parse import urljoin
 
 from tqdm import trange
 
-from fiddler.libs.http_client import RequestClient
-from fiddler.utils import logging
-from fiddler.v2.constants import (
+from fiddler.constants import (
     CONTENT_TYPE_OCTET_STREAM_HEADER,
     MULTI_PART_CHUNK_SIZE,
     MULTI_PART_UPLOAD_SIZE_THRESHOLD,
     UploadType,
 )
+from fiddler.libs.http_client import RequestClient
+from fiddler.utils.logger import get_logger
 from fiddler.v2.utils.response_handler import APIResponseHandler
 
-logger = logging.getLogger(__name__)
+logger = get_logger(__name__)
 
 UPLOAD_ID_KEY = 'upload_id'
 UPLOAD_TYPE_KEY = 'upload_type'
 RESOURCE_IDENT_KEY = 'resource_identifier'
 FILE_NAME_KEY = 'file_name'
 MULTIPART_UPLOAD_KEY = 'multipart_upload'
 NUM_ROWS_KEY = 'num_rows'
```

### Comparing `fiddler-client-2.0.0.dev6/fiddler/v2/api/job_mixin.py` & `fiddler-client-2.0.0.dev7/fiddler/v2/api/job_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 from http import HTTPStatus
 from typing import Iterator, List, Optional
 
 from requests.exceptions import ConnectionError
 
 from fiddler.exceptions import AsyncJobFailed
 from fiddler.libs.http_client import RequestClient
-from fiddler.utils import logging
+from fiddler.utils import logger
+from fiddler.utils.logger import get_logger
 from fiddler.v2.schema.job import JobStatus
 from fiddler.v2.utils.decorators import handle_api_error_response
 from fiddler.v2.utils.response_handler import JobResponseHandler
 
-logger = logging.getLogger(__name__)
+logger = get_logger(__name__)
 
 
 class JobMixin:
     DEFAULT_POLL_INTERVAL = 3  # In seconds
     DEFAULT_TIMEOUT = 1800  # 30 minutes in seconds
 
     client: RequestClient
```

### Comparing `fiddler-client-2.0.0.dev6/fiddler/v2/api/model_artifact_deploy.py` & `fiddler-client-2.0.0.dev7/fiddler/v2/api/model_artifact_deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import json
 import math
 import os
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Callable, Dict, List, Optional
 
+from fiddler.constants import CONTENT_TYPE_OCTET_STREAM_HEADER, \
+    MULTI_PART_CHUNK_SIZE
 from fiddler.libs.http_client import RequestClient
-from fiddler.utils import logging
-from fiddler.v2.constants import CONTENT_TYPE_OCTET_STREAM_HEADER, MULTI_PART_CHUNK_SIZE
+from fiddler.utils.logger import get_logger
 from fiddler.v2.schema.model_deployment import DeploymentParams
 from fiddler.v2.utils.response_handler import APIResponseHandler
 
-logger = logging.getLogger(__name__)
+logger = get_logger(__name__)
 
 
 class _AbstractModelDeployer(ABC):
     """Abstract class for deploying model artifact"""
 
     def __init__(
         self,
```

### Comparing `fiddler-client-2.0.0.dev6/fiddler/v2/api/model_deployment_mixin.py` & `fiddler-client-2.0.0.dev7/fiddler/v2/api/model_deployment_mixin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,98 @@
 from typing import Optional
 
 from fiddler.libs.http_client import RequestClient
-from fiddler.utils import logging
+from fiddler.utils import logger
+from fiddler.utils.logger import get_logger
 from fiddler.v2.schema.model_deployment import ModelDeployment
+from fiddler.v2.utils.compatibility_helpers import (
+    project_id_compat,
+    model_id_compat,
+    is_sync_id_compat,
+)
 from fiddler.v2.utils.decorators import check_version, handle_api_error_response
 
-logger = logging.getLogger(__name__)
+logger = get_logger(__name__)
 
 
 class ModelDeploymentMixin:
     """Model deployment api handler"""
 
     client: RequestClient
     organization_name: str
 
     @check_version(version_expr='>=23.1.0')
     @handle_api_error_response
     def get_model_deployment(
         self,
-        model_name: str,
-        project_name: str,
+        project_id: str = None,
+        model_id: str = None,
+        model_name: str = None,
+        project_name: str = None,
     ) -> ModelDeployment:
         """
         Get model deployment object
+        :params project_id: Project name
+        :params model_id: Model name
         :param model_name: Model name
         :param project_name: Project name
         :return: Model deployment object
         """
-        model_id = f'{self.organization_name}:{project_name}:{model_name}'
-        response = self.client.get(url=f'model-deployments/{model_id}')
+        project_name = project_id_compat(
+            project_id=project_id, project_name=project_name
+        )
+        model_name = model_id_compat(
+            model_id=model_id,
+            model_name=model_name,
+        )
+        model_id_url = f'{self.organization_name}:{project_name}:{model_name}'
+        response = self.client.get(url=f'model-deployments/{model_id_url}')
 
         return ModelDeployment(**response.json().get('data'))
 
+
     @check_version(version_expr='>=23.1.0')
     @handle_api_error_response
     def update_model_deployment(
         self,
-        model_name: str,
-        project_name: str,
+        project_id: str = None,
+        model_id: str = None,
         active: Optional[bool] = None,
         replicas: Optional[int] = None,
         cpu: Optional[int] = None,
         memory: Optional[int] = None,
+        is_sync: bool = True,
+        model_name: str = None,
+        project_name: str = None,
         wait: bool = True,
     ) -> ModelDeployment:
         """
         Update model deployment fields like replicas, cpu, memory
+
+        :param project_id: Project name
+        :param model_id: Model name
         :param model_name: Model name
         :param project_name: Project name
         :param active: Set False to scale down model deployment and True to scale up
         :param replicas: Number of model deployment replicas to run
         :param cpu: Amount of milli cpus to allocate for each replica
         :param memory: Amount of mebibytes memory to allocate for each replica
+        :param is_sync: Whether to wait for async job to finish or return
         :param wait: Whether to wait for async job to finish or return
         :return: Model deployment object
         """
+        project_name = project_id_compat(
+            project_id=project_id, project_name=project_name
+        )
+        model_name = model_id_compat(
+            model_id=model_id,
+            model_name=model_name,
+        )
+        wait = is_sync_id_compat(is_sync=is_sync, wait=wait)
+
         body = {}
 
         if active is not None:
             body['active'] = active
 
         if replicas is not None:
             body['replicas'] = replicas
```

### Comparing `fiddler-client-2.0.0.dev6/fiddler/v2/api/model_mixin.py` & `fiddler-client-2.0.0.dev7/fiddler/v2/api/model_mixin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 import os
 import shutil
 import tempfile
+import warnings
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 from pydantic import parse_obj_as
 
 from fiddler import ModelInfo
-from fiddler.core_objects import BaselineType
+from fiddler.constants import MULTI_PART_CHUNK_SIZE
+from fiddler.core_objects import ModelInputType, ModelTask
 from fiddler.libs.http_client import RequestClient
-from fiddler.utils import logging
-from fiddler.v2.api.baseline_mixin import BaselineMixin
+from fiddler.schemas.model_schema import ModelSchema
+from fiddler.schemas.model_spec import ModelSpec
+from fiddler.schemas.model_task_params import ModelTaskParams
+from fiddler.schemas.xai_params import XaiParams
+from fiddler.utils.logger import get_logger
 from fiddler.v2.api.model_artifact_deploy import (
     ModelArtifactDeployer,
     MultiPartModelArtifactDeployer,
 )
-from fiddler.v2.constants import MULTI_PART_CHUNK_SIZE
 from fiddler.v2.schema.model import Model
 from fiddler.v2.schema.model_deployment import ArtifactType, DeploymentParams
+from fiddler.v2.utils.compatibility_helpers import (
+    project_id_compat,
+    model_id_compat,
+    dataset_id_compat,
+    is_sync_id_compat,
+    model_dir_compat,
+)
 from fiddler.v2.utils.decorators import check_version, handle_api_error_response
 from fiddler.v2.utils.helpers import get_model_artifact_info, read_model_yaml
 from fiddler.v2.utils.response_handler import (
     APIResponseHandler,
     PaginatedResponseHandler,
 )
 from fiddler.v2.utils.validations import validate_artifact_dir
 
-logger = logging.getLogger(__name__)
+logger = get_logger(__name__)
 
 
 class ModelMixin:
     ADD_SURROGATE_MODEL_API_VERSION = '>=22.12.0'
     ADD_MODEL_ARTIFACT_API_VERSION = '>=22.12.0'
     DELETE_MODEL_API_VERSION = '>=22.12.0'
 
@@ -76,106 +87,171 @@
         """
         response = self.client.get(
             url=f'models/{self.organization_name}:{project_name}:{model_name}',
         )
         response_handler = APIResponseHandler(response)
         return Model.deserialize(response_handler)
 
-    def get_model_info(self, project_name: str, model_name: str) -> ModelInfo:
+    def get_model_info(
+        self,
+        project_id: str = None,
+        model_id: str = None,
+        project_name: str = None,
+        model_name: str = None,
+    ) -> ModelInfo:
         """Get ModelInfo for a model.
 
+        :params project_id: The project to which the model belongs to
+        :params model_id: The model name of which you need the details
         :params project_name: The project to which the model belongs to
         :params model_name: The model name of which you need the details
 
         :returns: A fiddler.ModelInfo object describing the model.
         """
+        project_name = project_id_compat(
+            project_id=project_id, project_name=project_name
+        )
+        model_name = model_id_compat(
+            model_id=model_id,
+            model_name=model_name,
+        )
         model_info_dict = self.get_model(
             project_name=project_name, model_name=model_name
         ).info
         return ModelInfo.from_dict(model_info_dict)
 
     @handle_api_error_response
-    def _add_model_call(
-        self, project_name: str, model_name: str, info: ModelInfo
+    def add_model(  # noqa: C901
+        self,
+        project_id: str = None,
+        model_id: str = None,
+        dataset_id: str = None,
+        model_info: Optional[ModelInfo] = None,
+        is_sync: Optional[bool] = True,
+        task: Optional[ModelTask] = None,
+        input_type: Optional[ModelInputType] = None,
+        schema: Optional[ModelSchema] = None,
+        spec: Optional[ModelSpec] = None,
+        task_params: Optional[ModelTaskParams] = None,
+        xai_params: Optional[XaiParams] = None,
+        display_name: Optional[str] = None,
+        description: Optional[str] = None,
+        algorithm: Optional[str] = None,
+        framework: Optional[str] = None,
+        event_id_col: Optional[str] = None,
+        event_ts_col: Optional[str] = None,
+        event_ts_format: Optional[str] = None,
+        wait: bool = True,
+        project_name: str = None,
+        model_name: str = None,
+        dataset_name: Optional[str] = None,
     ) -> Model:
         """
-        Function to add a model to fiddler for monitoring
-
+        Onboard model to Fiddler Platform
+        :params project_id: The project to which the model belongs to
+        :params model_id: The model name of which you need the details
+        :param dataset_id: name of the dataset
+        :param is_sync: Wait for job to complete or return after submitting
         :param project_name: project name where the model will be added
-        :type project_name: string
         :param model_name: name of the model
-        :type model_name: string
-        :param info: model related information
-        :type info: ModelInfo
-
-        :return: Model object which contains the model details
+        :param dataset_name: name of the dataset
+        :param model_info: (Deprecated) model related information from user
+        :param task: Task the model is designed to address
+        :param input_type: Whether the model is in the tabular or text
+        :param schema: ModelSchema object
+        :param spec: ModelSpec object
+        :param task_params: ModelTaskParams object
+        :param xai_params: XaiParams object
+        :param display_name: Display name for the model
+        :param description: Description for the model
+        :param algorithm: Algorithm used for this model
+        :param framework: Framework used for this model
+        :param event_id_col: Column name to use as event id
+        :param event_ts_col: Column name to use as event timestamp
+        :param event_ts_format: Format of the event timestamp specified in event_ts_col
+        :param wait: Whether to wait for job to complete or return after submitting
+            the job
         """
-        if not isinstance(info, ModelInfo):
+
+        project_name = project_id_compat(
+            project_id=project_id, project_name=project_name
+        )
+
+        model_name = model_id_compat(
+            model_id=model_id,
+            model_name=model_name,
+        )
+
+        dataset_name = dataset_id_compat(
+            dataset_id=dataset_id,
+            dataset_name=dataset_name,
+        )
+
+        if model_info:
+            warnings.warn(
+                'model_info is deprecated from 2.0.0. Use schema and spec instead',
+                DeprecationWarning,
+            )
+            if dataset_name:
+                model_info.datasets = [dataset_name]
+        elif not (schema and spec and input_type and task):
             raise ValueError(
-                f'The value passed to the info parameter must be a ModelInfo object.'
-                f'Instead, found value of type {type(info)}'
+                'Model requires either model_info or input_type, task, schema and spec'
             )
 
         request_body = {
             'name': model_name,
             'project_name': project_name,
             'organization_name': self.organization_name,
-            'info': info.to_dict(),
-            'model_type': None,
-            'file_list': None,
         }
 
+        if model_info:
+            request_body['info'] = model_info.to_dict()
+        if dataset_name:
+            request_body['dataset_name'] = dataset_name
+        if input_type:
+            request_body['input_type'] = input_type.value
+        if task:
+            request_body['task'] = task.value
+        if schema:
+            request_body['schema'] = schema.dict()
+        if spec:
+            request_body['spec'] = spec.dict()
+        if task_params:
+            request_body['task_params'] = task_params.dict()
+        if xai_params:
+            request_body['xai_params'] = xai_params.dict()
+        if description:
+            request_body['description'] = description
+        if algorithm:
+            request_body['algorithm'] = algorithm
+        if framework:
+            request_body['framework'] = framework
+        if display_name:
+            request_body['display_name'] = display_name
+        if event_id_col:
+            request_body['event_id_col'] = event_id_col
+        if event_ts_col:
+            request_body['event_ts_col'] = event_ts_col
+        if event_ts_format:
+            request_body['event_ts_format'] = event_ts_format
+
         response = self.client.post(
             url='models',
             data=request_body,
         )
-        logger.info('Model %s added to %s project', model_name, project_name)
-
-        return Model.deserialize(APIResponseHandler(response))
-
-    def add_model(
-        self,
-        project_name: str,
-        model_name: str,
-        dataset_name: str,
-        model_info: ModelInfo,
-    ) -> None:
-        """
-        Function to add a model to fiddler for monitoring
-
-        :param project_name: project name where the model will be added
-        :param model_name: name of the model
-        :param dataset_name: name of the dataset
-        :param model_info: model related information from user
-        """
 
-        if not isinstance(model_info, ModelInfo):
-            raise ValueError(
-                f'The value passed to the model_info parameter must be a ModelInfo '
-                f'object. Instead, found value of type {type(model_info)}'
-            )
+        logger.info('Model %s added to %s project', model_name, project_name)
 
-        # associate dataset_id with model_info. This was not done during
-        # from_dataset_info call.
-        model_info.datasets = [dataset_name]
+        model = Model.deserialize(APIResponseHandler(response))
+        if model.job_uuid and wait:
+            job_name = f'Model[{project_name}/{model_name}] - Initializing monitoring'
+            self.wait_for_job(uuid=model.job_uuid, job_name=job_name)  # noqa
 
-        model = self._add_model_call(
-            model_name=model_name,
-            project_name=project_name,
-            info=model_info,
-        )
-        BaselineMixin.add_baseline(
-            project_name=project_name,
-            model_name=model_name,
-            baseline_name='DEFAULT',
-            type=BaselineType.PRE_PRODUCTION,
-            run_async=True,
-            wait=True,
-        )
-        logger.info(f'Successfully added model {model.name} to project {project_name}')
+        return model
 
     @handle_api_error_response
     def update_model(
         self,
         model_name: str,
         project_name: str,
         info: Optional[ModelInfo] = None,
@@ -219,72 +295,120 @@
             data=body,
         )
         logger.info('Model[%s/%s] - Updated model', project_name, model_name)
 
         return Model.deserialize(APIResponseHandler(response))
 
     @handle_api_error_response
-    def delete_model(self, model_name: str, project_name: str) -> None:
+    def delete_model(
+        self,
+        project_id: str = None,
+        model_id: str = None,
+        model_name: str = None,
+        project_name: str = None,
+    ) -> None:
         """
         Delete a model
 
+        :params model_id: Model name to be deleted
+        :params project_id: Project name to which the model belongs to.
         :params model_name: Model name to be deleted
         :params project_name: Project name to which the model belongs to.
 
         :returns: None
         """
+        project_name = project_id_compat(
+            project_id=project_id, project_name=project_name
+        )
+
+        model_name = model_id_compat(
+            model_id=model_id,
+            model_name=model_name,
+        )
         logger.info('Deleting model %s from %s project', model_name, project_name)
         self.client.delete(
             url=f'models/{self.organization_name}:{project_name}:{model_name}',
         )
         logger.info('Deleted model %s from %s project', model_name, project_name)
 
     @handle_api_error_response
     def add_model_surrogate(
         self,
-        model_name: str,
-        project_name: str,
+        project_id: str = None,
+        model_id: str = None,
         deployment_params: Optional[DeploymentParams] = None,
+        model_name: str = None,
+        project_name: str = None,
         wait: bool = True,
     ) -> str:
         """
         Add surrogate model to an existing model
+
+        :params project_id: Project name to which the model belongs to.
+        :params model_id: Model name to be added
         :param model_name: Model name
         :param project_name: Project name
         :param deployment_params: Model deployment parameters
         :param wait: Whether to wait for job to complete or return after submitting
             the job
         :return: Async job uuid
         """
+        project_name = project_id_compat(
+            project_id=project_id, project_name=project_name
+        )
+
+        model_name = model_id_compat(
+            model_id=model_id,
+            model_name=model_name,
+        )
         return self._deploy_surrogate_model(
             model_name=model_name,
             project_name=project_name,
             deployment_params=deployment_params,
             wait=wait,
             update=False,
         )
 
     @check_version(version_expr='>=23.1.0')
     @handle_api_error_response
     def update_model_surrogate(
         self,
-        model_name: str,
-        project_name: str,
+        project_id: str = None,
+        model_id: str = None,
         deployment_params: Optional[DeploymentParams] = None,
+        is_sync: bool = True,
+        model_name: str = None,
+        project_name: str = None,
         wait: bool = True,
     ) -> str:
         """
         Re-generate surrogate model
+
+        :params project_id: Project name to which the model belongs to.
+        :params model_id: Model name to be updated
         :param model_name: Model name
+        :param is_sync: Whether to wait for job to complete or return after submitting
+            the job
         :param project_name: Project name
         :param deployment_params: Model deployment parameters
         :param wait: Whether to wait for job to complete or return after submitting
             the job
+
         :return: Async job uuid
         """
+        project_name = project_id_compat(
+            project_id=project_id, project_name=project_name
+        )
+
+        model_name = model_id_compat(
+            model_id=model_id,
+            model_name=model_name,
+        )
+
+        wait = is_sync_id_compat(is_sync=is_sync, wait=wait)
         return self._deploy_surrogate_model(
             model_name=model_name,
             project_name=project_name,
             deployment_params=deployment_params,
             wait=wait,
             update=True,
         )
@@ -425,57 +549,97 @@
             self.wait_for_job(uuid=job_uuid, job_name=job_name)  # noqa
 
         return job_uuid
 
     @handle_api_error_response
     def add_model_artifact(
         self,
-        model_name: str,
-        project_name: str,
-        artifact_dir: str,
+        project_id: str = None,
+        model_id: str = None,
+        model_dir: str = None,
         deployment_params: Optional[DeploymentParams] = None,
+        model_name: str = None,
+        project_name: str = None,
+        artifact_dir: str = None,
         wait: bool = True,
     ) -> str:
         """
         Add model artifact to an existing model
+
+        :params project_id: Project name to which the model belongs to.
+        :params model_id: Model name to be added
+        :param model_dir: Model artifact directory
         :param model_name: Model name
         :param project_name: Project name
         :param artifact_dir: Model artifact directory
         :param deployment_params: Model deployment parameters
         :param wait: Whether to wait for async job to finish or return
         :return: Async job uuid
         """
+        project_name = project_id_compat(
+            project_id=project_id, project_name=project_name
+        )
+
+        model_name = model_id_compat(
+            model_id=model_id,
+            model_name=model_name,
+        )
+        artifact_dir = model_dir_compat(
+            model_dir=model_dir,
+            artifact_dir=artifact_dir,
+        )
         return self._deploy_model_artifact(
             project_name=project_name,
             model_name=model_name,
             artifact_dir=artifact_dir,
             deployment_params=deployment_params,
             wait=wait,
             update=False,
         )
 
     @check_version(version_expr='>=22.12.0')
     @handle_api_error_response
     def update_model_artifact(
         self,
-        model_name: str,
-        project_name: str,
-        artifact_dir: str,
+        project_id: str = None,
+        model_id: str = None,
+        model_dir: str = None,
         deployment_params: Optional[DeploymentParams] = None,
+        is_sync: bool = True,
+        model_name: str = None,
+        project_name: str = None,
+        artifact_dir: str = None,
         wait: bool = True,
     ) -> str:
         """
         Update model artifact of an existing model
+
+        :params project_id: Project name to which the model belongs to.
+        :params model_id: Model name to be added
+        :param model_dir: Model artifact directory
         :param model_name: Model name
         :param project_name: Project name
         :param artifact_dir: Model artifact directory
         :param deployment_params: Model deployment parameters
         :param wait: Whether to wait for async job to finish or return
         :return: Async job uuid
         """
+        project_name = project_id_compat(
+            project_id=project_id, project_name=project_name
+        )
+
+        model_name = model_id_compat(
+            model_id=model_id,
+            model_name=model_name,
+        )
+        artifact_dir = model_dir_compat(
+            model_dir=model_dir,
+            artifact_dir=artifact_dir,
+        )
+        wait = is_sync_id_compat(is_sync=is_sync, wait=wait)
         return self._deploy_model_artifact(
             project_name=project_name,
             model_name=model_name,
             artifact_dir=artifact_dir,
             deployment_params=deployment_params,
             wait=wait,
             update=True,
@@ -490,7 +654,36 @@
 
         self.update_model(
             model_name=model_name,
             project_name=project_name,
             info=model_info,
             file_list=file_list,
         )
+
+    @handle_api_error_response
+    def download_artifacts(self, project_name: str, model_name: str, output_dir: Path):
+        """
+        download the model binary, package.py and model.yaml to the given
+        output dir.
+
+        :param project_name: Project name
+        :param model_name: Model name
+        :param output_dir: output directory
+        :return: None
+        """
+
+        if output_dir.exists():
+            raise ValueError(f'output dir already exists {output_dir}')
+
+        model_id = f'{self.organization_name}:{project_name}:{model_name}'
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            # Download tar file
+            tar_file_path = os.path.join(tmp_dir, 'artifact.tar')
+
+            with self.client.get(url=f'models/{model_id}/download-artifacts') as r:
+                r.raise_for_status()
+                with open(tar_file_path, mode='wb') as f:
+                    for chunk in r.iter_content(chunk_size=8192):
+                        if chunk:
+                            f.write(chunk)
+            os.makedirs(output_dir, exist_ok=True)
+            shutil.unpack_archive(tar_file_path, extract_dir=output_dir, format='tar')
```

### Comparing `fiddler-client-2.0.0.dev6/fiddler/v2/api/project_mixin.py` & `fiddler-client-2.0.0.dev7/fiddler/v2/api/project_mixin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from http import HTTPStatus
 from typing import List
 
 from pydantic import parse_obj_as
 
 from fiddler.libs.http_client import RequestClient
-from fiddler.utils import logging
+from fiddler.utils.logger import get_logger
 from fiddler.v2.schema.project import Project
+from fiddler.v2.utils.compatibility_helpers import project_id_compat
 from fiddler.v2.utils.decorators import handle_api_error_response
 from fiddler.v2.utils.response_handler import (
     APIResponseHandler,
     PaginatedResponseHandler,
 )
 
-logger = logging.getLogger(__name__)
+logger = get_logger(__name__)
 
 
 class ProjectMixin:
     client: RequestClient
     organization_name: str
 
     @handle_api_error_response
@@ -45,23 +46,26 @@
         """List the ids of all projects in the organization.
 
         :returns: List of strings containing the ids of each project.
         """
         projects = self.get_projects()
         return [p.name for p in projects]
 
-
     @handle_api_error_response
-    def delete_project(self, project_name: str) -> None:
+    def delete_project(self, project_id: str = None, project_name: str = None) -> None:
         """
         Delete a project
 
+        :params project_id: Name of the project to delete
         :params project_name: Name of the project to delete
         :returns: None
         """
+        project_name = project_id_compat(
+            project_id=project_id, project_name=project_name
+        )
         response = self.client.delete(
             url=f'projects/{self.organization_name}:{project_name}'
         )
         if response.status_code == HTTPStatus.OK:
             logger.info(f'{project_name} deleted successfully.')
         else:
             # @TODO: Handle non 200 status response
```

### Comparing `fiddler-client-2.0.0.dev6/fiddler/v2/constants.py` & `fiddler-client-2.0.0.dev7/fiddler/constants.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import enum
 
+DATASET_FIDDLER_ID = '__fiddler_id'
+ONE_LINE_PRINT = '¡í€'
+TIMESTAMP_FORMAT = '%Y-%m-%d %H:%M:%S.%f'
+
 # Headers
 CONTENT_TYPE_HEADER_KEY = 'Content-Type'
 CONTENT_TYPE_OCTET_STREAM = 'application/octet-stream'
 CONTENT_TYPE_OCTET_STREAM_HEADER = {CONTENT_TYPE_HEADER_KEY: CONTENT_TYPE_OCTET_STREAM}
 
 # Multi-part upload
 MULTI_PART_UPLOAD_SIZE_THRESHOLD = 5 * 1024 * 1024  # 5MB in bytes
@@ -11,14 +15,36 @@
 
 # File processor
 SUPPORTABLE_FILE_EXTENSIONS = ['.csv']
 CSV_EXTENSION = 'csv'
 
 # Version
 CURRENT_API_VERSION = 'v2'
+MIN_SERVER_VERSION = '23.4.0'
+
+COMPAT_MAPPING = {
+    'project_id': 'project_name',
+    'model_id': 'model_name',
+    'dataset_id': 'dataset_name',
+    'baseline_id': 'baseline_name',
+    'alert_id': 'alert_name',
+}
+
+
+class bcolors:
+    HEADER = '\033[95m'
+    OKBLUE = '\033[94m'
+    OKCYAN = '\033[96m'
+    OKGREEN = '\033[92m'
+    WARNING = '\033[93m'
+    FAIL = '\033[91m'
+    ENDCOLOR = '\033[0m'
+    BOLD = '\033[1m'
+    UNDERLINE = '\033[4m'
+
 
 @enum.unique
 class FiddlerTimestamp(str, enum.Enum):
     """Supported timestamp formats for events published to Fiddler"""
 
     EPOCH_MILLISECONDS = 'epoch milliseconds'
     EPOCH_SECONDS = 'epoch seconds'
@@ -28,14 +54,15 @@
 
 
 @enum.unique
 class FileType(str, enum.Enum):
     """Supported file types for ingestion"""
 
     CSV = '.csv'
+    PARQUET = '.parquet'
 
 
 @enum.unique
 class ServerDeploymentMode(str, enum.Enum):
     F1 = 'f1'
     F2 = 'f2'
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fiddler-client-2.0.0.dev6/fiddler/v2/schema/alert.py` & `fiddler-client-2.0.0.dev7/fiddler/v2/schema/alert.py`

 * *Files 5% similar despite different names*

```diff
@@ -144,27 +144,27 @@
     compare_to: CompareTo
     baseline_name: Optional[str]
     compare_period: Optional[ComparePeriod]
     warning_threshold: Optional[float]
     critical_threshold: float
     condition: AlertCondition
     time_bucket: BinSize
-    notifications: Optional[Dict[str, Dict[str, Any]]]
+    notifications: Optional[Dict[str, Any]]
 
 
 class AlertRule(BaseDataSchema):
     alert_rule_uuid: str = Field(alias='uuid')
     organization_name: str
-    project_id: str = Field(alias='project_name')
-    model_id: str = Field(alias='model_name')
+    project_name: str = Field(alias='project_name')
+    model_name: str = Field(alias='model_name')
     name: Optional[str]
     alert_type: AlertType
     metric: Metric
     columns: Optional[List[str]] = Field(alias='feature_names')
-    baseline_id: Optional[str] = Field(alias='baseline_name')
+    baseline_name: Optional[str] = Field(alias='baseline_name')
     priority: Priority
     compare_to: CompareTo
     compare_period: Optional[ComparePeriod]
     warning_threshold: Optional[float]
     critical_threshold: float
     condition: AlertCondition
     bin_size: BinSize = Field(alias='time_bucket')
```

### Comparing `fiddler-client-2.0.0.dev6/fiddler/v2/schema/dataset.py` & `fiddler-client-2.0.0.dev7/fiddler/v2/schema/dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Dict, List, Optional
 
+from fiddler.constants import FileType, UploadType
 from fiddler.core_objects import DatasetInfo
-from fiddler.exceptions import FiddlerAPIHTTPException
-from fiddler.v2.constants import FileType, UploadType
+from fiddler.exceptions import HttpException
 from fiddler.v2.utils.response_handler import APIResponseHandler
 
 
 class Dataset:
     def __init__(
             self,
         id: int,
@@ -27,15 +27,15 @@
 
     @classmethod
     def deserialize(cls, response: APIResponseHandler):
         data = response.get_data()
         try:
             return cls.from_dict(data)
         except KeyError as ke:
-            raise FiddlerAPIHTTPException(
+            raise HttpException(
                 status_code=response.status_code,
                 error_code=response.status_code,
                 message=f'Invalid response content. {str(ke)} in the response.',
                 errors=[],
             )
 
     @classmethod
```

### Comparing `fiddler-client-2.0.0.dev6/fiddler/v2/schema/events.py` & `fiddler-client-2.0.0.dev7/fiddler/v2/schema/events.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Optional
 
-from fiddler.v2.constants import FiddlerTimestamp, FileType, UploadType
+from fiddler.constants import FiddlerTimestamp, FileType, UploadType
 from fiddler.v2.schema.base import BaseDataSchema
 
 
 class EventsIngest(BaseDataSchema):
     file_name: List[str]
     batch_id: Optional[str] = None
     events_schema: Optional[dict] = None
```

### Comparing `fiddler-client-2.0.0.dev6/fiddler/v2/schema/model_deployment.py` & `fiddler-client-2.0.0.dev7/fiddler/v2/schema/model_deployment.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev6/fiddler/v2/utils/helpers.py` & `fiddler-client-2.0.0.dev7/fiddler/v2/utils/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 import yaml
 
+from fiddler.constants import FileType
 from fiddler.core_objects import ModelInfo
 from fiddler.exceptions import NotSupported
 from fiddler.v2.schema.server_info import Version
 
 
 def match_semver(version: Optional[Version], match_expr: str) -> bool:
     """
@@ -22,17 +23,15 @@
     if version.prerelease:
         return Version(version.major, version.minor, version.patch).match(match_expr)
 
     return version.match(match_expr)
 
 
 def raise_not_supported(
-    compatible_client_version: str,
-    client_version: str,
-    server_version: Version
+    compatible_client_version: str, client_version: str, server_version: Version
 ):
     """
     Raise error when client version is not compatible with the server version.
     :param compatible_client_version: Max client version supported for the server
     :param client_version: client version
     :param server_version: server version
     :return: NotSupported error
@@ -68,7 +67,16 @@
     """
     yaml_file = artifact_dir / 'model.yaml'
     if not yaml_file.is_file():
         return None
 
     with yaml_file.open() as f:
         return ModelInfo.from_dict(yaml.safe_load(f))
+
+
+def map_extension_to_file_type(file_path: Path) -> str:
+    file_extension = file_path.suffix
+    if file_extension == '.csv':
+        return FileType.CSV
+
+    if file_extension == '.parquet':
+        return FileType.PARQUET
```

### Comparing `fiddler-client-2.0.0.dev6/fiddler/v2/utils/response_handler.py` & `fiddler-client-2.0.0.dev7/fiddler/v2/utils/response_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 try:
     from simplejson import JSONDecodeError
 except ImportError:
     from json import JSONDecodeError
 
 import requests
 
-from fiddler.utils import logging
-from fiddler.exceptions import FiddlerAPIHTTPException
+from fiddler.exceptions import HttpException
+from fiddler.utils.logger import get_logger
 
-logger = logging.getLogger(__name__)
+logger = get_logger(__name__)
 
 
 class BaseResponseHandler:
     def __init__(self, response: requests.Response) -> None:
         self.response = response
         logger.debug(self.response.content)
 
     def get_data(self) -> Dict[str, Any]:
         try:
             dict_response = self.response.json().get('data')
         except JSONDecodeError:
-            raise FiddlerAPIHTTPException(
+            raise HttpException(
                 status_code=self.response.status_code,
                 error_code=self.response.status_code,
                 message=f'Invalid response content-type. {self.response.status_code}:{self.response.content}',
                 errors=[],
             )
         return dict_response
```

### Comparing `fiddler-client-2.0.0.dev6/fiddler/v2/validators/dataset_validator.py` & `fiddler-client-2.0.0.dev7/fiddler/v2/validators/dataset_validator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-import logging
 from pathlib import Path
 from typing import Dict
 
 import pandas as pd
 
+from fiddler.constants import FileType
 from fiddler.core_objects import DatasetInfo
+from fiddler.utils.logger import get_logger
+from fiddler.v2.utils.helpers import map_extension_to_file_type
 
-LOG = logging.getLogger(__name__)
+LOG = get_logger(__name__)
 
 NUM_ROWS = 1
 JUST_THE_HEADER = 0
 
 
 def validate_dataset_info(info: DatasetInfo) -> None:
     if not isinstance(info, DatasetInfo):
@@ -22,30 +24,37 @@
 
 def validate_dataset_shape(files: Dict[str, Path]) -> None:
     rows = 0
     columns = 0
 
     for _, file_path in files.items():
         try:
-            df = pd.read_csv(file_path, nrows=NUM_ROWS)
+            file_type = map_extension_to_file_type(file_path)
+            if file_type == FileType.CSV:
+                df = pd.read_csv(file_path, nrows=NUM_ROWS)
+            elif file_type == FileType.PARQUET:
+                df = pd.read_parquet(file_path)
             rows, columns = df.shape
         except pd.errors.EmptyDataError:
             rows = 0
             columns = 0
 
         # empty checks.
         if columns == 0:
             raise ValueError('No columns found in dataset provided.')
         if rows == 0:
             raise ValueError('No rows found in dataset provided.')
 
 
 def validate_dataset_columns(dataset_info: DatasetInfo, file_path: Path) -> None:
-    # we can safely assume that file_path points to a csv file
-    df = pd.read_csv(file_path, nrows=JUST_THE_HEADER)
+    file_type = map_extension_to_file_type(file_path)
+    if file_type == FileType.CSV:
+        df = pd.read_csv(file_path, nrows=JUST_THE_HEADER)
+    elif file_type == FileType.PARQUET:
+        df = pd.read_parquet(file_path)
 
     missing_cols = set(col.name for col in dataset_info.columns) - set(
         df.columns.str.strip()
     )
     if len(missing_cols) > 0:
         LOG.warning(
             'Following columns are missing from uploaded dataset, '
```

### Comparing `fiddler-client-2.0.0.dev6/fiddler/validator.py` & `fiddler-client-2.0.0.dev7/fiddler/utils/validator.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev6/fiddler_client.egg-info/PKG-INFO` & `fiddler-client-2.0.0.dev7/fiddler_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 2.0.0.dev6
+Version: 2.0.0.dev7
 Summary: Python client for Fiddler Service
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 License: UNKNOWN
 Description: Fiddler Client
         =============
         
@@ -42,15 +42,27 @@
               - unshare_project
               - share_project
               - process_avro
               - process_csv
           - #### **New Features**
             - Add `monitor_components` as an attribute of `CustomFeature`. Default to `False`
             - Remove `column` as a parameter in `add_alert_rule` and `get_alert_rules` functions
-            
+        
+        ### 1.8.2
+          - #### **Modifications**
+            - Fixed a bug where `min` and `max` for columns of type `float` in `dataset_info` are cast into `int` after uploaded
+        
+        ### 1.8.1
+          - #### **Modifications**
+            - Fixed a bug wherein null string was going in request body if body wasn't specified.
+            - Fix `categorical_target_class_details` when passed as an array
+            - Fix a bug where `fdl.ModelInputType.TEXT` were not being accepted properly
+            - Fix `categorical_target_class_details` when passed as an empty list
+        
+        
         ### 1.8.0
           - #### **Modifications**
             - Add new alert type -  `statistic` for setting alerts
             - Add `target_class_order` as a required field of `ModelInfo` object when `model_task` is `MULTICLASS_CLASSIFICATION`,
               `RANKING` or `BINARY_CLASSIFICATION`. Only applies for `BINARY_CLASSIFICATION` when target column is of type `CATEGORY`
             - Add `columns` as a parameter in `add_alert_rule` and `get_alert_rules` functions
             - Add deprecation warning for `column` as a parameter in `add_alert_rule` and `get_alert_rules` functions
```

### Comparing `fiddler-client-2.0.0.dev6/fiddler_client.egg-info/SOURCES.txt` & `fiddler-client-2.0.0.dev7/fiddler_client.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 MANIFEST.in
 PUBLIC.md
 README.md
 setup.py
 fiddler/__init__.py
 fiddler/_version.py
-fiddler/client.py
 fiddler/connection.py
 fiddler/constants.py
 fiddler/core_objects.py
-fiddler/dataset.py
 fiddler/exceptions.py
 fiddler/fiddler_api.py
-fiddler/model.py
-fiddler/monitoring_validator.py
-fiddler/project.py
-fiddler/validator.py
 fiddler/assets/__init__.py
 fiddler/assets/pg_reserved_words.py
 fiddler/libs/__init__.py
 fiddler/libs/http_client.py
 fiddler/packtools/__init__.py
 fiddler/packtools/gem.py
 fiddler/packtools/keras_ig_helpers.py
 fiddler/packtools/project_attributions_helpers.py
 fiddler/packtools/template_model.py
+fiddler/schemas/__init__.py
+fiddler/schemas/custom_features.py
+fiddler/schemas/model_schema.py
+fiddler/schemas/model_spec.py
+fiddler/schemas/model_task_params.py
+fiddler/schemas/xai_params.py
 fiddler/utils/__init__.py
 fiddler/utils/exceptions.py
 fiddler/utils/formatting.py
 fiddler/utils/general_checks.py
 fiddler/utils/helper.py
-fiddler/utils/logging.py
-fiddler/utils/pandas.py
+fiddler/utils/logger.py
+fiddler/utils/pandas_helper.py
+fiddler/utils/validator.py
 fiddler/v2/__init__.py
-fiddler/v2/constants.py
 fiddler/v2/api/__init__.py
 fiddler/v2/api/alert_mixin.py
 fiddler/v2/api/api.py
 fiddler/v2/api/baseline_mixin.py
+fiddler/v2/api/compatibility_mixin.py
 fiddler/v2/api/dataset_mixin.py
 fiddler/v2/api/events_mixin.py
 fiddler/v2/api/explainability_mixin.py
 fiddler/v2/api/helpers.py
+fiddler/v2/api/infer_schema_mixin.py
 fiddler/v2/api/job_mixin.py
 fiddler/v2/api/model_artifact_deploy.py
 fiddler/v2/api/model_deployment_mixin.py
 fiddler/v2/api/model_mixin.py
 fiddler/v2/api/project_mixin.py
 fiddler/v2/schema/__init__.py
 fiddler/v2/schema/alert.py
@@ -55,20 +57,48 @@
 fiddler/v2/schema/job.py
 fiddler/v2/schema/model.py
 fiddler/v2/schema/model_deployment.py
 fiddler/v2/schema/project.py
 fiddler/v2/schema/server_info.py
 fiddler/v2/schema/user.py
 fiddler/v2/utils/__init__.py
+fiddler/v2/utils/compatibility_helpers.py
 fiddler/v2/utils/decorators.py
 fiddler/v2/utils/helpers.py
 fiddler/v2/utils/response_handler.py
 fiddler/v2/utils/validations.py
 fiddler/v2/validators/__init__.py
 fiddler/v2/validators/dataset_validator.py
 fiddler_client.egg-info/PKG-INFO
 fiddler_client.egg-info/SOURCES.txt
 fiddler_client.egg-info/dependency_links.txt
 fiddler_client.egg-info/requires.txt
 fiddler_client.egg-info/top_level.txt
 tests/__init__.py
-tests/test_fiddler_api.py
+tests/test_infer_model_schema.py
+tests/test_object_inference.py
+tests/utils.py
+tests/fiddler/__init__.py
+tests/fiddler/utils/__init__.py
+tests/fiddler/utils/test_general_checks.py
+tests/fiddler/utils/test_pandas.py
+tests/fiddler/utils/tests_utils.py
+tests/v2/__init__.py
+tests/v2/base.py
+tests/v2/helper.py
+tests/v2/test_add_model.py
+tests/v2/test_alert.py
+tests/v2/test_baseline.py
+tests/v2/test_check_version_decorator.py
+tests/v2/test_custom_features.py
+tests/v2/test_dataset_api.py
+tests/v2/test_events_api.py
+tests/v2/test_exceptions.py
+tests/v2/test_explainability_apis.py
+tests/v2/test_file_upload.py
+tests/v2/test_helpers.py
+tests/v2/test_job.py
+tests/v2/test_model.py
+tests/v2/test_project.py
+tests/v2/test_response_handler.py
+tests/v2/test_upload_dataset.py
+tests/v2/test_validations.py
```

### Comparing `fiddler-client-2.0.0.dev6/setup.py` & `fiddler-client-2.0.0.dev7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,26 +25,21 @@
     long_description_content_type='text/markdown',
     url='https://fiddler.ai',
     packages=setuptools.find_packages(),
     install_requires=[
         'pip>=21.0',
         'requests<3',
         'requests-toolbelt',
-        'pandas>=1.2.5,<1.6',
-        'pyyaml',
-        'packaging',
-        'deepdiff',
-        'importlib-resources',
-        'Werkzeug',
-        'deprecation==2.1.0',
-        'pydantic>=1.9.0',
-        'urllib3<2',
+        'pandas>=1.2.5,<=1.5.3',
+        'pydantic==1.9.0',
         'deprecated==1.2.13',
         'semver>=2,<3',
         'tqdm==4.64.1',
+        'simplejson>=3.17.0',
+        'pyarrow>=12.0.1',
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
     ],
     python_requires='>3.6.3',
```

