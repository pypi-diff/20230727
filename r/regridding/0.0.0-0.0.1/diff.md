# Comparing `tmp/regridding-0.0.0.tar.gz` & `tmp/regridding-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regridding-0.0.0.tar", last modified: Sat Jun 10 21:45:31 2023, max compression
+gzip compressed data, was "regridding-0.0.1.tar", last modified: Thu Jul 27 17:04:03 2023, max compression
```

## Comparing `regridding-0.0.0.tar` & `regridding-0.0.1.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 21:45:30.995447 regridding-0.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 21:45:30.991446 regridding-0.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 21:45:30.995447 regridding-0.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-10 21:45:16.000000 regridding-0.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-10 21:45:16.000000 regridding-0.0.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-10 21:45:16.000000 regridding-0.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-10 21:45:16.000000 regridding-0.0.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-10 21:45:30.995447 regridding-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-10 21:45:16.000000 regridding-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 21:45:30.995447 regridding-0.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-10 21:45:16.000000 regridding-0.0.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 21:45:30.995447 regridding-0.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 21:45:16.000000 regridding-0.0.0/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 21:45:30.995447 regridding-0.0.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-10 21:45:16.000000 regridding-0.0.0/docs/_templates/class_custom.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-10 21:45:16.000000 regridding-0.0.0/docs/_templates/function_custom.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-10 21:45:16.000000 regridding-0.0.0/docs/_templates/module_custom.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-10 21:45:16.000000 regridding-0.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-10 21:45:16.000000 regridding-0.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-10 21:45:16.000000 regridding-0.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-10 21:45:16.000000 regridding-0.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 21:45:30.995447 regridding-0.0.0/regridding/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-10 21:45:16.000000 regridding-0.0.0/regridding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-10 21:45:16.000000 regridding-0.0.0/regridding/_interp_ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 21:45:30.995447 regridding-0.0.0/regridding/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 21:45:16.000000 regridding-0.0.0/regridding/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-10 21:45:16.000000 regridding-0.0.0/regridding/tests/test_interp_ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 21:45:30.995447 regridding-0.0.0/regridding.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-10 21:45:30.000000 regridding-0.0.0/regridding.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-10 21:45:30.000000 regridding-0.0.0/regridding.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 21:45:30.000000 regridding-0.0.0/regridding.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-10 21:45:30.000000 regridding-0.0.0/regridding.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-10 21:45:30.000000 regridding-0.0.0/regridding.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 21:45:30.995447 regridding-0.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:04:03.410561 regridding-0.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:04:03.406560 regridding-0.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:04:03.406560 regridding-0.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-27 17:03:51.000000 regridding-0.0.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-27 17:03:51.000000 regridding-0.0.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-27 17:03:51.000000 regridding-0.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-27 17:03:51.000000 regridding-0.0.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-27 17:04:03.410561 regridding-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-27 17:03:51.000000 regridding-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:04:03.406560 regridding-0.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-27 17:03:51.000000 regridding-0.0.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:04:03.406560 regridding-0.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 17:03:51.000000 regridding-0.0.1/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:04:03.406560 regridding-0.0.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-27 17:03:51.000000 regridding-0.0.1/docs/_templates/class_custom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-27 17:03:51.000000 regridding-0.0.1/docs/_templates/function_custom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-27 17:03:51.000000 regridding-0.0.1/docs/_templates/module_custom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-07-27 17:03:51.000000 regridding-0.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-27 17:03:51.000000 regridding-0.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-27 17:03:51.000000 regridding-0.0.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-27 17:03:51.000000 regridding-0.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:04:03.410561 regridding-0.0.1/regridding/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-27 17:03:51.000000 regridding-0.0.1/regridding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32163 2023-07-27 17:03:51.000000 regridding-0.0.1/regridding/_conservative_ramshaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-07-27 17:03:51.000000 regridding-0.0.1/regridding/_interp_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-07-27 17:03:51.000000 regridding-0.0.1/regridding/_regrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)   249506 2023-07-27 17:03:51.000000 regridding-0.0.1/regridding/inspect.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:04:03.410561 regridding-0.0.1/regridding/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 17:03:51.000000 regridding-0.0.1/regridding/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-27 17:03:51.000000 regridding-0.0.1/regridding/tests/test_interp_ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:04:03.410561 regridding-0.0.1/regridding.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-27 17:04:03.000000 regridding-0.0.1/regridding.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-27 17:04:03.000000 regridding-0.0.1/regridding.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 17:04:03.000000 regridding-0.0.1/regridding.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-27 17:04:03.000000 regridding-0.0.1/regridding.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-27 17:04:03.000000 regridding-0.0.1/regridding.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 17:04:03.410561 regridding-0.0.1/setup.cfg
```

### Comparing `regridding-0.0.0/.github/workflows/publish.yml` & `regridding-0.0.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `regridding-0.0.0/.github/workflows/tests.yml` & `regridding-0.0.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `regridding-0.0.0/PKG-INFO` & `regridding-0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regridding
-Version: 0.0.0
+Version: 0.0.1
 Summary: Numba-accelerated interpolation routines
 Author-email: "Roy T. Smart" <roytsmart@gmail.com>
 Project-URL: Homepage, https://github.com/byrdie/regridding
 Project-URL: Documentation, https://regridding.readthedocs.io/en/latest
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `regridding-0.0.0/README.md` & `regridding-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `regridding-0.0.0/docs/Makefile` & `regridding-0.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `regridding-0.0.0/docs/_templates/class_custom.rst` & `regridding-0.0.1/docs/_templates/class_custom.rst`

 * *Files identical despite different names*

### Comparing `regridding-0.0.0/docs/_templates/module_custom.rst` & `regridding-0.0.1/docs/_templates/module_custom.rst`

 * *Files identical despite different names*

### Comparing `regridding-0.0.0/docs/conf.py` & `regridding-0.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `regridding-0.0.0/docs/make.bat` & `regridding-0.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `regridding-0.0.0/pyproject.toml` & `regridding-0.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "numpy",
     "numba",
-    "astropy",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "scipy",
 ]
 doc = [
     "pytest",
+    "matplotlib",
     "graphviz",
     "sphinx-autodoc-typehints",
     "pydata-sphinx-theme",
     "jupyter-sphinx",
     "sphinx-favicon",
 ]
```

### Comparing `regridding-0.0.0/regridding/tests/test_interp_ndarray.py` & `regridding-0.0.1/regridding/tests/test_interp_ndarray.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     argvalues=[None, 0, -1]
 )
 def test_ndarray_linear_interpolation_1d(
         a: np.ndarray,
         x: np.ndarray,
         axis: None | int | tuple[int]
 ):
-    result = regridding.ndarray_linear_interpolation(a=a, coordinates=(x,), axis=axis)
+    result = regridding.ndarray_linear_interpolation(a=a, indices=(x,), axis=axis)
     expected = scipy.ndimage.map_coordinates(input=a, coordinates=x[np.newaxis], mode="nearest", order=1)
 
     assert np.allclose(result, expected)
 
 
 @pytest.mark.parametrize(
     argnames="a",
@@ -70,13 +70,11 @@
         a: np.ndarray,
         x: np.ndarray,
         y: np.ndarray,
         axis: None | tuple[int],
 ):
     x, y = np.broadcast_arrays(x, y)
 
-    result = regridding.ndarray_linear_interpolation(a=a, coordinates=(x, y), axis=axis)
+    result = regridding.ndarray_linear_interpolation(a=a, indices=(x, y), axis=axis)
     expected = scipy.ndimage.map_coordinates(input=a, coordinates=np.stack([x, y]), order=1)
 
-    print(result - expected)
-
     assert np.allclose(result, expected)
```

### Comparing `regridding-0.0.0/regridding.egg-info/PKG-INFO` & `regridding-0.0.1/regridding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regridding
-Version: 0.0.0
+Version: 0.0.1
 Summary: Numba-accelerated interpolation routines
 Author-email: "Roy T. Smart" <roytsmart@gmail.com>
 Project-URL: Homepage, https://github.com/byrdie/regridding
 Project-URL: Documentation, https://regridding.readthedocs.io/en/latest
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `regridding-0.0.0/regridding.egg-info/SOURCES.txt` & `regridding-0.0.1/regridding.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 docs/index.rst
 docs/make.bat
 docs/_static/.gitkeep
 docs/_templates/class_custom.rst
 docs/_templates/function_custom.rst
 docs/_templates/module_custom.rst
 regridding/__init__.py
+regridding/_conservative_ramshaw.py
 regridding/_interp_ndarray.py
+regridding/_regrid.py
+regridding/inspect.ipynb
 regridding.egg-info/PKG-INFO
 regridding.egg-info/SOURCES.txt
 regridding.egg-info/dependency_links.txt
 regridding.egg-info/requires.txt
 regridding.egg-info/top_level.txt
 regridding/tests/__init__.py
 regridding/tests/test_interp_ndarray.py
```

