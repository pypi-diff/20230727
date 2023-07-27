# Comparing `tmp/mongodb_odm-0.2.2.tar.gz` & `tmp/mongodb_odm-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodb_odm-0.2.2.tar", max compression
+gzip compressed data, was "mongodb_odm-0.2.3.tar", max compression
```

## Comparing `mongodb_odm-0.2.2.tar` & `mongodb_odm-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1056 2023-03-31 21:18:41.236449 mongodb_odm-0.2.2/LICENSE
--rw-r--r--   0        0        0     7214 2023-04-07 17:33:31.447106 mongodb_odm-0.2.2/README.md
--rw-r--r--   0        0        0      897 2023-04-24 06:10:00.161951 mongodb_odm-0.2.2/mongodb_odm/__init__.py
--rw-r--r--   0        0        0     1540 2023-04-07 17:33:31.451106 mongodb_odm-0.2.2/mongodb_odm/connection.py
--rw-r--r--   0        0        0     1230 2023-04-07 17:33:31.451106 mongodb_odm-0.2.2/mongodb_odm/data_conversion.py
--rw-r--r--   0        0        0       91 2023-03-31 21:18:41.240449 mongodb_odm-0.2.2/mongodb_odm/exceptions.py
--rw-r--r--   0        0        0     2824 2023-03-31 21:18:41.240449 mongodb_odm-0.2.2/mongodb_odm/fields.py
--rw-r--r--   0        0        0    14304 2023-04-24 06:10:00.165951 mongodb_odm-0.2.2/mongodb_odm/models.py
--rw-r--r--   0        0        0        0 2023-04-24 06:10:00.165951 mongodb_odm-0.2.2/mongodb_odm/py.typed
--rw-r--r--   0        0        0      577 2023-04-07 17:33:31.451106 mongodb_odm-0.2.2/mongodb_odm/types.py
--rw-r--r--   0        0        0        0 2023-03-31 21:18:41.240449 mongodb_odm-0.2.2/mongodb_odm/utils/__init__.py
--rw-r--r--   0        0        0      310 2023-04-07 17:33:31.451106 mongodb_odm-0.2.2/mongodb_odm/utils/_internal_models.py
--rw-r--r--   0        0        0     5453 2023-04-07 17:33:31.451106 mongodb_odm-0.2.2/mongodb_odm/utils/apply_indexes.py
--rw-r--r--   0        0        0     1566 2023-04-07 17:33:31.451106 mongodb_odm-0.2.2/mongodb_odm/utils/utils.py
--rw-r--r--   0        0        0     2633 2023-04-24 06:10:47.633935 mongodb_odm-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     8212 1970-01-01 00:00:00.000000 mongodb_odm-0.2.2/setup.py
--rw-r--r--   0        0        0     8869 1970-01-01 00:00:00.000000 mongodb_odm-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-07-21 16:45:45.671118 mongodb_odm-0.2.3/LICENSE
+-rw-r--r--   0        0        0     7214 2023-07-21 16:45:45.671118 mongodb_odm-0.2.3/README.md
+-rw-r--r--   0        0        0      897 2023-07-21 16:45:45.675118 mongodb_odm-0.2.3/mongodb_odm/__init__.py
+-rw-r--r--   0        0        0     2096 2023-07-27 14:54:47.606988 mongodb_odm-0.2.3/mongodb_odm/connection.py
+-rw-r--r--   0        0        0     1230 2023-07-21 16:45:45.675118 mongodb_odm-0.2.3/mongodb_odm/data_conversion.py
+-rw-r--r--   0        0        0      138 2023-07-27 14:54:47.606988 mongodb_odm-0.2.3/mongodb_odm/exceptions.py
+-rw-r--r--   0        0        0     2824 2023-07-21 16:45:45.675118 mongodb_odm-0.2.3/mongodb_odm/fields.py
+-rw-r--r--   0        0        0    15230 2023-07-27 14:54:47.606988 mongodb_odm-0.2.3/mongodb_odm/models.py
+-rw-r--r--   0        0        0        0 2023-07-21 16:45:45.675118 mongodb_odm-0.2.3/mongodb_odm/py.typed
+-rw-r--r--   0        0        0      577 2023-07-21 16:45:45.675118 mongodb_odm-0.2.3/mongodb_odm/types.py
+-rw-r--r--   0        0        0        0 2023-07-21 16:45:45.675118 mongodb_odm-0.2.3/mongodb_odm/utils/__init__.py
+-rw-r--r--   0        0        0      506 2023-07-27 14:54:47.606988 mongodb_odm-0.2.3/mongodb_odm/utils/_internal_models.py
+-rw-r--r--   0        0        0     5694 2023-07-27 14:54:47.606988 mongodb_odm-0.2.3/mongodb_odm/utils/apply_indexes.py
+-rw-r--r--   0        0        0     1725 2023-07-27 14:54:47.606988 mongodb_odm-0.2.3/mongodb_odm/utils/utils.py
+-rw-r--r--   0        0        0     2633 2023-07-27 16:03:19.471299 mongodb_odm-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     8667 1970-01-01 00:00:00.000000 mongodb_odm-0.2.3/PKG-INFO
```

### Comparing `mongodb_odm-0.2.2/LICENSE` & `mongodb_odm-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mongodb_odm-0.2.2/README.md` & `mongodb_odm-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `mongodb_odm-0.2.2/mongodb_odm/__init__.py` & `mongodb_odm-0.2.3/mongodb_odm/__init__.py`

 * *Files identical despite different names*

### Comparing `mongodb_odm-0.2.2/mongodb_odm/connection.py` & `mongodb_odm-0.2.3/mongodb_odm/connection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 import logging
-from typing import Any
+from typing import Any, Optional, Set
 
 from pymongo import MongoClient
 from pymongo.database import Database
 
-from .exceptions import ConnectionExist
+from .exceptions import ConnectionExist, InvalidConnection
 from .utils._internal_models import Connection
 
 logger = logging.getLogger(__name__)
 
 
 __connection_obj = Connection()
 
 
 def _get_connection_client(url: str) -> MongoClient[Any]:
     return MongoClient(url)
 
 
-def connect(url: str) -> MongoClient[Any]:
+def connect(url: str, databases: Optional[Set[str]] = None) -> MongoClient[Any]:
     if __connection_obj.client is not None:
         logger.warning("Already have an connection.")
         return __connection_obj.client
+
+    if databases is None:
+        databases = set()
+    client = _get_connection_client(url)
+    default_database = client.get_default_database().name
+    databases.add(default_database)
+
     __connection_obj.url = url
-    __connection_obj.client = _get_connection_client(url)
+    __connection_obj.databases = databases
+    __connection_obj.client = client
     logger.info("Connection established successfully")
     return __connection_obj.client
 
 
 def disconnect() -> bool:
     if __connection_obj.client:
         __connection_obj.client.close()
@@ -51,9 +59,14 @@
             return connect(__connection_obj.url)
         else:
             raise ConnectionExist("DB connection is not provided")
     else:
         return __connection_obj.client
 
 
-def db() -> Database[Any]:
-    return get_client().get_database()
+def db(database: Optional[str] = None) -> Database[Any]:
+    if database:
+        if not __connection_obj.databases or database not in __connection_obj.databases:
+            raise InvalidConnection(f'Invalid database key was passed "{database}"')
+        return get_client()[database]
+    else:
+        return get_client().get_database()
```

### Comparing `mongodb_odm-0.2.2/mongodb_odm/data_conversion.py` & `mongodb_odm-0.2.3/mongodb_odm/data_conversion.py`

 * *Files identical despite different names*

### Comparing `mongodb_odm-0.2.2/mongodb_odm/fields.py` & `mongodb_odm-0.2.3/mongodb_odm/fields.py`

 * *Files identical despite different names*

### Comparing `mongodb_odm-0.2.2/mongodb_odm/models.py` & `mongodb_odm-0.2.3/mongodb_odm/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,23 +11,27 @@
 from typing_extensions import Self
 
 from .connection import db, get_client
 from .data_conversion import dict2obj
 from .exceptions import ObjectDoesNotExist
 from .fields import Field
 from .types import DICT_TYPE, SORT_TYPE, ODMObjectId
-from .utils._internal_models import RelationalFieldInfo
-from .utils.utils import convert_model_to_collection, get_relationship_fields_info
+from .utils._internal_models import CollectionConfig, RelationalFieldInfo
+from .utils.utils import (
+    convert_model_to_collection,
+    get_database_name,
+    get_relationship_fields_info,
+)
 
 logger = logging.getLogger(__name__)
 INHERITANCE_FIELD_NAME = "_cls"
 
 RELATION_TYPE = Dict[str, RelationalFieldInfo]
 
-_cashed_collection: Dict[Any, Tuple[str, Optional[str]]] = {}
+_cashed_collection: Dict[Any, CollectionConfig] = {}
 _cashed_field_info: Dict[str, RELATION_TYPE] = {}
 
 
 def _clear_cache() -> None:
     global _cashed_collection, _cashed_field_info
     for key in [key for key in _cashed_collection.keys()]:
         del _cashed_collection[key]
@@ -41,14 +45,15 @@
         # Those fields will work as the default value of any child class.
         orm_mode: bool = True
         allow_population_by_field_name: bool = True
         collection_name: Optional[str] = None
         allow_inheritance: bool = False
         index_inheritance_field: bool = True
         indexes: List[IndexModel] = []
+        database: Optional[str] = None
 
     def __setattr__(self, key: str, value: Any) -> None:
         """
         Add '# type: ignore' as a comment if get type error while getting this value
         """
         self.__dict__[key] = value
 
@@ -72,37 +77,45 @@
                     f"Child Model{model.__name__} should declare a separate Config class."
                 )
             return base_model, model
         else:
             return model, None
 
     @classmethod
-    def __get_collection_config(cls) -> Tuple[str, Optional[str]]:
+    def __get_collection_config(cls) -> CollectionConfig:
         global _cashed_collection
         if cls in _cashed_collection:
             return _cashed_collection[cls]
 
         model, child_model = cls.__get_collection_class()
-        _cashed_collection[cls] = (
-            convert_model_to_collection(model),
-            convert_model_to_collection(child_model) if child_model else None,
+        _cashed_collection[cls] = CollectionConfig(
+            collection_name=convert_model_to_collection(model),
+            child_collection_name=convert_model_to_collection(child_model)
+            if child_model
+            else None,
+            database_name=get_database_name(model),
         )
         return _cashed_collection[cls]
 
     @classmethod
+    def _database_name(cls) -> Optional[str]:
+        config = cls.__get_collection_config()
+        return config.database_name
+
+    @classmethod
     def _get_collection_name(cls) -> str:
-        return cls.__get_collection_config()[0]
+        return cls.__get_collection_config().collection_name
 
     @classmethod
     def _get_child(cls) -> Optional[str]:
-        return cls.__get_collection_config()[1]
+        return cls.__get_collection_config().child_collection_name
 
     @classmethod
     def _get_collection(cls) -> Collection[Any]:
-        return db()[cls._get_collection_name()]
+        return db(cls._database_name())[cls._get_collection_name()]
 
     @classmethod
     def _db(cls) -> str:
         return cls._get_collection_name()
 
     @classmethod
     def get_inheritance_key(cls) -> Dict[str, Optional[str]]:
@@ -162,35 +175,43 @@
         inserted_id = _collection.insert_one(data, **kwargs).inserted_id
         self.__dict__.update({"_id": inserted_id, "id": inserted_id})
         return self
 
     @classmethod
     def find_raw(
         cls,
-        filter: DICT_TYPE = {},
-        projection: Dict[str, int] = {},
+        filter: Optional[DICT_TYPE] = None,
+        projection: Optional[DICT_TYPE] = None,
         **kwargs: Any,
     ) -> Cursor[Any]:
+        if filter is None:
+            filter = {}
+        if projection is None:
+            projection = {}
+
         _collection = cls._get_collection()
         if cls._get_child() is not None:
             filter = {**cls.get_inheritance_key(), **filter}
         if projection:
             return _collection.find(filter, projection, **kwargs)
         return _collection.find(filter, **kwargs)
 
     @classmethod
     def find(
         cls,
-        filter: DICT_TYPE = {},
-        projection: Dict[str, int] = {},
+        filter: Optional[DICT_TYPE] = None,
+        projection: Optional[DICT_TYPE] = None,
         sort: Optional[SORT_TYPE] = None,
         skip: Optional[int] = None,
         limit: Optional[int] = None,
         **kwargs: Any,
     ) -> Iterator[Self]:
+        if filter is None:
+            filter = {}
+
         qs = cls.find_raw(filter, projection, **kwargs)
         if sort:
             qs = qs.sort(sort)
         if skip:
             qs = qs.skip(skip)
         if limit:
             qs = qs.limit(limit)
@@ -210,19 +231,22 @@
                 yield model_children[data[INHERITANCE_FIELD_NAME]](**data)
             else:
                 yield cls(**data)
 
     @classmethod
     def find_one(
         cls,
-        filter: DICT_TYPE = {},
-        projection: Dict[str, int] = {},
+        filter: Optional[DICT_TYPE] = None,
+        projection: Optional[DICT_TYPE] = None,
         sort: Optional[SORT_TYPE] = None,
         **kwargs: Any,
     ) -> Optional[Self]:
+        if filter is None:
+            filter = {}
+
         qs = cls.find_raw(filter, projection=projection, **kwargs)
         if sort:
             qs = qs.sort(sort)
         for data in qs.limit(1):
             """limit 1 is equivalent to find_one and that is implemented in pymongo find_one"""
             return cls(**data)
         return None
@@ -248,22 +272,28 @@
     ) -> Tuple[Self, bool]:
         obj = cls.find_one(filter, sort=sort, **kwargs)
         if obj:
             return obj, False
         return cls(**filter).create(), True
 
     @classmethod
-    def count_documents(cls, filter: DICT_TYPE = {}, **kwargs: Any) -> int:
+    def count_documents(cls, filter: Optional[DICT_TYPE] = None, **kwargs: Any) -> int:
+        if filter is None:
+            filter = {}
+
         _collection = cls._get_collection()
         if cls._get_child() is not None:
             filter = {**cls.get_inheritance_key(), **filter}
         return _collection.count_documents(filter, **kwargs)
 
     @classmethod
-    def exists(cls, filter: DICT_TYPE = {}, **kwargs: Any) -> bool:
+    def exists(cls, filter: Optional[DICT_TYPE] = None, **kwargs: Any) -> bool:
+        if filter is None:
+            filter = {}
+
         _collection = cls._get_collection()
         if cls._get_child() is not None:
             filter = {**cls.get_inheritance_key(), **filter}
         return _collection.count_documents(filter, **kwargs, limit=1) >= 1
 
     @classmethod
     def aggregate(
@@ -287,23 +317,26 @@
         for obj in _collection.aggregate(pipeline, **kwargs):
             if get_raw is True:
                 yield obj
             else:
                 yield dict2obj(obj)
 
     @classmethod
-    def get_random_one(cls, filter: DICT_TYPE = {}, **kwargs: Any) -> Self:
+    def get_random_one(cls, filter: Optional[DICT_TYPE] = None, **kwargs: Any) -> Self:
+        if filter is None:
+            filter = {}
+
         if cls._get_child() is not None:
             filter = {**cls.get_inheritance_key(), **filter}
         pipeline = [{"$match": filter}, {"$sample": {"size": 1}}]
         for data in cls.aggregate(pipeline, get_raw=True, **kwargs):
             return cls(**data)
         raise ObjectDoesNotExist("Object not found.")
 
-    def update(self, raw: DICT_TYPE = {}, **kwargs: Any) -> UpdateResult:
+    def update(self, raw: Optional[DICT_TYPE] = None, **kwargs: Any) -> UpdateResult:
         filter = {"_id": self._id}
         if raw:
             updated_data = raw
         else:
             updated_data = {"$set": self.to_mongo()}
         if hasattr(self, "updated_at"):
             datetime_now = datetime.utcnow()
@@ -312,42 +345,42 @@
             updated_data["$set"]["updated_at"] = datetime_now
             self.__dict__.update({"updated_at": datetime_now})
 
         return self.update_one(filter, updated_data, **kwargs)
 
     @classmethod
     def update_one(
-        cls, filter: DICT_TYPE = {}, data: DICT_TYPE = {}, **kwargs: Any
+        cls, filter: DICT_TYPE, data: DICT_TYPE, **kwargs: Any
     ) -> UpdateResult:
         _collection = cls._get_collection()
         if cls._get_child() is not None:
             filter = {**cls.get_inheritance_key(), **filter}
         return _collection.update_one(filter, data, **kwargs)
 
     @classmethod
     def update_many(
-        cls, filter: DICT_TYPE = {}, data: DICT_TYPE = {}, **kwargs: Any
+        cls, filter: DICT_TYPE, data: DICT_TYPE, **kwargs: Any
     ) -> UpdateResult:
         _collection = cls._get_collection()
         if cls._get_child() is not None:
             filter = {**cls.get_inheritance_key(), **filter}
         return _collection.update_many(filter, data, **kwargs)
 
     def delete(self, **kwargs: Any) -> DeleteResult:
         return self.delete_one({"_id": self._id}, **kwargs)
 
     @classmethod
-    def delete_one(cls, filter: DICT_TYPE = {}, **kwargs: Any) -> DeleteResult:
+    def delete_one(cls, filter: DICT_TYPE, **kwargs: Any) -> DeleteResult:
         _collection = cls._get_collection()
         if cls._get_child() is not None:
             filter = {**cls.get_inheritance_key(), **filter}
         return _collection.delete_one(filter, **kwargs)
 
     @classmethod
-    def delete_many(cls, filter: DICT_TYPE = {}, **kwargs: Any) -> DeleteResult:
+    def delete_many(cls, filter: DICT_TYPE, **kwargs: Any) -> DeleteResult:
         _collection = cls._get_collection()
         if cls._get_child() is not None:
             filter = {**cls.get_inheritance_key(), **filter}
         return _collection.delete_many(filter, **kwargs)
 
     @classmethod
     def bulk_write(
@@ -356,22 +389,25 @@
         _collection = cls._get_collection()
         return _collection.bulk_write(requests, **kwargs)
 
     @classmethod
     def load_related(
         cls,
         object_list: Union[Iterator[Self], Sequence[Self]],
-        fields: List[str] = [],
+        fields: Optional[List[str]] = None,
         **kwargs: Any,
     ) -> Sequence[Self]:
+        if fields is None:
+            fields = []
+
         """Get model relational field from cache"""
         cached_field_info = cls.get_relational_field_info()
 
         """Match with user given fields"""
-        loadable_fields_info: DICT_TYPE = {}
+        loadable_fields_info: Optional[DICT_TYPE] = None
         if fields:
             loadable_fields_info = {}
             for field in fields:
                 if field not in cached_field_info:
                     raise Exception(f'Invalid field "{field}"')
                 loadable_fields_info[field] = cached_field_info[field]
         else:
```

### Comparing `mongodb_odm-0.2.2/mongodb_odm/types.py` & `mongodb_odm-0.2.3/mongodb_odm/types.py`

 * *Files identical despite different names*

### Comparing `mongodb_odm-0.2.2/mongodb_odm/utils/apply_indexes.py` & `mongodb_odm-0.2.3/mongodb_odm/utils/apply_indexes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 import logging
-from typing import Any, Dict, List, Tuple, Type
+from typing import Any, Dict, List, Optional, Tuple, Type
 
 from bson import SON
-from mongodb_odm.types import DICT_TYPE
+from pydantic import BaseModel
 from pymongo import ASCENDING, IndexModel
 
 from ..connection import db
 from ..models import INHERITANCE_FIELD_NAME, Document
 
 logger = logging.getLogger(__name__)
 
 
-def index_for_a_collection(operation: DICT_TYPE) -> Tuple[int, int]:
+class IndexOperation(BaseModel):
+    collection_name: str
+    create_indexes: List[Any]
+    database_name: Optional[str] = None
+
+
+def index_for_a_collection(operation: IndexOperation) -> Tuple[int, int]:
     """
     First get all indexes for a collection and match with operation.
     Remove full match object.
 
     If db_index partially match with operation_index then recreate/update it.
 
     For new_indexes unmatched with db_indexes create new index.
     For db_indexes unmatched with new_indexes drop indexes.
     """
     try:
-        collection = db()[operation["collection_name"]]
-        indexes = operation["create_indexes"]
+        collection = db(operation.database_name)[operation.collection_name]
+        indexes = operation.create_indexes
     except Exception:
         raise Exception("Invalid index object")
 
     db_indexes = []
     for index in collection.list_indexes():
         old_index = index.to_dict()  # type: ignore
         # Skip "_id" index since it's create by mongodb system
@@ -83,60 +89,62 @@
             new_indexes_store[new_index["name"]]
             for new_index in new_indexes
             if new_index
         ]
         try:
             collection.create_indexes(new_indexes)
         except Exception as e:
-            logger.error(f'\nProblem arise at "{operation["collection_name"]}": {e}\n')
+            logger.error(f'\nProblem arise at "{operation.collection_name}": {e}\n')
             raise e
 
     # TODO: apply action for update_indexes
 
     ne, de = len(new_indexes), len(delete_db_indexes)
     if ne > 0 or de > 0:
         logger.info(
-            f'Applied for "{operation["collection_name"]}": {de} deleted, {ne} added'
+            f'Applied for "{operation.collection_name}": {de} deleted, {ne} added'
         )
     return ne, de
 
 
 def get_model_indexes(model: Type[Document]) -> List[IndexModel]:
     if hasattr(model.Config, "indexes"):
         return list(model.Config.indexes)
     return []
 
 
-def get_all_indexes() -> List[DICT_TYPE]:
+def get_all_indexes() -> List[IndexOperation]:
     """
     First imports all child models of Document since it's the abstract parent model.
     Then retrieve all the child modules and will try to get indexes inside the Config class.
     """
-    operations: List[DICT_TYPE] = []
+    operations: List[IndexOperation] = []
     for model in Document.__subclasses__():
         indexes = get_model_indexes(model)
         if indexes:
-            collection_name = model._get_collection_name()
-            obj = {
-                "collection_name": collection_name,
-                "create_indexes": indexes,
-            }
+            obj = IndexOperation(
+                collection_name=model._get_collection_name(),
+                create_indexes=indexes,
+                database_name=model._database_name(),
+            )
             if (
                 hasattr(model.Config, "allow_inheritance")
                 and model.Config.allow_inheritance is True
             ):
                 """If a model has child model"""
                 if model.Config.index_inheritance_field is True:
                     """
                     No _cls indexes will apply if index_inheritance_field = False
                     """
-                    indexes.append(IndexModel([(INHERITANCE_FIELD_NAME, ASCENDING)]))
+                    obj.create_indexes.append(
+                        IndexModel([(INHERITANCE_FIELD_NAME, ASCENDING)])
+                    )
                 for child_model in model.__subclasses__():
                     """Get all indexes that are defined in child model"""
-                    indexes += get_model_indexes(child_model)
+                    obj.create_indexes += get_model_indexes(child_model)
             operations.append(obj)
     return operations
 
 
 def apply_indexes() -> None:
     """Run "python -m app.main apply-indexes" to apply and indexes."""
```

### Comparing `mongodb_odm-0.2.2/mongodb_odm/utils/utils.py` & `mongodb_odm-0.2.3/mongodb_odm/utils/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import re
-from typing import Any, Dict, List, Type
+from typing import Any, Dict, List, Optional, Type
 
 from pydantic import BaseModel
 
 from ..fields import _RelationshipInfo
 from ._internal_models import RelationalFieldInfo
 
 pattern = re.compile(r"(?<!^)(?=[A-Z])")
 
 
 def camel_to_snake(string: str) -> str:
     return pattern.sub("_", string).lower()
 
 
+def get_database_name(model: Any) -> Optional[str]:
+    if hasattr(model.Config, "database"):
+        return model.Config.database
+    return None
+
+
 def convert_model_to_collection(model: Any) -> str:
     if (
         hasattr(model.Config, "collection_name")
         and model.Config.collection_name is not None
     ):
         """By default model has Config in BaseModel"""
         return str(model.Config.collection_name)
```

### Comparing `mongodb_odm-0.2.2/pyproject.toml` & `mongodb_odm-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mongodb-odm"
-version = "0.2.2"
+version = "0.2.3"
 description = "MongoDB-ODM, NOSQL databases in Python, designed for simplicity, compatibility, and robustness."
 authors = ["Nayan Biswas <nayan32biswas@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 # homepage = "https://github.com/nayan32biswas/mongodb-odm"
 documentation = "https://mongodb-odm.readthedocs.io"
 repository = "https://github.com/nayan32biswas/mongodb-odm"
```

### Comparing `mongodb_odm-0.2.2/setup.py` & `mongodb_odm-0.2.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,514 +1,542 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 6573 203d  etup..packages =
-00000040: 205c 0a5b 276d 6f6e 676f 6462 5f6f 646d   \.['mongodb_odm
-00000050: 272c 2027 6d6f 6e67 6f64 625f 6f64 6d2e  ', 'mongodb_odm.
-00000060: 7574 696c 7327 5d0a 0a70 6163 6b61 6765  utils']..package
-00000070: 5f64 6174 6120 3d20 5c0a 7b27 273a 205b  _data = \.{'': [
-00000080: 272a 275d 7d0a 0a69 6e73 7461 6c6c 5f72  '*']}..install_r
-00000090: 6571 7569 7265 7320 3d20 5c0a 5b27 7079  equires = \.['py
-000000a0: 6461 6e74 6963 3e3d 312e 3130 2e37 2c3c  dantic>=1.10.7,<
-000000b0: 322e 302e 3027 2c20 2770 796d 6f6e 676f  2.0.0', 'pymongo
-000000c0: 5b73 7276 5d3e 3d34 2e33 2e33 2c3c 352e  [srv]>=4.3.3,<5.
-000000d0: 302e 3027 5d0a 0a73 6574 7570 5f6b 7761  0.0']..setup_kwa
-000000e0: 7267 7320 3d20 7b0a 2020 2020 276e 616d  rgs = {.    'nam
-000000f0: 6527 3a20 276d 6f6e 676f 6462 2d6f 646d  e': 'mongodb-odm
-00000100: 272c 0a20 2020 2027 7665 7273 696f 6e27  ',.    'version'
-00000110: 3a20 2730 2e32 2e32 272c 0a20 2020 2027  : '0.2.2',.    '
-00000120: 6465 7363 7269 7074 696f 6e27 3a20 274d  description': 'M
-00000130: 6f6e 676f 4442 2d4f 444d 2c20 4e4f 5351  ongoDB-ODM, NOSQ
-00000140: 4c20 6461 7461 6261 7365 7320 696e 2050  L databases in P
-00000150: 7974 686f 6e2c 2064 6573 6967 6e65 6420  ython, designed 
-00000160: 666f 7220 7369 6d70 6c69 6369 7479 2c20  for simplicity, 
-00000170: 636f 6d70 6174 6962 696c 6974 792c 2061  compatibility, a
-00000180: 6e64 2072 6f62 7573 746e 6573 732e 272c  nd robustness.',
-00000190: 0a20 2020 2027 6c6f 6e67 5f64 6573 6372  .    'long_descr
-000001a0: 6970 7469 6f6e 273a 2027 2320 4d6f 6e67  iption': '# Mong
-000001b0: 6f44 422d 4f44 4d5c 6e5c 6e3c 7020 616c  oDB-ODM\n\n<p al
-000001c0: 6967 6e3d 2263 656e 7465 7222 3e5c 6e20  ign="center">\n 
-000001d0: 2020 203c 656d 3e4d 6f6e 676f 4442 2d4f     <em>MongoDB-O
-000001e0: 444d 2c20 4e4f 5351 4c20 6461 7461 6261  DM, NOSQL databa
-000001f0: 7365 7320 696e 2050 7974 686f 6e2c 2064  ses in Python, d
-00000200: 6573 6967 6e65 6420 666f 7220 7369 6d70  esigned for simp
-00000210: 6c69 6369 7479 2c20 636f 6d70 6174 6962  licity, compatib
-00000220: 696c 6974 792c 2061 6e64 2072 6f62 7573  ility, and robus
-00000230: 746e 6573 732e 3c2f 656d 3e5c 6e3c 2f70  tness.</em>\n</p
-00000240: 3e5c 6e5c 6e3c 7020 616c 6967 6e3d 2263  >\n\n<p align="c
-00000250: 656e 7465 7222 3e5c 6e5c 6e3c 6120 6872  enter">\n\n<a hr
-00000260: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-00000270: 7562 2e63 6f6d 2f6e 6179 616e 3332 6269  ub.com/nayan32bi
-00000280: 7377 6173 2f6d 6f6e 676f 6462 2d6f 646d  swas/mongodb-odm
-00000290: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-000002a0: 7773 2f74 6573 742e 796d 6c22 2074 6172  ws/test.yml" tar
-000002b0: 6765 743d 225f 626c 616e 6b22 3e5c 6e20  get="_blank">\n 
-000002c0: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
-000002d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000002e0: 6e61 7961 6e33 3262 6973 7761 732f 6d6f  nayan32biswas/mo
-000002f0: 6e67 6f64 622d 6f64 6d2f 6163 7469 6f6e  ngodb-odm/action
-00000300: 732f 776f 726b 666c 6f77 732f 7465 7374  s/workflows/test
-00000310: 2e79 6d6c 2f62 6164 6765 2e73 7667 3f62  .yml/badge.svg?b
-00000320: 7261 6e63 683d 6d61 696e 2665 7665 6e74  ranch=main&event
-00000330: 3d70 7573 6822 2061 6c74 3d22 5465 7374  =push" alt="Test
-00000340: 223e 5c6e 3c2f 613e 5c6e 3c61 2068 7265  ">\n</a>\n<a hre
-00000350: 663d 2268 7474 7073 3a2f 2f63 6f76 6572  f="https://cover
-00000360: 6167 652d 6261 6467 652e 7361 6d75 656c  age-badge.samuel
-00000370: 636f 6c76 696e 2e77 6f72 6b65 7273 2e64  colvin.workers.d
-00000380: 6576 2f72 6564 6972 6563 742f 6e61 7961  ev/redirect/naya
-00000390: 6e33 3262 6973 7761 732f 6d6f 6e67 6f64  n32biswas/mongod
-000003a0: 622d 6f64 6d22 2074 6172 6765 743d 225f  b-odm" target="_
-000003b0: 626c 616e 6b22 3e5c 6e20 2020 203c 696d  blank">\n    <im
-000003c0: 6720 7372 633d 2268 7474 7073 3a2f 2f63  g src="https://c
-000003d0: 6f76 6572 6167 652d 6261 6467 652e 7361  overage-badge.sa
-000003e0: 6d75 656c 636f 6c76 696e 2e77 6f72 6b65  muelcolvin.worke
-000003f0: 7273 2e64 6576 2f6e 6179 616e 3332 6269  rs.dev/nayan32bi
-00000400: 7377 6173 2f6d 6f6e 676f 6462 2d6f 646d  swas/mongodb-odm
-00000410: 2e73 7667 2220 616c 743d 2243 6f76 6572  .svg" alt="Cover
-00000420: 6167 6522 3e5c 6e3c 6272 202f 3e5c 6e3c  age">\n<br />\n<
-00000430: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000440: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-00000450: 2f6d 6f6e 676f 6462 2d6f 646d 2f22 2074  /mongodb-odm/" t
-00000460: 6172 6765 743d 225f 626c 616e 6b22 3e5c  arget="_blank">\
-00000470: 6e20 2020 203c 696d 6720 616c 743d 2250  n    <img alt="P
-00000480: 7950 4922 2073 7263 3d22 6874 7470 733a  yPI" src="https:
-00000490: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-000004a0: 2f70 7970 692f 762f 6d6f 6e67 6f64 622d  /pypi/v/mongodb-
-000004b0: 6f64 6d3f 636f 6c6f 723d 2532 3333 3444  odm?color=%2334D
-000004c0: 3035 3826 6c61 6265 6c3d 5079 5069 2532  058&label=PyPi%2
-000004d0: 3050 6163 6b61 6765 223e 5c6e 3c2f 613e  0Package">\n</a>
-000004e0: 5c6e 3c61 2068 7265 663d 2268 7474 7073  \n<a href="https
-000004f0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
-00000500: 6563 742f 6d6f 6e67 6f64 622d 6f64 6d2f  ect/mongodb-odm/
-00000510: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
-00000520: 223e 5c6e 2020 2020 3c69 6d67 2061 6c74  ">\n    <img alt
-00000530: 3d22 5079 5049 202d 2050 7974 686f 6e20  ="PyPI - Python 
-00000540: 5665 7273 696f 6e22 2073 7263 3d22 6874  Version" src="ht
-00000550: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000560: 732e 696f 2f70 7970 692f 7079 7665 7273  s.io/pypi/pyvers
-00000570: 696f 6e73 2f6d 6f6e 676f 6462 2d6f 646d  ions/mongodb-odm
-00000580: 3f63 6f6c 6f72 3d25 3233 3334 4430 3538  ?color=%2334D058
-00000590: 223e 5c6e 3c2f 613e 5c6e 5c6e 3c2f 703e  ">\n</a>\n\n</p>
-000005a0: 5c6e 5c6e 2d2d 2d5c 6e5c 6e2a 2a44 6f63  \n\n---\n\n**Doc
-000005b0: 756d 656e 7461 7469 6f6e 2a2a 3a20 3c61  umentation**: <a
-000005c0: 2068 7265 663d 2268 7474 7073 3a2f 2f6d   href="https://m
-000005d0: 6f6e 676f 6462 2d6f 646d 2e72 6561 6474  ongodb-odm.readt
-000005e0: 6865 646f 6373 2e69 6f22 2074 6172 6765  hedocs.io" targe
-000005f0: 743d 225f 626c 616e 6b22 3e68 7474 7073  t="_blank">https
-00000600: 3a2f 2f6d 6f6e 676f 6462 2d6f 646d 2e72  ://mongodb-odm.r
-00000610: 6561 6474 6865 646f 6373 2e69 6f3c 2f61  eadthedocs.io</a
-00000620: 3e5c 6e5c 6e2a 2a50 7950 692a 2a3a 203c  >\n\n**PyPi**: <
-00000630: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000640: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-00000650: 2f6d 6f6e 676f 6462 2d6f 646d 2220 7461  /mongodb-odm" ta
-00000660: 7267 6574 3d22 5f62 6c61 6e6b 223e 6874  rget="_blank">ht
-00000670: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-00000680: 726f 6a65 6374 2f6d 6f6e 676f 6462 2d6f  roject/mongodb-o
-00000690: 646d 3c2f 613e 5c6e 5c6e 2a2a 5265 706f  dm</a>\n\n**Repo
-000006a0: 7369 746f 7279 2a2a 3a20 3c61 2068 7265  sitory**: <a hre
-000006b0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-000006c0: 622e 636f 6d2f 6e61 7961 6e33 3262 6973  b.com/nayan32bis
-000006d0: 7761 732f 6d6f 6e67 6f64 622d 6f64 6d22  was/mongodb-odm"
-000006e0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-000006f0: 3e68 7474 7073 3a2f 2f67 6974 6875 622e  >https://github.
-00000700: 636f 6d2f 6e61 7961 6e33 3262 6973 7761  com/nayan32biswa
-00000710: 732f 6d6f 6e67 6f64 622d 6f64 6d3c 2f61  s/mongodb-odm</a
-00000720: 3e5c 6e5c 6e2d 2d2d 5c6e 5c6e 2323 2049  >\n\n---\n\n## I
-00000730: 6e74 726f 6475 6374 696f 6e5c 6e5c 6e54  ntroduction\n\nT
-00000740: 6865 2070 7572 706f 7365 206f 6620 7468  he purpose of th
-00000750: 6973 206d 6f64 756c 6520 6973 2074 6f20  is module is to 
-00000760: 7072 6f76 6964 6520 6561 7379 2061 6363  provide easy acc
-00000770: 6573 7320 746f 2074 6865 2064 6174 6162  ess to the datab
-00000780: 6173 6520 7769 7468 2074 6865 2070 7974  ase with the pyt
-00000790: 686f 6e20 6f62 6a65 6374 2066 6561 7475  hon object featu
-000007a0: 7265 2077 6974 6820 2a2a 4d6f 6e67 6f44  re with **MongoD
-000007b0: 422a 2a20 616e 6420 2a2a 5079 4d6f 6e67  B** and **PyMong
-000007c0: 6f2a 2a2e 2057 6974 6820 5079 4d6f 6e67  o**. With PyMong
-000007d0: 6f20 7468 6174 2077 6173 2076 6572 7920  o that was very 
-000007e0: 6561 7379 2074 6f20 6d61 6b65 2073 7065  easy to make spe
-000007f0: 6c6c 696e 6720 6d69 7374 616b 6573 2069  lling mistakes i
-00000800: 6e20 6120 636f 6c6c 6563 7469 6f6e 206e  n a collection n
-00000810: 616d 6520 7768 656e 2079 6f75 2061 7265  ame when you are
-00000820: 2064 6f69 6e67 2064 6174 6162 6173 6520   doing database 
-00000830: 6f70 6572 6174 696f 6e2e 2054 6869 7320  operation. This 
-00000840: 6d6f 6475 6c65 2070 726f 7669 6465 7320  module provides 
-00000850: 796f 7520 7769 7468 206d 696e 696d 616c  you with minimal
-00000860: 204f 444d 2077 6974 6820 6120 6d6f 6465   ODM with a mode
-00000870: 6c69 6e67 2066 6561 7475 7265 2073 6f20  ling feature so 
-00000880: 7468 6174 2079 6f75 2064 6f6e e280 9974  that you don...t
-00000890: 2068 6176 6520 746f 206c 6f6f 6b20 7570   have to look up
-000008a0: 2074 6865 204d 6f6e 676f 4442 2064 6173   the MongoDB das
-000008b0: 6862 6f61 7264 284d 6f6e 676f 2043 6f6d  hboard(Mongo Com
-000008c0: 7061 7373 2920 746f 206b 6e6f 7720 6162  pass) to know ab
-000008d0: 6f75 7420 6669 656c 6420 6e61 6d65 7320  out field names 
-000008e0: 6f72 2064 6174 6120 7479 7065 732e 5c6e  or data types.\n
-000008f0: 5c6e 2a2a 4d6f 6e67 6f44 422d 4f44 4d2a  \n**MongoDB-ODM*
-00000900: 2a20 6973 2062 6173 6564 206f 6e20 5079  * is based on Py
-00000910: 7468 6f6e 2074 7970 6520 616e 6e6f 7461  thon type annota
-00000920: 7469 6f6e 732c 2061 6e64 2070 6f77 6572  tions, and power
-00000930: 6564 2062 7920 3c61 2068 7265 663d 2268  ed by <a href="h
-00000940: 7474 7073 3a2f 2f70 796d 6f6e 676f 2e72  ttps://pymongo.r
-00000950: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00000960: 2f73 7461 626c 652f 2220 636c 6173 733d  /stable/" class=
-00000970: 2265 7874 6572 6e61 6c2d 6c69 6e6b 2220  "external-link" 
-00000980: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
-00000990: 5079 4d6f 6e67 6f3c 2f61 3e20 616e 6420  PyMongo</a> and 
-000009a0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-000009b0: 2f64 6f63 732e 7079 6461 6e74 6963 2e64  /docs.pydantic.d
-000009c0: 6576 2f22 2063 6c61 7373 3d22 6578 7465  ev/" class="exte
-000009d0: 726e 616c 2d6c 696e 6b22 2074 6172 6765  rnal-link" targe
-000009e0: 743d 225f 626c 616e 6b22 3e50 7964 616e  t="_blank">Pydan
-000009f0: 7469 633c 2f61 3e2e 5c6e 5c6e 5468 6520  tic</a>.\n\nThe 
-00000a00: 6b65 7920 6665 6174 7572 6573 2061 7265  key features are
-00000a10: 3a5c 6e5c 6e2d 202a 2a49 6e74 7569 7469  :\n\n- **Intuiti
-00000a20: 7665 2074 6f20 7772 6974 652a 2a3a 2047  ve to write**: G
-00000a30: 7265 6174 2065 6469 746f 7220 7375 7070  reat editor supp
-00000a40: 6f72 742e 2043 6f6d 706c 6574 696f 6e20  ort. Completion 
-00000a50: 6576 6572 7977 6865 7265 2e20 4c65 7373  everywhere. Less
-00000a60: 2074 696d 6520 6465 6275 6767 696e 672e   time debugging.
-00000a70: 2044 6573 6967 6e65 6420 746f 2062 6520   Designed to be 
-00000a80: 6561 7379 2074 6f20 7573 6520 616e 6420  easy to use and 
-00000a90: 6c65 6172 6e2e 204c 6573 7320 7469 6d65  learn. Less time
-00000aa0: 2072 6561 6469 6e67 2064 6f63 732e 5c6e   reading docs.\n
-00000ab0: 2d20 2a2a 4561 7379 2074 6f20 7573 652a  - **Easy to use*
-00000ac0: 2a3a 2049 7420 6861 7320 7365 6e73 6962  *: It has sensib
-00000ad0: 6c65 2064 6566 6175 6c74 7320 616e 6420  le defaults and 
-00000ae0: 646f 6573 2061 206c 6f74 206f 6620 776f  does a lot of wo
-00000af0: 726b 2075 6e64 6572 6e65 6174 6820 746f  rk underneath to
-00000b00: 2073 696d 706c 6966 7920 7468 6520 636f   simplify the co
-00000b10: 6465 2079 6f75 2077 7269 7465 2e5c 6e2d  de you write.\n-
-00000b20: 202a 2a43 6f6d 7061 7469 626c 652a 2a3a   **Compatible**:
-00000b30: 2049 7420 6973 2064 6573 6967 6e65 6420   It is designed 
-00000b40: 746f 2062 6520 636f 6d70 6174 6962 6c65  to be compatible
-00000b50: 2077 6974 6820 2a2a 4661 7374 4150 492a   with **FastAPI*
-00000b60: 2a2c 202a 2a50 7964 616e 7469 632a 2a2c  *, **Pydantic**,
-00000b70: 2061 6e64 202a 2a50 794d 6f6e 676f 2a2a   and **PyMongo**
-00000b80: 2e5c 6e2d 202a 2a45 7874 656e 7369 626c  .\n- **Extensibl
-00000b90: 652a 2a3a 2059 6f75 2068 6176 6520 616c  e**: You have al
-00000ba0: 6c20 7468 6520 706f 7765 7220 6f66 202a  l the power of *
-00000bb0: 2a50 794d 6f6e 676f 2a2a 2061 6e64 202a  *PyMongo** and *
-00000bc0: 2a50 7964 616e 7469 632a 2a20 756e 6465  *Pydantic** unde
-00000bd0: 726e 6561 7468 2e5c 6e2d 202a 2a53 686f  rneath.\n- **Sho
-00000be0: 7274 2a2a 3a20 4d69 6e69 6d69 7a65 2063  rt**: Minimize c
-00000bf0: 6f64 6520 6475 706c 6963 6174 696f 6e2e  ode duplication.
-00000c00: 2041 2073 696e 676c 6520 7479 7065 2061   A single type a
-00000c10: 6e6e 6f74 6174 696f 6e20 646f 6573 2061  nnotation does a
-00000c20: 206c 6f74 206f 6620 776f 726b 2e20 4e6f   lot of work. No
-00000c30: 206e 6565 6420 746f 2064 7570 6c69 6361   need to duplica
-00000c40: 7465 206d 6f64 656c 7320 696e 202a 2a50  te models in **P
-00000c50: 794d 6f6e 676f 2a2a 2061 6e64 2050 7964  yMongo** and Pyd
-00000c60: 616e 7469 632e 5c6e 5c6e 2d2d 2d5c 6e5c  antic.\n\n---\n\
-00000c70: 6e23 2320 5265 7175 6972 656d 656e 745c  n## Requirement\
-00000c80: 6e5c 6e2a 2a4d 6f6e 676f 4442 2d4f 444d  n\n**MongoDB-ODM
-00000c90: 2a2a 2077 696c 6c20 776f 726b 206f 6e20  ** will work on 
-00000ca0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000cb0: 2f77 7777 2e70 7974 686f 6e2e 6f72 672f  /www.python.org/
-00000cc0: 646f 776e 6c6f 6164 732f 2220 636c 6173  downloads/" clas
-00000cd0: 733d 2265 7874 6572 6e61 6c2d 6c69 6e6b  s="external-link
-00000ce0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
-00000cf0: 223e 5079 7468 6f6e 2033 2e38 2061 6e64  ">Python 3.8 and
-00000d00: 2061 626f 7665 3c2f 613e 5c6e 5c6e 5468   above</a>\n\nTh
-00000d10: 6973 202a 2a4d 6f6e 676f 4442 2d4f 444d  is **MongoDB-ODM
-00000d20: 2a2a 2069 7320 6275 696c 7420 6f6e 2074  ** is built on t
-00000d30: 6f70 206f 6620 2a2a 5079 4d6f 6e67 6f2a  op of **PyMongo*
-00000d40: 2a20 616e 6420 2a2a 5079 6461 6e74 6963  * and **Pydantic
-00000d50: 2a2a 2e20 5468 6f73 6520 7061 636b 6167  **. Those packag
-00000d60: 6573 2061 7265 2072 6571 7569 7265 6420  es are required 
-00000d70: 616e 6420 7769 6c6c 2061 7574 6f2d 696e  and will auto-in
-00000d80: 7374 616c 6c20 7768 696c 6520 2a2a 4d6f  stall while **Mo
-00000d90: 6e67 6f44 422d 4f44 4d2a 2a20 7761 7320  ngoDB-ODM** was 
-00000da0: 696e 7374 616c 6c65 642e 5c6e 5c6e 2323  installed.\n\n##
-00000db0: 2049 6e73 7461 6c6c 6174 696f 6e5c 6e5c   Installation\n\
-00000dc0: 6e60 6060 636f 6e73 6f6c 655c 6e24 2070  n```console\n$ p
-00000dd0: 6970 2069 6e73 7461 6c6c 206d 6f6e 676f  ip install mongo
-00000de0: 6462 2d6f 646d 5c6e 6060 605c 6e5c 6e23  db-odm\n```\n\n#
-00000df0: 2320 4578 616d 706c 655c 6e5c 6e23 2323  # Example\n\n###
-00000e00: 2044 6566 696e 6520 6d6f 6465 6c5c 6e5c   Define model\n\
-00000e10: 6e60 6060 5079 7468 6f6e 5c6e 696d 706f  n```Python\nimpo
-00000e20: 7274 206f 735c 6e66 726f 6d20 7479 7069  rt os\nfrom typi
-00000e30: 6e67 2069 6d70 6f72 7420 4f70 7469 6f6e  ng import Option
-00000e40: 616c 5c6e 5c6e 6672 6f6d 206d 6f6e 676f  al\n\nfrom mongo
-00000e50: 6462 5f6f 646d 2069 6d70 6f72 7420 4153  db_odm import AS
-00000e60: 4345 4e44 494e 472c 2044 6f63 756d 656e  CENDING, Documen
-00000e70: 742c 2049 6e64 6578 4d6f 6465 6c2c 2063  t, IndexModel, c
-00000e80: 6f6e 6e65 6374 5c6e 5c6e 5c6e 636c 6173  onnect\n\n\nclas
-00000e90: 7320 506c 6179 6572 2844 6f63 756d 656e  s Player(Documen
-00000ea0: 7429 3a5c 6e20 2020 206e 616d 653a 2073  t):\n    name: s
-00000eb0: 7472 5c6e 2020 2020 636f 756e 7472 795f  tr\n    country_
-00000ec0: 636f 6465 3a20 7374 725c 6e20 2020 2072  code: str\n    r
-00000ed0: 6174 696e 673a 204f 7074 696f 6e61 6c5b  ating: Optional[
-00000ee0: 696e 745d 203d 204e 6f6e 655c 6e5c 6e20  int] = None\n\n 
-00000ef0: 2020 2063 6c61 7373 2043 6f6e 6669 6728     class Config(
-00000f00: 446f 6375 6d65 6e74 2e43 6f6e 6669 6729  Document.Config)
-00000f10: 3a5c 6e20 2020 2020 2020 2069 6e64 6578  :\n        index
-00000f20: 6573 203d 205b 5c6e 2020 2020 2020 2020  es = [\n        
-00000f30: 2020 2020 496e 6465 784d 6f64 656c 285b      IndexModel([
-00000f40: 2822 7261 7469 6e67 222c 2041 5343 454e  ("rating", ASCEN
-00000f50: 4449 4e47 295d 292c 5c6e 2020 2020 2020  DING)]),\n      
-00000f60: 2020 5d5c 6e60 6060 5c6e 5c6e 2323 2320    ]\n```\n\n### 
-00000f70: 5365 7420 436f 6e6e 6563 7469 6f6e 5c6e  Set Connection\n
-00000f80: 5c6e 6060 6050 7974 686f 6e5c 6e63 6f6e  \n```Python\ncon
-00000f90: 6e65 6374 286f 732e 656e 7669 726f 6e2e  nect(os.environ.
-00000fa0: 6765 7428 224d 4f4e 474f 5f55 524c 222c  get("MONGO_URL",
-00000fb0: 2022 6d6f 6e67 6f64 623a 2f2f 6c6f 6361   "mongodb://loca
-00000fc0: 6c68 6f73 743a 3237 3031 372f 7465 7374  lhost:27017/test
-00000fd0: 6462 2229 295c 6e60 6060 5c6e 5c6e 2323  db"))\n```\n\n##
-00000fe0: 2320 4372 6561 7465 2044 6f63 756d 656e  # Create Documen
-00000ff0: 745c 6e5c 6e60 6060 5079 7468 6f6e 5c6e  t\n\n```Python\n
-00001000: 7065 6c65 203d 2050 6c61 7965 7228 6e61  pele = Player(na
-00001010: 6d65 3d22 5065 6cc3 a922 2c20 636f 756e  me="Pel..", coun
-00001020: 7472 795f 636f 6465 3d22 4252 4122 292e  try_code="BRA").
-00001030: 6372 6561 7465 2829 5c6e 6d61 7261 646f  create()\nmarado
-00001040: 6e61 203d 2050 6c61 7965 7228 6e61 6d65  na = Player(name
-00001050: 3d22 4469 6567 6f20 4d61 7261 646f 6e61  ="Diego Maradona
-00001060: 222c 2063 6f75 6e74 7279 5f63 6f64 653d  ", country_code=
-00001070: 2241 5247 222c 2072 6174 696e 673d 3937  "ARG", rating=97
-00001080: 292e 6372 6561 7465 2829 5c6e 7a69 6461  ).create()\nzida
-00001090: 6e65 203d 2050 6c61 7965 7228 6e61 6d65  ne = Player(name
-000010a0: 3d22 5a69 6e65 6469 6e65 205a 6964 616e  ="Zinedine Zidan
-000010b0: 6522 2c20 636f 756e 7472 795f 636f 6465  e", country_code
-000010c0: 3d22 4652 4122 2c20 7261 7469 6e67 3d39  ="FRA", rating=9
-000010d0: 3629 2e63 7265 6174 6528 295c 6e60 6060  6).create()\n```
-000010e0: 5c6e 5c6e 2323 2320 5265 7472 6965 7665  \n\n### Retrieve
-000010f0: 2044 6f63 756d 656e 745c 6e5c 6e23 2323   Document\n\n###
-00001100: 2320 4669 6e64 2064 6174 6120 6672 6f6d  # Find data from
-00001110: 2063 6f6c 6c65 6374 696f 6e5c 6e5c 6e60   collection\n\n`
-00001120: 6060 5079 7468 6f6e 5c6e 666f 7220 706c  ``Python\nfor pl
-00001130: 6179 6572 2069 6e20 506c 6179 6572 2e66  ayer in Player.f
-00001140: 696e 6428 293a 5c6e 2020 2020 7072 696e  ind():\n    prin
-00001150: 7428 706c 6179 6572 295c 6e60 6060 5c6e  t(player)\n```\n
-00001160: 5c6e 2323 2323 2046 696e 6420 6f6e 6520  \n#### Find one 
-00001170: 6f62 6a65 6374 2077 6974 6820 6669 6c74  object with filt
-00001180: 6572 5c6e 5c6e 6060 6050 7974 686f 6e5c  er\n\n```Python\
-00001190: 6e70 6c61 7965 7220 3d20 506c 6179 6572  nplayer = Player
-000011a0: 2e66 696e 645f 6f6e 6528 7b22 6e61 6d65  .find_one({"name
-000011b0: 223a 2022 5065 6cc3 a922 7d29 5c6e 6060  ": "Pel.."})\n``
-000011c0: 605c 6e5c 6e23 2323 2055 7064 6174 6520  `\n\n### Update 
-000011d0: 4461 7461 5c6e 5c6e 6060 6050 7974 686f  Data\n\n```Pytho
-000011e0: 6e5c 6e70 6c61 7965 7220 3d20 506c 6179  n\nplayer = Play
-000011f0: 6572 2e66 696e 645f 6f6e 6528 7b22 6e61  er.find_one({"na
-00001200: 6d65 223a 2022 5065 6cc3 a922 7d29 5c6e  me": "Pel.."})\n
-00001210: 6966 2070 6c61 7965 723a 5c6e 2020 2020  if player:\n    
-00001220: 706c 6179 6572 2e72 6174 696e 6720 3d20  player.rating = 
-00001230: 3938 2020 2320 706f 7465 6e74 6961 6c5c  98  # potential\
-00001240: 6e20 2020 2070 6c61 7965 722e 7570 6461  n    player.upda
-00001250: 7465 2829 5c6e 6060 605c 6e5c 6e23 2323  te()\n```\n\n###
-00001260: 2044 656c 6574 6520 4461 7461 5c6e 5c6e   Delete Data\n\n
-00001270: 6060 6050 7974 686f 6e5c 6e70 6c61 7965  ```Python\nplaye
-00001280: 7220 3d20 506c 6179 6572 2e66 696e 645f  r = Player.find_
-00001290: 6f6e 6528 7b22 6e61 6d65 223a 2022 5065  one({"name": "Pe
-000012a0: 6cc3 a922 7d29 5c6e 6966 2070 6c61 7965  l.."})\nif playe
-000012b0: 723a 5c6e 2020 2020 706c 6179 6572 2e64  r:\n    player.d
-000012c0: 656c 6574 6528 295c 6e60 6060 5c6e 5c6e  elete()\n```\n\n
-000012d0: 2323 2320 4170 706c 7920 496e 6465 7865  ### Apply Indexe
-000012e0: 735c 6e5c 6e60 6060 5079 7468 6f6e 5c6e  s\n\n```Python\n
-000012f0: 696d 706f 7274 206f 735c 6e66 726f 6d20  import os\nfrom 
-00001300: 7479 7069 6e67 2069 6d70 6f72 7420 4f70  typing import Op
-00001310: 7469 6f6e 616c 5c6e 5c6e 6672 6f6d 206d  tional\n\nfrom m
-00001320: 6f6e 676f 6462 5f6f 646d 2069 6d70 6f72  ongodb_odm impor
-00001330: 7420 4153 4345 4e44 494e 472c 2044 6f63  t ASCENDING, Doc
-00001340: 756d 656e 742c 2049 6e64 6578 4d6f 6465  ument, IndexMode
-00001350: 6c2c 2063 6f6e 6e65 6374 5c6e 5c6e 5c6e  l, connect\n\n\n
-00001360: 636c 6173 7320 506c 6179 6572 2844 6f63  class Player(Doc
-00001370: 756d 656e 7429 3a5c 6e20 2020 206e 616d  ument):\n    nam
-00001380: 653a 2073 7472 5c6e 2020 2020 636f 756e  e: str\n    coun
-00001390: 7472 795f 636f 6465 3a20 7374 725c 6e20  try_code: str\n 
-000013a0: 2020 2072 6174 696e 673a 204f 7074 696f     rating: Optio
-000013b0: 6e61 6c5b 696e 745d 203d 204e 6f6e 655c  nal[int] = None\
-000013c0: 6e5c 6e20 2020 2063 6c61 7373 2043 6f6e  n\n    class Con
-000013d0: 6669 6728 446f 6375 6d65 6e74 2e43 6f6e  fig(Document.Con
-000013e0: 6669 6729 3a5c 6e20 2020 2020 2020 2069  fig):\n        i
-000013f0: 6e64 6578 6573 203d 205b 5c6e 2020 2020  ndexes = [\n    
-00001400: 2020 2020 2020 2020 496e 6465 784d 6f64          IndexMod
-00001410: 656c 285b 2822 7261 7469 6e67 222c 2041  el([("rating", A
-00001420: 5343 454e 4449 4e47 295d 292c 5c6e 2020  SCENDING)]),\n  
-00001430: 2020 2020 2020 5d5c 6e60 6060 5c6e 5c6e        ]\n```\n\n
-00001440: 2d20 546f 2063 7265 6174 6520 696e 6465  - To create inde
-00001450: 7865 7320 696e 2074 6865 2064 6174 6162  xes in the datab
-00001460: 6173 6520 6465 636c 6172 6520 5b49 6e64  ase declare [Ind
-00001470: 6578 4d6f 6465 6c5d 2868 7474 7073 3a2f  exModel](https:/
-00001480: 2f70 796d 6f6e 676f 2e72 6561 6474 6865  /pymongo.readthe
-00001490: 646f 6373 2e69 6f2f 656e 2f73 7461 626c  docs.io/en/stabl
-000014a0: 652f 7475 746f 7269 616c 2e68 746d 6c23  e/tutorial.html#
-000014b0: 696e 6465 7869 6e67 2920 616e 6420 6173  indexing) and as
-000014c0: 7369 676e 2069 6e20 696e 6465 7865 7320  sign in indexes 
-000014d0: 6172 7261 7920 696e 2043 6f6e 6669 6720  array in Config 
-000014e0: 636c 6173 732e 202a 2a49 6e64 6578 4d6f  class. **IndexMo
-000014f0: 6465 6c2a 2a20 6d6f 6475 6c65 7320 7468  del** modules th
-00001500: 6174 2061 7265 2064 6972 6563 746c 7920  at are directly 
-00001510: 696d 706f 7274 6564 2066 726f 6d20 2a2a  imported from **
-00001520: 7079 6d6f 6e67 6f2a 2a2e 5c6e 2d20 496d  pymongo**.\n- Im
-00001530: 706f 7274 2074 6865 2060 6170 706c 795f  port the `apply_
-00001540: 696e 6465 7865 7360 2066 726f 6d20 606d  indexes` from `m
-00001550: 6f6e 676f 6462 5f6f 646d 602e 2043 616c  ongodb_odm`. Cal
-00001560: 6c20 7468 6520 6061 7070 6c79 5f69 6e64  l the `apply_ind
-00001570: 6578 6573 6020 6675 6e63 7469 6f6e 2066  exes` function f
-00001580: 726f 6d20 796f 7572 2043 4c49 2e20 596f  rom your CLI. Yo
-00001590: 7520 6361 6e20 7573 6520 3c61 2068 7265  u can use <a hre
-000015a0: 663d 2268 7474 7073 3a2f 2f74 7970 6572  f="https://typer
-000015b0: 2e74 6961 6e67 6f6c 6f2e 636f 6d22 2063  .tiangolo.com" c
-000015c0: 6c61 7373 3d22 6578 7465 726e 616c 2d6c  lass="external-l
-000015d0: 696e 6b22 2074 6172 6765 743d 225f 626c  ink" target="_bl
-000015e0: 616e 6b22 3e54 7970 6572 3c2f 613e 2074  ank">Typer</a> t
-000015f0: 6f20 696d 706c 656d 656e 7420 434c 492e  o implement CLI.
-00001600: 5c6e 5c6e 2323 2045 7861 6d70 6c65 2043  \n\n## Example C
-00001610: 6f64 655c 6e5c 6e54 6869 7320 6973 2074  ode\n\nThis is t
-00001620: 6865 2065 7861 6d70 6c65 206f 6620 6675  he example of fu
-00001630: 6c6c 2063 6f64 6520 6f66 2061 626f 7665  ll code of above
-00001640: 2e5c 6e5c 6e60 6060 7079 7468 6f6e 5c6e  .\n\n```python\n
-00001650: 696d 706f 7274 206f 735c 6e66 726f 6d20  import os\nfrom 
-00001660: 7479 7069 6e67 2069 6d70 6f72 7420 4f70  typing import Op
-00001670: 7469 6f6e 616c 5c6e 5c6e 6672 6f6d 206d  tional\n\nfrom m
-00001680: 6f6e 676f 6462 5f6f 646d 2069 6d70 6f72  ongodb_odm impor
-00001690: 7420 4153 4345 4e44 494e 472c 2044 6f63  t ASCENDING, Doc
-000016a0: 756d 656e 742c 2049 6e64 6578 4d6f 6465  ument, IndexMode
-000016b0: 6c2c 2063 6f6e 6e65 6374 5c6e 5c6e 5c6e  l, connect\n\n\n
-000016c0: 636c 6173 7320 506c 6179 6572 2844 6f63  class Player(Doc
-000016d0: 756d 656e 7429 3a5c 6e20 2020 206e 616d  ument):\n    nam
-000016e0: 653a 2073 7472 5c6e 2020 2020 636f 756e  e: str\n    coun
-000016f0: 7472 795f 636f 6465 3a20 7374 725c 6e20  try_code: str\n 
-00001700: 2020 2072 6174 696e 673a 204f 7074 696f     rating: Optio
-00001710: 6e61 6c5b 696e 745d 203d 204e 6f6e 655c  nal[int] = None\
-00001720: 6e5c 6e20 2020 2063 6c61 7373 2043 6f6e  n\n    class Con
-00001730: 6669 6728 446f 6375 6d65 6e74 2e43 6f6e  fig(Document.Con
-00001740: 6669 6729 3a5c 6e20 2020 2020 2020 2069  fig):\n        i
-00001750: 6e64 6578 6573 203d 205b 5c6e 2020 2020  ndexes = [\n    
-00001760: 2020 2020 2020 2020 496e 6465 784d 6f64          IndexMod
-00001770: 656c 285b 2822 7261 7469 6e67 222c 2041  el([("rating", A
-00001780: 5343 454e 4449 4e47 295d 292c 5c6e 2020  SCENDING)]),\n  
-00001790: 2020 2020 2020 5d5c 6e5c 6e5c 6e63 6f6e        ]\n\n\ncon
-000017a0: 6e65 6374 286f 732e 656e 7669 726f 6e2e  nect(os.environ.
-000017b0: 6765 7428 224d 4f4e 474f 5f55 524c 222c  get("MONGO_URL",
-000017c0: 2022 6d6f 6e67 6f64 623a 2f2f 6c6f 6361   "mongodb://loca
-000017d0: 6c68 6f73 743a 3237 3031 372f 7465 7374  lhost:27017/test
-000017e0: 6462 2229 295c 6e5c 6e70 656c 6520 3d20  db"))\n\npele = 
-000017f0: 506c 6179 6572 286e 616d 653d 2250 656c  Player(name="Pel
-00001800: c3a9 222c 2063 6f75 6e74 7279 5f63 6f64  ..", country_cod
-00001810: 653d 2242 5241 2229 2e63 7265 6174 6528  e="BRA").create(
-00001820: 295c 6e6d 6172 6164 6f6e 6120 3d20 506c  )\nmaradona = Pl
-00001830: 6179 6572 286e 616d 653d 2244 6965 676f  ayer(name="Diego
-00001840: 204d 6172 6164 6f6e 6122 2c20 636f 756e   Maradona", coun
-00001850: 7472 795f 636f 6465 3d22 4152 4722 2c20  try_code="ARG", 
-00001860: 7261 7469 6e67 3d39 3729 2e63 7265 6174  rating=97).creat
-00001870: 6528 295c 6e7a 6964 616e 6520 3d20 506c  e()\nzidane = Pl
-00001880: 6179 6572 286e 616d 653d 225a 696e 6564  ayer(name="Zined
-00001890: 696e 6520 5a69 6461 6e65 222c 2063 6f75  ine Zidane", cou
-000018a0: 6e74 7279 5f63 6f64 653d 2246 5241 222c  ntry_code="FRA",
-000018b0: 2072 6174 696e 673d 3936 292e 6372 6561   rating=96).crea
-000018c0: 7465 2829 5c6e 5c6e 666f 7220 706c 6179  te()\n\nfor play
-000018d0: 6572 2069 6e20 506c 6179 6572 2e66 696e  er in Player.fin
-000018e0: 6428 293a 5c6e 2020 2020 7072 696e 7428  d():\n    print(
-000018f0: 706c 6179 6572 295c 6e5c 6e70 6c61 7965  player)\n\nplaye
-00001900: 7220 3d20 506c 6179 6572 2e66 696e 645f  r = Player.find_
-00001910: 6f6e 6528 7b22 6e61 6d65 223a 2022 5065  one({"name": "Pe
-00001920: 6cc3 a922 7d29 5c6e 6966 2070 6c61 7965  l.."})\nif playe
-00001930: 723a 5c6e 2020 2020 706c 6179 6572 2e72  r:\n    player.r
-00001940: 6174 696e 6720 3d20 3938 2020 2320 706f  ating = 98  # po
-00001950: 7465 6e74 6961 6c5c 6e20 2020 2070 6c61  tential\n    pla
-00001960: 7965 722e 7570 6461 7465 2829 5c6e 5c6e  yer.update()\n\n
-00001970: 706c 6179 6572 203d 2050 6c61 7965 722e  player = Player.
-00001980: 6669 6e64 5f6f 6e65 287b 226e 616d 6522  find_one({"name"
-00001990: 3a20 2250 656c c3a9 227d 295c 6e69 6620  : "Pel.."})\nif 
-000019a0: 706c 6179 6572 3a5c 6e20 2020 2070 6c61  player:\n    pla
-000019b0: 7965 722e 6465 6c65 7465 2829 5c6e 6060  yer.delete()\n``
-000019c0: 605c 6e5c 6e23 2323 2053 7570 706f 7274  `\n\n### Support
-000019d0: 6564 2046 7261 6d65 776f 726b 5c6e 5c6e  ed Framework\n\n
-000019e0: 2a2a 4d6f 6e67 6f44 422d 4f44 4d2a 2a20  **MongoDB-ODM** 
-000019f0: 6973 206e 6f74 2066 7261 6d65 776f 726b  is not framework
-00001a00: 2064 6570 656e 6465 6e74 2e20 5765 2063   dependent. We c
-00001a10: 616e 2075 7365 2074 6869 7320 7061 636b  an use this pack
-00001a20: 6167 6520 696e 2061 6e79 2073 7973 7465  age in any syste
-00001a30: 6d2e 2042 7574 2077 6520 7461 6b65 2073  m. But we take s
-00001a40: 7065 6369 616c 2063 6f6e 7369 6465 7261  pecial considera
-00001a50: 7469 6f6e 2062 6569 6e67 2063 6f6d 7061  tion being compa
-00001a60: 7469 626c 6520 7769 7468 203c 6120 6872  tible with <a hr
-00001a70: 6566 3d22 6874 7470 733a 2f2f 6661 7374  ef="https://fast
-00001a80: 6170 692e 7469 616e 676f 6c6f 2e63 6f6d  api.tiangolo.com
-00001a90: 2f22 2063 6c61 7373 3d22 6578 7465 726e  /" class="extern
-00001aa0: 616c 2d6c 696e 6b22 2074 6172 6765 743d  al-link" target=
-00001ab0: 225f 626c 616e 6b22 3e46 6173 7441 5049  "_blank">FastAPI
-00001ac0: 3c2f 613e 2061 6e64 203c 6120 6872 6566  </a> and <a href
-00001ad0: 3d22 6874 7470 733a 2f2f 666c 6173 6b2e  ="https://flask.
-00001ae0: 7061 6c6c 6574 7370 726f 6a65 6374 732e  palletsprojects.
-00001af0: 636f 6d2f 656e 2f32 2e32 2e78 2f22 2063  com/en/2.2.x/" c
-00001b00: 6c61 7373 3d22 6578 7465 726e 616c 2d6c  lass="external-l
-00001b10: 696e 6b22 2074 6172 6765 743d 225f 626c  ink" target="_bl
-00001b20: 616e 6b22 3e46 6c61 736b 3c2f 613e 2e5c  ank">Flask</a>.\
-00001b30: 6e5c 6e23 2323 2043 7265 6469 745c 6e5c  n\n### Credit\n\
-00001b40: 6e54 6869 7320 7061 636b 6167 6520 6973  nThis package is
-00001b50: 2062 7569 6c74 206f 6e20 746f 7020 6f66   built on top of
-00001b60: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00001b70: 2f2f 7079 6d6f 6e67 6f2e 7265 6164 7468  //pymongo.readth
-00001b80: 6564 6f63 732e 696f 2f65 6e2f 7374 6162  edocs.io/en/stab
-00001b90: 6c65 2220 636c 6173 733d 2265 7874 6572  le" class="exter
-00001ba0: 6e61 6c2d 6c69 6e6b 2220 7461 7267 6574  nal-link" target
-00001bb0: 3d22 5f62 6c61 6e6b 223e 5079 4d6f 6e67  ="_blank">PyMong
-00001bc0: 6f3c 2f61 3e20 616e 6420 3c61 2068 7265  o</a> and <a hre
-00001bd0: 663d 2268 7474 7073 3a2f 2f64 6f63 732e  f="https://docs.
-00001be0: 7079 6461 6e74 6963 2e64 6576 2220 636c  pydantic.dev" cl
-00001bf0: 6173 733d 2265 7874 6572 6e61 6c2d 6c69  ass="external-li
-00001c00: 6e6b 2220 7461 7267 6574 3d22 5f62 6c61  nk" target="_bla
-00001c10: 6e6b 223e 5079 6461 6e74 6963 3c2f 613e  nk">Pydantic</a>
-00001c20: 2e5c 6e5c 6e44 6f63 756d 656e 7461 7469  .\n\nDocumentati
-00001c30: 6f6e 2067 656e 6572 6174 6564 2062 7920  on generated by 
-00001c40: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00001c50: 2f77 7777 2e6d 6b64 6f63 732e 6f72 672f  /www.mkdocs.org/
-00001c60: 2220 636c 6173 733d 2265 7874 6572 6e61  " class="externa
-00001c70: 6c2d 6c69 6e6b 2220 7461 7267 6574 3d22  l-link" target="
-00001c80: 5f62 6c61 6e6b 223e 4d6b 446f 6373 3c2f  _blank">MkDocs</
-00001c90: 613e 2061 6e64 203c 6120 6872 6566 3d22  a> and <a href="
-00001ca0: 6874 7470 733a 2f2f 7371 7569 6466 756e  https://squidfun
-00001cb0: 6b2e 6769 7468 7562 2e69 6f2f 6d6b 646f  k.github.io/mkdo
-00001cc0: 6373 2d6d 6174 6572 6961 6c2f 2220 636c  cs-material/" cl
-00001cd0: 6173 733d 2265 7874 6572 6e61 6c2d 6c69  ass="external-li
-00001ce0: 6e6b 2220 7461 7267 6574 3d22 5f62 6c61  nk" target="_bla
-00001cf0: 6e6b 223e 4d61 7465 7269 616c 2066 6f72  nk">Material for
-00001d00: 204d 6b44 6f63 733c 2f61 3e2e 5c6e 5c6e   MkDocs</a>.\n\n
-00001d10: 446f 6375 6d65 6e74 6174 696f 6e20 696e  Documentation in
-00001d20: 7370 6972 6564 2062 7920 3c61 2068 7265  spired by <a hre
-00001d30: 663d 2268 7474 7073 3a2f 2f73 716c 6d6f  f="https://sqlmo
-00001d40: 6465 6c2e 7469 616e 676f 6c6f 2e63 6f6d  del.tiangolo.com
-00001d50: 2220 636c 6173 733d 2265 7874 6572 6e61  " class="externa
-00001d60: 6c2d 6c69 6e6b 2220 7461 7267 6574 3d22  l-link" target="
-00001d70: 5f62 6c61 6e6b 223e 5351 4c4d 6f64 656c  _blank">SQLModel
-00001d80: 3c2f 613e 2e5c 6e5c 6e42 7574 2077 6520  </a>.\n\nBut we 
-00001d90: 7573 6520 6f74 6865 7220 7061 636b 6167  use other packag
-00001da0: 6573 2066 6f72 2064 6576 656c 6f70 6d65  es for developme
-00001db0: 6e74 2061 6e64 206f 7468 6572 2070 7572  nt and other pur
-00001dc0: 706f 7365 732e 2043 6865 636b 202a 2a70  poses. Check **p
-00001dd0: 7970 726f 6a65 6374 2e74 6f6d 6c2a 2a20  yproject.toml** 
-00001de0: 746f 206b 6e6f 7720 6162 6f75 7420 616c  to know about al
-00001df0: 6c20 7061 636b 6167 6573 2077 6520 7573  l packages we us
-00001e00: 6520 746f 2062 7569 6c64 2074 6869 7320  e to build this 
-00001e10: 7061 636b 6167 652e 5c6e 5c6e 2323 204c  package.\n\n## L
-00001e20: 6963 656e 7365 5c6e 5c6e 5468 6973 2070  icense\n\nThis p
-00001e30: 726f 6a65 6374 2069 7320 6c69 6365 6e73  roject is licens
-00001e40: 6564 2075 6e64 6572 2074 6865 2074 6572  ed under the ter
-00001e50: 6d73 206f 6620 7468 6520 5b4d 4954 206c  ms of the [MIT l
-00001e60: 6963 656e 7365 5d28 6874 7470 733a 2f2f  icense](https://
-00001e70: 6769 7468 7562 2e63 6f6d 2f6e 6179 616e  github.com/nayan
-00001e80: 3332 6269 7377 6173 2f6d 6f6e 676f 6462  32biswas/mongodb
-00001e90: 2d6f 646d 2f62 6c6f 622f 6d61 696e 2f4c  -odm/blob/main/L
-00001ea0: 4943 454e 5345 292e 5c6e 272c 0a20 2020  ICENSE).\n',.   
-00001eb0: 2027 6175 7468 6f72 273a 2027 4e61 7961   'author': 'Naya
-00001ec0: 6e20 4269 7377 6173 272c 0a20 2020 2027  n Biswas',.    '
-00001ed0: 6175 7468 6f72 5f65 6d61 696c 273a 2027  author_email': '
-00001ee0: 6e61 7961 6e33 3262 6973 7761 7340 676d  nayan32biswas@gm
-00001ef0: 6169 6c2e 636f 6d27 2c0a 2020 2020 276d  ail.com',.    'm
-00001f00: 6169 6e74 6169 6e65 7227 3a20 274e 6f6e  aintainer': 'Non
-00001f10: 6527 2c0a 2020 2020 276d 6169 6e74 6169  e',.    'maintai
-00001f20: 6e65 725f 656d 6169 6c27 3a20 274e 6f6e  ner_email': 'Non
-00001f30: 6527 2c0a 2020 2020 2775 726c 273a 2027  e',.    'url': '
-00001f40: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001f50: 6f6d 2f6e 6179 616e 3332 6269 7377 6173  om/nayan32biswas
-00001f60: 2f6d 6f6e 676f 6462 2d6f 646d 272c 0a20  /mongodb-odm',. 
-00001f70: 2020 2027 7061 636b 6167 6573 273a 2070     'packages': p
-00001f80: 6163 6b61 6765 732c 0a20 2020 2027 7061  ackages,.    'pa
-00001f90: 636b 6167 655f 6461 7461 273a 2070 6163  ckage_data': pac
-00001fa0: 6b61 6765 5f64 6174 612c 0a20 2020 2027  kage_data,.    '
-00001fb0: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-00001fc0: 273a 2069 6e73 7461 6c6c 5f72 6571 7569  ': install_requi
-00001fd0: 7265 732c 0a20 2020 2027 7079 7468 6f6e  res,.    'python
-00001fe0: 5f72 6571 7569 7265 7327 3a20 273e 3d33  _requires': '>=3
-00001ff0: 2e38 2c3c 342e 3027 2c0a 7d0a 0a0a 7365  .8,<4.0',.}...se
-00002000: 7475 7028 2a2a 7365 7475 705f 6b77 6172  tup(**setup_kwar
-00002010: 6773 290a                                gs).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6d6f 6e67  : 2.1.Name: mong
+00000020: 6f64 622d 6f64 6d0a 5665 7273 696f 6e3a  odb-odm.Version:
+00000030: 2030 2e32 2e33 0a53 756d 6d61 7279 3a20   0.2.3.Summary: 
+00000040: 4d6f 6e67 6f44 422d 4f44 4d2c 204e 4f53  MongoDB-ODM, NOS
+00000050: 514c 2064 6174 6162 6173 6573 2069 6e20  QL databases in 
+00000060: 5079 7468 6f6e 2c20 6465 7369 676e 6564  Python, designed
+00000070: 2066 6f72 2073 696d 706c 6963 6974 792c   for simplicity,
+00000080: 2063 6f6d 7061 7469 6269 6c69 7479 2c20   compatibility, 
+00000090: 616e 6420 726f 6275 7374 6e65 7373 2e0a  and robustness..
+000000a0: 486f 6d65 2d70 6167 653a 2068 7474 7073  Home-page: https
+000000b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6e61  ://github.com/na
+000000c0: 7961 6e33 3262 6973 7761 732f 6d6f 6e67  yan32biswas/mong
+000000d0: 6f64 622d 6f64 6d0a 4c69 6365 6e73 653a  odb-odm.License:
+000000e0: 204d 4954 0a41 7574 686f 723a 204e 6179   MIT.Author: Nay
+000000f0: 616e 2042 6973 7761 730a 4175 7468 6f72  an Biswas.Author
+00000100: 2d65 6d61 696c 3a20 6e61 7961 6e33 3262  -email: nayan32b
+00000110: 6973 7761 7340 676d 6169 6c2e 636f 6d0a  iswas@gmail.com.
+00000120: 5265 7175 6972 6573 2d50 7974 686f 6e3a  Requires-Python:
+00000130: 203e 3d33 2e38 2c3c 342e 300a 436c 6173   >=3.8,<4.0.Clas
+00000140: 7369 6669 6572 3a20 4465 7665 6c6f 706d  sifier: Developm
+00000150: 656e 7420 5374 6174 7573 203a 3a20 3420  ent Status :: 4 
+00000160: 2d20 4265 7461 0a43 6c61 7373 6966 6965  - Beta.Classifie
+00000170: 723a 2046 7261 6d65 776f 726b 203a 3a20  r: Framework :: 
+00000180: 4173 796e 6349 4f0a 436c 6173 7369 6669  AsyncIO.Classifi
+00000190: 6572 3a20 496e 7465 6e64 6564 2041 7564  er: Intended Aud
+000001a0: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
+000001b0: 6572 730a 436c 6173 7369 6669 6572 3a20  ers.Classifier: 
+000001c0: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
+000001d0: 6520 3a3a 2053 6369 656e 6365 2f52 6573  e :: Science/Res
+000001e0: 6561 7263 680a 436c 6173 7369 6669 6572  earch.Classifier
+000001f0: 3a20 496e 7465 6e64 6564 2041 7564 6965  : Intended Audie
+00000200: 6e63 6520 3a3a 2053 7973 7465 6d20 4164  nce :: System Ad
+00000210: 6d69 6e69 7374 7261 746f 7273 0a43 6c61  ministrators.Cla
+00000220: 7373 6966 6965 723a 204c 6963 656e 7365  ssifier: License
+00000230: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+00000240: 203a 3a20 4d49 5420 4c69 6365 6e73 650a   :: MIT License.
+00000250: 436c 6173 7369 6669 6572 3a20 4f70 6572  Classifier: Oper
+00000260: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+00000270: 4f53 2049 6e64 6570 656e 6465 6e74 0a43  OS Independent.C
+00000280: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000290: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000002a0: 3a3a 2050 7974 686f 6e20 3a3a 2033 0a43  :: Python :: 3.C
+000002b0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+000002c0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000002d0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
+000002e0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+000002f0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000300: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000310: 2e39 0a43 6c61 7373 6966 6965 723a 2050  .9.Classifier: P
+00000320: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000330: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000340: 2033 2e31 300a 436c 6173 7369 6669 6572   3.10.Classifier
+00000350: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000360: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000370: 203a 3a20 332e 3131 0a43 6c61 7373 6966   :: 3.11.Classif
+00000380: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000390: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000003a0: 686f 6e20 3a3a 2033 203a 3a20 4f6e 6c79  hon :: 3 :: Only
+000003b0: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
+000003c0: 6963 203a 3a20 4461 7461 6261 7365 0a43  ic :: Database.C
+000003d0: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
+000003e0: 203a 3a20 4461 7461 6261 7365 203a 3a20   :: Database :: 
+000003f0: 4461 7461 6261 7365 2045 6e67 696e 6573  Database Engines
+00000400: 2f53 6572 7665 7273 0a43 6c61 7373 6966  /Servers.Classif
+00000410: 6965 723a 2054 6f70 6963 203a 3a20 496e  ier: Topic :: In
+00000420: 7465 726e 6574 0a43 6c61 7373 6966 6965  ternet.Classifie
+00000430: 723a 2054 6f70 6963 203a 3a20 496e 7465  r: Topic :: Inte
+00000440: 726e 6574 203a 3a20 5757 572f 4854 5450  rnet :: WWW/HTTP
+00000450: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
+00000460: 6963 203a 3a20 496e 7465 726e 6574 203a  ic :: Internet :
+00000470: 3a20 5757 572f 4854 5450 203a 3a20 4854  : WWW/HTTP :: HT
+00000480: 5450 2053 6572 7665 7273 0a43 6c61 7373  TP Servers.Class
+00000490: 6966 6965 723a 2054 7970 696e 6720 3a3a  ifier: Typing ::
+000004a0: 2054 7970 6564 0a52 6571 7569 7265 732d   Typed.Requires-
+000004b0: 4469 7374 3a20 7079 6461 6e74 6963 2028  Dist: pydantic (
+000004c0: 3e3d 312e 3130 2e37 2c3c 322e 302e 3029  >=1.10.7,<2.0.0)
+000004d0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+000004e0: 7079 6d6f 6e67 6f5b 7372 765d 2028 3e3d  pymongo[srv] (>=
+000004f0: 342e 332e 332c 3c35 2e30 2e30 290a 5072  4.3.3,<5.0.0).Pr
+00000500: 6f6a 6563 742d 5552 4c3a 2044 6f63 756d  oject-URL: Docum
+00000510: 656e 7461 7469 6f6e 2c20 6874 7470 733a  entation, https:
+00000520: 2f2f 6d6f 6e67 6f64 622d 6f64 6d2e 7265  //mongodb-odm.re
+00000530: 6164 7468 6564 6f63 732e 696f 0a50 726f  adthedocs.io.Pro
+00000540: 6a65 6374 2d55 524c 3a20 5265 706f 7369  ject-URL: Reposi
+00000550: 746f 7279 2c20 6874 7470 733a 2f2f 6769  tory, https://gi
+00000560: 7468 7562 2e63 6f6d 2f6e 6179 616e 3332  thub.com/nayan32
+00000570: 6269 7377 6173 2f6d 6f6e 676f 6462 2d6f  biswas/mongodb-o
+00000580: 646d 0a44 6573 6372 6970 7469 6f6e 2d43  dm.Description-C
+00000590: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
+000005a0: 742f 6d61 726b 646f 776e 0a0a 2320 4d6f  t/markdown..# Mo
+000005b0: 6e67 6f44 422d 4f44 4d0a 0a3c 7020 616c  ngoDB-ODM..<p al
+000005c0: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+000005d0: 2020 3c65 6d3e 4d6f 6e67 6f44 422d 4f44    <em>MongoDB-OD
+000005e0: 4d2c 204e 4f53 514c 2064 6174 6162 6173  M, NOSQL databas
+000005f0: 6573 2069 6e20 5079 7468 6f6e 2c20 6465  es in Python, de
+00000600: 7369 676e 6564 2066 6f72 2073 696d 706c  signed for simpl
+00000610: 6963 6974 792c 2063 6f6d 7061 7469 6269  icity, compatibi
+00000620: 6c69 7479 2c20 616e 6420 726f 6275 7374  lity, and robust
+00000630: 6e65 7373 2e3c 2f65 6d3e 0a3c 2f70 3e0a  ness.</em>.</p>.
+00000640: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000650: 7222 3e0a 0a3c 6120 6872 6566 3d22 6874  r">..<a href="ht
+00000660: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000670: 2f6e 6179 616e 3332 6269 7377 6173 2f6d  /nayan32biswas/m
+00000680: 6f6e 676f 6462 2d6f 646d 2f61 6374 696f  ongodb-odm/actio
+00000690: 6e73 2f77 6f72 6b66 6c6f 7773 2f74 6573  ns/workflows/tes
+000006a0: 742e 796d 6c22 2074 6172 6765 743d 225f  t.yml" target="_
+000006b0: 626c 616e 6b22 3e0a 2020 2020 3c69 6d67  blank">.    <img
+000006c0: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
+000006d0: 7468 7562 2e63 6f6d 2f6e 6179 616e 3332  thub.com/nayan32
+000006e0: 6269 7377 6173 2f6d 6f6e 676f 6462 2d6f  biswas/mongodb-o
+000006f0: 646d 2f61 6374 696f 6e73 2f77 6f72 6b66  dm/actions/workf
+00000700: 6c6f 7773 2f74 6573 742e 796d 6c2f 6261  lows/test.yml/ba
+00000710: 6467 652e 7376 673f 6272 616e 6368 3d6d  dge.svg?branch=m
+00000720: 6169 6e26 6576 656e 743d 7075 7368 2220  ain&event=push" 
+00000730: 616c 743d 2254 6573 7422 3e0a 3c2f 613e  alt="Test">.</a>
+00000740: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00000750: 2f2f 636f 7665 7261 6765 2d62 6164 6765  //coverage-badge
+00000760: 2e73 616d 7565 6c63 6f6c 7669 6e2e 776f  .samuelcolvin.wo
+00000770: 726b 6572 732e 6465 762f 7265 6469 7265  rkers.dev/redire
+00000780: 6374 2f6e 6179 616e 3332 6269 7377 6173  ct/nayan32biswas
+00000790: 2f6d 6f6e 676f 6462 2d6f 646d 2220 7461  /mongodb-odm" ta
+000007a0: 7267 6574 3d22 5f62 6c61 6e6b 223e 0a20  rget="_blank">. 
+000007b0: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+000007c0: 7073 3a2f 2f63 6f76 6572 6167 652d 6261  ps://coverage-ba
+000007d0: 6467 652e 7361 6d75 656c 636f 6c76 696e  dge.samuelcolvin
+000007e0: 2e77 6f72 6b65 7273 2e64 6576 2f6e 6179  .workers.dev/nay
+000007f0: 616e 3332 6269 7377 6173 2f6d 6f6e 676f  an32biswas/mongo
+00000800: 6462 2d6f 646d 2e73 7667 2220 616c 743d  db-odm.svg" alt=
+00000810: 2243 6f76 6572 6167 6522 3e0a 3c62 7220  "Coverage">.<br 
+00000820: 2f3e 0a3c 6120 6872 6566 3d22 6874 7470  />.<a href="http
+00000830: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000840: 6a65 6374 2f6d 6f6e 676f 6462 2d6f 646d  ject/mongodb-odm
+00000850: 2f22 2074 6172 6765 743d 225f 626c 616e  /" target="_blan
+00000860: 6b22 3e0a 2020 2020 3c69 6d67 2061 6c74  k">.    <img alt
+00000870: 3d22 5079 5049 2220 7372 633d 2268 7474  ="PyPI" src="htt
+00000880: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000890: 2e69 6f2f 7079 7069 2f76 2f6d 6f6e 676f  .io/pypi/v/mongo
+000008a0: 6462 2d6f 646d 3f63 6f6c 6f72 3d25 3233  db-odm?color=%23
+000008b0: 3334 4430 3538 266c 6162 656c 3d50 7950  34D058&label=PyP
+000008c0: 6925 3230 5061 636b 6167 6522 3e0a 3c2f  i%20Package">.</
+000008d0: 613e 0a3c 6120 6872 6566 3d22 6874 7470  a>.<a href="http
+000008e0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+000008f0: 6a65 6374 2f6d 6f6e 676f 6462 2d6f 646d  ject/mongodb-odm
+00000900: 2f22 2074 6172 6765 743d 225f 626c 616e  /" target="_blan
+00000910: 6b22 3e0a 2020 2020 3c69 6d67 2061 6c74  k">.    <img alt
+00000920: 3d22 5079 5049 202d 2050 7974 686f 6e20  ="PyPI - Python 
+00000930: 5665 7273 696f 6e22 2073 7263 3d22 6874  Version" src="ht
+00000940: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000950: 732e 696f 2f70 7970 692f 7079 7665 7273  s.io/pypi/pyvers
+00000960: 696f 6e73 2f6d 6f6e 676f 6462 2d6f 646d  ions/mongodb-odm
+00000970: 3f63 6f6c 6f72 3d25 3233 3334 4430 3538  ?color=%2334D058
+00000980: 223e 0a3c 2f61 3e0a 0a3c 2f70 3e0a 0a2d  ">.</a>..</p>..-
+00000990: 2d2d 0a0a 2a2a 446f 6375 6d65 6e74 6174  --..**Documentat
+000009a0: 696f 6e2a 2a3a 203c 6120 6872 6566 3d22  ion**: <a href="
+000009b0: 6874 7470 733a 2f2f 6d6f 6e67 6f64 622d  https://mongodb-
+000009c0: 6f64 6d2e 7265 6164 7468 6564 6f63 732e  odm.readthedocs.
+000009d0: 696f 2220 7461 7267 6574 3d22 5f62 6c61  io" target="_bla
+000009e0: 6e6b 223e 6874 7470 733a 2f2f 6d6f 6e67  nk">https://mong
+000009f0: 6f64 622d 6f64 6d2e 7265 6164 7468 6564  odb-odm.readthed
+00000a00: 6f63 732e 696f 3c2f 613e 0a0a 2a2a 5079  ocs.io</a>..**Py
+00000a10: 5069 2a2a 3a20 3c61 2068 7265 663d 2268  Pi**: <a href="h
+00000a20: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+00000a30: 7072 6f6a 6563 742f 6d6f 6e67 6f64 622d  project/mongodb-
+00000a40: 6f64 6d22 2074 6172 6765 743d 225f 626c  odm" target="_bl
+00000a50: 616e 6b22 3e68 7474 7073 3a2f 2f70 7970  ank">https://pyp
+00000a60: 692e 6f72 672f 7072 6f6a 6563 742f 6d6f  i.org/project/mo
+00000a70: 6e67 6f64 622d 6f64 6d3c 2f61 3e0a 0a2a  ngodb-odm</a>..*
+00000a80: 2a52 6570 6f73 6974 6f72 792a 2a3a 203c  *Repository**: <
+00000a90: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000aa0: 6769 7468 7562 2e63 6f6d 2f6e 6179 616e  github.com/nayan
+00000ab0: 3332 6269 7377 6173 2f6d 6f6e 676f 6462  32biswas/mongodb
+00000ac0: 2d6f 646d 2220 7461 7267 6574 3d22 5f62  -odm" target="_b
+00000ad0: 6c61 6e6b 223e 6874 7470 733a 2f2f 6769  lank">https://gi
+00000ae0: 7468 7562 2e63 6f6d 2f6e 6179 616e 3332  thub.com/nayan32
+00000af0: 6269 7377 6173 2f6d 6f6e 676f 6462 2d6f  biswas/mongodb-o
+00000b00: 646d 3c2f 613e 0a0a 2d2d 2d0a 0a23 2320  dm</a>..---..## 
+00000b10: 496e 7472 6f64 7563 7469 6f6e 0a0a 5468  Introduction..Th
+00000b20: 6520 7075 7270 6f73 6520 6f66 2074 6869  e purpose of thi
+00000b30: 7320 6d6f 6475 6c65 2069 7320 746f 2070  s module is to p
+00000b40: 726f 7669 6465 2065 6173 7920 6163 6365  rovide easy acce
+00000b50: 7373 2074 6f20 7468 6520 6461 7461 6261  ss to the databa
+00000b60: 7365 2077 6974 6820 7468 6520 7079 7468  se with the pyth
+00000b70: 6f6e 206f 626a 6563 7420 6665 6174 7572  on object featur
+00000b80: 6520 7769 7468 202a 2a4d 6f6e 676f 4442  e with **MongoDB
+00000b90: 2a2a 2061 6e64 202a 2a50 794d 6f6e 676f  ** and **PyMongo
+00000ba0: 2a2a 2e20 5769 7468 2050 794d 6f6e 676f  **. With PyMongo
+00000bb0: 2074 6861 7420 7761 7320 7665 7279 2065   that was very e
+00000bc0: 6173 7920 746f 206d 616b 6520 7370 656c  asy to make spel
+00000bd0: 6c69 6e67 206d 6973 7461 6b65 7320 696e  ling mistakes in
+00000be0: 2061 2063 6f6c 6c65 6374 696f 6e20 6e61   a collection na
+00000bf0: 6d65 2077 6865 6e20 796f 7520 6172 6520  me when you are 
+00000c00: 646f 696e 6720 6461 7461 6261 7365 206f  doing database o
+00000c10: 7065 7261 7469 6f6e 2e20 5468 6973 206d  peration. This m
+00000c20: 6f64 756c 6520 7072 6f76 6964 6573 2079  odule provides y
+00000c30: 6f75 2077 6974 6820 6d69 6e69 6d61 6c20  ou with minimal 
+00000c40: 4f44 4d20 7769 7468 2061 206d 6f64 656c  ODM with a model
+00000c50: 696e 6720 6665 6174 7572 6520 736f 2074  ing feature so t
+00000c60: 6861 7420 796f 7520 646f 6ee2 8099 7420  hat you don...t 
+00000c70: 6861 7665 2074 6f20 6c6f 6f6b 2075 7020  have to look up 
+00000c80: 7468 6520 4d6f 6e67 6f44 4220 6461 7368  the MongoDB dash
+00000c90: 626f 6172 6428 4d6f 6e67 6f20 436f 6d70  board(Mongo Comp
+00000ca0: 6173 7329 2074 6f20 6b6e 6f77 2061 626f  ass) to know abo
+00000cb0: 7574 2066 6965 6c64 206e 616d 6573 206f  ut field names o
+00000cc0: 7220 6461 7461 2074 7970 6573 2e0a 0a2a  r data types...*
+00000cd0: 2a4d 6f6e 676f 4442 2d4f 444d 2a2a 2069  *MongoDB-ODM** i
+00000ce0: 7320 6261 7365 6420 6f6e 2050 7974 686f  s based on Pytho
+00000cf0: 6e20 7479 7065 2061 6e6e 6f74 6174 696f  n type annotatio
+00000d00: 6e73 2c20 616e 6420 706f 7765 7265 6420  ns, and powered 
+00000d10: 6279 203c 6120 6872 6566 3d22 6874 7470  by <a href="http
+00000d20: 733a 2f2f 7079 6d6f 6e67 6f2e 7265 6164  s://pymongo.read
+00000d30: 7468 6564 6f63 732e 696f 2f65 6e2f 7374  thedocs.io/en/st
+00000d40: 6162 6c65 2f22 2063 6c61 7373 3d22 6578  able/" class="ex
+00000d50: 7465 726e 616c 2d6c 696e 6b22 2074 6172  ternal-link" tar
+00000d60: 6765 743d 225f 626c 616e 6b22 3e50 794d  get="_blank">PyM
+00000d70: 6f6e 676f 3c2f 613e 2061 6e64 203c 6120  ongo</a> and <a 
+00000d80: 6872 6566 3d22 6874 7470 733a 2f2f 646f  href="https://do
+00000d90: 6373 2e70 7964 616e 7469 632e 6465 762f  cs.pydantic.dev/
+00000da0: 2220 636c 6173 733d 2265 7874 6572 6e61  " class="externa
+00000db0: 6c2d 6c69 6e6b 2220 7461 7267 6574 3d22  l-link" target="
+00000dc0: 5f62 6c61 6e6b 223e 5079 6461 6e74 6963  _blank">Pydantic
+00000dd0: 3c2f 613e 2e0a 0a54 6865 206b 6579 2066  </a>...The key f
+00000de0: 6561 7475 7265 7320 6172 653a 0a0a 2d20  eatures are:..- 
+00000df0: 2a2a 496e 7475 6974 6976 6520 746f 2077  **Intuitive to w
+00000e00: 7269 7465 2a2a 3a20 4772 6561 7420 6564  rite**: Great ed
+00000e10: 6974 6f72 2073 7570 706f 7274 2e20 436f  itor support. Co
+00000e20: 6d70 6c65 7469 6f6e 2065 7665 7279 7768  mpletion everywh
+00000e30: 6572 652e 204c 6573 7320 7469 6d65 2064  ere. Less time d
+00000e40: 6562 7567 6769 6e67 2e20 4465 7369 676e  ebugging. Design
+00000e50: 6564 2074 6f20 6265 2065 6173 7920 746f  ed to be easy to
+00000e60: 2075 7365 2061 6e64 206c 6561 726e 2e20   use and learn. 
+00000e70: 4c65 7373 2074 696d 6520 7265 6164 696e  Less time readin
+00000e80: 6720 646f 6373 2e0a 2d20 2a2a 4561 7379  g docs..- **Easy
+00000e90: 2074 6f20 7573 652a 2a3a 2049 7420 6861   to use**: It ha
+00000ea0: 7320 7365 6e73 6962 6c65 2064 6566 6175  s sensible defau
+00000eb0: 6c74 7320 616e 6420 646f 6573 2061 206c  lts and does a l
+00000ec0: 6f74 206f 6620 776f 726b 2075 6e64 6572  ot of work under
+00000ed0: 6e65 6174 6820 746f 2073 696d 706c 6966  neath to simplif
+00000ee0: 7920 7468 6520 636f 6465 2079 6f75 2077  y the code you w
+00000ef0: 7269 7465 2e0a 2d20 2a2a 436f 6d70 6174  rite..- **Compat
+00000f00: 6962 6c65 2a2a 3a20 4974 2069 7320 6465  ible**: It is de
+00000f10: 7369 676e 6564 2074 6f20 6265 2063 6f6d  signed to be com
+00000f20: 7061 7469 626c 6520 7769 7468 202a 2a46  patible with **F
+00000f30: 6173 7441 5049 2a2a 2c20 2a2a 5079 6461  astAPI**, **Pyda
+00000f40: 6e74 6963 2a2a 2c20 616e 6420 2a2a 5079  ntic**, and **Py
+00000f50: 4d6f 6e67 6f2a 2a2e 0a2d 202a 2a45 7874  Mongo**..- **Ext
+00000f60: 656e 7369 626c 652a 2a3a 2059 6f75 2068  ensible**: You h
+00000f70: 6176 6520 616c 6c20 7468 6520 706f 7765  ave all the powe
+00000f80: 7220 6f66 202a 2a50 794d 6f6e 676f 2a2a  r of **PyMongo**
+00000f90: 2061 6e64 202a 2a50 7964 616e 7469 632a   and **Pydantic*
+00000fa0: 2a20 756e 6465 726e 6561 7468 2e0a 2d20  * underneath..- 
+00000fb0: 2a2a 5368 6f72 742a 2a3a 204d 696e 696d  **Short**: Minim
+00000fc0: 697a 6520 636f 6465 2064 7570 6c69 6361  ize code duplica
+00000fd0: 7469 6f6e 2e20 4120 7369 6e67 6c65 2074  tion. A single t
+00000fe0: 7970 6520 616e 6e6f 7461 7469 6f6e 2064  ype annotation d
+00000ff0: 6f65 7320 6120 6c6f 7420 6f66 2077 6f72  oes a lot of wor
+00001000: 6b2e 204e 6f20 6e65 6564 2074 6f20 6475  k. No need to du
+00001010: 706c 6963 6174 6520 6d6f 6465 6c73 2069  plicate models i
+00001020: 6e20 2a2a 5079 4d6f 6e67 6f2a 2a20 616e  n **PyMongo** an
+00001030: 6420 5079 6461 6e74 6963 2e0a 0a2d 2d2d  d Pydantic...---
+00001040: 0a0a 2323 2052 6571 7569 7265 6d65 6e74  ..## Requirement
+00001050: 0a0a 2a2a 4d6f 6e67 6f44 422d 4f44 4d2a  ..**MongoDB-ODM*
+00001060: 2a20 7769 6c6c 2077 6f72 6b20 6f6e 203c  * will work on <
+00001070: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00001080: 7777 772e 7079 7468 6f6e 2e6f 7267 2f64  www.python.org/d
+00001090: 6f77 6e6c 6f61 6473 2f22 2063 6c61 7373  ownloads/" class
+000010a0: 3d22 6578 7465 726e 616c 2d6c 696e 6b22  ="external-link"
+000010b0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+000010c0: 3e50 7974 686f 6e20 332e 3820 616e 6420  >Python 3.8 and 
+000010d0: 6162 6f76 653c 2f61 3e0a 0a54 6869 7320  above</a>..This 
+000010e0: 2a2a 4d6f 6e67 6f44 422d 4f44 4d2a 2a20  **MongoDB-ODM** 
+000010f0: 6973 2062 7569 6c74 206f 6e20 746f 7020  is built on top 
+00001100: 6f66 202a 2a50 794d 6f6e 676f 2a2a 2061  of **PyMongo** a
+00001110: 6e64 202a 2a50 7964 616e 7469 632a 2a2e  nd **Pydantic**.
+00001120: 2054 686f 7365 2070 6163 6b61 6765 7320   Those packages 
+00001130: 6172 6520 7265 7175 6972 6564 2061 6e64  are required and
+00001140: 2077 696c 6c20 6175 746f 2d69 6e73 7461   will auto-insta
+00001150: 6c6c 2077 6869 6c65 202a 2a4d 6f6e 676f  ll while **Mongo
+00001160: 4442 2d4f 444d 2a2a 2077 6173 2069 6e73  DB-ODM** was ins
+00001170: 7461 6c6c 6564 2e0a 0a23 2320 496e 7374  talled...## Inst
+00001180: 616c 6c61 7469 6f6e 0a0a 6060 6063 6f6e  allation..```con
+00001190: 736f 6c65 0a24 2070 6970 2069 6e73 7461  sole.$ pip insta
+000011a0: 6c6c 206d 6f6e 676f 6462 2d6f 646d 0a60  ll mongodb-odm.`
+000011b0: 6060 0a0a 2323 2045 7861 6d70 6c65 0a0a  ``..## Example..
+000011c0: 2323 2320 4465 6669 6e65 206d 6f64 656c  ### Define model
+000011d0: 0a0a 6060 6050 7974 686f 6e0a 696d 706f  ..```Python.impo
+000011e0: 7274 206f 730a 6672 6f6d 2074 7970 696e  rt os.from typin
+000011f0: 6720 696d 706f 7274 204f 7074 696f 6e61  g import Optiona
+00001200: 6c0a 0a66 726f 6d20 6d6f 6e67 6f64 625f  l..from mongodb_
+00001210: 6f64 6d20 696d 706f 7274 2041 5343 454e  odm import ASCEN
+00001220: 4449 4e47 2c20 446f 6375 6d65 6e74 2c20  DING, Document, 
+00001230: 496e 6465 784d 6f64 656c 2c20 636f 6e6e  IndexModel, conn
+00001240: 6563 740a 0a0a 636c 6173 7320 506c 6179  ect...class Play
+00001250: 6572 2844 6f63 756d 656e 7429 3a0a 2020  er(Document):.  
+00001260: 2020 6e61 6d65 3a20 7374 720a 2020 2020    name: str.    
+00001270: 636f 756e 7472 795f 636f 6465 3a20 7374  country_code: st
+00001280: 720a 2020 2020 7261 7469 6e67 3a20 4f70  r.    rating: Op
+00001290: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+000012a0: 6e65 0a0a 2020 2020 636c 6173 7320 436f  ne..    class Co
+000012b0: 6e66 6967 2844 6f63 756d 656e 742e 436f  nfig(Document.Co
+000012c0: 6e66 6967 293a 0a20 2020 2020 2020 2069  nfig):.        i
+000012d0: 6e64 6578 6573 203d 205b 0a20 2020 2020  ndexes = [.     
+000012e0: 2020 2020 2020 2049 6e64 6578 4d6f 6465         IndexMode
+000012f0: 6c28 5b28 2272 6174 696e 6722 2c20 4153  l([("rating", AS
+00001300: 4345 4e44 494e 4729 5d29 2c0a 2020 2020  CENDING)]),.    
+00001310: 2020 2020 5d0a 6060 600a 0a23 2323 2053      ].```..### S
+00001320: 6574 2043 6f6e 6e65 6374 696f 6e0a 0a60  et Connection..`
+00001330: 6060 5079 7468 6f6e 0a63 6f6e 6e65 6374  ``Python.connect
+00001340: 286f 732e 656e 7669 726f 6e2e 6765 7428  (os.environ.get(
+00001350: 224d 4f4e 474f 5f55 524c 222c 2022 6d6f  "MONGO_URL", "mo
+00001360: 6e67 6f64 623a 2f2f 6c6f 6361 6c68 6f73  ngodb://localhos
+00001370: 743a 3237 3031 372f 7465 7374 6462 2229  t:27017/testdb")
+00001380: 290a 6060 600a 0a23 2323 2043 7265 6174  ).```..### Creat
+00001390: 6520 446f 6375 6d65 6e74 0a0a 6060 6050  e Document..```P
+000013a0: 7974 686f 6e0a 7065 6c65 203d 2050 6c61  ython.pele = Pla
+000013b0: 7965 7228 6e61 6d65 3d22 5065 6cc3 a922  yer(name="Pel.."
+000013c0: 2c20 636f 756e 7472 795f 636f 6465 3d22  , country_code="
+000013d0: 4252 4122 292e 6372 6561 7465 2829 0a6d  BRA").create().m
+000013e0: 6172 6164 6f6e 6120 3d20 506c 6179 6572  aradona = Player
+000013f0: 286e 616d 653d 2244 6965 676f 204d 6172  (name="Diego Mar
+00001400: 6164 6f6e 6122 2c20 636f 756e 7472 795f  adona", country_
+00001410: 636f 6465 3d22 4152 4722 2c20 7261 7469  code="ARG", rati
+00001420: 6e67 3d39 3729 2e63 7265 6174 6528 290a  ng=97).create().
+00001430: 7a69 6461 6e65 203d 2050 6c61 7965 7228  zidane = Player(
+00001440: 6e61 6d65 3d22 5a69 6e65 6469 6e65 205a  name="Zinedine Z
+00001450: 6964 616e 6522 2c20 636f 756e 7472 795f  idane", country_
+00001460: 636f 6465 3d22 4652 4122 2c20 7261 7469  code="FRA", rati
+00001470: 6e67 3d39 3629 2e63 7265 6174 6528 290a  ng=96).create().
+00001480: 6060 600a 0a23 2323 2052 6574 7269 6576  ```..### Retriev
+00001490: 6520 446f 6375 6d65 6e74 0a0a 2323 2323  e Document..####
+000014a0: 2046 696e 6420 6461 7461 2066 726f 6d20   Find data from 
+000014b0: 636f 6c6c 6563 7469 6f6e 0a0a 6060 6050  collection..```P
+000014c0: 7974 686f 6e0a 666f 7220 706c 6179 6572  ython.for player
+000014d0: 2069 6e20 506c 6179 6572 2e66 696e 6428   in Player.find(
+000014e0: 293a 0a20 2020 2070 7269 6e74 2870 6c61  ):.    print(pla
+000014f0: 7965 7229 0a60 6060 0a0a 2323 2323 2046  yer).```..#### F
+00001500: 696e 6420 6f6e 6520 6f62 6a65 6374 2077  ind one object w
+00001510: 6974 6820 6669 6c74 6572 0a0a 6060 6050  ith filter..```P
+00001520: 7974 686f 6e0a 706c 6179 6572 203d 2050  ython.player = P
+00001530: 6c61 7965 722e 6669 6e64 5f6f 6e65 287b  layer.find_one({
+00001540: 226e 616d 6522 3a20 2250 656c c3a9 227d  "name": "Pel.."}
+00001550: 290a 6060 600a 0a23 2323 2055 7064 6174  ).```..### Updat
+00001560: 6520 4461 7461 0a0a 6060 6050 7974 686f  e Data..```Pytho
+00001570: 6e0a 706c 6179 6572 203d 2050 6c61 7965  n.player = Playe
+00001580: 722e 6669 6e64 5f6f 6e65 287b 226e 616d  r.find_one({"nam
+00001590: 6522 3a20 2250 656c c3a9 227d 290a 6966  e": "Pel.."}).if
+000015a0: 2070 6c61 7965 723a 0a20 2020 2070 6c61   player:.    pla
+000015b0: 7965 722e 7261 7469 6e67 203d 2039 3820  yer.rating = 98 
+000015c0: 2023 2070 6f74 656e 7469 616c 0a20 2020   # potential.   
+000015d0: 2070 6c61 7965 722e 7570 6461 7465 2829   player.update()
+000015e0: 0a60 6060 0a0a 2323 2320 4465 6c65 7465  .```..### Delete
+000015f0: 2044 6174 610a 0a60 6060 5079 7468 6f6e   Data..```Python
+00001600: 0a70 6c61 7965 7220 3d20 506c 6179 6572  .player = Player
+00001610: 2e66 696e 645f 6f6e 6528 7b22 6e61 6d65  .find_one({"name
+00001620: 223a 2022 5065 6cc3 a922 7d29 0a69 6620  ": "Pel.."}).if 
+00001630: 706c 6179 6572 3a0a 2020 2020 706c 6179  player:.    play
+00001640: 6572 2e64 656c 6574 6528 290a 6060 600a  er.delete().```.
+00001650: 0a23 2323 2041 7070 6c79 2049 6e64 6578  .### Apply Index
+00001660: 6573 0a0a 6060 6050 7974 686f 6e0a 696d  es..```Python.im
+00001670: 706f 7274 206f 730a 6672 6f6d 2074 7970  port os.from typ
+00001680: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
+00001690: 6e61 6c0a 0a66 726f 6d20 6d6f 6e67 6f64  nal..from mongod
+000016a0: 625f 6f64 6d20 696d 706f 7274 2041 5343  b_odm import ASC
+000016b0: 454e 4449 4e47 2c20 446f 6375 6d65 6e74  ENDING, Document
+000016c0: 2c20 496e 6465 784d 6f64 656c 2c20 636f  , IndexModel, co
+000016d0: 6e6e 6563 740a 0a0a 636c 6173 7320 506c  nnect...class Pl
+000016e0: 6179 6572 2844 6f63 756d 656e 7429 3a0a  ayer(Document):.
+000016f0: 2020 2020 6e61 6d65 3a20 7374 720a 2020      name: str.  
+00001700: 2020 636f 756e 7472 795f 636f 6465 3a20    country_code: 
+00001710: 7374 720a 2020 2020 7261 7469 6e67 3a20  str.    rating: 
+00001720: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+00001730: 4e6f 6e65 0a0a 2020 2020 636c 6173 7320  None..    class 
+00001740: 436f 6e66 6967 2844 6f63 756d 656e 742e  Config(Document.
+00001750: 436f 6e66 6967 293a 0a20 2020 2020 2020  Config):.       
+00001760: 2069 6e64 6578 6573 203d 205b 0a20 2020   indexes = [.   
+00001770: 2020 2020 2020 2020 2049 6e64 6578 4d6f           IndexMo
+00001780: 6465 6c28 5b28 2272 6174 696e 6722 2c20  del([("rating", 
+00001790: 4153 4345 4e44 494e 4729 5d29 2c0a 2020  ASCENDING)]),.  
+000017a0: 2020 2020 2020 5d0a 6060 600a 0a2d 2054        ].```..- T
+000017b0: 6f20 6372 6561 7465 2069 6e64 6578 6573  o create indexes
+000017c0: 2069 6e20 7468 6520 6461 7461 6261 7365   in the database
+000017d0: 2064 6563 6c61 7265 205b 496e 6465 784d   declare [IndexM
+000017e0: 6f64 656c 5d28 6874 7470 733a 2f2f 7079  odel](https://py
+000017f0: 6d6f 6e67 6f2e 7265 6164 7468 6564 6f63  mongo.readthedoc
+00001800: 732e 696f 2f65 6e2f 7374 6162 6c65 2f74  s.io/en/stable/t
+00001810: 7574 6f72 6961 6c2e 6874 6d6c 2369 6e64  utorial.html#ind
+00001820: 6578 696e 6729 2061 6e64 2061 7373 6967  exing) and assig
+00001830: 6e20 696e 2069 6e64 6578 6573 2061 7272  n in indexes arr
+00001840: 6179 2069 6e20 436f 6e66 6967 2063 6c61  ay in Config cla
+00001850: 7373 2e20 2a2a 496e 6465 784d 6f64 656c  ss. **IndexModel
+00001860: 2a2a 206d 6f64 756c 6573 2074 6861 7420  ** modules that 
+00001870: 6172 6520 6469 7265 6374 6c79 2069 6d70  are directly imp
+00001880: 6f72 7465 6420 6672 6f6d 202a 2a70 796d  orted from **pym
+00001890: 6f6e 676f 2a2a 2e0a 2d20 496d 706f 7274  ongo**..- Import
+000018a0: 2074 6865 2060 6170 706c 795f 696e 6465   the `apply_inde
+000018b0: 7865 7360 2066 726f 6d20 606d 6f6e 676f  xes` from `mongo
+000018c0: 6462 5f6f 646d 602e 2043 616c 6c20 7468  db_odm`. Call th
+000018d0: 6520 6061 7070 6c79 5f69 6e64 6578 6573  e `apply_indexes
+000018e0: 6020 6675 6e63 7469 6f6e 2066 726f 6d20  ` function from 
+000018f0: 796f 7572 2043 4c49 2e20 596f 7520 6361  your CLI. You ca
+00001900: 6e20 7573 6520 3c61 2068 7265 663d 2268  n use <a href="h
+00001910: 7474 7073 3a2f 2f74 7970 6572 2e74 6961  ttps://typer.tia
+00001920: 6e67 6f6c 6f2e 636f 6d22 2063 6c61 7373  ngolo.com" class
+00001930: 3d22 6578 7465 726e 616c 2d6c 696e 6b22  ="external-link"
+00001940: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00001950: 3e54 7970 6572 3c2f 613e 2074 6f20 696d  >Typer</a> to im
+00001960: 706c 656d 656e 7420 434c 492e 0a0a 2323  plement CLI...##
+00001970: 2045 7861 6d70 6c65 2043 6f64 650a 0a54   Example Code..T
+00001980: 6869 7320 6973 2074 6865 2065 7861 6d70  his is the examp
+00001990: 6c65 206f 6620 6675 6c6c 2063 6f64 6520  le of full code 
+000019a0: 6f66 2061 626f 7665 2e0a 0a60 6060 7079  of above...```py
+000019b0: 7468 6f6e 0a69 6d70 6f72 7420 6f73 0a66  thon.import os.f
+000019c0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+000019d0: 7420 4f70 7469 6f6e 616c 0a0a 6672 6f6d  t Optional..from
+000019e0: 206d 6f6e 676f 6462 5f6f 646d 2069 6d70   mongodb_odm imp
+000019f0: 6f72 7420 4153 4345 4e44 494e 472c 2044  ort ASCENDING, D
+00001a00: 6f63 756d 656e 742c 2049 6e64 6578 4d6f  ocument, IndexMo
+00001a10: 6465 6c2c 2063 6f6e 6e65 6374 0a0a 0a63  del, connect...c
+00001a20: 6c61 7373 2050 6c61 7965 7228 446f 6375  lass Player(Docu
+00001a30: 6d65 6e74 293a 0a20 2020 206e 616d 653a  ment):.    name:
+00001a40: 2073 7472 0a20 2020 2063 6f75 6e74 7279   str.    country
+00001a50: 5f63 6f64 653a 2073 7472 0a20 2020 2072  _code: str.    r
+00001a60: 6174 696e 673a 204f 7074 696f 6e61 6c5b  ating: Optional[
+00001a70: 696e 745d 203d 204e 6f6e 650a 0a20 2020  int] = None..   
+00001a80: 2063 6c61 7373 2043 6f6e 6669 6728 446f   class Config(Do
+00001a90: 6375 6d65 6e74 2e43 6f6e 6669 6729 3a0a  cument.Config):.
+00001aa0: 2020 2020 2020 2020 696e 6465 7865 7320          indexes 
+00001ab0: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+00001ac0: 496e 6465 784d 6f64 656c 285b 2822 7261  IndexModel([("ra
+00001ad0: 7469 6e67 222c 2041 5343 454e 4449 4e47  ting", ASCENDING
+00001ae0: 295d 292c 0a20 2020 2020 2020 205d 0a0a  )]),.        ]..
+00001af0: 0a63 6f6e 6e65 6374 286f 732e 656e 7669  .connect(os.envi
+00001b00: 726f 6e2e 6765 7428 224d 4f4e 474f 5f55  ron.get("MONGO_U
+00001b10: 524c 222c 2022 6d6f 6e67 6f64 623a 2f2f  RL", "mongodb://
+00001b20: 6c6f 6361 6c68 6f73 743a 3237 3031 372f  localhost:27017/
+00001b30: 7465 7374 6462 2229 290a 0a70 656c 6520  testdb"))..pele 
+00001b40: 3d20 506c 6179 6572 286e 616d 653d 2250  = Player(name="P
+00001b50: 656c c3a9 222c 2063 6f75 6e74 7279 5f63  el..", country_c
+00001b60: 6f64 653d 2242 5241 2229 2e63 7265 6174  ode="BRA").creat
+00001b70: 6528 290a 6d61 7261 646f 6e61 203d 2050  e().maradona = P
+00001b80: 6c61 7965 7228 6e61 6d65 3d22 4469 6567  layer(name="Dieg
+00001b90: 6f20 4d61 7261 646f 6e61 222c 2063 6f75  o Maradona", cou
+00001ba0: 6e74 7279 5f63 6f64 653d 2241 5247 222c  ntry_code="ARG",
+00001bb0: 2072 6174 696e 673d 3937 292e 6372 6561   rating=97).crea
+00001bc0: 7465 2829 0a7a 6964 616e 6520 3d20 506c  te().zidane = Pl
+00001bd0: 6179 6572 286e 616d 653d 225a 696e 6564  ayer(name="Zined
+00001be0: 696e 6520 5a69 6461 6e65 222c 2063 6f75  ine Zidane", cou
+00001bf0: 6e74 7279 5f63 6f64 653d 2246 5241 222c  ntry_code="FRA",
+00001c00: 2072 6174 696e 673d 3936 292e 6372 6561   rating=96).crea
+00001c10: 7465 2829 0a0a 666f 7220 706c 6179 6572  te()..for player
+00001c20: 2069 6e20 506c 6179 6572 2e66 696e 6428   in Player.find(
+00001c30: 293a 0a20 2020 2070 7269 6e74 2870 6c61  ):.    print(pla
+00001c40: 7965 7229 0a0a 706c 6179 6572 203d 2050  yer)..player = P
+00001c50: 6c61 7965 722e 6669 6e64 5f6f 6e65 287b  layer.find_one({
+00001c60: 226e 616d 6522 3a20 2250 656c c3a9 227d  "name": "Pel.."}
+00001c70: 290a 6966 2070 6c61 7965 723a 0a20 2020  ).if player:.   
+00001c80: 2070 6c61 7965 722e 7261 7469 6e67 203d   player.rating =
+00001c90: 2039 3820 2023 2070 6f74 656e 7469 616c   98  # potential
+00001ca0: 0a20 2020 2070 6c61 7965 722e 7570 6461  .    player.upda
+00001cb0: 7465 2829 0a0a 706c 6179 6572 203d 2050  te()..player = P
+00001cc0: 6c61 7965 722e 6669 6e64 5f6f 6e65 287b  layer.find_one({
+00001cd0: 226e 616d 6522 3a20 2250 656c c3a9 227d  "name": "Pel.."}
+00001ce0: 290a 6966 2070 6c61 7965 723a 0a20 2020  ).if player:.   
+00001cf0: 2070 6c61 7965 722e 6465 6c65 7465 2829   player.delete()
+00001d00: 0a60 6060 0a0a 2323 2320 5375 7070 6f72  .```..### Suppor
+00001d10: 7465 6420 4672 616d 6577 6f72 6b0a 0a2a  ted Framework..*
+00001d20: 2a4d 6f6e 676f 4442 2d4f 444d 2a2a 2069  *MongoDB-ODM** i
+00001d30: 7320 6e6f 7420 6672 616d 6577 6f72 6b20  s not framework 
+00001d40: 6465 7065 6e64 656e 742e 2057 6520 6361  dependent. We ca
+00001d50: 6e20 7573 6520 7468 6973 2070 6163 6b61  n use this packa
+00001d60: 6765 2069 6e20 616e 7920 7379 7374 656d  ge in any system
+00001d70: 2e20 4275 7420 7765 2074 616b 6520 7370  . But we take sp
+00001d80: 6563 6961 6c20 636f 6e73 6964 6572 6174  ecial considerat
+00001d90: 696f 6e20 6265 696e 6720 636f 6d70 6174  ion being compat
+00001da0: 6962 6c65 2077 6974 6820 3c61 2068 7265  ible with <a hre
+00001db0: 663d 2268 7474 7073 3a2f 2f66 6173 7461  f="https://fasta
+00001dc0: 7069 2e74 6961 6e67 6f6c 6f2e 636f 6d2f  pi.tiangolo.com/
+00001dd0: 2220 636c 6173 733d 2265 7874 6572 6e61  " class="externa
+00001de0: 6c2d 6c69 6e6b 2220 7461 7267 6574 3d22  l-link" target="
+00001df0: 5f62 6c61 6e6b 223e 4661 7374 4150 493c  _blank">FastAPI<
+00001e00: 2f61 3e20 616e 6420 3c61 2068 7265 663d  /a> and <a href=
+00001e10: 2268 7474 7073 3a2f 2f66 6c61 736b 2e70  "https://flask.p
+00001e20: 616c 6c65 7473 7072 6f6a 6563 7473 2e63  alletsprojects.c
+00001e30: 6f6d 2f65 6e2f 322e 322e 782f 2220 636c  om/en/2.2.x/" cl
+00001e40: 6173 733d 2265 7874 6572 6e61 6c2d 6c69  ass="external-li
+00001e50: 6e6b 2220 7461 7267 6574 3d22 5f62 6c61  nk" target="_bla
+00001e60: 6e6b 223e 466c 6173 6b3c 2f61 3e2e 0a0a  nk">Flask</a>...
+00001e70: 2323 2320 4372 6564 6974 0a0a 5468 6973  ### Credit..This
+00001e80: 2070 6163 6b61 6765 2069 7320 6275 696c   package is buil
+00001e90: 7420 6f6e 2074 6f70 206f 6620 3c61 2068  t on top of <a h
+00001ea0: 7265 663d 2268 7474 7073 3a2f 2f70 796d  ref="https://pym
+00001eb0: 6f6e 676f 2e72 6561 6474 6865 646f 6373  ongo.readthedocs
+00001ec0: 2e69 6f2f 656e 2f73 7461 626c 6522 2063  .io/en/stable" c
+00001ed0: 6c61 7373 3d22 6578 7465 726e 616c 2d6c  lass="external-l
+00001ee0: 696e 6b22 2074 6172 6765 743d 225f 626c  ink" target="_bl
+00001ef0: 616e 6b22 3e50 794d 6f6e 676f 3c2f 613e  ank">PyMongo</a>
+00001f00: 2061 6e64 203c 6120 6872 6566 3d22 6874   and <a href="ht
+00001f10: 7470 733a 2f2f 646f 6373 2e70 7964 616e  tps://docs.pydan
+00001f20: 7469 632e 6465 7622 2063 6c61 7373 3d22  tic.dev" class="
+00001f30: 6578 7465 726e 616c 2d6c 696e 6b22 2074  external-link" t
+00001f40: 6172 6765 743d 225f 626c 616e 6b22 3e50  arget="_blank">P
+00001f50: 7964 616e 7469 633c 2f61 3e2e 0a0a 446f  ydantic</a>...Do
+00001f60: 6375 6d65 6e74 6174 696f 6e20 6765 6e65  cumentation gene
+00001f70: 7261 7465 6420 6279 203c 6120 6872 6566  rated by <a href
+00001f80: 3d22 6874 7470 733a 2f2f 7777 772e 6d6b  ="https://www.mk
+00001f90: 646f 6373 2e6f 7267 2f22 2063 6c61 7373  docs.org/" class
+00001fa0: 3d22 6578 7465 726e 616c 2d6c 696e 6b22  ="external-link"
+00001fb0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00001fc0: 3e4d 6b44 6f63 733c 2f61 3e20 616e 6420  >MkDocs</a> and 
+00001fd0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00001fe0: 2f73 7175 6964 6675 6e6b 2e67 6974 6875  /squidfunk.githu
+00001ff0: 622e 696f 2f6d 6b64 6f63 732d 6d61 7465  b.io/mkdocs-mate
+00002000: 7269 616c 2f22 2063 6c61 7373 3d22 6578  rial/" class="ex
+00002010: 7465 726e 616c 2d6c 696e 6b22 2074 6172  ternal-link" tar
+00002020: 6765 743d 225f 626c 616e 6b22 3e4d 6174  get="_blank">Mat
+00002030: 6572 6961 6c20 666f 7220 4d6b 446f 6373  erial for MkDocs
+00002040: 3c2f 613e 2e0a 0a44 6f63 756d 656e 7461  </a>...Documenta
+00002050: 7469 6f6e 2069 6e73 7069 7265 6420 6279  tion inspired by
+00002060: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00002070: 2f2f 7371 6c6d 6f64 656c 2e74 6961 6e67  //sqlmodel.tiang
+00002080: 6f6c 6f2e 636f 6d22 2063 6c61 7373 3d22  olo.com" class="
+00002090: 6578 7465 726e 616c 2d6c 696e 6b22 2074  external-link" t
+000020a0: 6172 6765 743d 225f 626c 616e 6b22 3e53  arget="_blank">S
+000020b0: 514c 4d6f 6465 6c3c 2f61 3e2e 0a0a 4275  QLModel</a>...Bu
+000020c0: 7420 7765 2075 7365 206f 7468 6572 2070  t we use other p
+000020d0: 6163 6b61 6765 7320 666f 7220 6465 7665  ackages for deve
+000020e0: 6c6f 706d 656e 7420 616e 6420 6f74 6865  lopment and othe
+000020f0: 7220 7075 7270 6f73 6573 2e20 4368 6563  r purposes. Chec
+00002100: 6b20 2a2a 7079 7072 6f6a 6563 742e 746f  k **pyproject.to
+00002110: 6d6c 2a2a 2074 6f20 6b6e 6f77 2061 626f  ml** to know abo
+00002120: 7574 2061 6c6c 2070 6163 6b61 6765 7320  ut all packages 
+00002130: 7765 2075 7365 2074 6f20 6275 696c 6420  we use to build 
+00002140: 7468 6973 2070 6163 6b61 6765 2e0a 0a23  this package...#
+00002150: 2320 4c69 6365 6e73 650a 0a54 6869 7320  # License..This 
+00002160: 7072 6f6a 6563 7420 6973 206c 6963 656e  project is licen
+00002170: 7365 6420 756e 6465 7220 7468 6520 7465  sed under the te
+00002180: 726d 7320 6f66 2074 6865 205b 4d49 5420  rms of the [MIT 
+00002190: 6c69 6365 6e73 655d 2868 7474 7073 3a2f  license](https:/
+000021a0: 2f67 6974 6875 622e 636f 6d2f 6e61 7961  /github.com/naya
+000021b0: 6e33 3262 6973 7761 732f 6d6f 6e67 6f64  n32biswas/mongod
+000021c0: 622d 6f64 6d2f 626c 6f62 2f6d 6169 6e2f  b-odm/blob/main/
+000021d0: 4c49 4345 4e53 4529 2e0a 0a              LICENSE)...
```

