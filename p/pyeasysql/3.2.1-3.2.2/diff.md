# Comparing `tmp/pyeasysql-3.2.1.tar.gz` & `tmp/pyeasysql-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeasysql-3.2.1.tar", last modified: Tue Jul 25 17:57:27 2023, max compression
+gzip compressed data, was "pyeasysql-3.2.2.tar", last modified: Thu Jul 27 19:16:07 2023, max compression
```

## Comparing `pyeasysql-3.2.1.tar` & `pyeasysql-3.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 17:57:27.567480 pyeasysql-3.2.1/
-drwxrwxrwx   0        0        0        0 2023-07-25 17:57:27.556295 pyeasysql-3.2.1/EasySQL/
--rw-rw-rw-   0        0        0     3662 2023-07-24 11:39:55.000000 pyeasysql-3.2.1/EasySQL/ABC.py
--rw-rw-rw-   0        0        0     2887 2021-06-27 12:24:21.000000 pyeasysql-3.2.1/EasySQL/Characters.py
--rw-rw-rw-   0        0        0    15044 2023-07-25 08:56:23.000000 pyeasysql-3.2.1/EasySQL/Classes.py
--rw-rw-rw-   0        0        0     6202 2023-07-25 17:49:13.000000 pyeasysql-3.2.1/EasySQL/Commands.py
--rw-rw-rw-   0        0        0      945 2023-07-25 08:49:05.000000 pyeasysql-3.2.1/EasySQL/Constraints.py
--rw-rw-rw-   0        0        0      305 2023-07-11 12:44:34.000000 pyeasysql-3.2.1/EasySQL/Decorators.py
--rw-rw-rw-   0        0        0     2097 2023-07-09 09:35:55.000000 pyeasysql-3.2.1/EasySQL/EasyInstances.py
--rw-rw-rw-   0        0        0      757 2023-06-08 19:41:42.000000 pyeasysql-3.2.1/EasySQL/Exceptions.py
--rw-rw-rw-   0        0        0      457 2021-04-04 16:17:30.000000 pyeasysql-3.2.1/EasySQL/Logging.py
--rw-rw-rw-   0        0        0     3079 2023-07-23 11:44:26.000000 pyeasysql-3.2.1/EasySQL/Types.py
--rw-rw-rw-   0        0        0     2496 2022-04-15 06:15:51.000000 pyeasysql-3.2.1/EasySQL/Where.py
--rw-rw-rw-   0        0        0      298 2023-07-24 15:21:11.000000 pyeasysql-3.2.1/EasySQL/__init__.py
--rw-rw-rw-   0        0        0     1085 2023-07-23 15:33:54.000000 pyeasysql-3.2.1/LICENSE.md
--rw-rw-rw-   0        0        0     6084 2023-07-25 17:57:27.566483 pyeasysql-3.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     5412 2023-07-24 15:30:12.000000 pyeasysql-3.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 17:57:27.564489 pyeasysql-3.2.1/pyeasysql.egg-info/
--rw-rw-rw-   0        0        0     6084 2023-07-25 17:57:27.000000 pyeasysql-3.2.1/pyeasysql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-07-25 17:57:27.000000 pyeasysql-3.2.1/pyeasysql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 17:57:27.000000 pyeasysql-3.2.1/pyeasysql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-25 17:57:27.000000 pyeasysql-3.2.1/pyeasysql.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-25 17:57:27.000000 pyeasysql-3.2.1/pyeasysql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      717 2023-07-25 17:57:19.000000 pyeasysql-3.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-25 17:57:27.567480 pyeasysql-3.2.1/setup.cfg
--rw-rw-rw-   0        0        0      831 2023-07-24 16:25:04.000000 pyeasysql-3.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 19:16:07.844412 pyeasysql-3.2.2/
+drwxrwxrwx   0        0        0        0 2023-07-27 19:16:07.811077 pyeasysql-3.2.2/EasySQL/
+-rw-rw-rw-   0        0        0     3662 2023-07-24 11:39:55.000000 pyeasysql-3.2.2/EasySQL/ABC.py
+-rw-rw-rw-   0        0        0     2887 2021-06-27 12:24:21.000000 pyeasysql-3.2.2/EasySQL/Characters.py
+-rw-rw-rw-   0        0        0    15280 2023-07-27 18:17:08.000000 pyeasysql-3.2.2/EasySQL/Classes.py
+-rw-rw-rw-   0        0        0     6202 2023-07-25 17:49:13.000000 pyeasysql-3.2.2/EasySQL/Commands.py
+-rw-rw-rw-   0        0        0      945 2023-07-25 08:49:05.000000 pyeasysql-3.2.2/EasySQL/Constraints.py
+-rw-rw-rw-   0        0        0      305 2023-07-11 12:44:34.000000 pyeasysql-3.2.2/EasySQL/Decorators.py
+-rw-rw-rw-   0        0        0     2097 2023-07-09 09:35:55.000000 pyeasysql-3.2.2/EasySQL/EasyInstances.py
+-rw-rw-rw-   0        0        0      757 2023-06-08 19:41:42.000000 pyeasysql-3.2.2/EasySQL/Exceptions.py
+-rw-rw-rw-   0        0        0      457 2021-04-04 16:17:30.000000 pyeasysql-3.2.2/EasySQL/Logging.py
+-rw-rw-rw-   0        0        0     3079 2023-07-23 11:44:26.000000 pyeasysql-3.2.2/EasySQL/Types.py
+-rw-rw-rw-   0        0        0     2496 2022-04-15 06:15:51.000000 pyeasysql-3.2.2/EasySQL/Where.py
+-rw-rw-rw-   0        0        0      298 2023-07-24 15:21:11.000000 pyeasysql-3.2.2/EasySQL/__init__.py
+-rw-rw-rw-   0        0        0     1085 2023-07-23 15:33:54.000000 pyeasysql-3.2.2/LICENSE.md
+-rw-rw-rw-   0        0        0     6084 2023-07-27 19:16:07.838993 pyeasysql-3.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5412 2023-07-24 15:30:12.000000 pyeasysql-3.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 19:16:07.836451 pyeasysql-3.2.2/pyeasysql.egg-info/
+-rw-rw-rw-   0        0        0     6084 2023-07-27 19:16:07.000000 pyeasysql-3.2.2/pyeasysql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2023-07-27 19:16:07.000000 pyeasysql-3.2.2/pyeasysql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 19:16:07.000000 pyeasysql-3.2.2/pyeasysql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-27 19:16:07.000000 pyeasysql-3.2.2/pyeasysql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-27 19:16:07.000000 pyeasysql-3.2.2/pyeasysql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      717 2023-07-27 16:55:01.000000 pyeasysql-3.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-27 19:16:07.844412 pyeasysql-3.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      831 2023-07-24 16:25:04.000000 pyeasysql-3.2.2/setup.py
```

### Comparing `pyeasysql-3.2.1/EasySQL/ABC.py` & `pyeasysql-3.2.2/EasySQL/ABC.py`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.1/EasySQL/Characters.py` & `pyeasysql-3.2.2/EasySQL/Characters.py`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.1/EasySQL/Classes.py` & `pyeasysql-3.2.2/EasySQL/Classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         tags = (NOT_NULL,) if NOT_NULL in tags else ()
         super().__init__(name, column.sql_type, *tags, default=default)
 
     def __repr__(self):
         return f'<EasyForeignColumn "{self.name}" reference={self.refer_table.name}({self.refer_column.name})>'
 
     def get_sql(self):
-        return EasyColumn.get_sql(self) + f' REFERENCES {self.refer_table.name}({self.refer_column.name})'
+        return EasyColumn.get_sql(self)
 
 
 class EasyDatabase:
     _database: str = None
     _password: str = None
     _host: str = "127.0.0.1"
     _port: int = 3306
@@ -252,21 +252,24 @@
 
 
 class EasyTable:
     _database: EasyDatabase = NotImplemented
     _name: str = NotImplemented
     _columns: tuple = ()
 
-    PRIMARY: List[EasyColumn] = []
-    UNIQUES: List[Unique] = []
+    PRIMARY: List[EasyColumn] = None
+    UNIQUES: List[Unique] = None
 
     def __init_subclass__(cls, **kwargs):
         for key in ('database', 'name'):
             setattr(cls, f'_{key}', _safe_pop(kwargs, key) or getattr(cls, f'_{key}'))
 
+        cls.PRIMARY = []
+        cls.UNIQUES = []
+
         columns: List[EasyColumn] = [value for value in cls.__dict__.values() if isinstance(value, EasyColumn)]
         for column in columns:
             if UNIQUE in column.tags:
                 cls.UNIQUES.append(Unique(column))
             if PRIMARY in column.tags:
                 cls.PRIMARY.append(column)
 
@@ -302,14 +305,18 @@
         exists = bool(self._database.execute(command, buffered=True).fetchall())
         if not exists:
             if self._columns:
                 command = ', '.join([column.get_sql() for column in self._columns])
                 if len(self.PRIMARY) > 0:
                     command += f", PRIMARY KEY({', '.join(column.name for column in self.PRIMARY)})"
 
+                for column in self._columns:
+                    if isinstance(column, EasyForeignColumn):
+                        command += f", FOREIGN KEY ({column.name}) REFERENCES {column.refer_table.name}({column.refer_column.name})"
+
                 for unique in self.UNIQUES:
                     command += f", {unique.value}"
 
                 command = f"CREATE TABLE {self._name} ({command});"
                 self._database.execute(command)
             else:
                 raise ValueError('No columns where specified and table does not exist')
```

### Comparing `pyeasysql-3.2.1/EasySQL/Commands.py` & `pyeasysql-3.2.2/EasySQL/Commands.py`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.1/EasySQL/Constraints.py` & `pyeasysql-3.2.2/EasySQL/Constraints.py`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.1/EasySQL/EasyInstances.py` & `pyeasysql-3.2.2/EasySQL/EasyInstances.py`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.1/EasySQL/Exceptions.py` & `pyeasysql-3.2.2/EasySQL/Exceptions.py`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.1/EasySQL/Types.py` & `pyeasysql-3.2.2/EasySQL/Types.py`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.1/EasySQL/Where.py` & `pyeasysql-3.2.2/EasySQL/Where.py`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.1/LICENSE.md` & `pyeasysql-3.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.1/PKG-INFO` & `pyeasysql-3.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeasysql
-Version: 3.2.1
+Version: 3.2.2
 Summary: SQL Database management without even a SQL line
 Home-page: https://github.com/AGM-Studio/easysql
 Author: Ashenguard
 Author-email: Ashenguard <ashenguard@agmstudio.xyz>
 Project-URL: Homepage, https://github.com/agm-studio/easysql
 Project-URL: Bug Tracker, https://github.com/agm-studio/easysql/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyeasysql-3.2.1/README.md` & `pyeasysql-3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.1/pyeasysql.egg-info/PKG-INFO` & `pyeasysql-3.2.2/pyeasysql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeasysql
-Version: 3.2.1
+Version: 3.2.2
 Summary: SQL Database management without even a SQL line
 Home-page: https://github.com/AGM-Studio/easysql
 Author: Ashenguard
 Author-email: Ashenguard <ashenguard@agmstudio.xyz>
 Project-URL: Homepage, https://github.com/agm-studio/easysql
 Project-URL: Bug Tracker, https://github.com/agm-studio/easysql/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyeasysql-3.2.1/pyproject.toml` & `pyeasysql-3.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyeasysql"
-version = "3.2.1"
+version = "3.2.2"
 authors = [
   { name="Ashenguard", email="ashenguard@agmstudio.xyz" },
 ]
 description = "SQL Database management without even a SQL line"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `pyeasysql-3.2.1/setup.py` & `pyeasysql-3.2.2/setup.py`

 * *Files identical despite different names*

