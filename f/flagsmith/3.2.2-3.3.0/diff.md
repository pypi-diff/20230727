# Comparing `tmp/flagsmith-3.2.2.tar.gz` & `tmp/flagsmith-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flagsmith-3.2.2.tar", max compression
+gzip compressed data, was "flagsmith-3.3.0.tar", max compression
```

## Comparing `flagsmith-3.2.2.tar` & `flagsmith-3.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1476 2023-07-07 12:56:39.339852 flagsmith-3.2.2/LICENSE
--rw-r--r--   0        0        0     1118 2023-07-07 12:56:39.339852 flagsmith-3.2.2/Readme.md
--rw-r--r--   0        0        0       41 2023-07-07 12:56:39.343852 flagsmith-3.2.2/flagsmith/__init__.py
--rw-r--r--   0        0        0     2008 2023-07-07 12:56:39.343852 flagsmith-3.2.2/flagsmith/analytics.py
--rw-r--r--   0        0        0      106 2023-07-07 12:56:39.343852 flagsmith-3.2.2/flagsmith/exceptions.py
--rw-r--r--   0        0        0    11095 2023-07-07 12:56:39.343852 flagsmith-3.2.2/flagsmith/flagsmith.py
--rw-r--r--   0        0        0     4633 2023-07-07 12:56:39.343852 flagsmith-3.2.2/flagsmith/models.py
--rw-r--r--   0        0        0      822 2023-07-07 12:56:39.343852 flagsmith-3.2.2/flagsmith/polling_manager.py
--rw-r--r--   0        0        0        0 2023-07-07 12:56:39.343852 flagsmith-3.2.2/flagsmith/utils/__init__.py
--rw-r--r--   0        0        0      204 2023-07-07 12:56:39.343852 flagsmith-3.2.2/flagsmith/utils/identities.py
--rw-r--r--   0        0        0      724 2023-07-07 12:56:39.343852 flagsmith-3.2.2/pyproject.toml
--rw-r--r--   0        0        0     1935 1970-01-01 00:00:00.000000 flagsmith-3.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1476 2023-07-27 12:57:23.741132 flagsmith-3.3.0/LICENSE
+-rw-r--r--   0        0        0     1118 2023-07-27 12:57:23.741132 flagsmith-3.3.0/Readme.md
+-rw-r--r--   0        0        0       41 2023-07-27 12:57:23.741132 flagsmith-3.3.0/flagsmith/__init__.py
+-rw-r--r--   0        0        0     2008 2023-07-27 12:57:23.741132 flagsmith-3.3.0/flagsmith/analytics.py
+-rw-r--r--   0        0        0      106 2023-07-27 12:57:23.741132 flagsmith-3.3.0/flagsmith/exceptions.py
+-rw-r--r--   0        0        0    11095 2023-07-27 12:57:23.741132 flagsmith-3.3.0/flagsmith/flagsmith.py
+-rw-r--r--   0        0        0     4633 2023-07-27 12:57:23.741132 flagsmith-3.3.0/flagsmith/models.py
+-rw-r--r--   0        0        0      822 2023-07-27 12:57:23.741132 flagsmith-3.3.0/flagsmith/polling_manager.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:57:23.741132 flagsmith-3.3.0/flagsmith/utils/__init__.py
+-rw-r--r--   0        0        0      204 2023-07-27 12:57:23.741132 flagsmith-3.3.0/flagsmith/utils/identities.py
+-rw-r--r--   0        0        0      723 2023-07-27 12:57:23.741132 flagsmith-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1935 1970-01-01 00:00:00.000000 flagsmith-3.3.0/PKG-INFO
```

### Comparing `flagsmith-3.2.2/LICENSE` & `flagsmith-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flagsmith-3.2.2/Readme.md` & `flagsmith-3.3.0/Readme.md`

 * *Files identical despite different names*

### Comparing `flagsmith-3.2.2/flagsmith/analytics.py` & `flagsmith-3.3.0/flagsmith/analytics.py`

 * *Files identical despite different names*

### Comparing `flagsmith-3.2.2/flagsmith/flagsmith.py` & `flagsmith-3.3.0/flagsmith/flagsmith.py`

 * *Files identical despite different names*

### Comparing `flagsmith-3.2.2/flagsmith/models.py` & `flagsmith-3.3.0/flagsmith/models.py`

 * *Files identical despite different names*

### Comparing `flagsmith-3.2.2/flagsmith/polling_manager.py` & `flagsmith-3.3.0/flagsmith/polling_manager.py`

 * *Files identical despite different names*

### Comparing `flagsmith-3.2.2/pyproject.toml` & `flagsmith-3.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "flagsmith"
-version = "3.2.2"
+version = "3.3.0"
 description = "Flagsmith Python SDK"
 authors = ["Flagsmith <support@flagsmith.com>"]
 license = "BSD3"
 readme = "Readme.md"
 keywords = ["feature", "flag", "flagsmith", "remote", "config"]
 documentation = "https://docs.flagsmith.com"
 packages = [
     {include = "flagsmith"},
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
 requests = "^2.27.1"
 requests-futures = "^1.0.0"
-flagsmith-flag-engine = "^2.3.0"
+flagsmith-flag-engine = "^4.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-mock = "^3.6.1"
-black = "^21.12b0"
+black = "^23.3.0"
 pre-commit = "^2.17.0"
 responses = "^0.17.0"
 flake8 = "^4.0.1"
 isort = "^5.10.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `flagsmith-3.2.2/PKG-INFO` & `flagsmith-3.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: flagsmith
-Version: 3.2.2
+Version: 3.3.0
 Summary: Flagsmith Python SDK
 License: BSD3
 Keywords: feature,flag,flagsmith,remote,config
 Author: Flagsmith
 Author-email: support@flagsmith.com
 Requires-Python: >=3.7.0,<4
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: flagsmith-flag-engine (>=2.3.0,<3.0.0)
+Requires-Dist: flagsmith-flag-engine (>=4.0.0,<5.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: requests-futures (>=1.0.0,<2.0.0)
 Project-URL: Documentation, https://docs.flagsmith.com
 Description-Content-Type: text/markdown
 
 <img width="100%" src="https://github.com/Flagsmith/flagsmith/raw/main/static-files/hero.png"/>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: flagsmith Version: 3.2.2 Summary: Flagsmith Python
+Metadata-Version: 2.1 Name: flagsmith Version: 3.3.0 Summary: Flagsmith Python
 SDK License: BSD3 Keywords: feature,flag,flagsmith,remote,config Author:
 Flagsmith Author-email: support@flagsmith.com Requires-Python: >=3.7.0,<4
 Classifier: License :: Other/Proprietary License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: flagsmith-
-flag-engine (>=2.3.0,<3.0.0) Requires-Dist: requests (>=2.27.1,<3.0.0)
+flag-engine (>=4.0.0,<5.0.0) Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: requests-futures (>=1.0.0,<2.0.0) Project-URL: Documentation,
 https://docs.flagsmith.com Description-Content-Type: text/markdown [https://
 github.com/Flagsmith/flagsmith/raw/main/static-files/hero.png] # Flagsmith
 Python SDK > Flagsmith allows you to manage feature flags and remote config
 across multiple projects, environments and > organisations. The SDK for Python
 applications for [https://www.flagsmith.com/](https://www.flagsmith.com/). ##
 Adding to your project For full documentation visit [https://
```

