# Comparing `tmp/ansys_pyensight_core-0.5.0.tar.gz` & `tmp/ansys_pyensight_core-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_pyensight_core-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_pyensight_core-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_pyensight_core-0.5.0.tar` & `ansys_pyensight_core-0.5.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1089 2023-07-26 16:46:03.712791 ansys_pyensight_core-0.5.0/LICENSE
--rw-r--r--   0        0        0     8121 2023-07-26 16:46:03.712791 ansys_pyensight_core-0.5.0/README.rst
--rw-r--r--   0        0        0     3977 2023-07-26 16:46:03.744791 ansys_pyensight_core-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      828 2023-07-26 16:46:03.744791 ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/__init__.py
--rw-r--r--   0        0        0     3351 2023-07-26 16:46:03.744791 ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/deep_pixel_view.html
--rw-r--r--   0        0        0    24888 2023-07-26 16:46:03.744791 ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/dockerlauncher.py
--rw-r--r--   0        0        0    11803 2023-07-26 16:46:03.744791 ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/enscontext.py
--rw-r--r--   0        0        0    14948 2023-07-26 16:46:03.744791 ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/enshell_grpc.py
--rw-r--r--   0        0        0    14343 2023-07-26 16:46:03.744791 ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/ensight_grpc.py
--rw-r--r--   0        0        0    17343 2023-07-26 16:46:03.744791 ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/ensobj.py
--rw-r--r--   0        0        0     5900 2023-07-26 16:46:03.744791 ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/launch_ensight.py
--rw-r--r--   0        0        0     8957 2023-07-26 16:46:03.744791 ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/launcher.py
--rw-r--r--   0        0        0     7640 2023-07-26 16:46:03.744791 ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/listobj.py
--rw-r--r--   0        0        0    13908 2023-07-26 16:46:03.744791 ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/locallauncher.py
--rw-r--r--   0        0        0        0 2023-07-26 16:46:03.744791 ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/py.typed
--rw-r--r--   0        0        0    26241 2023-07-26 16:46:03.744791 ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/renderable.py
--rw-r--r--   0        0        0    58977 2023-07-26 16:46:03.744791 ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/session.py
--rw-r--r--   0        0        0      752 2023-07-26 16:46:03.744791 ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/sgeo_poll.html
--rw-r--r--   0        0        0        0 2023-07-26 16:46:03.744791 ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/utils/__init__.py
--rw-r--r--   0        0        0    17657 2023-07-26 16:46:03.744791 ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/utils/export.py
--rw-r--r--   0        0        0     3986 2023-07-26 16:46:03.744791 ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/utils/parts.py
--rw-r--r--   0        0        0    19035 2023-07-26 16:46:03.744791 ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/utils/query.py
--rw-r--r--   0        0        0     2397 2023-07-26 16:46:03.744791 ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/utils/support.py
--rw-r--r--   0        0        0    12285 2023-07-26 16:46:03.744791 ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/utils/views.py
--rw-r--r--   0        0        0    10831 1970-01-01 00:00:00.000000 ansys_pyensight_core-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-07-27 10:28:54.049978 ansys_pyensight_core-0.5.1/LICENSE
+-rw-r--r--   0        0        0     8121 2023-07-27 10:28:54.049978 ansys_pyensight_core-0.5.1/README.rst
+-rw-r--r--   0        0        0     3976 2023-07-27 10:28:54.085979 ansys_pyensight_core-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      828 2023-07-27 10:28:54.085979 ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/__init__.py
+-rw-r--r--   0        0        0     3351 2023-07-27 10:28:54.085979 ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/deep_pixel_view.html
+-rw-r--r--   0        0        0    24888 2023-07-27 10:28:54.085979 ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/dockerlauncher.py
+-rw-r--r--   0        0        0    11803 2023-07-27 10:28:54.085979 ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/enscontext.py
+-rw-r--r--   0        0        0    14948 2023-07-27 10:28:54.085979 ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/enshell_grpc.py
+-rw-r--r--   0        0        0    14343 2023-07-27 10:28:54.085979 ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/ensight_grpc.py
+-rw-r--r--   0        0        0    17343 2023-07-27 10:28:54.085979 ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/ensobj.py
+-rw-r--r--   0        0        0     5900 2023-07-27 10:28:54.085979 ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/launch_ensight.py
+-rw-r--r--   0        0        0     8957 2023-07-27 10:28:54.085979 ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/launcher.py
+-rw-r--r--   0        0        0     7640 2023-07-27 10:28:54.085979 ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/listobj.py
+-rw-r--r--   0        0        0    13908 2023-07-27 10:28:54.085979 ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/locallauncher.py
+-rw-r--r--   0        0        0        0 2023-07-27 10:28:54.085979 ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/py.typed
+-rw-r--r--   0        0        0    26241 2023-07-27 10:28:54.085979 ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/renderable.py
+-rw-r--r--   0        0        0    58977 2023-07-27 10:28:54.089979 ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/session.py
+-rw-r--r--   0        0        0      752 2023-07-27 10:28:54.089979 ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/sgeo_poll.html
+-rw-r--r--   0        0        0        0 2023-07-27 10:28:54.089979 ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/utils/__init__.py
+-rw-r--r--   0        0        0    17657 2023-07-27 10:28:54.089979 ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/utils/export.py
+-rw-r--r--   0        0        0     3986 2023-07-27 10:28:54.089979 ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/utils/parts.py
+-rw-r--r--   0        0        0    19035 2023-07-27 10:28:54.089979 ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/utils/query.py
+-rw-r--r--   0        0        0     2397 2023-07-27 10:28:54.089979 ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/utils/support.py
+-rw-r--r--   0        0        0    12285 2023-07-27 10:28:54.089979 ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/utils/views.py
+-rw-r--r--   0        0        0    10831 1970-01-01 00:00:00.000000 ansys_pyensight_core-0.5.1/PKG-INFO
```

### Comparing `ansys_pyensight_core-0.5.0/LICENSE` & `ansys_pyensight_core-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.0/README.rst` & `ansys_pyensight_core-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.0/pyproject.toml` & `ansys_pyensight_core-0.5.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "flit_core>=3.2,<4"
 ]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-pyensight-core"
-version = "0.5.0"
+version = "0.5.1"
 description = "A python wrapper for Ansys EnSight"
 readme = "README.rst"
 requires-python = ">=3.8,<4"
 license = {file = "LICENSE"}
 authors = [{name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"}]
 maintainers = [{name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"}]
 classifiers = [
@@ -41,25 +41,23 @@
 dev = [
     "build>=0.10.0",
     "bump2version>=1.0.1",
     "ipdb>=0.9.4",
     "dill>=0.3.5.1",
     "pre-commit>=3.3.3",
 ]
-
 tests = [
     "pytest==7.1.2",
     "pytest-cov==3.0.0",
     "dill>=0.3.5.1",
     "pytest-mock==3.10.0",
     "urllib3==1.26.10",
     "requests>=2.28.2",
     "pyansys-docker>=5.0.4",
 ]
-
 doc = [
     "Sphinx==7.0.1",
     "numpydoc==1.5.0",
     "ansys-sphinx-theme==0.9.9",
     "sphinx-copybutton==0.5.1",
     "sphinx-gallery==0.13.0",
     "sphinxcontrib-mermaid==0.8.1",
@@ -67,14 +65,24 @@
     "matplotlib==3.7.1",
     "requests>=2.28.2",
     "sphinxcontrib.jquery==3.0.0",
     "coverage-badge==1.1.0",
     "sphinxcontrib-openapi==0.8.1"
 ]
 
+[project.urls]
+Documentation = "https://ensight.docs.pyansys.com/"
+Homepage = "https://github.com/ansys/pyensight"
+Source = "https://github.com/ansys/pyensight"
+Tracker = "https://github.com/ansys/pyensight/issues"
+Changelog =  "https://github.com/ansys/pyensight/blob/main/CHANGELOG.rst"
+
+[tool.flit.module]
+name = "ansys.pyensight.core"
+
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "def __repr__",
@@ -87,24 +95,14 @@
 
 ignore_errors = true
 show_missing = true
 
 [tool.coverage.html]
 show_contexts = true
 
-[project.urls]
-Documentation = "https://ensight.docs.pyansys.com/"
-Homepage = "https://github.com/ansys/pyensight"
-Source = "https://github.com/ansys/pyensight"
-Tracker = "https://github.com/ansys/pyensight/issues"
-Changelog =  "https://github.com/ansys/pyensight/blob/main/CHANGELOG.rst"
-
-[tool.flit.module]
-name = "ansys.pyensight.core"
-
 [tool.black]
 line-length = 100
 src_paths = ["src/ansys", "doc"]
 
 [tool.pytest.ini_options]
 minversion = "7.1"
 testpaths = [
@@ -165,8 +163,8 @@
  "numpy",
  "PIL",
  "simple_upload_server.*"
 ]
 ignore_missing_imports = true
 
 [pydocstyle]
-convention = "numpy"
+convention = "numpy"
```

### Comparing `ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/__init__.py` & `ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/deep_pixel_view.html` & `ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/deep_pixel_view.html`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/dockerlauncher.py` & `ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/dockerlauncher.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/enscontext.py` & `ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/enscontext.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/enshell_grpc.py` & `ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/enshell_grpc.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/ensight_grpc.py` & `ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/ensight_grpc.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/ensobj.py` & `ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/ensobj.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/launch_ensight.py` & `ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/launch_ensight.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/launcher.py` & `ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/launcher.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/listobj.py` & `ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/listobj.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/locallauncher.py` & `ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/locallauncher.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/renderable.py` & `ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/renderable.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/session.py` & `ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/session.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/sgeo_poll.html` & `ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/sgeo_poll.html`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/utils/export.py` & `ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/utils/export.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/utils/parts.py` & `ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/utils/parts.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/utils/query.py` & `ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/utils/query.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/utils/support.py` & `ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/utils/support.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.0/src/ansys/pyensight/core/utils/views.py` & `ansys_pyensight_core-0.5.1/src/ansys/pyensight/core/utils/views.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.0/PKG-INFO` & `ansys_pyensight_core-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-pyensight-core
-Version: 0.5.0
+Version: 0.5.1
 Summary: A python wrapper for Ansys EnSight
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

