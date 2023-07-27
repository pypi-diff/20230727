# Comparing `tmp/cudagrad-0.0.25.tar.gz` & `tmp/cudagrad-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cudagrad-0.0.25.tar", last modified: Wed Jul 26 04:14:12 2023, max compression
+gzip compressed data, was "cudagrad-0.0.26.tar", last modified: Thu Jul 27 00:54:49 2023, max compression
```

## Comparing `cudagrad-0.0.25.tar` & `cudagrad-0.0.26.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-26 04:14:12.513261 cudagrad-0.0.25/
--rw-r--r--   0 ryan       (501) staff       (20)       44 2023-07-18 06:47:23.000000 cudagrad-0.0.25/MANIFEST.in
--rw-r--r--   0 ryan       (501) staff       (20)     3672 2023-07-26 04:14:12.513131 cudagrad-0.0.25/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)     3170 2023-07-25 01:40:28.000000 cudagrad-0.0.25/README.md
--rw-r--r--   0 ryan       (501) staff       (20)      693 2023-07-26 04:13:45.000000 cudagrad-0.0.25/pyproject.toml
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-26 04:14:12.513307 cudagrad-0.0.25/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     1592 2023-07-18 02:40:23.000000 cudagrad-0.0.25/setup.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-26 04:14:12.511319 cudagrad-0.0.25/src/
--rw-r--r--   0 ryan       (501) staff       (20)     2935 2023-07-26 04:09:20.000000 cudagrad-0.0.25/src/bindings.cpp
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-26 04:14:12.512657 cudagrad-0.0.25/src/cudagrad.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)     3672 2023-07-26 04:14:12.000000 cudagrad-0.0.25/src/cudagrad.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      318 2023-07-26 04:14:12.000000 cudagrad-0.0.25/src/cudagrad.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-26 04:14:12.000000 cudagrad-0.0.25/src/cudagrad.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-18 02:46:33.000000 cudagrad-0.0.25/src/cudagrad.egg-info/not-zip-safe
--rw-r--r--   0 ryan       (501) staff       (20)       15 2023-07-26 04:14:12.000000 cudagrad-0.0.25/src/cudagrad.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        9 2023-07-26 04:14:12.000000 cudagrad-0.0.25/src/cudagrad.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)    20537 2023-07-26 04:09:23.000000 cudagrad-0.0.25/src/cudagrad.hpp
--rw-r--r--   0 ryan       (501) staff       (20)      263 2023-07-26 03:31:20.000000 cudagrad-0.0.25/src/ops.cu
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-26 04:14:12.512799 cudagrad-0.0.25/tests/
--rw-r--r--   0 ryan       (501) staff       (20)     1050 2023-07-19 01:21:03.000000 cudagrad-0.0.25/tests/test.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-27 00:54:49.608209 cudagrad-0.0.26/
+-rw-r--r--   0 ryan       (501) staff       (20)       44 2023-07-18 06:47:23.000000 cudagrad-0.0.26/MANIFEST.in
+-rw-r--r--   0 ryan       (501) staff       (20)     3672 2023-07-27 00:54:49.608009 cudagrad-0.0.26/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)     3170 2023-07-25 01:40:28.000000 cudagrad-0.0.26/README.md
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-27 00:54:49.605754 cudagrad-0.0.26/cudagrad/
+-rw-r--r--   0 ryan       (501) staff       (20)       81 2023-07-27 00:50:13.000000 cudagrad-0.0.26/cudagrad/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     5187 2023-07-27 00:16:07.000000 cudagrad-0.0.26/cudagrad/mlp.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-27 00:54:49.606770 cudagrad-0.0.26/cudagrad.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)     3672 2023-07-27 00:54:49.000000 cudagrad-0.0.26/cudagrad.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      331 2023-07-27 00:54:49.000000 cudagrad-0.0.26/cudagrad.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-27 00:54:49.000000 cudagrad-0.0.26/cudagrad.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-27 00:32:51.000000 cudagrad-0.0.26/cudagrad.egg-info/not-zip-safe
+-rw-r--r--   0 ryan       (501) staff       (20)       15 2023-07-27 00:54:49.000000 cudagrad-0.0.26/cudagrad.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        9 2023-07-27 00:54:49.000000 cudagrad-0.0.26/cudagrad.egg-info/top_level.txt
+-rw-r--r--   0 ryan       (501) staff       (20)      693 2023-07-27 00:29:37.000000 cudagrad-0.0.26/pyproject.toml
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-27 00:54:49.608281 cudagrad-0.0.26/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)     1659 2023-07-27 00:49:51.000000 cudagrad-0.0.26/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-27 00:54:49.607409 cudagrad-0.0.26/src/
+-rw-r--r--   0 ryan       (501) staff       (20)     2944 2023-07-27 00:52:48.000000 cudagrad-0.0.26/src/bindings.cpp
+-rw-r--r--   0 ryan       (501) staff       (20)    20537 2023-07-26 04:09:23.000000 cudagrad-0.0.26/src/cudagrad.hpp
+-rw-r--r--   0 ryan       (501) staff       (20)      263 2023-07-26 03:31:20.000000 cudagrad-0.0.26/src/ops.cu
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-27 00:54:49.607739 cudagrad-0.0.26/tests/
+-rw-r--r--   0 ryan       (501) staff       (20)     1078 2023-07-27 00:15:15.000000 cudagrad-0.0.26/tests/test.py
```

### Comparing `cudagrad-0.0.25/PKG-INFO` & `cudagrad-0.0.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cudagrad
-Version: 0.0.25
+Version: 0.0.26
 Summary: A small autograd engine
 Home-page: https://github.com/yrom1/cudagrad
 Author: Ryan Moore
 Author-email: Ryan Moore <moorethreads@hey.com>
 Project-URL: Homepage, https://github.com/yrom1/cudagrad
 Project-URL: Bug Tracker, https://github.com/yrom1/cudagrad/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cudagrad-0.0.25/README.md` & `cudagrad-0.0.26/README.md`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.25/pyproject.toml` & `cudagrad-0.0.26/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=40.8.0", "wheel", "pybind11>=2.10.1", "toml",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cudagrad"
-version = "0.0.25"
+version = "0.0.26"
 description = "A small autograd engine"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [ "Programming Language :: Python :: 3", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "Ryan Moore"
 email = "moorethreads@hey.com"
```

### Comparing `cudagrad-0.0.25/setup.py` & `cudagrad-0.0.26/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 # Available at setup time due to pyproject.toml
 
 import toml
 from pybind11.setup_helpers import Pybind11Extension, build_ext
-from setuptools import setup
+from setuptools import find_packages, setup
 
 
 def get_version_from_toml():
-    data = toml.load('pyproject.toml')
-    version = data.get('project', {}).get('version', None)
+    data = toml.load("pyproject.toml")
+    version = data.get("project", {}).get("version", None)
     if version is None:
         raise RuntimeError("Can't get version in TOML!")
     else:
         return version
 
+
 __version__ = get_version_from_toml()
 
 # The main interface is through Pybind11Extension.
 # * You can add cxx_std=11/14/17, and then build_ext can be removed.
 # * You can set include_pybind11=false to add the include directory yourself,
 #   say from a submodule.
 #
 # Note:
 #   Sort input source files if you glob sources to ensure bit-for-bit
 #   reproducible builds (https://github.com/pybind/cudagrad/pull/53)
 
 ext_modules = [
-    Pybind11Extension("cudagrad",
+    Pybind11Extension(
+        "cudagrad.cudagrad_bindings",
         ["src/bindings.cpp"],
         # Example: passing in the version to the compiled code
-        define_macros = [('VERSION_INFO', __version__)],
-        ),
+        define_macros=[("VERSION_INFO", __version__)],
+    ),
 ]
 
 setup(
     name="cudagrad",
     version=__version__,
     author="Ryan Moore",
     author_email="moorethreads@hey.com",
@@ -43,9 +45,10 @@
     ext_modules=ext_modules,
     extras_require={"test": "pytest"},
     # Currently, build_ext only provides an optional "highest supported C++
     # level" feature, but in the future it may provide more features.
     cmdclass={"build_ext": build_ext},
     zip_safe=False,
     python_requires=">=3.7",
+    packages=find_packages(),
     include_package_data=True,
 )
```

### Comparing `cudagrad-0.0.25/src/bindings.cpp` & `cudagrad-0.0.26/src/bindings.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #include <pybind11/pybind11.h>
 
 #define STRINGIFY(x) #x
 #define MACRO_STRINGIFY(x) STRINGIFY(x)
 
 namespace py = pybind11;
 
-PYBIND11_MODULE(cudagrad, m) {
+PYBIND11_MODULE(cudagrad_bindings, m) {
     m.doc() = R"pbdoc(
         Pybind11 example plugin
         -----------------------
 
         .. currentmodule:: cudagrad
 
         .. autosummary::
```

### Comparing `cudagrad-0.0.25/src/cudagrad.egg-info/PKG-INFO` & `cudagrad-0.0.26/cudagrad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cudagrad
-Version: 0.0.25
+Version: 0.0.26
 Summary: A small autograd engine
 Home-page: https://github.com/yrom1/cudagrad
 Author: Ryan Moore
 Author-email: Ryan Moore <moorethreads@hey.com>
 Project-URL: Homepage, https://github.com/yrom1/cudagrad
 Project-URL: Bug Tracker, https://github.com/yrom1/cudagrad/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cudagrad-0.0.25/src/cudagrad.hpp` & `cudagrad-0.0.26/src/cudagrad.hpp`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.25/tests/test.py` & `cudagrad-0.0.26/tests/test.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 import cudagrad as cg
 import torch
 
 # assert cg.__version__ == '0.0.1'
 assert cg.add(1, 2) == 3
 assert cg.subtract(1, 2) == -1
 
+
 def flatten(l):
-  out = []
-  for item in l:
-    if isinstance(item, (list, tuple)):
-      out.extend(flatten(item))
-    else:
-      out.append(item)
-  return out
+    out = []
+    for item in l:
+        if isinstance(item, (list, tuple)):
+            out.extend(flatten(item))
+        else:
+            out.append(item)
+    return out
 
 
 at = torch.tensor(((2.0, 3.0), (4.0, 5.0)), requires_grad=True)
 bt = torch.tensor(((6.0, 7.0), (8.0, 9.0)), requires_grad=True)
 ct = torch.tensor(((10.0, 10.0), (10.0, 10.0)), requires_grad=True)
 dt = torch.tensor(((11.0, 11.0), (11.0, 11.0)), requires_grad=True)
 et = (at.matmul(bt) + ct) * dt
@@ -29,12 +30,12 @@
 b = cg.tensor([2, 2], [6.0, 7.0, 8.0, 9.0])
 c = cg.tensor([2, 2], [10.0, 10.0, 10.0, 10.0])
 d = cg.tensor([2, 2], [11.0, 11.0, 11.0, 11.0])
 e = ((a @ b) + c) * d
 f = e.sum()
 f.backward()
 
-assert f.data == flatten([ft.data.tolist()]) # this is annoying lol
+assert f.data == flatten([ft.data.tolist()])  # this is annoying lol
 assert a.data == flatten(at.data.tolist())
 assert b.data == flatten(bt.data.tolist())
 
-print('Tests passed!')
+print("Tests passed!")
```

