# Comparing `tmp/seldonian_experiments-0.2.1.tar.gz` & `tmp/seldonian_experiments-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seldonian_experiments-0.2.1.tar", last modified: Tue Jun 27 17:39:31 2023, max compression
+gzip compressed data, was "seldonian_experiments-0.2.2.tar", last modified: Thu Jul 27 15:31:15 2023, max compression
```

## Comparing `seldonian_experiments-0.2.1.tar` & `seldonian_experiments-0.2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-27 17:39:31.634804 seldonian_experiments-0.2.1/
--rw-r--r--   0 ahoag      (501) staff       (20)     1527 2022-04-25 15:36:26.000000 seldonian_experiments-0.2.1/LICENSE
--rw-r--r--   0 ahoag      (501) staff       (20)      816 2023-06-27 17:39:31.634636 seldonian_experiments-0.2.1/PKG-INFO
--rw-r--r--   0 ahoag      (501) staff       (20)      295 2022-11-11 21:28:20.000000 seldonian_experiments-0.2.1/README.md
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-27 17:39:31.627881 seldonian_experiments-0.2.1/examples/
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2023-03-09 21:51:03.000000 seldonian_experiments-0.2.1/examples/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4973 2023-03-27 18:38:58.000000 seldonian_experiments-0.2.1/examples/run_examples.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-27 17:39:31.632115 seldonian_experiments-0.2.1/experiments/
--rw-r--r--   0 ahoag      (501) staff       (20)       81 2023-03-09 00:38:52.000000 seldonian_experiments-0.2.1/experiments/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4062 2023-05-25 23:09:19.000000 seldonian_experiments-0.2.1/experiments/base_example.py
--rw-r--r--   0 ahoag      (501) staff       (20)    13506 2023-06-23 19:23:37.000000 seldonian_experiments-0.2.1/experiments/experiment_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)    42671 2023-06-22 22:30:47.000000 seldonian_experiments-0.2.1/experiments/experiments.py
--rw-r--r--   0 ahoag      (501) staff       (20)    39631 2023-05-25 22:09:58.000000 seldonian_experiments-0.2.1/experiments/generate_plots.py
--rw-r--r--   0 ahoag      (501) staff       (20)     3527 2023-05-25 22:54:38.000000 seldonian_experiments-0.2.1/experiments/headless_example.py
--rw-r--r--   0 ahoag      (501) staff       (20)    17398 2023-06-22 22:33:01.000000 seldonian_experiments-0.2.1/experiments/headless_experiments.py
--rw-r--r--   0 ahoag      (501) staff       (20)     8933 2023-04-25 19:01:34.000000 seldonian_experiments-0.2.1/experiments/headless_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)     2127 2023-05-08 15:32:53.000000 seldonian_experiments-0.2.1/experiments/perf_eval_funcs.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-27 17:39:31.633050 seldonian_experiments-0.2.1/seldonian_experiments.egg-info/
--rw-r--r--   0 ahoag      (501) staff       (20)      816 2023-06-27 17:39:31.000000 seldonian_experiments-0.2.1/seldonian_experiments.egg-info/PKG-INFO
--rw-r--r--   0 ahoag      (501) staff       (20)      680 2023-06-27 17:39:31.000000 seldonian_experiments-0.2.1/seldonian_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 ahoag      (501) staff       (20)        1 2023-06-27 17:39:31.000000 seldonian_experiments-0.2.1/seldonian_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 ahoag      (501) staff       (20)       17 2023-06-27 17:39:31.000000 seldonian_experiments-0.2.1/seldonian_experiments.egg-info/requires.txt
--rw-r--r--   0 ahoag      (501) staff       (20)       21 2023-06-27 17:39:31.000000 seldonian_experiments-0.2.1/seldonian_experiments.egg-info/top_level.txt
--rw-r--r--   0 ahoag      (501) staff       (20)       38 2023-06-27 17:39:31.634849 seldonian_experiments-0.2.1/setup.cfg
--rw-r--r--   0 ahoag      (501) staff       (20)      869 2023-06-27 17:39:18.000000 seldonian_experiments-0.2.1/setup.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-27 17:39:31.634295 seldonian_experiments-0.2.1/tests/
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-07-11 18:48:12.000000 seldonian_experiments-0.2.1/tests/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4276 2023-06-27 16:43:15.000000 seldonian_experiments-0.2.1/tests/conftest.py
--rw-r--r--   0 ahoag      (501) staff       (20)     9611 2023-05-26 14:48:12.000000 seldonian_experiments-0.2.1/tests/test_examples.py
--rw-r--r--   0 ahoag      (501) staff       (20)      848 2023-05-26 14:46:07.000000 seldonian_experiments-0.2.1/tests/test_experiments.py
--rw-r--r--   0 ahoag      (501) staff       (20)     9041 2023-05-22 23:02:27.000000 seldonian_experiments-0.2.1/tests/test_generate_plots.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 15:31:15.435941 seldonian_experiments-0.2.2/
+-rw-r--r--   0 ahoag      (501) staff       (20)     1527 2022-04-25 15:36:26.000000 seldonian_experiments-0.2.2/LICENSE
+-rw-r--r--   0 ahoag      (501) staff       (20)      816 2023-07-27 15:31:15.435776 seldonian_experiments-0.2.2/PKG-INFO
+-rw-r--r--   0 ahoag      (501) staff       (20)      295 2022-11-11 21:28:20.000000 seldonian_experiments-0.2.2/README.md
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 15:31:15.430540 seldonian_experiments-0.2.2/examples/
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2023-03-09 21:51:03.000000 seldonian_experiments-0.2.2/examples/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4973 2023-03-27 18:38:58.000000 seldonian_experiments-0.2.2/examples/run_examples.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 15:31:15.433597 seldonian_experiments-0.2.2/experiments/
+-rw-r--r--   0 ahoag      (501) staff       (20)       81 2023-03-09 00:38:52.000000 seldonian_experiments-0.2.2/experiments/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4062 2023-05-25 23:09:19.000000 seldonian_experiments-0.2.2/experiments/base_example.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    13605 2023-07-24 17:39:58.000000 seldonian_experiments-0.2.2/experiments/experiment_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    42680 2023-07-20 20:18:02.000000 seldonian_experiments-0.2.2/experiments/experiments.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    41974 2023-07-25 17:15:58.000000 seldonian_experiments-0.2.2/experiments/generate_plots.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     3527 2023-05-25 22:54:38.000000 seldonian_experiments-0.2.2/experiments/headless_example.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    17398 2023-06-22 22:33:01.000000 seldonian_experiments-0.2.2/experiments/headless_experiments.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     8933 2023-04-25 19:01:34.000000 seldonian_experiments-0.2.2/experiments/headless_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     2127 2023-05-08 15:32:53.000000 seldonian_experiments-0.2.2/experiments/perf_eval_funcs.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 15:31:15.434438 seldonian_experiments-0.2.2/seldonian_experiments.egg-info/
+-rw-r--r--   0 ahoag      (501) staff       (20)      816 2023-07-27 15:31:15.000000 seldonian_experiments-0.2.2/seldonian_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 ahoag      (501) staff       (20)      680 2023-07-27 15:31:15.000000 seldonian_experiments-0.2.2/seldonian_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)        1 2023-07-27 15:31:15.000000 seldonian_experiments-0.2.2/seldonian_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)       17 2023-07-27 15:31:15.000000 seldonian_experiments-0.2.2/seldonian_experiments.egg-info/requires.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)       21 2023-07-27 15:31:15.000000 seldonian_experiments-0.2.2/seldonian_experiments.egg-info/top_level.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)       38 2023-07-27 15:31:15.435987 seldonian_experiments-0.2.2/setup.cfg
+-rw-r--r--   0 ahoag      (501) staff       (20)      869 2023-07-27 15:31:01.000000 seldonian_experiments-0.2.2/setup.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-27 15:31:15.435472 seldonian_experiments-0.2.2/tests/
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-07-11 18:48:12.000000 seldonian_experiments-0.2.2/tests/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4276 2023-06-27 16:43:15.000000 seldonian_experiments-0.2.2/tests/conftest.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     9611 2023-05-26 14:48:12.000000 seldonian_experiments-0.2.2/tests/test_examples.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      848 2023-05-26 14:46:07.000000 seldonian_experiments-0.2.2/tests/test_experiments.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     9041 2023-05-22 23:02:27.000000 seldonian_experiments-0.2.2/tests/test_generate_plots.py
```

### Comparing `seldonian_experiments-0.2.1/LICENSE` & `seldonian_experiments-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.2.1/PKG-INFO` & `seldonian_experiments-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seldonian_experiments
-Version: 0.2.1
+Version: 0.2.2
 Summary: Library for running experiments with Seldonian algorithms
 Home-page: 
 Author: Austin Hoag
 Author-email: austinthomashoag@gmail.com
 Project-URL: Bug Tracker, https://github.com/seldonian-framework/Experiments/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `seldonian_experiments-0.2.1/examples/run_examples.py` & `seldonian_experiments-0.2.2/examples/run_examples.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.2.1/experiments/base_example.py` & `seldonian_experiments-0.2.2/experiments/base_example.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.2.1/experiments/experiment_utils.py` & `seldonian_experiments-0.2.2/experiments/experiment_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ Utilities used in the rest of the library """
 
 import os, copy, pickle, math
 import numpy as np
 
-from seldonian.RL.RL_runner import create_agent, run_trial_given_agent_and_env
+# from seldonian.RL.RL_runner import create_agent, run_trial_given_agent_and_env
+from seldonian.RL.RL_runner import create_agent_fromdict, run_trial_given_agent_and_env
 from seldonian.utils.stats_utils import weighted_sum_gamma
 from seldonian.dataset import SupervisedDataSet,RLDataSet
 from seldonian.utils.io_utils import load_pickle
 
 
 def generate_resampled_datasets(dataset, n_trials, save_dir):
     """Utility function for supervised learning to generate the
@@ -243,15 +244,15 @@
     """
     # Get trained model weights from running the Seldonian algo
     model = kwargs["model"]
     new_params = model.policy.get_params()
 
     # create env and agent
     hyperparameter_and_setting_dict = kwargs["hyperparameter_and_setting_dict"]
-    agent = create_agent(hyperparameter_and_setting_dict)
+    agent = create_agent_fromdict(hyperparameter_and_setting_dict)
     env = hyperparameter_and_setting_dict["env"]
 
     # set agent's weights to the trained model weights
     agent.set_new_params(new_params)
 
     # generate episodes
     num_episodes = kwargs["n_episodes_for_eval"]
```

### Comparing `seldonian_experiments-0.2.1/experiments/experiments.py` & `seldonian_experiments-0.2.2/experiments/experiments.py`

 * *Files 0% similar despite different names*

```diff
@@ -528,15 +528,14 @@
         ################################
         """" Run Seldonian algorithm """
         ################################
 
         try:
             SA = SeldonianAlgorithm(spec_for_exp)
             passed_safety, solution = SA.run(write_cs_logfile=verbose, debug=verbose)
-
         except (ValueError, ZeroDivisionError):
             passed_safety = False
             solution = "NSF"
 
         if verbose:
             print("Solution from running seldonian algorithm:")
             print(solution)
@@ -581,15 +580,15 @@
 
                 elif regime == "reinforcement_learning":
                     model = copy.deepcopy(SA.model)
                     model.policy.set_new_params(solution)
                     perf_eval_kwargs["model"] = model
                     perf_eval_kwargs[
                         "hyperparameter_and_setting_dict"
-                    ] = hyperparameter_and_setting_dict
+                    ] = kwargs["hyperparameter_and_setting_dict"]
                     episodes_for_eval, performance = perf_eval_fn(**perf_eval_kwargs)
 
                 if verbose:
                     print(f"Performance = {performance}")
                     print(
                         "Determining whether solution "
                         "is actually safe on ground truth"
```

### Comparing `seldonian_experiments-0.2.1/experiments/generate_plots.py` & `seldonian_experiments-0.2.2/experiments/generate_plots.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,19 +102,26 @@
         self.perf_eval_kwargs = perf_eval_kwargs
         self.constraint_eval_kwargs = constraint_eval_kwargs
         self.batch_epoch_dict = batch_epoch_dict
 
     def make_plots(
         self,
         model_label_dict={},
+        ignore_models=[],
         fontsize=12,
+        title_fontsize=12,
         legend_fontsize=8,
+        ncols_legend=3,
         performance_label="accuracy",
+        sr_label="Prob. of solution",
+        fr_label="Prob. of violation",
         performance_yscale="linear",
         performance_ylims=[],
+        hoz_axis_label="Amount of data",
+        show_confidence_level=True,
         marker_size=20,
         save_format="pdf",
         show_title=True,
         custom_title=None,
         include_legend=True,
         savename=None,
     ):
@@ -157,14 +164,16 @@
         # Figure out what experiments we have from subfolders in results_dir
         subfolders = [
             os.path.basename(f) for f in os.scandir(self.results_dir) if f.is_dir()
         ]
         all_models = [
             x.split("_results")[0] for x in subfolders if x.endswith("_results")
         ]
+        if ignore_models != []:
+            all_models = [x for x in all_models if x not in ignore_models]
         seldonian_models = list(set(all_models).intersection(seldonian_model_set))
         baselines = sorted(list(set(all_models).difference(seldonian_model_set)))
         if not (seldonian_models or baselines):
             print("No results for Seldonian models or baselines found ")
             return
 
         ## BASELINE RESULTS SETUP
@@ -232,23 +241,21 @@
             seldonian_dict[seldonian_model]["X_all"] = X_all
             seldonian_dict[seldonian_model]["X_passed"] = X_passed
 
         ## PLOTTING SETUP
         vert_size = 3 + n_constraints
         if include_legend:
             vert_size+=0.5
-            figsize = (9, vert_size)
+            figsize = (14, vert_size)
         else:
-            figsize = (9, vert_size)
+            figsize = (14, vert_size)
         fig = plt.figure(figsize=figsize)
         plot_index = 1
         n_rows = len(constraint_strs)
         n_cols = 3
-        fontsize = fontsize
-        legend_fontsize = legend_fontsize
         legend_handles = []
         legend_labels = []
 
         # One row per constraint
         for constraint_index, constraint_str in enumerate(constraint_strs):
             constraint_num = constraint_index+1
             delta = deltas[constraint_index]
@@ -263,26 +270,26 @@
 
             # Plot title (put above middle plot)
             if show_title:
                 if custom_title:
                     title = custom_title
                 else:
                     title = f"constraint: \ng={constraint_str}"
-                ax_sr.set_title(title, y=1.05, fontsize=10)
+                ax_sr.set_title(title, y=1.05, fontsize=title_fontsize)
 
             # Plot labels
             ax_performance.set_ylabel(performance_label, fontsize=fontsize)
-            ax_sr.set_ylabel("Prob. of solution", fontsize=fontsize)
-            ax_fr.set_ylabel("Prob. of violation", fontsize=fontsize)
+            ax_sr.set_ylabel(sr_label, fontsize=fontsize)
+            ax_fr.set_ylabel(fr_label, fontsize=fontsize)
 
             # Only put horizontal axis labels on last row of plots
             if constraint_index == n_constraints - 1:
-                ax_performance.set_xlabel("Amount of data", fontsize=fontsize)
-                ax_sr.set_xlabel("Amount of data", fontsize=fontsize)
-                ax_fr.set_xlabel("Amount of data", fontsize=fontsize)
+                ax_performance.set_xlabel(hoz_axis_label, fontsize=fontsize)
+                ax_sr.set_xlabel(hoz_axis_label, fontsize=fontsize)
+                ax_fr.set_xlabel(hoz_axis_label, fontsize=fontsize)
 
             # axis scaling
             ax_performance.set_xscale("log")
             if performance_yscale.lower() == "log":
                 ax_performance.set_yscale("log")
             ax_sr.set_xscale("log")
             ax_fr.set_xscale("log")
@@ -299,14 +306,70 @@
                 ax.xaxis.set_minor_locator(locmin)
                 ax.xaxis.set_minor_formatter(matplotlib.ticker.NullFormatter())
 
             ########################
             ### PERFORMANCE PLOT ###
             ########################
 
+
+            # Seldonian performance
+            for seldonian_i, seldonian_model in enumerate(seldonian_models):
+                this_seldonian_dict = seldonian_dict[seldonian_model]
+                seldonian_color = plot_colormap(seldonian_i)
+                df_seldonian_passed = this_seldonian_dict["df_seldonian_passed"]
+                mean_performance = df_seldonian_passed.groupby("data_frac").mean()[
+                    "performance"
+                ].to_numpy()
+                std_performance = df_seldonian_passed.groupby("data_frac").std()[
+                    "performance"
+                ].to_numpy()
+
+                n_passed = df_seldonian_passed.groupby("data_frac").count()[
+                    "performance"
+                ].to_numpy()
+                ste_performance = std_performance / np.sqrt(n_passed)
+                # Only show if 2 or more passed. Otherwise std is not defined.
+                gt1_mask = n_passed > 1
+                mean_performance_masked = mean_performance[gt1_mask]
+                std_performance_masked = std_performance[gt1_mask]
+                ste_performance_masked = ste_performance[gt1_mask]
+
+                X_passed_seldonian = this_seldonian_dict["X_passed"].to_numpy()
+                X_passed_seldonian_masked = X_passed_seldonian[gt1_mask]
+                (pl,) = ax_performance.plot(
+                    X_passed_seldonian_masked,
+                    mean_performance_masked,
+                    color=seldonian_color,
+                    # linestyle="--",
+                    linestyle="-",
+                )
+                if constraint_index == 0:
+                    legend_handles.append(pl)
+                    if seldonian_model in model_label_dict:
+                        legend_labels.append(model_label_dict[seldonian_model])
+                    else:
+                        legend_labels.append(seldonian_model)
+
+                ax_performance.scatter(
+                    X_passed_seldonian_masked,
+                    mean_performance_masked,
+                    color=seldonian_color,
+                    s=marker_size,
+                    marker="o",
+                    zorder=10
+                )
+                ax_performance.fill_between(
+                    X_passed_seldonian_masked,
+                    mean_performance_masked - ste_performance_masked,
+                    mean_performance_masked + ste_performance_masked,
+                    color=seldonian_color,
+                    alpha=0.5,
+                    zorder=10
+                )
+            
             # Baseline performance
             for baseline_i, baseline in enumerate(baselines):
                 baseline_color = plot_colormap(
                     baseline_i + len(seldonian_models)
                 )  # 0 is reserved for Seldonian model
                 this_baseline_dict = baseline_dict[baseline]
                 df_baseline_valid = this_baseline_dict["df_baseline_valid"]
@@ -317,90 +380,93 @@
                     "data_frac"
                 ).mean()["performance"]
                 baseline_std_performance = df_baseline_valid.groupby("data_frac").std()[
                     "performance"
                 ]
                 baseline_ste_performance = baseline_std_performance / np.sqrt(n_trials)
                 X_valid_baseline = this_baseline_dict["X_valid"]
+                n_valid = df_baseline_valid.groupby("data_frac").count()[
+                     "performance"
+                 ].to_numpy()
+                # Only show if 2 or more passed. Otherwise std is not defined.
+                gt1_mask = n_valid > 1
+                baseline_mean_performance_masked = baseline_mean_performance[gt1_mask]
+                baseline_std_performance_masked = baseline_std_performance[gt1_mask]
+                baseline_ste_performance_masked = baseline_ste_performance[gt1_mask]
+                X_valid_baseline_masked = X_valid_baseline[gt1_mask]
                 (pl,) = ax_performance.plot(
-                    X_valid_baseline.to_numpy(),
-                    baseline_mean_performance.to_numpy(),
+                    X_valid_baseline_masked.to_numpy(),
+                    baseline_mean_performance_masked.to_numpy(),
                     color=baseline_color,
                     label=baseline,
                 )
                 if constraint_index == 0:
                     legend_handles.append(pl)
                     if baseline in model_label_dict:
                         legend_labels.append(model_label_dict[baseline])
                     else:
                         legend_labels.append(baseline)
                 ax_performance.scatter(
-                    X_valid_baseline,
-                    baseline_mean_performance,
+                    X_valid_baseline_masked,
+                    baseline_mean_performance_masked,
                     color=baseline_color,
                     s=marker_size,
                     marker=marker_list[baseline_i],
                 )
                 ax_performance.fill_between(
-                    X_valid_baseline,
-                    baseline_mean_performance - baseline_ste_performance,
-                    baseline_mean_performance + baseline_ste_performance,
+                    X_valid_baseline_masked,
+                    baseline_mean_performance_masked - baseline_ste_performance_masked,
+                    baseline_mean_performance_masked + baseline_ste_performance_masked,
                     color=baseline_color,
                     alpha=0.5,
                 )
+           
+            if performance_ylims:
+                ax_performance.set_ylim(*performance_ylims)
+            ##########################
+            ### SOLUTION RATE PLOT ###
+            ##########################
 
-            # Seldonian performance
+            # Seldonian solution rate
             for seldonian_i, seldonian_model in enumerate(seldonian_models):
                 this_seldonian_dict = seldonian_dict[seldonian_model]
                 seldonian_color = plot_colormap(seldonian_i)
-                df_seldonian_passed = this_seldonian_dict["df_seldonian_passed"]
-                mean_performance = df_seldonian_passed.groupby("data_frac").mean()[
-                    "performance"
-                ].to_numpy()
-                std_performance = df_seldonian_passed.groupby("data_frac").std()[
-                    "performance"
-                ].to_numpy()
-                n_passed = df_seldonian_passed.groupby("data_frac").count()[
-                    "performance"
-                ].to_numpy()
-                ste_performance = std_performance / np.sqrt(n_passed)
-                X_passed_seldonian = this_seldonian_dict["X_passed"].to_numpy()
-                (pl,) = ax_performance.plot(
-                    X_passed_seldonian,
-                    mean_performance,
+                df_seldonian = this_seldonian_dict["df_seldonian"]
+                n_trials = df_seldonian["trial_i"].max() + 1
+                mean_sr = df_seldonian.groupby("data_frac").mean()["passed_safety"].to_numpy()
+                std_sr = df_seldonian.groupby("data_frac").std()["passed_safety"].to_numpy()
+                ste_sr = std_sr / np.sqrt(n_trials)
+
+                X_all_seldonian = this_seldonian_dict["X_all"].to_numpy()
+
+                ax_sr.plot(
+                    X_all_seldonian,
+                    mean_sr,
                     color=seldonian_color,
-                    linestyle="--",
+                    # linestyle="--",
+                    linestyle="-",
+                    label="QSA",
+                    zorder=10
                 )
-                if constraint_index == 0:
-                    legend_handles.append(pl)
-                    if seldonian_model in model_label_dict:
-                        legend_labels.append(model_label_dict[seldonian_model])
-                    else:
-                        legend_labels.append(seldonian_model)
-
-                ax_performance.scatter(
-                    X_passed_seldonian,
-                    mean_performance,
+                ax_sr.scatter(
+                    X_all_seldonian,
+                    mean_sr,
                     color=seldonian_color,
                     s=marker_size,
                     marker="o",
+                    zorder=10
                 )
-                ax_performance.fill_between(
-                    X_passed_seldonian,
-                    mean_performance - ste_performance,
-                    mean_performance + ste_performance,
+                ax_sr.fill_between(
+                    X_all_seldonian,
+                    mean_sr - ste_sr,
+                    mean_sr + ste_sr,
                     color=seldonian_color,
                     alpha=0.5,
+                    zorder=10
                 )
-            if performance_ylims:
-                ax_performance.set_ylim(*performance_ylims)
-            
-            ##########################
-            ### SOLUTION RATE PLOT ###
-            ##########################
 
             # Plot baseline solution rate
             # (sometimes it doesn't return a solution due to not having enough training data
             # to run model.fit() )
             for baseline_i, baseline in enumerate(baselines):
                 this_baseline_dict = baseline_dict[baseline]
                 baseline_color = plot_colormap(baseline_i + len(seldonian_models))
@@ -426,54 +492,65 @@
                     X_all_baseline,
                     mean_sr - ste_sr,
                     mean_sr + ste_sr,
                     color=baseline_color,
                     alpha=0.5,
                 )
 
-            # Seldonian solution rate
+            ax_sr.set_ylim(-0.05, 1.05)
+
+            ##########################
+            ### FAILURE RATE PLOT ###
+            ##########################
+
+            # Seldonian failure rate
             for seldonian_i, seldonian_model in enumerate(seldonian_models):
                 this_seldonian_dict = seldonian_dict[seldonian_model]
                 seldonian_color = plot_colormap(seldonian_i)
                 df_seldonian = this_seldonian_dict["df_seldonian"]
                 n_trials = df_seldonian["trial_i"].max() + 1
-                mean_sr = df_seldonian.groupby("data_frac").mean()["passed_safety"].to_numpy()
-                std_sr = df_seldonian.groupby("data_frac").std()["passed_safety"].to_numpy()
-                ste_sr = std_sr / np.sqrt(n_trials)
+
+                gstr_failed = 'g' + str(constraint_num) + '_failed'
+
+                mean_fr = df_seldonian.groupby("data_frac").mean()[
+                    gstr_failed].to_numpy()
+                # Need to groupby data frac
+                std_fr = df_seldonian.groupby("data_frac").std()[
+                    gstr_failed].to_numpy()
+
+                ste_fr = std_fr / np.sqrt(n_trials)
 
                 X_all_seldonian = this_seldonian_dict["X_all"].to_numpy()
 
-                ax_sr.plot(
+                ax_fr.plot(
                     X_all_seldonian,
-                    mean_sr,
+                    mean_fr,
                     color=seldonian_color,
-                    linestyle="--",
+                    # linestyle="--",
+                    linestyle="-",
                     label="QSA",
+                    zorder=10
                 )
-                ax_sr.scatter(
+                ax_fr.fill_between(
                     X_all_seldonian,
-                    mean_sr,
+                    mean_fr - ste_fr,
+                    mean_fr + ste_fr,
                     color=seldonian_color,
-                    s=marker_size,
-                    marker="o",
+                    alpha=0.5,
+                    zorder=10
                 )
-                ax_sr.fill_between(
+                ax_fr.scatter(
                     X_all_seldonian,
-                    mean_sr - ste_sr,
-                    mean_sr + ste_sr,
+                    mean_fr,
                     color=seldonian_color,
-                    alpha=0.5,
+                    s=marker_size,
+                    marker="o",
+                    zorder=10
                 )
 
-            ax_sr.set_ylim(-0.05, 1.05)
-
-            ##########################
-            ### FAILURE RATE PLOT ###
-            ##########################
-
             # Baseline failure rate
             for baseline_i, baseline in enumerate(baselines):
                 baseline_color = plot_colormap(baseline_i + len(seldonian_models))
                 # Baseline performance
                 this_baseline_dict = baseline_dict[baseline]
                 df_baseline = this_baseline_dict["df_baseline"]
                 n_trials = df_baseline["trial_i"].max() + 1
@@ -510,70 +587,30 @@
                     X_all_baseline,
                     baseline_mean_fr - baseline_ste_fr,
                     baseline_mean_fr + baseline_ste_fr,
                     color=baseline_color,
                     alpha=0.5,
                 )
 
-            # Seldonian failure rate
-            for seldonian_i, seldonian_model in enumerate(seldonian_models):
-                this_seldonian_dict = seldonian_dict[seldonian_model]
-                seldonian_color = plot_colormap(seldonian_i)
-                df_seldonian = this_seldonian_dict["df_seldonian"]
-                n_trials = df_seldonian["trial_i"].max() + 1
-
-                gstr_failed = 'g' + str(constraint_num) + '_failed'
-
-                mean_fr = df_seldonian.groupby("data_frac").mean()[
-                    gstr_failed].to_numpy()
-                # Need to groupby data frac
-                std_fr = df_seldonian.groupby("data_frac").std()[
-                    gstr_failed].to_numpy()
-
-                ste_fr = std_fr / np.sqrt(n_trials)
-
-                X_all_seldonian = this_seldonian_dict["X_all"].to_numpy()
-
-                ax_fr.plot(
-                    X_all_seldonian,
-                    mean_fr,
-                    color=seldonian_color,
-                    linestyle="--",
-                    label="QSA",
-                )
-                ax_fr.fill_between(
-                    X_all_seldonian,
-                    mean_fr - ste_fr,
-                    mean_fr + ste_fr,
-                    color=seldonian_color,
-                    alpha=0.5,
-                )
-                ax_fr.scatter(
-                    X_all_seldonian,
-                    mean_fr,
-                    color=seldonian_color,
-                    s=marker_size,
-                    marker="o",
-                )
+            ax_fr.set_ylim(-0.05, 1.05)
+            if show_confidence_level:
                 ax_fr.axhline(
                     y=delta, color="k", linestyle="--", label=f"delta={delta}"
                 )
-            ax_fr.set_ylim(-0.05, 1.05)
-
         plt.tight_layout()
 
         if include_legend:
             fig.subplots_adjust(bottom=0.25)
-            ncol = 4
             fig.legend(
-                legend_handles[::-1],
-                legend_labels[::-1],
+                legend_handles,
+                legend_labels,
                 bbox_to_anchor=(0.5, 0.15),
                 loc="upper center",
-                ncol=ncol,
+                ncol=ncols_legend,
+                fontsize=legend_fontsize,
             )
 
         if savename:
             plt.savefig(savename, format=save_format,bbox_inches="tight")
             print(f"Saved {savename}")
         else:
             plt.show()
@@ -963,26 +1000,36 @@
 
         print("Running experiment")
         dataset = self.spec.dataset
 
         if self.datagen_method == "generate_episodes":
             # generate full-size datasets for each trial so that
             # we can reference them for each data_frac
+            try:
+                n_workers_for_episode_generation = self.hyperparameter_and_setting_dict["n_workers_for_episode_generation"]
+            except:
+                n_workers_for_episode_generation = self.n_workers
             save_dir = os.path.join(self.results_dir, "regenerated_datasets")
             os.makedirs(save_dir, exist_ok=True)
             print("generating new episodes for each trial")
             for trial_i in range(self.n_trials):
-                print(f"Trial: {trial_i}")
+                print(f"Trial: {trial_i+1}/{self.n_trials}")
                 savename = os.path.join(
                     save_dir, f"regenerated_data_trial{trial_i}.pkl"
                 )
+                print(savename)
                 if not os.path.exists(savename):
-                    episodes, agent = run_trial(
-                        self.hyperparameter_and_setting_dict, parallel=False
-                    )
+                    if n_workers_for_episode_generation > 1:
+                        episodes = run_trial(
+                            self.hyperparameter_and_setting_dict, parallel=True, n_workers=n_workers_for_episode_generation,
+                        )
+                    else:
+                        episodes = run_trial(
+                            self.hyperparameter_and_setting_dict, parallel=False
+                        )
                     # Save episodes
                     save_pickle(savename, episodes, verbose=True)
                 else:
                     print(f"{savename} already created")
 
         run_seldonian_kwargs = dict(
             spec=self.spec,
```

### Comparing `seldonian_experiments-0.2.1/experiments/headless_example.py` & `seldonian_experiments-0.2.2/experiments/headless_example.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.2.1/experiments/headless_experiments.py` & `seldonian_experiments-0.2.2/experiments/headless_experiments.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.2.1/experiments/headless_utils.py` & `seldonian_experiments-0.2.2/experiments/headless_utils.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.2.1/experiments/perf_eval_funcs.py` & `seldonian_experiments-0.2.2/experiments/perf_eval_funcs.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.2.1/seldonian_experiments.egg-info/PKG-INFO` & `seldonian_experiments-0.2.2/seldonian_experiments.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seldonian-experiments
-Version: 0.2.1
+Version: 0.2.2
 Summary: Library for running experiments with Seldonian algorithms
 Home-page: 
 Author: Austin Hoag
 Author-email: austinthomashoag@gmail.com
 Project-URL: Bug Tracker, https://github.com/seldonian-framework/Experiments/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `seldonian_experiments-0.2.1/seldonian_experiments.egg-info/SOURCES.txt` & `seldonian_experiments-0.2.2/seldonian_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.2.1/setup.py` & `seldonian_experiments-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seldonian_experiments",
-    version="0.2.1",
+    version="0.2.2",
     author="Austin Hoag",
     author_email="austinthomashoag@gmail.com",
     description="Library for running experiments with Seldonian algorithms",
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="",
```

### Comparing `seldonian_experiments-0.2.1/tests/conftest.py` & `seldonian_experiments-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.2.1/tests/test_examples.py` & `seldonian_experiments-0.2.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.2.1/tests/test_experiments.py` & `seldonian_experiments-0.2.2/tests/test_experiments.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.2.1/tests/test_generate_plots.py` & `seldonian_experiments-0.2.2/tests/test_generate_plots.py`

 * *Files identical despite different names*

