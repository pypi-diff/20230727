# Comparing `tmp/gammarer.aws-daily-cost-usage-reporter-0.9.6.tar.gz` & `tmp/gammarer.aws-daily-cost-usage-reporter-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-daily-cost-usage-reporter-0.9.6.tar", last modified: Wed Jul 26 19:19:35 2023, max compression
+gzip compressed data, was "gammarer.aws-daily-cost-usage-reporter-0.9.7.tar", last modified: Thu Jul 27 19:19:59 2023, max compression
```

## Comparing `gammarer.aws-daily-cost-usage-reporter-0.9.6.tar` & `gammarer.aws-daily-cost-usage-reporter-0.9.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:19:35.154818 gammarer.aws-daily-cost-usage-reporter-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-26 19:19:23.000000 gammarer.aws-daily-cost-usage-reporter-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 19:19:23.000000 gammarer.aws-daily-cost-usage-reporter-0.9.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-26 19:19:35.154818 gammarer.aws-daily-cost-usage-reporter-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-26 19:19:23.000000 gammarer.aws-daily-cost-usage-reporter-0.9.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-26 19:19:23.000000 gammarer.aws-daily-cost-usage-reporter-0.9.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 19:19:35.154818 gammarer.aws-daily-cost-usage-reporter-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-26 19:19:23.000000 gammarer.aws-daily-cost-usage-reporter-0.9.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:19:35.154818 gammarer.aws-daily-cost-usage-reporter-0.9.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:19:35.154818 gammarer.aws-daily-cost-usage-reporter-0.9.6/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:19:35.154818 gammarer.aws-daily-cost-usage-reporter-0.9.6/src/gammarer/aws_daily_cost_usage_reporter/
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-07-26 19:19:23.000000 gammarer.aws-daily-cost-usage-reporter-0.9.6/src/gammarer/aws_daily_cost_usage_reporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:19:35.154818 gammarer.aws-daily-cost-usage-reporter-0.9.6/src/gammarer/aws_daily_cost_usage_reporter/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-26 19:19:23.000000 gammarer.aws-daily-cost-usage-reporter-0.9.6/src/gammarer/aws_daily_cost_usage_reporter/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   233519 2023-07-26 19:19:23.000000 gammarer.aws-daily-cost-usage-reporter-0.9.6/src/gammarer/aws_daily_cost_usage_reporter/_jsii/aws-daily-cost-usage-reporter@0.9.6.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 19:19:23.000000 gammarer.aws-daily-cost-usage-reporter-0.9.6/src/gammarer/aws_daily_cost_usage_reporter/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:19:35.154818 gammarer.aws-daily-cost-usage-reporter-0.9.6/src/gammarer.aws_daily_cost_usage_reporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-26 19:19:35.000000 gammarer.aws-daily-cost-usage-reporter-0.9.6/src/gammarer.aws_daily_cost_usage_reporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-26 19:19:35.000000 gammarer.aws-daily-cost-usage-reporter-0.9.6/src/gammarer.aws_daily_cost_usage_reporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 19:19:35.000000 gammarer.aws-daily-cost-usage-reporter-0.9.6/src/gammarer.aws_daily_cost_usage_reporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-26 19:19:35.000000 gammarer.aws-daily-cost-usage-reporter-0.9.6/src/gammarer.aws_daily_cost_usage_reporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 19:19:35.000000 gammarer.aws-daily-cost-usage-reporter-0.9.6/src/gammarer.aws_daily_cost_usage_reporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:19:59.195878 gammarer.aws-daily-cost-usage-reporter-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-27 19:19:47.000000 gammarer.aws-daily-cost-usage-reporter-0.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 19:19:47.000000 gammarer.aws-daily-cost-usage-reporter-0.9.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-27 19:19:59.195878 gammarer.aws-daily-cost-usage-reporter-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-27 19:19:47.000000 gammarer.aws-daily-cost-usage-reporter-0.9.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-27 19:19:47.000000 gammarer.aws-daily-cost-usage-reporter-0.9.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 19:19:59.195878 gammarer.aws-daily-cost-usage-reporter-0.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-27 19:19:47.000000 gammarer.aws-daily-cost-usage-reporter-0.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:19:59.191878 gammarer.aws-daily-cost-usage-reporter-0.9.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:19:59.191878 gammarer.aws-daily-cost-usage-reporter-0.9.7/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:19:59.195878 gammarer.aws-daily-cost-usage-reporter-0.9.7/src/gammarer/aws_daily_cost_usage_reporter/
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-07-27 19:19:47.000000 gammarer.aws-daily-cost-usage-reporter-0.9.7/src/gammarer/aws_daily_cost_usage_reporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:19:59.195878 gammarer.aws-daily-cost-usage-reporter-0.9.7/src/gammarer/aws_daily_cost_usage_reporter/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-27 19:19:47.000000 gammarer.aws-daily-cost-usage-reporter-0.9.7/src/gammarer/aws_daily_cost_usage_reporter/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   233518 2023-07-27 19:19:47.000000 gammarer.aws-daily-cost-usage-reporter-0.9.7/src/gammarer/aws_daily_cost_usage_reporter/_jsii/aws-daily-cost-usage-reporter@0.9.7.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:19:47.000000 gammarer.aws-daily-cost-usage-reporter-0.9.7/src/gammarer/aws_daily_cost_usage_reporter/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:19:59.195878 gammarer.aws-daily-cost-usage-reporter-0.9.7/src/gammarer.aws_daily_cost_usage_reporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-27 19:19:59.000000 gammarer.aws-daily-cost-usage-reporter-0.9.7/src/gammarer.aws_daily_cost_usage_reporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-27 19:19:59.000000 gammarer.aws-daily-cost-usage-reporter-0.9.7/src/gammarer.aws_daily_cost_usage_reporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:19:59.000000 gammarer.aws-daily-cost-usage-reporter-0.9.7/src/gammarer.aws_daily_cost_usage_reporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-27 19:19:59.000000 gammarer.aws-daily-cost-usage-reporter-0.9.7/src/gammarer.aws_daily_cost_usage_reporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 19:19:59.000000 gammarer.aws-daily-cost-usage-reporter-0.9.7/src/gammarer.aws_daily_cost_usage_reporter.egg-info/top_level.txt
```

### Comparing `gammarer.aws-daily-cost-usage-reporter-0.9.6/LICENSE` & `gammarer.aws-daily-cost-usage-reporter-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-daily-cost-usage-reporter-0.9.6/PKG-INFO` & `gammarer.aws-daily-cost-usage-reporter-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-daily-cost-usage-reporter
-Version: 0.9.6
+Version: 0.9.7
 Summary: Cost & Usage Reports
 Home-page: https://github.com/yicr/aws-daily-cost-usage-reporter.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-daily-cost-usage-reporter.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-daily-cost-usage-reporter-0.9.6/README.md` & `gammarer.aws-daily-cost-usage-reporter-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-daily-cost-usage-reporter-0.9.6/setup.py` & `gammarer.aws-daily-cost-usage-reporter-0.9.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-daily-cost-usage-reporter",
-    "version": "0.9.6",
+    "version": "0.9.7",
     "description": "Cost & Usage Reports",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-daily-cost-usage-reporter.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_daily_cost_usage_reporter",
         "gammarer.aws_daily_cost_usage_reporter._jsii"
     ],
     "package_data": {
         "gammarer.aws_daily_cost_usage_reporter._jsii": [
-            "aws-daily-cost-usage-reporter@0.9.6.jsii.tgz"
+            "aws-daily-cost-usage-reporter@0.9.7.jsii.tgz"
         ],
         "gammarer.aws_daily_cost_usage_reporter": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `gammarer.aws-daily-cost-usage-reporter-0.9.6/src/gammarer/aws_daily_cost_usage_reporter/__init__.py` & `gammarer.aws-daily-cost-usage-reporter-0.9.7/src/gammarer/aws_daily_cost_usage_reporter/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-daily-cost-usage-reporter-0.9.6/src/gammarer.aws_daily_cost_usage_reporter.egg-info/PKG-INFO` & `gammarer.aws-daily-cost-usage-reporter-0.9.7/src/gammarer.aws_daily_cost_usage_reporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-daily-cost-usage-reporter
-Version: 0.9.6
+Version: 0.9.7
 Summary: Cost & Usage Reports
 Home-page: https://github.com/yicr/aws-daily-cost-usage-reporter.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-daily-cost-usage-reporter.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-daily-cost-usage-reporter-0.9.6/src/gammarer.aws_daily_cost_usage_reporter.egg-info/SOURCES.txt` & `gammarer.aws-daily-cost-usage-reporter-0.9.7/src/gammarer.aws_daily_cost_usage_reporter.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_daily_cost_usage_reporter.egg-info/SOURCES.txt
 src/gammarer.aws_daily_cost_usage_reporter.egg-info/dependency_links.txt
 src/gammarer.aws_daily_cost_usage_reporter.egg-info/requires.txt
 src/gammarer.aws_daily_cost_usage_reporter.egg-info/top_level.txt
 src/gammarer/aws_daily_cost_usage_reporter/__init__.py
 src/gammarer/aws_daily_cost_usage_reporter/py.typed
 src/gammarer/aws_daily_cost_usage_reporter/_jsii/__init__.py
-src/gammarer/aws_daily_cost_usage_reporter/_jsii/aws-daily-cost-usage-reporter@0.9.6.jsii.tgz
+src/gammarer/aws_daily_cost_usage_reporter/_jsii/aws-daily-cost-usage-reporter@0.9.7.jsii.tgz
```

