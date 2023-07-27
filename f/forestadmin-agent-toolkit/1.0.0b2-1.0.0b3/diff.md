# Comparing `tmp/forestadmin_agent_toolkit-1.0.0b2.tar.gz` & `tmp/forestadmin_agent_toolkit-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_agent_toolkit-1.0.0b2.tar", max compression
+gzip compressed data, was "forestadmin_agent_toolkit-1.0.0b3.tar", max compression
```

## Comparing `forestadmin_agent_toolkit-1.0.0b2.tar` & `forestadmin_agent_toolkit-1.0.0b3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0        0 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/README.md
--rw-r--r--   0        0        0        0 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/__init__.py
--rw-r--r--   0        0        0     4908 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/agent.py
--rw-r--r--   0        0        0      135 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/exceptions.py
--rw-r--r--   0        0        0      628 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/options.py
--rw-r--r--   0        0        0        0 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/actions/__init__.py
--rw-r--r--   0        0        0     2292 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/actions/requests.py
--rw-r--r--   0        0        0     5964 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/actions/resources.py
--rw-r--r--   0        0        0      464 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/base.py
--rw-r--r--   0        0        0      913 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/collections/__init__.py
--rw-r--r--   0        0        0     2494 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/collections/charts_collection.py
--rw-r--r--   0        0        0     1708 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/collections/charts_datasource.py
--rw-r--r--   0        0        0    15947 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/collections/crud.py
--rw-r--r--   0        0        0    19417 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/collections/crud_related.py
--rw-r--r--   0        0        0     2966 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/collections/decorators.py
--rw-r--r--   0        0        0      148 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/collections/exceptions.py
--rw-r--r--   0        0        0    11045 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/collections/filter.py
--rw-r--r--   0        0        0     5624 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/collections/requests.py
--rw-r--r--   0        0        0     9466 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/collections/stats.py
--rw-r--r--   0        0        0        0 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/security/__init__.py
--rw-r--r--   0        0        0      144 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/security/exceptions.py
--rw-r--r--   0        0        0     3763 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/security/resources.py
--rw-r--r--   0        0        0        0 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/services/__init__.py
--rw-r--r--   0        0        0     8403 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/services/permissions/__init__.py
--rw-r--r--   0        0        0      264 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/services/permissions/options.py
--rw-r--r--   0        0        0     1660 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/services/serializers/__init__.py
--rw-r--r--   0        0        0     9523 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/services/serializers/json_api.py
--rw-r--r--   0        0        0        0 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/__init__.py
--rw-r--r--   0        0        0     3227 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/authentication.py
--rw-r--r--   0        0        0     2266 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/context.py
--rw-r--r--   0        0        0     1392 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/csv.py
--rw-r--r--   0        0        0        0 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/forest_schema/__init__.py
--rw-r--r--   0        0        0     3039 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/forest_schema/action_values.py
--rw-r--r--   0        0        0     4308 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/forest_schema/emitter.py
--rw-r--r--   0        0        0     2236 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/forest_schema/filterable.py
--rw-r--r--   0        0        0     4508 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py
--rw-r--r--   0        0        0     2288 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py
--rw-r--r--   0        0        0     7847 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py
--rw-r--r--   0        0        0      506 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/forest_schema/generator_segment.py
--rw-r--r--   0        0        0     3057 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/forest_schema/type.py
--rw-r--r--   0        0        0     1281 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/forest_schema/validation.py
--rw-r--r--   0        0        0     4019 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/http.py
--rw-r--r--   0        0        0     1683 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/id.py
--rw-r--r--   0        0        0      541 2023-07-26 13:24:28.433169 forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/token.py
--rw-r--r--   0        0        0     1771 2023-07-26 13:24:46.557273 forestadmin_agent_toolkit-1.0.0b2/pyproject.toml
--rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 forestadmin_agent_toolkit-1.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/__init__.py
+-rw-r--r--   0        0        0     4908 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/agent.py
+-rw-r--r--   0        0        0      135 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/exceptions.py
+-rw-r--r--   0        0        0      628 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/options.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/actions/__init__.py
+-rw-r--r--   0        0        0     2292 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/actions/requests.py
+-rw-r--r--   0        0        0     6127 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/actions/resources.py
+-rw-r--r--   0        0        0      464 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/base.py
+-rw-r--r--   0        0        0      913 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/__init__.py
+-rw-r--r--   0        0        0     2494 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/charts_collection.py
+-rw-r--r--   0        0        0     1708 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/charts_datasource.py
+-rw-r--r--   0        0        0    15947 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/crud.py
+-rw-r--r--   0        0        0    19417 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/crud_related.py
+-rw-r--r--   0        0        0     2966 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/decorators.py
+-rw-r--r--   0        0        0      148 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/exceptions.py
+-rw-r--r--   0        0        0    11045 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/filter.py
+-rw-r--r--   0        0        0     5624 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/requests.py
+-rw-r--r--   0        0        0     9466 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/stats.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/security/__init__.py
+-rw-r--r--   0        0        0      144 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/security/exceptions.py
+-rw-r--r--   0        0        0     3763 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/security/resources.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/services/__init__.py
+-rw-r--r--   0        0        0     8403 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/services/permissions/__init__.py
+-rw-r--r--   0        0        0      264 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/services/permissions/options.py
+-rw-r--r--   0        0        0     1660 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/services/serializers/__init__.py
+-rw-r--r--   0        0        0     9523 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/services/serializers/json_api.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/__init__.py
+-rw-r--r--   0        0        0     3227 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/authentication.py
+-rw-r--r--   0        0        0     2266 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/context.py
+-rw-r--r--   0        0        0     1392 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/csv.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/__init__.py
+-rw-r--r--   0        0        0     3039 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/action_values.py
+-rw-r--r--   0        0        0     4308 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/emitter.py
+-rw-r--r--   0        0        0     2236 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/filterable.py
+-rw-r--r--   0        0        0     4508 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py
+-rw-r--r--   0        0        0     2288 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py
+-rw-r--r--   0        0        0     7847 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py
+-rw-r--r--   0        0        0      506 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/generator_segment.py
+-rw-r--r--   0        0        0     3057 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/type.py
+-rw-r--r--   0        0        0     1281 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/validation.py
+-rw-r--r--   0        0        0     4019 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/http.py
+-rw-r--r--   0        0        0     1683 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/id.py
+-rw-r--r--   0        0        0      541 2023-07-27 12:28:59.063672 forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/token.py
+-rw-r--r--   0        0        0     1771 2023-07-27 12:29:17.163636 forestadmin_agent_toolkit-1.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 forestadmin_agent_toolkit-1.0.0b3/PKG-INFO
```

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/agent.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/agent.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/options.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/options.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/actions/requests.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/actions/requests.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/actions/resources.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/actions/resources.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,15 +85,21 @@
             .get("fields", [])  # type: ignore
         )
         data: Optional[Dict[str, Any]] = None
         if forest_fields:
             data = ForestValueConverter.make_form_data_from_fields(request.collection.datasource, forest_fields)
 
         _filter = await self._get_records_selection(request)
-        fields = await request.collection.get_form(request.user, request.action_name, data, _filter)
+        fields = await request.collection.get_form(
+            request.user,
+            request.action_name,
+            data,
+            _filter,
+            {"changed_field": request.body.get("data", {}).get("attributes", {}).get("changed_field")},
+        )
 
         return build_success_response(
             {
                 "fields": [
                     await SchemaActionGenerator.build_field_schema(request.collection.datasource, field)
                     for field in fields
                 ]
```

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/collections/__init__.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/collections/charts_collection.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/charts_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/collections/charts_datasource.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/charts_datasource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/collections/crud.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/crud.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/collections/crud_related.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/crud_related.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/collections/decorators.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/decorators.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/collections/filter.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/filter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/collections/requests.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/requests.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/collections/stats.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/collections/stats.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/resources/security/resources.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/resources/security/resources.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/services/permissions/__init__.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/services/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/services/serializers/__init__.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/services/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/services/serializers/json_api.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/services/serializers/json_api.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/authentication.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/authentication.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/context.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/csv.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/csv.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/forest_schema/action_values.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/action_values.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/forest_schema/emitter.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/emitter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/forest_schema/filterable.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/filterable.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/forest_schema/type.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/type.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/forest_schema/validation.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/forest_schema/validation.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/http.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/http.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/id.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/id.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/forestadmin/agent_toolkit/utils/token.py` & `forestadmin_agent_toolkit-1.0.0b3/forestadmin/agent_toolkit/utils/token.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b2/pyproject.toml` & `forestadmin_agent_toolkit-1.0.0b3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-agent-toolkit"
-version = "1.0.0-beta.2"
+version = "1.0.0-beta.3"
 description = ""
 authors = [ "Valentin Monté <valentinm@forestadmin.com>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "forestadmin"
 
 [tool.poetry.dependencies]
@@ -16,15 +16,15 @@
 typing-extensions = ">=4.2.0, <5.0"
 tzdata = "~2022.6"
 aiohttp = "~=3.8"
 oic = "~=1.4"
 python-jose = ">=3.3, <4.0"
 cachetools = "~=5.2"
 marshmallow-jsonapi = ">=0.24.0, <1.0"
-forestadmin-datasource-toolkit = "^1.0.0-beta.2"
+forestadmin-datasource-toolkit = "^1.0.0-beta.3"
 [[tool.poetry.dependencies.pandas]]
 version = "<=1.1.5"
 python = "<3.7.1"
 
 [[tool.poetry.dependencies.pandas]]
 version = ">=1.3.4,<=1.3.5"
 python = ">=3.7.1,<3.8"
```

### Comparing `forestadmin_agent_toolkit-1.0.0b2/PKG-INFO` & `forestadmin_agent_toolkit-1.0.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: forestadmin-agent-toolkit
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: 
 Author: Valentin Monté
 Author-email: valentinm@forestadmin.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8,<4.0)
 Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0) ; python_version < "3.9"
 Requires-Dist: cachetools (>=5.2,<6.0)
-Requires-Dist: forestadmin-datasource-toolkit (>=1.0.0-beta.2,<2.0.0)
+Requires-Dist: forestadmin-datasource-toolkit (>=1.0.0-beta.3,<2.0.0)
 Requires-Dist: marshmallow-jsonapi (>=0.24.0,<1.0)
 Requires-Dist: oic (>=1.4,<2.0)
 Requires-Dist: pandas (<=1.1.5) ; python_full_version < "3.7.1"
 Requires-Dist: pandas (>=1.3.4,<=1.3.5) ; python_full_version >= "3.7.1" and python_version < "3.8"
 Requires-Dist: pandas (>=1.4.0) ; python_version >= "3.8"
 Requires-Dist: python-jose (>=3.3,<4.0)
 Requires-Dist: typing-extensions (>=4.2.0,<5.0)
```

