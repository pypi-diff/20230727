# Comparing `tmp/alembic_postgresql_enum-0.1.3a2.tar.gz` & `tmp/alembic_postgresql_enum-0.1.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alembic_postgresql_enum-0.1.3a2.tar", max compression
+gzip compressed data, was "alembic_postgresql_enum-0.1.4a0.tar", max compression
```

## Comparing `alembic_postgresql_enum-0.1.3a2.tar` & `alembic_postgresql_enum-0.1.4a0.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0     1082 2023-05-26 08:19:49.153846 alembic_postgresql_enum-0.1.3a2/LICENSE
--rw-r--r--   0        0        0     4263 2023-05-26 14:50:54.441763 alembic_postgresql_enum-0.1.3a2/README.md
--rw-r--r--   0        0        0       60 2023-07-19 17:05:28.063788 alembic_postgresql_enum-0.1.3a2/alembic_postgresql_enum/__init__.py
--rw-r--r--   0        0        0     4821 2023-07-19 16:50:35.569872 alembic_postgresql_enum-0.1.3a2/alembic_postgresql_enum/enum_alteration.py
--rw-r--r--   0        0        0     2191 2023-07-19 16:50:35.581872 alembic_postgresql_enum-0.1.3a2/alembic_postgresql_enum/enum_creation.py
--rw-r--r--   0        0        0     3890 2023-07-19 17:50:40.549511 alembic_postgresql_enum-0.1.3a2/alembic_postgresql_enum/get_enum_data.py
--rw-r--r--   0        0        0      810 2023-07-19 18:53:58.752409 alembic_postgresql_enum-0.1.3a2/pyproject.toml
--rw-r--r--   0        0        0     5103 1970-01-01 00:00:00.000000 alembic_postgresql_enum-0.1.3a2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-26 08:19:49.153846 alembic_postgresql_enum-0.1.4a0/LICENSE
+-rw-r--r--   0        0        0     3985 2023-07-26 19:58:44.754677 alembic_postgresql_enum-0.1.4a0/README.md
+-rw-r--r--   0        0        0       32 2023-07-26 19:11:56.863336 alembic_postgresql_enum-0.1.4a0/alembic_postgresql_enum/__init__.py
+-rw-r--r--   0        0        0     1718 2023-07-26 19:11:56.863336 alembic_postgresql_enum-0.1.4a0/alembic_postgresql_enum/compare_dispatch.py
+-rw-r--r--   0        0        0     6270 2023-07-26 19:58:15.881837 alembic_postgresql_enum-0.1.4a0/alembic_postgresql_enum/enum_alteration.py
+-rw-r--r--   0        0        0     1145 2023-07-26 19:11:56.863336 alembic_postgresql_enum-0.1.4a0/alembic_postgresql_enum/enum_creation.py
+-rw-r--r--   0        0        0     1174 2023-07-26 19:11:56.863336 alembic_postgresql_enum-0.1.4a0/alembic_postgresql_enum/enum_deletion.py
+-rw-r--r--   0        0        0      606 2023-07-26 19:11:55.927316 alembic_postgresql_enum-0.1.4a0/alembic_postgresql_enum/enum_op_base.py
+-rw-r--r--   0        0        0     4799 2023-07-27 07:02:52.233793 alembic_postgresql_enum-0.1.4a0/alembic_postgresql_enum/get_enum_data.py
+-rw-r--r--   0        0        0      902 2023-07-27 07:13:19.051159 alembic_postgresql_enum-0.1.4a0/pyproject.toml
+-rw-r--r--   0        0        0     4824 1970-01-01 00:00:00.000000 alembic_postgresql_enum-0.1.4a0/PKG-INFO
```

### Comparing `alembic_postgresql_enum-0.1.3a2/LICENSE` & `alembic_postgresql_enum-0.1.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.3a2/README.md` & `alembic_postgresql_enum-0.1.4a0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -110,19 +110,17 @@
 It is fine if you do not have any data in your database. 
 But in most cases it is not.
 
 So adjust migration like that
 
 ```python
 def upgrade():
-    op.sync_enum_values('public', 'myenum', ['one', 'two', 'tree', 'three'], [('example_table', 'enum_field')])
-    op.execute("""UPDATE example_table SET enum_field = 'three' WHERE enum_field = 'tree'""")
-    op.sync_enum_values('public', 'myenum', ['one', 'two', 'three'], [('example_table', 'enum_field')])
+    op.sync_enum_values('public', 'myenum', ['one', 'two', 'three'], [('example_table', 'enum_field')],
+                        enum_values_to_rename=[('tree', 'three')])
 
 
 def downgrade():
-    op.sync_enum_values('public', 'myenum', ['one', 'two', 'tree', 'three'], [('example_table', 'enum_field')])
-    op.execute("""UPDATE example_table SET enum_field = 'tree' WHERE enum_field = 'three'""")
-    op.sync_enum_values('public', 'myenum', ['one', 'two', 'tree'], [('example_table', 'enum_field')])
+    op.sync_enum_values('public', 'myenum', ['one', 'two', 'tree'], [('example_table', 'enum_field')],
+                        enum_values_to_rename=[('three', 'tree')])
 ```
 
 Expand old values with new one, update all old values with new one, remove old enum value
```

### Comparing `alembic_postgresql_enum-0.1.3a2/alembic_postgresql_enum/get_enum_data.py` & `alembic_postgresql_enum-0.1.4a0/alembic_postgresql_enum/get_enum_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 # Based on https://github.com/dw/alembic-autogenerate-enums
+from collections import defaultdict
 from contextlib import contextmanager
 from dataclasses import dataclass
-from typing import Optional, Dict, List, Tuple
+from typing import Dict, Tuple, TYPE_CHECKING, Any, Set, FrozenSet
 
 import sqlalchemy
+from sqlalchemy import MetaData
 
+if TYPE_CHECKING:
+    from sqlalchemy.engine import Dialect
 
-@dataclass
-class EnumToTable:
+
+@dataclass(frozen=True)
+class TableReference:
     table_name: str
     column_name: str
-    enum_name: str
+
+    def to_tuple(self) -> Tuple[str, str]:
+        return self.table_name, self.column_name
+
+
+EnumNamesToValues = Dict[str, Tuple[str, ...]]
+EnumNamesToTableReferences = Dict[str, FrozenSet[TableReference]]
 
 
 @dataclass
 class DeclaredEnumValues:
-    # enum name -> tuple of values
-    enum_definitions: Dict[str, Tuple[str]]
-    table_definitions: Optional[List[EnumToTable]] = None
+    enum_values: EnumNamesToValues
+    enum_table_references: EnumNamesToTableReferences
 
 
-def get_defined_enums(conn, schema: str):
+def get_defined_enums(conn, schema: str) -> EnumNamesToValues:
     """
-    Return a dict mapping PostgreSQL enumeration types to the set of their
+    Return a dict mapping PostgreSQL defined enumeration types to the set of their
     defined values.
     :param conn:
         SQLAlchemy connection instance.
     :param str schema:
         Schema name (e.g. "public").
     :returns DeclaredEnumValues:
         enum_definitions={
@@ -41,18 +51,18 @@
                   WHERE enumtypid = t.oid)
         FROM pg_catalog.pg_type t
         LEFT JOIN pg_catalog.pg_namespace n ON n.oid = t.typnamespace
         WHERE
             t.typtype = 'e'
             AND n.nspname = :schema
     """
-    return DeclaredEnumValues({
+    return {
         r[0]: tuple(r[1])
         for r in conn.execute(sqlalchemy.text(sql), dict(schema=schema))
-    })
+    }
 
 
 def get_enum_values(enum_type: sqlalchemy.Enum, dialect) -> 'Tuple[str, ...]':
     # For specific case when types.TypeDecorator is used
     if isinstance(enum_type, sqlalchemy.types.TypeDecorator):
         def value_processor(value):
             return enum_type.process_bind_param(
@@ -61,64 +71,71 @@
             )
     else:
         def value_processor(enum_value):
             return enum_value
     return tuple(value_processor(value) for value in enum_type.enums)
 
 
-def get_declared_enums(metadata, schema: str, default_schema: str, dialect):
+def column_type_is_enum(column_type: Any) -> bool:
+    if isinstance(column_type, sqlalchemy.Enum):
+        return True
+
+    # For specific case when types.TypeDecorator is used
+    if isinstance(getattr(column_type, 'impl', None), sqlalchemy.Enum):
+        return True
+
+    return False
+
+
+def get_declared_enums(metadata: MetaData, schema: str, default_schema: str, dialect: 'Dialect') -> DeclaredEnumValues:
     """
-    Return a dict mapping SQLAlchemy enumeration types to the set of their
-    declared values.
+    Return a dict mapping SQLAlchemy declared enumeration types to the set of their values
+    with columns where enums are used.
     :param metadata:
-        ...
+        SqlAlchemy schema
     :param str schema:
         Schema name (e.g. "public").
     :param default_schema:
         Default schema name, likely will be "public"
-    :param dialect:
+    :param dialect: todo may be a good idea to get rid of it as library only supports postgresql
         Current sql dialect
     :returns DeclaredEnumValues:
-        enum_definitions: {
+        enum_values: {
             "my_enum": tuple(["a", "b", "c"]),
         },
-        table_definitions: [
-            EnumToTable(table_name="my_table", column_name="my_column", enum_name="my_enum"),
-        ]
+        enum_table_references: {
+            "my_enum": {
+                EnumToTable(table_name="my_table", column_name="my_column")
+            }
+        }
     """
-    types = set()
-    table_definitions = []
+    enum_name_to_values = dict()
+    enum_name_to_table_references: defaultdict[str, Set[TableReference]] = defaultdict(set)
 
     for table in metadata.tables.values():
         for column in table.columns:
+            # if column is in different schema
             if not hasattr(column.type, 'schema'):
                 continue
-
             if schema != (column.type.schema or default_schema):
                 continue
 
-            if isinstance(column.type, sqlalchemy.Enum):
-                types.add(column.type)
-
-            # For specific case when types.TypeDecorator is used
-            elif isinstance(getattr(column.type, 'impl', None), sqlalchemy.Enum):
-                types.add(column.type)
-
-            else:
+            if not column_type_is_enum(column.type):
                 continue
 
-            table_definitions.append(
-                EnumToTable(table.name, column.name, column.type.name)
-            )
+            if column.type.name not in enum_name_to_values:
+                enum_name_to_values[column.type.name] = get_enum_values(column.type, dialect)
+
+            enum_name_to_table_references[column.type.name].add(TableReference(table.name, column.name))
 
     return DeclaredEnumValues(
-        enum_definitions={
-            t.name: get_enum_values(t, dialect) for t in types
-        },
-        table_definitions=table_definitions,
+        enum_values=enum_name_to_values,
+        enum_table_references={enum_name: frozenset(table_references)
+                               for enum_name, table_references
+                               in enum_name_to_table_references.items()},
     )
 
 
 @contextmanager
 def get_connection(operations) -> sqlalchemy.engine.Connection:
     """
     SQLAlchemy 2.0 changes the operation binding location; bridge function to support
```

### Comparing `alembic_postgresql_enum-0.1.3a2/PKG-INFO` & `alembic_postgresql_enum-0.1.4a0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: alembic-postgresql-enum
-Version: 0.1.3a2
+Version: 0.1.4a0
 Summary: Alembic autogenerate support for creation, alteration and deletion of enums
 License: MIT
 Author: RustyGuard
 Requires-Python: >=3.7,<4.0
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -131,19 +131,17 @@
 It is fine if you do not have any data in your database. 
 But in most cases it is not.
 
 So adjust migration like that
 
 ```python
 def upgrade():
-    op.sync_enum_values('public', 'myenum', ['one', 'two', 'tree', 'three'], [('example_table', 'enum_field')])
-    op.execute("""UPDATE example_table SET enum_field = 'three' WHERE enum_field = 'tree'""")
-    op.sync_enum_values('public', 'myenum', ['one', 'two', 'three'], [('example_table', 'enum_field')])
+    op.sync_enum_values('public', 'myenum', ['one', 'two', 'three'], [('example_table', 'enum_field')],
+                        enum_values_to_rename=[('tree', 'three')])
 
 
 def downgrade():
-    op.sync_enum_values('public', 'myenum', ['one', 'two', 'tree', 'three'], [('example_table', 'enum_field')])
-    op.execute("""UPDATE example_table SET enum_field = 'tree' WHERE enum_field = 'three'""")
-    op.sync_enum_values('public', 'myenum', ['one', 'two', 'tree'], [('example_table', 'enum_field')])
+    op.sync_enum_values('public', 'myenum', ['one', 'two', 'tree'], [('example_table', 'enum_field')],
+                        enum_values_to_rename=[('three', 'tree')])
 ```
 
 Expand old values with new one, update all old values with new one, remove old enum value
```

