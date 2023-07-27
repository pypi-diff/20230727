# Comparing `tmp/asmysql-0.1.0.tar.gz` & `tmp/asmysql-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asmysql-0.1.0.tar", max compression
+gzip compressed data, was "asmysql-0.1.1.tar", max compression
```

## Comparing `asmysql-0.1.0.tar` & `asmysql-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      403 2023-07-16 08:53:39.390539 asmysql-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1063 2023-07-16 09:30:17.834594 asmysql-0.1.0/LICENSE
--rw-r--r--   0        0        0     1628 2023-07-16 08:59:14.610547 asmysql-0.1.0/README.md
--rw-r--r--   0        0        0     1698 2023-07-16 08:55:25.054541 asmysql-0.1.0/README_zh.md
--rw-r--r--   0        0        0       58 2023-07-15 13:39:13.748777 asmysql-0.1.0/asmysql/__init__.py
--rw-r--r--   0        0        0     3566 2023-07-16 08:50:12.754533 asmysql-0.1.0/asmysql/_asmysql.py
--rw-r--r--   0        0        0     1453 2023-07-16 08:43:53.034524 asmysql-0.1.0/asmysql/_cursor_client.py
--rw-r--r--   0        0        0     1387 2023-07-16 08:44:09.054524 asmysql-0.1.0/asmysql/_result.py
--rw-r--r--   0        0        0      883 2023-07-16 09:10:37.618564 asmysql-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2197 1970-01-01 00:00:00.000000 asmysql-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      510 2023-07-25 16:29:04.218975 asmysql-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1063 2023-07-25 16:29:04.218975 asmysql-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1628 2023-07-25 16:29:04.218975 asmysql-0.1.1/README.md
+-rw-r--r--   0        0        0     1698 2023-07-25 16:29:04.218975 asmysql-0.1.1/README_zh.md
+-rw-r--r--   0        0        0     1530 2023-07-25 16:29:04.218975 asmysql-0.1.1/asmysql/__cursor_client.py
+-rw-r--r--   0        0        0       58 2023-07-25 16:29:04.218975 asmysql-0.1.1/asmysql/__init__.py
+-rw-r--r--   0        0        0     3567 2023-07-25 16:29:04.218975 asmysql-0.1.1/asmysql/_asmysql.py
+-rw-r--r--   0        0        0     1670 2023-07-25 16:29:04.218975 asmysql-0.1.1/asmysql/_result.py
+-rw-r--r--   0        0        0     1182 2023-07-27 14:55:25.667736 asmysql-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2529 1970-01-01 00:00:00.000000 asmysql-0.1.1/PKG-INFO
```

### Comparing `asmysql-0.1.0/LICENSE` & `asmysql-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asmysql-0.1.0/README.md` & `asmysql-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `asmysql-0.1.0/README_zh.md` & `asmysql-0.1.1/README_zh.md`

 * *Files identical despite different names*

### Comparing `asmysql-0.1.0/asmysql/_asmysql.py` & `asmysql-0.1.1/asmysql/_asmysql.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Final, final, Optional
 from aiomysql import Pool, create_pool
 
-from ._cursor_client import CursorClient
+from .__cursor_client import CursorClient
 
 
 class AsMysql:
     """异步的数据库aiomysql封装类"""
     host: str = '127.0.0.1'
     port: int = 3306
     user: str = ''
```

### Comparing `asmysql-0.1.0/asmysql/_cursor_client.py` & `asmysql-0.1.1/asmysql/__cursor_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 from aiomysql import Pool
 from pymysql.err import MySQLError
 
 from ._result import Result
 
 
 class CursorClient:
-    """这个是封装aiomysql的cursor客户端"""
+    """这个是封装aiomysql的cursor客户端
+
+    这个是 asmysql 内部使用的类，并不会暴露给客户端
+    """
     def __init__(self, pool: Pool):
         """执行语句参考：
         https://pymysql.readthedocs.io/en/latest/modules/cursors.html
         """
         self.__pool: Pool = pool
 
     def __repr__(self):
```

### Comparing `asmysql-0.1.0/asmysql/_result.py` & `asmysql-0.1.1/asmysql/_result.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Final, Optional
 from typing import AsyncIterator
+from functools import lru_cache
 from aiomysql import Cursor
 
 
 class Result:
     def __init__(self, query: str, *, rows: int = None, cursor: Cursor = None, err: Exception = None):
         if bool(cursor) ^ bool(err):
             self.query: Final[str] = query
@@ -12,14 +13,23 @@
             self.err: Final[Exception] = err
         else:
             raise AttributeError("require arg: cursor or err")
 
     def __repr__(self):
         return f'<{self.__class__.__name__}: {self.query}>'
 
+    @property
+    @lru_cache
+    def err_msg(self):
+        if self.err:
+            err_str = self.err.__str__() or self.err.__doc__.replace('\n', '')
+            return f"{self.err.__class__.__name__} {err_str}"
+        else:
+            return ""
+
     async def fetch_one(self) -> Optional[tuple]:
         """获取一条记录"""
         if not self.err:
             return await self.__cursor.fetchone()
 
     async def fetch_many(self, size: int = None) -> list[tuple]:
         """获取多条记录"""
```

### Comparing `asmysql-0.1.0/pyproject.toml` & `asmysql-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 [tool.poetry]
 name = "asmysql"
-version = "0.1.0"
+version = "0.1.1"
 description = "封装aiomysql的异步mysql客户端引擎。"
 license = "MIT"
 authors = ["vastxiao <vastxiao@gmail.com>"]
 homepage = "https://github.com/Vastxiao/asmysql"
+repository = "https://github.com/Vastxiao/asmysql"
+documentation = "https://github.com/Vastxiao/asmysql/blob/main/README.md"
 keywords = ["async", "asyncio", "mysql", "aiomysql"]
 readme = "README.md"
 include = ["CHANGELOG.md", "README_zh.md"]
 
 [tool.poetry.urls]
-"vastxiao" = "https://vastxiao.github.io/"
+"asmysql readme-zh" = "https://github.com/Vastxiao/asmysql/blob/main/README_zh.md"
+"asmysql changelog" = "https://github.com/Vastxiao/asmysql/blob/main/CHANGELOG.md"
+"vastxiao blog" = "https://vastxiao.github.io/"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiomysql = "^0.2.0"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.14.0"
 
+
 [[tool.poetry.source]]
-name = "ali"
-url = "https://mirrors.aliyun.com/pypi/simple/"
+name = "tx"
+url = "https://mirrors.cloud.tencent.com/pypi/simple"
 priority = "primary"
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "primary"
 [[tool.poetry.source]]
-name = "tx"
-url = "https://mirrors.cloud.tencent.com/pypi/simple"
+name = "ali"
+url = "https://mirrors.aliyun.com/pypi/simple/"
 priority = "primary"
 
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
```

### Comparing `asmysql-0.1.0/PKG-INFO` & `asmysql-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: asmysql
-Version: 0.1.0
+Version: 0.1.1
 Summary: 封装aiomysql的异步mysql客户端引擎。
 Home-page: https://github.com/Vastxiao/asmysql
 License: MIT
 Keywords: async,asyncio,mysql,aiomysql
 Author: vastxiao
 Author-email: vastxiao@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiomysql (>=0.2.0,<0.3.0)
-Project-URL: vastxiao, https://vastxiao.github.io/
+Project-URL: Documentation, https://github.com/Vastxiao/asmysql/blob/main/README.md
+Project-URL: Repository, https://github.com/Vastxiao/asmysql
+Project-URL: asmysql readme-zh, https://github.com/Vastxiao/asmysql/blob/main/README_zh.md
+Project-URL: asmysql changelog, https://github.com/Vastxiao/asmysql/blob/main/CHANGELOG.md
+Project-URL: vastxiao blog, https://vastxiao.github.io/
 Description-Content-Type: text/markdown
 
 # asmysql
 
 ## Introduction
 
 asmysql is a library for using the MySQL asynchronous client, which is a wrapper for aiomysql.
```

