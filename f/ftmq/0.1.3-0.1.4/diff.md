# Comparing `tmp/ftmq-0.1.3.tar.gz` & `tmp/ftmq-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftmq-0.1.3.tar", max compression
+gzip compressed data, was "ftmq-0.1.4.tar", max compression
```

## Comparing `ftmq-0.1.3.tar` & `ftmq-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1077 2023-04-04 14:31:45.930293 ftmq-0.1.3/LICENSE
--rw-r--r--   0        0        0     4376 2023-06-20 10:59:09.516461 ftmq-0.1.3/README.md
--rw-r--r--   0        0        0       22 2023-06-21 05:48:36.344091 ftmq-0.1.3/ftmq/__init__.py
--rw-r--r--   0        0        0     2714 2023-06-20 10:59:09.516461 ftmq-0.1.3/ftmq/cli.py
--rw-r--r--   0        0        0       43 2023-02-17 15:30:40.666516 ftmq-0.1.3/ftmq/exceptions.py
--rw-r--r--   0        0        0     5115 2023-06-14 18:50:42.961409 ftmq-0.1.3/ftmq/filters.py
--rw-r--r--   0        0        0     1964 2023-06-20 10:59:09.516461 ftmq-0.1.3/ftmq/io.py
--rw-r--r--   0        0        0     1784 2023-06-14 17:04:10.502390 ftmq-0.1.3/ftmq/query.py
--rw-r--r--   0        0        0      383 2023-06-14 15:32:48.293679 ftmq-0.1.3/ftmq/types.py
--rw-r--r--   0        0        0      973 2023-06-14 20:07:15.762203 ftmq-0.1.3/ftmq/util.py
--rw-r--r--   0        0        0     1316 2023-06-21 05:48:36.344091 ftmq-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5549 1970-01-01 00:00:00.000000 ftmq-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-04 14:31:45.930293 ftmq-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4376 2023-06-20 10:59:09.516461 ftmq-0.1.4/README.md
+-rw-r--r--   0        0        0       22 2023-07-27 08:29:13.876418 ftmq-0.1.4/ftmq/__init__.py
+-rw-r--r--   0        0        0     2714 2023-06-20 10:59:09.516461 ftmq-0.1.4/ftmq/cli.py
+-rw-r--r--   0        0        0       43 2023-02-17 15:30:40.666516 ftmq-0.1.4/ftmq/exceptions.py
+-rw-r--r--   0        0        0     5115 2023-06-14 18:50:42.961409 ftmq-0.1.4/ftmq/filters.py
+-rw-r--r--   0        0        0     2151 2023-07-26 18:11:21.346315 ftmq-0.1.4/ftmq/io.py
+-rw-r--r--   0        0        0     1784 2023-06-14 17:04:10.502390 ftmq-0.1.4/ftmq/query.py
+-rw-r--r--   0        0        0      383 2023-06-14 15:32:48.293679 ftmq-0.1.4/ftmq/types.py
+-rw-r--r--   0        0        0      973 2023-06-14 20:07:15.762203 ftmq-0.1.4/ftmq/util.py
+-rw-r--r--   0        0        0     1388 2023-07-27 08:29:13.876418 ftmq-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5646 1970-01-01 00:00:00.000000 ftmq-0.1.4/PKG-INFO
```

### Comparing `ftmq-0.1.3/LICENSE` & `ftmq-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.3/README.md` & `ftmq-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.3/ftmq/cli.py` & `ftmq-0.1.4/ftmq/cli.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.3/ftmq/filters.py` & `ftmq-0.1.4/ftmq/filters.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.3/ftmq/io.py` & `ftmq-0.1.4/ftmq/io.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import contextlib
 import sys
 from typing import Any, Iterable, Literal
 
 import orjson
+from banal import is_listish
 from followthemoney import model
 from nomenklatura.entity import CE, CompositeEntity
 from nomenklatura.util import PathLike
 from smart_open import open
 
 from .types import CEGenerator, SDict
 
@@ -30,25 +31,32 @@
         yield fh
     finally:
         if fh not in (sys.stdout.buffer, sys.stdin.buffer):
             fh.close()
 
 
 def smart_read_proxies(
-    uri: PathLike, mode: str | None = "rb", serialize: bool | None = True
+    uri: PathLike | Iterable[PathLike],
+    mode: str | None = "rb",
+    serialize: bool | None = True,
 ) -> CEGenerator:
+    if is_listish(uri):
+        for u in uri:
+            yield from smart_read_proxies(u, mode, serialize)
+        return
+
     with smart_open(uri, sys.stdin.buffer, mode=mode) as fh:
         while True:
             line = fh.readline()
             if not line:
                 break
             data = orjson.loads(line)
             if serialize:
                 data = load_proxy(data)
-            data.datasets.discard("default")
+                data.datasets.discard("default")
             yield data
 
 
 def smart_write_proxies(
     uri: PathLike,
     proxies: Iterable[CE | SDict],
     mode: str | None = "wb",
```

### Comparing `ftmq-0.1.3/ftmq/query.py` & `ftmq-0.1.4/ftmq/query.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.3/ftmq/util.py` & `ftmq-0.1.4/ftmq/util.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.3/pyproject.toml` & `ftmq-0.1.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ftmq"
-version = "0.1.3"
+version = "0.1.4"
 description = "followthemoney query dsl and io helpers"
 authors = ["Simon Wörpel <simon.woerpel@pm.me>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/investigativedata/ftmq"
 repository = "https://github.com/investigativedata/ftmq"
 documentation = "https://github.com/investigativedata/ftmq"
@@ -21,23 +21,26 @@
 ftmq = "ftmq.cli:cli"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/investigativedata/ftmq/issues"
 
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.10,<3.13"
 banal = "^1.0.6"
 followthemoney = "^3.4.0"
-nomenklatura = "^2.14.0"
+nomenklatura = "<3"
 orjson = "^3.9.1"
 PyICU = "^2.11"
 smart-open = {version = "6.3.0", extras = ["all"]}
 click = "^8.1.3"
 click-default-group = "^1.2.2"
+cryptography = ">=41.0.2"
+certifi = ">=2023.07.22"
+scipy = ">=1.10.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
 black = "^23.3.0"
 isort = "^5.12.0"
 mypy = "^1.3.0"
```

### Comparing `ftmq-0.1.3/PKG-INFO` & `ftmq-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: ftmq
-Version: 0.1.3
+Version: 0.1.4
 Summary: followthemoney query dsl and io helpers
 Home-page: https://github.com/investigativedata/ftmq
 License: MIT
 Author: Simon Wörpel
 Author-email: simon.woerpel@pm.me
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<3.13
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyICU (>=2.11,<3.0)
 Requires-Dist: banal (>=1.0.6,<2.0.0)
+Requires-Dist: certifi (>=2023.07.22)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
+Requires-Dist: cryptography (>=41.0.2)
 Requires-Dist: followthemoney (>=3.4.0,<4.0.0)
-Requires-Dist: nomenklatura (>=2.14.0,<3.0.0)
+Requires-Dist: nomenklatura (<3)
 Requires-Dist: orjson (>=3.9.1,<4.0.0)
+Requires-Dist: scipy (>=1.10.0)
 Requires-Dist: smart-open[all] (==6.3.0)
 Project-URL: Bug Tracker, https://github.com/investigativedata/ftmq/issues
 Project-URL: Documentation, https://github.com/investigativedata/ftmq
 Project-URL: Repository, https://github.com/investigativedata/ftmq
 Description-Content-Type: text/markdown
 
 [![ftmq on pypi](https://img.shields.io/pypi/v/ftmq)](https://pypi.org/project/ftmq/) [![Python test and package](https://github.com/investigativedata/ftmq/actions/workflows/python.yml/badge.svg)](https://github.com/investigativedata/ftmq/actions/workflows/python.yml) [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit) [![Coverage Status](https://coveralls.io/repos/github/investigativedata/ftmq/badge.svg?branch=main)](https://coveralls.io/github/investigativedata/ftmq?branch=main) [![MIT License](https://img.shields.io/pypi/l/ftmq)](./LICENSE)
```

