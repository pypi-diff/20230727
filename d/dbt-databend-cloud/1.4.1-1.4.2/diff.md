# Comparing `tmp/dbt_databend_cloud-1.4.1-py3-none-any.whl.zip` & `tmp/dbt_databend_cloud-1.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,27 @@
-Zip file size: 19171 bytes, number of entries: 20
+Zip file size: 22821 bytes, number of entries: 25
 -rw-r--r--  2.0 unx      545 b- defN 23-Feb-12 13:44 dbt/adapters/databend/__init__.py
--rw-r--r--  2.0 unx       18 b- defN 23-Jul-14 14:19 dbt/adapters/databend/__version__.py
+-rw-r--r--  2.0 unx       18 b- defN 23-Jul-27 03:22 dbt/adapters/databend/__version__.py
 -rw-r--r--  2.0 unx     1607 b- defN 23-Feb-12 13:44 dbt/adapters/databend/column.py
--rw-r--r--  2.0 unx     7131 b- defN 23-Jul-14 13:07 dbt/adapters/databend/connections.py
--rw-r--r--  2.0 unx    11247 b- defN 23-Feb-12 13:44 dbt/adapters/databend/impl.py
--rw-r--r--  2.0 unx     2802 b- defN 23-Feb-12 13:44 dbt/adapters/databend/relation.py
+-rw-r--r--  2.0 unx     7531 b- defN 23-Jul-27 03:22 dbt/adapters/databend/connections.py
+-rw-r--r--  2.0 unx    11224 b- defN 23-Jul-27 03:22 dbt/adapters/databend/impl.py
+-rw-r--r--  2.0 unx     2885 b- defN 23-Jul-27 03:22 dbt/adapters/databend/relation.py
 -rw-r--r--  2.0 unx       52 b- defN 23-Feb-12 13:44 dbt/include/databend/__init__.py
--rw-r--r--  2.0 unx       77 b- defN 23-Feb-12 13:44 dbt/include/databend/dbt_project.yml
--rw-r--r--  2.0 unx      185 b- defN 23-Feb-12 13:44 dbt/include/databend/profile_template.yml
--rw-r--r--  2.0 unx     8965 b- defN 23-Feb-12 13:44 dbt/include/databend/macros/adapters.sql
+-rw-r--r--  2.0 unx       77 b- defN 23-Jul-27 03:22 dbt/include/databend/dbt_project.yml
+-rw-r--r--  2.0 unx      185 b- defN 23-Jul-18 07:59 dbt/include/databend/profile_template.yml
+-rw-r--r--  2.0 unx     5771 b- defN 23-Jul-27 03:22 dbt/include/databend/macros/adapters.sql
 -rw-r--r--  2.0 unx      796 b- defN 23-Feb-12 13:44 dbt/include/databend/macros/catalog.sql
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-12 13:44 dbt/include/databend/macros/incremental.sql
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-12 13:44 dbt/include/databend/macros/snapshot.sql
 -rw-r--r--  2.0 unx      285 b- defN 23-Feb-12 13:44 dbt/include/databend/macros/utils.sql
+-rw-r--r--  2.0 unx     1095 b- defN 23-Jul-27 03:22 dbt/include/databend/macros/adapters/apply_grants.sql
+-rw-r--r--  2.0 unx      826 b- defN 23-Jul-27 03:22 dbt/include/databend/macros/adapters/relation.sql
+-rw-r--r--  2.0 unx     6216 b- defN 23-Jul-27 03:22 dbt/include/databend/macros/materializations/incremental.sql
 -rw-r--r--  2.0 unx     1111 b- defN 23-Feb-12 13:44 dbt/include/databend/macros/materializations/seed.sql
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-14 14:28 dbt_databend_cloud-1.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      856 b- defN 23-Jul-14 14:28 dbt_databend_cloud-1.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 14:28 dbt_databend_cloud-1.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Jul-14 14:28 dbt_databend_cloud-1.4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1839 b- defN 23-Jul-14 14:28 dbt_databend_cloud-1.4.1.dist-info/RECORD
-20 files, 48969 bytes uncompressed, 16083 bytes compressed:  67.2%
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-27 03:22 dbt/include/databend/macros/materializations/snapshot.sql
+-rw-r--r--  2.0 unx     2987 b- defN 23-Jul-27 03:22 dbt/include/databend/macros/materializations/table.sql
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-27 03:25 dbt_databend_cloud-1.4.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      907 b- defN 23-Jul-27 03:25 dbt_databend_cloud-1.4.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-27 03:25 dbt_databend_cloud-1.4.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Jul-27 03:25 dbt_databend_cloud-1.4.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2393 b- defN 23-Jul-27 03:25 dbt_databend_cloud-1.4.2.dist-info/RECORD
+25 files, 57964 bytes uncompressed, 18807 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -36,26 +36,41 @@
 
 Filename: dbt/include/databend/macros/snapshot.sql
 Comment: 
 
 Filename: dbt/include/databend/macros/utils.sql
 Comment: 
 
+Filename: dbt/include/databend/macros/adapters/apply_grants.sql
+Comment: 
+
+Filename: dbt/include/databend/macros/adapters/relation.sql
+Comment: 
+
+Filename: dbt/include/databend/macros/materializations/incremental.sql
+Comment: 
+
 Filename: dbt/include/databend/macros/materializations/seed.sql
 Comment: 
 
-Filename: dbt_databend_cloud-1.4.1.dist-info/LICENSE
+Filename: dbt/include/databend/macros/materializations/snapshot.sql
+Comment: 
+
+Filename: dbt/include/databend/macros/materializations/table.sql
+Comment: 
+
+Filename: dbt_databend_cloud-1.4.2.dist-info/LICENSE
 Comment: 
 
-Filename: dbt_databend_cloud-1.4.1.dist-info/METADATA
+Filename: dbt_databend_cloud-1.4.2.dist-info/METADATA
 Comment: 
 
-Filename: dbt_databend_cloud-1.4.1.dist-info/WHEEL
+Filename: dbt_databend_cloud-1.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: dbt_databend_cloud-1.4.1.dist-info/top_level.txt
+Filename: dbt_databend_cloud-1.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: dbt_databend_cloud-1.4.1.dist-info/RECORD
+Filename: dbt_databend_cloud-1.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dbt/adapters/databend/__version__.py

```diff
@@ -1 +1 @@
-version = "1.4.1"
+version = "1.4.2"
```

## dbt/adapters/databend/connections.py

```diff
@@ -8,15 +8,15 @@
 from dbt.adapters.sql import SQLConnectionManager as connection_cls
 from dbt.contracts.connection import AdapterResponse
 from dbt.events import AdapterLogger
 from typing import Optional, Tuple, List, Any
 from databend_sqlalchemy import connector
 
 from dbt.exceptions import (
-    RuntimeException,
+    Exception,
 )
 
 logger = AdapterLogger("databend")
 
 
 @dataclass
 class DatabendAdapterResponse(AdapterResponse):
@@ -31,15 +31,16 @@
     """
 
     host: Optional[str] = None
     port: Optional[int] = None
     database: Optional[str] = None
     username: Optional[str] = None
     password: Optional[str] = None
-    schema: str = "default"
+    schema: Optional[str] = None
+    secure: Optional[bool] = None
 
     # Add credentials members here, like:
     # host: str
     # port: int
     # username: str
     # password: str
 
@@ -57,15 +58,15 @@
             data["database"] = None
         return data
 
     def __post_init__(self):
         # databend classifies database and schema as the same thing
         self.database = None
         if self.database is not None and self.database != self.schema:
-            raise dbt.exceptions.RuntimeException(
+            raise dbt.exceptions.Exception(
                 f"    schema: {self.schema} \n"
                 f"    database: {self.database} \n"
                 f"On Databend, database must be omitted or have the same value as"
                 f" schema."
             )
 
     @property
@@ -100,15 +101,15 @@
         try:
             yield
 
         except Exception as e:
             logger.debug("Error running SQL: {}".format(sql))
             logger.debug("Rolling back transaction.")
             self.rollback_if_open()
-            raise dbt.exceptions.RuntimeException(str(e))
+            raise dbt.exceptions.Exception(str(e))
 
     # except for DML statements where explicitly defined
     def add_begin_query(self, *args, **kwargs):
         pass
 
     def add_commit_query(self, *args, **kwargs):
         pass
@@ -137,32 +138,41 @@
         try:
             # handle = mysql.connector.connect(
             #     # host=credentials.host,
             #     # port=credentials.port,
             #     # user=credentials.username,
             #     # password=credentials.password,
             # )
-            handle = connector.connect(
-                f"https://{credentials.username}:{credentials.password}@{credentials.host}:{credentials.port}?secure=true"
-            )
+            if credentials.secure is None:
+                credentials.secure = True
+
+            if credentials.secure:
+                handle = connector.connect(
+                    f"https://{credentials.username}:{credentials.password}@{credentials.host}:{credentials.port}/{credentials.schema}?secure=true "
+                )
+            else:
+                handle = connector.connect(
+                    f"http://{credentials.username}:{credentials.password}@{credentials.host}:{credentials.port}/{credentials.schema}?secure=false "
+                )
+
         except Exception as e:
             logger.debug("Error opening connection: {}".format(e))
             connection.handle = None
             connection.state = "fail"
             raise dbt.exceptions.FailedToConnectException(str(e))
         connection.state = "open"
         connection.handle = handle
         return connection
 
     @classmethod
     def get_response(cls, _):
         return "OK"
 
     def execute(
-        self, sql: str, auto_begin: bool = False, fetch: bool = False
+            self, sql: str, auto_begin: bool = False, fetch: bool = False
     ) -> Tuple[AdapterResponse, agate.Table]:
         # don't apply the query comment here
         # it will be applied after ';' queries are split
         _, cursor = self.add_query(sql, auto_begin)
         response = self.get_response(cursor)
         # table: rows, column_names=None, column_types=None, row_names=None
         if fetch:
@@ -179,15 +189,15 @@
         if cursor is None:
             conn = self.get_thread_connection()
             if conn is None or conn.name is None:
                 conn_name = "<None>"
             else:
                 conn_name = conn.name
 
-            raise RuntimeException(
+            raise Exception(
                 "Tried to run an empty query on model '{}'. If you are "
                 "conditionally running\nsql, eg. in a model hook, make "
                 "sure your `else` clause contains valid sql!\n\n"
                 "Provided SQL:\n{}".format(conn_name, sql)
             )
 
         return connection, cursor
```

## dbt/adapters/databend/impl.py

```diff
@@ -95,15 +95,15 @@
 
     @classmethod
     def convert_date_type(cls, agate_table: agate.Table, col_idx: int) -> str:
         return "date"
 
     @classmethod
     def convert_time_type(cls, agate_table: agate.Table, col_idx: int) -> str:
-        raise dbt.exceptions.NotImplementedException(
+        raise dbt.exceptions.DbtRuntimeError(
             "`convert_time_type` is not implemented for this adapter!"
         )
 
     def quote(self, identifier):
         return "{}".format(identifier)
 
     def check_schema_exists(self, database, schema):
@@ -119,15 +119,15 @@
     ) -> List[DatabendRelation]:
         kwargs = {"schema_relation": schema_relation}
         results = self.execute_macro(LIST_RELATIONS_MACRO_NAME, kwargs=kwargs)
 
         relations = []
         for row in results:
             if len(row) != 4:
-                raise dbt.exceptions.RuntimeException(
+                raise dbt.exceptions.DbtRuntimeError(
                     f"Invalid value from 'show table extended ...', "
                     f"got {len(row)} values, expected 4"
                 )
             _database, name, schema, type_info = row
             rel_type = RelationType.View if "view" in type_info else RelationType.Table
             relation = self.Relation.create(
                 database=None,
@@ -147,16 +147,16 @@
             table.rows,
             table.column_names,
             text_only_columns=["table_schema", "table_name"],
         )
         return table.where(_catalog_filter_schemas(manifest))
 
     def get_relation(self, database: Optional[str], schema: str, identifier: str):
-        if not self.Relation.include_policy.database:
-            database = None
+        # if not self.Relation.include_policy.database:
+        #     database = None
 
         return super().get_relation(database, schema, identifier)
 
     def parse_show_columns(
         self, _relation: DatabendRelation, raw_rows: List[agate.Row]
     ) -> List[DatabendColumn]:
         rows = [
@@ -178,15 +178,15 @@
         rows: List[agate.Row] = super().get_columns_in_relation(relation)
 
         return self.parse_show_columns(relation, rows)
 
     def get_catalog(self, manifest):
         schema_map = self._get_catalog_schemas(manifest)
         if len(schema_map) > 1:
-            dbt.exceptions.raise_compiler_error(
+            dbt.exceptions.DbtRuntimeError(
                 f"Expected only one database in get_catalog, found "
                 f"{list(schema_map)}"
             )
 
         with executor(self.config) as tpe:
             futures: List[Future[agate.Table]] = []
             for info, schemas in schema_map.items():
@@ -207,28 +207,28 @@
     def _get_one_catalog(
         self,
         information_schema: InformationSchema,
         schemas: Set[str],
         manifest: Manifest,
     ) -> agate.Table:
         if len(schemas) != 1:
-            dbt.exceptions.raise_compiler_error(
+            dbt.exceptions.DbtRuntimeError(
                 f"Expected only one schema in databend _get_one_catalog, found {schemas}"
             )
 
         return super()._get_one_catalog(information_schema, schemas, manifest)
 
     def update_column_sql(
         self,
         dst_name: str,
         dst_column: str,
         clause: str,
         where_clause: Optional[str] = None,
     ) -> str:
-        raise dbt.exceptions.NotImplementedException(
+        raise dbt.exceptions.DbtInternalError(
             "`update_column_sql` is not implemented for this adapter!"
         )
 
     def run_sql_for_tests(self, sql, fetch, conn):
         cursor = conn.handle.cursor()
         try:
             cursor.execute(sql)
@@ -335,8 +335,8 @@
 
     @property
     def default_python_submission_method(self):
         raise NotImplementedError("default_python_submission_method is not specified")
 
     @property
     def python_submission_helpers(self):
-        raise NotImplementedError("python_submission_helpers is not specified")
+        raise NotImplementedError("python_submission_helpers is not specified")
```

## dbt/adapters/databend/relation.py

```diff
@@ -1,8 +1,8 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import Optional, TypeVar, Any, Type, Dict, Union, Iterator, Tuple, Set
 import dbt.exceptions
 from dbt.adapters.base.relation import BaseRelation, Policy
 from dbt.contracts.relation import (
     Path,
     RelationType,
 )
@@ -23,37 +23,38 @@
 
 
 Self = TypeVar("Self", bound="DatabendRelation")
 
 
 @dataclass(frozen=True, eq=False, repr=False)
 class DatabendRelation(BaseRelation):
-    quote_policy: DatabendQuotePolicy = DatabendQuotePolicy()
-    include_policy: DatabendIncludePolicy = DatabendIncludePolicy()
+    quote_policy: Policy = field(default_factory=lambda: DatabendQuotePolicy())
+    include_policy: DatabendIncludePolicy = field(
+        default_factory=lambda: DatabendIncludePolicy()
+    )
     quote_character: str = ""
 
     def __post_init__(self):
         if self.database != self.schema and self.database:
-            raise dbt.exceptions.RuntimeException(
+            raise dbt.exceptions.DbtRuntimeError(
                 f"    schema: {self.schema} \n"
                 f"    database: {self.database} \n"
                 f"On Databend, database must be omitted or have the same value as"
                 f" schema."
             )
 
     @classmethod
     def create(
-        cls: Type[Self],
-        database: Optional[str] = None,
-        schema: Optional[str] = None,
-        identifier: Optional[str] = None,
-        type: Optional[RelationType] = None,
-        **kwargs,
+            cls: Type[Self],
+            database: Optional[str] = None,
+            schema: Optional[str] = None,
+            identifier: Optional[str] = None,
+            type: Optional[RelationType] = None,
+            **kwargs,
     ) -> Self:
-        cls.database = None
         database = None
         kwargs.update(
             {
                 "path": {
                     "database": database,
                     "schema": schema,
                     "identifier": identifier,
@@ -61,35 +62,35 @@
                 "type": type,
             }
         )
         return cls.from_dict(kwargs)
 
     def render(self):
         if self.include_policy.database and self.include_policy.schema:
-            raise dbt.exceptions.RuntimeException(
+            raise dbt.exceptions.DbtRuntimeError(
                 "Got a databend relation with schema and database set to "
                 "include, but only one can be set"
             )
         return super().render()
 
     @classmethod
     def get_path(
-        cls, relation: BaseRelation, information_schema_view: Optional[str]
+            cls, relation: BaseRelation, information_schema_view: Optional[str]
     ) -> Path:
         Path.database = None
         return Path(
             database=None,
             schema=relation.schema,
             identifier="INFORMATION_SCHEMA",
         )
 
     def matches(
-        self,
-        database: Optional[str] = None,
-        schema: Optional[str] = None,
-        identifier: Optional[str] = None,
+            self,
+            database: Optional[str] = None,
+            schema: Optional[str] = None,
+            identifier: Optional[str] = None,
     ):
         if database:
-            raise dbt.exceptions.RuntimeException(
+            raise dbt.exceptions.DbtRuntimeError(
                 f"Passed unexpected schema value {schema} to Relation.matches"
             )
         return self.schema == schema and self.identifier == identifier
```

## dbt/include/databend/dbt_project.yml

```diff
@@ -1,5 +1,5 @@
 name: dbt_databend
-version: 1.3.0
+version: 1.5.0
 config-version: 2
 
 macro-paths: ["macros"]
```

## dbt/include/databend/macros/adapters.sql

```diff
@@ -1,66 +1,19 @@
 /* For examples of how to fill out the macros please refer to the postgres adapter and docs
 postgres adapter macros: https://github.com/dbt-labs/dbt-core/blob/main/plugins/postgres/dbt/include/postgres/macros/adapters.sql
 dbt docs: https://docs.getdbt.com/docs/contributing/building-a-new-adapter
 */
 
--- {% macro databend__alter_column_type(relation,column_name,new_column_type) -%}
--- '''Changes column name or data type'''
--- /*
---     1. Create a new column (w/ temp name and correct type)
---     2. Copy data over to it
---     3. Drop the existing column (cascade!)
---     4. Rename the new column to existing column
--- */
--- {% endmacro %}
-
--- {% macro databend__check_schema_exists(information_schema,schema) -%}
--- '''Checks if schema name exists and returns number or times it shows up.'''
--- /*
---     1. Check if schemas exist
---     2. return number of rows or columns that match searched parameter
--- */
--- {% endmacro %}
-
---  Example from postgres adapter in dbt-core
---  Notice how you can build out other methods than the designated ones for the impl.py file,
---  to make a more robust adapter. ex. (verify_database)
-
-/*
-
- {% macro postgres__create_schema(relation) -%}
-   {% if relation.database -%}
-    {{ adapter.verify_database(relation.database) }}
-  {%- endif -%}   {%- call statement('create_schema') -%}
-     create schema if not exists {{ relation.without_identifier().include(database=False) }}
-   {%- endcall -%}
- {% endmacro %}
- 
-*/
-
 {% macro databend__create_schema(relation) -%}
 '''Creates a new schema in the  target database, if schema already exists, method is a no-op. '''
   {%- call statement('create_schema') -%}
     create database if not exists {{ relation.without_identifier().include(database=False) }}
   {% endcall %}
 {% endmacro %}
 
-/*
-
-{% macro postgres__drop_schema(relation) -%}
-  {% if relation.database -%}
-    {{ adapter.verify_database(relation.database) }}
-  {%- endif -%}
-  {%- call statement('drop_schema') -%}
-    drop schema if exists {{ relation.without_identifier().include(database=False) }} cascade
-  {%- endcall -%}
-{% endmacro %}
-
-*/
-
 {% macro databend__drop_relation(relation) -%}
 '''Deletes relatonship identifer between tables.'''
 /*
   1. If database exists
   2. Create a new schema if passed schema does not exist already
 */
   {% call statement('drop_relation', auto_begin=False) -%}
@@ -75,38 +28,14 @@
   2. search all calls of schema, and change include value to False, cascade it to backtrack
 */
   {%- call statement('drop_schema') -%}
     drop database if exists {{ relation.without_identifier().include(database=False) }}
   {%- endcall -%}
 {% endmacro %}
 
-/*
-
- Example of 1 of 3 required macros that does not have a default implementation
-{% macro postgres__get_columns_in_relation(relation) -%}
-  {% call statement('get_columns_in_relation', fetch_result=True) %}
-      select
-          column_name,
-          data_type,
-          character_maximum_length,
-          numeric_precision,
-          numeric_scale
-      from {{ relation.information_schema('columns') }}
-      where table_name = '{{ relation.identifier }}'
-        {% if relation.schema %}
-        and table_schema = '{{ relation.schema }}'
-        {% endif %}
-      order by ordinal_position
-  {% endcall %}
-  {% set table = load_result('get_columns_in_relation').table %}
-  {{ return(sql_convert_columns_in_relation(table)) }}
-{% endmacro %}
-*/
-
-
 {% macro databend__get_columns_in_relation(relation) -%}
 '''Returns a list of Columns in a table.'''
 /*
   1. select as many values from column as needed
   2. search relations to columns
   3. where table name is equal to the relation identifier
   4. if a relation schema exists and table schema is equal to the relation schema
@@ -127,39 +56,14 @@
     {% endif %}
   {% endcall %}
   {% do return(load_result('get_columns_in_relation').table) %}
 {% endmacro %}
 
 --  Example of 2 of 3 required macros that do not come with a default implementation
 
-/*
-
-{% macro postgres__list_relations_without_caching(schema_relation) %}
-  {% call statement('list_relations_without_caching', fetch_result=True) -%}
-    select
-      '{{ schema_relation.database }}' as database,
-      tablename as name,
-      schemaname as schema,
-      'table' as type
-    from pg_tables
-    where schemaname ilike '{{ schema_relation.schema }}'
-    union all
-    select
-      '{{ schema_relation.database }}' as database,
-      viewname as name,
-      schemaname as schema,
-      'view' as type
-    from pg_views
-    where schemaname ilike '{{ schema_relation.schema }}'
-  {% endcall %}
-  {{ return(load_result('list_relations_without_caching').table) }}
-{% endmacro %}
-
-*/
-
 {% macro databend__list_relations_without_caching(schema_relation) -%}
 '''creates a table of relations withough using local caching.'''
   {% call statement('list_relations_without_caching', fetch_result=True) -%}
     select
       null as db,
       name as name,
       database as schema,
@@ -215,34 +119,25 @@
   {% do return(tmp_relation) %}
 {% endmacro %}
 
 {% macro databend__generate_database_name(custom_database_name=none, node=none) -%}
   {% do return(None) %}
 {%- endmacro %}
 
-/*
-
-Example 3 of 3 of required macros that does not have a default implementation.
- ** Good example of building out small methods ** please refer to impl.py for implementation of now() in postgres plugin
-{% macro postgres__current_timestamp() -%}
-  now()
-{%- endmacro %}
-
-*/
 {% macro databend__current_timestamp() -%}
   NOW()
 {%- endmacro %}
 
 {% macro databend__create_table_as(temporary, relation, sql) -%}
   {%- set sql_header = config.get('sql_header', none) -%}
 
   {{ sql_header if sql_header is not none }}
 
   {% if temporary -%}
-    create transient table {{ relation.name }}
+    create transient table {{ relation.name }} if not exist
   {%- else %}
     create table {{ relation.include(database=False) }}
     {{ cluster_by_clause(label="cluster by") }}
   {%- endif %}
   as {{ sql }}
 {%- endmacro %}
```

## Comparing `dbt_databend_cloud-1.4.1.dist-info/LICENSE` & `dbt_databend_cloud-1.4.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dbt_databend_cloud-1.4.1.dist-info/METADATA` & `dbt_databend_cloud-1.4.2.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: dbt-databend-cloud
-Version: 1.4.1
+Version: 1.4.2
 Summary: The Databend adapter plugin for dbt
 Home-page: https://github.com/databendcloud/dbt-databend.git
 Author: Databend Cloud Team
 Author-email: zhangzhihan@datafuselabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: dbt-core (~=1.3.0)
+Requires-Dist: dbt-core (~=1.5.0)
 Requires-Dist: databend-py (~=0.4.6)
 Requires-Dist: databend-sqlalchemy (~=0.2.4)
 
 The Databend adapter plugin for dbt
```

