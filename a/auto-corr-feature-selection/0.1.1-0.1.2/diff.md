# Comparing `tmp/auto_corr_feature_selection-0.1.1.tar.gz` & `tmp/auto_corr_feature_selection-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_corr_feature_selection-0.1.1.tar", max compression
+gzip compressed data, was "auto_corr_feature_selection-0.1.2.tar", max compression
```

## Comparing `auto_corr_feature_selection-0.1.1.tar` & `auto_corr_feature_selection-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3136 2023-07-19 14:13:50.699169 auto_corr_feature_selection-0.1.1/README.md
--rw-r--r--   0        0        0       66 2023-07-19 11:37:26.859400 auto_corr_feature_selection-0.1.1/auto_corr_feature_selection/__init__.py
--rw-r--r--   0        0        0     3088 2023-07-19 13:48:29.439086 auto_corr_feature_selection-0.1.1/auto_corr_feature_selection/auto_corr_feature_selection.py
--rw-r--r--   0        0        0      740 2023-07-20 12:31:13.482452 auto_corr_feature_selection-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3734 1970-01-01 00:00:00.000000 auto_corr_feature_selection-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3136 2023-07-19 14:13:50.699169 auto_corr_feature_selection-0.1.2/README.md
+-rw-r--r--   0        0        0       66 2023-07-19 11:37:26.859400 auto_corr_feature_selection-0.1.2/auto_corr_feature_selection/__init__.py
+-rw-r--r--   0        0        0     3079 2023-07-27 14:27:34.277475 auto_corr_feature_selection-0.1.2/auto_corr_feature_selection/auto_corr_feature_selection.py
+-rw-r--r--   0        0        0      850 2023-07-27 14:31:33.745449 auto_corr_feature_selection-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3799 1970-01-01 00:00:00.000000 auto_corr_feature_selection-0.1.2/PKG-INFO
```

### Comparing `auto_corr_feature_selection-0.1.1/README.md` & `auto_corr_feature_selection-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `auto_corr_feature_selection-0.1.1/auto_corr_feature_selection/auto_corr_feature_selection.py` & `auto_corr_feature_selection-0.1.2/auto_corr_feature_selection/auto_corr_feature_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,32 +56,30 @@
             list: A list of column names with correlation above the threshold.
         """
 
         selected_columns = []
         remaining_columns = [i for i in range(len(self.__data.columns))]
 
         while len(remaining_columns):
-
             # Store the correlation hit count for each column
             correlation_counts = {}
 
             for i in remaining_columns:
-
                 # Count the number of columns with a correlation greater than the threshold
                 corr_matrix = self.correlation_matrix()
                 count = np.sum(abs(corr_matrix.iloc[i]) >= threshold)
                 correlation_counts[i] = count
 
             if not correlation_counts:
                 break
 
             # Get the column with the highest number of matches
             max_column = max(
                 correlation_counts,
-                key=lambda x, cc=correlation_counts: (cc[x], self.__data.columns[x]),
+                key=lambda x: (correlation_counts[x], self.__data.columns[x]),
                 default=None,
             )
 
             if max_column is None:
                 break
 
             selected_columns.append(max_column)
```

### Comparing `auto_corr_feature_selection-0.1.1/pyproject.toml` & `auto_corr_feature_selection-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 [tool.poetry]
 name = "auto_corr_feature_selection"
-version = "0.1.1"
+version = "0.1.2"
 description = "Automatically select the most relevant features based on correlation."
-authors = ["Andres Di Giovanni <andresdigiovanni@gmail.com>"]
+authors = ["Andrés Di Giovanni <andresdigiovanni@gmail.com>"]
 readme = "README.md"
+license = "MIT"
 packages = [{include = "auto_corr_feature_selection"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 pandas = ">1.5.0"
 numpy = "^1.25.1"
 scikit-learn = "^1.3.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 pre-commit = "^2.20.0"
 
+[project.urls]
+Homepage = "https://github.com/andresdigiovanni/auto-corr-feature-selection"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
 include = '\.pyi?$'
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `auto_corr_feature_selection-0.1.1/PKG-INFO` & `auto_corr_feature_selection-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: auto-corr-feature-selection
-Version: 0.1.1
+Version: 0.1.2
 Summary: Automatically select the most relevant features based on correlation.
-Author: Andres Di Giovanni
+License: MIT
+Author: Andrés Di Giovanni
 Author-email: andresdigiovanni@gmail.com
 Requires-Python: >=3.9
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.25.1,<2.0.0)
 Requires-Dist: pandas (>1.5.0)
 Requires-Dist: scikit-learn (>=1.3.0,<2.0.0)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

