# Comparing `tmp/krisi-1.1.1.tar.gz` & `tmp/krisi-1.2.0.tar.gz`

## Comparing `krisi-1.1.1.tar` & `krisi-1.2.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 krisi-1.1.1/.flake8
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 krisi-1.1.1/.isort.cfg
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 krisi-1.1.1/mkdocs.yaml
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 krisi-1.1.1/.vscode/launch.json
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 krisi-1.1.1/.vscode/settings.json
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/__init__.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/sharedtypes.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/analyse/__init__.py
--rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/analyse/correlations.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/analyse/dataset.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/analyse/utils.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/__init__.py
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/assertions.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/compare.py
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/group.py
--rw-r--r--   0        0        0    13443 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/metric.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/score.py
--rw-r--r--   0        0        0    23800 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/scorecard.py
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/type.py
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/utils.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/library/__init__.py
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/library/benchmarking.py
--rw-r--r--   0        0        0    14142 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/library/default_metrics_classification.py
--rw-r--r--   0        0        0     6277 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/library/default_metrics_regression.py
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/library/diagrams.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/evaluate/library/metric_wrappers.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/report/__init__.py
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/report/console.py
--rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/report/graph.py
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/report/interactive.py
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/report/pdf.py
--rw-r--r--   0        0        0     8271 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/report/report.py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/report/type.py
--rw-r--r--   0        0        0     6230 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/report/vizualise.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/report/library/console/diagrams.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/report/library/pdf_layouts/scorecard/report.css
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/report/library/pdf_layouts/scorecard/report.html
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/utils/__init__.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/utils/console_plot.py
--rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/utils/data.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/utils/enums.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/utils/environment.py
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/utils/io.py
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/utils/iterable_helpers.py
--rw-r--r--   0        0        0     6973 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/utils/printing.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/utils/state.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/utils/devutils/environment_checks.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/utils/devutils/generate_from_examples.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 krisi-1.1.1/src/krisi/utils/devutils/timing.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 krisi-1.1.1/.gitignore
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 krisi-1.1.1/LICENSE
--rw-r--r--   0        0        0    61727 2020-02-02 00:00:00.000000 krisi-1.1.1/README.md
--rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 krisi-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    66463 2020-02-02 00:00:00.000000 krisi-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 krisi-1.2.0/.flake8
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 krisi-1.2.0/.isort.cfg
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 krisi-1.2.0/mkdocs.yaml
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 krisi-1.2.0/.vscode/launch.json
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 krisi-1.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/__init__.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/sharedtypes.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/analyse/__init__.py
+-rw-r--r--   0        0        0     4825 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/analyse/correlations.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/analyse/dataset.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/analyse/utils.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/evaluate/__init__.py
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/evaluate/assertions.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/evaluate/compare.py
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/evaluate/group.py
+-rw-r--r--   0        0        0    13706 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/evaluate/metric.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/evaluate/score.py
+-rw-r--r--   0        0        0    23810 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/evaluate/scorecard.py
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/evaluate/type.py
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/evaluate/utils.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/evaluate/library/__init__.py
+-rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/evaluate/library/benchmarking.py
+-rw-r--r--   0        0        0    16414 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/evaluate/library/default_metrics_classification.py
+-rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/evaluate/library/default_metrics_regression.py
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/evaluate/library/diagrams.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/evaluate/library/metric_wrappers.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/report/__init__.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/report/console.py
+-rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/report/graph.py
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/report/interactive.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/report/pdf.py
+-rw-r--r--   0        0        0     8271 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/report/report.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/report/type.py
+-rw-r--r--   0        0        0     6230 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/report/vizualise.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/report/library/console/diagrams.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/report/library/pdf_layouts/scorecard/report.css
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/report/library/pdf_layouts/scorecard/report.html
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/utils/__init__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/utils/console_plot.py
+-rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/utils/data.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/utils/enums.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/utils/environment.py
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/utils/io.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/utils/iterable_helpers.py
+-rw-r--r--   0        0        0     6973 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/utils/printing.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/utils/state.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/utils/devutils/environment_checks.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/utils/devutils/generate_from_examples.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 krisi-1.2.0/src/krisi/utils/devutils/timing.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 krisi-1.2.0/.gitignore
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 krisi-1.2.0/LICENSE
+-rw-r--r--   0        0        0    61727 2020-02-02 00:00:00.000000 krisi-1.2.0/README.md
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 krisi-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    66565 2020-02-02 00:00:00.000000 krisi-1.2.0/PKG-INFO
```

### Comparing `krisi-1.1.1/mkdocs.yaml` & `krisi-1.2.0/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `krisi-1.1.1/.vscode/settings.json` & `krisi-1.2.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `krisi-1.1.1/src/krisi/analyse/correlations.py` & `krisi-1.2.0/src/krisi/analyse/correlations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from functools import reduce
 from pathlib import Path
 from typing import List, Optional, Tuple
 
-import matplotlib.pyplot as plt
 import pandas as pd
 from typing_extensions import Literal
 
 from krisi.evaluate.type import PathConst
 from krisi.report.graph import create_save_graphs
 from krisi.utils.state import RunType, get_global_state
 
@@ -61,14 +60,16 @@
     window: int,
     step: int,
     name: str,
     save_or_display: List[Literal["save", "display"]],
     save_location: str,
     top_k: int,
 ) -> None:
+    import matplotlib.pyplot as plt
+
     fig, ax = plt.subplots(2, 1)
     title = f"Summary of {name} | window - {window} ~ step - {step}"
     fig.suptitle(title)
 
     # ranking = corr_mean/corr_std
 
     df_unrolled_in_time[corr_std.nsmallest(top_k).index.values].plot(
```

### Comparing `krisi-1.1.1/src/krisi/analyse/dataset.py` & `krisi-1.2.0/src/krisi/analyse/dataset.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.1/src/krisi/evaluate/assertions.py` & `krisi-1.2.0/src/krisi/evaluate/assertions.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.1/src/krisi/evaluate/compare.py` & `krisi-1.2.0/src/krisi/evaluate/compare.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.1/src/krisi/evaluate/group.py` & `krisi-1.2.0/src/krisi/evaluate/group.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.1/src/krisi/evaluate/metric.py` & `krisi-1.2.0/src/krisi/evaluate/metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,14 +314,23 @@
         key: str,
     ):
         if self.__dict__[key] is not None:
             raise ValueError("This metric already contains a result.")
         else:
             self.__dict__[key] = result
 
+    def reset_metric(self) -> Metric:
+        self.result = None
+        self.result_rolling = None
+        self.rolling_properties = None
+        self.diagnostics = None
+        self._from_group = False
+        self.comparison_result = None
+        return self
+
 
 def create_diagram_rolling(obj: Metric) -> Optional[List[InteractiveFigure]]:
     if obj.plot_funcs_rolling is None:
         logging.info("No plot_funcs_rolling (Plotting Function Rolling) specified")
         return None
     elif isinstance(obj.result_rolling, Exception) or obj.result_rolling is None:
         return None
```

### Comparing `krisi-1.1.1/src/krisi/evaluate/score.py` & `krisi-1.2.0/src/krisi/evaluate/score.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.1/src/krisi/evaluate/scorecard.py` & `krisi-1.2.0/src/krisi/evaluate/scorecard.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,15 +241,15 @@
             for k in all_keys:
                 if k not in key:
                     if isinstance(scorecard_copy.__dict__[k], Metric):
                         del scorecard_copy.__dict__[k]
 
             return scorecard_copy
         elif isinstance(key, str):
-            return getattr(self, key, Metric("Unknown Metric"))
+            return deepcopy(getattr(self, key, Metric("Unknown Metric")))
 
     def __delitem__(self, key: str) -> None:
         del self[key]
 
     def __repr__(self) -> str:
         self.print(mode=PrintMode.minimal)
         return super().__repr__()
```

### Comparing `krisi-1.1.1/src/krisi/evaluate/type.py` & `krisi-1.2.0/src/krisi/evaluate/type.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     reg_err = "Forecast Errors - Regression"
     stats = "General Statistics"
     unknown = "Unknown"
 
 
 class SampleTypes(Enum):
     insample = "insample"
+    validation = "validation"
     outofsample = "outofsample"
 
 
 class Calculation(ParsableEnum):
     single = "single"
     rolling = "rolling"
     both = "both"
```

### Comparing `krisi-1.1.1/src/krisi/evaluate/utils.py` & `krisi-1.2.0/src/krisi/evaluate/utils.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.1/src/krisi/evaluate/library/__init__.py` & `krisi-1.2.0/src/krisi/evaluate/library/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from typing import List
 
 from krisi.evaluate.metric import Metric
 from krisi.evaluate.type import DatasetType
 
+from .default_metrics_classification import *
 from .default_metrics_classification import (
     binary_classification_balanced_metrics,
     binary_classification_imbalanced_metrics,
     binary_classification_metrics_balanced_benchmarking,
     binary_classification_metrics_imbalanced_benchmarking,
     minimal_binary_classification_metrics,
     minimal_multiclass_classification_metrics,
     multiclass_classification_metrics,
 )
+from .default_metrics_regression import *
 from .default_metrics_regression import (
     all_regression_metrics,
     low_computation_regression_metrics,
     minimal_regression_metrics,
 )
```

### Comparing `krisi-1.1.1/src/krisi/evaluate/library/default_metrics_classification.py` & `krisi-1.2.0/src/krisi/evaluate/library/default_metrics_classification.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,16 +17,19 @@
     display_density_plot,
     display_single_value,
     display_time_series,
 )
 from krisi.evaluate.library.metric_wrappers import (
     bennet_s,
     brier_multi,
+    pred_y_imbalance_ratio,
+    wrap_avg_precision,
     wrap_brier_score,
     wrap_roc_auc,
+    y_label_imbalance_ratio,
 )
 from krisi.evaluate.metric import Metric
 from krisi.evaluate.type import Calculation, MetricCategories, Purpose
 
 accuracy_binary = Metric[float](
     name="Accuracy",
     key="accuracy",
@@ -198,24 +201,25 @@
     purpose=Purpose.loss,
 )
 """~"""
 
 roc_auc_binary_micro, roc_auc_binary_macro, roc_auc_binary_weighted = [
     Metric[float](
         name=f"ROC AUC ({mode}))",
-        key=f"roc_auc_binary_{mode}",
+        key=f"roc_auc_{mode}",
         category=MetricCategories.class_err,
         info="Compute Area Under the Receiver Operating Characteristic Curve (ROC AUC) from prediction scores. Note: this implementation can be used with binary, multiclass and multilabel classification, but some restrictions apply (see Parameters). https://scikit-learn.org/stable/modules/generated/sklearn.metrics.roc_auc_score.html",
         func=wrap_roc_auc,
         parameters={"average": mode},
         plot_funcs=[(display_single_value, dict(width=750.0))],
         plot_funcs_rolling=(display_time_series, dict(width=1500.0)),
         accepts_probabilities=True,
         supports_multiclass=True,
         purpose=Purpose.objective,
+        calculation=Calculation.single,
     )
     for mode in ["micro", "macro", "weighted"]
 ]
 """~"""
 
 
 roc_auc_multi_micro, roc_auc_multi_macro = [
@@ -227,31 +231,79 @@
         func=wrap_roc_auc,
         parameters={"average": mode, "multi_class": "ovr"},
         plot_funcs=[(display_single_value, dict(width=750.0))],
         plot_funcs_rolling=(display_time_series, dict(width=1500.0)),
         accepts_probabilities=True,
         supports_multiclass=True,
         purpose=Purpose.objective,
+        calculation=Calculation.single,
     )
     for mode in ["micro", "macro"]
 ]
+
+avg_precision_micro, avg_precision_macro, avg_precision_weighted = [
+    Metric[float](
+        name=f"Average Precision ({mode}))",
+        key=f"avg_precision_{mode}",
+        category=MetricCategories.class_err,
+        info="Compute average precision (AP) from prediction scores. AP summarizes a precision-recall curve as the weighted mean of precisions achieved at each threshold, with the increase in recall from the previous threshold used as the weight. https://scikit-learn.org/stable/modules/generated/sklearn.metrics.average_precision_score.html#sklearn.metrics.average_precision_score",
+        func=wrap_avg_precision,
+        parameters={"average": mode},
+        plot_funcs=[(display_single_value, dict(width=750.0))],
+        plot_funcs_rolling=(display_time_series, dict(width=1500.0)),
+        accepts_probabilities=True,
+        supports_multiclass=True,
+        purpose=Purpose.objective,
+    )
+    for mode in ["micro", "macro", "weighted"]
+]
+"""~"""
 # """~"""
 # ndcg = Metric[float](
 #     name="NDCG Score",
 #     key="ndcg",
 #     category=MetricCategories.class_err,
 #     info="Compute Normalized Discounted Cumulative Gain. Sum the true scores ranked in the order induced by the predicted scores, after applying a logarithmic discount. Then divide by the best possible score (Ideal DCG, obtained for a perfect ranking) to obtain a score between 0 and 1. This ranking metric returns a high value if true labels are ranked high by y_score.",
 #     func=ndcg_score,
 #     parameters={},
 #     plot_funcs=[(display_single_value, dict(width=750.0))],
 #     plot_funcs_rolling=(display_time_series, dict(width=1500.0)),
 #     accepts_probabilities=False,
 #     supports_multiclass=True,
 # )
 
+imbalance_ratio_y = Metric[float](
+    name="Imbalance Ratio: labels in y",
+    key="imbalance_ratio_y",
+    category=MetricCategories.class_err,
+    info="Measurement of how skewed the target dataset is",
+    func=y_label_imbalance_ratio,
+    parameters={"pos_label": 1},
+    plot_funcs=[(display_single_value, dict(width=750.0))],
+    plot_funcs_rolling=(display_time_series, dict(width=1500.0)),
+    accepts_probabilities=False,
+    supports_multiclass=False,
+    purpose=Purpose.diagram,
+    calculation=Calculation.single,
+)
+imbalance_ratio_pred_y = Metric[float](
+    name="Imbalance Ratio: y vs pred",
+    key="imbalance_ratio_pred_y",
+    category=MetricCategories.class_err,
+    info="Measurement of how skewed the pos_label for prediction vs target is",
+    func=pred_y_imbalance_ratio,
+    parameters={"pos_label": 1},
+    plot_funcs=[(display_single_value, dict(width=750.0))],
+    plot_funcs_rolling=(display_time_series, dict(width=1500.0)),
+    accepts_probabilities=False,
+    supports_multiclass=False,
+    purpose=Purpose.diagram,
+    calculation=Calculation.single,
+)
+
 
 binary_classification_balanced_metrics = [
     accuracy_binary,
     recall_binary,
     precision_binary,
     f_one_score_binary,
     f_one_score_macro,
@@ -275,15 +327,17 @@
     f_one_score_binary,
     f_one_score_macro,
     kappa,
     matthew_corr,
     brier_score,
     calibration,
     roc_auc_binary_macro,
-    cross_entropy,
+    avg_precision_macro,
+    imbalance_ratio_y,
+    imbalance_ratio_pred_y,
 ]
 binary_classification_metrics_balanced_benchmarking = [
     Group[pd.Series](
         name="benchmark",
         key="benchmark",
         metrics=binary_classification_balanced_metrics,
         postprocess_funcs=[model_benchmarking(RandomClassifier())],
```

### Comparing `krisi-1.1.1/src/krisi/evaluate/library/default_metrics_regression.py` & `krisi-1.2.0/src/krisi/evaluate/library/default_metrics_regression.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,22 +13,20 @@
 from krisi.evaluate.group import Group
 from krisi.evaluate.library.diagrams import (
     display_acf_plot,
     display_density_plot,
     display_single_value,
     display_time_series,
 )
-from krisi.evaluate.library.metric_wrappers import ljung_box
 from krisi.evaluate.metric import Metric
 from krisi.evaluate.type import (
     Calculation,
     ComputationalComplexity,
     MetricCategories,
     Purpose,
-    SampleTypes,
 )
 
 mae = Metric[float](
     name="Mean Absolute Error",
     key="mae",
     category=MetricCategories.reg_err,
     info="(Mean absolute error) represents the difference between the original and predicted values extracted by averaged the absolute difference over the data set.",
@@ -146,25 +144,25 @@
     func=lambda res, **kwargs: res.std(),
     plot_funcs=[(display_single_value, dict(width=900.0))],
     plot_funcs_rolling=(display_time_series, dict(width=1500.0)),
     purpose=Purpose.diagram,
 )
 """ ~ """
 
-ljung_box_statistics = Metric[pd.DataFrame](
-    name="Ljung Box Statistics",
-    key="ljung_box_statistics",
-    category=MetricCategories.residual,
-    func=lambda y, pred, **kwargs: ljung_box(y, pred, **kwargs),
-    info="If p is larger than our significance level then we cannot dismiss the null-hypothesis that the residuals are a random walk.",
-    restrict_to_sample=SampleTypes.insample,
-    comp_complexity=ComputationalComplexity.high,
-    calculation=Calculation.single,
-    purpose=Purpose.diagram,
-)
+# ljung_box_statistics = Metric[pd.DataFrame](
+#     name="Ljung Box Statistics",
+#     key="ljung_box_statistics",
+#     category=MetricCategories.residual,
+#     func=lambda y, pred, **kwargs: ljung_box(y, pred, **kwargs),
+#     info="If p is larger than our significance level then we cannot dismiss the null-hypothesis that the residuals are a random walk.",
+#     restrict_to_sample=SampleTypes.insample,
+#     comp_complexity=ComputationalComplexity.high,
+#     calculation=Calculation.single,
+#     purpose=Purpose.diagram,
+# )
 """ ~ """
 
 residual_group = Group[pd.Series](
     name="residual_group",
     key="residual_group",
     metrics=[residuals_mean, residuals_std],
     preprocess_func=lambda y, pred, prob, **kwargs: y - pred,
@@ -178,15 +176,15 @@
     smape,
     mse,
     rmse,
     # rmsle,
     r_two,
     residuals,
     residual_group,
-    ljung_box_statistics,
+    # ljung_box_statistics,
 ]
 """ ~ """
 
 minimal_regression_metrics = [
     mae,
     mape,
     mse,
```

### Comparing `krisi-1.1.1/src/krisi/evaluate/library/diagrams.py` & `krisi-1.2.0/src/krisi/evaluate/library/diagrams.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 import numpy as np
 import pandas as pd
 from sklearn.calibration import calibration_curve
 
 if TYPE_CHECKING:
     import plotly.graph_objects as go
 
-from statsmodels.tsa.stattools import acf, pacf
-
 from krisi.evaluate.type import MetricResult
 
 
 def display_time_series(data: List[MetricResult], **kwargs) -> "go.Figure":
     import plotly.express as px
 
     title = kwargs.get("title", "")
@@ -43,14 +41,15 @@
     return fig
 
 
 def display_acf_plot(
     data: MetricResult, plot_pacf: bool = False, **kwargs
 ) -> "go.Figure":
     import plotly.graph_objects as go
+    from statsmodels.tsa.stattools import acf, pacf
 
     title = "Partial Autocorrelation (PACF)" if plot_pacf else "Autocorrelation (ACF)"
 
     if not isinstance(data, pd.Series):
         data = pd.Series(data)
 
     corr_array = (
@@ -102,41 +101,31 @@
         data = pd.Series(data)
     fig = px.histogram(data, marginal="box")  # or violin, rug
 
     return fig
 
 
 def calculate_calibration_bins(
-    data: MetricResult, n_bins: int = 10, **kwargs
+    data: MetricResult, pos_label: int, n_bins: int, **kwargs
 ) -> Tuple[np.ndarray, np.ndarray]:
     y_true = data["y"]
     y_prob = data["probs"]
 
-    prob_true, prob_pred = calibration_curve(y_true, y_prob, n_bins=n_bins)
+    prob_true, prob_pred = calibration_curve(
+        y_true, y_prob, pos_label=pos_label, n_bins=n_bins
+    )
     return prob_true, prob_pred
-    # # sort probabilities and corresponding true labels in ascending order
-    # order = np.argsort(y_prob)
-    # y_true = y_true[order]
-    # y_prob = y_prob[order]
-
-    # # calculate fraction of positives at each probability bin
-    # bins = np.arange(0, 1.1, bin_size)
-    # bin_indices = np.digitize(y_prob, bins)
-    # bin_counts = np.bincount(bin_indices, minlength=len(bins) + 1)
 
-    # num_positives = np.cumsum(bin_counts[:-1])
-    # fraction_positives = num_positives / (num_positives + np.sum(y_true))
 
-    # return fraction_positives, bins
-
-
-def callibration_plot(data: MetricResult, n_bins: int = 10, **kwargs) -> "go.Figure":
+def callibration_plot(
+    data: MetricResult, n_bins: int = 8, pos_label: int = 1, **kwargs
+) -> "go.Figure":
     import plotly.graph_objects as go
 
-    fraction_positives, bins = calculate_calibration_bins(data, n_bins)
+    fraction_positives, bins = calculate_calibration_bins(data, pos_label, n_bins)
     scatter = go.Scatter(
         x=bins, y=fraction_positives, mode="lines+markers", name="Data Points"
     )
 
     perfect_calibration = go.Scatter(
         x=[0, 1],
         y=[0, 1],
```

### Comparing `krisi-1.1.1/src/krisi/report/console.py` & `krisi-1.2.0/src/krisi/report/console.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.1/src/krisi/report/graph.py` & `krisi-1.2.0/src/krisi/report/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from pathlib import Path
 from typing import List
 
-import matplotlib.pyplot as plt
 import networkx as nx
 import numpy as np
 import pandas as pd
 from typing_extensions import Literal
 
 from krisi.evaluate.type import PathConst
 from krisi.utils.io import ensure_path
@@ -61,14 +60,16 @@
     G: nx.Graph,
     corr_direction: Literal["positive", "negative"],
     min_correlation: float,
     save_location: Path,
     file_name: str,
     save_or_display: List[Literal["save", "display"]],
 ):
+    import matplotlib.pyplot as plt
+
     # Creates a copy of the graph
     H = G.copy()
 
     # Checks all the edges and removes some based on corr_direction
     for stock1, stock2, weight in G.edges(data=True):
         # if we only want to see the positive correlations we then delete the edges with weight smaller than 0
         if corr_direction == "positive":
```

### Comparing `krisi-1.1.1/src/krisi/report/interactive.py` & `krisi-1.2.0/src/krisi/report/interactive.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.1/src/krisi/report/pdf.py` & `krisi-1.2.0/src/krisi/report/pdf.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.1/src/krisi/report/report.py` & `krisi-1.2.0/src/krisi/report/report.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.1/src/krisi/report/type.py` & `krisi-1.2.0/src/krisi/report/type.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.1/src/krisi/report/vizualise.py` & `krisi-1.2.0/src/krisi/report/vizualise.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.1/src/krisi/report/library/console/diagrams.py` & `krisi-1.2.0/src/krisi/report/library/console/diagrams.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     return plx.build()
 
 
 def callibration_plot(data: pd.Series, width: float, height: float, title: str) -> str:
     plx.clf()
 
-    fraction_positives, bins = calculate_calibration_bins(data)
+    fraction_positives, bins = calculate_calibration_bins(data, pos_label=1, n_bins=8)
     plx.plot(
         bins, fraction_positives, marker="hd", color="red", label="Calibration Curve"
     )
     plx.scatter(
         [0, 0.25, 0.5, 0.75, 1],
         [0, 0.25, 0.5, 0.75, 1],
         label="Perfect Calibration",
```

### Comparing `krisi-1.1.1/src/krisi/report/library/pdf_layouts/scorecard/report.css` & `krisi-1.2.0/src/krisi/report/library/pdf_layouts/scorecard/report.css`

 * *Files identical despite different names*

### Comparing `krisi-1.1.1/src/krisi/report/library/pdf_layouts/scorecard/report.html` & `krisi-1.2.0/src/krisi/report/library/pdf_layouts/scorecard/report.html`

 * *Files identical despite different names*

### Comparing `krisi-1.1.1/src/krisi/utils/console_plot.py` & `krisi-1.2.0/src/krisi/utils/console_plot.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.1/src/krisi/utils/data.py` & `krisi-1.2.0/src/krisi/utils/data.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import itertools
+from random import sample
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
-from statsmodels.tsa.arima_process import ArmaProcess
 
 from krisi.sharedtypes import Task
 
 
 def make_it_stationary(ds: pd.Series) -> pd.Series:
     """If the ds, is a random walk with drift, take first differences to make it stationary."""
     print(f"Making the Series {ds.name} stationary.")
@@ -15,14 +16,16 @@
 
 def generating_arima_synthetic_data(
     target_col: str,
     nsample: int = 1000,
     ar: List[float] = [1.0, -0.9],
     ma: List[float] = [1.0],
 ) -> pd.Series:
+    from statsmodels.tsa.arima_process import ArmaProcess
+
     """Generate Synthetic data with ARIMA process."""
     print(f"Generating Synthetic ARIMA process with nsamples:{nsample}")
 
     # Plot 1: AR parameter = +0.9,
     # exponent of PHI is opposite due to original signal processing literature convention
     ar = np.array(ar)
     ma = np.array(ma)
@@ -168,27 +171,105 @@
     return X, y
 
 
 def generate_synthetic_predictions_binary(
     target: pd.Series,
     sample_weights: Optional[pd.Series] = None,
     index: Optional[pd.Index] = None,
+    smoothing_window: Optional[int] = None,
 ) -> pd.DataFrame:
     if index is None:
         index = target.index
     if sample_weights is None:
         sample_weights = pd.Series(np.ones(len(target)), index=index)
     target = target.copy()
-    target[target == 0.0] = -1
-    prob_mean_class_1 = (target * sample_weights).mean() / 2 + 0.5
-    prob_class_1 = np.random.normal(prob_mean_class_1, 0.1, len(index)).clip(0, 1)
+
+    weighted_target = target * sample_weights
+    expanding_target_mean = weighted_target.expanding(min_periods=1).mean()
+    prob_mean_class_1 = expanding_target_mean.mean()
+    prob_std_class_1 = expanding_target_mean.std()
+    prob_class_1 = pd.Series(
+        np.random.normal(prob_mean_class_1, prob_std_class_1, len(index)).clip(0, 1)
+    )
+
+    if smoothing_window is not None:
+        prob_class_1 = prob_class_1.rolling(
+            window=smoothing_window, min_periods=1
+        ).mean()
+
     prob_class_0 = 1 - prob_class_1
     return pd.DataFrame(
         {
-            "predictions_RandomClassifier": (prob_class_1 > prob_mean_class_1).astype(
-                "int"
-            ),
-            "probabilities_RandomClassifier_0": prob_class_0,
-            "probabilities_RandomClassifier_1": prob_class_1,
+            "predictions_RandomClassifier": (prob_class_1 > prob_class_1.mean())
+            .astype("int")
+            .values,
+            "probabilities_RandomClassifier_0": prob_class_0.values,
+            "probabilities_RandomClassifier_1": prob_class_1.values,
         },
         index=index,
     )
+
+
+def shuffle_df_in_chunks(
+    df: pd.DataFrame, chunk_size: Union[int, float]
+) -> pd.DataFrame:
+    """Shuffles a dataframe by rows in chunks.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Data, whose rows should be shuffled in chunks
+    chunk_size : Union[int, float]
+        Either a fixed chunk size or a fraction of the total number of rows
+
+    Returns
+    -------
+    pd.DataFrame
+        Shuffled DataFrame by rows in chunks.
+    """
+    original_index = df.index
+    df = df.reset_index(drop=True)
+    chunk_size = (
+        int(chunk_size * len(df)) if isinstance(chunk_size, float) else chunk_size
+    )
+    num_rows = df.shape[0]
+    num_chunks = num_rows // chunk_size
+    shuffled_idx = []
+    for i in sample(list(range(num_chunks)), num_chunks):
+        start_idx = i * chunk_size
+        end_idx = (i + 1) * chunk_size
+        shuffled_idx.append(df.index[start_idx:end_idx])
+
+    # If there are any remaining rows, shuffle and append them as well
+    if num_rows % chunk_size != 0:
+        shuffled_idx.append(df.index[num_chunks * chunk_size :])
+
+    df = df.copy()
+    df.index = df.index[np.concatenate(shuffled_idx)]
+    df.sort_index(inplace=True)
+    df.index = original_index
+
+    return df
+
+
+def combinatorial_shuffling_in_chunks(
+    df: pd.DataFrame, chunk_size: int, select_index: int
+) -> pd.DataFrame:
+    original_index = df.index
+    df = df.reset_index(drop=True)
+    chunks = [(i, i + chunk_size) for i in range(0, len(df), chunk_size)]
+    if chunks[-1][1] > len(df):
+        chunks[-2] = (chunks[-2][0], len(df))
+        chunks = chunks[:-1]
+
+    premuted_chunks = list(itertools.permutations(chunks))[
+        1:
+    ]  # skip the first one, which is the original order
+
+    flatten_ranges = [
+        id for start, stop in premuted_chunks[select_index] for id in range(start, stop)
+    ]
+    df = df.copy()
+    df.index = df.index[flatten_ranges]
+    df.sort_index(inplace=True)
+    df.index = original_index
+    return df
```

### Comparing `krisi-1.1.1/src/krisi/utils/environment.py` & `krisi-1.2.0/src/krisi/utils/environment.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.1/src/krisi/utils/io.py` & `krisi-1.2.0/src/krisi/utils/io.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.1/src/krisi/utils/iterable_helpers.py` & `krisi-1.2.0/src/krisi/utils/iterable_helpers.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.1/src/krisi/utils/printing.py` & `krisi-1.2.0/src/krisi/utils/printing.py`

 * *Files identical despite different names*

### Comparing `krisi-1.1.1/src/krisi/utils/devutils/timing.py` & `krisi-1.2.0/src/krisi/utils/devutils/timing.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from time import monotonic
+from typing import Any, Callable, Tuple
 
 import numpy as np
 import pandas as pd
 from sklearn.metrics import mean_absolute_error
 
 from krisi import score
 from krisi.evaluate.type import Calculation
@@ -14,19 +15,20 @@
 y = pd.Series(np.random.rand(lengthofdataset), name="y")
 predictions = pd.Series(np.random.rand(lengthofdataset), name="predictions")
 
 
 window = 30
 
 
-def timeingit(func):
+def timeingit(func: Callable) -> Tuple[Any, float]:
     start_time = monotonic()
     res = func()
-    print(f"Run time: {monotonic() - start_time} seconds")
-    return res
+    runtime = monotonic() - start_time
+    print(f"Run time: {runtime} seconds")
+    return res, runtime
 
 
 def func1():
     return [
         func(y_roll, predictions[y_roll.index])
         for y_roll in y.rolling(window=window, step=window)
     ]
```

### Comparing `krisi-1.1.1/.gitignore` & `krisi-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `krisi-1.1.1/LICENSE` & `krisi-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `krisi-1.1.1/README.md` & `krisi-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `krisi-1.1.1/pyproject.toml` & `krisi-1.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "krisi"
-version = "1.1.1"
+version = "1.2.0"
 authors = [
   { name="Mark Szulyovszky", email="mark@dreamfaster.ai" },
   { name="Daniel Szemerey", email="daniel@dreamfaster.ai" },
 ]
 description = "Testing and Reporting framework for Time Series Analysis"
 readme = "README.md"
 license = { file="LICENSE" }
@@ -34,15 +34,14 @@
 
   #Plotting libraries
   "rich",
   "tqdm",
   "plotext",
 
   #TS and Modeling libraries
-  "statsmodels >=0.12.1",
   "scikit-learn"
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project.urls]
@@ -79,16 +78,20 @@
 plotting = [
   "plotly",
   "dash",
   "jupyter_dash",
   "weasyprint",
   "kaleido",
   "pangocffi",
+  "statsmodels >=0.12.1",
+]
+analysis=[
   "matplotlib",
-  "networkx"
+  "networkx",
+  "statsmodels >=0.12.1",
 ]
 
 [tool.hatch.envs.quality]
 dependencies = [
   "krisi[quality]"
 ]
 detached = true
@@ -134,15 +137,15 @@
   "src",
   ".",
 ]
 testpaths = ["tests"] 
 
 # bumpver command: ``bumpver update --patch``
 [tool.bumpver]
-current_version = "1.1.1"
+current_version = "1.2.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore(Release): Bump version from {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `krisi-1.1.1/PKG-INFO` & `krisi-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krisi
-Version: 1.1.1
+Version: 1.2.0
 Summary: Testing and Reporting framework for Time Series Analysis
 Project-URL: Documentation, https://dream-faster.github.io/krisi
 Project-URL: Issues, https://github.com/dream-faster/krisi/issues
 Project-URL: Source, https://github.com/dream-faster/krisi
 Author-email: Mark Szulyovszky <mark@dreamfaster.ai>, Daniel Szemerey <daniel@dreamfaster.ai>
 License: MIT License
         
@@ -56,34 +56,36 @@
 Requires-Dist: dill
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: plotext
 Requires-Dist: pytest
 Requires-Dist: rich
 Requires-Dist: scikit-learn
-Requires-Dist: statsmodels>=0.12.1
 Requires-Dist: tqdm
 Requires-Dist: typing-extensions
+Provides-Extra: analysis
+Requires-Dist: matplotlib; extra == 'analysis'
+Requires-Dist: networkx; extra == 'analysis'
+Requires-Dist: statsmodels>=0.12.1; extra == 'analysis'
 Provides-Extra: docs
 Requires-Dist: image; extra == 'docs'
 Requires-Dist: mkdocs-autorefs; extra == 'docs'
 Requires-Dist: mkdocs-gallery==0.7.6; extra == 'docs'
 Requires-Dist: mkdocs-glightbox>=0.3; extra == 'docs'
 Requires-Dist: mkdocs-include-markdown-plugin; extra == 'docs'
 Requires-Dist: mkdocs-jupyter; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
 Requires-Dist: mkdocstrings-python; extra == 'docs'
 Provides-Extra: plotting
 Requires-Dist: dash; extra == 'plotting'
 Requires-Dist: jupyter-dash; extra == 'plotting'
 Requires-Dist: kaleido; extra == 'plotting'
-Requires-Dist: matplotlib; extra == 'plotting'
-Requires-Dist: networkx; extra == 'plotting'
 Requires-Dist: pangocffi; extra == 'plotting'
 Requires-Dist: plotly; extra == 'plotting'
+Requires-Dist: statsmodels>=0.12.1; extra == 'plotting'
 Requires-Dist: weasyprint; extra == 'plotting'
 Provides-Extra: quality
 Requires-Dist: black~=22.10.0; extra == 'quality'
 Requires-Dist: flake8~=4.0.1; extra == 'quality'
 Requires-Dist: isort~=5.10.1; extra == 'quality'
 Requires-Dist: pre-commit~=2.20.0; extra == 'quality'
 Provides-Extra: tests
```

