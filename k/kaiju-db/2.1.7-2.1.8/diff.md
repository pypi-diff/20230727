# Comparing `tmp/kaiju_db-2.1.7-py3-none-any.whl.zip` & `tmp/kaiju_db-2.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 20394 bytes, number of entries: 12
--rw-r--r--  2.0 unx      183 b- defN 23-Jul-16 14:43 kaiju_db/__init__.py
--rw-r--r--  2.0 unx     3740 b- defN 23-Jul-16 14:43 kaiju_db/functions.py
--rw-r--r--  2.0 unx    59537 b- defN 23-Jul-16 14:43 kaiju_db/services.py
--rw-r--r--  2.0 unx      453 b- defN 23-Jul-16 14:43 kaiju_db/types.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-16 14:43 kaiju_db/tests/__init__.py
--rw-r--r--  2.0 unx     3292 b- defN 23-Jul-16 14:43 kaiju_db/tests/fixtures.py
--rw-r--r--  2.0 unx     4846 b- defN 23-Jul-16 14:43 kaiju_db/tests/test_db.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Jul-16 14:44 kaiju_db-2.1.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     3204 b- defN 23-Jul-16 14:44 kaiju_db-2.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-16 14:44 kaiju_db-2.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-16 14:44 kaiju_db-2.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      939 b- defN 23-Jul-16 14:44 kaiju_db-2.1.7.dist-info/RECORD
-12 files, 76905 bytes uncompressed, 18822 bytes compressed:  75.5%
+Zip file size: 20882 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      184 b- defN 23-Jul-27 19:34 kaiju_db/__init__.py
+-rw-r--r--  2.0 unx     3740 b- defN 23-Jul-27 19:34 kaiju_db/functions.py
+-rw-r--r--  2.0 unx    61457 b- defN 23-Jul-27 19:34 kaiju_db/services.py
+-rw-r--r--  2.0 unx      453 b- defN 23-Jul-27 19:34 kaiju_db/types.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-27 19:34 kaiju_db/tests/__init__.py
+-rw-r--r--  2.0 unx     3292 b- defN 23-Jul-27 19:34 kaiju_db/tests/fixtures.py
+-rw-r--r--  2.0 unx     4846 b- defN 23-Jul-27 19:34 kaiju_db/tests/test_db.py
+-rw-rw-rw-  2.0 unx      610 b- defN 23-Jul-27 19:34 kaiju_db-2.1.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3259 b- defN 23-Jul-27 19:34 kaiju_db-2.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-27 19:34 kaiju_db-2.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-27 19:34 kaiju_db-2.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      939 b- defN 23-Jul-27 19:34 kaiju_db-2.1.8.dist-info/RECORD
+12 files, 78881 bytes uncompressed, 19310 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: kaiju_db/tests/fixtures.py
 Comment: 
 
 Filename: kaiju_db/tests/test_db.py
 Comment: 
 
-Filename: kaiju_db-2.1.7.dist-info/LICENSE
+Filename: kaiju_db-2.1.8.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_db-2.1.7.dist-info/METADATA
+Filename: kaiju_db-2.1.8.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_db-2.1.7.dist-info/WHEEL
+Filename: kaiju_db-2.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_db-2.1.7.dist-info/top_level.txt
+Filename: kaiju_db-2.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_db-2.1.7.dist-info/RECORD
+Filename: kaiju_db-2.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_db/__init__.py

```diff
@@ -1,8 +1,8 @@
 from .types import *
 from .functions import *
 from .services import *
 
-__version__ = '2.1.7'
-__python_version__ = '3.8'
+__version__ = '2.1.8'
+__python_version__ = '3.11'
 __author__ = 'antonnidhoggr@me.com'
 __service_package__ = True
```

## kaiju_db/services.py

```diff
@@ -1,64 +1,50 @@
 """Database services."""
 
 import abc
+from collections.abc import AsyncGenerator, Collection, Hashable
+from enum import Enum
+from functools import cached_property
 from pathlib import Path
-from typing import (
-    cast,
-    List,
-    Collection,
-    TypedDict,
-    AsyncGenerator,
-    Union,
-    Optional,
-    Generic,
-    TypeVar,
-    Hashable,
-    Dict,
-    FrozenSet,
-    Literal,
-)
+from typing import Generic, List, Literal, Optional, TypedDict, TypeVar, Union, cast, final
 
 import sqlalchemy as sa
 import sqlalchemy.dialects.postgresql as sa_pg
+from kaiju_tools.app import SERVICE_CLASS_REGISTRY, ContextableService, Service
+from kaiju_tools.encoding import dumps, load, loads
+from kaiju_tools.exceptions import Conflict, InternalError, MethodNotAllowed, NotFound, ValidationError
+from kaiju_tools.interfaces import DataStore, Locks, PublicInterface
+from sqlalchemy import MetaData, Table, text
 from sqlalchemy.exc import IntegrityError
-from sqlalchemy.sql.expression import nullslast
-from sqlalchemy import MetaData, text, Table  # noqa pycharm
-from sqlalchemy.ext.asyncio import create_async_engine  # noqa pycharm
-
-from kaiju_tools.app import ContextableService, SERVICE_CLASS_REGISTRY, Service
-from kaiju_tools.interfaces import DataStore, Locks
-from kaiju_tools.exceptions import ValidationError, NotFound, Conflict, InternalError, MethodNotAllowed
-from kaiju_tools.encoding import dumps, loads, load
+from sqlalchemy.ext.asyncio import create_async_engine
+from sqlalchemy.sql.expression import nullslast  # noqa: package
+
 from kaiju_db.functions import SQL_FUNCTIONS, UserFunction
 
-__all__ = ['DatabaseService', 'SQLService', 'FixtureService', 'DatabaseMigrationService']
+
+__all__ = ['DatabaseService', 'SQLService', 'PermHook', 'FixtureService', 'DatabaseMigrationService']
 
 
 async def setup_asyncpg_jsonb_codec(conn):
     """Set up JSONB codec for asyncpg.
 
-    This occurs for all new connections and
-    can be overridden by third party dialects.
-
-    .. versionadded:: 1.4.27
-
+    Overriden for binary json serializer.
     """
 
     def _jsonb_encoder(str_value):
-        # \x01 is the prefix for jsonb used by PostgreSQL.
+        # \x01 is the prefix for jsonb used by Postgres.
         # asyncpg requires it when format='binary'
         return b'\x01' + str_value
 
     def _jsonb_decoder(bin_value):
-        # the byte is the \x01 prefix for jsonb used by PostgreSQL.
+        # the byte is the \x01 prefix for jsonb used by Postgres.
         # asyncpg returns it when format='binary'
         return loads(bin_value[1:])
 
-    asyncpg_connection = conn._connection
+    asyncpg_connection = conn._connection  # noqa
     await asyncpg_connection.set_type_codec(
         'jsonb',
         encoder=_jsonb_encoder,
         decoder=_jsonb_decoder,
         schema='pg_catalog',
         format='binary',
     )
@@ -86,15 +72,15 @@
         root_password: str = '',
         root_database: str = 'postgres',
         metadata: MetaData = None,
         init_db: bool = True,
         init_tables: bool = True,
         pool_size: int = 10,
         idle_connection_lifetime: int = 3600,
-        extensions: List[str] = None,
+        extensions: list[str] = None,
         functions=SQL_FUNCTIONS,
         logger=None,
     ):
         """Initialize.
 
         :param app:
         :param host: db url or address
@@ -246,15 +232,14 @@
         engine = create_async_engine(
             f'postgresql+asyncpg://{user}:{password}@{self._host}:{self._port}/{db}',
             json_serializer=dumps,
             json_deserializer=loads,
             pool_size=self._pool_size,
             pool_recycle=self._idle_connection_lifetime,
         )
-
         return engine
 
     async def _db_exists(self, conn) -> bool:
         self.logger.debug('Checking database "%s".', self._db)
         result = await conn.execute(text(f"SELECT 1 FROM pg_database WHERE datname = '{self._db}';"))  # noqa
         return bool(result.first())
 
@@ -273,17 +258,17 @@
         await conn.execute(text(f'GRANT CONNECT ON DATABASE {self._db} TO {self._user};'))
         await conn.execute(text(f'GRANT pg_read_all_data TO {self._user};'))
         await conn.execute(text(f'GRANT pg_write_all_data TO {self._user};'))
         await conn.execute(text(f'GRANT EXECUTE ON ALL FUNCTIONS IN SCHEMA public TO {self._user};'))
         await conn.execute(text(f'GRANT USAGE, SELECT ON ALL SEQUENCES IN SCHEMA public TO {self._user};'))
 
     async def _create_extension(self, conn, ext: str) -> None:
-        self.logger.info('Creating extension "%s" in database "%s".', ext, self._db)
         result = await conn.execute(text(f"SELECT 1 FROM pg_extension WHERE extname='{ext}';"))  # noqa
         if not result.first():
+            self.logger.info('Creating extension "%s" in database "%s".', ext, self._db)
             await conn.execute(text(f'CREATE EXTENSION "{ext}";'))
 
     async def _create_functions(self, conn):
         for _function_key in self._functions_registry:
             _function = self._functions_registry[_function_key]
             if issubclass(_function, UserFunction):
                 _function = _function.sql()
@@ -298,27 +283,27 @@
     desc: str
 
 
 _Id = TypeVar('_Id', bound=Hashable)
 _Row = TypeVar('_Row', bound=dict)
 _Columns = Union[Collection[str], Literal['*'], None]
 _SortField = Union[_SortDesc, _SortAsc, str]
-_Sort = Optional[List[_SortField]]
-_Condition = Union[dict, List[dict], None]
+_Sort = Optional[list[_SortField]]
+_Condition = Union[dict, list[dict], None]
 
 
 class _List(TypedDict):
     """Type hinting for a list query."""
 
-    count: Optional[int]  #: total rows matching the query, None if count hasn't been requested
+    count: int | None  #: total rows matching the query, None if count hasn't been requested
     offset: int  #: row offset for this selection
-    page: Optional[int]  #: current page number, None if count hasn't been requested
-    pages: Optional[int]  #: total pages, None if count hasn't been requested
+    page: int | None  #: current page number, None if count hasn't been requested
+    pages: int | None  #: total pages, None if count hasn't been requested
     on_page: int  #: number of rows on this page
-    data: Optional[List[_Row]]  #: returned rows, None if limit was set to 0
+    data: list[_Row] | None  #: returned rows, None if limit was set to 0
 
 
 class SQLService(Service, DataStore, Generic[_Id, _Row], abc.ABC):
     """Base SQL service interface with common commands and errors.
 
     Optimized for a single primary key only with a name "id"
 
@@ -370,27 +355,28 @@
         INVALID_ORDERING = 'query.invalid_ordering_command'
         INVALID_PAGINATION_OFFSET = 'query.invalid_pagination_offset'
         INVALID_PAGINATION_LIMIT = 'query.invalid_pagination_limit'
         INVALID_COLUMN = 'query.invalid_insert_column'
 
     DEFAULT_ROW_LIMIT = 24  #: defaults of LIMIT on queries
     MAX_ROW_LIMIT = 1000  #: max size of queries
+    MAX_GET_QUERY_SIZE = 65535
 
     select_columns = None  #: you can specify a whitelist of output columns here
     select_columns_blacklist = None
     update_columns = None  #: you may specify columns for update here
     update_columns_blacklist = None
     insert_columns = None  #: you may specify insert columns here
     insert_columns_blacklist = None
     table = None  #: here should be your table
 
     virtual_columns = None  # virtual SQL columns (i.e. functions) names and definitions
     # virtual columns can be selected but never updated / inserted
 
-    def __init__(self, app, database_service: Union[DatabaseService, str] = None, logger=None):
+    def __init__(self, app, database_service: DatabaseService | str = None, logger=None):
         """Initialize."""
 
         def _prepare_whitelist(whitelist, blacklist):
             if blacklist:
                 whitelist = {col.name for col in self.table.columns} if whitelist is None else set(whitelist)
                 return frozenset(whitelist.difference(set(blacklist)))
             elif whitelist:
@@ -454,34 +440,34 @@
     def delete_condition_hook(sql):
         """Set up specific delete conditions."""
         return sql
 
     def _create_primary_key_condition_for_single_key(self, sql, _id: _Id):
         return sql.where(self._primary_key == _id)
 
-    def _create_list_primary_key_condition_for_single_key(self, sql, _id: Union[_Id, Collection[_Id]]):
+    def _create_list_primary_key_condition_for_single_key(self, sql, _id: _Id | Collection[_Id]):
         if not isinstance(_id, (list, tuple, set)):
             _id = [_id]
         return sql.where(self._primary_key.in_(_id))
 
-    def _parse_composite_id(self, _id: Union[Dict[str, _Id], Collection[_Id], _Id]):
+    def _parse_composite_id(self, _id: dict[str, _Id] | Collection[_Id] | _Id):
         conditions = []
         try:
             if isinstance(_id, dict):
                 for col in self._primary_key:
                     conditions.append(col == _id[col.name])
             else:
                 for value, col in zip(_id, self._primary_key):
                     conditions.append(col == value)
         except KeyError:
             raise ValidationError('Primary key field is not present.')
         else:
             return sa.and_(*conditions)
 
-    def _create_list_primary_key_condition_for_composite_key(self, sql, _id: Union[_Id, Collection[_Id]]):
+    def _create_list_primary_key_condition_for_composite_key(self, sql, _id: _Id | Collection[_Id]):
         if not isinstance(_id, (list, tuple, set)):
             _id = [_id]
         condition = sa.or_(*(self._parse_composite_id(n) for n in _id))
         return sql.where(condition)
 
     def _create_primary_key_condition_for_composite_key(self, sql, _id):
         condition = self._parse_composite_id(_id)
@@ -565,15 +551,15 @@
         if table is None:
             table = self.table
         sql = table.select().with_only_columns(*self._primary_key_list)
         sql = self._list_primary_key_condition(sql, _id)
         sql = self.get_condition_hook(sql)
         return sql
 
-    async def m_exists(self, id: Collection[_Id], _connection=None) -> FrozenSet[_Id]:
+    async def m_exists(self, id: Collection[_Id], _connection=None) -> frozenset[_Id]:
         """Return a set of existing IDs for a list of IDs.
 
         If you have composite primary keys you should pass dictionary objects
         in id field, like this:
 
         .. code-block:: python
 
@@ -597,15 +583,15 @@
 
     def _sql_get_column(self, table, column: str):
         """Return an SQLAlchemy column by its name."""
         try:
             return self.table.columns[column]
         except KeyError:
             raise ValidationError(
-                'Requested field doesn\'t exists',
+                'Requested field does not exists',
                 obj=table.name,
                 field=column,
                 service=self.service_name,
                 code=SQLService.ErrorCode.FIELD_DOES_NOT_EXISTS,
             )
 
     def _sql_get_columns(self, columns, table=None) -> list:
@@ -633,15 +619,14 @@
                 virtual = [sa.text(value + f' AS {name}') for name, value in self.virtual_columns.items()]
                 columns = [*columns, *virtual]
         else:
             if isinstance(columns, str):
                 columns = [columns]
 
             if self.virtual_columns:
-
                 _columns = []
 
                 for column in columns:
                     if column in self.virtual_columns:
                         value = self.virtual_columns[column]
                         _columns.append(sa.text(value + f' AS {column}'))
                     elif self.select_columns:
@@ -657,15 +642,15 @@
                     columns = [self._sql_get_column(table, key) for key in columns if key in self.select_columns]
                 else:
                     columns = [self._sql_get_column(table, key) for key in columns]
 
         return columns
 
     @staticmethod
-    def _filter_columns(columns: List[sa.Column], whitelist: Optional[frozenset]):
+    def _filter_columns(columns: list[sa.Column], whitelist: frozenset | None):
         if whitelist is None:
             return columns
         else:
             return [col for col in columns if col.name in whitelist]
 
     def _create_get_query(self, _id: _Id, columns, table=None):
         if table is None:
@@ -693,47 +678,53 @@
             raise ValidationError('Null "columns" param is not allowed in a get query.')
 
         sql = self._create_get_query(id, columns)
         result = await self._wrap_get(_connection, sql)
         result = result.first()
         if not result:
             raise NotFound(
-                'Object doesn\'t exist.',
+                'Object does not exist.',
                 service=self.service_name,
                 object_id=str(id),
                 code=SQLService.ErrorCode.NOT_FOUND,
             )
         if columns:
             return result._asdict()
 
-    def _create_m_get_query(self, _id: Collection[_Id], columns, table=None):
+    def _create_m_get_query(self, _id: Collection[_Id], conditions: _Condition, columns, table=None):
         if table is None:
             table = self.table
         columns = self._sql_get_columns(columns, table=table)
         sql = table.select().with_only_columns(*columns)
-        sql = self._list_primary_key_condition(sql, _id)
+        if _id:
+            sql = self._list_primary_key_condition(sql, _id)
+        if conditions:
+            sql = self._create_conditions(sql, conditions, table)
         sql = self.get_condition_hook(sql)
+        sql = sql.limit(self.MAX_GET_QUERY_SIZE)
         return sql
 
-    async def m_get(self, id: Collection[_Id], columns: _Columns = '*', _connection=None) -> List[_Row]:
+    async def m_get(
+        self, id: Collection[_Id] = None, conditions: _Condition = None, columns: _Columns = '*', _connection=None
+    ) -> list[_Row]:
         """Return multiple objects.
 
         Objects that don't exist will be skipped.
         Returns all data at once without pagination. Use `SQLService.list` if
         you want pagination or sorting.
 
         If you have composite primary keys you should pass dictionary objects
         in id field, like this:
 
         .. code-block:: python
 
             await service.m_get([{'id': 1, 'key': 'abc'}, ...], ...)
 
         """
-        sql = self._create_m_get_query(id, columns)
+        sql = self._create_m_get_query(id, conditions, columns)
         result = await self._wrap_get(_connection, sql)
         return [row._asdict() for row in result.all()]
 
     def _create_delete_query(self, _id: _Id, columns, table=None):
         if table is None:
             table = self.table
         columns = self._sql_get_columns(columns, table=table)
@@ -759,15 +750,15 @@
         :raises NotFound: if object doesn't exist or already was deleted
         """
         sql = self._create_delete_query(id, columns)
         result = await self._wrap_delete(_connection, sql)
         result = result.first()
         if result is None:
             raise NotFound(
-                'Object doesn\'t exist thus it can\'t be removed.',
+                'Object does not exist thus it cannot be removed.',
                 service=self.service_name,
                 object_id=str(id),
                 code=SQLService.ErrorCode.NOT_FOUND,
             )
         if columns:
             return result._asdict()
 
@@ -782,15 +773,15 @@
             sql = self._create_conditions(sql, conditions, table)
         sql = self.delete_condition_hook(sql)
         sql = sql.returning(*columns)
         return sql
 
     async def m_delete(
         self, id: Collection[_Id] = None, conditions: _Condition = None, columns: _Columns = None, _connection=None
-    ) -> List[_Row]:
+    ) -> list[_Row]:
         """Remove multiple objects from a table. Non-existing objects will be skipped.
 
         If you have composite primary keys you should pass dictionary objects
         in id field, like this:
 
         .. code-block:: python
 
@@ -898,15 +889,15 @@
         self,
         data: Collection[dict],
         columns: _Columns = '*',
         _connection=None,
         on_conflict: str = None,
         on_conflict_keys: list = None,
         on_conflict_values: dict = None,
-    ) -> List[_Row]:
+    ) -> list[_Row]:
         """Create multiple objects.
 
         :param data: list of objects data
         :param columns: columns to return, None for no return
         :param on_conflict: on conflict clause if required ('do_nothing', 'do_update')
         :param on_conflict_keys: list of on conflict constraints
         :param on_conflict_values: an object with on conflict values, used only by `do_update` clause
@@ -978,15 +969,15 @@
             sql = self._create_conditions(sql, conditions, table)
         sql = self.update_condition_hook(sql)
         sql = sql.returning(*columns)
         return sql
 
     async def m_update(
         self, id: Collection[_Id], data: dict, conditions: _Condition = None, columns: _Columns = '*', _connection=None
-    ) -> List[_Row]:
+    ) -> list[_Row]:
         """Update multiple objects with the same data. Non-existing objects will be skipped.
 
         If you have composite primary keys you should pass dictionary objects
         in id field, like this:
 
         .. code-block:: python
 
@@ -1375,15 +1366,15 @@
         self.root_dir = Path(root_dir).resolve()
         self.fixtures = fixtures
         self.empty_tables_only = empty_tables_only
         self.load_on_init = load_on_init
 
     async def init(self):
         if not self.root_dir.exists():
-            self.logger.warn('Fixture path does not exist', root_dir=str(self.root_dir))
+            self.logger.warning('Fixture path does not exist', root_dir=str(self.root_dir))
         if self.load_on_init:
             await self.load_all()
 
     async def load_all(self) -> None:
         """Load all fixtures in the root dir."""
         for path in self.root_dir.rglob('*.json'):
             if self.fixtures and path.stem not in self.fixtures:
@@ -1432,15 +1423,15 @@
     """Simple migration tool."""
 
     class State(TypedDict, total=False):
         """Migration state as in the migrations json file."""
 
         id: int  #: identifier
         comments: str  #: commit SHA
-        commands: List[str]  #: command or a set of commands to perform
+        commands: list[str]  #: command or a set of commands to perform
 
     table = sa.Table('db_info', sa.MetaData(), sa.Column('key', sa.TEXT), sa.Column('value', sa_pg.JSONB))
     _state_key = 'state'
     _null_state = -1
 
     def __init__(
         self,
@@ -1497,15 +1488,15 @@
         :param to_: state to migrate to (by default the last state is used)
         :param migrations_file: optional migrations file path
         :return: current state id
         """
         if migrations_file is None:
             migrations_file = self._migrations_file
         with open(migrations_file) as f:
-            migrations: List[DatabaseMigrationService.State] = load(f)
+            migrations: list[DatabaseMigrationService.State] = load(f)
         if not migrations:
             return self._null_state
         identifier = await self._locks.acquire(self._lock_key)  # TODO: lock context
         try:
             state_id = await self.get_state()
             self.logger.debug('Current state: #%d.', state_id)
             if from_ is None:
@@ -1544,10 +1535,62 @@
             await self._db.execute(sql)
             state_id = self._null_state
         else:
             state_id = state['value']
         return state_id
 
 
+class PermHook(PublicInterface, abc.ABC):
+    """Sql service with a user permissions hook.
+
+    it uses 'user_id' column by default to check if objects can be edited or viewed by users.
+    You should modify `_set_user_condition()` if you intend to use different columns.
+    """
+
+    service_name: str
+    table: sa.Table
+
+    class Permission(Enum):
+        """User permissions.
+
+        These keys will be joined with <service_name> to create unique permission keys for each
+        service.
+        """
+
+        MODIFY_OTHERS = 'modify_others'
+        VIEW_OTHERS = 'view_others'
+
+    @final
+    @cached_property
+    def permission_modify(self) -> str:
+        """Get a modify permission key."""
+        return f'{self.service_name}.{self.Permission.MODIFY_OTHERS.value}'
+
+    @final
+    @cached_property
+    def permission_view(self) -> str:
+        """Get a view permission key."""
+        return f'{self.service_name}.{self.Permission.VIEW_OTHERS.value}'
+
+    def _set_user_condition(self, sql, permission: str):
+        """Place user condition."""
+        if not self.has_permission(permission):
+            user_id = self.get_user_id()
+            sql = sql.where(self.table.c.user_id == user_id)
+        return sql
+
+    def _update_condition_hook(self, sql):
+        """Place user condition on update operations."""
+        return self._set_user_condition(sql, self.permission_modify)
+
+    def _delete_condition_hook(self, sql):
+        """Place user condition on delete operations."""
+        return self._update_condition_hook(sql)
+
+    def _get_condition_hook(self, sql):
+        """Place user condition on get and list operations."""
+        return self._set_user_condition(sql, self.permission_view)
+
+
 SERVICE_CLASS_REGISTRY.register(DatabaseService)
 SERVICE_CLASS_REGISTRY.register(DatabaseMigrationService)
 SERVICE_CLASS_REGISTRY.register(FixtureService)
```

## Comparing `kaiju_db-2.1.7.dist-info/LICENSE` & `kaiju_db-2.1.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_db-2.1.7.dist-info/METADATA` & `kaiju_db-2.1.8.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 Metadata-Version: 2.1
 Name: kaiju-db
-Version: 2.1.7
+Version: 2.1.8
 Summary: Postgresql db services and tools
 Home-page: https://gitlab.com/kaiju-python/kaiju-db
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: asyncpg (>=0.27)
+Requires-Dist: asyncpg (>=0.28)
 Requires-Dist: greenlet (>=2.0.2)
-Requires-Dist: sqlalchemy[asyncio] (>=2.0.17)
+Requires-Dist: sqlalchemy[asyncio] (>=2.0.19)
 Requires-Dist: sqlalchemy-utils (>=0.41)
 Requires-Dist: kaiju-tools (<3,>=2)
 Provides-Extra: dev
 Requires-Dist: bump2version (>=1.0) ; extra == 'dev'
 Requires-Dist: pyroma (>=4.1) ; extra == 'dev'
 Requires-Dist: bandit (>=1.7) ; extra == 'dev'
 Requires-Dist: black (>=22.12) ; extra == 'dev'
 Requires-Dist: flake8 (>=6.0) ; extra == 'dev'
+Requires-Dist: flake8-walrus (>=1.2.0) ; extra == 'dev'
 Requires-Dist: pyproject-flake8 ; extra == 'dev'
 Requires-Dist: pre-commit (>=3.1) ; extra == 'dev'
 Requires-Dist: pydocstyle (>=6.3) ; extra == 'dev'
 Requires-Dist: setup-cfg-fmt (>=2.2) ; extra == 'dev'
 Requires-Dist: restructuredtext-lint (>=1.4) ; extra == 'dev'
 Requires-Dist: tox (>=3.28) ; extra == 'dev'
 Requires-Dist: tox-pyenv (>=1.1) ; extra == 'dev'
 Requires-Dist: pip-tools (>=6.13) ; extra == 'dev'
 Requires-Dist: pyupgrade (>=3.4) ; extra == 'dev'
 Requires-Dist: towncrier (>=23.6) ; extra == 'dev'
+Requires-Dist: isort (>=5.12.0) ; extra == 'dev'
+Requires-Dist: xenon (>=0.9.0) ; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: sphinx ; extra == 'docs'
 Requires-Dist: python-docs-theme ; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest (>=7.4) ; extra == 'test'
 Requires-Dist: pytest-asyncio (>=0.21) ; extra == 'test'
 Requires-Dist: docker (>=6.1.3) ; extra == 'test'
@@ -62,15 +63,15 @@
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style - Black
 
 Summary
 -------
 
-**Python** >=3.8
+**Python** >=3.11
 **Postgresql** >= 14
 
 `Project documentation <https://kaiju-db.readthedocs.io/en/latest/>`_
 
 System and user tasks management classes.
 They are used to schedule and execute sets of RPC commands across applications.
```

## Comparing `kaiju_db-2.1.7.dist-info/RECORD` & `kaiju_db-2.1.8.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-kaiju_db/__init__.py,sha256=TcVf9qx07DH8TF-AO-Nc8iEmPsXtEBRUfqFh4PdbxSA,183
+kaiju_db/__init__.py,sha256=sN9E1RDeZEKB9nKNTDI_kId0ukHfMcrIpZau_nQOSNs,184
 kaiju_db/functions.py,sha256=JUHNd5uYbEtziTsihE-iPctYraUC-S3pfC2mo3EmtPo,3740
-kaiju_db/services.py,sha256=ItReJP7012cg53euK-4Af4NZGtYexVgxZqCy4bfLFvA,59537
+kaiju_db/services.py,sha256=rBrxnw_KqNVP0ilVWmQiYDa-czZS51BTe4y9SG0tAcc,61457
 kaiju_db/types.py,sha256=0ORvc2CaCcKUNibTR5o9EI5DOFQjM_uDg5S58aF8MyU,453
 kaiju_db/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kaiju_db/tests/fixtures.py,sha256=XtkmjBFFPbcBdUWNJBiGanrHjrPQW1yYzoC61sxxzD4,3292
 kaiju_db/tests/test_db.py,sha256=bVpj8sTiANdtet2hoiRefZbf3mAsGzkw0s4RbBF0pAg,4846
-kaiju_db-2.1.7.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
-kaiju_db-2.1.7.dist-info/METADATA,sha256=SSOEe4iP6Vp328eQ8GQUHksEJ07RTNxi6RynV3nEGm8,3204
-kaiju_db-2.1.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-kaiju_db-2.1.7.dist-info/top_level.txt,sha256=-jcfPgSkIz8rxFCPp_XIg5g9tVsDmBd1wdxayb_mkNU,9
-kaiju_db-2.1.7.dist-info/RECORD,,
+kaiju_db-2.1.8.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
+kaiju_db-2.1.8.dist-info/METADATA,sha256=d6EGkMhjC0DEZ3MEZvEuU9Eq6kRFOUqBHUmNBdtCCvA,3259
+kaiju_db-2.1.8.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+kaiju_db-2.1.8.dist-info/top_level.txt,sha256=-jcfPgSkIz8rxFCPp_XIg5g9tVsDmBd1wdxayb_mkNU,9
+kaiju_db-2.1.8.dist-info/RECORD,,
```

