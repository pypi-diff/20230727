# Comparing `tmp/starlette_werkzeug_debugger-0.1.0.tar.gz` & `tmp/starlette_werkzeug_debugger-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette_werkzeug_debugger-0.1.0.tar", last modified: Tue Jun 20 11:43:23 2023, max compression
+gzip compressed data, was "starlette_werkzeug_debugger-0.1.1.tar", last modified: Thu Jul 27 15:17:55 2023, max compression
```

## Comparing `starlette_werkzeug_debugger-0.1.0.tar` & `starlette_werkzeug_debugger-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-06-20 11:43:23.254830 starlette_werkzeug_debugger-0.1.0/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      128 2023-06-19 16:24:57.000000 starlette_werkzeug_debugger-0.1.0/.editorconfig
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-06-20 11:43:23.253831 starlette_werkzeug_debugger-0.1.0/.github/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-06-20 11:43:23.254830 starlette_werkzeug_debugger-0.1.0/.github/workflows/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      795 2023-06-20 10:33:43.000000 starlette_werkzeug_debugger-0.1.0/.github/workflows/python-package.yml
--rw-r--r--   0 mirec     (1000) mirec     (1000)      117 2023-06-19 16:46:46.000000 starlette_werkzeug_debugger-0.1.0/.gitignore
--rw-r--r--   0 mirec     (1000) mirec     (1000)      197 2023-06-20 04:33:48.000000 starlette_werkzeug_debugger-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 mirec     (1000) mirec     (1000)    17720 2023-06-20 04:33:24.000000 starlette_werkzeug_debugger-0.1.0/.pylintrc
--rw-r--r--   0 mirec     (1000) mirec     (1000)      235 2023-06-20 11:42:01.000000 starlette_werkzeug_debugger-0.1.0/CHANGELOG.md
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1073 2023-06-19 16:29:38.000000 starlette_werkzeug_debugger-0.1.0/LICENSE
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2666 2023-06-20 11:43:23.254830 starlette_werkzeug_debugger-0.1.0/PKG-INFO
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1933 2023-06-20 10:47:32.000000 starlette_werkzeug_debugger-0.1.0/README.rst
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1174 2023-06-20 11:42:01.000000 starlette_werkzeug_debugger-0.1.0/pyproject.toml
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-06-20 11:43:23.254830 starlette_werkzeug_debugger-0.1.0/sample_usage/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      284 2023-06-20 11:32:39.000000 starlette_werkzeug_debugger-0.1.0/sample_usage/fastapi_example.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      457 2023-06-20 11:32:39.000000 starlette_werkzeug_debugger-0.1.0/sample_usage/starlette_example.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2023-06-20 11:43:23.254830 starlette_werkzeug_debugger-0.1.0/setup.cfg
--rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2023-06-19 16:26:05.000000 starlette_werkzeug_debugger-0.1.0/setup.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-06-20 11:43:23.254830 starlette_werkzeug_debugger-0.1.0/starlette_werkzeug_debugger/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     3041 2023-06-20 10:27:46.000000 starlette_werkzeug_debugger-0.1.0/starlette_werkzeug_debugger/__init__.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-06-20 11:43:23.254830 starlette_werkzeug_debugger-0.1.0/starlette_werkzeug_debugger.egg-info/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2666 2023-06-20 11:43:23.000000 starlette_werkzeug_debugger-0.1.0/starlette_werkzeug_debugger.egg-info/PKG-INFO
--rw-r--r--   0 mirec     (1000) mirec     (1000)      560 2023-06-20 11:43:23.000000 starlette_werkzeug_debugger-0.1.0/starlette_werkzeug_debugger.egg-info/SOURCES.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)        1 2023-06-20 11:43:23.000000 starlette_werkzeug_debugger-0.1.0/starlette_werkzeug_debugger.egg-info/dependency_links.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)       72 2023-06-20 11:43:23.000000 starlette_werkzeug_debugger-0.1.0/starlette_werkzeug_debugger.egg-info/requires.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)       28 2023-06-20 11:43:23.000000 starlette_werkzeug_debugger-0.1.0/starlette_werkzeug_debugger.egg-info/top_level.txt
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-06-20 11:43:23.254830 starlette_werkzeug_debugger-0.1.0/tests/
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2023-06-20 04:43:35.000000 starlette_werkzeug_debugger-0.1.0/tests/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     3867 2023-06-20 10:26:34.000000 starlette_werkzeug_debugger-0.1.0/tests/test_debugger.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      379 2023-06-20 10:29:15.000000 starlette_werkzeug_debugger-0.1.0/tox.ini
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-07-27 15:17:55.033007 starlette_werkzeug_debugger-0.1.1/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      128 2023-06-19 16:24:57.000000 starlette_werkzeug_debugger-0.1.1/.editorconfig
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-07-27 15:17:55.032007 starlette_werkzeug_debugger-0.1.1/.github/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-07-27 15:17:55.033007 starlette_werkzeug_debugger-0.1.1/.github/workflows/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      795 2023-06-20 10:33:43.000000 starlette_werkzeug_debugger-0.1.1/.github/workflows/python-package.yml
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      117 2023-06-19 16:46:46.000000 starlette_werkzeug_debugger-0.1.1/.gitignore
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      197 2023-06-20 04:33:48.000000 starlette_werkzeug_debugger-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 mirec     (1000) mirec     (1000)    17720 2023-06-20 04:33:24.000000 starlette_werkzeug_debugger-0.1.1/.pylintrc
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      375 2023-07-27 15:17:35.000000 starlette_werkzeug_debugger-0.1.1/CHANGELOG.md
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1073 2023-06-19 16:29:38.000000 starlette_werkzeug_debugger-0.1.1/LICENSE
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2666 2023-07-27 15:17:55.033007 starlette_werkzeug_debugger-0.1.1/PKG-INFO
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1933 2023-06-20 10:47:32.000000 starlette_werkzeug_debugger-0.1.1/README.rst
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1173 2023-07-27 15:17:35.000000 starlette_werkzeug_debugger-0.1.1/pyproject.toml
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-07-27 15:17:55.033007 starlette_werkzeug_debugger-0.1.1/sample_usage/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      284 2023-06-20 11:32:39.000000 starlette_werkzeug_debugger-0.1.1/sample_usage/fastapi_example.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2811 2023-06-23 03:41:08.000000 starlette_werkzeug_debugger-0.1.1/sample_usage/fastapi_swagger_integraation.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      457 2023-06-20 11:32:39.000000 starlette_werkzeug_debugger-0.1.1/sample_usage/starlette_example.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-07-27 15:17:55.033007 starlette_werkzeug_debugger-0.1.1/sample_usage/static/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      767 2023-06-23 03:40:04.000000 starlette_werkzeug_debugger-0.1.1/sample_usage/static/swagger_extra.css
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2010 2023-06-23 03:40:08.000000 starlette_werkzeug_debugger-0.1.1/sample_usage/static/swagger_extra.js
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2023-07-27 15:17:55.034007 starlette_werkzeug_debugger-0.1.1/setup.cfg
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2023-06-19 16:26:05.000000 starlette_werkzeug_debugger-0.1.1/setup.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-07-27 15:17:55.033007 starlette_werkzeug_debugger-0.1.1/starlette_werkzeug_debugger/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     3041 2023-06-20 10:27:46.000000 starlette_werkzeug_debugger-0.1.1/starlette_werkzeug_debugger/__init__.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-07-27 15:17:55.033007 starlette_werkzeug_debugger-0.1.1/starlette_werkzeug_debugger.egg-info/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2666 2023-07-27 15:17:55.000000 starlette_werkzeug_debugger-0.1.1/starlette_werkzeug_debugger.egg-info/PKG-INFO
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      680 2023-07-27 15:17:55.000000 starlette_werkzeug_debugger-0.1.1/starlette_werkzeug_debugger.egg-info/SOURCES.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        1 2023-07-27 15:17:55.000000 starlette_werkzeug_debugger-0.1.1/starlette_werkzeug_debugger.egg-info/dependency_links.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       72 2023-07-27 15:17:55.000000 starlette_werkzeug_debugger-0.1.1/starlette_werkzeug_debugger.egg-info/requires.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       28 2023-07-27 15:17:55.000000 starlette_werkzeug_debugger-0.1.1/starlette_werkzeug_debugger.egg-info/top_level.txt
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-07-27 15:17:55.033007 starlette_werkzeug_debugger-0.1.1/tests/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2023-06-20 04:43:35.000000 starlette_werkzeug_debugger-0.1.1/tests/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     3867 2023-06-20 10:26:34.000000 starlette_werkzeug_debugger-0.1.1/tests/test_debugger.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      400 2023-07-27 15:16:16.000000 starlette_werkzeug_debugger-0.1.1/tox.ini
```

### Comparing `starlette_werkzeug_debugger-0.1.0/.github/workflows/python-package.yml` & `starlette_werkzeug_debugger-0.1.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `starlette_werkzeug_debugger-0.1.0/.pylintrc` & `starlette_werkzeug_debugger-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `starlette_werkzeug_debugger-0.1.0/LICENSE` & `starlette_werkzeug_debugger-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `starlette_werkzeug_debugger-0.1.0/PKG-INFO` & `starlette_werkzeug_debugger-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starlette_werkzeug_debugger
-Version: 0.1.0
+Version: 0.1.1
 Summary: Werkzeug debugger middleware for Starlette
 Author-email: Miroslav Bendík <miroslav.bendik@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/mireq/starlette-werkzeug-debugger
 Project-URL: documentation, https://github.com/mireq/starlette-werkzeug-debugger
 Project-URL: repository, https://github.com/mireq/starlette-werkzeug-debugger
 Project-URL: changelog, https://github.com/mireq/starlette-werkzeug-debugger/blob/master/CHANGELOG.md
```

### Comparing `starlette_werkzeug_debugger-0.1.0/README.rst` & `starlette_werkzeug_debugger-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `starlette_werkzeug_debugger-0.1.0/pyproject.toml` & `starlette_werkzeug_debugger-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,40 +8,39 @@
 dynamic = ["version"]
 authors = [
 	{ name = "Miroslav Bendík", email = "miroslav.bendik@gmail.com" }
 ]
 classifiers = [
 	"Programming Language :: Python :: 3",
 ]
-dependencies = [
-	"werkzeug",
-	"starlette",
-]
+dependencies = []
 
 [project.urls]
 homepage = "https://github.com/mireq/starlette-werkzeug-debugger"
 documentation = "https://github.com/mireq/starlette-werkzeug-debugger"
 repository = "https://github.com/mireq/starlette-werkzeug-debugger"
 changelog = "https://github.com/mireq/starlette-werkzeug-debugger/blob/master/CHANGELOG.md"
 
 [project.optional-dependencies]
 dev = [
 	"tox",
 	"pylint",
 	"pre-commit",
 	"bump2version",
-	"commitizen"
+	"commitizen",
+	"werkzeug",
+	"starlette"
 ]
 
 [build-system]
 requires = ["setuptools", "setuptools-scm", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 include = ["starlette_werkzeug_debugger*"]
 
 [tool.setuptools_scm]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.1.0"
+version = "0.1.1"
 tag_format = "$version"
```

### Comparing `starlette_werkzeug_debugger-0.1.0/starlette_werkzeug_debugger/__init__.py` & `starlette_werkzeug_debugger-0.1.1/starlette_werkzeug_debugger/__init__.py`

 * *Files identical despite different names*

### Comparing `starlette_werkzeug_debugger-0.1.0/starlette_werkzeug_debugger.egg-info/PKG-INFO` & `starlette_werkzeug_debugger-0.1.1/starlette_werkzeug_debugger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starlette-werkzeug-debugger
-Version: 0.1.0
+Version: 0.1.1
 Summary: Werkzeug debugger middleware for Starlette
 Author-email: Miroslav Bendík <miroslav.bendik@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/mireq/starlette-werkzeug-debugger
 Project-URL: documentation, https://github.com/mireq/starlette-werkzeug-debugger
 Project-URL: repository, https://github.com/mireq/starlette-werkzeug-debugger
 Project-URL: changelog, https://github.com/mireq/starlette-werkzeug-debugger/blob/master/CHANGELOG.md
```

### Comparing `starlette_werkzeug_debugger-0.1.0/starlette_werkzeug_debugger.egg-info/SOURCES.txt` & `starlette_werkzeug_debugger-0.1.1/starlette_werkzeug_debugger.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 LICENSE
 README.rst
 pyproject.toml
 setup.py
 tox.ini
 .github/workflows/python-package.yml
 sample_usage/fastapi_example.py
+sample_usage/fastapi_swagger_integraation.py
 sample_usage/starlette_example.py
+sample_usage/static/swagger_extra.css
+sample_usage/static/swagger_extra.js
 starlette_werkzeug_debugger/__init__.py
 starlette_werkzeug_debugger.egg-info/PKG-INFO
 starlette_werkzeug_debugger.egg-info/SOURCES.txt
 starlette_werkzeug_debugger.egg-info/dependency_links.txt
 starlette_werkzeug_debugger.egg-info/requires.txt
 starlette_werkzeug_debugger.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `starlette_werkzeug_debugger-0.1.0/tests/test_debugger.py` & `starlette_werkzeug_debugger-0.1.1/tests/test_debugger.py`

 * *Files identical despite different names*

