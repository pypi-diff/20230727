# Comparing `tmp/aiohttp_deps-0.3.1.tar.gz` & `tmp/aiohttp_deps-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp_deps-0.3.1.tar", max compression
+gzip compressed data, was "aiohttp_deps-0.3.2.tar", max compression
```

## Comparing `aiohttp_deps-0.3.1.tar` & `aiohttp_deps-0.3.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-07-26 11:11:47.779408 aiohttp_deps-0.3.1/LICENSE
--rw-r--r--   0        0        0     9687 2023-07-26 11:11:47.779408 aiohttp_deps-0.3.1/README.md
--rw-r--r--   0        0        0      539 2023-07-26 11:11:47.779408 aiohttp_deps-0.3.1/aiohttp_deps/__init__.py
--rw-r--r--   0        0        0     3265 2023-07-26 11:11:47.779408 aiohttp_deps-0.3.1/aiohttp_deps/initializer.py
--rw-r--r--   0        0        0        0 2023-07-26 11:11:47.779408 aiohttp_deps-0.3.1/aiohttp_deps/py.typed
--rw-r--r--   0        0        0     1250 2023-07-26 11:11:47.779408 aiohttp_deps-0.3.1/aiohttp_deps/router.py
--rw-r--r--   0        0        0      898 2023-07-26 11:11:47.779408 aiohttp_deps-0.3.1/aiohttp_deps/router.pyi
--rw-r--r--   0        0        0    12061 2023-07-26 11:11:47.779408 aiohttp_deps-0.3.1/aiohttp_deps/swagger.py
--rw-r--r--   0        0        0    10950 2023-07-26 11:11:47.779408 aiohttp_deps-0.3.1/aiohttp_deps/utils.py
--rw-r--r--   0        0        0     1385 2023-07-26 11:11:47.779408 aiohttp_deps-0.3.1/aiohttp_deps/view.py
--rw-r--r--   0        0        0     1784 2023-07-26 11:11:47.779408 aiohttp_deps-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    10841 1970-01-01 00:00:00.000000 aiohttp_deps-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-27 05:55:49.767371 aiohttp_deps-0.3.2/LICENSE
+-rw-r--r--   0        0        0     9687 2023-07-27 05:55:49.767371 aiohttp_deps-0.3.2/README.md
+-rw-r--r--   0        0        0      539 2023-07-27 05:55:49.767371 aiohttp_deps-0.3.2/aiohttp_deps/__init__.py
+-rw-r--r--   0        0        0     3265 2023-07-27 05:55:49.767371 aiohttp_deps-0.3.2/aiohttp_deps/initializer.py
+-rw-r--r--   0        0        0        0 2023-07-27 05:55:49.767371 aiohttp_deps-0.3.2/aiohttp_deps/py.typed
+-rw-r--r--   0        0        0     1250 2023-07-27 05:55:49.767371 aiohttp_deps-0.3.2/aiohttp_deps/router.py
+-rw-r--r--   0        0        0      898 2023-07-27 05:55:49.767371 aiohttp_deps-0.3.2/aiohttp_deps/router.pyi
+-rw-r--r--   0        0        0    13031 2023-07-27 05:55:49.767371 aiohttp_deps-0.3.2/aiohttp_deps/swagger.py
+-rw-r--r--   0        0        0    10950 2023-07-27 05:55:49.767371 aiohttp_deps-0.3.2/aiohttp_deps/utils.py
+-rw-r--r--   0        0        0     1385 2023-07-27 05:55:49.767371 aiohttp_deps-0.3.2/aiohttp_deps/view.py
+-rw-r--r--   0        0        0     1784 2023-07-27 05:55:49.771371 aiohttp_deps-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    10841 1970-01-01 00:00:00.000000 aiohttp_deps-0.3.2/PKG-INFO
```

### Comparing `aiohttp_deps-0.3.1/LICENSE` & `aiohttp_deps-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.3.1/README.md` & `aiohttp_deps-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.3.1/aiohttp_deps/__init__.py` & `aiohttp_deps-0.3.2/aiohttp_deps/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.3.1/aiohttp_deps/initializer.py` & `aiohttp_deps-0.3.2/aiohttp_deps/initializer.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.3.1/aiohttp_deps/router.py` & `aiohttp_deps-0.3.2/aiohttp_deps/router.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.3.1/aiohttp_deps/router.pyi` & `aiohttp_deps-0.3.2/aiohttp_deps/router.pyi`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.3.1/aiohttp_deps/swagger.py` & `aiohttp_deps-0.3.2/aiohttp_deps/swagger.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,14 +81,25 @@
     def dummy(_var: annotation.annotation) -> None:  # type: ignore
         """Dummy function to use for type resolution."""
 
     var = get_type_hints(dummy).get("_var")
     return var == Optional[var]
 
 
+def _get_param_schema(annotation: Optional[inspect.Parameter]) -> Dict[str, Any]:
+    if annotation is None or annotation.annotation == annotation.empty:
+        return {}
+
+    def dummy(_var: annotation.annotation) -> None:  # type: ignore
+        """Dummy function to use for type resolution."""
+
+    var = get_type_hints(dummy).get("_var")
+    return pydantic.TypeAdapter(var).json_schema(ref_template=REF_TEMPLATE)
+
+
 def _add_route_def(  # noqa: C901, WPS210, WPS211
     openapi_schema: Dict[str, Any],
     route: web.ResourceRoute,
     method: str,
     graph: DependencyGraph,
     extra_openapi: Dict[str, Any],
     extra_openapi_schemas: Dict[str, Any],
@@ -136,40 +147,49 @@
                     "content": {content_type: {"schema": input_schema}},
                 }
             else:
                 route_info["requestBody"] = {
                     "content": {content_type: {}},
                 }
         elif isinstance(dependency.dependency, Query):
+            schema = _get_param_schema(dependency.signature)
+            openapi_schema["components"]["schemas"].update(schema.pop("$defs", {}))
             _insert_in_params(
                 {
                     "name": dependency.dependency.alias or dependency.param_name,
                     "in": "query",
                     "description": dependency.dependency.description,
                     "required": not _is_optional(dependency.signature),
+                    "schema": schema,
                 },
             )
         elif isinstance(dependency.dependency, Header):
             name = dependency.dependency.alias or dependency.param_name
+            schema = _get_param_schema(dependency.signature)
+            openapi_schema["components"]["schemas"].update(schema.pop("$defs", {}))
             _insert_in_params(
                 {
                     "name": name.capitalize(),
                     "in": "header",
                     "description": dependency.dependency.description,
                     "required": not _is_optional(dependency.signature),
+                    "schema": schema,
                 },
             )
         elif isinstance(dependency.dependency, Path):
+            schema = _get_param_schema(dependency.signature)
+            openapi_schema["components"]["schemas"].update(schema.pop("$defs", {}))
             _insert_in_params(
                 {
                     "name": dependency.dependency.alias or dependency.param_name,
                     "in": "path",
                     "description": dependency.dependency.description,
                     "required": not _is_optional(dependency.signature),
                     "allowEmptyValue": _is_optional(dependency.signature),
+                    "schema": schema,
                 },
             )
 
     route_info["parameters"] = list(params.values())
     openapi_schema["paths"][route.resource.canonical].update(
         {method.lower(): always_merger.merge(route_info, extra_openapi)},
     )
```

### Comparing `aiohttp_deps-0.3.1/aiohttp_deps/utils.py` & `aiohttp_deps-0.3.2/aiohttp_deps/utils.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.3.1/aiohttp_deps/view.py` & `aiohttp_deps-0.3.2/aiohttp_deps/view.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.3.1/pyproject.toml` & `aiohttp_deps-0.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "aiohttp-deps"
 description = "Dependency injection for AioHTTP"
 authors = ["Taskiq team <taskiq@no-reply.com>"]
 maintainers = ["Taskiq team <taskiq@no-reply.com>"]
-version = "0.3.1"
+version = "0.3.2"
 readme = "README.md"
 license = "LICENSE"
 classifiers = [
     "Typing :: Typed",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `aiohttp_deps-0.3.1/PKG-INFO` & `aiohttp_deps-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp-deps
-Version: 0.3.1
+Version: 0.3.2
 Summary: Dependency injection for AioHTTP
 Home-page: https://github.com/taskiq-python/aiohttp-deps
 License: LICENSE
 Keywords: aiohttp,taskiq-dependencies
 Author: Taskiq team
 Author-email: taskiq@no-reply.com
 Maintainer: Taskiq team
```

