# Comparing `tmp/pymeilisearch_scraper-0.1.0.tar.gz` & `tmp/pymeilisearch_scraper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeilisearch_scraper-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pymeilisearch_scraper-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pymeilisearch_scraper-0.1.0.tar` & `pymeilisearch_scraper-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    23138 2023-07-27 13:08:26.770515 pymeilisearch_scraper-0.1.0/README.md
--rw-r--r--   0        0        0     1519 2023-07-27 13:08:26.858515 pymeilisearch_scraper-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      285 2023-07-27 13:08:26.858515 pymeilisearch_scraper-0.1.0/scraper/__init__.py
--rw-r--r--   0        0        0     2049 2023-07-27 13:08:26.858515 pymeilisearch_scraper-0.1.0/scraper/__main__.py
--rw-r--r--   0        0        0        1 2023-07-27 13:08:26.858515 pymeilisearch_scraper-0.1.0/scraper/src/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 13:08:26.858515 pymeilisearch_scraper-0.1.0/scraper/src/config/__init__.py
--rw-r--r--   0        0        0     1303 2023-07-27 13:08:26.858515 pymeilisearch_scraper-0.1.0/scraper/src/config/browser_handler.py
--rw-r--r--   0        0        0     3674 2023-07-27 13:08:26.862515 pymeilisearch_scraper-0.1.0/scraper/src/config/config_loader.py
--rw-r--r--   0        0        0     3206 2023-07-27 13:08:26.862515 pymeilisearch_scraper-0.1.0/scraper/src/config/config_validator.py
--rw-r--r--   0        0        0     2963 2023-07-27 13:08:26.862515 pymeilisearch_scraper-0.1.0/scraper/src/config/selectors_parser.py
--rw-r--r--   0        0        0     7180 2023-07-27 13:08:26.862515 pymeilisearch_scraper-0.1.0/scraper/src/config/urls_parser.py
--rw-r--r--   0        0        0      202 2023-07-27 13:08:26.862515 pymeilisearch_scraper-0.1.0/scraper/src/config/version.py
--rw-r--r--   0        0        0     1786 2023-07-27 13:08:26.862515 pymeilisearch_scraper-0.1.0/scraper/src/custom_downloader_middleware.py
--rw-r--r--   0        0        0     4426 2023-07-27 13:08:26.862515 pymeilisearch_scraper-0.1.0/scraper/src/custom_dupefilter.py
--rw-r--r--   0        0        0    10680 2023-07-27 13:08:26.862515 pymeilisearch_scraper-0.1.0/scraper/src/documentation_spider.py
--rw-r--r--   0        0        0      898 2023-07-27 13:08:26.862515 pymeilisearch_scraper-0.1.0/scraper/src/helpers.py
--rw-r--r--   0        0        0     4312 2023-07-27 13:08:26.862515 pymeilisearch_scraper-0.1.0/scraper/src/index.py
--rw-r--r--   0        0        0      532 2023-07-27 13:08:26.862515 pymeilisearch_scraper-0.1.0/scraper/src/js_executor.py
--rw-r--r--   0        0        0     6538 2023-07-27 13:08:26.862515 pymeilisearch_scraper-0.1.0/scraper/src/meilisearch_helper.py
--rw-r--r--   0        0        0        0 2023-07-27 13:08:26.862515 pymeilisearch_scraper-0.1.0/scraper/src/strategies/__init__.py
--rw-r--r--   0        0        0     5603 2023-07-27 13:08:26.862515 pymeilisearch_scraper-0.1.0/scraper/src/strategies/abstract_strategy.py
--rw-r--r--   0        0        0     1679 2023-07-27 13:08:26.862515 pymeilisearch_scraper-0.1.0/scraper/src/strategies/anchor.py
--rw-r--r--   0        0        0    13926 2023-07-27 13:08:26.862515 pymeilisearch_scraper-0.1.0/scraper/src/strategies/default_strategy.py
--rw-r--r--   0        0        0      915 2023-07-27 13:08:26.862515 pymeilisearch_scraper-0.1.0/scraper/src/strategies/hierarchy.py
--rw-r--r--   0        0        0    24601 1970-01-01 00:00:00.000000 pymeilisearch_scraper-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    23138 2023-07-27 13:27:49.549405 pymeilisearch_scraper-0.1.1/README.md
+-rw-r--r--   0        0        0     1519 2023-07-27 13:27:49.637408 pymeilisearch_scraper-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      285 2023-07-27 13:27:49.637408 pymeilisearch_scraper-0.1.1/scraper/__init__.py
+-rw-r--r--   0        0        0     2049 2023-07-27 13:27:49.637408 pymeilisearch_scraper-0.1.1/scraper/__main__.py
+-rw-r--r--   0        0        0        1 2023-07-27 13:27:49.637408 pymeilisearch_scraper-0.1.1/scraper/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 13:27:49.637408 pymeilisearch_scraper-0.1.1/scraper/src/config/__init__.py
+-rw-r--r--   0        0        0     1303 2023-07-27 13:27:49.637408 pymeilisearch_scraper-0.1.1/scraper/src/config/browser_handler.py
+-rw-r--r--   0        0        0     3674 2023-07-27 13:27:49.637408 pymeilisearch_scraper-0.1.1/scraper/src/config/config_loader.py
+-rw-r--r--   0        0        0     3206 2023-07-27 13:27:49.637408 pymeilisearch_scraper-0.1.1/scraper/src/config/config_validator.py
+-rw-r--r--   0        0        0     2963 2023-07-27 13:27:49.637408 pymeilisearch_scraper-0.1.1/scraper/src/config/selectors_parser.py
+-rw-r--r--   0        0        0     7180 2023-07-27 13:27:49.637408 pymeilisearch_scraper-0.1.1/scraper/src/config/urls_parser.py
+-rw-r--r--   0        0        0      202 2023-07-27 13:27:49.637408 pymeilisearch_scraper-0.1.1/scraper/src/config/version.py
+-rw-r--r--   0        0        0     1786 2023-07-27 13:27:49.637408 pymeilisearch_scraper-0.1.1/scraper/src/custom_downloader_middleware.py
+-rw-r--r--   0        0        0     4426 2023-07-27 13:27:49.637408 pymeilisearch_scraper-0.1.1/scraper/src/custom_dupefilter.py
+-rw-r--r--   0        0        0    10680 2023-07-27 13:27:49.637408 pymeilisearch_scraper-0.1.1/scraper/src/documentation_spider.py
+-rw-r--r--   0        0        0      898 2023-07-27 13:27:49.637408 pymeilisearch_scraper-0.1.1/scraper/src/helpers.py
+-rw-r--r--   0        0        0     4312 2023-07-27 13:27:49.637408 pymeilisearch_scraper-0.1.1/scraper/src/index.py
+-rw-r--r--   0        0        0      532 2023-07-27 13:27:49.641409 pymeilisearch_scraper-0.1.1/scraper/src/js_executor.py
+-rw-r--r--   0        0        0     6538 2023-07-27 13:27:49.641409 pymeilisearch_scraper-0.1.1/scraper/src/meilisearch_helper.py
+-rw-r--r--   0        0        0        0 2023-07-27 13:27:49.641409 pymeilisearch_scraper-0.1.1/scraper/src/strategies/__init__.py
+-rw-r--r--   0        0        0     5603 2023-07-27 13:27:49.641409 pymeilisearch_scraper-0.1.1/scraper/src/strategies/abstract_strategy.py
+-rw-r--r--   0        0        0     1679 2023-07-27 13:27:49.641409 pymeilisearch_scraper-0.1.1/scraper/src/strategies/anchor.py
+-rw-r--r--   0        0        0    13926 2023-07-27 13:27:49.641409 pymeilisearch_scraper-0.1.1/scraper/src/strategies/default_strategy.py
+-rw-r--r--   0        0        0      915 2023-07-27 13:27:49.641409 pymeilisearch_scraper-0.1.1/scraper/src/strategies/hierarchy.py
+-rw-r--r--   0        0        0    24601 1970-01-01 00:00:00.000000 pymeilisearch_scraper-0.1.1/PKG-INFO
```

### Comparing `pymeilisearch_scraper-0.1.0/README.md` & `pymeilisearch_scraper-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pymeilisearch_scraper-0.1.0/pyproject.toml` & `pymeilisearch_scraper-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "pymeilisearch-scraper"
-version = "0.1.0"
+version = "0.1.1"
 description = "Documentation scrapper for PyMeilisearch"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
     {name = "ANSYS, Inc.", email="pyansys.core@ansys.com"},
 ]
 maintainers = [{name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"}]
```

### Comparing `pymeilisearch_scraper-0.1.0/scraper/__main__.py` & `pymeilisearch_scraper-0.1.1/scraper/__main__.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch_scraper-0.1.0/scraper/src/config/browser_handler.py` & `pymeilisearch_scraper-0.1.1/scraper/src/config/browser_handler.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch_scraper-0.1.0/scraper/src/config/config_loader.py` & `pymeilisearch_scraper-0.1.1/scraper/src/config/config_loader.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch_scraper-0.1.0/scraper/src/config/config_validator.py` & `pymeilisearch_scraper-0.1.1/scraper/src/config/config_validator.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch_scraper-0.1.0/scraper/src/config/selectors_parser.py` & `pymeilisearch_scraper-0.1.1/scraper/src/config/selectors_parser.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch_scraper-0.1.0/scraper/src/config/urls_parser.py` & `pymeilisearch_scraper-0.1.1/scraper/src/config/urls_parser.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch_scraper-0.1.0/scraper/src/custom_downloader_middleware.py` & `pymeilisearch_scraper-0.1.1/scraper/src/custom_downloader_middleware.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch_scraper-0.1.0/scraper/src/custom_dupefilter.py` & `pymeilisearch_scraper-0.1.1/scraper/src/custom_dupefilter.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch_scraper-0.1.0/scraper/src/documentation_spider.py` & `pymeilisearch_scraper-0.1.1/scraper/src/documentation_spider.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch_scraper-0.1.0/scraper/src/helpers.py` & `pymeilisearch_scraper-0.1.1/scraper/src/helpers.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch_scraper-0.1.0/scraper/src/index.py` & `pymeilisearch_scraper-0.1.1/scraper/src/index.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch_scraper-0.1.0/scraper/src/js_executor.py` & `pymeilisearch_scraper-0.1.1/scraper/src/js_executor.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch_scraper-0.1.0/scraper/src/meilisearch_helper.py` & `pymeilisearch_scraper-0.1.1/scraper/src/meilisearch_helper.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch_scraper-0.1.0/scraper/src/strategies/abstract_strategy.py` & `pymeilisearch_scraper-0.1.1/scraper/src/strategies/abstract_strategy.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch_scraper-0.1.0/scraper/src/strategies/anchor.py` & `pymeilisearch_scraper-0.1.1/scraper/src/strategies/anchor.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch_scraper-0.1.0/scraper/src/strategies/default_strategy.py` & `pymeilisearch_scraper-0.1.1/scraper/src/strategies/default_strategy.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch_scraper-0.1.0/scraper/src/strategies/hierarchy.py` & `pymeilisearch_scraper-0.1.1/scraper/src/strategies/hierarchy.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch_scraper-0.1.0/PKG-INFO` & `pymeilisearch_scraper-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeilisearch-scraper
-Version: 0.1.0
+Version: 0.1.1
 Summary: Documentation scrapper for PyMeilisearch
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymeilisearch-scraper Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: pymeilisearch-scraper Version: 0.1.1 Summary:
 Documentation scrapper for PyMeilisearch Author-email: "ANSYS, Inc."
 core@ansys.com> Maintainer-email: "ANSYS, Inc."
 core@ansys.com> Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Science/Research Classifier: Topic :: Scientific/Engineering :: Information
 Analysis Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
```

