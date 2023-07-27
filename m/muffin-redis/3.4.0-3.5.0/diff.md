# Comparing `tmp/muffin-redis-3.4.0.tar.gz` & `tmp/muffin_redis-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin-redis-3.4.0.tar", last modified: Sat Mar  4 11:43:12 2023, max compression
+gzip compressed data, was "muffin_redis-3.5.0.tar", max compression
```

## Comparing `muffin-redis-3.4.0.tar` & `muffin_redis-3.5.0.tar`

### file list

```diff
@@ -1,16 +1,5 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 11:43:12.829488 muffin-redis-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-04 11:43:03.000000 muffin-redis-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-04 11:43:03.000000 muffin-redis-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-03-04 11:43:12.829488 muffin-redis-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-03-04 11:43:03.000000 muffin-redis-3.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 11:43:12.829488 muffin-redis-3.4.0/muffin_redis/
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-03-04 11:43:03.000000 muffin-redis-3.4.0/muffin_redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 11:43:03.000000 muffin-redis-3.4.0/muffin_redis/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 11:43:12.829488 muffin-redis-3.4.0/muffin_redis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-03-04 11:43:12.000000 muffin-redis-3.4.0/muffin_redis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-04 11:43:12.000000 muffin-redis-3.4.0/muffin_redis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 11:43:12.000000 muffin-redis-3.4.0/muffin_redis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-04 11:43:12.000000 muffin-redis-3.4.0/muffin_redis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-04 11:43:12.000000 muffin-redis-3.4.0/muffin_redis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-03-04 11:43:03.000000 muffin-redis-3.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-04 11:43:12.829488 muffin-redis-3.4.0/setup.cfg
+-rw-r--r--   0        0        0     3575 2023-07-27 13:14:48.743720 muffin_redis-3.5.0/README.rst
+-rw-r--r--   0        0        0     3428 2023-07-27 13:14:48.743720 muffin_redis-3.5.0/muffin_redis/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 13:14:48.743720 muffin_redis-3.5.0/muffin_redis/py.typed
+-rw-r--r--   0        0        0     1926 2023-07-27 13:14:48.747720 muffin_redis-3.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4576 1970-01-01 00:00:00.000000 muffin_redis-3.5.0/PKG-INFO
```

### Comparing `muffin-redis-3.4.0/PKG-INFO` & `muffin_redis-3.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: muffin-redis
-Version: 3.4.0
+Version: 3.5.0
 Summary: Redis support for Muffin framework.
-Author-email: Kirill Klenov <horneds@gmail.com>
-License: MIT License
-Project-URL: homepage, https://github.com/klen/muffin-redis
-Project-URL: repository, https://github.com/klen/muffin-redis
+Home-page: https://github.com/klen/muffin-redis
+License: MIT
 Keywords: redis,muffin,asgi,asyncio
+Author: Kirill Klenov
+Author-email: horneds@gmail.com
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Framework :: AsyncIO
-Requires-Python: >=3.8
+Provides-Extra: redislite
+Requires-Dist: muffin (>=0,<1)
+Requires-Dist: redis (>=4.5.1,<5.0.0)
+Requires-Dist: redislite ; extra == "redislite"
+Project-URL: Repository, https://github.com/klen/muffin-redis
 Description-Content-Type: text/x-rst
-Provides-Extra: tests
-Provides-Extra: dev
-License-File: LICENSE
 
 Muffin-Redis
 ############
 
 .. _description:
 
 Muffin-Redis -- Redis support for Muffin framework.
@@ -49,15 +51,15 @@
 .. contents::
 
 .. _requirements:
 
 Requirements
 =============
 
-- python >= 3.7
+- python >= 3.8
 
 .. _installation:
 
 Installation
 =============
 
 **Muffin-Redis** should be installed using pip: ::
@@ -103,27 +105,27 @@
 
 .. _Asyncio: https://docs.python.org/3/library/asyncio.html
 .. _aioredis: https://github.com/aio-libs/aioredis
 
 Configuration options
 ----------------------
 
-=========================== ======================================= =========================== 
+=========================== ======================================= ===========================
 Name                        Default value                           Description
 --------------------------- --------------------------------------- ---------------------------
 **url**                     ``"redis://localhost"``                 Redis connection URL
 **db**                      ``None``                                Number of the Redis DB
 **password**                ``None``                                Connection password
 **encoding**                ``"utf-8"``                             Connection encoding
 **poolsize**                ``10``                                  Connections pool size (set 0 to disable pooling)
 **decode_responses**        ``True``                                Decode binary responses
 **jsonify**                 ``False``                               Use json to store/read objects with get/set
 **blocking**                ``True``                                Wait for an available connection
 **timeout**                 ``20``                                  Timeout to get a connection
-=========================== ======================================= =========================== 
+=========================== ======================================= ===========================
 
 .. _bugtracker:
 
 Bug tracker
 ===========
 
 If you have any suggestions, bug reports or
@@ -150,7 +152,8 @@
 
 Licensed under a `MIT license`_.
 
 .. _links:
 
 .. _klen: https://github.com/klen
 .. _MIT license: http://opensource.org/licenses/MIT
+
```

### Comparing `muffin-redis-3.4.0/README.rst` & `muffin_redis-3.5.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 .. contents::
 
 .. _requirements:
 
 Requirements
 =============
 
-- python >= 3.7
+- python >= 3.8
 
 .. _installation:
 
 Installation
 =============
 
 **Muffin-Redis** should be installed using pip: ::
@@ -78,27 +78,27 @@
 
 .. _Asyncio: https://docs.python.org/3/library/asyncio.html
 .. _aioredis: https://github.com/aio-libs/aioredis
 
 Configuration options
 ----------------------
 
-=========================== ======================================= =========================== 
+=========================== ======================================= ===========================
 Name                        Default value                           Description
 --------------------------- --------------------------------------- ---------------------------
 **url**                     ``"redis://localhost"``                 Redis connection URL
 **db**                      ``None``                                Number of the Redis DB
 **password**                ``None``                                Connection password
 **encoding**                ``"utf-8"``                             Connection encoding
 **poolsize**                ``10``                                  Connections pool size (set 0 to disable pooling)
 **decode_responses**        ``True``                                Decode binary responses
 **jsonify**                 ``False``                               Use json to store/read objects with get/set
 **blocking**                ``True``                                Wait for an available connection
 **timeout**                 ``20``                                  Timeout to get a connection
-=========================== ======================================= =========================== 
+=========================== ======================================= ===========================
 
 .. _bugtracker:
 
 Bug tracker
 ===========
 
 If you have any suggestions, bug reports or
```

### Comparing `muffin-redis-3.4.0/muffin_redis/__init__.py` & `muffin_redis-3.5.0/muffin_redis/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,63 +1,72 @@
 """Redis support for Muffin framework."""
 
 from __future__ import annotations
 
 from contextlib import suppress
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, Any, ClassVar, Dict, Optional
 
 from asgi_tools._compat import json_dumps, json_loads
 from muffin.plugins import BasePlugin
 from redis.asyncio import BlockingConnectionPool, ConnectionPool, Redis, RedisError
 
 if TYPE_CHECKING:
     from muffin import Application
     from redis.typing import EncodableT, KeyT
 
 
 class Plugin(BasePlugin):
-
     """Manage Redis."""
 
     name = "redis"
-    defaults = {
+    defaults: ClassVar[Dict[str, Any]] = {
         "url": "redis://localhost",
         "db": None,
         "password": None,
         "encoding": "utf-8",
         "decode_responses": True,
         "jsonify": False,
         "poolsize": 10,
         "blocking": True,
         "timeout": 20,
+        "redislite": False,
     }
 
     Error = RedisError
 
-    def __init__(self, app: Optional[Application], **options):
+    def __init__(self, app: Optional[Application] = None, **options):
         """Initialize the plugin."""
         self.__client__: Optional[Redis] = None
+        self.redislite = None
         super().__init__(app, **options)
 
     async def startup(self):
         """Setup a redis connection."""
+        cfg = self.cfg
+
         params = {
-            "db": self.cfg.db,
-            "password": self.cfg.password,
-            "decode_responses": self.cfg.decode_responses,
-            "encoding": self.cfg.encoding,
+            "db": cfg.db,
+            "password": cfg.password,
+            "decode_responses": cfg.decode_responses,
+            "encoding": cfg.encoding,
         }
 
-        if self.cfg.blocking:
-            params["timeout"] = self.cfg.timeout
+        if cfg.blocking:
+            params["timeout"] = cfg.timeout
+
+        pool_cls = BlockingConnectionPool if cfg.blocking else ConnectionPool
+
+        url = cfg.url
+        if cfg.redislite:
+            from redislite import Redis as RedisLite
+
+            self.redislite = RedisLite()
+            url = f"unix://{self.redislite.socket_file}"
 
-        pool_cls = BlockingConnectionPool if self.cfg.blocking else ConnectionPool
-        pool = pool_cls.from_url(
-            self.cfg.url, max_connections=self.cfg.poolsize, **params,
-        )
+        pool = pool_cls.from_url(url, max_connections=cfg.poolsize, **params)
         self.__client__ = Redis(connection_pool=pool)
 
     @property
     def client(self) -> Redis:
         """Return a client instance."""
         if self.__client__ is None:
             raise RuntimeError("Redis Plugin should be started")
@@ -75,14 +84,16 @@
     async def __aexit__(self, *args):
         await self.client.__aexit__(*args)
 
     async def shutdown(self):
         """Close the redis pool."""
         await self.client.close()
         await self.client.connection_pool.disconnect()
+        if self.redislite is not None:
+            self.redislite.shutdown()
 
     def set(
         self,
         name: KeyT,
         value: EncodableT,
         *,
         jsonify: Optional[bool] = None,
```

### Comparing `muffin-redis-3.4.0/pyproject.toml` & `muffin_redis-3.5.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,54 @@
-[project]
+[tool.poetry]
 name = "muffin-redis"
-version = "3.4.0"
+version = "3.5.0"
 description = "Redis support for Muffin framework."
 readme = "README.rst"
-requires-python = ">=3.8"
-license = {"text" = "MIT License"}
-authors = [{ name = "Kirill Klenov", email = "horneds@gmail.com" }]
+license = "MIT"
+authors = ["Kirill Klenov <horneds@gmail.com>"]
+homepage = "https://github.com/klen/muffin-redis"
+repository = "https://github.com/klen/muffin-redis"
 keywords = ["redis", "muffin", "asgi", "asyncio"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Framework :: AsyncIO",
 ]
-dependencies = [
-  "muffin >= 0.92",
-  "redis >= 4.5.1",
-]
-
-[project.urls]
-homepage = "https://github.com/klen/muffin-redis"
-repository = "https://github.com/klen/muffin-redis"
-
-[project.optional-dependencies]
-tests = [
-  "pytest",
-  "pytest-aio",
-  "pytest-mypy",
-  "pytest-redislite",
-  "types-redis",
-  "ruff",
-]
-dev = ["pre-commit", "refurb", "bump2version"]
 
-[tool.setuptools]
-packages = ['muffin_redis']
 
-[tool.setuptools.package-data]
-muffin_redis = ["py.typed"]
+[tool.poetry.dependencies]
+python = "^3.8"
+muffin = "^0"
+redis = "^4.5.1"
+
+# Optional dependencies
+redislite = { version = "*", optional = true }
+
+[tool.poetry.extras]
+redislite = ["redislite"]
+
+[tool.poetry.group.dev.dependencies]
+ipdb = "*"
+ruff = "*"
+black = "*"
+pytest = "*"
+pre-commit = "*"
+pytest-aio = "*"
+pytest-mypy = "*"
 
 [tool.pytest.ini_options]
-addopts = "-xsv"
 log_cli = true
+addopts = "-lxsv"
 
 [tool.mypy]
 packages = ["muffin_redis"]
 install_types = true
 non_interactive = true
 ignore_missing_imports = true
 
@@ -73,8 +70,32 @@
 
 [tool.ruff]
 fix = true
 line-length = 100
 target-version = "py38"
 exclude = [".venv", "docs", "examples"]
 select = ["ALL"]
-ignore = ["D", "UP", "ANN", "DJ", "EM", "RSE", "SLF", "RET", "S101", "PLR2004", "PLR0912", "N804", "A003", "TRY003"]
+ignore = [
+  "D",
+  "UP",
+  "ANN",
+  "DJ",
+  "EM",
+  "RSE",
+  "SLF",
+  "RET",
+  "S101",
+  "PLR2004",
+  "PLR0912",
+  "N804",
+  "A003",
+  "TRY003",
+]
+
+[tool.black]
+line-length = 100
+target-version = ["py311"]
+preview = true
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

