# Comparing `tmp/slim_trees-0.2.2.tar.gz` & `tmp/slim_trees-0.2.3.tar.gz`

## Comparing `slim_trees-0.2.2.tar` & `slim_trees-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 slim_trees-0.2.2/slim_trees/__init__.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 slim_trees-0.2.2/slim_trees/compression_utils.py
--rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 slim_trees-0.2.2/slim_trees/lgbm_booster.py
--rw-r--r--   0        0        0     7799 2020-02-02 00:00:00.000000 slim_trees-0.2.2/slim_trees/pickling.py
--rw-r--r--   0        0        0     5345 2020-02-02 00:00:00.000000 slim_trees-0.2.2/slim_trees/sklearn_tree.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 slim_trees-0.2.2/slim_trees/utils.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 slim_trees-0.2.2/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 slim_trees-0.2.2/LICENSE
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 slim_trees-0.2.2/README.md
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 slim_trees-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 slim_trees-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 slim_trees-0.2.3/slim_trees/__init__.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 slim_trees-0.2.3/slim_trees/compression_utils.py
+-rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 slim_trees-0.2.3/slim_trees/lgbm_booster.py
+-rw-r--r--   0        0        0     7799 2020-02-02 00:00:00.000000 slim_trees-0.2.3/slim_trees/pickling.py
+-rw-r--r--   0        0        0     6657 2020-02-02 00:00:00.000000 slim_trees-0.2.3/slim_trees/sklearn_tree.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 slim_trees-0.2.3/slim_trees/utils.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 slim_trees-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 slim_trees-0.2.3/LICENSE
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 slim_trees-0.2.3/README.md
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 slim_trees-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 slim_trees-0.2.3/PKG-INFO
```

### Comparing `slim_trees-0.2.2/slim_trees/__init__.py` & `slim_trees-0.2.3/slim_trees/__init__.py`

 * *Files identical despite different names*

### Comparing `slim_trees-0.2.2/slim_trees/compression_utils.py` & `slim_trees-0.2.3/slim_trees/compression_utils.py`

 * *Files identical despite different names*

### Comparing `slim_trees-0.2.2/slim_trees/lgbm_booster.py` & `slim_trees-0.2.3/slim_trees/lgbm_booster.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,29 @@
 import os
 import pickle
 import re
 import sys
 from typing import Any, BinaryIO, List, Tuple
 
 import numpy as np
+from packaging.version import Version
 
 from slim_trees import __version__ as slim_trees_version
 from slim_trees.compression_utils import (
     compress_half_int_float_array,
     decompress_half_int_float_array,
     safe_cast,
 )
 from slim_trees.utils import check_version
 
 try:
+    from lightgbm import __version__ as _lightgbm_version
     from lightgbm.basic import Booster
+
+    lightgbm_version = Version(_lightgbm_version)
 except ImportError:
     print("LightGBM does not seem to be installed.")
     sys.exit(os.EX_CONFIG)
 
 
 def dump(model: Any, file: BinaryIO):
     p = pickle.Pickler(file)
@@ -53,29 +57,38 @@
 
     booster = reconstructor(*args)
     decompressed_state = _decompress_booster_state(state)
     booster.__setstate__(decompressed_state)
     return booster
 
 
+_handle_key_name = (
+    "_handle" if lightgbm_version.major == 4 else "handle"  # noqa[PLR2004]
+)
+
+
 def _compress_booster_state(state: dict):
     """
     For a given state dictionary, store data in a structured format that can then
     be saved to disk in a way that can be compressed.
     """
     assert type(state) == dict
-    compressed_state = {k: v for k, v in state.items() if k != "handle"}
-    compressed_state["compressed_handle"] = _compress_booster_handle(state["handle"])
+    compressed_state = {k: v for k, v in state.items() if k != _handle_key_name}
+    compressed_state["compressed_handle"] = _compress_booster_handle(
+        state[_handle_key_name]
+    )
     return compressed_state
 
 
 def _decompress_booster_state(compressed_state: dict):
     assert type(compressed_state) == dict
     state = {k: v for k, v in compressed_state.items() if k != "compressed_handle"}
-    state["handle"] = _decompress_booster_handle(compressed_state["compressed_handle"])
+    state[_handle_key_name] = _decompress_booster_handle(
+        compressed_state["compressed_handle"]
+    )
     return state
 
 
 FRONT_STRING_REGEX = r"(?:\w+(?:=.*)?\n)*\n(?=Tree)"
 BACK_STRING_REGEX = r"end of trees(?:\n)+(?:.|\n)*"
 TREE_GROUP_REGEX = r"(Tree=\d+\n+)((?:.+\n)*)\n\n"
 
@@ -117,16 +130,18 @@
         int64_array = np.array(str_list, dtype=np.int64)
         return safe_cast(int64_array, dtype)
     assert np.can_cast(dtype, np.float64)
     return np.array(str_list, dtype=dtype)
 
 
 def _compress_booster_handle(model_string: str) -> Tuple[str, List[dict], str]:
-    if not model_string.startswith("tree\nversion=v3"):
-        raise ValueError("Only v3 is supported for the booster string format.")
+    if not model_string.startswith(f"tree\nversion=v{lightgbm_version.major}"):
+        raise ValueError(
+            f"Only v{lightgbm_version.major} is supported for the booster string format."
+        )
 
     front_str_match = re.search(FRONT_STRING_REGEX, model_string)
     if front_str_match is None:
         raise ValueError("Could not find front string.")
 
     # delete tree_sizes line since this messes up the tree parsing by LightGBM if not set correctly
     # todo calculate correct tree_sizes
```

### Comparing `slim_trees-0.2.2/slim_trees/pickling.py` & `slim_trees-0.2.3/slim_trees/pickling.py`

 * *Files identical despite different names*

### Comparing `slim_trees-0.2.2/.gitignore` & `slim_trees-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `slim_trees-0.2.2/LICENSE` & `slim_trees-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `slim_trees-0.2.2/README.md` & `slim_trees-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `slim_trees-0.2.2/pyproject.toml` & `slim_trees-0.2.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "slim-trees"
 description = "A python package for efficient pickling of ML models."
-version = "0.2.2"
+version = "0.2.3"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.8"
 authors = [
     { name = "Pavel Zwerschke", email = "pavel.zwerschke@quantco.com" },
 ]
 classifiers = [
@@ -21,18 +21,18 @@
 ]
 dependencies = [
     "numpy",
 ]
 
 [project.optional-dependencies]
 lightgbm = [
-    "lightgbm <4.0",
+    "lightgbm >=3.2,<4.1",
 ]
 scikit-learn = [
-    "scikit-learn <1.3.0",
+    "scikit-learn >=1.1.0,<1.4",
 ]
 
 [project.urls]
 Homepage = "https://github.com/quantco/slim-trees"
 
 [tool.hatch.build.targets.sdist]
 include = [
```

### Comparing `slim_trees-0.2.2/PKG-INFO` & `slim_trees-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: slim-trees
-Version: 0.2.2
+Version: 0.2.3
 Summary: A python package for efficient pickling of ML models.
 Project-URL: Homepage, https://github.com/quantco/slim-trees
 Author-email: Pavel Zwerschke <pavel.zwerschke@quantco.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: numpy
 Provides-Extra: lightgbm
-Requires-Dist: lightgbm<4.0; extra == 'lightgbm'
+Requires-Dist: lightgbm<4.1,>=3.2; extra == 'lightgbm'
 Provides-Extra: scikit-learn
-Requires-Dist: scikit-learn<1.3.0; extra == 'scikit-learn'
+Requires-Dist: scikit-learn<1.4,>=1.1.0; extra == 'scikit-learn'
 Description-Content-Type: text/markdown
 
 # Slim Trees
 
 [![CI](https://github.com/quantco/slim-trees/actions/workflows/ci.yml/badge.svg)](https://github.com/quantco/slim-trees/actions/workflows/ci.yml)
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/slim-trees?logoColor=white&logo=conda-forge)](https://anaconda.org/conda-forge/slim-trees)
 [![pypi-version](https://img.shields.io/pypi/v/slim-trees.svg?logo=pypi&logoColor=white)](https://pypi.org/project/slim-trees)
```

