# Comparing `tmp/forestadmin_datasource_sqlalchemy-1.0.0b2.tar.gz` & `tmp/forestadmin_datasource_sqlalchemy-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_datasource_sqlalchemy-1.0.0b2.tar", max compression
+gzip compressed data, was "forestadmin_datasource_sqlalchemy-1.0.0b3.tar", max compression
```

## Comparing `forestadmin_datasource_sqlalchemy-1.0.0b2.tar` & `forestadmin_datasource_sqlalchemy-1.0.0b3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        0 2023-07-26 13:23:56.494995 forestadmin_datasource_sqlalchemy-1.0.0b2/README.md
--rw-r--r--   0        0        0        0 2023-07-26 13:23:56.494995 forestadmin_datasource_sqlalchemy-1.0.0b2/forestadmin/datasource_sqlalchemy/__init__.py
--rw-r--r--   0        0        0    11076 2023-07-26 13:23:56.494995 forestadmin_datasource_sqlalchemy-1.0.0b2/forestadmin/datasource_sqlalchemy/collections.py
--rw-r--r--   0        0        0     3045 2023-07-26 13:23:56.494995 forestadmin_datasource_sqlalchemy-1.0.0b2/forestadmin/datasource_sqlalchemy/datasource.py
--rw-r--r--   0        0        0      612 2023-07-26 13:23:56.494995 forestadmin_datasource_sqlalchemy-1.0.0b2/forestadmin/datasource_sqlalchemy/exceptions.py
--rw-r--r--   0        0        0     1923 2023-07-26 13:23:56.494995 forestadmin_datasource_sqlalchemy-1.0.0b2/forestadmin/datasource_sqlalchemy/interfaces.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:56.494995 forestadmin_datasource_sqlalchemy-1.0.0b2/forestadmin/datasource_sqlalchemy/utils/__init__.py
--rw-r--r--   0        0        0     5956 2023-07-26 13:23:56.494995 forestadmin_datasource_sqlalchemy-1.0.0b2/forestadmin/datasource_sqlalchemy/utils/aggregation.py
--rw-r--r--   0        0        0     6235 2023-07-26 13:23:56.494995 forestadmin_datasource_sqlalchemy-1.0.0b2/forestadmin/datasource_sqlalchemy/utils/model_converter.py
--rw-r--r--   0        0        0    10207 2023-07-26 13:23:56.494995 forestadmin_datasource_sqlalchemy-1.0.0b2/forestadmin/datasource_sqlalchemy/utils/query_factory.py
--rw-r--r--   0        0        0     2943 2023-07-26 13:23:56.494995 forestadmin_datasource_sqlalchemy-1.0.0b2/forestadmin/datasource_sqlalchemy/utils/record_serializer.py
--rw-r--r--   0        0        0      519 2023-07-26 13:23:56.494995 forestadmin_datasource_sqlalchemy-1.0.0b2/forestadmin/datasource_sqlalchemy/utils/relationships.py
--rw-r--r--   0        0        0     7029 2023-07-26 13:23:56.494995 forestadmin_datasource_sqlalchemy-1.0.0b2/forestadmin/datasource_sqlalchemy/utils/type_converter.py
--rw-r--r--   0        0        0     1808 2023-07-26 13:24:14.411272 forestadmin_datasource_sqlalchemy-1.0.0b2/pyproject.toml
--rw-r--r--   0        0        0      873 1970-01-01 00:00:00.000000 forestadmin_datasource_sqlalchemy-1.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0    11179 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/collections.py
+-rw-r--r--   0        0        0     3045 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/datasource.py
+-rw-r--r--   0        0        0      612 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/exceptions.py
+-rw-r--r--   0        0        0     1923 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/interfaces.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/__init__.py
+-rw-r--r--   0        0        0     5956 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/aggregation.py
+-rw-r--r--   0        0        0     6235 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/model_converter.py
+-rw-r--r--   0        0        0    10207 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/query_factory.py
+-rw-r--r--   0        0        0     2943 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/record_serializer.py
+-rw-r--r--   0        0        0      519 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/relationships.py
+-rw-r--r--   0        0        0     7029 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/type_converter.py
+-rw-r--r--   0        0        0     1808 2023-07-27 12:28:44.964527 forestadmin_datasource_sqlalchemy-1.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0      873 1970-01-01 00:00:00.000000 forestadmin_datasource_sqlalchemy-1.0.0b3/PKG-INFO
```

### Comparing `forestadmin_datasource_sqlalchemy-1.0.0b2/forestadmin/datasource_sqlalchemy/collections.py` & `forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/collections.py`

 * *Files 4% similar despite different names*

```diff
@@ -162,35 +162,35 @@
         for parent_field, child_fields in projection.relations.items():
             normalized_projection.extend(self._normalize_projection(child_fields, f"{prefix}{parent_field}:"))
         return Projection(*normalized_projection)
 
     async def aggregate(
         self,
         caller: User,
-        filter: Optional[Filter],
+        filter_: Optional[Filter],
         aggregation: Aggregation,
         limit: Optional[int] = None,
     ) -> List[AggregateResult]:
         with self.datasource.Session.begin() as session:  #  type: ignore
             dialect: Dialect = session.bind.dialect  #  type: ignore
-            filter = cast(Filter, self._cast_filter(filter)) or None
-            query = QueryFactory.build_aggregate(dialect, self, filter, aggregation, limit)
+            filter_ = cast(Filter, self._cast_filter(filter_)) or None
+            query = QueryFactory.build_aggregate(dialect, self, filter_, aggregation, limit)
             res: List[Dict[str, Any]] = session.execute(query)  #  type: ignore
             return aggregations_to_records(res)
 
     @handle_sqlalchemy_error
     async def create(self, caller: User, data: List[RecordsDataAlias]) -> List[RecordsDataAlias]:
         with self.datasource.Session.begin() as session:  #  type: ignore
             instances = QueryFactory.create(self, data)
             session.bulk_save_objects(instances, return_defaults=True)  # type: ignore
             return instances_to_records(self, instances)
 
-    async def update(self, caller: User, filter: Optional[Filter], patch: RecordsDataAlias) -> None:
+    async def update(self, caller: User, filter_: Optional[Filter], patch: RecordsDataAlias) -> None:
         with self.datasource.Session.begin() as session:  #  type: ignore
-            query = QueryFactory.update(self, filter, patch)
+            query = QueryFactory.update(self, filter_, patch)
             session.execute(query)  # type: ignore
 
     def _cast_condition_tree(self, tree: ConditionTree) -> ConditionTree:
         if isinstance(tree, ConditionTreeLeaf):
             if TypeGetter.get(tree.value, None) == PrimitiveType.DATE:
                 iso_format = tree.value
                 if isinstance(iso_format, str):
@@ -198,38 +198,43 @@
                         iso_format = iso_format[:-1]
                     iso_format = datetime.fromisoformat(iso_format).replace(
                         tzinfo=zoneinfo.ZoneInfo("UTC")
                     )  # type: ignore
                 tree = tree.override({"value": iso_format})
         return tree
 
-    def _cast_filter(self, filter: Union[Filter, PaginatedFilter, None]) -> Union[Filter, PaginatedFilter, None]:
-        if filter and filter.condition_tree:
-            filter = filter.override(
-                {"condition_tree": filter.condition_tree.replace(self._cast_condition_tree)}  # type: ignore
+    def _cast_filter(self, filter_: Union[Filter, PaginatedFilter, None]) -> Union[Filter, PaginatedFilter, None]:
+        if filter_ and filter_.condition_tree:
+            filter_ = filter_.override(
+                {"condition_tree": filter_.condition_tree.replace(self._cast_condition_tree)}  # type: ignore
             )
-        return filter
+        return filter_
 
-    async def list(self, caller: User, filter: PaginatedFilter, projection: Projection) -> List[RecordsDataAlias]:
+    async def list(self, caller: User, filter_: PaginatedFilter, projection: Projection) -> List[RecordsDataAlias]:
         with self.datasource.Session.begin() as session:  #  type: ignore
             normalized_projection = self._normalize_projection(projection)
-            filter = cast(PaginatedFilter, self._cast_filter(filter))
-            query = QueryFactory.build_list(self, filter, normalized_projection)
+            filter_ = cast(PaginatedFilter, self._cast_filter(filter_))
+            query = QueryFactory.build_list(self, filter_, normalized_projection)
             res = session.execute(query).all()  #  type: ignore
-            records = projections_to_records(normalized_projection, res, filter.timezone)  # type: ignore
+            records = projections_to_records(normalized_projection, res, filter_.timezone)  # type: ignore
             return records
 
-    async def delete(self, caller: User, filter: Optional[Filter]) -> None:
+    async def delete(self, caller: User, filter_: Optional[Filter]) -> None:
         with self.datasource.Session.begin() as session:  #  type: ignore
-            query = QueryFactory.delete(self, filter)
+            query = QueryFactory.delete(self, filter_)
             session.execute(query)  # type: ignore
 
     async def get_form(
-        self, caller: User, name: str, data: Optional[RecordsDataAlias], filter: Optional[Filter]
+        self,
+        caller: User,
+        name: str,
+        data: Optional[RecordsDataAlias],
+        filter_: Optional[Filter],
+        meta: Optional[Dict[str, Any]],
     ) -> List[ActionField]:
-        return await super().get_form(caller, name, data, filter)
+        return await super().get_form(caller, name, data, filter_, meta)
 
-    async def execute(self, caller: User, name: str, data: RecordsDataAlias, filter: Optional[Filter]) -> ActionResult:
-        return await super().execute(caller, name, data, filter)
+    async def execute(self, caller: User, name: str, data: RecordsDataAlias, filter_: Optional[Filter]) -> ActionResult:
+        return await super().execute(caller, name, data, filter_)
 
     async def render_chart(self, caller: User, name: str, record_id: List) -> Chart:
         return await super().render_chart(caller, name, record_id)
```

### Comparing `forestadmin_datasource_sqlalchemy-1.0.0b2/forestadmin/datasource_sqlalchemy/datasource.py` & `forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/datasource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.0.0b2/forestadmin/datasource_sqlalchemy/exceptions.py` & `forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/exceptions.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.0.0b2/forestadmin/datasource_sqlalchemy/interfaces.py` & `forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/interfaces.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.0.0b2/forestadmin/datasource_sqlalchemy/utils/aggregation.py` & `forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/aggregation.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.0.0b2/forestadmin/datasource_sqlalchemy/utils/model_converter.py` & `forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/model_converter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.0.0b2/forestadmin/datasource_sqlalchemy/utils/query_factory.py` & `forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/query_factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.0.0b2/forestadmin/datasource_sqlalchemy/utils/record_serializer.py` & `forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/record_serializer.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.0.0b2/forestadmin/datasource_sqlalchemy/utils/relationships.py` & `forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/relationships.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.0.0b2/forestadmin/datasource_sqlalchemy/utils/type_converter.py` & `forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/type_converter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.0.0b2/pyproject.toml` & `forestadmin_datasource_sqlalchemy-1.0.0b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-datasource-sqlalchemy"
-version = "1.0.0-beta.2"
+version = "1.0.0-beta.3"
 description = ""
 authors = [ "Valentin Monté <valentinm@forestadmin.com>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "forestadmin"
 
 [tool.semantic_release]
@@ -20,16 +20,16 @@
 build_command = "pip install poetry && poetry build"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 typing-extensions = "~=4.2"
 tzdata = "~=2022.6"
 sqlalchemy = "^1.4.44"
-forestadmin-datasource-toolkit = "^1.0.0-beta.2"
-forestadmin-agent-toolkit = "^1.0.0-beta.2"
+forestadmin-datasource-toolkit = "^1.0.0-beta.3"
+forestadmin-agent-toolkit = "^1.0.0-beta.3"
 
 [tool.poetry.dependencies."backports.zoneinfo"]
 version = "~=0.2.1"
 python = "<3.9"
 extras = [ "tzdata",]
 
 [tool.poetry.group.test]
```

### Comparing `forestadmin_datasource_sqlalchemy-1.0.0b2/PKG-INFO` & `forestadmin_datasource_sqlalchemy-1.0.0b3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: forestadmin-datasource-sqlalchemy
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
 Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0) ; python_version < "3.9"
-Requires-Dist: forestadmin-agent-toolkit (>=1.0.0-beta.2,<2.0.0)
-Requires-Dist: forestadmin-datasource-toolkit (>=1.0.0-beta.2,<2.0.0)
+Requires-Dist: forestadmin-agent-toolkit (>=1.0.0-beta.3,<2.0.0)
+Requires-Dist: forestadmin-datasource-toolkit (>=1.0.0-beta.3,<2.0.0)
 Requires-Dist: sqlalchemy (>=1.4.44,<2.0.0)
 Requires-Dist: typing-extensions (>=4.2,<5.0)
 Requires-Dist: tzdata (>=2022.6,<2023.0)
 Description-Content-Type: text/markdown
```

