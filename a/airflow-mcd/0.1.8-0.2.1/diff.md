# Comparing `tmp/airflow_mcd-0.1.8.tar.gz` & `tmp/airflow_mcd-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/airflow_mcd-0.1.8.tar", last modified: Wed Jul 26 16:15:43 2023, max compression
+gzip compressed data, was "dist/airflow_mcd-0.2.1.tar", last modified: Thu Jul 27 15:00:59 2023, max compression
```

## Comparing `airflow_mcd-0.1.8.tar` & `airflow_mcd-0.2.1.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.105794 airflow_mcd-0.1.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.101794 airflow_mcd-0.1.8/.circleci/
--rw-r--r--   0 root         (0) root         (0)      168 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/.circleci/README
--rw-r--r--   0 root         (0) root         (0)     3102 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/.circleci/config.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.101794 airflow_mcd-0.1.8/.circleci/trufflehog_config/
--rw-r--r--   0 root         (0) root         (0)      377 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/.circleci/trufflehog_config/allowlist.json
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/.coveragerc
--rw-r--r--   0 root         (0) root         (0)     1818 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/.gitignore
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1129 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/Makefile
--rw-r--r--   0 root         (0) root         (0)     9568 2023-07-26 16:15:43.105794 airflow_mcd-0.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      958 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/README-dev.md
--rw-r--r--   0 root         (0) root         (0)     8755 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.101794 airflow_mcd-0.1.8/airflow_mcd/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/airflow_mcd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.101794 airflow_mcd-0.1.8/airflow_mcd/callbacks/
--rw-r--r--   0 root         (0) root         (0)     7042 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/airflow_mcd/callbacks/client.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/airflow_mcd/callbacks/mcd_callbacks.py
--rw-r--r--   0 root         (0) root         (0)     6336 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/airflow_mcd/callbacks/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.101794 airflow_mcd-0.1.8/airflow_mcd/hooks/
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/airflow_mcd/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2784 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/airflow_mcd/hooks/session_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.101794 airflow_mcd-0.1.8/airflow_mcd/operators/
--rw-r--r--   0 root         (0) root         (0)       89 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/airflow_mcd/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/airflow_mcd/operators/base_operator.py
--rw-r--r--   0 root         (0) root         (0)     3895 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/airflow_mcd/operators/circuit_breaker_operators.py
--rw-r--r--   0 root         (0) root         (0)    15407 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/airflow_mcd/operators/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.101794 airflow_mcd-0.1.8/airflow_mcd.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9568 2023-07-26 16:15:43.000000 airflow_mcd-0.1.8/airflow_mcd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1137 2023-07-26 16:15:43.000000 airflow_mcd-0.1.8/airflow_mcd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 16:15:43.000000 airflow_mcd-0.1.8/airflow_mcd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-26 16:15:43.000000 airflow_mcd-0.1.8/airflow_mcd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-26 16:15:43.000000 airflow_mcd-0.1.8/airflow_mcd.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.101794 airflow_mcd-0.1.8/examples/
--rw-r--r--   0 root         (0) root         (0)     2050 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/examples/sample_circuit_dag.py
--rw-r--r--   0 root         (0) root         (0)       45 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/requirements-ci.txt
--rw-r--r--   0 root         (0) root         (0)      195 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-07-26 16:15:43.105794 airflow_mcd-0.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1483 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.101794 airflow_mcd-0.1.8/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.101794 airflow_mcd-0.1.8/tests/callbacks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/tests/callbacks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15028 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/tests/callbacks/test_callbacks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.101794 airflow_mcd-0.1.8/tests/hooks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/tests/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3780 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/tests/hooks/test_session_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.105794 airflow_mcd-0.1.8/tests/operators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/tests/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      719 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/tests/operators/test_base_op.py
--rw-r--r--   0 root         (0) root         (0)     5843 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/tests/operators/test_circuit_breaker_op.py
--rw-r--r--   0 root         (0) root         (0)     1529 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/tests/operators/test_dbt_cli_config.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/tests/operators/test_dbt_default_config_provider.py
--rw-r--r--   0 root         (0) root         (0)    21136 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/tests/operators/test_dbt_operator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.676613 airflow_mcd-0.2.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.672613 airflow_mcd-0.2.1/.circleci/
+-rw-r--r--   0 root         (0) root         (0)      168 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/.circleci/README
+-rw-r--r--   0 root         (0) root         (0)     3102 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/.circleci/config.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.672613 airflow_mcd-0.2.1/.circleci/trufflehog_config/
+-rw-r--r--   0 root         (0) root         (0)      377 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/.circleci/trufflehog_config/allowlist.json
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/Makefile
+-rw-r--r--   0 root         (0) root         (0)     9590 2023-07-27 15:00:59.676613 airflow_mcd-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2000 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/README-dev.md
+-rw-r--r--   0 root         (0) root         (0)     8777 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.672613 airflow_mcd-0.2.1/airflow_mcd/
+-rw-r--r--   0 root         (0) root         (0)      458 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/airflow_mcd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.672613 airflow_mcd-0.2.1/airflow_mcd/callbacks/
+-rw-r--r--   0 root         (0) root         (0)     7042 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/airflow_mcd/callbacks/client.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/airflow_mcd/callbacks/mcd_callbacks.py
+-rw-r--r--   0 root         (0) root         (0)     6336 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/airflow_mcd/callbacks/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.672613 airflow_mcd-0.2.1/airflow_mcd/hooks/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/airflow_mcd/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4492 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/airflow_mcd/hooks/session_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.672613 airflow_mcd-0.2.1/airflow_mcd/operators/
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/airflow_mcd/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/airflow_mcd/operators/base_operator.py
+-rw-r--r--   0 root         (0) root         (0)     3895 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/airflow_mcd/operators/circuit_breaker_operators.py
+-rw-r--r--   0 root         (0) root         (0)    15407 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/airflow_mcd/operators/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.672613 airflow_mcd-0.2.1/airflow_mcd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9590 2023-07-27 15:00:59.000000 airflow_mcd-0.2.1/airflow_mcd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-07-27 15:00:59.000000 airflow_mcd-0.2.1/airflow_mcd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 15:00:59.000000 airflow_mcd-0.2.1/airflow_mcd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-27 15:00:59.000000 airflow_mcd-0.2.1/airflow_mcd.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-27 15:00:59.000000 airflow_mcd-0.2.1/airflow_mcd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-27 15:00:59.000000 airflow_mcd-0.2.1/airflow_mcd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.672613 airflow_mcd-0.2.1/examples/
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/examples/sample_circuit_dag.py
+-rw-r--r--   0 root         (0) root         (0)       45 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/requirements-ci.txt
+-rw-r--r--   0 root         (0) root         (0)      195 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-07-27 15:00:59.676613 airflow_mcd-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1579 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.672613 airflow_mcd-0.2.1/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.672613 airflow_mcd-0.2.1/tests/callbacks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/tests/callbacks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15028 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/tests/callbacks/test_callbacks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.672613 airflow_mcd-0.2.1/tests/hooks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/tests/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/tests/hooks/test_session_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.676613 airflow_mcd-0.2.1/tests/operators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/tests/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      719 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/tests/operators/test_base_op.py
+-rw-r--r--   0 root         (0) root         (0)     5843 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/tests/operators/test_circuit_breaker_op.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/tests/operators/test_dbt_cli_config.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/tests/operators/test_dbt_default_config_provider.py
+-rw-r--r--   0 root         (0) root         (0)    21136 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/tests/operators/test_dbt_operator.py
```

### Comparing `airflow_mcd-0.1.8/.circleci/config.yml` & `airflow_mcd-0.2.1/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.8/.gitignore` & `airflow_mcd-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.8/LICENSE` & `airflow_mcd-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.8/Makefile` & `airflow_mcd-0.2.1/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -25,13 +25,16 @@
 	@# These suppressed warnings are all from the Airflow package :/.
 	export DEBUG=True; PYTHONWARNINGS="ignore::DeprecationWarning" PYTHONWARNINGS="ignore::FutureWarning" \
 		nosetests ./tests --with-coverage --cover-package=$(PY_FRIENDLY_PACKAGE_NAME) --with-xunit
 
 install-with-tests: install
 	. $(ENVIRONMENT_NAME)/bin/activate; $(MAKE) test
 
-distribute: install
+package: install
 	. $(ENVIRONMENT_NAME)/bin/activate; \
 	pip install -r requirements-ci.txt; \
-	python setup.py sdist bdist_wheel; \
+	python setup.py sdist bdist_wheel;
+
+distribute: package
+	. $(ENVIRONMENT_NAME)/bin/activate; \
 	twine check dist/*; \
 	twine upload --non-interactive dist/*
```

### Comparing `airflow_mcd-0.1.8/PKG-INFO` & `airflow_mcd-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow_mcd
-Version: 0.1.8
+Version: 0.2.1
 Summary: Monte Carlo's Apache Airflow Provider
 Home-page: https://www.montecarlodata.com/
 Author: Monte Carlo Data, Inc
 Author-email: info@montecarlodata.com
 License: Apache Software License (Apache 2.0)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -36,15 +36,15 @@
 This package can be added like any other python dependency to Airflow (e.g. via `requirements.txt`).
 
 ## Basic usage
 
 ### Callbacks
 
 Sends a webhook back to Monte Carlo upon an event in Airflow. [Detailed examples and documentation here]
-(https://docs.getmontecarlo.com/edit/airflow-v2). Callbacks are at the DAG or Task level.
+(https://docs.getmontecarlo.com/docs/airflow-incidents-dags-and-tasks). Callbacks are at the DAG or Task level.
 
 To import: `from airflow_mcd.callbacks import mcd_callbacks`
 
 #### Broad Callbacks
 
 if you don't have existing callbacks, these provide all-in-one callbacks:
```

### Comparing `airflow_mcd-0.1.8/README.md` & `airflow_mcd-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 This package can be added like any other python dependency to Airflow (e.g. via `requirements.txt`).
 
 ## Basic usage
 
 ### Callbacks
 
 Sends a webhook back to Monte Carlo upon an event in Airflow. [Detailed examples and documentation here]
-(https://docs.getmontecarlo.com/edit/airflow-v2). Callbacks are at the DAG or Task level.
+(https://docs.getmontecarlo.com/docs/airflow-incidents-dags-and-tasks). Callbacks are at the DAG or Task level.
 
 To import: `from airflow_mcd.callbacks import mcd_callbacks`
 
 #### Broad Callbacks
 
 if you don't have existing callbacks, these provide all-in-one callbacks:
```

### Comparing `airflow_mcd-0.1.8/airflow_mcd/callbacks/client.py` & `airflow_mcd-0.2.1/airflow_mcd/callbacks/client.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.8/airflow_mcd/callbacks/mcd_callbacks.py` & `airflow_mcd-0.2.1/airflow_mcd/callbacks/mcd_callbacks.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.8/airflow_mcd/callbacks/utils.py` & `airflow_mcd-0.2.1/airflow_mcd/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.8/airflow_mcd/operators/base_operator.py` & `airflow_mcd-0.2.1/airflow_mcd/operators/base_operator.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.8/airflow_mcd/operators/circuit_breaker_operators.py` & `airflow_mcd-0.2.1/airflow_mcd/operators/circuit_breaker_operators.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.8/airflow_mcd/operators/dbt.py` & `airflow_mcd-0.2.1/airflow_mcd/operators/dbt.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.8/airflow_mcd.egg-info/PKG-INFO` & `airflow_mcd-0.2.1/airflow_mcd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-mcd
-Version: 0.1.8
+Version: 0.2.1
 Summary: Monte Carlo's Apache Airflow Provider
 Home-page: https://www.montecarlodata.com/
 Author: Monte Carlo Data, Inc
 Author-email: info@montecarlodata.com
 License: Apache Software License (Apache 2.0)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -36,15 +36,15 @@
 This package can be added like any other python dependency to Airflow (e.g. via `requirements.txt`).
 
 ## Basic usage
 
 ### Callbacks
 
 Sends a webhook back to Monte Carlo upon an event in Airflow. [Detailed examples and documentation here]
-(https://docs.getmontecarlo.com/edit/airflow-v2). Callbacks are at the DAG or Task level.
+(https://docs.getmontecarlo.com/docs/airflow-incidents-dags-and-tasks). Callbacks are at the DAG or Task level.
 
 To import: `from airflow_mcd.callbacks import mcd_callbacks`
 
 #### Broad Callbacks
 
 if you don't have existing callbacks, these provide all-in-one callbacks:
```

### Comparing `airflow_mcd-0.1.8/airflow_mcd.egg-info/SOURCES.txt` & `airflow_mcd-0.2.1/airflow_mcd.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 .circleci/README
 .circleci/config.yml
 .circleci/trufflehog_config/allowlist.json
 airflow_mcd/__init__.py
 airflow_mcd.egg-info/PKG-INFO
 airflow_mcd.egg-info/SOURCES.txt
 airflow_mcd.egg-info/dependency_links.txt
+airflow_mcd.egg-info/entry_points.txt
 airflow_mcd.egg-info/requires.txt
 airflow_mcd.egg-info/top_level.txt
 airflow_mcd/callbacks/client.py
 airflow_mcd/callbacks/mcd_callbacks.py
 airflow_mcd/callbacks/utils.py
 airflow_mcd/hooks/__init__.py
 airflow_mcd/hooks/session_hook.py
```

### Comparing `airflow_mcd-0.1.8/examples/sample_circuit_dag.py` & `airflow_mcd-0.2.1/examples/sample_circuit_dag.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.8/setup.py` & `airflow_mcd-0.2.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,9 +35,10 @@
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10'
     ],
     python_requires='>=3.7',
-    setup_requires=['setuptools', 'setuptools_scm']
+    setup_requires=['setuptools', 'setuptools_scm'],
+    entry_points=dict(apache_airflow_provider=["provider_info=airflow_mcd:get_provider_info"])
 )
```

### Comparing `airflow_mcd-0.1.8/tests/callbacks/test_callbacks.py` & `airflow_mcd-0.2.1/tests/callbacks/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.8/tests/hooks/test_session_hook.py` & `airflow_mcd-0.2.1/tests/hooks/test_session_hook.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.8/tests/operators/test_base_op.py` & `airflow_mcd-0.2.1/tests/operators/test_base_op.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.8/tests/operators/test_circuit_breaker_op.py` & `airflow_mcd-0.2.1/tests/operators/test_circuit_breaker_op.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.8/tests/operators/test_dbt_cli_config.py` & `airflow_mcd-0.2.1/tests/operators/test_dbt_cli_config.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.8/tests/operators/test_dbt_default_config_provider.py` & `airflow_mcd-0.2.1/tests/operators/test_dbt_default_config_provider.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.8/tests/operators/test_dbt_operator.py` & `airflow_mcd-0.2.1/tests/operators/test_dbt_operator.py`

 * *Files identical despite different names*

