# Comparing `tmp/simpleindex-0.6.1.tar.gz` & `tmp/simpleindex-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleindex-0.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "simpleindex-0.6.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `simpleindex-0.6.1.tar` & `simpleindex-0.6.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       35 2022-12-13 08:36:34.732210 simpleindex-0.6.1/.gitignore
--rw-r--r--   0        0        0     1081 2022-12-13 08:36:34.732279 simpleindex-0.6.1/LICENSE
--rw-r--r--   0        0        0     2429 2023-07-27 08:09:14.455559 simpleindex-0.6.1/README.md
--rw-r--r--   0        0        0      734 2023-01-18 08:06:10.774035 simpleindex-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      268 2023-07-27 08:11:14.715102 simpleindex-0.6.1/src/simpleindex/__init__.py
--rw-r--r--   0        0        0     1708 2023-01-18 08:06:10.774980 simpleindex-0.6.1/src/simpleindex/__main__.py
--rw-r--r--   0        0        0     2787 2023-07-27 08:07:02.955604 simpleindex-0.6.1/src/simpleindex/configs.py
--rw-r--r--   0        0        0     3950 2023-01-18 08:06:10.775608 simpleindex-0.6.1/src/simpleindex/routes.py
--rw-r--r--   0        0        0        0 2022-12-13 08:36:34.732827 simpleindex-0.6.1/tests/examples/__init__.py
--rw-r--r--   0        0        0      916 2022-12-13 08:36:34.732898 simpleindex-0.6.1/tests/examples/annotated.toml
--rw-r--r--   0        0        0     1972 2023-01-18 08:06:10.775716 simpleindex-0.6.1/tests/test_build_routes.py
--rw-r--r--   0        0        0     1345 2023-01-18 08:06:10.775933 simpleindex-0.6.1/tests/test_configs.py
--rw-r--r--   0        0        0     2841 2023-01-18 08:06:10.776269 simpleindex-0.6.1/tests/test_routes.py
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 simpleindex-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0       35 2022-12-13 08:36:34.732210 simpleindex-0.6.2/.gitignore
+-rw-r--r--   0        0        0     1081 2022-12-13 08:36:34.732279 simpleindex-0.6.2/LICENSE
+-rw-r--r--   0        0        0     2429 2023-07-27 08:09:14.455559 simpleindex-0.6.2/README.md
+-rw-r--r--   0        0        0      734 2023-01-18 08:06:10.774035 simpleindex-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      268 2023-07-27 08:14:00.540919 simpleindex-0.6.2/src/simpleindex/__init__.py
+-rw-r--r--   0        0        0     1708 2023-01-18 08:06:10.774980 simpleindex-0.6.2/src/simpleindex/__main__.py
+-rw-r--r--   0        0        0     2796 2023-07-27 08:13:41.617015 simpleindex-0.6.2/src/simpleindex/configs.py
+-rw-r--r--   0        0        0     3950 2023-01-18 08:06:10.775608 simpleindex-0.6.2/src/simpleindex/routes.py
+-rw-r--r--   0        0        0        0 2022-12-13 08:36:34.732827 simpleindex-0.6.2/tests/examples/__init__.py
+-rw-r--r--   0        0        0      916 2022-12-13 08:36:34.732898 simpleindex-0.6.2/tests/examples/annotated.toml
+-rw-r--r--   0        0        0     1972 2023-01-18 08:06:10.775716 simpleindex-0.6.2/tests/test_build_routes.py
+-rw-r--r--   0        0        0     1345 2023-01-18 08:06:10.775933 simpleindex-0.6.2/tests/test_configs.py
+-rw-r--r--   0        0        0     2841 2023-01-18 08:06:10.776269 simpleindex-0.6.2/tests/test_routes.py
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 simpleindex-0.6.2/PKG-INFO
```

### Comparing `simpleindex-0.6.1/LICENSE` & `simpleindex-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleindex-0.6.1/README.md` & `simpleindex-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `simpleindex-0.6.1/pyproject.toml` & `simpleindex-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simpleindex-0.6.1/src/simpleindex/__main__.py` & `simpleindex-0.6.2/src/simpleindex/__main__.py`

 * *Files identical despite different names*

### Comparing `simpleindex-0.6.1/src/simpleindex/configs.py` & `simpleindex-0.6.2/src/simpleindex/configs.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import dataclasses
 import functools
 import importlib.metadata
 import pathlib
 import typing
 
 import pydantic
-import pydantic_core.core_schema as core_schema
 import toml
 
 from .routes import Route
 
 
 class ConfigurationFileNotFound(ValueError):
     def __init__(self, loc: str) -> None:
@@ -57,14 +56,16 @@
 
     @classmethod
     def __get_validators__(cls):  # Pydantic 1.x compatibility.
         yield _validate_route_source
 
     @classmethod
     def __get_pydantic_core_schema__(cls, source, handler):  # Pydantic 2.
+        import pydantic_core.core_schema as core_schema
+
         return core_schema.general_plain_validator_function(_validate_route_source)
 
 
 class _Route(pydantic.BaseModel):
     source: _RouteSource
     to: str
```

### Comparing `simpleindex-0.6.1/src/simpleindex/routes.py` & `simpleindex-0.6.2/src/simpleindex/routes.py`

 * *Files identical despite different names*

### Comparing `simpleindex-0.6.1/tests/examples/annotated.toml` & `simpleindex-0.6.2/tests/examples/annotated.toml`

 * *Files identical despite different names*

### Comparing `simpleindex-0.6.1/tests/test_build_routes.py` & `simpleindex-0.6.2/tests/test_build_routes.py`

 * *Files identical despite different names*

### Comparing `simpleindex-0.6.1/tests/test_configs.py` & `simpleindex-0.6.2/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `simpleindex-0.6.1/tests/test_routes.py` & `simpleindex-0.6.2/tests/test_routes.py`

 * *Files identical despite different names*

### Comparing `simpleindex-0.6.1/PKG-INFO` & `simpleindex-0.6.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleindex
-Version: 0.6.1
+Version: 0.6.2
 Summary: PEP 503 Simple Repository index by declaring routing rules.
 Home-page: https://github.com/uranusjr/simpleindex
 Author: Tzu-ping Chung
 Author-email: uranusjr@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: packaging >=20.9
```

