# Comparing `tmp/business-rules-enhanced-1.3.7.tar.gz` & `tmp/business-rules-enhanced-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "business-rules-enhanced-1.3.7.tar", last modified: Wed Jun 28 19:20:11 2023, max compression
+gzip compressed data, was "business-rules-enhanced-1.4.0.tar", last modified: Thu Jul 27 13:02:08 2023, max compression
```

## Comparing `business-rules-enhanced-1.3.7.tar` & `business-rules-enhanced-1.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 19:20:11.234890 business-rules-enhanced-1.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-28 19:19:38.000000 business-rules-enhanced-1.3.7/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-28 19:19:38.000000 business-rules-enhanced-1.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 19:19:38.000000 business-rules-enhanced-1.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-28 19:20:11.234890 business-rules-enhanced-1.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-06-28 19:19:38.000000 business-rules-enhanced-1.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 19:20:11.230889 business-rules-enhanced-1.3.7/business_rules/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-28 19:19:38.000000 business-rules-enhanced-1.3.7/business_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-28 19:19:38.000000 business-rules-enhanced-1.3.7/business_rules/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-28 19:19:38.000000 business-rules-enhanced-1.3.7/business_rules/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-28 19:19:38.000000 business-rules-enhanced-1.3.7/business_rules/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    58941 2023-06-28 19:19:38.000000 business-rules-enhanced-1.3.7/business_rules/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    20588 2023-06-28 19:19:38.000000 business-rules-enhanced-1.3.7/business_rules/six.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-28 19:19:38.000000 business-rules-enhanced-1.3.7/business_rules/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-28 19:19:38.000000 business-rules-enhanced-1.3.7/business_rules/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 19:20:11.234890 business-rules-enhanced-1.3.7/business_rules_enhanced.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-28 19:20:11.000000 business-rules-enhanced-1.3.7/business_rules_enhanced.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-28 19:20:11.000000 business-rules-enhanced-1.3.7/business_rules_enhanced.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 19:20:11.000000 business-rules-enhanced-1.3.7/business_rules_enhanced.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-28 19:20:11.000000 business-rules-enhanced-1.3.7/business_rules_enhanced.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 19:20:11.234890 business-rules-enhanced-1.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-28 19:19:38.000000 business-rules-enhanced-1.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:02:08.548084 business-rules-enhanced-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-27 13:01:48.000000 business-rules-enhanced-1.4.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-27 13:01:48.000000 business-rules-enhanced-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 13:01:48.000000 business-rules-enhanced-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-27 13:02:08.548084 business-rules-enhanced-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-07-27 13:01:48.000000 business-rules-enhanced-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:02:08.548084 business-rules-enhanced-1.4.0/business_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-27 13:01:48.000000 business-rules-enhanced-1.4.0/business_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-27 13:01:48.000000 business-rules-enhanced-1.4.0/business_rules/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-27 13:01:48.000000 business-rules-enhanced-1.4.0/business_rules/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-27 13:01:48.000000 business-rules-enhanced-1.4.0/business_rules/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58985 2023-07-27 13:01:48.000000 business-rules-enhanced-1.4.0/business_rules/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20588 2023-07-27 13:01:48.000000 business-rules-enhanced-1.4.0/business_rules/six.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-07-27 13:01:48.000000 business-rules-enhanced-1.4.0/business_rules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-27 13:01:48.000000 business-rules-enhanced-1.4.0/business_rules/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:02:08.548084 business-rules-enhanced-1.4.0/business_rules_enhanced.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-27 13:02:08.000000 business-rules-enhanced-1.4.0/business_rules_enhanced.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-27 13:02:08.000000 business-rules-enhanced-1.4.0/business_rules_enhanced.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:02:08.000000 business-rules-enhanced-1.4.0/business_rules_enhanced.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 13:02:08.000000 business-rules-enhanced-1.4.0/business_rules_enhanced.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 13:02:08.548084 business-rules-enhanced-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-27 13:01:48.000000 business-rules-enhanced-1.4.0/setup.py
```

### Comparing `business-rules-enhanced-1.3.7/LICENSE` & `business-rules-enhanced-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.7/PKG-INFO` & `business-rules-enhanced-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: business-rules-enhanced
-Version: 1.3.7
+Version: 1.4.0
 Summary: Fork of Venmo-Business-Rules: Python DSL for setting up business intelligence rules that can be configured without code  History -------  1.0.1 +++++ released 2016-3-16  - Fixes a packaging bug preventing 1.0.0 from being installed on some platforms.  1.0.0 +++++ released 2016-3-16  - Removes caching layer on rule decorator 
 Home-page: https://github.com/cdisc-org/business-rules
 Author: cdisc-org
 Author-email: UNKNOWN
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `business-rules-enhanced-1.3.7/README.md` & `business-rules-enhanced-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.7/business_rules/actions.py` & `business-rules-enhanced-1.4.0/business_rules/actions.py`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.7/business_rules/engine.py` & `business-rules-enhanced-1.4.0/business_rules/engine.py`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.7/business_rules/operators.py` & `business-rules-enhanced-1.4.0/business_rules/operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1042,22 +1042,20 @@
         within a group_by column. The dataframe is grouped by a certain column
         and the check is applied to each group.
         """
         target = self.replace_prefix(other_value.get("target"))
         min_count: int = other_value.get("comparator") or 1
         group_by_column = self.replace_prefix(other_value.get("within"))
         grouped = self.value.groupby(group_by_column)
-        results = grouped.apply(lambda x: self.validate_series_length(x[target], min_count))
-        return pd.Series(results.explode().tolist())
+        results = grouped.apply(lambda x: self.validate_series_length(x, target, min_count))
+        return pd.Series(results.sort_index(level=1).tolist())
 
-    def validate_series_length(self, ser: pd.Series, min_length: int):
-        if len(ser) > min_length:
-            return [True] * len(ser)
-        else:
-            return [False] * min_length
+    def validate_series_length(self, data: pd.DataFrame, target: str, min_length: int):
+        value_counts = data[target].value_counts().to_dict()
+        return data[target].apply(lambda x: value_counts.get(x, 0) > min_length)
 
     @type_operator(FIELD_DATAFRAME)
     def not_present_on_multiple_rows_within(self, other_value: dict):
         return ~self.present_on_multiple_rows_within(other_value)
 
     def detect_reference(self, row, value_column, target_column, context=None):
         if context:
```

### Comparing `business-rules-enhanced-1.3.7/business_rules/six.py` & `business-rules-enhanced-1.4.0/business_rules/six.py`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.7/business_rules/utils.py` & `business-rules-enhanced-1.4.0/business_rules/utils.py`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.7/business_rules/variables.py` & `business-rules-enhanced-1.4.0/business_rules/variables.py`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.7/business_rules_enhanced.egg-info/PKG-INFO` & `business-rules-enhanced-1.4.0/business_rules_enhanced.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: business-rules-enhanced
-Version: 1.3.7
+Version: 1.4.0
 Summary: Fork of Venmo-Business-Rules: Python DSL for setting up business intelligence rules that can be configured without code  History -------  1.0.1 +++++ released 2016-3-16  - Fixes a packaging bug preventing 1.0.0 from being installed on some platforms.  1.0.0 +++++ released 2016-3-16  - Removes caching layer on rule decorator 
 Home-page: https://github.com/cdisc-org/business-rules
 Author: cdisc-org
 Author-email: UNKNOWN
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `business-rules-enhanced-1.3.7/setup.py` & `business-rules-enhanced-1.4.0/setup.py`

 * *Files identical despite different names*

