# Comparing `tmp/seldonian_engine-0.8.2.tar.gz` & `tmp/seldonian_engine-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seldonian_engine-0.8.2.tar", last modified: Thu Jul 27 15:56:16 2023, max compression
+gzip compressed data, was "seldonian_engine-0.8.3.tar", last modified: Thu Jul 27 16:16:20 2023, max compression
```

## Comparing `seldonian_engine-0.8.2.tar` & `seldonian_engine-0.8.3.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 15:56:16.265778 seldonian_engine-0.8.2/
--rw-r--r--   0 ahoag      (501) staff       (20)     1527 2022-09-12 23:15:58.000000 seldonian_engine-0.8.2/LICENSE
--rw-r--r--   0 ahoag      (501) staff       (20)     2133 2023-07-27 15:56:16.265595 seldonian_engine-0.8.2/PKG-INFO
--rw-r--r--   0 ahoag      (501) staff       (20)     1642 2023-07-20 04:24:35.000000 seldonian_engine-0.8.2/README.md
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 15:56:16.244941 seldonian_engine-0.8.2/seldonian/
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 15:56:16.247495 seldonian_engine-0.8.2/seldonian/RL/
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 15:56:16.248573 seldonian_engine-0.8.2/seldonian/RL/Agents/
--rw-r--r--   0 ahoag      (501) staff       (20)     1733 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/RL/Agents/Agent.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 15:56:16.248929 seldonian_engine-0.8.2/seldonian/RL/Agents/Bases/
--rw-r--r--   0 ahoag      (501) staff       (20)     4537 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/RL/Agents/Bases/Fourier.py
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.2/seldonian/RL/Agents/Bases/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1043 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/RL/Agents/Discrete_Random_Agent.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 15:56:16.249678 seldonian_engine-0.8.2/seldonian/RL/Agents/Function_Approximators/
--rw-r--r--   0 ahoag      (501) staff       (20)      554 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/RL/Agents/Function_Approximators/Function_Approximator.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1333 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/RL/Agents/Function_Approximators/Linear_FA.py
--rw-r--r--   0 ahoag      (501) staff       (20)     2854 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/RL/Agents/Function_Approximators/Table.py
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.2/seldonian/RL/Agents/Function_Approximators/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     3054 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/RL/Agents/Parameterized_non_learning_softmax_agent.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 15:56:16.250301 seldonian_engine-0.8.2/seldonian/RL/Agents/Policies/
--rw-r--r--   0 ahoag      (501) staff       (20)     4906 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/RL/Agents/Policies/Policy.py
--rw-r--r--   0 ahoag      (501) staff       (20)     6459 2023-05-31 21:23:44.000000 seldonian_engine-0.8.2/seldonian/RL/Agents/Policies/Softmax.py
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.2/seldonian/RL/Agents/Policies/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.2/seldonian/RL/Agents/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)      794 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/RL/Agents/keyboard_gridworld.py
--rw-r--r--   0 ahoag      (501) staff       (20)      406 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/RL/Agents/mountain_car_rough_solution.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 15:56:16.250834 seldonian_engine-0.8.2/seldonian/RL/Env_Description/
--rw-r--r--   0 ahoag      (501) staff       (20)     2001 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/RL/Env_Description/Env_Description.py
--rw-r--r--   0 ahoag      (501) staff       (20)     2311 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/RL/Env_Description/Spaces.py
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.2/seldonian/RL/Env_Description/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     3698 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/RL/RL_generate_dataset_and_spec_file.py
--rw-r--r--   0 ahoag      (501) staff       (20)     2335 2023-05-31 21:23:44.000000 seldonian_engine-0.8.2/seldonian/RL/RL_model.py
--rw-r--r--   0 ahoag      (501) staff       (20)     6640 2023-07-27 15:51:46.000000 seldonian_engine-0.8.2/seldonian/RL/RL_runner.py
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.2/seldonian/RL/__init__.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 15:56:16.251947 seldonian_engine-0.8.2/seldonian/RL/environments/
--rw-r--r--   0 ahoag      (501) staff       (20)     1364 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/RL/environments/Environment.py
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.2/seldonian/RL/environments/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4075 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/RL/environments/gridworld.py
--rw-r--r--   0 ahoag      (501) staff       (20)     2352 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/RL/environments/mountaincar.py
--rw-r--r--   0 ahoag      (501) staff       (20)      984 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/RL/environments/n_step_mountaincar.py
--rw-r--r--   0 ahoag      (501) staff       (20)     2807 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/RL/environments/simglucose_env.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1196 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/RL/generate_gridworld_episodes.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1236 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/RL/generate_mountaincar_episodes.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1337 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/RL/generate_simglucose_episodes.py
--rw-r--r--   0 ahoag      (501) staff       (20)      615 2022-09-13 15:24:12.000000 seldonian_engine-0.8.2/seldonian/RL/hyperparams_and_settings.py
--rw-r--r--   0 ahoag      (501) staff       (20)     3991 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/RL/profiling_seldonian_RL.py
--rw-r--r--   0 ahoag      (501) staff       (20)       33 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/__init__.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 15:56:16.252356 seldonian_engine-0.8.2/seldonian/candidate_selection/
--rw-r--r--   0 ahoag      (501) staff       (20)       40 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/candidate_selection/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)    19265 2023-06-22 21:24:25.000000 seldonian_engine-0.8.2/seldonian/candidate_selection/candidate_selection.py
--rw-r--r--   0 ahoag      (501) staff       (20)    12880 2023-06-22 21:24:25.000000 seldonian_engine-0.8.2/seldonian/dataset.py
--rw-r--r--   0 ahoag      (501) staff       (20)    21029 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/hyperparam_search.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 15:56:16.255069 seldonian_engine-0.8.2/seldonian/models/
--rw-r--r--   0 ahoag      (501) staff       (20)       48 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/models/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     8288 2023-05-31 21:23:44.000000 seldonian_engine-0.8.2/seldonian/models/models.py
--rw-r--r--   0 ahoag      (501) staff       (20)    19375 2023-07-20 23:54:53.000000 seldonian_engine-0.8.2/seldonian/models/objectives.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1284 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/models/pytorch_cnn.py
--rw-r--r--   0 ahoag      (501) staff       (20)     6883 2023-05-31 21:23:44.000000 seldonian_engine-0.8.2/seldonian/models/pytorch_model.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1084 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/models/sklearn_lr.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4758 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/models/sklearn_model.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1559 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/models/tensorflow_cnn.py
--rw-r--r--   0 ahoag      (501) staff       (20)     6068 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/models/tensorflow_model.py
--rw-r--r--   0 ahoag      (501) staff       (20)    20883 2023-07-20 23:54:53.000000 seldonian_engine-0.8.2/seldonian/models/zhat_funcs.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 15:56:16.255516 seldonian_engine-0.8.2/seldonian/optimizers/
--rw-r--r--   0 ahoag      (501) staff       (20)       43 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/optimizers/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)    10884 2023-04-03 17:05:25.000000 seldonian_engine-0.8.2/seldonian/optimizers/gradient_descent.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 15:56:16.256918 seldonian_engine-0.8.2/seldonian/parse_tree/
--rw-r--r--   0 ahoag      (501) staff       (20)       75 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/parse_tree/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)    39983 2023-07-20 23:54:53.000000 seldonian_engine-0.8.2/seldonian/parse_tree/nodes.py
--rw-r--r--   0 ahoag      (501) staff       (20)     3828 2023-04-19 20:33:28.000000 seldonian_engine-0.8.2/seldonian/parse_tree/operators.py
--rw-r--r--   0 ahoag      (501) staff       (20)    46709 2023-07-20 04:24:40.000000 seldonian_engine-0.8.2/seldonian/parse_tree/parse_tree.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 15:56:16.257745 seldonian_engine-0.8.2/seldonian/safety_test/
--rw-r--r--   0 ahoag      (501) staff       (20)       36 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/safety_test/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4272 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/safety_test/safety_test.py
--rw-r--r--   0 ahoag      (501) staff       (20)    15854 2023-06-22 21:24:25.000000 seldonian_engine-0.8.2/seldonian/seldonian_algorithm.py
--rw-r--r--   0 ahoag      (501) staff       (20)    22099 2023-06-22 21:24:25.000000 seldonian_engine-0.8.2/seldonian/spec.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 15:56:16.258872 seldonian_engine-0.8.2/seldonian/utils/
--rw-r--r--   0 ahoag      (501) staff       (20)      468 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/utils/RL_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)       24 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/utils/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1685 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/utils/io_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)     6851 2023-07-20 04:24:40.000000 seldonian_engine-0.8.2/seldonian/utils/plot_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)     2035 2023-07-20 23:54:53.000000 seldonian_engine-0.8.2/seldonian/utils/stats_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4210 2023-06-22 21:24:25.000000 seldonian_engine-0.8.2/seldonian/utils/tutorial_utils.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 15:56:16.259305 seldonian_engine-0.8.2/seldonian/warnings/
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.2/seldonian/warnings/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)      344 2023-03-08 18:13:56.000000 seldonian_engine-0.8.2/seldonian/warnings/custom_warnings.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 15:56:16.260161 seldonian_engine-0.8.2/seldonian_engine.egg-info/
--rw-r--r--   0 ahoag      (501) staff       (20)     2133 2023-07-27 15:56:16.000000 seldonian_engine-0.8.2/seldonian_engine.egg-info/PKG-INFO
--rw-r--r--   0 ahoag      (501) staff       (20)     3050 2023-07-27 15:56:16.000000 seldonian_engine-0.8.2/seldonian_engine.egg-info/SOURCES.txt
--rw-r--r--   0 ahoag      (501) staff       (20)        1 2023-07-27 15:56:16.000000 seldonian_engine-0.8.2/seldonian_engine.egg-info/dependency_links.txt
--rw-r--r--   0 ahoag      (501) staff       (20)      148 2023-07-27 15:56:16.000000 seldonian_engine-0.8.2/seldonian_engine.egg-info/requires.txt
--rw-r--r--   0 ahoag      (501) staff       (20)       16 2023-07-27 15:56:16.000000 seldonian_engine-0.8.2/seldonian_engine.egg-info/top_level.txt
--rw-r--r--   0 ahoag      (501) staff       (20)       38 2023-07-27 15:56:16.265829 seldonian_engine-0.8.2/setup.cfg
--rw-r--r--   0 ahoag      (501) staff       (20)     1070 2023-07-27 15:56:08.000000 seldonian_engine-0.8.2/setup.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 15:56:16.265281 seldonian_engine-0.8.2/tests/
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.2/tests/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)    14897 2023-06-22 21:24:25.000000 seldonian_engine-0.8.2/tests/conftest.py
--rw-r--r--   0 ahoag      (501) staff       (20)    13340 2023-06-22 21:24:25.000000 seldonian_engine-0.8.2/tests/test_RL.py
--rw-r--r--   0 ahoag      (501) staff       (20)     6913 2023-06-22 21:24:25.000000 seldonian_engine-0.8.2/tests/test_dataset.py
--rw-r--r--   0 ahoag      (501) staff       (20)      828 2022-09-21 21:32:24.000000 seldonian_engine-0.8.2/tests/test_io_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)     2381 2023-07-20 04:24:40.000000 seldonian_engine-0.8.2/tests/test_models.py
--rw-r--r--   0 ahoag      (501) staff       (20)     5548 2023-07-20 23:54:53.000000 seldonian_engine-0.8.2/tests/test_objectives.py
--rw-r--r--   0 ahoag      (501) staff       (20)    65550 2023-07-20 04:24:40.000000 seldonian_engine-0.8.2/tests/test_parse_tree.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1223 2022-09-12 23:15:58.000000 seldonian_engine-0.8.2/tests/test_plot_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4820 2023-06-22 21:24:25.000000 seldonian_engine-0.8.2/tests/test_safety_test.py
--rw-r--r--   0 ahoag      (501) staff       (20)    61920 2023-07-20 04:24:40.000000 seldonian_engine-0.8.2/tests/test_seldonian_algorithm.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1582 2023-02-09 17:42:02.000000 seldonian_engine-0.8.2/tests/test_sklearn.py
--rw-r--r--   0 ahoag      (501) staff       (20)     6389 2022-11-07 22:08:04.000000 seldonian_engine-0.8.2/tests/test_spec.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1272 2022-09-21 21:32:24.000000 seldonian_engine-0.8.2/tests/test_stats_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)      544 2022-09-21 21:32:24.000000 seldonian_engine-0.8.2/tests/test_tutorial_utils.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 16:16:20.022262 seldonian_engine-0.8.3/
+-rw-r--r--   0 ahoag      (501) staff       (20)     1527 2022-09-12 23:15:58.000000 seldonian_engine-0.8.3/LICENSE
+-rw-r--r--   0 ahoag      (501) staff       (20)     2133 2023-07-27 16:16:20.022093 seldonian_engine-0.8.3/PKG-INFO
+-rw-r--r--   0 ahoag      (501) staff       (20)     1642 2023-07-20 04:24:35.000000 seldonian_engine-0.8.3/README.md
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 16:16:20.004823 seldonian_engine-0.8.3/seldonian/
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 16:16:20.007324 seldonian_engine-0.8.3/seldonian/RL/
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 16:16:20.008355 seldonian_engine-0.8.3/seldonian/RL/Agents/
+-rw-r--r--   0 ahoag      (501) staff       (20)     1733 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/RL/Agents/Agent.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 16:16:20.008821 seldonian_engine-0.8.3/seldonian/RL/Agents/Bases/
+-rw-r--r--   0 ahoag      (501) staff       (20)     4537 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/RL/Agents/Bases/Fourier.py
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.3/seldonian/RL/Agents/Bases/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1043 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/RL/Agents/Discrete_Random_Agent.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 16:16:20.009486 seldonian_engine-0.8.3/seldonian/RL/Agents/Function_Approximators/
+-rw-r--r--   0 ahoag      (501) staff       (20)      554 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/RL/Agents/Function_Approximators/Function_Approximator.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1333 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/RL/Agents/Function_Approximators/Linear_FA.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     2854 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/RL/Agents/Function_Approximators/Table.py
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.3/seldonian/RL/Agents/Function_Approximators/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     3054 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/RL/Agents/Parameterized_non_learning_softmax_agent.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 16:16:20.009997 seldonian_engine-0.8.3/seldonian/RL/Agents/Policies/
+-rw-r--r--   0 ahoag      (501) staff       (20)     4906 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/RL/Agents/Policies/Policy.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     6459 2023-05-31 21:23:44.000000 seldonian_engine-0.8.3/seldonian/RL/Agents/Policies/Softmax.py
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.3/seldonian/RL/Agents/Policies/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.3/seldonian/RL/Agents/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      794 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/RL/Agents/keyboard_gridworld.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      406 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/RL/Agents/mountain_car_rough_solution.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 16:16:20.010453 seldonian_engine-0.8.3/seldonian/RL/Env_Description/
+-rw-r--r--   0 ahoag      (501) staff       (20)     2001 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/RL/Env_Description/Env_Description.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     2311 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/RL/Env_Description/Spaces.py
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.3/seldonian/RL/Env_Description/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     3698 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/RL/RL_generate_dataset_and_spec_file.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     2335 2023-05-31 21:23:44.000000 seldonian_engine-0.8.3/seldonian/RL/RL_model.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     6027 2023-07-27 16:13:15.000000 seldonian_engine-0.8.3/seldonian/RL/RL_runner.py
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.3/seldonian/RL/__init__.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 16:16:20.011335 seldonian_engine-0.8.3/seldonian/RL/environments/
+-rw-r--r--   0 ahoag      (501) staff       (20)     1364 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/RL/environments/Environment.py
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.3/seldonian/RL/environments/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4075 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/RL/environments/gridworld.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     2352 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/RL/environments/mountaincar.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      984 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/RL/environments/n_step_mountaincar.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     2807 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/RL/environments/simglucose_env.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1196 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/RL/generate_gridworld_episodes.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1236 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/RL/generate_mountaincar_episodes.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1337 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/RL/generate_simglucose_episodes.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      615 2022-09-13 15:24:12.000000 seldonian_engine-0.8.3/seldonian/RL/hyperparams_and_settings.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     3991 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/RL/profiling_seldonian_RL.py
+-rw-r--r--   0 ahoag      (501) staff       (20)       33 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/__init__.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 16:16:20.011665 seldonian_engine-0.8.3/seldonian/candidate_selection/
+-rw-r--r--   0 ahoag      (501) staff       (20)       40 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/candidate_selection/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    19265 2023-06-22 21:24:25.000000 seldonian_engine-0.8.3/seldonian/candidate_selection/candidate_selection.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    12880 2023-06-22 21:24:25.000000 seldonian_engine-0.8.3/seldonian/dataset.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    21029 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/hyperparam_search.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 16:16:20.013872 seldonian_engine-0.8.3/seldonian/models/
+-rw-r--r--   0 ahoag      (501) staff       (20)       48 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/models/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     8288 2023-05-31 21:23:44.000000 seldonian_engine-0.8.3/seldonian/models/models.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    19375 2023-07-20 23:54:53.000000 seldonian_engine-0.8.3/seldonian/models/objectives.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1284 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/models/pytorch_cnn.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     6883 2023-05-31 21:23:44.000000 seldonian_engine-0.8.3/seldonian/models/pytorch_model.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1084 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/models/sklearn_lr.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4758 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/models/sklearn_model.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1559 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/models/tensorflow_cnn.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     6068 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/models/tensorflow_model.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    20883 2023-07-20 23:54:53.000000 seldonian_engine-0.8.3/seldonian/models/zhat_funcs.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 16:16:20.014271 seldonian_engine-0.8.3/seldonian/optimizers/
+-rw-r--r--   0 ahoag      (501) staff       (20)       43 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/optimizers/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    10884 2023-04-03 17:05:25.000000 seldonian_engine-0.8.3/seldonian/optimizers/gradient_descent.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 16:16:20.015306 seldonian_engine-0.8.3/seldonian/parse_tree/
+-rw-r--r--   0 ahoag      (501) staff       (20)       75 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/parse_tree/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    39983 2023-07-20 23:54:53.000000 seldonian_engine-0.8.3/seldonian/parse_tree/nodes.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     3828 2023-04-19 20:33:28.000000 seldonian_engine-0.8.3/seldonian/parse_tree/operators.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    46709 2023-07-20 04:24:40.000000 seldonian_engine-0.8.3/seldonian/parse_tree/parse_tree.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 16:16:20.016076 seldonian_engine-0.8.3/seldonian/safety_test/
+-rw-r--r--   0 ahoag      (501) staff       (20)       36 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/safety_test/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4272 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/safety_test/safety_test.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    15854 2023-06-22 21:24:25.000000 seldonian_engine-0.8.3/seldonian/seldonian_algorithm.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    22099 2023-06-22 21:24:25.000000 seldonian_engine-0.8.3/seldonian/spec.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 16:16:20.017145 seldonian_engine-0.8.3/seldonian/utils/
+-rw-r--r--   0 ahoag      (501) staff       (20)      468 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/utils/RL_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)       24 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/utils/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1685 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/utils/io_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     6851 2023-07-20 04:24:40.000000 seldonian_engine-0.8.3/seldonian/utils/plot_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     2035 2023-07-20 23:54:53.000000 seldonian_engine-0.8.3/seldonian/utils/stats_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4210 2023-06-22 21:24:25.000000 seldonian_engine-0.8.3/seldonian/utils/tutorial_utils.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 16:16:20.017552 seldonian_engine-0.8.3/seldonian/warnings/
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.3/seldonian/warnings/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      344 2023-03-08 18:13:56.000000 seldonian_engine-0.8.3/seldonian/warnings/custom_warnings.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 16:16:20.018363 seldonian_engine-0.8.3/seldonian_engine.egg-info/
+-rw-r--r--   0 ahoag      (501) staff       (20)     2133 2023-07-27 16:16:19.000000 seldonian_engine-0.8.3/seldonian_engine.egg-info/PKG-INFO
+-rw-r--r--   0 ahoag      (501) staff       (20)     3050 2023-07-27 16:16:20.000000 seldonian_engine-0.8.3/seldonian_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)        1 2023-07-27 16:16:19.000000 seldonian_engine-0.8.3/seldonian_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)      148 2023-07-27 16:16:19.000000 seldonian_engine-0.8.3/seldonian_engine.egg-info/requires.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)       16 2023-07-27 16:16:19.000000 seldonian_engine-0.8.3/seldonian_engine.egg-info/top_level.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)       38 2023-07-27 16:16:20.022312 seldonian_engine-0.8.3/setup.cfg
+-rw-r--r--   0 ahoag      (501) staff       (20)     1070 2023-07-27 16:16:14.000000 seldonian_engine-0.8.3/setup.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 16:16:20.021801 seldonian_engine-0.8.3/tests/
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.3/tests/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    14897 2023-06-22 21:24:25.000000 seldonian_engine-0.8.3/tests/conftest.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    13326 2023-07-27 16:13:15.000000 seldonian_engine-0.8.3/tests/test_RL.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     6913 2023-06-22 21:24:25.000000 seldonian_engine-0.8.3/tests/test_dataset.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      828 2022-09-21 21:32:24.000000 seldonian_engine-0.8.3/tests/test_io_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     2381 2023-07-20 04:24:40.000000 seldonian_engine-0.8.3/tests/test_models.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     5548 2023-07-20 23:54:53.000000 seldonian_engine-0.8.3/tests/test_objectives.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    65550 2023-07-20 04:24:40.000000 seldonian_engine-0.8.3/tests/test_parse_tree.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1223 2022-09-12 23:15:58.000000 seldonian_engine-0.8.3/tests/test_plot_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4820 2023-06-22 21:24:25.000000 seldonian_engine-0.8.3/tests/test_safety_test.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    61920 2023-07-20 04:24:40.000000 seldonian_engine-0.8.3/tests/test_seldonian_algorithm.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1582 2023-02-09 17:42:02.000000 seldonian_engine-0.8.3/tests/test_sklearn.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     6389 2022-11-07 22:08:04.000000 seldonian_engine-0.8.3/tests/test_spec.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1272 2022-09-21 21:32:24.000000 seldonian_engine-0.8.3/tests/test_stats_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      544 2022-09-21 21:32:24.000000 seldonian_engine-0.8.3/tests/test_tutorial_utils.py
```

### Comparing `seldonian_engine-0.8.2/LICENSE` & `seldonian_engine-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/PKG-INFO` & `seldonian_engine-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seldonian_engine
-Version: 0.8.2
+Version: 0.8.3
 Summary: Core library for Seldonian algorithms
 Home-page: 
 Author: Austin Hoag
 Author-email: austinthomashoag@gmail.com
 Project-URL: Bug Tracker, https://github.com/seldonian-framework/Engine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `seldonian_engine-0.8.2/README.md` & `seldonian_engine-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/RL/Agents/Agent.py` & `seldonian_engine-0.8.3/seldonian/RL/Agents/Agent.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/RL/Agents/Bases/Fourier.py` & `seldonian_engine-0.8.3/seldonian/RL/Agents/Bases/Fourier.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/RL/Agents/Discrete_Random_Agent.py` & `seldonian_engine-0.8.3/seldonian/RL/Agents/Discrete_Random_Agent.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/RL/Agents/Function_Approximators/Function_Approximator.py` & `seldonian_engine-0.8.3/seldonian/RL/Agents/Function_Approximators/Function_Approximator.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/RL/Agents/Function_Approximators/Linear_FA.py` & `seldonian_engine-0.8.3/seldonian/RL/Agents/Function_Approximators/Linear_FA.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/RL/Agents/Function_Approximators/Table.py` & `seldonian_engine-0.8.3/seldonian/RL/Agents/Function_Approximators/Table.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/RL/Agents/Parameterized_non_learning_softmax_agent.py` & `seldonian_engine-0.8.3/seldonian/RL/Agents/Parameterized_non_learning_softmax_agent.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/RL/Agents/Policies/Policy.py` & `seldonian_engine-0.8.3/seldonian/RL/Agents/Policies/Policy.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/RL/Agents/Policies/Softmax.py` & `seldonian_engine-0.8.3/seldonian/RL/Agents/Policies/Softmax.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/RL/Agents/keyboard_gridworld.py` & `seldonian_engine-0.8.3/seldonian/RL/Agents/keyboard_gridworld.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/RL/Env_Description/Env_Description.py` & `seldonian_engine-0.8.3/seldonian/RL/Env_Description/Env_Description.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/RL/Env_Description/Spaces.py` & `seldonian_engine-0.8.3/seldonian/RL/Env_Description/Spaces.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/RL/RL_generate_dataset_and_spec_file.py` & `seldonian_engine-0.8.3/seldonian/RL/RL_generate_dataset_and_spec_file.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/RL/RL_model.py` & `seldonian_engine-0.8.3/seldonian/RL/RL_model.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/RL/RL_runner.py` & `seldonian_engine-0.8.3/seldonian/RL/RL_runner.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,32 +10,14 @@
 
 from seldonian.dataset import Episode
 
 import multiprocessing as mp
 from concurrent.futures import ProcessPoolExecutor
 
 
-def run_all_trials(hyperparameter_and_setting_dict):
-    """Run many trials, each of which consist
-    of the same number of episodes.
-
-    :param hyperparameter_and_setting_dict: Specifies the
-        environment, agent, number of episodes per trial,
-        and number of trials
-    :type hyperparameter_and_setting_dict: dict
-
-    :return: List((List of episodes, agent)_i) for i trials
-    """
-    num_trials = hyperparameter_and_setting_dict["num_trials"]
-    trials = []
-    for trial_num in range(num_trials):
-        trials.append(run_trial(hyperparameter_and_setting_dict)[0])
-    return trials
-
-
 def run_trial(
     hyperparameter_and_setting_dict, model_params=None, parallel=False, n_workers=8
 ):
     """Run a single trial consists of an arbitrary number of episodes.
 
     :param hyperparameter_and_setting_dict: Specifies the
         environment, agent and number of episodes to run
@@ -71,15 +53,15 @@
         ) as ex:
             results = ex.map(run_episode_from_dict, param1, param2)
             for ep in results:
                 episodes.append(ep)
     else:
         for episode_num in range(num_episodes):
             episodes.append(run_episode(agent, env))
-    return episodes, agent
+    return episodes
 
 
 def run_trial_given_agent_and_env(agent, env, num_episodes):
     """A wrapper for run_trial() where parameters
     are specified explicity rather than via a dictionary.
 
     :param agent: RL Agent
```

### Comparing `seldonian_engine-0.8.2/seldonian/RL/environments/Environment.py` & `seldonian_engine-0.8.3/seldonian/RL/environments/Environment.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/RL/environments/gridworld.py` & `seldonian_engine-0.8.3/seldonian/RL/environments/gridworld.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/RL/environments/mountaincar.py` & `seldonian_engine-0.8.3/seldonian/RL/environments/mountaincar.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/RL/environments/n_step_mountaincar.py` & `seldonian_engine-0.8.3/seldonian/RL/environments/n_step_mountaincar.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/RL/environments/simglucose_env.py` & `seldonian_engine-0.8.3/seldonian/RL/environments/simglucose_env.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/RL/generate_gridworld_episodes.py` & `seldonian_engine-0.8.3/seldonian/RL/generate_gridworld_episodes.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/RL/generate_mountaincar_episodes.py` & `seldonian_engine-0.8.3/seldonian/RL/generate_mountaincar_episodes.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/RL/generate_simglucose_episodes.py` & `seldonian_engine-0.8.3/seldonian/RL/generate_simglucose_episodes.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/RL/hyperparams_and_settings.py` & `seldonian_engine-0.8.3/seldonian/RL/hyperparams_and_settings.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/RL/profiling_seldonian_RL.py` & `seldonian_engine-0.8.3/seldonian/RL/profiling_seldonian_RL.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/candidate_selection/candidate_selection.py` & `seldonian_engine-0.8.3/seldonian/candidate_selection/candidate_selection.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/dataset.py` & `seldonian_engine-0.8.3/seldonian/dataset.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/hyperparam_search.py` & `seldonian_engine-0.8.3/seldonian/hyperparam_search.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/models/models.py` & `seldonian_engine-0.8.3/seldonian/models/models.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/models/objectives.py` & `seldonian_engine-0.8.3/seldonian/models/objectives.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/models/pytorch_cnn.py` & `seldonian_engine-0.8.3/seldonian/models/pytorch_cnn.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/models/pytorch_model.py` & `seldonian_engine-0.8.3/seldonian/models/pytorch_model.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/models/sklearn_lr.py` & `seldonian_engine-0.8.3/seldonian/models/sklearn_lr.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/models/sklearn_model.py` & `seldonian_engine-0.8.3/seldonian/models/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/models/tensorflow_cnn.py` & `seldonian_engine-0.8.3/seldonian/models/tensorflow_cnn.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/models/tensorflow_model.py` & `seldonian_engine-0.8.3/seldonian/models/tensorflow_model.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/models/zhat_funcs.py` & `seldonian_engine-0.8.3/seldonian/models/zhat_funcs.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/optimizers/gradient_descent.py` & `seldonian_engine-0.8.3/seldonian/optimizers/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/parse_tree/nodes.py` & `seldonian_engine-0.8.3/seldonian/parse_tree/nodes.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/parse_tree/operators.py` & `seldonian_engine-0.8.3/seldonian/parse_tree/operators.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/parse_tree/parse_tree.py` & `seldonian_engine-0.8.3/seldonian/parse_tree/parse_tree.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/safety_test/safety_test.py` & `seldonian_engine-0.8.3/seldonian/safety_test/safety_test.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/seldonian_algorithm.py` & `seldonian_engine-0.8.3/seldonian/seldonian_algorithm.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/spec.py` & `seldonian_engine-0.8.3/seldonian/spec.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/utils/io_utils.py` & `seldonian_engine-0.8.3/seldonian/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/utils/plot_utils.py` & `seldonian_engine-0.8.3/seldonian/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/utils/stats_utils.py` & `seldonian_engine-0.8.3/seldonian/utils/stats_utils.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian/utils/tutorial_utils.py` & `seldonian_engine-0.8.3/seldonian/utils/tutorial_utils.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/seldonian_engine.egg-info/PKG-INFO` & `seldonian_engine-0.8.3/seldonian_engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seldonian-engine
-Version: 0.8.2
+Version: 0.8.3
 Summary: Core library for Seldonian algorithms
 Home-page: 
 Author: Austin Hoag
 Author-email: austinthomashoag@gmail.com
 Project-URL: Bug Tracker, https://github.com/seldonian-framework/Engine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `seldonian_engine-0.8.2/seldonian_engine.egg-info/SOURCES.txt` & `seldonian_engine-0.8.3/seldonian_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/setup.py` & `seldonian_engine-0.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seldonian_engine",
-    version="0.8.2",
+    version="0.8.3",
     author="Austin Hoag",
     author_email="austinthomashoag@gmail.com",
     description="Core library for Seldonian algorithms",
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="",
```

### Comparing `seldonian_engine-0.8.2/tests/conftest.py` & `seldonian_engine-0.8.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/tests/test_RL.py` & `seldonian_engine-0.8.3/tests/test_RL.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,15 @@
     with the behavior policy (uniform random). """
     hyperparam_and_setting_dict = {}
     hyperparam_and_setting_dict["env"] = Gridworld()
     hyperparam_and_setting_dict["agent"] = "Parameterized_non_learning_softmax_agent"
     hyperparam_and_setting_dict["num_episodes"] = 10
     hyperparam_and_setting_dict["vis"] = False
 
-    episodes, agent = run_trial(hyperparam_and_setting_dict)
+    episodes = run_trial(hyperparam_and_setting_dict)
 
     assert len(episodes) == 10
     first_episode = episodes[0]
     observations = first_episode.observations
     actions = first_episode.actions
     rewards = first_episode.rewards
     pis = first_episode.action_probs
@@ -287,15 +287,15 @@
     hyperparam_and_setting_dict["agent"] = "Parameterized_non_learning_softmax_agent"
     hyperparam_and_setting_dict["basis"] = "Fourier"
     hyperparam_and_setting_dict["order"] = 2
     hyperparam_and_setting_dict["max_coupled_vars"] = -1
     hyperparam_and_setting_dict["num_episodes"] = 10
     hyperparam_and_setting_dict["vis"] = False
 
-    episodes, agent = run_trial(hyperparam_and_setting_dict)
+    episodes = run_trial(hyperparam_and_setting_dict)
 
     assert len(episodes) == 10
     first_episode = episodes[0]
     observations = first_episode.observations
     actions = first_episode.actions
     rewards = first_episode.rewards
     pis = first_episode.action_probs
```

### Comparing `seldonian_engine-0.8.2/tests/test_dataset.py` & `seldonian_engine-0.8.3/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/tests/test_io_utils.py` & `seldonian_engine-0.8.3/tests/test_io_utils.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/tests/test_models.py` & `seldonian_engine-0.8.3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/tests/test_objectives.py` & `seldonian_engine-0.8.3/tests/test_objectives.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/tests/test_parse_tree.py` & `seldonian_engine-0.8.3/tests/test_parse_tree.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/tests/test_plot_utils.py` & `seldonian_engine-0.8.3/tests/test_plot_utils.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/tests/test_safety_test.py` & `seldonian_engine-0.8.3/tests/test_safety_test.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/tests/test_seldonian_algorithm.py` & `seldonian_engine-0.8.3/tests/test_seldonian_algorithm.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/tests/test_sklearn.py` & `seldonian_engine-0.8.3/tests/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/tests/test_spec.py` & `seldonian_engine-0.8.3/tests/test_spec.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/tests/test_stats_utils.py` & `seldonian_engine-0.8.3/tests/test_stats_utils.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.2/tests/test_tutorial_utils.py` & `seldonian_engine-0.8.3/tests/test_tutorial_utils.py`

 * *Files identical despite different names*

