# Comparing `tmp/magql-1.0.0.tar.gz` & `tmp/magql-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magql-1.0.0.tar", last modified: Mon Jul 24 15:57:06 2023, max compression
+gzip compressed data, was "magql-1.0.1.tar", last modified: Thu Jul 27 02:28:39 2023, max compression
```

## Comparing `magql-1.0.0.tar` & `magql-1.0.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     1264 2023-07-24 15:57:06.000000 magql-1.0.0/CHANGES.md
--rw-r--r--   0        0        0     1552 2023-07-24 15:57:06.000000 magql-1.0.0/LICENSE.md
--rw-r--r--   0        0        0      716 2023-07-24 15:57:06.000000 magql-1.0.0/README.md
--rw-r--r--   0        0        0   990900 2023-07-24 15:57:06.000000 magql-1.0.0/docs/_static/magql.png
--rw-r--r--   0        0        0      183 2023-07-24 15:57:06.000000 magql-1.0.0/docs/_static/theme.css
--rw-r--r--   0        0        0     1929 2023-07-24 15:57:06.000000 magql-1.0.0/docs/api.md
--rw-r--r--   0        0        0       48 2023-07-24 15:57:06.000000 magql-1.0.0/docs/changes.md
--rw-r--r--   0        0        0     1676 2023-07-24 15:57:06.000000 magql-1.0.0/docs/conf.py
--rw-r--r--   0        0        0      810 2023-07-24 15:57:06.000000 magql-1.0.0/docs/index.md
--rw-r--r--   0        0        0       31 2023-07-24 15:57:06.000000 magql-1.0.0/docs/license.md
--rw-r--r--   0        0        0     3079 2023-07-24 15:57:06.000000 magql-1.0.0/docs/references.md
--rw-r--r--   0        0        0     4495 2023-07-24 15:57:06.000000 magql-1.0.0/docs/resolvers.md
--rw-r--r--   0        0        0     2612 2023-07-24 15:57:06.000000 magql-1.0.0/docs/scalars.md
--rw-r--r--   0        0        0     8776 2023-07-24 15:57:06.000000 magql-1.0.0/docs/start.md
--rw-r--r--   0        0        0     8515 2023-07-24 15:57:06.000000 magql-1.0.0/docs/validation.md
--rw-r--r--   0        0        0     1194 2023-07-24 15:57:06.000000 magql-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       68 2023-07-24 15:57:06.000000 magql-1.0.0/requirements/dev.in
--rw-r--r--   0        0        0     1108 2023-07-24 15:57:06.000000 magql-1.0.0/requirements/dev.txt
--rw-r--r--   0        0        0       17 2023-07-24 15:57:06.000000 magql-1.0.0/requirements/docs.in
--rw-r--r--   0        0        0     1493 2023-07-24 15:57:06.000000 magql-1.0.0/requirements/docs.txt
--rw-r--r--   0        0        0       16 2023-07-24 15:57:06.000000 magql-1.0.0/requirements/tests.in
--rw-r--r--   0        0        0      343 2023-07-24 15:57:06.000000 magql-1.0.0/requirements/tests.txt
--rw-r--r--   0        0        0       42 2023-07-24 15:57:06.000000 magql-1.0.0/requirements/types.in
--rw-r--r--   0        0        0      661 2023-07-24 15:57:06.000000 magql-1.0.0/requirements/types.txt
--rw-r--r--   0        0        0     1003 2023-07-24 15:57:06.000000 magql-1.0.0/src/magql/__init__.py
--rw-r--r--   0        0        0     4072 2023-07-24 15:57:06.000000 magql-1.0.0/src/magql/check_delete.py
--rw-r--r--   0        0        0      606 2023-07-24 15:57:06.000000 magql-1.0.0/src/magql/filters.py
--rw-r--r--   0        0        0    38334 2023-07-24 15:57:06.000000 magql-1.0.0/src/magql/nodes.py
--rw-r--r--   0        0        0        0 2023-07-24 15:57:06.000000 magql-1.0.0/src/magql/py.typed
--rw-r--r--   0        0        0     4036 2023-07-24 15:57:06.000000 magql-1.0.0/src/magql/scalars.py
--rw-r--r--   0        0        0     8345 2023-07-24 15:57:06.000000 magql-1.0.0/src/magql/schema.py
--rw-r--r--   0        0        0     3537 2023-07-24 15:57:06.000000 magql-1.0.0/src/magql/search.py
--rw-r--r--   0        0        0     3850 2023-07-24 15:57:06.000000 magql-1.0.0/src/magql/validators.py
--rw-r--r--   0        0        0     4917 2023-07-24 15:57:06.000000 magql-1.0.0/tests/test_nodes.py
--rw-r--r--   0        0        0     1772 2023-07-24 15:57:06.000000 magql-1.0.0/tests/test_resolver.py
--rw-r--r--   0        0        0     2822 2023-07-24 15:57:06.000000 magql-1.0.0/tests/test_type_refs.py
--rw-r--r--   0        0        0     4659 2023-07-24 15:57:06.000000 magql-1.0.0/tests/test_validation/test_argument_validation.py
--rw-r--r--   0        0        0      692 2023-07-24 15:57:06.000000 magql-1.0.0/tox.ini
--rw-r--r--   0        0        0     1193 1970-01-01 00:00:00.000000 magql-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1389 2023-07-27 02:28:39.000000 magql-1.0.1/CHANGES.md
+-rw-r--r--   0        0        0     1552 2023-07-27 02:28:39.000000 magql-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0      716 2023-07-27 02:28:39.000000 magql-1.0.1/README.md
+-rw-r--r--   0        0        0   990900 2023-07-27 02:28:39.000000 magql-1.0.1/docs/_static/magql.png
+-rw-r--r--   0        0        0      183 2023-07-27 02:28:39.000000 magql-1.0.1/docs/_static/theme.css
+-rw-r--r--   0        0        0     1929 2023-07-27 02:28:39.000000 magql-1.0.1/docs/api.md
+-rw-r--r--   0        0        0       48 2023-07-27 02:28:39.000000 magql-1.0.1/docs/changes.md
+-rw-r--r--   0        0        0     1676 2023-07-27 02:28:39.000000 magql-1.0.1/docs/conf.py
+-rw-r--r--   0        0        0      810 2023-07-27 02:28:39.000000 magql-1.0.1/docs/index.md
+-rw-r--r--   0        0        0       31 2023-07-27 02:28:39.000000 magql-1.0.1/docs/license.md
+-rw-r--r--   0        0        0     3079 2023-07-27 02:28:39.000000 magql-1.0.1/docs/references.md
+-rw-r--r--   0        0        0     4495 2023-07-27 02:28:39.000000 magql-1.0.1/docs/resolvers.md
+-rw-r--r--   0        0        0     2612 2023-07-27 02:28:39.000000 magql-1.0.1/docs/scalars.md
+-rw-r--r--   0        0        0     8776 2023-07-27 02:28:39.000000 magql-1.0.1/docs/start.md
+-rw-r--r--   0        0        0     8515 2023-07-27 02:28:39.000000 magql-1.0.1/docs/validation.md
+-rw-r--r--   0        0        0     1194 2023-07-27 02:28:39.000000 magql-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-07-27 02:28:39.000000 magql-1.0.1/requirements/dev.in
+-rw-r--r--   0        0        0     1108 2023-07-27 02:28:39.000000 magql-1.0.1/requirements/dev.txt
+-rw-r--r--   0        0        0       17 2023-07-27 02:28:39.000000 magql-1.0.1/requirements/docs.in
+-rw-r--r--   0        0        0     1493 2023-07-27 02:28:39.000000 magql-1.0.1/requirements/docs.txt
+-rw-r--r--   0        0        0       16 2023-07-27 02:28:39.000000 magql-1.0.1/requirements/tests.in
+-rw-r--r--   0        0        0      343 2023-07-27 02:28:39.000000 magql-1.0.1/requirements/tests.txt
+-rw-r--r--   0        0        0       42 2023-07-27 02:28:39.000000 magql-1.0.1/requirements/types.in
+-rw-r--r--   0        0        0      661 2023-07-27 02:28:39.000000 magql-1.0.1/requirements/types.txt
+-rw-r--r--   0        0        0     1003 2023-07-27 02:28:39.000000 magql-1.0.1/src/magql/__init__.py
+-rw-r--r--   0        0        0     4072 2023-07-27 02:28:39.000000 magql-1.0.1/src/magql/check_delete.py
+-rw-r--r--   0        0        0      606 2023-07-27 02:28:39.000000 magql-1.0.1/src/magql/filters.py
+-rw-r--r--   0        0        0    38334 2023-07-27 02:28:39.000000 magql-1.0.1/src/magql/nodes.py
+-rw-r--r--   0        0        0        0 2023-07-27 02:28:39.000000 magql-1.0.1/src/magql/py.typed
+-rw-r--r--   0        0        0     4174 2023-07-27 02:28:39.000000 magql-1.0.1/src/magql/scalars.py
+-rw-r--r--   0        0        0     8345 2023-07-27 02:28:39.000000 magql-1.0.1/src/magql/schema.py
+-rw-r--r--   0        0        0     3537 2023-07-27 02:28:39.000000 magql-1.0.1/src/magql/search.py
+-rw-r--r--   0        0        0     3850 2023-07-27 02:28:39.000000 magql-1.0.1/src/magql/validators.py
+-rw-r--r--   0        0        0     4917 2023-07-27 02:28:39.000000 magql-1.0.1/tests/test_nodes.py
+-rw-r--r--   0        0        0     1772 2023-07-27 02:28:39.000000 magql-1.0.1/tests/test_resolver.py
+-rw-r--r--   0        0        0      894 2023-07-27 02:28:39.000000 magql-1.0.1/tests/test_scalars.py
+-rw-r--r--   0        0        0     2822 2023-07-27 02:28:39.000000 magql-1.0.1/tests/test_type_refs.py
+-rw-r--r--   0        0        0     4659 2023-07-27 02:28:39.000000 magql-1.0.1/tests/test_validation/test_argument_validation.py
+-rw-r--r--   0        0        0      692 2023-07-27 02:28:39.000000 magql-1.0.1/tox.ini
+-rw-r--r--   0        0        0     1193 1970-01-01 00:00:00.000000 magql-1.0.1/PKG-INFO
```

### Comparing `magql-1.0.0/CHANGES.md` & `magql-1.0.1/CHANGES.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Version 1.0.1
+-------------
+
+Released 2023-07-26
+
+-   Built-in scalar method overrides do not cause recursion. {issue}`88`
+
+
 Version 1.0.0
 -------------
 
 Released 2023-07-24
 
 -   Complete rewrite. {pr}`74`
```

### Comparing `magql-1.0.0/LICENSE.md` & `magql-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/README.md` & `magql-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/docs/_static/magql.png` & `magql-1.0.1/docs/_static/magql.png`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/docs/api.md` & `magql-1.0.1/docs/api.md`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/docs/conf.py` & `magql-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/docs/index.md` & `magql-1.0.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/docs/references.md` & `magql-1.0.1/docs/references.md`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/docs/resolvers.md` & `magql-1.0.1/docs/resolvers.md`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/docs/scalars.md` & `magql-1.0.1/docs/scalars.md`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/docs/start.md` & `magql-1.0.1/docs/start.md`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/docs/validation.md` & `magql-1.0.1/docs/validation.md`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/pyproject.toml` & `magql-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "magql"
-version = "1.0.0"
+version = "1.0.1"
 description = "The magical GraphQL framework that generates an API for your data."
 readme = "README.md"
 license = {file = "LICENSE.md"}
 authors = [{name = "David Lord", email = "davidism@gmail.com"}]
 requires-python = ">=3.10"
 dependencies = [
     "graphql-core>=3",
```

### Comparing `magql-1.0.0/requirements/dev.txt` & `magql-1.0.1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/requirements/docs.txt` & `magql-1.0.1/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/requirements/types.txt` & `magql-1.0.1/requirements/types.txt`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/src/magql/__init__.py` & `magql-1.0.1/src/magql/__init__.py`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/src/magql/check_delete.py` & `magql-1.0.1/src/magql/check_delete.py`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/src/magql/filters.py` & `magql-1.0.1/src/magql/filters.py`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/src/magql/nodes.py` & `magql-1.0.1/src/magql/nodes.py`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/src/magql/scalars.py` & `magql-1.0.1/src/magql/scalars.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,61 +21,64 @@
 def parse_int(value: t.Any) -> t.Any:
     if isinstance(value, str):
         try:
             value = int(value)
         except ValueError:
             pass
 
-    return graphql.GraphQLInt.parse_value(value)
+    return _original_parse_int(value)
 
 
 Int: Scalar = Scalar("Int")
 """Built-in GraphQL ``Int`` type. Extends GraphQL-Core implementation to accept string
 values. Strings are common when using HTML forms.
 """
 Int._graphql_node = graphql.GraphQLInt
+_original_parse_int = graphql.GraphQLInt.parse_value
 graphql.GraphQLInt.parse_value = parse_int  # type: ignore[method-assign]
 
 
 def parse_float(value: t.Any) -> t.Any:
     if isinstance(value, str):
         try:
             value = float(value)
         except ValueError:
             pass
 
-    return graphql.GraphQLFloat.parse_value(value)
+    return _original_parse_float(value)
 
 
 Float: Scalar = Scalar("Float")
 """Built-in GraphQL ``Float`` type. Extends GraphQL-Core implementation to accept string
 values. Strings are common when using HTML forms.
 """
 Float._graphql_node = graphql.GraphQLFloat
+_original_parse_float = graphql.GraphQLFloat.parse_value
 graphql.GraphQLFloat.parse_value = parse_float  # type: ignore[method-assign]
 
 
 def parse_boolean(value: t.Any) -> t.Any:
     if isinstance(value, str):
         v = value.lower()
 
         if v in {"1", "on", "true"}:
             value = True
         elif v in {"0", "off", "false"}:
             value = False
 
-    return graphql.GraphQLBoolean.parse_value(value)
+    return _original_parse_boolean(value)
 
 
 Boolean: Scalar = Scalar("Boolean")
 """Built-in GraphQL ``Boolean`` type. Extends GraphQL-Core implementation to accept
 common case-insensitive string values; 1, on, true; 0, off, false. In particular, HTML
 forms send "on".
 """
 Boolean._graphql_node = graphql.GraphQLBoolean
+_original_parse_boolean = graphql.GraphQLBoolean.parse_value
 graphql.GraphQLBoolean.parse_value = parse_boolean  # type: ignore[method-assign]
 
 ID: Scalar = Scalar("ID")
 """Built-in GraphQL ``ID`` type. Accepts strings, ints, and floats, converting them all
 to strings.
 """
 ID._graphql_node = graphql.GraphQLID
```

### Comparing `magql-1.0.0/src/magql/schema.py` & `magql-1.0.1/src/magql/schema.py`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/src/magql/search.py` & `magql-1.0.1/src/magql/search.py`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/src/magql/validators.py` & `magql-1.0.1/src/magql/validators.py`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/tests/test_nodes.py` & `magql-1.0.1/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/tests/test_resolver.py` & `magql-1.0.1/tests/test_resolver.py`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/tests/test_type_refs.py` & `magql-1.0.1/tests/test_type_refs.py`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/tests/test_validation/test_argument_validation.py` & `magql-1.0.1/tests/test_validation/test_argument_validation.py`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/tox.ini` & `magql-1.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `magql-1.0.0/PKG-INFO` & `magql-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magql
-Version: 1.0.0
+Version: 1.0.1
 Summary: The magical GraphQL framework that generates an API for your data.
 Author-email: David Lord <davidism@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: graphql-core>=3
 Requires-Dist: python-dateutil
 Project-URL: Changes, https://magql.autoinvent.dev/changes.html
```

