# Comparing `tmp/simpleindex-0.6.0.tar.gz` & `tmp/simpleindex-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleindex-0.6.0.tar", last modified: Wed Jan 18 08:09:07 2023, max compression
+gzip compressed data, was "simpleindex-0.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `simpleindex-0.6.0.tar` & `simpleindex-0.6.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       35 2022-12-13 08:36:34.732210 simpleindex-0.6.0/.gitignore
--rw-r--r--   0        0        0     1081 2022-12-13 08:36:34.732279 simpleindex-0.6.0/LICENSE
--rw-r--r--   0        0        0     2428 2022-12-13 08:36:34.732352 simpleindex-0.6.0/README.md
--rw-r--r--   0        0        0      734 2023-01-18 08:06:10.774035 simpleindex-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      161 2023-01-18 08:08:17.267507 simpleindex-0.6.0/src/simpleindex/__init__.py
--rw-r--r--   0        0        0     1708 2023-01-18 08:06:10.774980 simpleindex-0.6.0/src/simpleindex/__main__.py
--rw-r--r--   0        0        0     2465 2023-01-18 08:06:10.775099 simpleindex-0.6.0/src/simpleindex/configs.py
--rw-r--r--   0        0        0     3950 2023-01-18 08:06:10.775608 simpleindex-0.6.0/src/simpleindex/routes.py
--rw-r--r--   0        0        0        0 2022-12-13 08:36:34.732827 simpleindex-0.6.0/tests/examples/__init__.py
--rw-r--r--   0        0        0      916 2022-12-13 08:36:34.732898 simpleindex-0.6.0/tests/examples/annotated.toml
--rw-r--r--   0        0        0     1972 2023-01-18 08:06:10.775716 simpleindex-0.6.0/tests/test_build_routes.py
--rw-r--r--   0        0        0     1345 2023-01-18 08:06:10.775933 simpleindex-0.6.0/tests/test_configs.py
--rw-r--r--   0        0        0     2841 2023-01-18 08:06:10.776269 simpleindex-0.6.0/tests/test_routes.py
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 simpleindex-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       35 2022-12-13 08:36:34.732210 simpleindex-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1081 2022-12-13 08:36:34.732279 simpleindex-0.6.1/LICENSE
+-rw-r--r--   0        0        0     2429 2023-07-27 08:09:14.455559 simpleindex-0.6.1/README.md
+-rw-r--r--   0        0        0      734 2023-01-18 08:06:10.774035 simpleindex-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      268 2023-07-27 08:11:14.715102 simpleindex-0.6.1/src/simpleindex/__init__.py
+-rw-r--r--   0        0        0     1708 2023-01-18 08:06:10.774980 simpleindex-0.6.1/src/simpleindex/__main__.py
+-rw-r--r--   0        0        0     2787 2023-07-27 08:07:02.955604 simpleindex-0.6.1/src/simpleindex/configs.py
+-rw-r--r--   0        0        0     3950 2023-01-18 08:06:10.775608 simpleindex-0.6.1/src/simpleindex/routes.py
+-rw-r--r--   0        0        0        0 2022-12-13 08:36:34.732827 simpleindex-0.6.1/tests/examples/__init__.py
+-rw-r--r--   0        0        0      916 2022-12-13 08:36:34.732898 simpleindex-0.6.1/tests/examples/annotated.toml
+-rw-r--r--   0        0        0     1972 2023-01-18 08:06:10.775716 simpleindex-0.6.1/tests/test_build_routes.py
+-rw-r--r--   0        0        0     1345 2023-01-18 08:06:10.775933 simpleindex-0.6.1/tests/test_configs.py
+-rw-r--r--   0        0        0     2841 2023-01-18 08:06:10.776269 simpleindex-0.6.1/tests/test_routes.py
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 simpleindex-0.6.1/PKG-INFO
```

### Comparing `simpleindex-0.6.0/LICENSE` & `simpleindex-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleindex-0.6.0/README.md` & `simpleindex-0.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 [entry point]: https://setuptools.readthedocs.io/en/latest/userguide/entry_point.html#advertising-behavior
 
 A new route type should subclass `simpleindex.routes.Route`, and implement behaviour to respond to HTTP requests.
 
 The `Route` instance has two attributes:
 
 * `root`: A `pathlib.Path` pointing to the directory containing the configuration file current being served.
-* `to`: The `to` string in the configuratio block.
+* `to`: The `to` string in the configuration block.
 
 For example, here's how you might want to implement Amazon S3 support:
 
 ```python
 # simpleindex_s3.py
 
 from simpleindex.routes import Response, Route
```

### Comparing `simpleindex-0.6.0/pyproject.toml` & `simpleindex-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simpleindex-0.6.0/src/simpleindex/__main__.py` & `simpleindex-0.6.1/src/simpleindex/__main__.py`

 * *Files identical despite different names*

### Comparing `simpleindex-0.6.0/src/simpleindex/configs.py` & `simpleindex-0.6.1/src/simpleindex/configs.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import dataclasses
 import functools
 import importlib.metadata
 import pathlib
 import typing
 
 import pydantic
+import pydantic_core.core_schema as core_schema
 import toml
 
 from .routes import Route
 
 
 class ConfigurationFileNotFound(ValueError):
     def __init__(self, loc: str) -> None:
@@ -33,32 +34,39 @@
 
 @functools.lru_cache(maxsize=None)
 def _get_route_source_choices() -> typing.Dict[str, typing.Type[Route]]:
     entry_points = importlib.metadata.entry_points()
     return {ep.name: ep.load() for ep in entry_points.get("simpleindex.routes", [])}
 
 
-def _validate_route_source(v: typing.Union[str, _RouteSource]) -> _RouteSource:
+def _validate_route_source(
+    v: typing.Union[str, _RouteSource],
+    _: typing.Optional[core_schema.ValidationInfo] = None,
+) -> _RouteSource:
     if isinstance(v, _RouteSource):
         return v
     try:
         return _RouteSource(name=v, value=_get_route_source_choices()[v])
     except KeyError:
         raise ValueError(v)
 
 
 @dataclasses.dataclass()
 class _RouteSource:
     name: str
     value: typing.Type[Route]
 
     @classmethod
-    def __get_validators__(cls):
+    def __get_validators__(cls):  # Pydantic 1.x compatibility.
         yield _validate_route_source
 
+    @classmethod
+    def __get_pydantic_core_schema__(cls, source, handler):  # Pydantic 2.
+        return core_schema.general_plain_validator_function(_validate_route_source)
+
 
 class _Route(pydantic.BaseModel):
     source: _RouteSource
     to: str
 
     def derive(self, root: pathlib.Path) -> Route:
         return self.source.value(root=root, to=self.to)
```

### Comparing `simpleindex-0.6.0/src/simpleindex/routes.py` & `simpleindex-0.6.1/src/simpleindex/routes.py`

 * *Files identical despite different names*

### Comparing `simpleindex-0.6.0/tests/examples/annotated.toml` & `simpleindex-0.6.1/tests/examples/annotated.toml`

 * *Files identical despite different names*

### Comparing `simpleindex-0.6.0/tests/test_build_routes.py` & `simpleindex-0.6.1/tests/test_build_routes.py`

 * *Files identical despite different names*

### Comparing `simpleindex-0.6.0/tests/test_configs.py` & `simpleindex-0.6.1/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `simpleindex-0.6.0/tests/test_routes.py` & `simpleindex-0.6.1/tests/test_routes.py`

 * *Files identical despite different names*

### Comparing `simpleindex-0.6.0/PKG-INFO` & `simpleindex-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleindex
-Version: 0.6.0
+Version: 0.6.1
 Summary: PEP 503 Simple Repository index by declaring routing rules.
 Home-page: https://github.com/uranusjr/simpleindex
 Author: Tzu-ping Chung
 Author-email: uranusjr@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: packaging >=20.9
```

