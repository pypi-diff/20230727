# Comparing `tmp/klib-1.0.7.tar.gz` & `tmp/klib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klib-1.0.7.tar", max compression
+gzip compressed data, was "klib-1.1.0.tar", max compression
```

## Comparing `klib-1.0.7.tar` & `klib-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1069 2022-07-29 17:32:38.054377 klib-1.0.7/LICENSE
--rw-r--r--   0        0        0     5622 2022-11-15 06:45:57.292065 klib-1.0.7/README.md
--rw-r--r--   0        0        0     2043 2022-11-24 15:04:13.326100 klib-1.0.7/pyproject.toml
--rw-r--r--   0        0        0      933 2022-11-24 15:04:44.719569 klib-1.0.7/src/klib/__init__.py
--rw-r--r--   0        0        0       54 2022-11-24 15:04:26.122192 klib-1.0.7/src/klib/_version.py
--rw-r--r--   0        0        0    20719 2022-11-24 15:05:30.023479 klib-1.0.7/src/klib/clean.py
--rw-r--r--   0        0        0    27168 2022-11-24 15:10:18.549582 klib-1.0.7/src/klib/describe.py
--rw-r--r--   0        0        0     1759 2022-09-16 18:22:27.368052 klib-1.0.7/src/klib/scripts/performance.py
--rw-r--r--   0        0        0     9569 2022-11-24 15:08:49.217718 klib-1.0.7/src/klib/utils.py
--rw-r--r--   0        0        0        0 2022-07-29 17:32:38.390459 klib-1.0.7/tests/__init__.py
--rw-r--r--   0        0        0    11220 2022-11-14 07:54:26.687324 klib-1.0.7/tests/test_clean.py
--rw-r--r--   0        0        0     3803 2022-11-24 15:09:34.237802 klib-1.0.7/tests/test_describe.py
--rw-r--r--   0        0        0     9236 2022-09-18 15:07:59.633763 klib-1.0.7/tests/test_util.py
--rw-r--r--   0        0        0     6577 1970-01-01 00:00:00.000000 klib-1.0.7/setup.py
--rw-r--r--   0        0        0     6418 1970-01-01 00:00:00.000000 klib-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-07-29 17:32:38.054377 klib-1.1.0/LICENSE
+-rw-r--r--   0        0        0     6641 2023-07-27 15:29:23.883519 klib-1.1.0/README.md
+-rw-r--r--   0        0        0     2791 2023-07-27 16:14:46.581492 klib-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1033 2023-07-27 16:15:40.773253 klib-1.1.0/src/klib/__init__.py
+-rw-r--r--   0        0        0       54 2023-07-27 16:12:00.886675 klib-1.1.0/src/klib/_version.py
+-rw-r--r--   0        0        0    20871 2023-07-27 15:29:23.896625 klib-1.1.0/src/klib/clean.py
+-rw-r--r--   0        0        0    35236 2023-07-27 16:14:17.270224 klib-1.1.0/src/klib/describe.py
+-rw-r--r--   0        0        0        0 2023-07-27 15:29:23.897081 klib-1.1.0/src/klib/scripts/__init__.py
+-rw-r--r--   0        0        0     1745 2023-07-27 15:29:23.897579 klib-1.1.0/src/klib/scripts/performance.py
+-rw-r--r--   0        0        0     9779 2023-07-27 15:29:23.897878 klib-1.1.0/src/klib/utils.py
+-rw-r--r--   0        0        0        0 2022-07-29 17:32:38.390459 klib-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0    10815 2023-07-27 15:29:23.898195 klib-1.1.0/tests/test_clean.py
+-rw-r--r--   0        0        0     3799 2023-07-27 15:29:23.898345 klib-1.1.0/tests/test_describe.py
+-rw-r--r--   0        0        0     9181 2023-07-27 15:29:23.898650 klib-1.1.0/tests/test_util.py
+-rw-r--r--   0        0        0     7508 1970-01-01 00:00:00.000000 klib-1.1.0/PKG-INFO
```

### Comparing `klib-1.0.7/LICENSE` & `klib-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `klib-1.0.7/README.md` & `klib-1.1.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -73,14 +73,32 @@
 ```python
 klib.corr_plot(df, target='wine') # default representation of correlations with the feature column
 ```
 
 <p align="center"><img src="https://raw.githubusercontent.com/akanz1/klib/main/examples/images/example_target_corr_plot.png" alt="Target Corr Plot Example" width="720" height="600"></p>
 
 ```python
+klib.corr_interactive_plot(df, split="neg").show()
+
+# The interactive plot has the same parameters as the corr_plot, but with additional Plotly heatmap graph object kwargs.
+klib.corr_interactive_plot(df, split="neg", zmax=0)
+```
+
+<p align="center"><img src="https://github.com/akanz1/klib/assets/124513922/27b79ece-dc22-410c-9816-fcc4cfc97edc"  alt="Interactive Corr Plot Simple Example" width="720" height="600"></p>
+
+<p align="center"><img src="https://github.com/akanz1/klib/assets/124513922/d986dc6c-84dc-4693-b276-6b4df7023e0f" alt="Interactive Corr Plot with zmax kwarg Example" width="720" height="600"></p>
+
+```python
+#Since corr_interactive_plot returns a Graph Object Figure, it supports the update_layout chain method.
+klib.corr_interactive_plot(wine, split="neg").update_layout(template="simple_white")
+```
+
+<p align="center"><img src="https://github.com/akanz1/klib/assets/124513922/fb7ac102-6daf-4e30-a24c-db168c7cf42c" alt="Interactive Corr Plot Chained Example" width="720" height="600"></p>
+
+```python
 klib.dist_plot(df) # default representation of a distribution plot, other settings include fill_range, histogram, ...
 ```
 
 <p align="center"><img src="https://raw.githubusercontent.com/akanz1/klib/main/examples/images/example_dist_plot.png" alt="Dist Plot Example" width="910" height="130"></p>
 
 ```python
 klib.cat_plot(data, top=4, bottom=4) # representation of the 4 most & least common values in each categorical column
```

#### html2text {}

```diff
@@ -48,14 +48,24 @@
 ```python klib.corr_plot(df, split='pos') # displaying only positive
 correlations, other settings include threshold, cmap... klib.corr_plot(df,
 split='neg') # displaying only negative correlations ```
                               [Corr Plot Example]
 ```python klib.corr_plot(df, target='wine') # default representation of
 correlations with the feature column ```
                           [Target Corr Plot Example]
+```python klib.corr_interactive_plot(df, split="neg").show() # The interactive
+plot has the same parameters as the corr_plot, but with additional Plotly
+heatmap graph object kwargs. klib.corr_interactive_plot(df, split="neg",
+zmax=0) ```
+                    [Interactive Corr Plot Simple Example]
+                [Interactive Corr Plot with zmax kwarg Example]
+```python #Since corr_interactive_plot returns a Graph Object Figure, it
+supports the update_layout chain method. klib.corr_interactive_plot(wine,
+split="neg").update_layout(template="simple_white") ```
+                    [Interactive Corr Plot Chained Example]
 ```python klib.dist_plot(df) # default representation of a distribution plot,
 other settings include fill_range, histogram, ... ```
                               [Dist Plot Example]
 ```python klib.cat_plot(data, top=4, bottom=4) # representation of the 4 most &
 least common values in each categorical column ```
                               [Cat Plot Example]
 Further examples, as well as applications of the functions in **klib.clean()**
```

### Comparing `klib-1.0.7/src/klib/__init__.py` & `klib-1.1.0/src/klib/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-"""
-Data Science Module for Python
+"""Data cleaning and visualisation functions for Python.
+
 ===============================
 klib is an easy to use Python library of customized functions for cleaning and \
 analyzing data.
 """
 
 __author__ = """Andreas Kanz"""
 
@@ -11,26 +11,28 @@
 from klib.clean import clean_column_names
 from klib.clean import convert_datatypes
 from klib.clean import data_cleaning
 from klib.clean import drop_missing
 from klib.clean import mv_col_handling
 from klib.clean import pool_duplicate_subsets
 from klib.describe import cat_plot
+from klib.describe import corr_interactive_plot
 from klib.describe import corr_mat
 from klib.describe import corr_plot
 from klib.describe import dist_plot
 from klib.describe import missingval_plot
 
 __all__ = [
+    "__version__",
+    "cat_plot",
     "clean_column_names",
     "convert_datatypes",
-    "data_cleaning",
-    "drop_missing",
-    "mv_col_handling",
-    "pool_duplicate_subsets",
-    "cat_plot",
+    "corr_interactive_plot",
     "corr_mat",
     "corr_plot",
+    "data_cleaning",
     "dist_plot",
+    "drop_missing",
     "missingval_plot",
-    "__version__",
+    "mv_col_handling",
+    "pool_duplicate_subsets",
 ]
```

### Comparing `klib-1.0.7/src/klib/clean.py` & `klib-1.1.0/src/klib/clean.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 :author: Andreas Kanz
 """
 from __future__ import annotations
 
 import itertools
 import re
 from typing import Literal
-from typing import Optional
 
 import numpy as np
 import pandas as pd
 
 from klib.describe import corr_mat
 from klib.utils import _diff_report
 from klib.utils import _drop_duplicates
@@ -25,30 +24,31 @@
     "data_cleaning",
     "drop_missing",
     "mv_col_handling",
 ]
 
 
 def _optimize_ints(data: pd.Series | pd.DataFrame) -> pd.DataFrame:
-    df = pd.DataFrame(data).copy()
+    df = pd.DataFrame(data).copy()  # noqa: PD901
     ints = df.select_dtypes(include=["int64"]).columns.tolist()
     df[ints] = df[ints].apply(pd.to_numeric, downcast="integer")
     return df
 
 
 def _optimize_floats(data: pd.Series | pd.DataFrame) -> pd.DataFrame:
     data = pd.DataFrame(data).copy()
     floats = data.select_dtypes(include=["float64"]).columns.tolist()
     data[floats] = data[floats].apply(pd.to_numeric, downcast="float")
     return data
 
 
 def clean_column_names(data: pd.DataFrame, hints: bool = True) -> pd.DataFrame:
-    """Clean the column names of the provided Pandas Dataframe and optionally \
-        provides hints on duplicate and long column names.
+    """Clean the column names of the provided Pandas Dataframe.
+
+    Optionally provides hints on duplicate and long column names.
 
     Parameters
     ----------
     data : pd.DataFrame
         Original Dataframe with columns to be cleaned
     hints : bool, optional
         Print out hints on column name duplication and colum name length, by default \
@@ -63,15 +63,15 @@
 
     # Handle CamelCase
     for i, col in enumerate(data.columns):
         matches = re.findall(re.compile("[a-z][A-Z]"), col)
         column = col
         for match in matches:
             column = column.replace(match, f"{match[0]}_{match[1]}")
-            data.rename(columns={data.columns[i]: column}, inplace=True)
+            data = data.rename(columns={data.columns[i]: column})
 
     data.columns = (
         data.columns.str.replace("\n", "_", regex=False)
         .str.replace("(", "_", regex=False)
         .str.replace(")", "_", regex=False)
         .str.replace("'", "_", regex=False)
         .str.replace('"', "_", regex=False)
@@ -98,40 +98,44 @@
         .str.strip("_")
         .str.lower()
     )
 
     if dupl_idx := [i for i, x in enumerate(data.columns.duplicated()) if x]:
         dupl_before = data.columns[dupl_idx].tolist()
         data.columns = [
-            col if col not in data.columns[:i] else f"{col}_{str(i)}"
+            col if col not in data.columns[:i] else f"{col}_{i!s}"
             for i, col in enumerate(data.columns)
         ]
-
+        print_statement = ""
         if hints:
-            print(
+            # add string to print statement
+            print_statement = (
                 f"Duplicate column names detected! Columns with index {dupl_idx} and "
-                f"names {dupl_before}) have been renamed to "
-                f"{data.columns[dupl_idx].tolist()}."
+                f"names {dupl_before} have been renamed to "
+                f"{data.columns[dupl_idx].tolist()}.",
             )
 
-    long_col_names = [x for x in data.columns if len(x) > 25]
-    if long_col_names and hints:
-        print(
-            "Long column names detected (>25 characters). Consider renaming the "
-            f"following columns {long_col_names}."
-        )
+            if long_col_names := [
+                x for x in data.columns if len(x) > 25  # noqa: PLR2004
+            ]:
+                print_statement += (
+                    "Long column names detected (>25 characters). Consider renaming "
+                    f"the following columns {long_col_names}.",
+                )
+
+            print(print_statement)
 
     return data
 
 
 def convert_datatypes(
     data: pd.DataFrame,
     category: bool = True,
     cat_threshold: float = 0.05,
-    cat_exclude: Optional[list[str | int]] = None,
+    cat_exclude: list[str | int] | None = None,
 ) -> pd.DataFrame:
     """Convert columns to best possible dtypes using dtypes supporting pd.NA.
 
     Temporarily not converting to integers due to an issue in pandas. This is expected \
         to be fixed in pandas 1.1. See https://github.com/pandas-dev/pandas/issues/33803
 
     Parameters
@@ -171,28 +175,27 @@
 
         data[col] = data[col].convert_dtypes(
             convert_integer=False,
             convert_floating=False,
         )
 
     data = _optimize_ints(data)
-    data = _optimize_floats(data)
-
-    return data
+    return _optimize_floats(data)
 
 
 def drop_missing(
     data: pd.DataFrame,
     drop_threshold_cols: float = 1,
     drop_threshold_rows: float = 1,
-    col_exclude: Optional[list[str]] = None,
+    col_exclude: list[str] | None = None,
 ) -> pd.DataFrame:
-    """Drop completely empty columns and rows by default and optionally provides \
-        flexibility to loosen restrictions to drop additional non-empty columns and \
-        rows based on the fraction of NA-values.
+    """Drop completely empty columns and rows by default.
+
+    Optionally provides flexibility to loosen restrictions to drop additional \
+    non-empty columns and rows based on the fraction of NA-values.
 
     Parameters
     ----------
     data : pd.DataFrame
         2D dataset that can be coerced into Pandas DataFrame
     drop_threshold_cols : float, optional
         Drop columns with NA-ratio equal to or above the specified threshold, by \
@@ -220,42 +223,46 @@
     data_exclude = data[col_exclude]
 
     data = pd.DataFrame(data).copy()
 
     data_dropped = data.drop(columns=col_exclude, errors="ignore")
     data_dropped = data_dropped.drop(
         columns=data_dropped.loc[
-            :, _missing_vals(data)["mv_cols_ratio"] > drop_threshold_cols
-        ].columns
+            :,
+            _missing_vals(data)["mv_cols_ratio"] > drop_threshold_cols,
+        ].columns,
     ).dropna(axis=1, how="all")
 
     data = pd.concat([data_dropped, data_exclude], axis=1)
 
     return data.drop(
         index=data.loc[
-            _missing_vals(data)["mv_rows_ratio"] > drop_threshold_rows, :
-        ].index
+            _missing_vals(data)["mv_rows_ratio"] > drop_threshold_rows,
+            :,
+        ].index,
     ).dropna(axis=0, how="all")
 
 
 def data_cleaning(
     data: pd.DataFrame,
     drop_threshold_cols: float = 0.9,
     drop_threshold_rows: float = 0.9,
     drop_duplicates: bool = True,
     convert_dtypes: bool = True,
-    col_exclude: Optional[list[str]] = None,
+    col_exclude: list[str] | None = None,
     category: bool = True,
     cat_threshold: float = 0.03,
-    cat_exclude: Optional[list[str | int]] = None,
+    cat_exclude: list[str | int] | None = None,
     clean_col_names: bool = True,
-    show: Optional[Literal["all", "changes"]] = "changes",
+    show: Literal["all", "changes"] | None = "changes",
 ) -> pd.DataFrame:
-    """Perform initial data cleaning tasks on a dataset, such as dropping single \
-        valued and empty rows, empty columns as well as optimizing the datatypes.
+    """Perform initial data cleaning tasks on a dataset.
+
+    For example dropping single valued and empty rows, empty columns as well as \
+    optimizing the datatypes.
 
     Parameters
     ----------
     data : pd.DataFrame
         2D dataset that can be coerced into Pandas DataFrame
     drop_threshold_cols : float, optional
         Drop columns with NA-ratio equal to or above the specified threshold, by \
@@ -317,22 +324,25 @@
     _validate_input_bool(drop_duplicates, "drop_duplicates")
     _validate_input_bool(convert_dtypes, "convert_datatypes")
     _validate_input_bool(category, "category")
     _validate_input_range(cat_threshold, "cat_threshold", 0, 1)
 
     data = pd.DataFrame(data).copy()
     data_cleaned = drop_missing(
-        data, drop_threshold_cols, drop_threshold_rows, col_exclude=col_exclude
+        data,
+        drop_threshold_cols,
+        drop_threshold_rows,
+        col_exclude=col_exclude,
     )
 
     if clean_col_names:
         data_cleaned = clean_column_names(data_cleaned)
 
     single_val_cols = data_cleaned.columns[
-        data_cleaned.nunique(dropna=False) == 1
+        data_cleaned.nunique(dropna=False) == 1  # noqa: PD101
     ].tolist()
     single_val_cols = [col for col in single_val_cols if col not in col_exclude]
     data_cleaned = data_cleaned.drop(columns=single_val_cols)
 
     dupl_rows = None
 
     if drop_duplicates:
@@ -354,22 +364,23 @@
     )
 
     return data_cleaned
 
 
 def mv_col_handling(
     data: pd.DataFrame,
-    target: Optional[str | pd.Series | list[str]] = None,
+    target: str | pd.Series | list[str] | None = None,
     mv_threshold: float = 0.1,
     corr_thresh_features: float = 0.5,
     corr_thresh_target: float = 0.3,
     return_details: bool = False,
 ) -> pd.DataFrame | tuple[pd.DataFrame, list[str], list[str]]:
-    """Convert columns with a high ratio of missing values into binary features and \
-    eventually drops them based on their correlation with other features and the \
+    """Convert columns with a high ratio of missing values into binary features.
+
+    Eventually drops them based on their correlation with other features and the \
     target variable.
 
     This function follows a three step process:
     - 1) Identify features with a high ratio of missing values (above 'mv_threshold').
     - 2) Identify high correlations of these features among themselves and with \
         other features in the dataset (above 'corr_thresh_features').
     - 3) Features with high ratio of missing values and high correlation among each \
@@ -418,15 +429,15 @@
     _validate_input_range(corr_thresh_target, "corr_thresh_target", 0, 1)
 
     data = pd.DataFrame(data).copy()
     data_local = data.copy()
     mv_ratios = _missing_vals(data_local)["mv_cols_ratio"]
     cols_mv = mv_ratios[mv_ratios > mv_threshold].index.tolist()
     data_local[cols_mv] = (
-        data_local[cols_mv].applymap(lambda x: x if pd.isnull(x) else 1).fillna(0)
+        data_local[cols_mv].applymap(lambda x: x if pd.isna(x) else 1).fillna(0)
     )
 
     high_corr_features = []
     data_temp = data_local.copy()
     for col in cols_mv:
         corrmat = corr_mat(data_temp, colored=False)
         if abs(corrmat[col]).nlargest(2)[1] > corr_thresh_features:
@@ -447,27 +458,28 @@
 
 
 def pool_duplicate_subsets(
     data: pd.DataFrame,
     col_dupl_thresh: float = 0.2,
     subset_thresh: float = 0.2,
     min_col_pool: int = 3,
-    exclude: Optional[list[str]] = None,
+    exclude: list[str] | None = None,
     return_details: bool = False,
 ) -> pd.DataFrame | tuple[pd.DataFrame, list[str]]:
-    """Check for duplicates in subsets of columns and pools them. This can reduce \
-        the number of columns in the data without loosing much information. Suitable \
-        columns are combined to subsets and tested for duplicates. In case sufficient \
-        duplicates can be found, the respective columns are aggregated into a \
-        "pooled_var" column. Identical numbers in the "pooled_var" column indicate \
-        identical information in the respective rows.
-
-        Note:  It is advised to exclude features that provide sufficient informational \
-        content by themselves as well as the target column by using the "exclude" \
-        setting.
+    """Check for duplicates in subsets of columns and pools them.
+
+    This can reduce the number of columns in the data without loosing much \
+    information. Suitable columns are combined to subsets and tested for duplicates. \
+    In case sufficient duplicates can be found, the respective columns are aggregated \
+    into a "pooled_var" column. Identical numbers in the "pooled_var" column indicate \
+    identical information in the respective rows.
+
+    Note:  It is advised to exclude features that provide sufficient informational \
+    content by themselves as well as the target column by using the "exclude" \
+    setting.
 
     Parameters
     ----------
     data : pd.DataFrame
         2D dataset that can be coerced into Pandas DataFrame
     col_dupl_thresh : float, optional
         Columns with a ratio of duplicates higher than "col_dupl_thresh" are \
@@ -530,24 +542,24 @@
             # Get the best possible iterator and process the data
             best_subset = itertools.islice(
                 itertools.combinations(check, len(check) - i),
                 max_idx,
                 max_idx + 1,
             )
 
-            best_subset = data[list(list(best_subset)[0])]
+            best_subset = data[list(next(iter(best_subset)))]
             subset_cols = best_subset.columns.tolist()
 
             unique_subset = (
                 best_subset.drop_duplicates()
                 .reset_index()
                 .rename(columns={"index": "pooled_vars"})
             )
             data = data.merge(unique_subset, how="left", on=subset_cols).drop(
-                columns=subset_cols
+                columns=subset_cols,
             )
             data.index = pd.RangeIndex(len(data))
             break
 
     data = pd.concat([data, pd.DataFrame(excluded_cols)], axis=1)
 
     return (data, subset_cols) if return_details else data
```

### Comparing `klib-1.0.7/src/klib/describe.py` & `klib-1.1.0/src/klib/describe.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,48 +3,55 @@
 :author: Andreas Kanz
 
 """
 from __future__ import annotations
 
 from typing import Any
 from typing import Literal
-from typing import Optional
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+import plotly.graph_objects as go
 import scipy
 import seaborn as sns
 from matplotlib import ticker
 from matplotlib.colors import LinearSegmentedColormap
 from matplotlib.colors import to_rgb
-from matplotlib.gridspec import GridSpec
+from matplotlib.gridspec import GridSpec  # noqa: TCH002
+from screeninfo import get_monitors
 
 from klib.utils import _corr_selector
 from klib.utils import _missing_vals
 from klib.utils import _validate_input_bool
 from klib.utils import _validate_input_int
 from klib.utils import _validate_input_num_data
 from klib.utils import _validate_input_range
 from klib.utils import _validate_input_smaller
 from klib.utils import _validate_input_sum_larger
 
-__all__ = ["cat_plot", "corr_mat", "corr_plot", "dist_plot", "missingval_plot"]
+__all__ = [
+    "cat_plot",
+    "corr_interactive_plot",
+    "corr_mat",
+    "corr_plot",
+    "dist_plot",
+    "missingval_plot",
+]
 
 
-def cat_plot(
+def cat_plot(  # noqa: C901, PLR0915
     data: pd.DataFrame,
     figsize: tuple[float, float] = (18, 18),
     top: int = 3,
     bottom: int = 3,
     bar_color_top: str = "#5ab4ac",
     bar_color_bottom: str = "#d8b365",
 ) -> GridSpec:
-    """Two-dimensional visualization of the number and frequency of categorical \
-        features.
+    """Two-dimensional visualization of number and frequency of categorical features.
 
     Parameters
     ----------
     data : pd.DataFrame
         2D dataset that can be coerced into Pandas DataFrame. If a Pandas DataFrame \
         is provided, the index/column information is used to label the plots
     figsize : tuple[float, float], optional
@@ -107,38 +114,44 @@
             value_counts_top = value_counts_idx_top = []
 
         if bottom == 0:
             value_counts_bot = value_counts_idx_bot = []
 
         data.loc[data[col].isin(value_counts_idx_top), col] = 10
         data.loc[data[col].isin(value_counts_idx_bot), col] = 0
-        data.loc[((data[col] != 10) & (data[col] != 0)), col] = 5
+        data.loc[((data[col] != 10) & (data[col] != 0)), col] = 5  # noqa: PLR2004
         data[col] = data[col].rolling(2, min_periods=1).mean()
 
         value_counts_idx_top = [elem[:20] for elem in value_counts_idx_top]
         value_counts_idx_bot = [elem[:20] for elem in value_counts_idx_bot]
         sum_top = sum(value_counts_top)
         sum_bot = sum(value_counts_bot)
 
         # Barcharts
         ax_top = fig.add_subplot(gs[:1, count : count + 1])
         ax_top.bar(
-            value_counts_idx_top, value_counts_top, color=bar_color_top, width=0.85
+            value_counts_idx_top,
+            value_counts_top,
+            color=bar_color_top,
+            width=0.85,
         )
         ax_top.bar(
-            value_counts_idx_bot, value_counts_bot, color=bar_color_bottom, width=0.85
+            value_counts_idx_bot,
+            value_counts_bot,
+            color=bar_color_bottom,
+            width=0.85,
         )
         ax_top.set(frame_on=False)
         ax_top.tick_params(axis="x", labelrotation=90)
 
         # Summary stats
         ax_bottom = fig.add_subplot(gs[1:2, count : count + 1])
         plt.subplots_adjust(hspace=0.075)
-        ax_bottom.get_yaxis().set_visible(False)
-        ax_bottom.get_xaxis().set_visible(False)
+        ax_bottom.get_yaxis().set_visible(False)  # noqa: FBT003
+        ax_bottom.get_xaxis().set_visible(False)  # noqa: FBT003
         ax_bottom.set(frame_on=False)
         ax_bottom.text(
             0,
             0,
             f"Unique values: {n_unique}\n\n"
             f"Top {lim_top}: {sum_top} ({sum_top/data.shape[0]*100:.1f}%)\n"
             f"Bot {lim_bot}: {sum_bot} ({sum_bot/data.shape[0]*100:.1f}%)",
@@ -148,39 +161,45 @@
         )
 
     # Heatmap
     color_bot_rgb = to_rgb(bar_color_bottom)
     color_white = to_rgb("#FFFFFF")
     color_top_rgb = to_rgb(bar_color_top)
     cat_plot_cmap = LinearSegmentedColormap.from_list(
-        "cat_plot_cmap", [color_bot_rgb, color_white, color_top_rgb], N=200
+        "cat_plot_cmap",
+        [color_bot_rgb, color_white, color_top_rgb],
+        N=200,
     )
     ax_hm = fig.add_subplot(gs[2:, :])
     sns.heatmap(data, cmap=cat_plot_cmap, cbar=False, vmin=0, vmax=10, ax=ax_hm)
     ax_hm.set_yticks(np.round(ax_hm.get_yticks()[::5], -1))
     ax_hm.set_yticklabels(ax_hm.get_yticks())
     ax_hm.set_xticklabels(
         ax_hm.get_xticklabels(),
         horizontalalignment="center",
         fontweight="light",
         fontsize="medium",
     )
     ax_hm.tick_params(length=1, colors="#111111")
     gs.figure.suptitle(
-        "Categorical data plot", x=0.5, y=0.91, fontsize=18, color="#111111"
+        "Categorical data plot",
+        x=0.5,
+        y=0.91,
+        fontsize=18,
+        color="#111111",
     )
 
     return gs
 
 
 def corr_mat(
     data: pd.DataFrame,
-    split: Optional[Literal["pos", "neg", "high", "low"]] = None,
+    split: Literal["pos", "neg", "high", "low"] | None = None,
     threshold: float = 0,
-    target: Optional[pd.DataFrame | pd.Series | np.ndarray | str] = None,
+    target: pd.DataFrame | pd.Series | np.ndarray | str | None = None,
     method: Literal["pearson", "spearman", "kendall"] = "pearson",
     colored: bool = True,
 ) -> pd.DataFrame | pd.Series:
     """Return a color-encoded correlation matrix.
 
     Parameters
     ----------
@@ -233,15 +252,15 @@
             data = data.drop(target, axis=1)
 
         elif isinstance(target, (list, pd.Series, np.ndarray)):
             target_data = pd.Series(target)
             target = target_data.name
 
         corr = pd.DataFrame(
-            data.corrwith(target_data, method=method, numeric_only=True)
+            data.corrwith(target_data, method=method, numeric_only=True),
         )
         corr = corr.sort_values(corr.columns[0], ascending=False)
         corr.columns = [target]
 
     else:
         corr = data.corr(method=method, numeric_only=True)
 
@@ -250,26 +269,25 @@
     if colored:
         return corr.style.applymap(color_negative_red).format("{:.2f}", na_rep="-")
     return corr
 
 
 def corr_plot(
     data: pd.DataFrame,
-    split: Optional[Literal["pos", "neg", "high", "low"]] = None,
+    split: Literal["pos", "neg", "high", "low"] | None = None,
     threshold: float = 0,
-    target: Optional[pd.Series | str] = None,
+    target: pd.Series | str | None = None,
     method: Literal["pearson", "spearman", "kendall"] = "pearson",
     cmap: str = "BrBG",
     figsize: tuple[float, float] = (12, 10),
     annot: bool = True,
     dev: bool = False,
-    **kwargs,
+    **kwargs,  # noqa: ANN003
 ) -> plt.Axes:
-    """Two-dimensional visualization of the correlation between feature-columns \
-        excluding NA values.
+    """2D visualization of the correlation between feature-columns excluding NA values.
 
     Parameters
     ----------
     data : pd.DataFrame
         2D dataset that can be coerced into Pandas DataFrame. If a Pandas DataFrame \
         is provided, the index/column information is used to label the plots
     split : Optional[str], optional
@@ -405,27 +423,242 @@
             y=0.85,
             ha="left",
         )
 
     return ax
 
 
+def corr_interactive_plot(
+    data: pd.DataFrame,
+    split: Literal["pos", "neg", "high", "low"] | None = None,
+    threshold: float = 0.0,
+    target: pd.Series | str | None = None,
+    method: Literal["pearson", "spearman", "kendall"] = "pearson",
+    cmap: str = "BrBG",
+    figsize: tuple[float, float] = (12, 10),
+    annot: bool = True,
+    **kwargs,  # noqa: ANN003
+) -> go.Figure:
+    """Interactive 2D visualization of the correlation between feature-columns.
+
+    Parameters
+    ----------
+    data : pd.DataFrame
+        2D dataset that can be coerced into a Pandas DataFrame. If a
+        Pandas DataFrame is provided, the index/column information is
+        used to label the plots.
+
+    split : Optional[str], optional
+        Type of split to be performed
+        {None, "pos", "neg", "high", "low"}, by default None
+
+        - None: visualize all correlations between the feature-columns
+
+        - pos: visualize all positive correlations between the
+            feature-columns above the threshold
+
+        - neg: visualize all negative correlations between the
+            feature-columns below the threshold
+
+        - high: visualize all correlations between the
+            feature-columns for which abs(corr) > threshold is True
+
+        - low: visualize all correlations between the
+            feature-columns for which abs(corr) < threshold is True
+
+    threshold : float, optional
+        Value between 0 and 1 to set the correlation threshold,
+        by default 0 unless split = "high" or split = "low", in
+        which case the default is 0.3
+
+    target : Optional[pd.Series | str], optional
+        Specify a target for correlation. For example, the label column
+        to generate only the correlations between each feature and the
+        label, by default None
+
+    method : Literal['pearson', 'spearman', 'kendall'], optional
+        Method for correlation calculation:
+        {"pearson", "spearman", "kendall"}, by default "pearson"
+
+        - pearson: measures linear relationships and requires normally
+            distributed and homoscedastic data.
+        - spearman: ranked/ordinal correlation, measures monotonic
+            relationships.
+        - kendall: ranked/ordinal correlation, measures monotonic
+            relationships. Computationally more expensive but more
+            robust in smaller datasets than "spearman".
+
+    cmap : str, optional
+        The mapping from data values to color space, plotly
+        colormap name or object, or list of colors, by default "BrBG"
+
+    figsize : tuple[float, float], optional
+        Use to control the figure size, by default (12, 10)
+
+    annot : bool, optional
+        Use to show or hide annotations, by default True
+
+    **kwargs : optional
+        Additional elements to control the visualization of the plot.
+            These additional arguments will be passed to the `go.Heatmap`
+            function in Plotly.
+
+        Specific kwargs used in this function:
+
+        - colorscale: str or list, optional
+            The colorscale to be used for the heatmap. It controls the
+            mapping of data values to colors in the heatmap.
+
+        - zmax: float, optional
+            The maximum value of the color scale. It limits the upper
+            range of the colorbar displayed on the heatmap.
+
+        - zmin: float, optional
+            The minimum value of the color scale. It limits the lower
+            range of the colorbar displayed on the heatmap.
+
+        - text: pd.DataFrame, optional
+            A DataFrame containing text to display on the heatmap. This
+            text will be shown on the heatmap cells corresponding to the
+            correlation values.
+
+        - texttemplate: str, optional
+            A text template string to format the text display on the
+            heatmap. This allows you to customize how the text appears,
+            including the display of the correlation values.
+
+        - textfont: dict, optional
+            A dictionary specifying the font properties for the text on
+            the heatmap. You can customize the font size, color, family,
+            etc., for the text annotations.
+
+        - x: list, optional
+            The list of column names for the x-axis of the heatmap. It
+            allows you to customize the labels displayed on the x-axis.
+
+        - y: list, optional
+            The list of row names for the y-axis of the heatmap. It
+            allows you to customize the labels displayed on the y-axis.
+
+        - z: pd.DataFrame, optional
+            The 2D array representing the correlation matrix to be
+            visualized. This is the core data for generating the heatmap,
+            containing the correlation values.
+
+        - Many more kwargs are available, e.g., "hovertemplate" to control
+            the legend hover template, or options to adjust the borderwidth
+            and opacity of the heatmap. For a comprehensive list of
+            available kwargs, please refer to the Plotly Heatmap documentation.
+
+        Kwargs can be supplied through a dictionary of key-value pairs
+        (see above) and can be found in Plotly Heatmap documentation.
+
+    Returns
+    -------
+    heatmap : plotly.graph_objs._figure.Figure
+        A Plotly Figure object representing the heatmap visualization of
+        feature correlations.
+    """
+    # Validate Inputs
+    _validate_input_range(threshold, "threshold", -1, 1)
+    _validate_input_bool(annot, "annot")
+
+    data = pd.DataFrame(data).iloc[:, ::-1]
+
+    corr = corr_mat(
+        data,
+        split=split,
+        threshold=threshold,
+        target=target,
+        method=method,
+        colored=False,
+    )
+
+    mask = np.zeros_like(corr, dtype=bool)
+
+    if target is None:
+        mask = np.triu(np.ones_like(corr, dtype=bool))
+        np.fill_diagonal(corr.to_numpy(), np.nan)
+        corr = corr.where(mask == 1)
+    else:
+        corr = corr.iloc[::-1, :]
+
+    vmax = np.round(np.nanmax(corr) - 0.05, 2)
+    vmin = np.round(np.nanmin(corr) + 0.05, 2)
+
+    vmax = -vmin if split == "neg" else vmax
+    vmin = -vmax if split == "pos" else vmin
+
+    vtext = corr.round(2).fillna("") if annot else None
+
+    # Specify kwargs for the heatmap
+    kwargs = {
+        "colorscale": cmap,
+        "zmax": vmax,
+        "zmin": vmin,
+        "text": vtext,
+        "texttemplate": "%{text}",
+        "textfont": {"size": 12},
+        "x": corr.columns,
+        "y": corr.index,
+        "z": corr,
+        **kwargs,
+    }
+
+    # Draw heatmap with masked corr and default settings
+    heatmap = go.Figure(
+        data=go.Heatmap(
+            hoverongaps=False,
+            xgap=1,
+            ygap=1,
+            **kwargs,
+        ),
+    )
+
+    dpi = 96  # more or less arbitrary default value
+    for monitor in get_monitors():
+        if monitor.is_primary:
+            if monitor.width_mm is None or monitor.height_mm is None:
+                continue
+            dpi = monitor.width / (monitor.width_mm / 25.4)
+            break
+
+    if dpi is None:
+        try:
+            monitor = get_monitors()[0]
+            dpi = monitor.width / (monitor.width_mm / 25.4)
+        except ValueError as exc:
+            msg = "Monitor doesn't exist"
+            raise LookupError(msg) from exc
+
+    heatmap.update_layout(
+        title=f"Feature-correlation ({method})",
+        title_font={"size": 24},
+        title_x=0.5,
+        autosize=True,
+        width=figsize[0] * dpi,
+        height=(figsize[1] + 1) * dpi,
+        xaxis={"autorange": "reversed"},
+    )
+
+    return heatmap
+
+
 def dist_plot(
     data: pd.DataFrame,
     mean_color: str = "orange",
     size: int = 3,
     fill_range: tuple = (0.025, 0.975),
     showall: bool = False,
-    kde_kws: Optional[dict[str, Any]] = None,
-    rug_kws: Optional[dict[str, Any]] = None,
-    fill_kws: Optional[dict[str, Any]] = None,
-    font_kws: Optional[dict[str, Any]] = None,
-):
-    """Two-dimensional visualization of the distribution of non binary numerical \
-        features.
+    kde_kws: dict[str, Any] | None = None,
+    rug_kws: dict[str, Any] | None = None,
+    fill_kws: dict[str, Any] | None = None,
+    font_kws: dict[str, Any] | None = None,
+) -> None | Any:  # noqa: ANN401
+    """2D visualization of the distribution of non binary numerical features.
 
     Parameters
     ----------
     data : pd.DataFrame
         2D dataset that can be coerced into Pandas DataFrame. If a Pandas DataFrame \
         is provided, the index/column information is used to label the plots
     mean_color : str, optional
@@ -478,38 +711,37 @@
     font_kws = (
         {"color": "#111111", "weight": "normal", "size": 11}
         if font_kws is None
         else font_kws.copy()
     )
 
     data = pd.DataFrame(data.copy()).dropna(axis=1, how="all")
-    df = data.copy()
-    data = data.loc[:, data.nunique() > 2]
-    if data.shape[0] > 10000:
+    df = data.copy()  # noqa: PD901
+    data = data.loc[:, data.nunique() > 2]  # noqa: PLR2004
+    if data.shape[0] > 10000:  # noqa: PLR2004
         data = data.sample(n=10000, random_state=408)
         print(
             "Large dataset detected, using 10000 random samples for the plots. Summary"
-            " statistics are still based on the entire dataset."
+            " statistics are still based on the entire dataset.",
         )
     cols = list(data.select_dtypes(include=["number"]).columns)
     data = data[cols]
 
     if not cols:
         print("No columns with numeric data were detected.")
         return None
 
-    if len(cols) >= 20 and not showall:
+    if len(cols) >= 20 and not showall:  # noqa: PLR2004
         print(
             "Note: The number of non binary numerical features is very large "
             f"({len(cols)}), please consider splitting the data. Showing plots for "
-            "the first 20 numerical features. Override this by setting showall=True."
+            "the first 20 numerical features. Override this by setting showall=True.",
         )
         cols = cols[:20]
 
-    g = None
     for col in cols:
         col_data = data[col].dropna(axis=0)
         col_df = df[col].dropna(axis=0)
 
         g = sns.displot(
             col_data,
             kind="kde",
@@ -602,18 +834,19 @@
             0.1,
             f"Count: {len(col_df)}",
             fontdict=font_kws,
             transform=g.axes[0, 0].transAxes,
         )
         g.axes[0, 0].legend(loc="upper right")
 
-    return g.axes[0, 0]
+        return g.axes[0, 0]
+    return None
 
 
-def missingval_plot(
+def missingval_plot(  # noqa: PLR0915
     data: pd.DataFrame,
     cmap: str = "PuBuGn",
     figsize: tuple = (20, 20),
     sort: bool = False,
     spine_color: str = "#EEEEEE",
 ) -> GridSpec:
     """Two-dimensional visualization of the missing values in a dataset.
@@ -645,15 +878,15 @@
 
     data = pd.DataFrame(data)
 
     if sort:
         mv_cols_sorted = data.isna().sum(axis=0).sort_values(ascending=False)
         final_cols = (
             mv_cols_sorted.drop(
-                mv_cols_sorted[mv_cols_sorted.values == 0].keys().tolist()
+                mv_cols_sorted[mv_cols_sorted.to_numpy() == 0].keys().tolist(),
             )
             .keys()
             .tolist()
         )
         data = data[final_cols]
         print("Displaying only columns with missing values.")
 
@@ -672,38 +905,38 @@
     ax2 = fig.add_subplot(gs[1:, :5])
     ax3 = fig.add_subplot(gs[:1, 5:])
     ax4 = fig.add_subplot(gs[1:, 5:])
 
     # ax1 - Barplot
     colors = plt.get_cmap(cmap)(mv_cols / np.max(mv_cols))  # color bars by height
     ax1.bar(range(len(mv_cols)), np.round((mv_cols_ratio) * 100, 2), color=colors)
-    ax1.get_xaxis().set_visible(False)
+    ax1.get_xaxis().set_visible(False)  # noqa: FBT003
     ax1.set(frame_on=False, xlim=(-0.5, len(mv_cols) - 0.5))
     ax1.set_ylim(0, np.max(mv_cols_ratio) * 100)
     ax1.grid(linestyle=":", linewidth=1)
     ax1.yaxis.set_major_formatter(ticker.PercentFormatter(decimals=1))
     ax1.tick_params(axis="y", colors="#111111", length=1)
 
     # annotate values on top of the bars
-    for rect, label in zip(ax1.patches, mv_cols):
+    for rect, label in zip(ax1.patches, mv_cols, strict=True):
         height = rect.get_height()
         ax1.text(
             rect.get_x() + rect.get_width() / 2,
             height + max(np.log(1 + height / 6), 0.075),
             label,
             ha="center",
             va="bottom",
             rotation=90,
             alpha=0.5,
             fontsize="11",
         )
 
-    ax1.set_frame_on(True)
+    ax1.set_frame_on(True)  # noqa: FBT003
     for _, spine in ax1.spines.items():
-        spine.set_visible(True)
+        spine.set_visible(True)  # noqa: FBT003
         spine.set_color(spine_color)
     ax1.spines["top"].set_color(None)
 
     # ax2 - Heatmap
     sns.heatmap(data.isna(), cbar=False, cmap="binary", ax=ax2)
     ax2.set_yticks(np.round(ax2.get_yticks()[::5], -1))
     ax2.set_yticklabels(ax2.get_yticks())
@@ -711,21 +944,21 @@
         ax2.get_xticklabels(),
         horizontalalignment="center",
         fontweight="light",
         fontsize="12",
     )
     ax2.tick_params(length=1, colors="#111111")
     for _, spine in ax2.spines.items():
-        spine.set_visible(True)
+        spine.set_visible(True)  # noqa: FBT003
         spine.set_color(spine_color)
 
     # ax3 - Summary
     fontax3 = {"color": "#111111", "weight": "normal", "size": 14}
-    ax3.get_xaxis().set_visible(False)
-    ax3.get_yaxis().set_visible(False)
+    ax3.get_xaxis().set_visible(False)  # noqa: FBT003
+    ax3.get_yaxis().set_visible(False)  # noqa: FBT003
     ax3.set(frame_on=False)
 
     ax3.text(
         0.025,
         0.875,
         f"Total: {np.round(total_datapoints/1000,1)}K",
         transform=ax3.transAxes,
@@ -757,15 +990,15 @@
         0.075,
         f"Max-row: {np.round(mv_rows.max()/data.shape[1]*100)}%",
         transform=ax3.transAxes,
         fontdict=fontax3,
     )
 
     # ax4 - Scatter plot
-    ax4.get_yaxis().set_visible(False)
+    ax4.get_yaxis().set_visible(False)  # noqa: FBT003
     for _, spine in ax4.spines.items():
         spine.set_color(spine_color)
     ax4.tick_params(axis="x", colors="#111111", length=1)
 
     ax4.scatter(
         mv_rows,
         range(len(mv_rows)),
@@ -776,11 +1009,15 @@
         vmin=1,
     )
     ax4.set_ylim((0, len(mv_rows))[::-1])  # limit and invert y-axis
     ax4.set_xlim(0, max(mv_rows) + 0.5)
     ax4.grid(linestyle=":", linewidth=1)
 
     gs.figure.suptitle(
-        "Missing value plot", x=0.45, y=0.94, fontsize=18, color="#111111"
+        "Missing value plot",
+        x=0.45,
+        y=0.94,
+        fontsize=18,
+        color="#111111",
     )
 
     return gs
```

### Comparing `klib-1.0.7/src/klib/scripts/performance.py` & `klib-1.1.0/src/klib/scripts/performance.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-"""
-Measuring the performance of key functionality.
+"""Measuring the performance of key functionality.
 
 :author: Andreas Kanz
 """
 import functools
 from pathlib import Path
 from time import perf_counter
 
-import klib
 import matplotlib.pyplot as plt
 import pandas as pd
 
+import klib
+
 # Paths
 base_path = Path(__file__).resolve().parents[3]
 print(base_path)
 data_path = base_path / "examples"
 
 # Data Import
 filepath = data_path / "NFL_DATASET.csv"
@@ -57,16 +57,18 @@
     df_times["missingval_plot"] = pd.Series([time_missingval_plot() for _ in range(7)])
     df_times["dist_plot"] = pd.Series([time_dist_plot() for _ in range(7)])
     df_times["cat_plot"] = pd.Series([time_cat_plot() for _ in range(7)])
     df_times = df_times.fillna(df_times.mean())
     fig, ax = plt.subplots(nrows=1, ncols=4, figsize=(14, 7))
     reference_values = [5, 10, 10, 10]
 
-    for i, (col, ref) in enumerate(zip(df_times.columns, reference_values)):
-        ax[i].boxplot(df_times[col])  # pylint: disable=unsubscriptable-object
+    for i, (col, ref) in enumerate(
+        zip(df_times.columns, reference_values, strict=True),
+    ):
+        ax[i].boxplot(df_times[col])
         ax[i].set_title(" ".join(col.split("_")).title())
         ax[i].axhline(ref)
     fig.suptitle("Performance", fontsize=16)
     fig.savefig("boxplots.png")
 
 
 if __name__ == "__main__":
```

### Comparing `klib-1.0.7/src/klib/utils.py` & `klib-1.1.0/src/klib/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-"""
-Utilities and auxiliary functions.
+"""Utilities and auxiliary functions.
 
 :author: Andreas Kanz
 
 """
 from __future__ import annotations
 
 from typing import Literal
-from typing import Optional
 from typing import TypedDict
 
 import numpy as np
 import pandas as pd
 
 
 def _corr_selector(
     corr: pd.Series | pd.DataFrame,
-    split: Optional[Literal["pos", "neg", "high", "low"]] = None,
+    split: Literal["pos", "neg", "high", "low"] | None = None,
     threshold: float = 0,
 ) -> pd.Series | pd.DataFrame:
     """Select the desired correlations using this utility function.
 
     Parameters
     ----------
     corr : pd.Series | pd.DataFrame
@@ -37,49 +35,50 @@
     pd.DataFrame
         List or matrix of (filtered) correlations
     """
     if split == "pos":
         corr = corr.where((corr >= threshold) & (corr > 0))
         print(
             'Displaying positive correlations. Specify a positive "threshold" to '
-            "limit the results further."
+            "limit the results further.",
         )
     elif split == "neg":
         corr = corr.where((corr <= threshold) & (corr < 0))
         print(
             'Displaying negative correlations. Specify a negative "threshold" to '
-            "limit the results further."
+            "limit the results further.",
         )
     elif split == "high":
         threshold = 0.3 if threshold <= 0 else threshold
         corr = corr.where(np.abs(corr) >= threshold)
         print(
             f"Displaying absolute correlations above the threshold ({threshold}). "
-            'Specify a positive "threshold" to limit the results further.'
+            'Specify a positive "threshold" to limit the results further.',
         )
     elif split == "low":
         threshold = 0.3 if threshold <= 0 else threshold
         corr = corr.where(np.abs(corr) <= threshold)
         print(
             f"Displaying absolute correlations below the threshold ({threshold}). "
-            'Specify a positive "threshold" to limit the results further.'
+            'Specify a positive "threshold" to limit the results further.',
         )
 
     return corr
 
 
 def _diff_report(
     data: pd.DataFrame,
     data_cleaned: pd.DataFrame,
-    dupl_rows: Optional[list[str | int]] = None,
-    single_val_cols: Optional[list[str]] = None,
-    show: Optional[Literal["all", "changes"]] = "changes",
+    dupl_rows: list[str | int] | None = None,
+    single_val_cols: list[str] | None = None,
+    show: Literal["all", "changes"] | None = "changes",
 ) -> None:
-    """Provide information about changes between two datasets, such as dropped rows \
-        and columns, memory usage and missing values.
+    """Provide information about changes between two datasets.
+
+    This includes dropped rows and columns, memory usage and missing values.
 
     Parameters
     ----------
     data : pd.DataFrame
         2D dataset that can be coerced into Pandas DataFrame. Input the initial \
         dataset here
     data_cleaned : pd.DataFrame
@@ -115,43 +114,51 @@
     data_cl_mv_tot = _missing_vals(data_cleaned)["mv_total"]
 
     if show == "all":
         data_mem = _memory_usage(data, deep=True)
         data_cl_mem = _memory_usage(data_cleaned, deep=True)
         _print_cleaning_details("Before data cleaning:\n", data, data_mv_tot, data_mem)
         _print_cleaning_details(
-            "After data cleaning:\n", data_cleaned, data_cl_mv_tot, data_cl_mem
+            "After data cleaning:\n",
+            data_cleaned,
+            data_cl_mv_tot,
+            data_cl_mem,
         )
 
     print(
         f"Shape of cleaned data: {data_cleaned.shape} - "
-        f"Remaining NAs: {data_cl_mv_tot}\n\n"
+        f"Remaining NAs: {data_cl_mv_tot}\n\n",
     )
     print(f"Dropped rows: {data.shape[0]-data_cleaned.shape[0]}")
     print(
-        f"     of which {len(dupl_rows)} duplicates. (Rows (first 150 shown): {dupl_rows[:150]})\n"  # noqa
+        f"     of which {len(dupl_rows)} duplicates. (Rows (first 150 shown): {dupl_rows[:150]})\n",  # noqa: E501
     )
     print(f"Dropped columns: {data.shape[1]-data_cleaned.shape[1]}")
     print(
         f"     of which {len(single_val_cols)} single valued."
-        f"     Columns: {single_val_cols}"
+        f"     Columns: {single_val_cols}",
     )
     print(f"Dropped missing values: {data_mv_tot-data_cl_mv_tot}")
     mem_change = data_mem - data_cl_mem
     mem_perc = round(100 * mem_change / data_mem, 2)
     print(f"Reduced memory by at least: {round(mem_change,3)} MB (-{mem_perc}%)\n")
 
 
-def _print_cleaning_details(arg0, arg1, arg2, arg3) -> None:
-    print(arg0)
-    print(f"dtypes:\n{arg1.dtypes.value_counts()}")
-    print(f"\nNumber of rows: {str(arg1.shape[0]).rjust(8)}")
-    print(f"Number of cols: {str(arg1.shape[1]).rjust(8)}")
-    print(f"Missing values: {str(arg2).rjust(8)}")
-    print(f"Memory usage: {str(arg3).rjust(7)} MB")
+def _print_cleaning_details(
+    header: str,
+    data: pd.DataFrame | pd.Series,
+    missing_vals: int,
+    mem_usage: float,
+) -> None:
+    print(header)
+    print(f"dtypes:\n{data.dtypes.value_counts()}")
+    print(f"\nNumber of rows: {str(data.shape[0]).rjust(8)}")
+    print(f"Number of cols: {str(data.shape[1]).rjust(8)}")
+    print(f"Missing values: {str(missing_vals).rjust(8)}")
+    print(f"Memory usage: {str(mem_usage).rjust(7)} MB")
     print("_______________________________________________________\n")
 
 
 def _drop_duplicates(data: pd.DataFrame) -> tuple[pd.DataFrame, list[str | int]]:
     """Provide information on and drops duplicate rows.
 
     Parameters
@@ -228,54 +235,49 @@
         "mv_rows": mv_rows,
         "mv_cols": mv_cols,
         "mv_rows_ratio": mv_rows_ratio,
         "mv_cols_ratio": mv_cols_ratio,
     }
 
 
-def _validate_input_bool(value: bool, desc) -> None:
+def _validate_input_bool(value: bool, desc: str) -> None:
     if not isinstance(value, bool):
-        raise TypeError(
-            f"Input value for '{desc}' is {type(value)} but should be a boolean."
-        )
+        msg = f"Input value for '{desc}' is {type(value)} but should be a boolean."
+        raise TypeError(msg)
 
 
-def _validate_input_int(value: int, desc) -> None:
+def _validate_input_int(value: int, desc: str) -> None:
     if not isinstance(value, int):
-        raise TypeError(
-            f"Input value for '{desc}' is {type(value)} but should be an integer."
-        )
+        msg = f"Input value for '{desc}' is {type(value)} but should be an integer."
+        raise TypeError(msg)
 
 
-def _validate_input_range(value, desc, lower, upper) -> None:
+def _validate_input_range(value: float, desc: str, lower: float, upper: float) -> None:
     if value < lower or value > upper:
-        raise ValueError(
-            f"'{desc}' = {value} but should be {lower} <= '{desc}' <= {upper}."
-        )
+        msg = f"'{desc}' = {value} but should be {lower} <= '{desc}' <= {upper}."
+        raise ValueError(msg)
 
 
-def _validate_input_smaller(value1, value2, desc) -> None:
+def _validate_input_smaller(value1: int, value2: int, desc: str) -> None:
     if value1 > value2:
-        raise ValueError(
-            f"The first input for '{desc}' should be smaller or equal to the second."
-        )
+        msg = f"The first input for '{desc}' should be smaller or equal to the second."
+        raise ValueError(msg)
 
 
-def _validate_input_sum_smaller(limit, desc, *args) -> None:
+def _validate_input_sum_smaller(limit: float, desc: str, *args) -> None:  # noqa: ANN002
     if sum(args) > limit:
-        raise ValueError(
+        msg = (
             f"The sum of input values for '{desc}' should be less or equal to {limit}."
         )
+        raise ValueError(msg)
 
 
-def _validate_input_sum_larger(limit, desc, *args) -> None:
+def _validate_input_sum_larger(limit: float, desc: str, *args) -> None:  # noqa: ANN002
     if sum(args) < limit:
-        raise ValueError(
-            f"The sum of input values for '{desc}' should be larger/equal to {limit}."
-        )
+        msg = f"The sum of input values for '{desc}' should be larger/equal to {limit}."
+        raise ValueError(msg)
 
 
-def _validate_input_num_data(value: pd.DataFrame, desc) -> None:
+def _validate_input_num_data(value: pd.DataFrame, desc: str) -> None:
     if value.select_dtypes(include=["number"]).empty:
-        raise TypeError(
-            f"Input value for '{desc}' should contain at least one numerical column."
-        )
+        msg = f"Input value for '{desc}' should contain at least one numerical column."
+        raise TypeError(msg)
```

### Comparing `klib-1.0.7/tests/test_clean.py` & `klib-1.1.0/tests/test_clean.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from __future__ import annotations
+
 import io
 import sys
 import unittest
 
 import numpy as np
 import pandas as pd
-
 from klib.clean import clean_column_names
 from klib.clean import convert_datatypes
 from klib.clean import data_cleaning
 from klib.clean import drop_missing
 from klib.clean import pool_duplicate_subsets
 
 
@@ -19,25 +20,25 @@
             {
                 "Asd 5$ & (3€)": [1, 2, 3],
                 "3+3": [2, 3, 4],
                 "AsdFer #9": [3, 4, 5],
                 '"asdäöüß"': [5, 6, 7],
                 "dupli": [5, 6, 8],
                 "also": [9, 2, 7],
-                "-Ä-__________!?:;some/(... \n ..))(++$%/name/    -.....": [2, 3, 7],
-            }
+                "-ä-__________!?:;some/(... \n ..))(++$%/name/    -.....": [2, 3, 7],
+            },
         )
         cls.df2 = pd.DataFrame(
             {
                 "dupli": [3, 2, 1],
                 "also": [4, 5, 7],
                 "verylongColumnNamesareHardtoRead": [9, 2, 7],
                 "< #total@": [2, 6, 4],
                 "count >= 10": [6, 3, 2],
-            }
+            },
         )
         cls.df_clean_column_names = pd.concat([cls.df1, cls.df2], axis=1)
 
     def test_clean_column_names(self):
         expected_results = [
             "asd_5_dollar_and_3_euro",
             "3_plus_3",
@@ -49,32 +50,31 @@
             "dupli_7",
             "also_8",
             "verylong_column_namesare_hardto_read",
             "smaller_hash_total_at",
             "count_larger_equal_10",
         ]
         for i, _ in enumerate(expected_results):
-            self.assertEqual(
-                clean_column_names(self.df_clean_column_names).columns[i],
-                expected_results[i],
+            assert (
+                clean_column_names(self.df_clean_column_names).columns[i]
+                == expected_results[i]
             )
         for i, _ in enumerate(expected_results):
-            self.assertEqual(
-                clean_column_names(self.df_clean_column_names, hints=False).columns[i],
-                expected_results[i],
+            assert (
+                clean_column_names(self.df_clean_column_names, hints=False).columns[i]
+                == expected_results[i]
             )
 
+    def test_clean_column_names_prints(self):
         captured_output = io.StringIO()
         sys.stdout = captured_output
         clean_column_names(self.df_clean_column_names, hints=True)
         sys.stdout = sys.__stdout__
-        self.assertEqual(
-            captured_output.getvalue(),
-            "Long column names detected (>25 characters). Consider renaming the "
-            "following columns ['ae_some_plus_plus_dollar_percent_name', 'verylong_column_namesare_hardto_read'].\n",
+        assert captured_output.getvalue() == (
+            "(\"Duplicate column names detected! Columns with index [7, 8] and names ['dupli', 'also'] have been renamed to ['dupli_7', 'also_8'].\", \"Long column names detected (>25 characters). Consider renaming the following columns ['ae_some_plus_plus_dollar_percent_name', 'verylong_column_namesare_hardto_read'].\")\n"
         )
 
 
 class Test_drop_missing(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.df_data_drop = pd.DataFrame(
@@ -86,67 +86,47 @@
                 [pd.NA, 2, 3, 4, pd.NA],
                 [pd.NA, 6, 7, pd.NA, pd.NA],
             ],
             columns=["c1", "c2", "c3", "c4", "c5"],
         )
 
     def test_drop_missing(self):
-        self.assertEqual(drop_missing(self.df_data_drop).shape, (4, 4))
+        assert drop_missing(self.df_data_drop).shape == (4, 4)
 
         # Drop further columns based on threshold
-        self.assertEqual(
-            drop_missing(self.df_data_drop, drop_threshold_cols=0.5).shape, (4, 3)
-        )
-        self.assertEqual(
-            drop_missing(
-                self.df_data_drop, drop_threshold_cols=0.5, col_exclude=["c1"]
-            ).shape,
-            (4, 4),
-        )
-        self.assertEqual(
-            drop_missing(self.df_data_drop, drop_threshold_cols=0.49).shape, (4, 2)
-        )
-        self.assertEqual(
-            drop_missing(self.df_data_drop, drop_threshold_cols=0).shape, (0, 0)
-        )
+        assert drop_missing(self.df_data_drop, drop_threshold_cols=0.5).shape == (4, 3)
+        assert drop_missing(
+            self.df_data_drop,
+            drop_threshold_cols=0.5,
+            col_exclude=["c1"],
+        ).shape == (4, 4)
+        assert drop_missing(self.df_data_drop, drop_threshold_cols=0.49).shape == (4, 2)
+        assert drop_missing(self.df_data_drop, drop_threshold_cols=0).shape == (0, 0)
 
         # Drop further rows based on threshold
-        self.assertEqual(
-            drop_missing(self.df_data_drop, drop_threshold_rows=0.67).shape, (4, 4)
-        )
-        self.assertEqual(
-            drop_missing(self.df_data_drop, drop_threshold_rows=0.5).shape, (4, 4)
-        )
-        self.assertEqual(
-            drop_missing(self.df_data_drop, drop_threshold_rows=0.49).shape, (3, 4)
-        )
-        self.assertEqual(
-            drop_missing(self.df_data_drop, drop_threshold_rows=0.25).shape, (3, 4)
-        )
-        self.assertEqual(
-            drop_missing(self.df_data_drop, drop_threshold_rows=0.24).shape, (2, 4)
-        )
-        self.assertEqual(
-            drop_missing(
-                self.df_data_drop, drop_threshold_rows=0.24, col_exclude=["c1"]
-            ).shape,
-            (2, 5),
-        )
-        self.assertEqual(
-            drop_missing(
-                self.df_data_drop, drop_threshold_rows=0.24, col_exclude=["c2"]
-            ).shape,
-            (2, 4),
-        )
-        self.assertEqual(
-            drop_missing(
-                self.df_data_drop, drop_threshold_rows=0.51, col_exclude=["c1"]
-            ).shape,
-            (3, 5),
-        )
+        assert drop_missing(self.df_data_drop, drop_threshold_rows=0.67).shape == (4, 4)
+        assert drop_missing(self.df_data_drop, drop_threshold_rows=0.5).shape == (4, 4)
+        assert drop_missing(self.df_data_drop, drop_threshold_rows=0.49).shape == (3, 4)
+        assert drop_missing(self.df_data_drop, drop_threshold_rows=0.25).shape == (3, 4)
+        assert drop_missing(self.df_data_drop, drop_threshold_rows=0.24).shape == (2, 4)
+        assert drop_missing(
+            self.df_data_drop,
+            drop_threshold_rows=0.24,
+            col_exclude=["c1"],
+        ).shape == (2, 5)
+        assert drop_missing(
+            self.df_data_drop,
+            drop_threshold_rows=0.24,
+            col_exclude=["c2"],
+        ).shape == (2, 4)
+        assert drop_missing(
+            self.df_data_drop,
+            drop_threshold_rows=0.51,
+            col_exclude=["c1"],
+        ).shape == (3, 5)
 
 
 class Test_data_cleaning(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.df_data_cleaning = pd.DataFrame(
             [
@@ -157,147 +137,143 @@
                 [pd.NA, "c", 3, 4, pd.NA, 1],
                 [pd.NA, "d", 7, pd.NA, pd.NA, 1],
             ],
             columns=["c1", "c2", "c3", "c 4", "c5", "c6"],
         )
 
     def test_data_cleaning(self):
-        self.assertEqual(data_cleaning(self.df_data_cleaning, show="all").shape, (5, 4))
-        self.assertEqual(data_cleaning(self.df_data_cleaning, show=None).shape, (5, 4))
+        assert data_cleaning(self.df_data_cleaning, show="all").shape == (5, 4)
+        assert data_cleaning(self.df_data_cleaning, show=None).shape == (5, 4)
 
-        self.assertEqual(
-            data_cleaning(self.df_data_cleaning, col_exclude=["c6"]).shape, (5, 5)
-        )
+        assert data_cleaning(self.df_data_cleaning, col_exclude=["c6"]).shape == (5, 5)
 
-        self.assertEqual(
-            data_cleaning(
-                self.df_data_cleaning,
-                show="changes",
-                clean_col_names=False,
-                drop_duplicates=False,
-            ).columns.tolist(),
-            ["c2", "c3", "c 4", "c5"],
-        )
-
-        self.assertEqual(
-            data_cleaning(
-                self.df_data_cleaning,
-                show="changes",
-                clean_col_names=False,
-                drop_duplicates=False,
-            ).columns.tolist(),
-            ["c2", "c3", "c 4", "c5"],
-        )
+        assert data_cleaning(
+            self.df_data_cleaning,
+            show="changes",
+            clean_col_names=False,
+            drop_duplicates=False,
+        ).columns.tolist() == ["c2", "c3", "c 4", "c5"]
+
+        assert data_cleaning(
+            self.df_data_cleaning,
+            show="changes",
+            clean_col_names=False,
+            drop_duplicates=False,
+        ).columns.tolist() == ["c2", "c3", "c 4", "c5"]
 
         expected_results = ["string", "float32", "O", "O"]
         for i, _ in enumerate(expected_results):
-            self.assertEqual(
-                data_cleaning(self.df_data_cleaning, convert_dtypes=True).dtypes[i],
-                expected_results[i],
+            assert (
+                data_cleaning(self.df_data_cleaning, convert_dtypes=True).dtypes[i]
+                == expected_results[i]
             )
 
         expected_results = ["O", "O", "O", "O"]
         for i, _ in enumerate(expected_results):
-            self.assertEqual(
-                data_cleaning(self.df_data_cleaning, convert_dtypes=False).dtypes[i],
-                expected_results[i],
+            assert (
+                data_cleaning(self.df_data_cleaning, convert_dtypes=False).dtypes[i]
+                == expected_results[i]
             )
 
         expected_results = ["O", "O", "O", "O"]
         for i, _ in enumerate(expected_results):
-            self.assertEqual(
-                data_cleaning(self.df_data_cleaning, convert_dtypes=False).dtypes[i],
-                expected_results[i],
+            assert (
+                data_cleaning(self.df_data_cleaning, convert_dtypes=False).dtypes[i]
+                == expected_results[i]
             )
 
 
 class Test_convert_dtypes(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.df_data_convert = pd.DataFrame(
             [
                 [1, 7.0, "y", "x", pd.NA, "v"],
                 [3, 8.0, "d", "e", pd.NA, "v"],
                 [5, 7.0, "o", "z", pd.NA, "v"],
                 [1, 7.0, "u", "f", pd.NA, "p"],
                 [1, 7.0, "u", "f", pd.NA, "p"],
                 [2, 7.0, "g", "a", pd.NA, "p"],
-            ]
+            ],
         )
 
     def test_convert_dtypes(self):
         expected_results = [
             "int8",
             "float32",
             "string",
             "string",
             "category",
             "category",
         ]
         for i, _ in enumerate(expected_results):
-            self.assertEqual(
-                convert_datatypes(self.df_data_convert, cat_threshold=0.4).dtypes[i],
-                expected_results[i],
+            assert (
+                convert_datatypes(self.df_data_convert, cat_threshold=0.4).dtypes[i]
+                == expected_results[i]
             )
 
         expected_results = [
             "int8",
             "float32",
             "string",
             "string",
             "object",
             "string",
         ]
         for i, _ in enumerate(expected_results):
-            self.assertEqual(
-                convert_datatypes(self.df_data_convert).dtypes[i], expected_results[i]
+            assert (
+                convert_datatypes(self.df_data_convert).dtypes[i] == expected_results[i]
             )
 
         expected_results = [
             "int8",
             "float32",
             "string",
             "string",
             "object",
             "category",
         ]
         for i, _ in enumerate(expected_results):
-            self.assertEqual(
+            assert (
                 convert_datatypes(
-                    self.df_data_convert, cat_threshold=0.5, cat_exclude=[4]
-                ).dtypes[i],
-                expected_results[i],
+                    self.df_data_convert,
+                    cat_threshold=0.5,
+                    cat_exclude=[4],
+                ).dtypes[i]
+                == expected_results[i]
             )
 
         expected_results = [
             "int8",
             "float32",
             "string",
             "category",
             "object",
             "category",
         ]
         for i, _ in enumerate(expected_results):
-            self.assertEqual(
+            assert (
                 convert_datatypes(
-                    self.df_data_convert, cat_threshold=0.95, cat_exclude=[2, 4]
-                ).dtypes[i],
-                expected_results[i],
+                    self.df_data_convert,
+                    cat_threshold=0.95,
+                    cat_exclude=[2, 4],
+                ).dtypes[i]
+                == expected_results[i]
             )
 
         expected_results = ["int8", "float32", "string", "string", "object", "string"]
         for i, _ in enumerate(expected_results):
-            self.assertEqual(
+            assert (
                 convert_datatypes(
                     self.df_data_convert,
                     category=False,
                     cat_threshold=0.95,
                     cat_exclude=[2, 4],
-                ).dtypes[i],
-                expected_results[i],
+                ).dtypes[i]
+                == expected_results[i]
             )
 
 
 class Test_pool_duplicate_subsets(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.df_data_subsets = pd.DataFrame(
@@ -309,37 +285,38 @@
                 [1, 7, "u", "z", pd.NA, "p"],
                 [2, 7, "g", "z", pd.NA, "p"],
             ],
             columns=["c1", "c2", "c3", "c4", "c5", "c6"],
         )
 
     def test_pool_duplicate_subsets(self):
-        self.assertEqual(pool_duplicate_subsets(self.df_data_subsets).shape, (6, 3))
-        self.assertEqual(
-            pool_duplicate_subsets(self.df_data_subsets, col_dupl_thresh=1).shape,
-            (6, 6),
-        )
-
-        self.assertEqual(
-            pool_duplicate_subsets(self.df_data_subsets, subset_thresh=0).shape, (6, 2)
-        )
-
-        self.assertEqual(
-            pool_duplicate_subsets(self.df_data_subsets, return_details=True)[0].shape,
-            (6, 3),
-        )
-        self.assertEqual(
-            pool_duplicate_subsets(self.df_data_subsets, return_details=True)[1],
-            ["c1", "c2", "c3", "c5"],
-        )
+        assert pool_duplicate_subsets(self.df_data_subsets).shape == (6, 3)
+        assert pool_duplicate_subsets(
+            self.df_data_subsets,
+            col_dupl_thresh=1,
+        ).shape == (6, 6)
+
+        assert pool_duplicate_subsets(self.df_data_subsets, subset_thresh=0).shape == (
+            6,
+            2,
+        )
+
+        assert pool_duplicate_subsets(self.df_data_subsets, return_details=True)[
+            0
+        ].shape == (6, 3)
+        assert pool_duplicate_subsets(self.df_data_subsets, return_details=True)[1] == [
+            "c1",
+            "c2",
+            "c3",
+            "c5",
+        ]
 
-        self.assertEqual(
-            pool_duplicate_subsets(self.df_data_subsets, exclude=["c1"]).shape,
-            (6, 4),
+        assert pool_duplicate_subsets(self.df_data_subsets, exclude=["c1"]).shape == (
+            6,
+            4,
         )
 
-        self.assertEqual(
-            pool_duplicate_subsets(
-                self.df_data_subsets, exclude=["c1"], return_details=True
-            )[1],
-            ["c2", "c5", "c6"],
-        )
+        assert pool_duplicate_subsets(
+            self.df_data_subsets,
+            exclude=["c1"],
+            return_details=True,
+        )[1] == ["c2", "c5", "c6"]
```

### Comparing `klib-1.0.7/tests/test_describe.py` & `klib-1.1.0/tests/test_describe.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from __future__ import annotations
+
 import unittest
 
 import numpy as np
 import pandas as pd
-
 from klib.describe import corr_mat
 
 
 class Test_corr_mat(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.data_corr_df = pd.DataFrame(
@@ -17,98 +18,101 @@
         cls.data_corr_list = [1, 2, -3]
         cls.data_corr_target_series = pd.Series([1, 2, -3], name="Target Series")
         cls.data_corr_target_array = np.array([1, 2, -3])
         cls.data_corr_target_list = [1, 2, -3]
 
     def test_output_type(self):
         # Test conversion from pd.io.formats.style.Styler to pd.core.frame.DataFrame
-        self.assertIsInstance(
-            type(corr_mat(self.data_corr_df)), type(pd.io.formats.style.Styler)
+        assert isinstance(
+            type(corr_mat(self.data_corr_df)),
+            type(pd.io.formats.style.Styler),
         )
-        self.assertIsInstance(
-            type(corr_mat(self.data_corr_list)), type(pd.io.formats.style.Styler)
+        assert isinstance(
+            type(corr_mat(self.data_corr_list)),
+            type(pd.io.formats.style.Styler),
         )
-        self.assertIsInstance(
+        assert isinstance(
             type(corr_mat(self.data_corr_df, target="Col1")),
             type(pd.io.formats.style.Styler),
         )
-        self.assertIsInstance(
+        assert isinstance(
             type(corr_mat(self.data_corr_df, target=self.data_corr_target_series)),
             type(pd.io.formats.style.Styler),
         )
-        self.assertIsInstance(
+        assert isinstance(
             type(corr_mat(self.data_corr_df, target=self.data_corr_target_array)),
             type(pd.io.formats.style.Styler),
         )
-        self.assertIsInstance(
+        assert isinstance(
             type(corr_mat(self.data_corr_df, target=self.data_corr_target_list)),
             type(pd.io.formats.style.Styler),
         )
 
-        self.assertIsInstance(
-            type(corr_mat(self.data_corr_df, colored=False)), type(pd.DataFrame)
+        assert isinstance(
+            type(corr_mat(self.data_corr_df, colored=False)),
+            type(pd.DataFrame),
         )
-        self.assertIsInstance(
-            type(corr_mat(self.data_corr_list, colored=False)), type(pd.DataFrame)
+        assert isinstance(
+            type(corr_mat(self.data_corr_list, colored=False)),
+            type(pd.DataFrame),
         )
-        self.assertIsInstance(
+        assert isinstance(
             type(corr_mat(self.data_corr_df, target="Col1", colored=False)),
             type(pd.DataFrame),
         )
-        self.assertIsInstance(
+        assert isinstance(
             type(
                 corr_mat(
                     self.data_corr_df,
                     target=self.data_corr_target_series,
                     colored=False,
-                )
+                ),
             ),
             type(pd.DataFrame),
         )
-        self.assertIsInstance(
+        assert isinstance(
             type(
                 corr_mat(
-                    self.data_corr_df, target=self.data_corr_target_array, colored=False
-                )
+                    self.data_corr_df,
+                    target=self.data_corr_target_array,
+                    colored=False,
+                ),
             ),
             type(pd.DataFrame),
         )
-        self.assertIsInstance(
+        assert isinstance(
             type(
                 corr_mat(
-                    self.data_corr_df, target=self.data_corr_target_list, colored=False
-                )
+                    self.data_corr_df,
+                    target=self.data_corr_target_list,
+                    colored=False,
+                ),
             ),
             type(pd.DataFrame),
         )
 
     def test_output_shape(self):
         # Test for output dimensions
-        self.assertEqual(
-            corr_mat(self.data_corr_df).data.shape[0],
-            corr_mat(self.data_corr_df).data.shape[1],
-        )
-        self.assertEqual(
-            corr_mat(self.data_corr_list).data.shape[0],
-            corr_mat(self.data_corr_list).data.shape[1],
-        )
-        self.assertEqual(
-            corr_mat(self.data_corr_df, target="Col1", colored=False).shape, (3, 1)
-        )
-        self.assertEqual(
-            corr_mat(
-                self.data_corr_df, target=self.data_corr_target_series, colored=False
-            ).shape,
-            (4, 1),
-        )
-        self.assertEqual(
-            corr_mat(
-                self.data_corr_df, target=self.data_corr_target_array, colored=False
-            ).shape,
-            (4, 1),
-        )
-        self.assertEqual(
-            corr_mat(
-                self.data_corr_df, target=self.data_corr_target_list, colored=False
-            ).shape,
-            (4, 1),
-        )
+        assert (
+            corr_mat(self.data_corr_df).data.shape[0]
+            == corr_mat(self.data_corr_df).data.shape[1]
+        )
+        assert (
+            corr_mat(self.data_corr_list).data.shape[0]
+            == corr_mat(self.data_corr_list).data.shape[1]
+        )
+        assert corr_mat(self.data_corr_df, target="Col1", colored=False).shape == (3, 1)
+        assert corr_mat(
+            self.data_corr_df,
+            target=self.data_corr_target_series,
+            colored=False,
+        ).shape == (4, 1)
+        assert corr_mat(
+            self.data_corr_df,
+            target=self.data_corr_target_array,
+            colored=False,
+        ).shape == (4, 1)
+        assert corr_mat(
+            self.data_corr_df,
+            target=self.data_corr_target_list,
+            colored=False,
+        ).shape == (4, 1)
```

### Comparing `klib-1.0.7/tests/test_util.py` & `klib-1.1.0/tests/test_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import unittest
 
 import numpy as np
 import pandas as pd
-
 from klib.utils import _corr_selector
 from klib.utils import _drop_duplicates
 from klib.utils import _missing_vals
 from klib.utils import _validate_input_bool
 from klib.utils import _validate_input_int
 from klib.utils import _validate_input_num_data
 from klib.utils import _validate_input_range
@@ -22,94 +21,101 @@
             [
                 [1, 7, 2, 2, 4, 7],
                 [3, 8, 3, 3, 7, 1],
                 [5, 7, 9, 5, 1, 4],
                 [1, 7, 8, 6, 1, 8],
                 [1, 7, 5, 6, 2, 6],
                 [2, 7, 3, 3, 5, 3],
-            ]
+            ],
         )
 
         cls.target = pd.Series([1, 2, 4, 7, 4, 2])
 
     def test__corr_selector_matrix(self):
-        self.assertEqual(_corr_selector(self.df_data_corr.corr()).shape, (6, 6))
-        self.assertEqual(
-            _corr_selector(self.df_data_corr.corr(), split="pos").isna().sum().sum(), 18
+        assert _corr_selector(self.df_data_corr.corr()).shape == (6, 6)
+        assert (
+            _corr_selector(self.df_data_corr.corr(), split="pos").isna().sum().sum()
+            == 18
         )
-        self.assertEqual(
+        assert (
             _corr_selector(self.df_data_corr.corr(), split="pos", threshold=0.5)
             .isna()
             .sum()
-            .sum(),
-            26,
+            .sum()
+            == 26
         )
-        self.assertEqual(
+        assert (
             _corr_selector(self.df_data_corr.corr(), split="neg", threshold=-0.75)
             .isna()
             .sum()
-            .sum(),
-            32,
+            .sum()
+            == 32
         )
-        self.assertEqual(
+        assert (
             _corr_selector(self.df_data_corr.corr(), split="high", threshold=0.15)
             .isna()
             .sum()
-            .sum(),
-            4,
+            .sum()
+            == 4
         )
-        self.assertEqual(
+        assert (
             _corr_selector(self.df_data_corr.corr(), split="low", threshold=0.85)
             .isna()
             .sum()
-            .sum(),
-            6,
+            .sum()
+            == 6
         )
 
     def test__corr_selector_label(self):
-        self.assertEqual(
-            _corr_selector(self.df_data_corr.corrwith(self.target)).shape, (6,)
-        )
-        self.assertEqual(
+        assert _corr_selector(self.df_data_corr.corrwith(self.target)).shape == (6,)
+        assert (
             _corr_selector(self.df_data_corr.corrwith(self.target), split="pos")
             .isna()
-            .sum(),
-            3,
+            .sum()
+            == 3
         )
-        self.assertEqual(
+        assert (
             _corr_selector(
-                self.df_data_corr.corrwith(self.target), split="pos", threshold=0.8
+                self.df_data_corr.corrwith(self.target),
+                split="pos",
+                threshold=0.8,
             )
             .isna()
-            .sum(),
-            4,
+            .sum()
+            == 4
         )
-        self.assertEqual(
+        assert (
             _corr_selector(
-                self.df_data_corr.corrwith(self.target), split="neg", threshold=-0.7
+                self.df_data_corr.corrwith(self.target),
+                split="neg",
+                threshold=-0.7,
             )
             .isna()
-            .sum(),
-            5,
+            .sum()
+            == 5
         )
-        self.assertEqual(
+        assert (
             _corr_selector(
-                self.df_data_corr.corrwith(self.target), split="high", threshold=0.2
+                self.df_data_corr.corrwith(self.target),
+                split="high",
+                threshold=0.2,
             )
             .isna()
-            .sum(),
-            1,
+            .sum()
+            == 1
         )
-        self.assertEqual(
+        assert (
             _corr_selector(
-                self.df_data_corr.corrwith(self.target), split="low", threshold=0.8
+                self.df_data_corr.corrwith(self.target),
+                split="low",
+                threshold=0.8,
             )
             .isna()
-            .sum(),
-            2,
+            .sum()
+            == 2
         )
 
 
 class Test__drop_duplicates(unittest.TestCase):
     @classmethod
     def setUpClass(cls: pd.DataFrame) -> pd.DataFrame:
         cls.data_dupl_df = pd.DataFrame(
@@ -117,28 +123,26 @@
                 [pd.NA, pd.NA, pd.NA, pd.NA],
                 [1, 2, 3, 4],
                 [1, 2, 3, 4],
                 [1, 2, 3, 4],
                 [2, 3, 4, 5],
                 [1, 2, 3, pd.NA],
                 [pd.NA, pd.NA, pd.NA, pd.NA],
-            ]
+            ],
         )
 
     def test__drop_dupl(self):
         # Test dropping of duplicate rows
         self.assertAlmostEqual(_drop_duplicates(self.data_dupl_df)[0].shape, (4, 4))
         # Test if the resulting DataFrame is equal to using the pandas method
-        self.assertTrue(
-            _drop_duplicates(self.data_dupl_df)[0].equals(
-                self.data_dupl_df.drop_duplicates().reset_index(drop=True)
-            )
+        assert _drop_duplicates(self.data_dupl_df)[0].equals(
+            self.data_dupl_df.drop_duplicates().reset_index(drop=True),
         )
         # Test number of duplicates
-        self.assertEqual(len(_drop_duplicates(self.data_dupl_df)[1]), 3)
+        assert len(_drop_duplicates(self.data_dupl_df)[1]) == 3
 
 
 class Test__missing_vals(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.data_mv_list = [
             [1, np.nan, 3, 4],
@@ -170,36 +174,34 @@
             self.assertAlmostEqual(_missing_vals(self.data_mv_df)["mv_cols"][i], result)
 
     def test_mv_rows_ratio(self):
         # Test missing values ratio for each row
         expected_results = [0.25, 0.5, 0.25, 0.25]
         for i, result in enumerate(expected_results):
             self.assertAlmostEqual(
-                _missing_vals(self.data_mv_df)["mv_rows_ratio"][i], result
+                _missing_vals(self.data_mv_df)["mv_rows_ratio"][i],
+                result,
             )
 
         # Test if missing value ratio is between 0 and 1
         for i, _ in enumerate(self.data_mv_df):
-            self.assertTrue(
-                0 <= _missing_vals(self.data_mv_df)["mv_rows_ratio"][i] <= 1
-            )
+            assert 0 <= _missing_vals(self.data_mv_df)["mv_rows_ratio"][i] <= 1
 
     def test_mv_cols_ratio(self):
         # Test missing values ratio for each column
         expected_results = [1 / 4, 0.25, 0.25, 0.5]
         for i, result in enumerate(expected_results):
             self.assertAlmostEqual(
-                _missing_vals(self.data_mv_df)["mv_cols_ratio"][i], result
+                _missing_vals(self.data_mv_df)["mv_cols_ratio"][i],
+                result,
             )
 
         # Test if missing value ratio is between 0 and 1
         for i, _ in enumerate(self.data_mv_df):
-            self.assertTrue(
-                0 <= _missing_vals(self.data_mv_df)["mv_cols_ratio"][i] <= 1
-            )
+            assert 0 <= _missing_vals(self.data_mv_df)["mv_cols_ratio"][i] <= 1
 
 
 class Test__validate_input(unittest.TestCase):
     def test__validate_input_bool(self):
         # Raises an exception if the input is not boolean
         with self.assertRaises(TypeError):
             _validate_input_bool("True", None)
@@ -257,9 +259,10 @@
             _validate_input_sum_larger(7, "Test Sum >= 7", 1, 2, 3)
 
     def test__validate_input_num_data(self):
         with self.assertRaises(TypeError):
             _validate_input_num_data(pd.DataFrame({"col1": ["a", "b", "c"]}), None)
 
         _validate_input_num_data(
-            pd.DataFrame({"col1": [1, 2, 3]}), None
+            pd.DataFrame({"col1": [1, 2, 3]}),
+            None,
         )  # No exception
```

### Comparing `klib-1.0.7/setup.py` & `klib-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,412 +1,470 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 655f 6469  etup..package_di
-00000040: 7220 3d20 5c0a 7b27 273a 2027 7372 6327  r = \.{'': 'src'
-00000050: 7d0a 0a70 6163 6b61 6765 7320 3d20 5c0a  }..packages = \.
-00000060: 5b27 6b6c 6962 272c 2027 6b6c 6962 2e73  ['klib', 'klib.s
-00000070: 6372 6970 7473 275d 0a0a 7061 636b 6167  cripts']..packag
-00000080: 655f 6461 7461 203d 205c 0a7b 2727 3a20  e_data = \.{'': 
-00000090: 5b27 2a27 5d7d 0a0a 696e 7374 616c 6c5f  ['*']}..install_
-000000a0: 7265 7175 6972 6573 203d 205c 0a5b 274a  requires = \.['J
-000000b0: 696e 6a61 323e 3d33 2e30 2e33 2c3c 342e  inja2>=3.0.3,<4.
-000000c0: 302e 3027 2c0a 2027 6d61 7470 6c6f 746c  0.0',. 'matplotl
-000000d0: 6962 3e3d 332e 302e 332c 3c34 2e30 2e30  ib>=3.0.3,<4.0.0
-000000e0: 272c 0a20 276e 756d 7079 3e3d 312e 3136  ',. 'numpy>=1.16
-000000f0: 2e33 2c3c 322e 302e 3027 2c0a 2027 7061  .3,<2.0.0',. 'pa
-00000100: 6e64 6173 3e3d 312e 322e 302c 3c32 2e30  ndas>=1.2.0,<2.0
-00000110: 2e30 272c 0a20 2773 6369 7079 3e3d 312e  .0',. 'scipy>=1.
-00000120: 312e 302c 3c32 2e30 2e30 272c 0a20 2773  1.0,<2.0.0',. 's
-00000130: 6561 626f 726e 3e3d 302e 3131 2e32 2c3c  eaborn>=0.11.2,<
-00000140: 302e 3133 2e30 275d 0a0a 7365 7475 705f  0.13.0']..setup_
-00000150: 6b77 6172 6773 203d 207b 0a20 2020 2027  kwargs = {.    '
-00000160: 6e61 6d65 273a 2027 6b6c 6962 272c 0a20  name': 'klib',. 
-00000170: 2020 2027 7665 7273 696f 6e27 3a20 2731     'version': '1
-00000180: 2e30 2e37 272c 0a20 2020 2027 6465 7363  .0.7',.    'desc
-00000190: 7269 7074 696f 6e27 3a20 2743 7573 746f  ription': 'Custo
-000001a0: 6d69 7a65 6420 6461 7461 2070 7265 7072  mized data prepr
-000001b0: 6f63 6573 7369 6e67 2066 756e 6374 696f  ocessing functio
-000001c0: 6e73 2066 6f72 2066 7265 7175 656e 7420  ns for frequent 
-000001d0: 7461 736b 732e 272c 0a20 2020 2027 6c6f  tasks.',.    'lo
-000001e0: 6e67 5f64 6573 6372 6970 7469 6f6e 273a  ng_description':
-000001f0: 2027 3c70 2061 6c69 676e 3d22 6365 6e74   '<p align="cent
-00000200: 6572 223e 3c69 6d67 2073 7263 3d22 6874  er"><img src="ht
-00000210: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00000220: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00000230: 616b 616e 7a31 2f6b 6c69 622f 6d61 696e  akanz1/klib/main
-00000240: 2f65 7861 6d70 6c65 732f 696d 6167 6573  /examples/images
-00000250: 2f68 6561 6465 722e 706e 6722 2061 6c74  /header.png" alt
-00000260: 3d22 6b6c 6962 2048 6561 6465 7222 2077  ="klib Header" w
-00000270: 6964 7468 3d22 3835 3922 2068 6569 6768  idth="859" heigh
-00000280: 743d 2233 3034 223e 3c2f 703e 5c6e 5c6e  t="304"></p>\n\n
-00000290: 5b21 5b46 6c61 6b65 3820 2620 5079 5465  [![Flake8 & PyTe
-000002a0: 7374 5d28 6874 7470 733a 2f2f 6769 7468  st](https://gith
-000002b0: 7562 2e63 6f6d 2f61 6b61 6e7a 312f 6b6c  ub.com/akanz1/kl
-000002c0: 6962 2f77 6f72 6b66 6c6f 7773 2f46 6c61  ib/workflows/Fla
-000002d0: 6b65 3825 3230 2546 3025 3946 2539 3025  ke8%20%F0%9F%90%
-000002e0: 3844 2532 3050 7954 6573 7425 3230 2532  8D%20PyTest%20%2
-000002f0: 3025 3230 2543 3225 4234 2f62 6164 6765  0%20%C2%B4/badge
-00000300: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
-00000310: 6974 6875 622e 636f 6d2f 616b 616e 7a31  ithub.com/akanz1
-00000320: 2f6b 6c69 6229 5c6e 5b21 5b4c 616e 6775  /klib)\n[![Langu
-00000330: 6167 655d 2868 7474 7073 3a2f 2f69 6d67  age](https://img
-00000340: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
-00000350: 7562 2f6c 616e 6775 6167 6573 2f74 6f70  ub/languages/top
-00000360: 2f61 6b61 6e7a 312f 6b6c 6962 295d 2868  /akanz1/klib)](h
-00000370: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
-00000380: 7072 6f6a 6563 742f 6b6c 6962 2f29 5c6e  project/klib/)\n
-00000390: 5b21 5b4c 6173 7420 436f 6d6d 6974 5d28  [![Last Commit](
-000003a0: 6874 7470 733a 2f2f 6261 6467 656e 2e6e  https://badgen.n
-000003b0: 6574 2f67 6974 6875 622f 6c61 7374 2d63  et/github/last-c
-000003c0: 6f6d 6d69 742f 616b 616e 7a31 2f6b 6c69  ommit/akanz1/kli
-000003d0: 622f 6d61 696e 295d 2868 7474 7073 3a2f  b/main)](https:/
-000003e0: 2f67 6974 6875 622e 636f 6d2f 616b 616e  /github.com/akan
-000003f0: 7a31 2f6b 6c69 622f 636f 6d6d 6974 732f  z1/klib/commits/
-00000400: 6d61 696e 295c 6e5b 215b 5175 616c 6974  main)\n[![Qualit
-00000410: 7920 4761 7465 2053 7461 7475 735d 2868  y Gate Status](h
-00000420: 7474 7073 3a2f 2f73 6f6e 6172 636c 6f75  ttps://sonarclou
-00000430: 642e 696f 2f61 7069 2f70 726f 6a65 6374  d.io/api/project
-00000440: 5f62 6164 6765 732f 6d65 6173 7572 653f  _badges/measure?
-00000450: 7072 6f6a 6563 743d 616b 616e 7a31 5f6b  project=akanz1_k
-00000460: 6c69 6226 6d65 7472 6963 3d61 6c65 7274  lib&metric=alert
-00000470: 5f73 7461 7475 7329 5d28 6874 7470 733a  _status)](https:
-00000480: 2f2f 736f 6e61 7263 6c6f 7564 2e69 6f2f  //sonarcloud.io/
-00000490: 6461 7368 626f 6172 643f 6964 3d61 6b61  dashboard?id=aka
-000004a0: 6e7a 315f 6b6c 6962 295c 6e5b 215b 5363  nz1_klib)\n[![Sc
-000004b0: 7275 7469 6e69 7a65 725d 2868 7474 7073  rutinizer](https
-000004c0: 3a2f 2f73 6372 7574 696e 697a 6572 2d63  ://scrutinizer-c
-000004d0: 692e 636f 6d2f 672f 616b 616e 7a31 2f6b  i.com/g/akanz1/k
-000004e0: 6c69 622f 6261 6467 6573 2f71 7561 6c69  lib/badges/quali
-000004f0: 7479 2d73 636f 7265 2e70 6e67 3f62 3d6d  ty-score.png?b=m
-00000500: 6169 6e29 5d28 6874 7470 733a 2f2f 7363  ain)](https://sc
-00000510: 7275 7469 6e69 7a65 722d 6369 2e63 6f6d  rutinizer-ci.com
-00000520: 2f67 2f61 6b61 6e7a 312f 6b6c 6962 2f29  /g/akanz1/klib/)
-00000530: 5c6e 5b21 5b63 6f64 6563 6f76 5d28 6874  \n[![codecov](ht
-00000540: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
-00000550: 2f67 682f 616b 616e 7a31 2f6b 6c69 622f  /gh/akanz1/klib/
-00000560: 6272 616e 6368 2f6d 6169 6e2f 6772 6170  branch/main/grap
-00000570: 682f 6261 6467 652e 7376 6729 5d28 6874  h/badge.svg)](ht
-00000580: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
-00000590: 2f67 682f 616b 616e 7a31 2f6b 6c69 6229  /gh/akanz1/klib)
-000005a0: 5c6e 5c6e 2a2a 6b6c 6962 2a2a 2069 7320  \n\n**klib** is 
-000005b0: 6120 5079 7468 6f6e 206c 6962 7261 7279  a Python library
-000005c0: 2066 6f72 2069 6d70 6f72 7469 6e67 2c20   for importing, 
-000005d0: 636c 6561 6e69 6e67 2c20 616e 616c 797a  cleaning, analyz
-000005e0: 696e 6720 616e 6420 7072 6570 726f 6365  ing and preproce
-000005f0: 7373 696e 6720 6461 7461 2e20 4578 706c  ssing data. Expl
-00000600: 616e 6174 696f 6e73 206f 6e20 6b65 7920  anations on key 
-00000610: 6675 6e63 7469 6f6e 616c 6974 6965 7320  functionalities 
-00000620: 6361 6e20 6265 2066 6f75 6e64 206f 6e20  can be found on 
-00000630: 5b4d 6564 6975 6d20 2f20 546f 7761 7264  [Medium / Toward
-00000640: 7344 6174 6153 6369 656e 6365 5d28 6874  sDataScience](ht
-00000650: 7470 733a 2f2f 6d65 6469 756d 2e63 6f6d  tps://medium.com
-00000660: 2f40 616b 616e 7a29 2061 6e64 2069 6e20  /@akanz) and in 
-00000670: 7468 6520 5b65 7861 6d70 6c65 735d 2865  the [examples](e
-00000680: 7861 6d70 6c65 7329 2073 6563 7469 6f6e  xamples) section
-00000690: 2e20 4164 6469 7469 6f6e 616c 6c79 2c20  . Additionally, 
-000006a0: 7468 6572 6520 6172 6520 6772 6561 7420  there are great 
-000006b0: 696e 7472 6f64 7563 7469 6f6e 7320 616e  introductions an
-000006c0: 6420 6f76 6572 7669 6577 7320 6f66 2074  d overviews of t
-000006d0: 6865 2066 756e 6374 696f 6e61 6c69 7479  he functionality
-000006e0: 206f 6e20 5b50 7974 686f 6e42 7974 6573   on [PythonBytes
-000006f0: 5d28 6874 7470 733a 2f2f 7079 7468 6f6e  ](https://python
-00000700: 6279 7465 732e 666d 2f65 7069 736f 6465  bytes.fm/episode
-00000710: 732f 7368 6f77 2f32 3430 2f74 6869 732d  s/show/240/this-
-00000720: 6973 2d67 6974 6875 622d 796f 7572 2d70  is-github-your-p
-00000730: 696c 6f74 2d73 7065 616b 696e 6729 206f  ilot-speaking) o
-00000740: 7220 6f6e 205b 596f 7554 7562 6520 2844  r on [YouTube (D
-00000750: 6174 6120 5072 6f66 6573 736f 7229 5d28  ata Professor)](
-00000760: 6874 7470 733a 2f2f 7777 772e 796f 7574  https://www.yout
-00000770: 7562 652e 636f 6d2f 7761 7463 683f 763d  ube.com/watch?v=
-00000780: 5552 6a4a 5645 655a 7878 5529 2e5c 6e5c  URjJVEeZxxU).\n\
-00000790: 6e23 2320 496e 7374 616c 6c61 7469 6f6e  n## Installation
-000007a0: 5c6e 5c6e 5573 6520 7468 6520 7061 636b  \n\nUse the pack
-000007b0: 6167 6520 6d61 6e61 6765 7220 5b70 6970  age manager [pip
-000007c0: 5d28 6874 7470 733a 2f2f 7069 702e 7079  ](https://pip.py
-000007d0: 7061 2e69 6f2f 656e 2f73 7461 626c 652f  pa.io/en/stable/
-000007e0: 2920 746f 2069 6e73 7461 6c6c 206b 6c69  ) to install kli
-000007f0: 622e 5c6e 5c6e 5b21 5b50 7950 4920 5665  b.\n\n[![PyPI Ve
-00000800: 7273 696f 6e5d 2868 7474 7073 3a2f 2f69  rsion](https://i
-00000810: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-00000820: 7069 2f76 2f6b 6c69 6229 5d28 6874 7470  pi/v/klib)](http
-00000830: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-00000840: 6a65 6374 2f6b 6c69 622f 295c 6e5b 215b  ject/klib/)\n[![
-00000850: 446f 776e 6c6f 6164 735d 2868 7474 7073  Downloads](https
-00000860: 3a2f 2f70 6570 792e 7465 6368 2f62 6164  ://pepy.tech/bad
-00000870: 6765 2f6b 6c69 622f 6d6f 6e74 6829 5d28  ge/klib/month)](
-00000880: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-00000890: 2f70 726f 6a65 6374 2f6b 6c69 622f 295c  /project/klib/)\
-000008a0: 6e5c 6e60 6060 6261 7368 5c6e 7069 7020  n\n```bash\npip 
-000008b0: 696e 7374 616c 6c20 2d55 206b 6c69 625c  install -U klib\
-000008c0: 6e60 6060 5c6e 5c6e 416c 7465 726e 6174  n```\n\nAlternat
-000008d0: 6976 656c 792c 2074 6f20 696e 7374 616c  ively, to instal
-000008e0: 6c20 7468 6973 2070 6163 6b61 6765 2077  l this package w
-000008f0: 6974 6820 636f 6e64 6120 7275 6e3a 5c6e  ith conda run:\n
-00000900: 5c6e 5b21 5b43 6f6e 6461 2056 6572 7369  \n[![Conda Versi
-00000910: 6f6e 5d28 6874 7470 733a 2f2f 696d 672e  on](https://img.
-00000920: 7368 6965 6c64 732e 696f 2f63 6f6e 6461  shields.io/conda
-00000930: 2f76 6e2f 636f 6e64 612d 666f 7267 652f  /vn/conda-forge/
-00000940: 6b6c 6962 295d 2868 7474 7073 3a2f 2f61  klib)](https://a
-00000950: 6e61 636f 6e64 612e 6f72 672f 636f 6e64  naconda.org/cond
-00000960: 612d 666f 7267 652f 6b6c 6962 295c 6e5b  a-forge/klib)\n[
-00000970: 215b 436f 6e64 6120 446f 776e 6c6f 6164  ![Conda Download
-00000980: 735d 2868 7474 7073 3a2f 2f69 6d67 2e73  s](https://img.s
-00000990: 6869 656c 6473 2e69 6f2f 636f 6e64 612f  hields.io/conda/
-000009a0: 646e 2f63 6f6e 6461 2d66 6f72 6765 2f6b  dn/conda-forge/k
-000009b0: 6c69 622e 7376 6729 5d28 6874 7470 733a  lib.svg)](https:
-000009c0: 2f2f 616e 6163 6f6e 6461 2e6f 7267 2f63  //anaconda.org/c
-000009d0: 6f6e 6461 2d66 6f72 6765 2f6b 6c69 6229  onda-forge/klib)
-000009e0: 5c6e 5c6e 6060 6062 6173 685c 6e63 6f6e  \n\n```bash\ncon
-000009f0: 6461 2069 6e73 7461 6c6c 202d 6320 636f  da install -c co
-00000a00: 6e64 612d 666f 7267 6520 6b6c 6962 5c6e  nda-forge klib\n
-00000a10: 6060 605c 6e5c 6e23 2320 5573 6167 655c  ```\n\n## Usage\
-00000a20: 6e5c 6e60 6060 7079 7468 6f6e 5c6e 696d  n\n```python\nim
-00000a30: 706f 7274 206b 6c69 625c 6e69 6d70 6f72  port klib\nimpor
-00000a40: 7420 7061 6e64 6173 2061 7320 7064 5c6e  t pandas as pd\n
-00000a50: 5c6e 6466 203d 2070 642e 4461 7461 4672  \ndf = pd.DataFr
-00000a60: 616d 6528 6461 7461 295c 6e5c 6e23 206b  ame(data)\n\n# k
-00000a70: 6c69 622e 6465 7363 7269 6265 202d 2066  lib.describe - f
-00000a80: 756e 6374 696f 6e73 2066 6f72 2076 6973  unctions for vis
-00000a90: 7561 6c69 7a69 6e67 2064 6174 6173 6574  ualizing dataset
-00000aa0: 735c 6e2d 206b 6c69 622e 6361 745f 706c  s\n- klib.cat_pl
-00000ab0: 6f74 2864 6629 2023 2072 6574 7572 6e73  ot(df) # returns
-00000ac0: 2061 2076 6973 7561 6c69 7a61 7469 6f6e   a visualization
-00000ad0: 206f 6620 7468 6520 6e75 6d62 6572 2061   of the number a
-00000ae0: 6e64 2066 7265 7175 656e 6379 206f 6620  nd frequency of 
-00000af0: 6361 7465 676f 7269 6361 6c20 6665 6174  categorical feat
-00000b00: 7572 6573 5c6e 2d20 6b6c 6962 2e63 6f72  ures\n- klib.cor
-00000b10: 725f 6d61 7428 6466 2920 2320 7265 7475  r_mat(df) # retu
-00000b20: 726e 7320 6120 636f 6c6f 722d 656e 636f  rns a color-enco
-00000b30: 6465 6420 636f 7272 656c 6174 696f 6e20  ded correlation 
-00000b40: 6d61 7472 6978 5c6e 2d20 6b6c 6962 2e63  matrix\n- klib.c
-00000b50: 6f72 725f 706c 6f74 2864 6629 2023 2072  orr_plot(df) # r
-00000b60: 6574 7572 6e73 2061 2063 6f6c 6f72 2d65  eturns a color-e
-00000b70: 6e63 6f64 6564 2068 6561 746d 6170 2c20  ncoded heatmap, 
-00000b80: 6964 6561 6c20 666f 7220 636f 7272 656c  ideal for correl
-00000b90: 6174 696f 6e73 5c6e 2d20 6b6c 6962 2e64  ations\n- klib.d
-00000ba0: 6973 745f 706c 6f74 2864 6629 2023 2072  ist_plot(df) # r
-00000bb0: 6574 7572 6e73 2061 2064 6973 7472 6962  eturns a distrib
-00000bc0: 7574 696f 6e20 706c 6f74 2066 6f72 2065  ution plot for e
-00000bd0: 7665 7279 206e 756d 6572 6963 2066 6561  very numeric fea
-00000be0: 7475 7265 5c6e 2d20 6b6c 6962 2e6d 6973  ture\n- klib.mis
-00000bf0: 7369 6e67 7661 6c5f 706c 6f74 2864 6629  singval_plot(df)
-00000c00: 2023 2072 6574 7572 6e73 2061 2066 6967   # returns a fig
-00000c10: 7572 6520 636f 6e74 6169 6e69 6e67 2069  ure containing i
-00000c20: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
-00000c30: 206d 6973 7369 6e67 2076 616c 7565 735c   missing values\
-00000c40: 6e5c 6e23 206b 6c69 622e 636c 6561 6e20  n\n# klib.clean 
-00000c50: 2d20 6675 6e63 7469 6f6e 7320 666f 7220  - functions for 
-00000c60: 636c 6561 6e69 6e67 2064 6174 6173 6574  cleaning dataset
-00000c70: 735c 6e2d 206b 6c69 622e 6461 7461 5f63  s\n- klib.data_c
-00000c80: 6c65 616e 696e 6728 6466 2920 2320 7065  leaning(df) # pe
-00000c90: 7266 6f72 6d73 2064 6174 6163 6c65 616e  rforms dataclean
-00000ca0: 696e 6720 2864 726f 7020 6475 706c 6963  ing (drop duplic
-00000cb0: 6174 6573 2026 2065 6d70 7479 2072 6f77  ates & empty row
-00000cc0: 732f 636f 6c73 2c20 6164 6a75 7374 2064  s/cols, adjust d
-00000cd0: 7479 7065 732c 2e2e 2e29 5c6e 2d20 6b6c  types,...)\n- kl
-00000ce0: 6962 2e63 6c65 616e 5f63 6f6c 756d 6e5f  ib.clean_column_
-00000cf0: 6e61 6d65 7328 6466 2920 2320 636c 6561  names(df) # clea
-00000d00: 6e73 2061 6e64 2073 7461 6e64 6172 6469  ns and standardi
-00000d10: 7a65 7320 636f 6c75 6d6e 206e 616d 6573  zes column names
-00000d20: 2c20 616c 736f 2063 616c 6c65 6420 696e  , also called in
-00000d30: 7369 6465 2064 6174 615f 636c 6561 6e69  side data_cleani
-00000d40: 6e67 2829 5c6e 2d20 6b6c 6962 2e63 6f6e  ng()\n- klib.con
-00000d50: 7665 7274 5f64 6174 6174 7970 6573 2864  vert_datatypes(d
-00000d60: 6629 2023 2063 6f6e 7665 7274 7320 6578  f) # converts ex
-00000d70: 6973 7469 6e67 2074 6f20 6d6f 7265 2065  isting to more e
-00000d80: 6666 6963 6965 6e74 2064 7479 7065 732c  fficient dtypes,
-00000d90: 2061 6c73 6f20 6361 6c6c 6564 2069 6e73   also called ins
-00000da0: 6964 6520 6461 7461 5f63 6c65 616e 696e  ide data_cleanin
-00000db0: 6728 295c 6e2d 206b 6c69 622e 6472 6f70  g()\n- klib.drop
-00000dc0: 5f6d 6973 7369 6e67 2864 6629 2023 2064  _missing(df) # d
-00000dd0: 726f 7073 206d 6973 7369 6e67 2076 616c  rops missing val
-00000de0: 7565 732c 2061 6c73 6f20 6361 6c6c 6564  ues, also called
-00000df0: 2069 6e20 6461 7461 5f63 6c65 616e 696e   in data_cleanin
-00000e00: 6728 295c 6e2d 206b 6c69 622e 6d76 5f63  g()\n- klib.mv_c
-00000e10: 6f6c 5f68 616e 646c 696e 6728 6466 2920  ol_handling(df) 
-00000e20: 2320 6472 6f70 7320 6665 6174 7572 6573  # drops features
-00000e30: 2077 6974 6820 6869 6768 2072 6174 696f   with high ratio
-00000e40: 206f 6620 6d69 7373 696e 6720 7661 6c73   of missing vals
-00000e50: 2062 6173 6564 206f 6e20 696e 666f 726d   based on inform
-00000e60: 6174 696f 6e61 6c20 636f 6e74 656e 745c  ational content\
-00000e70: 6e2d 206b 6c69 622e 706f 6f6c 5f64 7570  n- klib.pool_dup
-00000e80: 6c69 6361 7465 5f73 7562 7365 7473 2864  licate_subsets(d
-00000e90: 6629 2023 2070 6f6f 6c73 2073 7562 7365  f) # pools subse
-00000ea0: 7420 6f66 2063 6f6c 7320 6261 7365 6420  t of cols based 
-00000eb0: 6f6e 2064 7570 6c69 6361 7465 7320 7769  on duplicates wi
-00000ec0: 7468 206d 696e 2e20 6c6f 7373 206f 6620  th min. loss of 
-00000ed0: 696e 666f 726d 6174 696f 6e5c 6e60 6060  information\n```
-00000ee0: 5c6e 5c6e 2323 2045 7861 6d70 6c65 735c  \n\n## Examples\
-00000ef0: 6e5c 6e46 696e 6420 616c 6c20 6176 6169  n\nFind all avai
-00000f00: 6c61 626c 6520 6578 616d 706c 6573 2061  lable examples a
-00000f10: 7320 7765 6c6c 2061 7320 6170 706c 6963  s well as applic
-00000f20: 6174 696f 6e73 206f 6620 7468 6520 6675  ations of the fu
-00000f30: 6e63 7469 6f6e 7320 696e 202a 2a6b 6c69  nctions in **kli
-00000f40: 622e 636c 6561 6e28 292a 2a20 7769 7468  b.clean()** with
-00000f50: 2064 6574 6169 6c65 6420 6465 7363 7269   detailed descri
-00000f60: 7074 696f 6e73 203c 6120 6872 6566 3d22  ptions <a href="
-00000f70: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000f80: 6f6d 2f61 6b61 6e7a 312f 6b6c 6962 2f74  om/akanz1/klib/t
-00000f90: 7265 652f 6d61 696e 2f65 7861 6d70 6c65  ree/main/example
-00000fa0: 7322 3e68 6572 653c 2f61 3e2e 5c6e 5c6e  s">here</a>.\n\n
-00000fb0: 6060 6070 7974 686f 6e5c 6e6b 6c69 622e  ```python\nklib.
-00000fc0: 6d69 7373 696e 6776 616c 5f70 6c6f 7428  missingval_plot(
-00000fd0: 6466 2920 2320 6465 6661 756c 7420 7265  df) # default re
-00000fe0: 7072 6573 656e 7461 7469 6f6e 206f 6620  presentation of 
-00000ff0: 6d69 7373 696e 6720 7661 6c75 6573 2069  missing values i
-00001000: 6e20 6120 4461 7461 4672 616d 652c 2070  n a DataFrame, p
-00001010: 6c65 6e74 7920 6f66 2073 6574 7469 6e67  lenty of setting
-00001020: 7320 6172 6520 6176 6169 6c61 626c 655c  s are available\
-00001030: 6e60 6060 5c6e 5c6e 3c70 2061 6c69 676e  n```\n\n<p align
-00001040: 3d22 6365 6e74 6572 223e 3c69 6d67 2073  ="center"><img s
-00001050: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
-00001060: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-00001070: 742e 636f 6d2f 616b 616e 7a31 2f6b 6c69  t.com/akanz1/kli
-00001080: 622f 6d61 696e 2f65 7861 6d70 6c65 732f  b/main/examples/
-00001090: 696d 6167 6573 2f65 7861 6d70 6c65 5f6d  images/example_m
-000010a0: 765f 706c 6f74 2e70 6e67 2220 616c 743d  v_plot.png" alt=
-000010b0: 224d 6973 7369 6e67 7661 6c75 6520 506c  "Missingvalue Pl
-000010c0: 6f74 2045 7861 6d70 6c65 2220 7769 6474  ot Example" widt
-000010d0: 683d 2231 3030 3022 2068 6569 6768 743d  h="1000" height=
-000010e0: 2231 3039 3122 3e3c 2f70 3e5c 6e5c 6e60  "1091"></p>\n\n`
-000010f0: 6060 7079 7468 6f6e 5c6e 6b6c 6962 2e63  ``python\nklib.c
-00001100: 6f72 725f 706c 6f74 2864 662c 2073 706c  orr_plot(df, spl
-00001110: 6974 3d5c 2770 6f73 5c27 2920 2320 6469  it=\'pos\') # di
-00001120: 7370 6c61 7969 6e67 206f 6e6c 7920 706f  splaying only po
-00001130: 7369 7469 7665 2063 6f72 7265 6c61 7469  sitive correlati
-00001140: 6f6e 732c 206f 7468 6572 2073 6574 7469  ons, other setti
-00001150: 6e67 7320 696e 636c 7564 6520 7468 7265  ngs include thre
-00001160: 7368 6f6c 642c 2063 6d61 702e 2e2e 5c6e  shold, cmap...\n
-00001170: 6b6c 6962 2e63 6f72 725f 706c 6f74 2864  klib.corr_plot(d
-00001180: 662c 2073 706c 6974 3d5c 276e 6567 5c27  f, split=\'neg\'
-00001190: 2920 2320 6469 7370 6c61 7969 6e67 206f  ) # displaying o
-000011a0: 6e6c 7920 6e65 6761 7469 7665 2063 6f72  nly negative cor
-000011b0: 7265 6c61 7469 6f6e 735c 6e60 6060 5c6e  relations\n```\n
-000011c0: 5c6e 3c70 2061 6c69 676e 3d22 6365 6e74  \n<p align="cent
-000011d0: 6572 223e 3c69 6d67 2073 7263 3d22 6874  er"><img src="ht
-000011e0: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-000011f0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00001200: 616b 616e 7a31 2f6b 6c69 622f 6d61 696e  akanz1/klib/main
-00001210: 2f65 7861 6d70 6c65 732f 696d 6167 6573  /examples/images
-00001220: 2f65 7861 6d70 6c65 5f63 6f72 725f 706c  /example_corr_pl
-00001230: 6f74 2e70 6e67 2220 616c 743d 2243 6f72  ot.png" alt="Cor
-00001240: 7220 506c 6f74 2045 7861 6d70 6c65 2220  r Plot Example" 
-00001250: 7769 6474 683d 2237 3230 2220 6865 6967  width="720" heig
-00001260: 6874 3d22 3333 3822 3e3c 2f70 3e5c 6e5c  ht="338"></p>\n\
-00001270: 6e60 6060 7079 7468 6f6e 5c6e 6b6c 6962  n```python\nklib
-00001280: 2e63 6f72 725f 706c 6f74 2864 662c 2074  .corr_plot(df, t
-00001290: 6172 6765 743d 5c27 7769 6e65 5c27 2920  arget=\'wine\') 
-000012a0: 2320 6465 6661 756c 7420 7265 7072 6573  # default repres
-000012b0: 656e 7461 7469 6f6e 206f 6620 636f 7272  entation of corr
-000012c0: 656c 6174 696f 6e73 2077 6974 6820 7468  elations with th
-000012d0: 6520 6665 6174 7572 6520 636f 6c75 6d6e  e feature column
-000012e0: 5c6e 6060 605c 6e5c 6e3c 7020 616c 6967  \n```\n\n<p alig
-000012f0: 6e3d 2263 656e 7465 7222 3e3c 696d 6720  n="center"><img 
-00001300: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
-00001310: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00001320: 6e74 2e63 6f6d 2f61 6b61 6e7a 312f 6b6c  nt.com/akanz1/kl
-00001330: 6962 2f6d 6169 6e2f 6578 616d 706c 6573  ib/main/examples
-00001340: 2f69 6d61 6765 732f 6578 616d 706c 655f  /images/example_
-00001350: 7461 7267 6574 5f63 6f72 725f 706c 6f74  target_corr_plot
-00001360: 2e70 6e67 2220 616c 743d 2254 6172 6765  .png" alt="Targe
-00001370: 7420 436f 7272 2050 6c6f 7420 4578 616d  t Corr Plot Exam
-00001380: 706c 6522 2077 6964 7468 3d22 3732 3022  ple" width="720"
-00001390: 2068 6569 6768 743d 2236 3030 223e 3c2f   height="600"></
-000013a0: 703e 5c6e 5c6e 6060 6070 7974 686f 6e5c  p>\n\n```python\
-000013b0: 6e6b 6c69 622e 6469 7374 5f70 6c6f 7428  nklib.dist_plot(
-000013c0: 6466 2920 2320 6465 6661 756c 7420 7265  df) # default re
-000013d0: 7072 6573 656e 7461 7469 6f6e 206f 6620  presentation of 
-000013e0: 6120 6469 7374 7269 6275 7469 6f6e 2070  a distribution p
-000013f0: 6c6f 742c 206f 7468 6572 2073 6574 7469  lot, other setti
-00001400: 6e67 7320 696e 636c 7564 6520 6669 6c6c  ngs include fill
-00001410: 5f72 616e 6765 2c20 6869 7374 6f67 7261  _range, histogra
-00001420: 6d2c 202e 2e2e 5c6e 6060 605c 6e5c 6e3c  m, ...\n```\n\n<
-00001430: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
-00001440: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
-00001450: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
-00001460: 7263 6f6e 7465 6e74 2e63 6f6d 2f61 6b61  rcontent.com/aka
-00001470: 6e7a 312f 6b6c 6962 2f6d 6169 6e2f 6578  nz1/klib/main/ex
-00001480: 616d 706c 6573 2f69 6d61 6765 732f 6578  amples/images/ex
-00001490: 616d 706c 655f 6469 7374 5f70 6c6f 742e  ample_dist_plot.
-000014a0: 706e 6722 2061 6c74 3d22 4469 7374 2050  png" alt="Dist P
-000014b0: 6c6f 7420 4578 616d 706c 6522 2077 6964  lot Example" wid
-000014c0: 7468 3d22 3931 3022 2068 6569 6768 743d  th="910" height=
-000014d0: 2231 3330 223e 3c2f 703e 5c6e 5c6e 6060  "130"></p>\n\n``
-000014e0: 6070 7974 686f 6e5c 6e6b 6c69 622e 6361  `python\nklib.ca
-000014f0: 745f 706c 6f74 2864 6174 612c 2074 6f70  t_plot(data, top
-00001500: 3d34 2c20 626f 7474 6f6d 3d34 2920 2320  =4, bottom=4) # 
-00001510: 7265 7072 6573 656e 7461 7469 6f6e 206f  representation o
-00001520: 6620 7468 6520 3420 6d6f 7374 2026 206c  f the 4 most & l
-00001530: 6561 7374 2063 6f6d 6d6f 6e20 7661 6c75  east common valu
-00001540: 6573 2069 6e20 6561 6368 2063 6174 6567  es in each categ
-00001550: 6f72 6963 616c 2063 6f6c 756d 6e5c 6e60  orical column\n`
-00001560: 6060 5c6e 5c6e 3c70 2061 6c69 676e 3d22  ``\n\n<p align="
-00001570: 6365 6e74 6572 223e 3c69 6d67 2073 7263  center"><img src
-00001580: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-00001590: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-000015a0: 636f 6d2f 616b 616e 7a31 2f6b 6c69 622f  com/akanz1/klib/
-000015b0: 6d61 696e 2f65 7861 6d70 6c65 732f 696d  main/examples/im
-000015c0: 6167 6573 2f65 7861 6d70 6c65 5f63 6174  ages/example_cat
-000015d0: 5f70 6c6f 742e 706e 6722 2061 6c74 3d22  _plot.png" alt="
-000015e0: 4361 7420 506c 6f74 2045 7861 6d70 6c65  Cat Plot Example
-000015f0: 2220 7769 6474 683d 2231 3030 3022 2068  " width="1000" h
-00001600: 6569 6768 743d 2231 3030 3022 3e3c 2f70  eight="1000"></p
-00001610: 3e5c 6e5c 6e46 7572 7468 6572 2065 7861  >\n\nFurther exa
-00001620: 6d70 6c65 732c 2061 7320 7765 6c6c 2061  mples, as well a
-00001630: 7320 6170 706c 6963 6174 696f 6e73 206f  s applications o
-00001640: 6620 7468 6520 6675 6e63 7469 6f6e 7320  f the functions 
-00001650: 696e 202a 2a6b 6c69 622e 636c 6561 6e28  in **klib.clean(
-00001660: 292a 2a20 6361 6e20 6265 2066 6f75 6e64  )** can be found
-00001670: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00001680: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6b61  //github.com/aka
-00001690: 6e7a 312f 6b6c 6962 2f74 7265 652f 6d61  nz1/klib/tree/ma
-000016a0: 696e 2f65 7861 6d70 6c65 7323 6461 7461  in/examples#data
-000016b0: 2d63 6c65 616e 696e 672d 616e 642d 6167  -cleaning-and-ag
-000016c0: 6772 6574 6174 696f 6e22 3e68 6572 653c  gretation">here<
-000016d0: 2f61 3e2e 5c6e 5c6e 2323 2043 6f6e 7472  /a>.\n\n## Contr
-000016e0: 6962 7574 696e 675c 6e5c 6e5b 215b 4f70  ibuting\n\n[![Op
-000016f0: 656e 2069 6e20 5669 7375 616c 2053 7475  en in Visual Stu
-00001700: 6469 6f20 436f 6465 5d28 6874 7470 733a  dio Code](https:
-00001710: 2f2f 6f70 656e 2e76 7363 6f64 652e 6465  //open.vscode.de
-00001720: 762f 6261 6467 6573 2f6f 7065 6e2d 696e  v/badges/open-in
-00001730: 2d76 7363 6f64 652e 7376 6729 5d28 6874  -vscode.svg)](ht
-00001740: 7470 733a 2f2f 6f70 656e 2e76 7363 6f64  tps://open.vscod
-00001750: 652e 6465 762f 616b 616e 7a31 2f6b 6c69  e.dev/akanz1/kli
-00001760: 6229 5c6e 5c6e 5075 6c6c 2072 6571 7565  b)\n\nPull reque
-00001770: 7374 7320 616e 6420 6964 6561 732c 2065  sts and ideas, e
-00001780: 7370 6563 6961 6c6c 7920 666f 7220 6675  specially for fu
-00001790: 7274 6865 7220 6675 6e63 7469 6f6e 7320  rther functions 
-000017a0: 6172 6520 7765 6c63 6f6d 652e 2046 6f72  are welcome. For
-000017b0: 206d 616a 6f72 2063 6861 6e67 6573 206f   major changes o
-000017c0: 7220 6665 6564 6261 636b 2c20 706c 6561  r feedback, plea
-000017d0: 7365 206f 7065 6e20 616e 2069 7373 7565  se open an issue
-000017e0: 2066 6972 7374 2074 6f20 6469 7363 7573   first to discus
-000017f0: 7320 7768 6174 2079 6f75 2077 6f75 6c64  s what you would
-00001800: 206c 696b 6520 746f 2063 6861 6e67 652e   like to change.
-00001810: 5c6e 5c6e 2323 204c 6963 656e 7365 5c6e  \n\n## License\n
-00001820: 5c6e 5b4d 4954 5d28 6874 7470 733a 2f2f  \n[MIT](https://
-00001830: 6368 6f6f 7365 616c 6963 656e 7365 2e63  choosealicense.c
-00001840: 6f6d 2f6c 6963 656e 7365 732f 6d69 742f  om/licenses/mit/
-00001850: 295c 6e27 2c0a 2020 2020 2761 7574 686f  )\n',.    'autho
-00001860: 7227 3a20 2741 6e64 7265 6173 204b 616e  r': 'Andreas Kan
-00001870: 7a27 2c0a 2020 2020 2761 7574 686f 725f  z',.    'author_
-00001880: 656d 6169 6c27 3a20 2761 6e64 7265 6173  email': 'andreas
-00001890: 4061 6b61 6e7a 2e64 6527 2c0a 2020 2020  @akanz.de',.    
-000018a0: 276d 6169 6e74 6169 6e65 7227 3a20 274e  'maintainer': 'N
-000018b0: 6f6e 6527 2c0a 2020 2020 276d 6169 6e74  one',.    'maint
-000018c0: 6169 6e65 725f 656d 6169 6c27 3a20 274e  ainer_email': 'N
-000018d0: 6f6e 6527 2c0a 2020 2020 2775 726c 273a  one',.    'url':
-000018e0: 2027 4e6f 6e65 272c 0a20 2020 2027 7061   'None',.    'pa
-000018f0: 636b 6167 655f 6469 7227 3a20 7061 636b  ckage_dir': pack
-00001900: 6167 655f 6469 722c 0a20 2020 2027 7061  age_dir,.    'pa
-00001910: 636b 6167 6573 273a 2070 6163 6b61 6765  ckages': package
-00001920: 732c 0a20 2020 2027 7061 636b 6167 655f  s,.    'package_
-00001930: 6461 7461 273a 2070 6163 6b61 6765 5f64  data': package_d
-00001940: 6174 612c 0a20 2020 2027 696e 7374 616c  ata,.    'instal
-00001950: 6c5f 7265 7175 6972 6573 273a 2069 6e73  l_requires': ins
-00001960: 7461 6c6c 5f72 6571 7569 7265 732c 0a20  tall_requires,. 
-00001970: 2020 2027 7079 7468 6f6e 5f72 6571 7569     'python_requi
-00001980: 7265 7327 3a20 273e 3d33 2e38 2e30 2c3c  res': '>=3.8.0,<
-00001990: 332e 3132 272c 0a7d 0a0a 0a73 6574 7570  3.12',.}...setup
-000019a0: 282a 2a73 6574 7570 5f6b 7761 7267 7329  (**setup_kwargs)
-000019b0: 0a                                       .
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6b6c 6962  : 2.1.Name: klib
+00000020: 0a56 6572 7369 6f6e 3a20 312e 312e 300a  .Version: 1.1.0.
+00000030: 5375 6d6d 6172 793a 2043 7573 746f 6d69  Summary: Customi
+00000040: 7a65 6420 6461 7461 2070 7265 7072 6f63  zed data preproc
+00000050: 6573 7369 6e67 2066 756e 6374 696f 6e73  essing functions
+00000060: 2066 6f72 2066 7265 7175 656e 7420 7461   for frequent ta
+00000070: 736b 732e 0a4c 6963 656e 7365 3a20 4d49  sks..License: MI
+00000080: 540a 4175 7468 6f72 3a20 416e 6472 6561  T.Author: Andrea
+00000090: 7320 4b61 6e7a 0a41 7574 686f 722d 656d  s Kanz.Author-em
+000000a0: 6169 6c3a 2061 6e64 7265 6173 4061 6b61  ail: andreas@aka
+000000b0: 6e7a 2e64 650a 5265 7175 6972 6573 2d50  nz.de.Requires-P
+000000c0: 7974 686f 6e3a 203e 3d33 2e38 2e30 2c3c  ython: >=3.8.0,<
+000000d0: 342e 302e 300a 436c 6173 7369 6669 6572  4.0.0.Classifier
+000000e0: 3a20 4c69 6365 6e73 6520 3a3a 204f 5349  : License :: OSI
+000000f0: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
+00000100: 204c 6963 656e 7365 0a43 6c61 7373 6966   License.Classif
+00000110: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000120: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000130: 686f 6e20 3a3a 2033 0a43 6c61 7373 6966  hon :: 3.Classif
+00000140: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000150: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000160: 686f 6e20 3a3a 2033 2e38 0a43 6c61 7373  hon :: 3.8.Class
+00000170: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000180: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000190: 7974 686f 6e20 3a3a 2033 2e39 0a43 6c61  ython :: 3.9.Cla
+000001a0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+000001b0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000001c0: 2050 7974 686f 6e20 3a3a 2033 2e31 300a   Python :: 3.10.
+000001d0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+000001e0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000001f0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000200: 3131 0a52 6571 7569 7265 732d 4469 7374  11.Requires-Dist
+00000210: 3a20 4a69 6e6a 6132 2028 3e3d 332e 302e  : Jinja2 (>=3.0.
+00000220: 332c 3c34 2e30 2e30 290a 5265 7175 6972  3,<4.0.0).Requir
+00000230: 6573 2d44 6973 743a 206d 6174 706c 6f74  es-Dist: matplot
+00000240: 6c69 6220 283e 3d33 2e30 2e33 2c3c 342e  lib (>=3.0.3,<4.
+00000250: 302e 3029 0a52 6571 7569 7265 732d 4469  0.0).Requires-Di
+00000260: 7374 3a20 6e75 6d70 7920 283e 3d31 2e31  st: numpy (>=1.1
+00000270: 362e 332c 3c32 2e30 2e30 290a 5265 7175  6.3,<2.0.0).Requ
+00000280: 6972 6573 2d44 6973 743a 2070 616e 6461  ires-Dist: panda
+00000290: 7320 283e 3d31 2e32 2c3c 332e 3029 0a52  s (>=1.2,<3.0).R
+000002a0: 6571 7569 7265 732d 4469 7374 3a20 706c  equires-Dist: pl
+000002b0: 6f74 6c79 2028 3e3d 352e 322e 322c 3c36  otly (>=5.2.2,<6
+000002c0: 2e30 2e30 290a 5265 7175 6972 6573 2d44  .0.0).Requires-D
+000002d0: 6973 743a 2073 6369 7079 2028 3e3d 312e  ist: scipy (>=1.
+000002e0: 312e 302c 3c32 2e30 2e30 290a 5265 7175  1.0,<2.0.0).Requ
+000002f0: 6972 6573 2d44 6973 743a 2073 6372 6565  ires-Dist: scree
+00000300: 6e69 6e66 6f20 283e 3d30 2e38 2e31 2c3c  ninfo (>=0.8.1,<
+00000310: 302e 392e 3029 0a52 6571 7569 7265 732d  0.9.0).Requires-
+00000320: 4469 7374 3a20 7365 6162 6f72 6e20 283e  Dist: seaborn (>
+00000330: 3d30 2e31 312e 3229 0a44 6573 6372 6970  =0.11.2).Descrip
+00000340: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
+00000350: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
+00000360: 0a0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
+00000370: 6572 223e 3c69 6d67 2073 7263 3d22 6874  er"><img src="ht
+00000380: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00000390: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+000003a0: 616b 616e 7a31 2f6b 6c69 622f 6d61 696e  akanz1/klib/main
+000003b0: 2f65 7861 6d70 6c65 732f 696d 6167 6573  /examples/images
+000003c0: 2f68 6561 6465 722e 706e 6722 2061 6c74  /header.png" alt
+000003d0: 3d22 6b6c 6962 2048 6561 6465 7222 2077  ="klib Header" w
+000003e0: 6964 7468 3d22 3835 3922 2068 6569 6768  idth="859" heigh
+000003f0: 743d 2233 3034 223e 3c2f 703e 0a0a 5b21  t="304"></p>..[!
+00000400: 5b46 6c61 6b65 3820 2620 5079 5465 7374  [Flake8 & PyTest
+00000410: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000420: 2e63 6f6d 2f61 6b61 6e7a 312f 6b6c 6962  .com/akanz1/klib
+00000430: 2f77 6f72 6b66 6c6f 7773 2f46 6c61 6b65  /workflows/Flake
+00000440: 3825 3230 2546 3025 3946 2539 3025 3844  8%20%F0%9F%90%8D
+00000450: 2532 3050 7954 6573 7425 3230 2532 3025  %20PyTest%20%20%
+00000460: 3230 2543 3225 4234 2f62 6164 6765 2e73  20%C2%B4/badge.s
+00000470: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
+00000480: 6875 622e 636f 6d2f 616b 616e 7a31 2f6b  hub.com/akanz1/k
+00000490: 6c69 6229 0a5b 215b 4c61 6e67 7561 6765  lib).[![Language
+000004a0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+000004b0: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+000004c0: 6c61 6e67 7561 6765 732f 746f 702f 616b  languages/top/ak
+000004d0: 616e 7a31 2f6b 6c69 6229 5d28 6874 7470  anz1/klib)](http
+000004e0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+000004f0: 6a65 6374 2f6b 6c69 622f 290a 5b21 5b4c  ject/klib/).[![L
+00000500: 6173 7420 436f 6d6d 6974 5d28 6874 7470  ast Commit](http
+00000510: 733a 2f2f 6261 6467 656e 2e6e 6574 2f67  s://badgen.net/g
+00000520: 6974 6875 622f 6c61 7374 2d63 6f6d 6d69  ithub/last-commi
+00000530: 742f 616b 616e 7a31 2f6b 6c69 622f 6d61  t/akanz1/klib/ma
+00000540: 696e 295d 2868 7474 7073 3a2f 2f67 6974  in)](https://git
+00000550: 6875 622e 636f 6d2f 616b 616e 7a31 2f6b  hub.com/akanz1/k
+00000560: 6c69 622f 636f 6d6d 6974 732f 6d61 696e  lib/commits/main
+00000570: 290a 5b21 5b51 7561 6c69 7479 2047 6174  ).[![Quality Gat
+00000580: 6520 5374 6174 7573 5d28 6874 7470 733a  e Status](https:
+00000590: 2f2f 736f 6e61 7263 6c6f 7564 2e69 6f2f  //sonarcloud.io/
+000005a0: 6170 692f 7072 6f6a 6563 745f 6261 6467  api/project_badg
+000005b0: 6573 2f6d 6561 7375 7265 3f70 726f 6a65  es/measure?proje
+000005c0: 6374 3d61 6b61 6e7a 315f 6b6c 6962 266d  ct=akanz1_klib&m
+000005d0: 6574 7269 633d 616c 6572 745f 7374 6174  etric=alert_stat
+000005e0: 7573 295d 2868 7474 7073 3a2f 2f73 6f6e  us)](https://son
+000005f0: 6172 636c 6f75 642e 696f 2f64 6173 6862  arcloud.io/dashb
+00000600: 6f61 7264 3f69 643d 616b 616e 7a31 5f6b  oard?id=akanz1_k
+00000610: 6c69 6229 0a5b 215b 5363 7275 7469 6e69  lib).[![Scrutini
+00000620: 7a65 725d 2868 7474 7073 3a2f 2f73 6372  zer](https://scr
+00000630: 7574 696e 697a 6572 2d63 692e 636f 6d2f  utinizer-ci.com/
+00000640: 672f 616b 616e 7a31 2f6b 6c69 622f 6261  g/akanz1/klib/ba
+00000650: 6467 6573 2f71 7561 6c69 7479 2d73 636f  dges/quality-sco
+00000660: 7265 2e70 6e67 3f62 3d6d 6169 6e29 5d28  re.png?b=main)](
+00000670: 6874 7470 733a 2f2f 7363 7275 7469 6e69  https://scrutini
+00000680: 7a65 722d 6369 2e63 6f6d 2f67 2f61 6b61  zer-ci.com/g/aka
+00000690: 6e7a 312f 6b6c 6962 2f29 0a5b 215b 636f  nz1/klib/).[![co
+000006a0: 6465 636f 765d 2868 7474 7073 3a2f 2f63  decov](https://c
+000006b0: 6f64 6563 6f76 2e69 6f2f 6768 2f61 6b61  odecov.io/gh/aka
+000006c0: 6e7a 312f 6b6c 6962 2f62 7261 6e63 682f  nz1/klib/branch/
+000006d0: 6d61 696e 2f67 7261 7068 2f62 6164 6765  main/graph/badge
+000006e0: 2e73 7667 295d 2868 7474 7073 3a2f 2f63  .svg)](https://c
+000006f0: 6f64 6563 6f76 2e69 6f2f 6768 2f61 6b61  odecov.io/gh/aka
+00000700: 6e7a 312f 6b6c 6962 290a 0a2a 2a6b 6c69  nz1/klib)..**kli
+00000710: 622a 2a20 6973 2061 2050 7974 686f 6e20  b** is a Python 
+00000720: 6c69 6272 6172 7920 666f 7220 696d 706f  library for impo
+00000730: 7274 696e 672c 2063 6c65 616e 696e 672c  rting, cleaning,
+00000740: 2061 6e61 6c79 7a69 6e67 2061 6e64 2070   analyzing and p
+00000750: 7265 7072 6f63 6573 7369 6e67 2064 6174  reprocessing dat
+00000760: 612e 2045 7870 6c61 6e61 7469 6f6e 7320  a. Explanations 
+00000770: 6f6e 206b 6579 2066 756e 6374 696f 6e61  on key functiona
+00000780: 6c69 7469 6573 2063 616e 2062 6520 666f  lities can be fo
+00000790: 756e 6420 6f6e 205b 4d65 6469 756d 202f  und on [Medium /
+000007a0: 2054 6f77 6172 6473 4461 7461 5363 6965   TowardsDataScie
+000007b0: 6e63 655d 2868 7474 7073 3a2f 2f6d 6564  nce](https://med
+000007c0: 6975 6d2e 636f 6d2f 4061 6b61 6e7a 2920  ium.com/@akanz) 
+000007d0: 616e 6420 696e 2074 6865 205b 6578 616d  and in the [exam
+000007e0: 706c 6573 5d28 6578 616d 706c 6573 2920  ples](examples) 
+000007f0: 7365 6374 696f 6e2e 2041 6464 6974 696f  section. Additio
+00000800: 6e61 6c6c 792c 2074 6865 7265 2061 7265  nally, there are
+00000810: 2067 7265 6174 2069 6e74 726f 6475 6374   great introduct
+00000820: 696f 6e73 2061 6e64 206f 7665 7276 6965  ions and overvie
+00000830: 7773 206f 6620 7468 6520 6675 6e63 7469  ws of the functi
+00000840: 6f6e 616c 6974 7920 6f6e 205b 5079 7468  onality on [Pyth
+00000850: 6f6e 4279 7465 735d 2868 7474 7073 3a2f  onBytes](https:/
+00000860: 2f70 7974 686f 6e62 7974 6573 2e66 6d2f  /pythonbytes.fm/
+00000870: 6570 6973 6f64 6573 2f73 686f 772f 3234  episodes/show/24
+00000880: 302f 7468 6973 2d69 732d 6769 7468 7562  0/this-is-github
+00000890: 2d79 6f75 722d 7069 6c6f 742d 7370 6561  -your-pilot-spea
+000008a0: 6b69 6e67 2920 6f72 206f 6e20 5b59 6f75  king) or on [You
+000008b0: 5475 6265 2028 4461 7461 2050 726f 6665  Tube (Data Profe
+000008c0: 7373 6f72 295d 2868 7474 7073 3a2f 2f77  ssor)](https://w
+000008d0: 7777 2e79 6f75 7475 6265 2e63 6f6d 2f77  ww.youtube.com/w
+000008e0: 6174 6368 3f76 3d55 526a 4a56 4565 5a78  atch?v=URjJVEeZx
+000008f0: 7855 292e 0a0a 2323 2049 6e73 7461 6c6c  xU)...## Install
+00000900: 6174 696f 6e0a 0a55 7365 2074 6865 2070  ation..Use the p
+00000910: 6163 6b61 6765 206d 616e 6167 6572 205b  ackage manager [
+00000920: 7069 705d 2868 7474 7073 3a2f 2f70 6970  pip](https://pip
+00000930: 2e70 7970 612e 696f 2f65 6e2f 7374 6162  .pypa.io/en/stab
+00000940: 6c65 2f29 2074 6f20 696e 7374 616c 6c20  le/) to install 
+00000950: 6b6c 6962 2e0a 0a5b 215b 5079 5049 2056  klib...[![PyPI V
+00000960: 6572 7369 6f6e 5d28 6874 7470 733a 2f2f  ersion](https://
+00000970: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000980: 7970 692f 762f 6b6c 6962 295d 2868 7474  ypi/v/klib)](htt
+00000990: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
+000009a0: 6f6a 6563 742f 6b6c 6962 2f29 0a5b 215b  oject/klib/).[![
+000009b0: 446f 776e 6c6f 6164 735d 2868 7474 7073  Downloads](https
+000009c0: 3a2f 2f70 6570 792e 7465 6368 2f62 6164  ://pepy.tech/bad
+000009d0: 6765 2f6b 6c69 622f 6d6f 6e74 6829 5d28  ge/klib/month)](
+000009e0: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+000009f0: 2f70 726f 6a65 6374 2f6b 6c69 622f 290a  /project/klib/).
+00000a00: 0a60 6060 6261 7368 0a70 6970 2069 6e73  .```bash.pip ins
+00000a10: 7461 6c6c 202d 5520 6b6c 6962 0a60 6060  tall -U klib.```
+00000a20: 0a0a 416c 7465 726e 6174 6976 656c 792c  ..Alternatively,
+00000a30: 2074 6f20 696e 7374 616c 6c20 7468 6973   to install this
+00000a40: 2070 6163 6b61 6765 2077 6974 6820 636f   package with co
+00000a50: 6e64 6120 7275 6e3a 0a0a 5b21 5b43 6f6e  nda run:..[![Con
+00000a60: 6461 2056 6572 7369 6f6e 5d28 6874 7470  da Version](http
+00000a70: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000a80: 696f 2f63 6f6e 6461 2f76 6e2f 636f 6e64  io/conda/vn/cond
+00000a90: 612d 666f 7267 652f 6b6c 6962 295d 2868  a-forge/klib)](h
+00000aa0: 7474 7073 3a2f 2f61 6e61 636f 6e64 612e  ttps://anaconda.
+00000ab0: 6f72 672f 636f 6e64 612d 666f 7267 652f  org/conda-forge/
+00000ac0: 6b6c 6962 290a 5b21 5b43 6f6e 6461 2044  klib).[![Conda D
+00000ad0: 6f77 6e6c 6f61 6473 5d28 6874 7470 733a  ownloads](https:
+00000ae0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000af0: 2f63 6f6e 6461 2f64 6e2f 636f 6e64 612d  /conda/dn/conda-
+00000b00: 666f 7267 652f 6b6c 6962 2e73 7667 295d  forge/klib.svg)]
+00000b10: 2868 7474 7073 3a2f 2f61 6e61 636f 6e64  (https://anacond
+00000b20: 612e 6f72 672f 636f 6e64 612d 666f 7267  a.org/conda-forg
+00000b30: 652f 6b6c 6962 290a 0a60 6060 6261 7368  e/klib)..```bash
+00000b40: 0a63 6f6e 6461 2069 6e73 7461 6c6c 202d  .conda install -
+00000b50: 6320 636f 6e64 612d 666f 7267 6520 6b6c  c conda-forge kl
+00000b60: 6962 0a60 6060 0a0a 2323 2055 7361 6765  ib.```..## Usage
+00000b70: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
+00000b80: 7274 206b 6c69 620a 696d 706f 7274 2070  rt klib.import p
+00000b90: 616e 6461 7320 6173 2070 640a 0a64 6620  andas as pd..df 
+00000ba0: 3d20 7064 2e44 6174 6146 7261 6d65 2864  = pd.DataFrame(d
+00000bb0: 6174 6129 0a0a 2320 6b6c 6962 2e64 6573  ata)..# klib.des
+00000bc0: 6372 6962 6520 2d20 6675 6e63 7469 6f6e  cribe - function
+00000bd0: 7320 666f 7220 7669 7375 616c 697a 696e  s for visualizin
+00000be0: 6720 6461 7461 7365 7473 0a2d 206b 6c69  g datasets.- kli
+00000bf0: 622e 6361 745f 706c 6f74 2864 6629 2023  b.cat_plot(df) #
+00000c00: 2072 6574 7572 6e73 2061 2076 6973 7561   returns a visua
+00000c10: 6c69 7a61 7469 6f6e 206f 6620 7468 6520  lization of the 
+00000c20: 6e75 6d62 6572 2061 6e64 2066 7265 7175  number and frequ
+00000c30: 656e 6379 206f 6620 6361 7465 676f 7269  ency of categori
+00000c40: 6361 6c20 6665 6174 7572 6573 0a2d 206b  cal features.- k
+00000c50: 6c69 622e 636f 7272 5f6d 6174 2864 6629  lib.corr_mat(df)
+00000c60: 2023 2072 6574 7572 6e73 2061 2063 6f6c   # returns a col
+00000c70: 6f72 2d65 6e63 6f64 6564 2063 6f72 7265  or-encoded corre
+00000c80: 6c61 7469 6f6e 206d 6174 7269 780a 2d20  lation matrix.- 
+00000c90: 6b6c 6962 2e63 6f72 725f 706c 6f74 2864  klib.corr_plot(d
+00000ca0: 6629 2023 2072 6574 7572 6e73 2061 2063  f) # returns a c
+00000cb0: 6f6c 6f72 2d65 6e63 6f64 6564 2068 6561  olor-encoded hea
+00000cc0: 746d 6170 2c20 6964 6561 6c20 666f 7220  tmap, ideal for 
+00000cd0: 636f 7272 656c 6174 696f 6e73 0a2d 206b  correlations.- k
+00000ce0: 6c69 622e 6469 7374 5f70 6c6f 7428 6466  lib.dist_plot(df
+00000cf0: 2920 2320 7265 7475 726e 7320 6120 6469  ) # returns a di
+00000d00: 7374 7269 6275 7469 6f6e 2070 6c6f 7420  stribution plot 
+00000d10: 666f 7220 6576 6572 7920 6e75 6d65 7269  for every numeri
+00000d20: 6320 6665 6174 7572 650a 2d20 6b6c 6962  c feature.- klib
+00000d30: 2e6d 6973 7369 6e67 7661 6c5f 706c 6f74  .missingval_plot
+00000d40: 2864 6629 2023 2072 6574 7572 6e73 2061  (df) # returns a
+00000d50: 2066 6967 7572 6520 636f 6e74 6169 6e69   figure containi
+00000d60: 6e67 2069 6e66 6f72 6d61 7469 6f6e 2061  ng information a
+00000d70: 626f 7574 206d 6973 7369 6e67 2076 616c  bout missing val
+00000d80: 7565 730a 0a23 206b 6c69 622e 636c 6561  ues..# klib.clea
+00000d90: 6e20 2d20 6675 6e63 7469 6f6e 7320 666f  n - functions fo
+00000da0: 7220 636c 6561 6e69 6e67 2064 6174 6173  r cleaning datas
+00000db0: 6574 730a 2d20 6b6c 6962 2e64 6174 615f  ets.- klib.data_
+00000dc0: 636c 6561 6e69 6e67 2864 6629 2023 2070  cleaning(df) # p
+00000dd0: 6572 666f 726d 7320 6461 7461 636c 6561  erforms dataclea
+00000de0: 6e69 6e67 2028 6472 6f70 2064 7570 6c69  ning (drop dupli
+00000df0: 6361 7465 7320 2620 656d 7074 7920 726f  cates & empty ro
+00000e00: 7773 2f63 6f6c 732c 2061 646a 7573 7420  ws/cols, adjust 
+00000e10: 6474 7970 6573 2c2e 2e2e 290a 2d20 6b6c  dtypes,...).- kl
+00000e20: 6962 2e63 6c65 616e 5f63 6f6c 756d 6e5f  ib.clean_column_
+00000e30: 6e61 6d65 7328 6466 2920 2320 636c 6561  names(df) # clea
+00000e40: 6e73 2061 6e64 2073 7461 6e64 6172 6469  ns and standardi
+00000e50: 7a65 7320 636f 6c75 6d6e 206e 616d 6573  zes column names
+00000e60: 2c20 616c 736f 2063 616c 6c65 6420 696e  , also called in
+00000e70: 7369 6465 2064 6174 615f 636c 6561 6e69  side data_cleani
+00000e80: 6e67 2829 0a2d 206b 6c69 622e 636f 6e76  ng().- klib.conv
+00000e90: 6572 745f 6461 7461 7479 7065 7328 6466  ert_datatypes(df
+00000ea0: 2920 2320 636f 6e76 6572 7473 2065 7869  ) # converts exi
+00000eb0: 7374 696e 6720 746f 206d 6f72 6520 6566  sting to more ef
+00000ec0: 6669 6369 656e 7420 6474 7970 6573 2c20  ficient dtypes, 
+00000ed0: 616c 736f 2063 616c 6c65 6420 696e 7369  also called insi
+00000ee0: 6465 2064 6174 615f 636c 6561 6e69 6e67  de data_cleaning
+00000ef0: 2829 0a2d 206b 6c69 622e 6472 6f70 5f6d  ().- klib.drop_m
+00000f00: 6973 7369 6e67 2864 6629 2023 2064 726f  issing(df) # dro
+00000f10: 7073 206d 6973 7369 6e67 2076 616c 7565  ps missing value
+00000f20: 732c 2061 6c73 6f20 6361 6c6c 6564 2069  s, also called i
+00000f30: 6e20 6461 7461 5f63 6c65 616e 696e 6728  n data_cleaning(
+00000f40: 290a 2d20 6b6c 6962 2e6d 765f 636f 6c5f  ).- klib.mv_col_
+00000f50: 6861 6e64 6c69 6e67 2864 6629 2023 2064  handling(df) # d
+00000f60: 726f 7073 2066 6561 7475 7265 7320 7769  rops features wi
+00000f70: 7468 2068 6967 6820 7261 7469 6f20 6f66  th high ratio of
+00000f80: 206d 6973 7369 6e67 2076 616c 7320 6261   missing vals ba
+00000f90: 7365 6420 6f6e 2069 6e66 6f72 6d61 7469  sed on informati
+00000fa0: 6f6e 616c 2063 6f6e 7465 6e74 0a2d 206b  onal content.- k
+00000fb0: 6c69 622e 706f 6f6c 5f64 7570 6c69 6361  lib.pool_duplica
+00000fc0: 7465 5f73 7562 7365 7473 2864 6629 2023  te_subsets(df) #
+00000fd0: 2070 6f6f 6c73 2073 7562 7365 7420 6f66   pools subset of
+00000fe0: 2063 6f6c 7320 6261 7365 6420 6f6e 2064   cols based on d
+00000ff0: 7570 6c69 6361 7465 7320 7769 7468 206d  uplicates with m
+00001000: 696e 2e20 6c6f 7373 206f 6620 696e 666f  in. loss of info
+00001010: 726d 6174 696f 6e0a 6060 600a 0a23 2320  rmation.```..## 
+00001020: 4578 616d 706c 6573 0a0a 4669 6e64 2061  Examples..Find a
+00001030: 6c6c 2061 7661 696c 6162 6c65 2065 7861  ll available exa
+00001040: 6d70 6c65 7320 6173 2077 656c 6c20 6173  mples as well as
+00001050: 2061 7070 6c69 6361 7469 6f6e 7320 6f66   applications of
+00001060: 2074 6865 2066 756e 6374 696f 6e73 2069   the functions i
+00001070: 6e20 2a2a 6b6c 6962 2e63 6c65 616e 2829  n **klib.clean()
+00001080: 2a2a 2077 6974 6820 6465 7461 696c 6564  ** with detailed
+00001090: 2064 6573 6372 6970 7469 6f6e 7320 3c61   descriptions <a
+000010a0: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+000010b0: 6974 6875 622e 636f 6d2f 616b 616e 7a31  ithub.com/akanz1
+000010c0: 2f6b 6c69 622f 7472 6565 2f6d 6169 6e2f  /klib/tree/main/
+000010d0: 6578 616d 706c 6573 223e 6865 7265 3c2f  examples">here</
+000010e0: 613e 2e0a 0a60 6060 7079 7468 6f6e 0a6b  a>...```python.k
+000010f0: 6c69 622e 6d69 7373 696e 6776 616c 5f70  lib.missingval_p
+00001100: 6c6f 7428 6466 2920 2320 6465 6661 756c  lot(df) # defaul
+00001110: 7420 7265 7072 6573 656e 7461 7469 6f6e  t representation
+00001120: 206f 6620 6d69 7373 696e 6720 7661 6c75   of missing valu
+00001130: 6573 2069 6e20 6120 4461 7461 4672 616d  es in a DataFram
+00001140: 652c 2070 6c65 6e74 7920 6f66 2073 6574  e, plenty of set
+00001150: 7469 6e67 7320 6172 6520 6176 6169 6c61  tings are availa
+00001160: 626c 650a 6060 600a 0a3c 7020 616c 6967  ble.```..<p alig
+00001170: 6e3d 2263 656e 7465 7222 3e3c 696d 6720  n="center"><img 
+00001180: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
+00001190: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+000011a0: 6e74 2e63 6f6d 2f61 6b61 6e7a 312f 6b6c  nt.com/akanz1/kl
+000011b0: 6962 2f6d 6169 6e2f 6578 616d 706c 6573  ib/main/examples
+000011c0: 2f69 6d61 6765 732f 6578 616d 706c 655f  /images/example_
+000011d0: 6d76 5f70 6c6f 742e 706e 6722 2061 6c74  mv_plot.png" alt
+000011e0: 3d22 4d69 7373 696e 6776 616c 7565 2050  ="Missingvalue P
+000011f0: 6c6f 7420 4578 616d 706c 6522 2077 6964  lot Example" wid
+00001200: 7468 3d22 3130 3030 2220 6865 6967 6874  th="1000" height
+00001210: 3d22 3130 3931 223e 3c2f 703e 0a0a 6060  ="1091"></p>..``
+00001220: 6070 7974 686f 6e0a 6b6c 6962 2e63 6f72  `python.klib.cor
+00001230: 725f 706c 6f74 2864 662c 2073 706c 6974  r_plot(df, split
+00001240: 3d27 706f 7327 2920 2320 6469 7370 6c61  ='pos') # displa
+00001250: 7969 6e67 206f 6e6c 7920 706f 7369 7469  ying only positi
+00001260: 7665 2063 6f72 7265 6c61 7469 6f6e 732c  ve correlations,
+00001270: 206f 7468 6572 2073 6574 7469 6e67 7320   other settings 
+00001280: 696e 636c 7564 6520 7468 7265 7368 6f6c  include threshol
+00001290: 642c 2063 6d61 702e 2e2e 0a6b 6c69 622e  d, cmap....klib.
+000012a0: 636f 7272 5f70 6c6f 7428 6466 2c20 7370  corr_plot(df, sp
+000012b0: 6c69 743d 276e 6567 2729 2023 2064 6973  lit='neg') # dis
+000012c0: 706c 6179 696e 6720 6f6e 6c79 206e 6567  playing only neg
+000012d0: 6174 6976 6520 636f 7272 656c 6174 696f  ative correlatio
+000012e0: 6e73 0a60 6060 0a0a 3c70 2061 6c69 676e  ns.```..<p align
+000012f0: 3d22 6365 6e74 6572 223e 3c69 6d67 2073  ="center"><img s
+00001300: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+00001310: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00001320: 742e 636f 6d2f 616b 616e 7a31 2f6b 6c69  t.com/akanz1/kli
+00001330: 622f 6d61 696e 2f65 7861 6d70 6c65 732f  b/main/examples/
+00001340: 696d 6167 6573 2f65 7861 6d70 6c65 5f63  images/example_c
+00001350: 6f72 725f 706c 6f74 2e70 6e67 2220 616c  orr_plot.png" al
+00001360: 743d 2243 6f72 7220 506c 6f74 2045 7861  t="Corr Plot Exa
+00001370: 6d70 6c65 2220 7769 6474 683d 2237 3230  mple" width="720
+00001380: 2220 6865 6967 6874 3d22 3333 3822 3e3c  " height="338"><
+00001390: 2f70 3e0a 0a60 6060 7079 7468 6f6e 0a6b  /p>..```python.k
+000013a0: 6c69 622e 636f 7272 5f70 6c6f 7428 6466  lib.corr_plot(df
+000013b0: 2c20 7461 7267 6574 3d27 7769 6e65 2729  , target='wine')
+000013c0: 2023 2064 6566 6175 6c74 2072 6570 7265   # default repre
+000013d0: 7365 6e74 6174 696f 6e20 6f66 2063 6f72  sentation of cor
+000013e0: 7265 6c61 7469 6f6e 7320 7769 7468 2074  relations with t
+000013f0: 6865 2066 6561 7475 7265 2063 6f6c 756d  he feature colum
+00001400: 6e0a 6060 600a 0a3c 7020 616c 6967 6e3d  n.```..<p align=
+00001410: 2263 656e 7465 7222 3e3c 696d 6720 7372  "center"><img sr
+00001420: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00001430: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00001440: 2e63 6f6d 2f61 6b61 6e7a 312f 6b6c 6962  .com/akanz1/klib
+00001450: 2f6d 6169 6e2f 6578 616d 706c 6573 2f69  /main/examples/i
+00001460: 6d61 6765 732f 6578 616d 706c 655f 7461  mages/example_ta
+00001470: 7267 6574 5f63 6f72 725f 706c 6f74 2e70  rget_corr_plot.p
+00001480: 6e67 2220 616c 743d 2254 6172 6765 7420  ng" alt="Target 
+00001490: 436f 7272 2050 6c6f 7420 4578 616d 706c  Corr Plot Exampl
+000014a0: 6522 2077 6964 7468 3d22 3732 3022 2068  e" width="720" h
+000014b0: 6569 6768 743d 2236 3030 223e 3c2f 703e  eight="600"></p>
+000014c0: 0a0a 6060 6070 7974 686f 6e0a 6b6c 6962  ..```python.klib
+000014d0: 2e63 6f72 725f 696e 7465 7261 6374 6976  .corr_interactiv
+000014e0: 655f 706c 6f74 2864 662c 2073 706c 6974  e_plot(df, split
+000014f0: 3d22 6e65 6722 292e 7368 6f77 2829 0a0a  ="neg").show()..
+00001500: 2320 5468 6520 696e 7465 7261 6374 6976  # The interactiv
+00001510: 6520 706c 6f74 2068 6173 2074 6865 2073  e plot has the s
+00001520: 616d 6520 7061 7261 6d65 7465 7273 2061  ame parameters a
+00001530: 7320 7468 6520 636f 7272 5f70 6c6f 742c  s the corr_plot,
+00001540: 2062 7574 2077 6974 6820 6164 6469 7469   but with additi
+00001550: 6f6e 616c 2050 6c6f 746c 7920 6865 6174  onal Plotly heat
+00001560: 6d61 7020 6772 6170 6820 6f62 6a65 6374  map graph object
+00001570: 206b 7761 7267 732e 0a6b 6c69 622e 636f   kwargs..klib.co
+00001580: 7272 5f69 6e74 6572 6163 7469 7665 5f70  rr_interactive_p
+00001590: 6c6f 7428 6466 2c20 7370 6c69 743d 226e  lot(df, split="n
+000015a0: 6567 222c 207a 6d61 783d 3029 0a60 6060  eg", zmax=0).```
+000015b0: 0a0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
+000015c0: 6572 223e 3c69 6d67 2073 7263 3d22 6874  er"><img src="ht
+000015d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000015e0: 2f61 6b61 6e7a 312f 6b6c 6962 2f61 7373  /akanz1/klib/ass
+000015f0: 6574 732f 3132 3435 3133 3932 322f 3237  ets/124513922/27
+00001600: 6237 3965 6365 2d64 6332 322d 3431 3063  b79ece-dc22-410c
+00001610: 2d39 3831 362d 6663 6334 6366 6339 3765  -9816-fcc4cfc97e
+00001620: 6463 2220 2061 6c74 3d22 496e 7465 7261  dc"  alt="Intera
+00001630: 6374 6976 6520 436f 7272 2050 6c6f 7420  ctive Corr Plot 
+00001640: 5369 6d70 6c65 2045 7861 6d70 6c65 2220  Simple Example" 
+00001650: 7769 6474 683d 2237 3230 2220 6865 6967  width="720" heig
+00001660: 6874 3d22 3630 3022 3e3c 2f70 3e0a 0a3c  ht="600"></p>..<
+00001670: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+00001680: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+00001690: 3a2f 2f67 6974 6875 622e 636f 6d2f 616b  ://github.com/ak
+000016a0: 616e 7a31 2f6b 6c69 622f 6173 7365 7473  anz1/klib/assets
+000016b0: 2f31 3234 3531 3339 3232 2f64 3938 3664  /124513922/d986d
+000016c0: 6336 632d 3834 6463 2d34 3639 332d 6232  c6c-84dc-4693-b2
+000016d0: 3736 2d36 6234 6466 3730 3233 6530 6622  76-6b4df7023e0f"
+000016e0: 2061 6c74 3d22 496e 7465 7261 6374 6976   alt="Interactiv
+000016f0: 6520 436f 7272 2050 6c6f 7420 7769 7468  e Corr Plot with
+00001700: 207a 6d61 7820 6b77 6172 6720 4578 616d   zmax kwarg Exam
+00001710: 706c 6522 2077 6964 7468 3d22 3732 3022  ple" width="720"
+00001720: 2068 6569 6768 743d 2236 3030 223e 3c2f   height="600"></
+00001730: 703e 0a0a 6060 6070 7974 686f 6e0a 2353  p>..```python.#S
+00001740: 696e 6365 2063 6f72 725f 696e 7465 7261  ince corr_intera
+00001750: 6374 6976 655f 706c 6f74 2072 6574 7572  ctive_plot retur
+00001760: 6e73 2061 2047 7261 7068 204f 626a 6563  ns a Graph Objec
+00001770: 7420 4669 6775 7265 2c20 6974 2073 7570  t Figure, it sup
+00001780: 706f 7274 7320 7468 6520 7570 6461 7465  ports the update
+00001790: 5f6c 6179 6f75 7420 6368 6169 6e20 6d65  _layout chain me
+000017a0: 7468 6f64 2e0a 6b6c 6962 2e63 6f72 725f  thod..klib.corr_
+000017b0: 696e 7465 7261 6374 6976 655f 706c 6f74  interactive_plot
+000017c0: 2877 696e 652c 2073 706c 6974 3d22 6e65  (wine, split="ne
+000017d0: 6722 292e 7570 6461 7465 5f6c 6179 6f75  g").update_layou
+000017e0: 7428 7465 6d70 6c61 7465 3d22 7369 6d70  t(template="simp
+000017f0: 6c65 5f77 6869 7465 2229 0a60 6060 0a0a  le_white").```..
+00001800: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00001810: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00001820: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
+00001830: 6b61 6e7a 312f 6b6c 6962 2f61 7373 6574  kanz1/klib/asset
+00001840: 732f 3132 3435 3133 3932 322f 6662 3761  s/124513922/fb7a
+00001850: 6331 3032 2d36 6461 662d 3465 3330 2d61  c102-6daf-4e30-a
+00001860: 3234 632d 6462 3136 3863 3763 6634 3263  24c-db168c7cf42c
+00001870: 2220 616c 743d 2249 6e74 6572 6163 7469  " alt="Interacti
+00001880: 7665 2043 6f72 7220 506c 6f74 2043 6861  ve Corr Plot Cha
+00001890: 696e 6564 2045 7861 6d70 6c65 2220 7769  ined Example" wi
+000018a0: 6474 683d 2237 3230 2220 6865 6967 6874  dth="720" height
+000018b0: 3d22 3630 3022 3e3c 2f70 3e0a 0a60 6060  ="600"></p>..```
+000018c0: 7079 7468 6f6e 0a6b 6c69 622e 6469 7374  python.klib.dist
+000018d0: 5f70 6c6f 7428 6466 2920 2320 6465 6661  _plot(df) # defa
+000018e0: 756c 7420 7265 7072 6573 656e 7461 7469  ult representati
+000018f0: 6f6e 206f 6620 6120 6469 7374 7269 6275  on of a distribu
+00001900: 7469 6f6e 2070 6c6f 742c 206f 7468 6572  tion plot, other
+00001910: 2073 6574 7469 6e67 7320 696e 636c 7564   settings includ
+00001920: 6520 6669 6c6c 5f72 616e 6765 2c20 6869  e fill_range, hi
+00001930: 7374 6f67 7261 6d2c 202e 2e2e 0a60 6060  stogram, ....```
+00001940: 0a0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
+00001950: 6572 223e 3c69 6d67 2073 7263 3d22 6874  er"><img src="ht
+00001960: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00001970: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00001980: 616b 616e 7a31 2f6b 6c69 622f 6d61 696e  akanz1/klib/main
+00001990: 2f65 7861 6d70 6c65 732f 696d 6167 6573  /examples/images
+000019a0: 2f65 7861 6d70 6c65 5f64 6973 745f 706c  /example_dist_pl
+000019b0: 6f74 2e70 6e67 2220 616c 743d 2244 6973  ot.png" alt="Dis
+000019c0: 7420 506c 6f74 2045 7861 6d70 6c65 2220  t Plot Example" 
+000019d0: 7769 6474 683d 2239 3130 2220 6865 6967  width="910" heig
+000019e0: 6874 3d22 3133 3022 3e3c 2f70 3e0a 0a60  ht="130"></p>..`
+000019f0: 6060 7079 7468 6f6e 0a6b 6c69 622e 6361  ``python.klib.ca
+00001a00: 745f 706c 6f74 2864 6174 612c 2074 6f70  t_plot(data, top
+00001a10: 3d34 2c20 626f 7474 6f6d 3d34 2920 2320  =4, bottom=4) # 
+00001a20: 7265 7072 6573 656e 7461 7469 6f6e 206f  representation o
+00001a30: 6620 7468 6520 3420 6d6f 7374 2026 206c  f the 4 most & l
+00001a40: 6561 7374 2063 6f6d 6d6f 6e20 7661 6c75  east common valu
+00001a50: 6573 2069 6e20 6561 6368 2063 6174 6567  es in each categ
+00001a60: 6f72 6963 616c 2063 6f6c 756d 6e0a 6060  orical column.``
+00001a70: 600a 0a3c 7020 616c 6967 6e3d 2263 656e  `..<p align="cen
+00001a80: 7465 7222 3e3c 696d 6720 7372 633d 2268  ter"><img src="h
+00001a90: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00001aa0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00001ab0: 2f61 6b61 6e7a 312f 6b6c 6962 2f6d 6169  /akanz1/klib/mai
+00001ac0: 6e2f 6578 616d 706c 6573 2f69 6d61 6765  n/examples/image
+00001ad0: 732f 6578 616d 706c 655f 6361 745f 706c  s/example_cat_pl
+00001ae0: 6f74 2e70 6e67 2220 616c 743d 2243 6174  ot.png" alt="Cat
+00001af0: 2050 6c6f 7420 4578 616d 706c 6522 2077   Plot Example" w
+00001b00: 6964 7468 3d22 3130 3030 2220 6865 6967  idth="1000" heig
+00001b10: 6874 3d22 3130 3030 223e 3c2f 703e 0a0a  ht="1000"></p>..
+00001b20: 4675 7274 6865 7220 6578 616d 706c 6573  Further examples
+00001b30: 2c20 6173 2077 656c 6c20 6173 2061 7070  , as well as app
+00001b40: 6c69 6361 7469 6f6e 7320 6f66 2074 6865  lications of the
+00001b50: 2066 756e 6374 696f 6e73 2069 6e20 2a2a   functions in **
+00001b60: 6b6c 6962 2e63 6c65 616e 2829 2a2a 2063  klib.clean()** c
+00001b70: 616e 2062 6520 666f 756e 6420 3c61 2068  an be found <a h
+00001b80: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00001b90: 6875 622e 636f 6d2f 616b 616e 7a31 2f6b  hub.com/akanz1/k
+00001ba0: 6c69 622f 7472 6565 2f6d 6169 6e2f 6578  lib/tree/main/ex
+00001bb0: 616d 706c 6573 2364 6174 612d 636c 6561  amples#data-clea
+00001bc0: 6e69 6e67 2d61 6e64 2d61 6767 7265 7461  ning-and-aggreta
+00001bd0: 7469 6f6e 223e 6865 7265 3c2f 613e 2e0a  tion">here</a>..
+00001be0: 0a23 2320 436f 6e74 7269 6275 7469 6e67  .## Contributing
+00001bf0: 0a0a 5b21 5b4f 7065 6e20 696e 2056 6973  ..[![Open in Vis
+00001c00: 7561 6c20 5374 7564 696f 2043 6f64 655d  ual Studio Code]
+00001c10: 2868 7474 7073 3a2f 2f6f 7065 6e2e 7673  (https://open.vs
+00001c20: 636f 6465 2e64 6576 2f62 6164 6765 732f  code.dev/badges/
+00001c30: 6f70 656e 2d69 6e2d 7673 636f 6465 2e73  open-in-vscode.s
+00001c40: 7667 295d 2868 7474 7073 3a2f 2f6f 7065  vg)](https://ope
+00001c50: 6e2e 7673 636f 6465 2e64 6576 2f61 6b61  n.vscode.dev/aka
+00001c60: 6e7a 312f 6b6c 6962 290a 0a50 756c 6c20  nz1/klib)..Pull 
+00001c70: 7265 7175 6573 7473 2061 6e64 2069 6465  requests and ide
+00001c80: 6173 2c20 6573 7065 6369 616c 6c79 2066  as, especially f
+00001c90: 6f72 2066 7572 7468 6572 2066 756e 6374  or further funct
+00001ca0: 696f 6e73 2061 7265 2077 656c 636f 6d65  ions are welcome
+00001cb0: 2e20 466f 7220 6d61 6a6f 7220 6368 616e  . For major chan
+00001cc0: 6765 7320 6f72 2066 6565 6462 6163 6b2c  ges or feedback,
+00001cd0: 2070 6c65 6173 6520 6f70 656e 2061 6e20   please open an 
+00001ce0: 6973 7375 6520 6669 7273 7420 746f 2064  issue first to d
+00001cf0: 6973 6375 7373 2077 6861 7420 796f 7520  iscuss what you 
+00001d00: 776f 756c 6420 6c69 6b65 2074 6f20 6368  would like to ch
+00001d10: 616e 6765 2e0a 0a23 2320 4c69 6365 6e73  ange...## Licens
+00001d20: 650a 0a5b 4d49 545d 2868 7474 7073 3a2f  e..[MIT](https:/
+00001d30: 2f63 686f 6f73 6561 6c69 6365 6e73 652e  /choosealicense.
+00001d40: 636f 6d2f 6c69 6365 6e73 6573 2f6d 6974  com/licenses/mit
+00001d50: 2f29 0a0a                                /)..
```

