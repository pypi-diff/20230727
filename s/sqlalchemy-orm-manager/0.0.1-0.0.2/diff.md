# Comparing `tmp/sqlalchemy_orm_manager-0.0.1.tar.gz` & `tmp/sqlalchemy_orm_manager-0.0.2.tar.gz`

## Comparing `sqlalchemy_orm_manager-0.0.1.tar` & `sqlalchemy_orm_manager-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.1/Pipfile
--rw-r--r--   0        0        0    22994 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.1/Pipfile.lock
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.1/pytest.ini
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.1/sqlalchemy_manager/__init__.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.1/sqlalchemy_manager/decorators.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.1/sqlalchemy_manager/exceptions.py
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.1/sqlalchemy_manager/managers.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.1/sqlalchemy_manager/meta.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.1/sqlalchemy_manager/pagination.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.1/tests/test_manager.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.1/LICENSE
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.1/README.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/Pipfile
+-rw-r--r--   0        0        0    22994 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/Pipfile.lock
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/pytest.ini
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/sqlalchemy_manager/__init__.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/sqlalchemy_manager/decorators.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/sqlalchemy_manager/exceptions.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/sqlalchemy_manager/managers.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/sqlalchemy_manager/meta.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/sqlalchemy_manager/pagination.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/tests/test_manager.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/README.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/PKG-INFO
```

### Comparing `sqlalchemy_orm_manager-0.0.1/Pipfile.lock` & `sqlalchemy_orm_manager-0.0.2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `sqlalchemy_orm_manager-0.0.1/sqlalchemy_manager/decorators.py` & `sqlalchemy_orm_manager-0.0.2/sqlalchemy_manager/decorators.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_orm_manager-0.0.1/sqlalchemy_manager/managers.py` & `sqlalchemy_orm_manager-0.0.2/sqlalchemy_manager/managers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Generic, Tuple, Type, TypeVar, Union
+from typing import Any, Generic, Tuple, Type, TypeVar, Union
 
 from sqlalchemy import select
 from sqlalchemy.exc import NoResultFound
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.orm import Session
 
 from .meta import ManagerMeta
@@ -46,16 +46,23 @@
         if not instance:
             instance = self.model(**kwargs)
             await self.create(instance, commit)
             created = True
 
         return instance, created
 
-    async def search(self, params: dict, page: int = 1) -> Pagination:
-        statement = select(self.model).filter_by(**params)
+    async def search(self, *criteria: Any, **params: dict) -> Pagination:
+        page = params.pop('page', 1)
+        statement = select(self.model)
+
+        if params:
+            statement = statement.filter_by(**params)
+
+        if criteria:
+            statement = statement.where(*criteria)
 
         pagination = await self.paginator_class(self.model, self.session, statement, page).paginate()
 
         return pagination
 
     async def update(self, instance: T, **kwargs):
         for key, value in kwargs.items():
@@ -98,16 +105,23 @@
         if not instance:
             instance = self.model(**kwargs)
             self.create(instance, commit)
             created = True
 
         return instance, created
 
-    def search(self, params: dict, page: int = 1) -> Pagination:
-        statement = select(self.model).filter_by(**params)
+    def search(self, *criteria: Any, **params: dict) -> Pagination:
+        page = params.pop('page', 1)
+        statement = select(self.model)
+
+        if params:
+            statement = statement.filter_by(**params)
+
+        if criteria:
+            statement = statement.where(*criteria)
 
         return self.paginator_class(self.model, self.session, statement, page).paginate()
 
     def update(self, instance: T, **kwargs):
         for key, value in kwargs.items():
             setattr(instance, key, value)
```

### Comparing `sqlalchemy_orm_manager-0.0.1/sqlalchemy_manager/meta.py` & `sqlalchemy_orm_manager-0.0.2/sqlalchemy_manager/meta.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_orm_manager-0.0.1/sqlalchemy_manager/pagination.py` & `sqlalchemy_orm_manager-0.0.2/sqlalchemy_manager/pagination.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_orm_manager-0.0.1/tests/conftest.py` & `sqlalchemy_orm_manager-0.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_orm_manager-0.0.1/tests/test_manager.py` & `sqlalchemy_orm_manager-0.0.2/tests/test_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+from sqlalchemy import and_
 
 from tests import User
 
 
 def test_create(user_manager):
     user_name = 'Bob'
 
@@ -63,19 +64,27 @@
     assert not created
 
 
 def test_search(user_manager):
     user_manager.create(User(name='Bob', lastname='Johnson'))
     user_manager.create(User(name='Bob', lastname='Carlson'))
 
-    result = user_manager.search({'name': 'Bob'})
+    result = user_manager.search(name='Bob')
 
     assert result.total == 2
 
-    result = user_manager.search({'lastname': 'Carlson'})
+    result = user_manager.search(lastname='Carlson')
+
+    assert result.total == 1
+
+    result = user_manager.search(name='Bob', lastname='Johnson')
+
+    assert result.total == 1
+
+    result = user_manager.search(and_(User.name == 'Bob', User.lastname == 'Johnson'))
 
     assert result.total == 1
 
 
 @pytest.mark.asyncio
 async def test_async_create(get_async_user_manager):
     user_manager = await get_async_user_manager
@@ -151,16 +160,24 @@
 @pytest.mark.asyncio
 async def test_async_search(get_async_user_manager):
     user_manager = await get_async_user_manager
 
     await user_manager.create(User(name='Bob', lastname='Johnson'))
     await user_manager.create(User(name='Bob', lastname='Carlson'))
 
-    result = await user_manager.search({'name': 'Bob'})
+    result = await user_manager.search(name='Bob')
 
     assert result.total == 2
 
-    result = await user_manager.search({'lastname': 'Carlson'})
+    result = await user_manager.search(lastname='Carlson')
+
+    assert result.total == 1
+
+    result = await user_manager.search(name='Bob', lastname='Johnson')
+
+    assert result.total == 1
+
+    result = await user_manager.search(and_(User.name == 'Bob', User.lastname == 'Johnson'))
 
     assert result.total == 1
 
     await user_manager.session.close()
```

### Comparing `sqlalchemy_orm_manager-0.0.1/.gitignore` & `sqlalchemy_orm_manager-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlalchemy_orm_manager-0.0.1/LICENSE` & `sqlalchemy_orm_manager-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_orm_manager-0.0.1/README.md` & `sqlalchemy_orm_manager-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_orm_manager-0.0.1/pyproject.toml` & `sqlalchemy_orm_manager-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sqlalchemy_orm_manager"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "Nazar Kaliuzhnyi", email = "kaluzghnyy@gmail.com" },
 ]
 description = "A base manager class to handle CRUD on SQLAlchemy models."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sqlalchemy_orm_manager-0.0.1/PKG-INFO` & `sqlalchemy_orm_manager-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy_orm_manager
-Version: 0.0.1
+Version: 0.0.2
 Summary: A base manager class to handle CRUD on SQLAlchemy models.
 Project-URL: Homepage, https://github.com/nakeeon/SQLAlchemy-Manager
 Author-email: Nazar Kaliuzhnyi <kaluzghnyy@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

