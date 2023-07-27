# Comparing `tmp/edvart-1.1.0.tar.gz` & `tmp/edvart-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edvart-1.1.0.tar", max compression
+gzip compressed data, was "edvart-1.1.1.tar", max compression
```

## Comparing `edvart-1.1.0.tar` & `edvart-1.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1064 2023-07-20 14:02:58.341205 edvart-1.1.0/LICENSE
--rw-r--r--   0        0        0      459 2023-07-20 14:02:58.531205 edvart-1.1.0/edvart/__init__.py
--rw-r--r--   0        0        0     4513 2023-07-27 14:10:53.416242 edvart-1.1.0/edvart/data_types.py
--rw-r--r--   0        0        0     1129 2023-07-20 14:02:58.344539 edvart-1.1.0/edvart/decorators.py
--rw-r--r--   0        0        0     2732 2023-07-20 14:02:58.421205 edvart-1.1.0/edvart/example_datasets.py
--rw-r--r--   0        0        0     1127 2023-07-20 14:02:58.344539 edvart-1.1.0/edvart/export_utils.py
--rw-r--r--   0        0        0     4759 2023-07-20 14:02:58.344539 edvart-1.1.0/edvart/pandas_formatting.py
--rw-r--r--   0        0        0     6127 2023-07-20 14:02:58.344539 edvart-1.1.0/edvart/plots.py
--rwxr-xr-x   0        0        0    40227 2023-07-27 14:10:53.416242 edvart-1.1.0/edvart/report.py
--rw-r--r--   0        0        0       42 2023-07-20 14:02:58.347872 edvart-1.1.0/edvart/report_sections/__init__.py
--rw-r--r--   0        0        0    40075 2023-07-20 14:02:58.347872 edvart-1.1.0/edvart/report_sections/bivariate_analysis.py
--rw-r--r--   0        0        0     1823 2023-07-20 14:02:58.347872 edvart-1.1.0/edvart/report_sections/code_string_formatting.py
--rw-r--r--   0        0        0    38313 2023-07-20 14:02:58.347872 edvart-1.1.0/edvart/report_sections/dataset_overview.py
--rw-r--r--   0        0        0    27953 2023-07-20 14:02:58.504538 edvart-1.1.0/edvart/report_sections/group_analysis.py
--rw-r--r--   0        0        0    33687 2023-07-27 14:10:22.816319 edvart-1.1.0/edvart/report_sections/multivariate_analysis.py
--rw-r--r--   0        0        0     6680 2023-07-20 14:02:58.671205 edvart-1.1.0/edvart/report_sections/section_base.py
--rw-r--r--   0        0        0     4380 2023-07-20 14:02:58.347872 edvart-1.1.0/edvart/report_sections/table_of_contents.py
--rw-r--r--   0        0        0      510 2023-07-20 14:02:58.347872 edvart-1.1.0/edvart/report_sections/timeseries_analysis/__init__.py
--rw-r--r--   0        0        0     9011 2023-07-20 14:02:58.347872 edvart-1.1.0/edvart/report_sections/timeseries_analysis/autocorrelation.py
--rw-r--r--   0        0        0    11933 2023-07-20 14:02:58.347872 edvart-1.1.0/edvart/report_sections/timeseries_analysis/boxplots_over_time.py
--rw-r--r--   0        0        0     6742 2023-07-20 14:02:58.347872 edvart-1.1.0/edvart/report_sections/timeseries_analysis/fourier_transform.py
--rw-r--r--   0        0        0     8409 2023-07-20 14:02:58.347872 edvart-1.1.0/edvart/report_sections/timeseries_analysis/rolling_statistics.py
--rw-r--r--   0        0        0     6956 2023-07-20 14:02:58.351205 edvart-1.1.0/edvart/report_sections/timeseries_analysis/seasonal_decomposition.py
--rw-r--r--   0        0        0     8568 2023-07-20 14:02:58.351205 edvart-1.1.0/edvart/report_sections/timeseries_analysis/short_time_ft.py
--rw-r--r--   0        0        0     6878 2023-07-20 14:02:58.351205 edvart-1.1.0/edvart/report_sections/timeseries_analysis/stationarity_tests.py
--rw-r--r--   0        0        0     8138 2023-07-27 14:10:22.816319 edvart-1.1.0/edvart/report_sections/timeseries_analysis/time_analysis_plot.py
--rw-r--r--   0        0        0    13844 2023-07-20 14:02:58.351205 edvart-1.1.0/edvart/report_sections/timeseries_analysis/timeseries_analysis.py
--rw-r--r--   0        0        0    10060 2023-07-20 14:02:58.351205 edvart-1.1.0/edvart/report_sections/umap.py
--rw-r--r--   0        0        0    17023 2023-07-20 14:02:58.351205 edvart-1.1.0/edvart/report_sections/univariate_analysis.py
--rwxr-xr-x   0        0        0    12528 2023-07-27 14:10:53.416242 edvart-1.1.0/edvart/utils.py
--rw-r--r--   0        0        0  4769813 2023-07-20 14:02:58.377872 edvart-1.1.0/example-datasets/Meteorite_Landings.csv
--rw-r--r--   0        0        0    17732 2023-07-20 14:02:58.377872 edvart-1.1.0/example-datasets/auto.csv
--rw-r--r--   0        0        0    39839 2023-07-20 14:02:58.381205 edvart-1.1.0/example-datasets/global_temp.csv
--rw-r--r--   0        0        0  2295543 2023-07-20 14:02:58.391205 edvart-1.1.0/example-datasets/pollution.csv
--rw-r--r--   0        0        0    60302 2023-07-20 14:02:58.391205 edvart-1.1.0/example-datasets/titanic.csv
--rw-r--r--   0        0        0     1077 2023-07-27 14:11:01.589556 edvart-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1129 1970-01-01 00:00:00.000000 edvart-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-20 14:02:58.341205 edvart-1.1.1/LICENSE
+-rw-r--r--   0        0        0      459 2023-07-20 14:02:58.531205 edvart-1.1.1/edvart/__init__.py
+-rw-r--r--   0        0        0     4513 2023-07-27 14:10:53.416242 edvart-1.1.1/edvart/data_types.py
+-rw-r--r--   0        0        0     1129 2023-07-20 14:02:58.344539 edvart-1.1.1/edvart/decorators.py
+-rw-r--r--   0        0        0     2732 2023-07-20 14:02:58.421205 edvart-1.1.1/edvart/example_datasets.py
+-rw-r--r--   0        0        0     1127 2023-07-20 14:02:58.344539 edvart-1.1.1/edvart/export_utils.py
+-rw-r--r--   0        0        0     4759 2023-07-20 14:02:58.344539 edvart-1.1.1/edvart/pandas_formatting.py
+-rw-r--r--   0        0        0     6127 2023-07-20 14:02:58.344539 edvart-1.1.1/edvart/plots.py
+-rwxr-xr-x   0        0        0    40227 2023-07-27 14:10:53.416242 edvart-1.1.1/edvart/report.py
+-rw-r--r--   0        0        0       42 2023-07-20 14:02:58.347872 edvart-1.1.1/edvart/report_sections/__init__.py
+-rw-r--r--   0        0        0    40075 2023-07-20 14:02:58.347872 edvart-1.1.1/edvart/report_sections/bivariate_analysis.py
+-rw-r--r--   0        0        0     1823 2023-07-20 14:02:58.347872 edvart-1.1.1/edvart/report_sections/code_string_formatting.py
+-rw-r--r--   0        0        0    38313 2023-07-20 14:02:58.347872 edvart-1.1.1/edvart/report_sections/dataset_overview.py
+-rw-r--r--   0        0        0    27953 2023-07-20 14:02:58.504538 edvart-1.1.1/edvart/report_sections/group_analysis.py
+-rw-r--r--   0        0        0    33689 2023-07-27 14:11:24.542832 edvart-1.1.1/edvart/report_sections/multivariate_analysis.py
+-rw-r--r--   0        0        0     6680 2023-07-20 14:02:58.671205 edvart-1.1.1/edvart/report_sections/section_base.py
+-rw-r--r--   0        0        0     4380 2023-07-20 14:02:58.347872 edvart-1.1.1/edvart/report_sections/table_of_contents.py
+-rw-r--r--   0        0        0      510 2023-07-20 14:02:58.347872 edvart-1.1.1/edvart/report_sections/timeseries_analysis/__init__.py
+-rw-r--r--   0        0        0     9011 2023-07-20 14:02:58.347872 edvart-1.1.1/edvart/report_sections/timeseries_analysis/autocorrelation.py
+-rw-r--r--   0        0        0    11933 2023-07-20 14:02:58.347872 edvart-1.1.1/edvart/report_sections/timeseries_analysis/boxplots_over_time.py
+-rw-r--r--   0        0        0     6742 2023-07-20 14:02:58.347872 edvart-1.1.1/edvart/report_sections/timeseries_analysis/fourier_transform.py
+-rw-r--r--   0        0        0     8409 2023-07-20 14:02:58.347872 edvart-1.1.1/edvart/report_sections/timeseries_analysis/rolling_statistics.py
+-rw-r--r--   0        0        0     6956 2023-07-20 14:02:58.351205 edvart-1.1.1/edvart/report_sections/timeseries_analysis/seasonal_decomposition.py
+-rw-r--r--   0        0        0     8568 2023-07-20 14:02:58.351205 edvart-1.1.1/edvart/report_sections/timeseries_analysis/short_time_ft.py
+-rw-r--r--   0        0        0     6878 2023-07-20 14:02:58.351205 edvart-1.1.1/edvart/report_sections/timeseries_analysis/stationarity_tests.py
+-rw-r--r--   0        0        0     8140 2023-07-27 14:11:24.542832 edvart-1.1.1/edvart/report_sections/timeseries_analysis/time_analysis_plot.py
+-rw-r--r--   0        0        0    13844 2023-07-20 14:02:58.351205 edvart-1.1.1/edvart/report_sections/timeseries_analysis/timeseries_analysis.py
+-rw-r--r--   0        0        0    10060 2023-07-20 14:02:58.351205 edvart-1.1.1/edvart/report_sections/umap.py
+-rw-r--r--   0        0        0    17023 2023-07-20 14:02:58.351205 edvart-1.1.1/edvart/report_sections/univariate_analysis.py
+-rwxr-xr-x   0        0        0    12528 2023-07-27 14:10:53.416242 edvart-1.1.1/edvart/utils.py
+-rw-r--r--   0        0        0  4769813 2023-07-20 14:02:58.377872 edvart-1.1.1/example-datasets/Meteorite_Landings.csv
+-rw-r--r--   0        0        0    17732 2023-07-20 14:02:58.377872 edvart-1.1.1/example-datasets/auto.csv
+-rw-r--r--   0        0        0    39839 2023-07-20 14:02:58.381205 edvart-1.1.1/example-datasets/global_temp.csv
+-rw-r--r--   0        0        0  2295543 2023-07-20 14:02:58.391205 edvart-1.1.1/example-datasets/pollution.csv
+-rw-r--r--   0        0        0    60302 2023-07-20 14:02:58.391205 edvart-1.1.1/example-datasets/titanic.csv
+-rw-r--r--   0        0        0     1077 2023-07-27 14:11:30.276151 edvart-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1129 1970-01-01 00:00:00.000000 edvart-1.1.1/PKG-INFO
```

### Comparing `edvart-1.1.0/LICENSE` & `edvart-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/edvart/data_types.py` & `edvart-1.1.1/edvart/data_types.py`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/edvart/decorators.py` & `edvart-1.1.1/edvart/decorators.py`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/edvart/example_datasets.py` & `edvart-1.1.1/edvart/example_datasets.py`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/edvart/export_utils.py` & `edvart-1.1.1/edvart/export_utils.py`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/edvart/pandas_formatting.py` & `edvart-1.1.1/edvart/pandas_formatting.py`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/edvart/plots.py` & `edvart-1.1.1/edvart/plots.py`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/edvart/report.py` & `edvart-1.1.1/edvart/report.py`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/edvart/report_sections/bivariate_analysis.py` & `edvart-1.1.1/edvart/report_sections/bivariate_analysis.py`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/edvart/report_sections/code_string_formatting.py` & `edvart-1.1.1/edvart/report_sections/code_string_formatting.py`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/edvart/report_sections/dataset_overview.py` & `edvart-1.1.1/edvart/report_sections/dataset_overview.py`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/edvart/report_sections/group_analysis.py` & `edvart-1.1.1/edvart/report_sections/group_analysis.py`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/edvart/report_sections/multivariate_analysis.py` & `edvart-1.1.1/edvart/report_sections/multivariate_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
                     f"MultivariateAnalysis.MultivariateAnalysisSubsection.{str(sub)}"
                     for sub in self.subsections_0
                 ]
                 code += f", subsections={arg_subsections_names}".replace("'", "")
             if self.columns is not None:
                 code += f", columns={self.columns}"
             if self.color_col is not None:
-                code += f", color_col={self.color_col}"
+                code += f", color_col='{self.color_col}'"
             code += ")"
             cells.append(nbfv4.new_code_cell(code))
             for sub in self.subsections:
                 if sub.verbosity > 0:
                     sub.add_cells(cells)
         else:
             super().add_cells(cells)
```

### Comparing `edvart-1.1.0/edvart/report_sections/section_base.py` & `edvart-1.1.1/edvart/report_sections/section_base.py`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/edvart/report_sections/table_of_contents.py` & `edvart-1.1.1/edvart/report_sections/table_of_contents.py`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/edvart/report_sections/timeseries_analysis/autocorrelation.py` & `edvart-1.1.1/edvart/report_sections/timeseries_analysis/autocorrelation.py`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/edvart/report_sections/timeseries_analysis/boxplots_over_time.py` & `edvart-1.1.1/edvart/report_sections/timeseries_analysis/boxplots_over_time.py`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/edvart/report_sections/timeseries_analysis/fourier_transform.py` & `edvart-1.1.1/edvart/report_sections/timeseries_analysis/fourier_transform.py`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/edvart/report_sections/timeseries_analysis/rolling_statistics.py` & `edvart-1.1.1/edvart/report_sections/timeseries_analysis/rolling_statistics.py`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/edvart/report_sections/timeseries_analysis/seasonal_decomposition.py` & `edvart-1.1.1/edvart/report_sections/timeseries_analysis/seasonal_decomposition.py`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/edvart/report_sections/timeseries_analysis/short_time_ft.py` & `edvart-1.1.1/edvart/report_sections/timeseries_analysis/short_time_ft.py`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/edvart/report_sections/timeseries_analysis/stationarity_tests.py` & `edvart-1.1.1/edvart/report_sections/timeseries_analysis/stationarity_tests.py`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/edvart/report_sections/timeseries_analysis/time_analysis_plot.py` & `edvart-1.1.1/edvart/report_sections/timeseries_analysis/time_analysis_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
         section_header = nbfv4.new_markdown_cell(self.get_title(section_level=2))
         cells.append(section_header)
 
         default_call = "time_analysis_plot(df=df"
         if self.columns is not None:
             default_call += f", columns={self.columns}"
         if self.color_col is not None:
-            default_call += f", color_col={self.color_col}"
+            default_call += f", color_col='{self.color_col}'"
         if self.separate_plots:
             default_call += ", separate_plots=True"
         default_call += ")"
 
         if self.verbosity <= 1:
             code = default_call
         else:
```

### Comparing `edvart-1.1.0/edvart/report_sections/timeseries_analysis/timeseries_analysis.py` & `edvart-1.1.1/edvart/report_sections/timeseries_analysis/timeseries_analysis.py`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/edvart/report_sections/umap.py` & `edvart-1.1.1/edvart/report_sections/umap.py`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/edvart/report_sections/univariate_analysis.py` & `edvart-1.1.1/edvart/report_sections/univariate_analysis.py`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/edvart/utils.py` & `edvart-1.1.1/edvart/utils.py`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/example-datasets/Meteorite_Landings.csv` & `edvart-1.1.1/example-datasets/Meteorite_Landings.csv`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/example-datasets/auto.csv` & `edvart-1.1.1/example-datasets/auto.csv`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/example-datasets/global_temp.csv` & `edvart-1.1.1/example-datasets/global_temp.csv`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/example-datasets/pollution.csv` & `edvart-1.1.1/example-datasets/pollution.csv`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/example-datasets/titanic.csv` & `edvart-1.1.1/example-datasets/titanic.csv`

 * *Files identical despite different names*

### Comparing `edvart-1.1.0/pyproject.toml` & `edvart-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edvart"
-version = "1.1.0"  # DO NOT CHANGE - managed by Git tags and CI
+version = "1.1.1"  # DO NOT CHANGE - managed by Git tags and CI
 license = "MIT"
 repository = "https://github.com/datamole-ai/edvart"
 description = "Effective data visualization and reporting tool"
 authors = ["Michal Belak <michal.belak@datamole.ai>"]
 include = ["example-datasets/*.csv"]
 exclude = ["tests"]
```

### Comparing `edvart-1.1.0/PKG-INFO` & `edvart-1.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edvart
-Version: 1.1.0
+Version: 1.1.1
 Summary: Effective data visualization and reporting tool
 Home-page: https://github.com/datamole-ai/edvart
 License: MIT
 Author: Michal Belak
 Author-email: michal.belak@datamole.ai
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

