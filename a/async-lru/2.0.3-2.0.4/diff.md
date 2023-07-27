# Comparing `tmp/async-lru-2.0.3.tar.gz` & `tmp/async-lru-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async-lru-2.0.3.tar", last modified: Fri Jul  7 19:00:21 2023, max compression
+gzip compressed data, was "async-lru-2.0.4.tar", last modified: Thu Jul 27 19:12:01 2023, max compression
```

## Comparing `async-lru-2.0.3.tar` & `async-lru-2.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:00:21.228657 async-lru-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-07 18:59:59.000000 async-lru-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-07 18:59:59.000000 async-lru-2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-07 18:59:59.000000 async-lru-2.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-07 19:00:21.228657 async-lru-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-07-07 18:59:59.000000 async-lru-2.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:00:21.228657 async-lru-2.0.3/async_lru/
--rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-07-07 18:59:59.000000 async-lru-2.0.3/async_lru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:59:59.000000 async-lru-2.0.3/async_lru/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:00:21.228657 async-lru-2.0.3/async_lru.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-07 19:00:21.000000 async-lru-2.0.3/async_lru.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-07 19:00:21.000000 async-lru-2.0.3/async_lru.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:00:21.000000 async-lru-2.0.3/async_lru.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-07 19:00:21.000000 async-lru-2.0.3/async_lru.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 19:00:21.000000 async-lru-2.0.3/async_lru.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-07 19:00:21.232658 async-lru-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-07 18:59:59.000000 async-lru-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:00:21.228657 async-lru-2.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-07 18:59:59.000000 async-lru-2.0.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-07-07 18:59:59.000000 async-lru-2.0.3/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-07 18:59:59.000000 async-lru-2.0.3/tests/test_cache_clear.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-07 18:59:59.000000 async-lru-2.0.3/tests/test_cache_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-07 18:59:59.000000 async-lru-2.0.3/tests/test_cache_invalidate.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-07 18:59:59.000000 async-lru-2.0.3/tests/test_close.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-07 18:59:59.000000 async-lru-2.0.3/tests/test_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-07-07 18:59:59.000000 async-lru-2.0.3/tests/test_internals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-07 18:59:59.000000 async-lru-2.0.3/tests/test_partialmethod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-07 18:59:59.000000 async-lru-2.0.3/tests/test_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-07 18:59:59.000000 async-lru-2.0.3/tests/test_ttl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:12:01.223422 async-lru-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-27 19:11:41.000000 async-lru-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-27 19:11:41.000000 async-lru-2.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-27 19:11:41.000000 async-lru-2.0.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-27 19:12:01.223422 async-lru-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-27 19:11:41.000000 async-lru-2.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:12:01.219421 async-lru-2.0.4/async_lru/
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-07-27 19:11:41.000000 async-lru-2.0.4/async_lru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:11:41.000000 async-lru-2.0.4/async_lru/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:12:01.219421 async-lru-2.0.4/async_lru.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-27 19:12:01.000000 async-lru-2.0.4/async_lru.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-27 19:12:01.000000 async-lru-2.0.4/async_lru.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:12:01.000000 async-lru-2.0.4/async_lru.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-27 19:12:01.000000 async-lru-2.0.4/async_lru.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-27 19:12:01.000000 async-lru-2.0.4/async_lru.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-27 19:12:01.223422 async-lru-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-27 19:11:41.000000 async-lru-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:12:01.223422 async-lru-2.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-27 19:11:41.000000 async-lru-2.0.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-07-27 19:11:41.000000 async-lru-2.0.4/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-27 19:11:41.000000 async-lru-2.0.4/tests/test_cache_clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-27 19:11:41.000000 async-lru-2.0.4/tests/test_cache_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-27 19:11:41.000000 async-lru-2.0.4/tests/test_cache_invalidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-27 19:11:41.000000 async-lru-2.0.4/tests/test_close.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-27 19:11:41.000000 async-lru-2.0.4/tests/test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-07-27 19:11:41.000000 async-lru-2.0.4/tests/test_internals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-27 19:11:41.000000 async-lru-2.0.4/tests/test_partialmethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-27 19:11:41.000000 async-lru-2.0.4/tests/test_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-27 19:11:41.000000 async-lru-2.0.4/tests/test_ttl.py
```

### Comparing `async-lru-2.0.3/LICENSE` & `async-lru-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `async-lru-2.0.3/PKG-INFO` & `async-lru-2.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-lru
-Version: 2.0.3
+Version: 2.0.4
 Summary: Simple LRU cache for asyncio
 Home-page: https://github.com/aio-libs/async-lru
 Maintainer: aiohttp team <team@aiohttp.org>
 Maintainer-email: team@aiohttp.org
 License: MIT License
 Project-URL: Chat: Matrix, https://matrix.to/#/#aio-libs:matrix.org
 Project-URL: Chat: Matrix Space, https://matrix.to/#/#aio-libs-space:matrix.org
@@ -16,48 +16,51 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-async_lru
+async-lru
 =========
 
 :info: Simple lru cache for asyncio
 
-.. image:: https://travis-ci.com/aio-libs/async_lru.svg?branch=master
-    :target: https://travis-ci.com/aio-libs/async_lru
+.. image:: https://github.com/aio-libs/async-lru/actions/workflows/ci-cd.yml/badge.svg?event=push
+   :target: https://github.com/aio-libs/async-lru/actions/workflows/ci-cd.yml?query=event:push
+   :alt: GitHub Actions CI/CD workflows status
+
+.. image:: https://img.shields.io/pypi/v/async-lru.svg?logo=Python&logoColor=white
+   :target: https://pypi.org/project/async-lru
+   :alt: async-lru @ PyPI
 
-.. image:: https://img.shields.io/pypi/v/async_lru.svg
-    :target: https://pypi.python.org/pypi/async_lru
-
-.. image:: https://codecov.io/gh/aio-libs/async_lru/branch/master/graph/badge.svg
-    :target: https://codecov.io/gh/aio-libs/async_lru
+.. image:: https://codecov.io/gh/aio-libs/async-lru/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/aio-libs/async-lru
 
 .. image:: https://img.shields.io/matrix/aio-libs:matrix.org?label=Discuss%20on%20Matrix%20at%20%23aio-libs%3Amatrix.org&logo=matrix&server_fqdn=matrix.org&style=flat
    :target: https://matrix.to/#/%23aio-libs:matrix.org
    :alt: Matrix Room — #aio-libs:matrix.org
 
 .. image:: https://img.shields.io/matrix/aio-libs-space:matrix.org?label=Discuss%20on%20Matrix%20at%20%23aio-libs-space%3Amatrix.org&logo=matrix&server_fqdn=matrix.org&style=flat
    :target: https://matrix.to/#/%23aio-libs-space:matrix.org
    :alt: Matrix Space — #aio-libs-space:matrix.org
 
 Installation
 ------------
 
 .. code-block:: shell
 
-    pip install async_lru
+    pip install async-lru
 
 Usage
 -----
 
 This package is a port of Python's built-in `functools.lru_cache <https://docs.python.org/3/library/functools.html#functools.lru_cache>`_ function for `asyncio <https://docs.python.org/3/library/asyncio.html>`_. To better handle async behaviour, it also ensures multiple concurrent calls will only result in 1 call to the wrapped function, with all ``await``\s receiving the result of that call when it completes.
 
 .. code-block:: python
```

### Comparing `async-lru-2.0.3/README.rst` & `async-lru-2.0.4/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-async_lru
+async-lru
 =========
 
 :info: Simple lru cache for asyncio
 
-.. image:: https://travis-ci.com/aio-libs/async_lru.svg?branch=master
-    :target: https://travis-ci.com/aio-libs/async_lru
+.. image:: https://github.com/aio-libs/async-lru/actions/workflows/ci-cd.yml/badge.svg?event=push
+   :target: https://github.com/aio-libs/async-lru/actions/workflows/ci-cd.yml?query=event:push
+   :alt: GitHub Actions CI/CD workflows status
+
+.. image:: https://img.shields.io/pypi/v/async-lru.svg?logo=Python&logoColor=white
+   :target: https://pypi.org/project/async-lru
+   :alt: async-lru @ PyPI
 
-.. image:: https://img.shields.io/pypi/v/async_lru.svg
-    :target: https://pypi.python.org/pypi/async_lru
-
-.. image:: https://codecov.io/gh/aio-libs/async_lru/branch/master/graph/badge.svg
-    :target: https://codecov.io/gh/aio-libs/async_lru
+.. image:: https://codecov.io/gh/aio-libs/async-lru/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/aio-libs/async-lru
 
 .. image:: https://img.shields.io/matrix/aio-libs:matrix.org?label=Discuss%20on%20Matrix%20at%20%23aio-libs%3Amatrix.org&logo=matrix&server_fqdn=matrix.org&style=flat
    :target: https://matrix.to/#/%23aio-libs:matrix.org
    :alt: Matrix Room — #aio-libs:matrix.org
 
 .. image:: https://img.shields.io/matrix/aio-libs-space:matrix.org?label=Discuss%20on%20Matrix%20at%20%23aio-libs-space%3Amatrix.org&logo=matrix&server_fqdn=matrix.org&style=flat
    :target: https://matrix.to/#/%23aio-libs-space:matrix.org
    :alt: Matrix Space — #aio-libs-space:matrix.org
 
 Installation
 ------------
 
 .. code-block:: shell
 
-    pip install async_lru
+    pip install async-lru
 
 Usage
 -----
 
 This package is a port of Python's built-in `functools.lru_cache <https://docs.python.org/3/library/functools.html#functools.lru_cache>`_ function for `asyncio <https://docs.python.org/3/library/asyncio.html>`_. To better handle async behaviour, it also ensures multiple concurrent calls will only result in 1 call to the wrapped function, with all ``await``\s receiving the result of that call when it completes.
 
 .. code-block:: python
```

### Comparing `async-lru-2.0.3/async_lru/__init__.py` & `async-lru-2.0.4/async_lru/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
 
-__version__ = "2.0.3"
+__version__ = "2.0.4"
 
 __all__ = ("alru_cache",)
 
 
 _T = TypeVar("_T")
 _R = TypeVar("_R")
 _Coro = Coroutine[Any, Any, _R]
@@ -115,14 +115,18 @@
         else:
             cache_item.cancel()
             return True
 
     def cache_clear(self) -> None:
         self.__hits = 0
         self.__misses = 0
+
+        for c in self.__cache.values():
+            if c.later_call:
+                c.later_call.cancel()
         self.__cache.clear()
         self.__tasks.clear()
 
     async def cache_close(self, *, wait: bool = False) -> None:
         self.__closed = True
 
         tasks = list(self.__tasks)
@@ -158,15 +162,15 @@
 
     def _cache_miss(self, key: Hashable) -> None:
         self.__misses += 1
 
     def _task_done_callback(
         self, fut: "asyncio.Future[_R]", key: Hashable, task: "asyncio.Task[_R]"
     ) -> None:
-        self.__tasks.remove(task)
+        self.__tasks.discard(task)
 
         cache_item = self.__cache.get(key)
         if self.__ttl is not None and cache_item is not None:
             loop = asyncio.get_running_loop()
             cache_item.later_call = loop.call_later(
                 self.__ttl, self.__cache.pop, key, None
             )
```

### Comparing `async-lru-2.0.3/async_lru.egg-info/PKG-INFO` & `async-lru-2.0.4/async_lru.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-lru
-Version: 2.0.3
+Version: 2.0.4
 Summary: Simple LRU cache for asyncio
 Home-page: https://github.com/aio-libs/async-lru
 Maintainer: aiohttp team <team@aiohttp.org>
 Maintainer-email: team@aiohttp.org
 License: MIT License
 Project-URL: Chat: Matrix, https://matrix.to/#/#aio-libs:matrix.org
 Project-URL: Chat: Matrix Space, https://matrix.to/#/#aio-libs-space:matrix.org
@@ -16,48 +16,51 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-async_lru
+async-lru
 =========
 
 :info: Simple lru cache for asyncio
 
-.. image:: https://travis-ci.com/aio-libs/async_lru.svg?branch=master
-    :target: https://travis-ci.com/aio-libs/async_lru
+.. image:: https://github.com/aio-libs/async-lru/actions/workflows/ci-cd.yml/badge.svg?event=push
+   :target: https://github.com/aio-libs/async-lru/actions/workflows/ci-cd.yml?query=event:push
+   :alt: GitHub Actions CI/CD workflows status
+
+.. image:: https://img.shields.io/pypi/v/async-lru.svg?logo=Python&logoColor=white
+   :target: https://pypi.org/project/async-lru
+   :alt: async-lru @ PyPI
 
-.. image:: https://img.shields.io/pypi/v/async_lru.svg
-    :target: https://pypi.python.org/pypi/async_lru
-
-.. image:: https://codecov.io/gh/aio-libs/async_lru/branch/master/graph/badge.svg
-    :target: https://codecov.io/gh/aio-libs/async_lru
+.. image:: https://codecov.io/gh/aio-libs/async-lru/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/aio-libs/async-lru
 
 .. image:: https://img.shields.io/matrix/aio-libs:matrix.org?label=Discuss%20on%20Matrix%20at%20%23aio-libs%3Amatrix.org&logo=matrix&server_fqdn=matrix.org&style=flat
    :target: https://matrix.to/#/%23aio-libs:matrix.org
    :alt: Matrix Room — #aio-libs:matrix.org
 
 .. image:: https://img.shields.io/matrix/aio-libs-space:matrix.org?label=Discuss%20on%20Matrix%20at%20%23aio-libs-space%3Amatrix.org&logo=matrix&server_fqdn=matrix.org&style=flat
    :target: https://matrix.to/#/%23aio-libs-space:matrix.org
    :alt: Matrix Space — #aio-libs-space:matrix.org
 
 Installation
 ------------
 
 .. code-block:: shell
 
-    pip install async_lru
+    pip install async-lru
 
 Usage
 -----
 
 This package is a port of Python's built-in `functools.lru_cache <https://docs.python.org/3/library/functools.html#functools.lru_cache>`_ function for `asyncio <https://docs.python.org/3/library/asyncio.html>`_. To better handle async behaviour, it also ensures multiple concurrent calls will only result in 1 call to the wrapped function, with all ``await``\s receiving the result of that call when it completes.
 
 .. code-block:: python
```

### Comparing `async-lru-2.0.3/async_lru.egg-info/SOURCES.txt` & `async-lru-2.0.4/async_lru.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `async-lru-2.0.3/setup.cfg` & `async-lru-2.0.4/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	
 	Development Status :: 5 - Production/Stable
 	
 	Framework :: AsyncIO
 keywords = 
 	asyncio
 	lru
@@ -45,15 +46,16 @@
 [options.package_data]
 * = 
 	py.typed
 
 [flake8]
 exclude = .git,.env,__pycache__,.eggs
 max-line-length = 88
-ignore = N801,N802,N803,E252,W503,E133,E203
+extend-select = B950
+ignore = N801,N802,N803,E252,W503,E133,E203,E501
 
 [coverage:run]
 branch = True
 omit = site-packages
 
 [isort]
 line_length = 88
@@ -61,15 +63,15 @@
 multi_line_output = 3
 force_grid_wrap = 0
 combine_as_imports = True
 lines_after_imports = 2
 known_first_party = async_lru
 
 [tool:pytest]
-addopts = -s --keep-duplicates --cache-clear --verbose --no-cov-on-fail --cov=async_lru --cov-report=term --cov-report=html
+addopts = -s --keep-duplicates --cache-clear --verbose --no-cov-on-fail --cov=async_lru --cov=tests/ --cov-report=term --cov-report=html
 filterwarnings = 
 	error
 testpaths = tests/
 junit_family = xunit2
 asyncio_mode = auto
 timeout = 15
```

### Comparing `async-lru-2.0.3/tests/conftest.py` & `async-lru-2.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `async-lru-2.0.3/tests/test_basic.py` & `async-lru-2.0.4/tests/test_basic.py`

 * *Files 5% similar despite different names*

```diff
@@ -139,17 +139,17 @@
 
     assert ret1 == ret2
 
     assert (
         coro1._LRUCacheWrapper__cache[1].fut.result()  # type: ignore[attr-defined]
         == coro2._LRUCacheWrapper__cache[1].fut.result()  # type: ignore[attr-defined]
     )
-    assert coro1._LRUCacheWrapper__cache != coro2._LRUCacheWrapper__cache  # type: ignore[attr-defined]  # noqa: E501
-    assert coro1._LRUCacheWrapper__cache.keys() == coro2._LRUCacheWrapper__cache.keys()  # type: ignore[attr-defined]  # noqa: E501
-    assert coro1._LRUCacheWrapper__cache is not coro2._LRUCacheWrapper__cache  # type: ignore[attr-defined]  # noqa: E501
+    assert coro1._LRUCacheWrapper__cache != coro2._LRUCacheWrapper__cache  # type: ignore[attr-defined]
+    assert coro1._LRUCacheWrapper__cache.keys() == coro2._LRUCacheWrapper__cache.keys()  # type: ignore[attr-defined]
+    assert coro1._LRUCacheWrapper__cache is not coro2._LRUCacheWrapper__cache  # type: ignore[attr-defined]
 
 
 async def test_alru_cache_parameters() -> None:
     @alru_cache
     async def coro(val: int) -> int:
         return val
```

### Comparing `async-lru-2.0.3/tests/test_cache_info.py` & `async-lru-2.0.4/tests/test_cache_info.py`

 * *Files identical despite different names*

### Comparing `async-lru-2.0.3/tests/test_cache_invalidate.py` & `async-lru-2.0.4/tests/test_cache_invalidate.py`

 * *Files identical despite different names*

### Comparing `async-lru-2.0.3/tests/test_close.py` & `async-lru-2.0.4/tests/test_close.py`

 * *Files identical despite different names*

### Comparing `async-lru-2.0.3/tests/test_exception.py` & `async-lru-2.0.4/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `async-lru-2.0.3/tests/test_internals.py` & `async-lru-2.0.4/tests/test_internals.py`

 * *Files identical despite different names*

### Comparing `async-lru-2.0.3/tests/test_partialmethod.py` & `async-lru-2.0.4/tests/test_partialmethod.py`

 * *Files identical despite different names*

### Comparing `async-lru-2.0.3/tests/test_size.py` & `async-lru-2.0.4/tests/test_size.py`

 * *Files identical despite different names*

### Comparing `async-lru-2.0.3/tests/test_ttl.py` & `async-lru-2.0.4/tests/test_ttl.py`

 * *Files identical despite different names*

