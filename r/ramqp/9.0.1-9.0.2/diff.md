# Comparing `tmp/ramqp-9.0.1.tar.gz` & `tmp/ramqp-9.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramqp-9.0.1.tar", max compression
+gzip compressed data, was "ramqp-9.0.2.tar", max compression
```

## Comparing `ramqp-9.0.1.tar` & `ramqp-9.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0        0        0        0 2023-07-24 11:42:00.967762 ramqp-9.0.1/LICENSES/
--rw-r--r--   0        0        0    15177 2023-07-24 11:42:00.967762 ramqp-9.0.1/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0     7466 2023-07-24 11:42:00.968762 ramqp-9.0.1/README.md
--rw-r--r--   0        0        0     1465 2023-07-24 11:42:15.479999 ramqp-9.0.1/pyproject.toml
--rw-r--r--   0        0        0      321 2023-07-24 11:42:00.969762 ramqp-9.0.1/ramqp/__init__.py
--rw-r--r--   0        0        0    16371 2023-07-24 11:42:00.969762 ramqp-9.0.1/ramqp/abstract.py
--rw-r--r--   0        0        0      668 2023-07-24 11:42:00.969762 ramqp-9.0.1/ramqp/amqp.py
--rw-r--r--   0        0        0     2729 2023-07-24 11:42:00.970763 ramqp-9.0.1/ramqp/config.py
--rw-r--r--   0        0        0    10056 2023-07-24 11:42:00.970763 ramqp-9.0.1/ramqp/depends.py
--rw-r--r--   0        0        0     7010 2023-07-24 11:42:00.970763 ramqp-9.0.1/ramqp/metrics.py
--rw-r--r--   0        0        0     8652 2023-07-24 11:42:00.970763 ramqp-9.0.1/ramqp/mo.py
--rw-r--r--   0        0        0        0 2023-07-24 11:42:01.103774 ramqp-9.0.1/ramqp/py.typed
--rw-r--r--   0        0        0     1367 2023-07-24 11:42:00.970763 ramqp-9.0.1/ramqp/utils.py
--rw-r--r--   0        0        0     8357 1970-01-01 00:00:00.000000 ramqp-9.0.1/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-07-27 15:18:00.993518 ramqp-9.0.2/LICENSES/
+-rw-r--r--   0        0        0    15177 2023-07-27 15:18:00.993518 ramqp-9.0.2/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0     7466 2023-07-27 15:18:00.994518 ramqp-9.0.2/README.md
+-rw-r--r--   0        0        0     1465 2023-07-27 15:18:14.845792 ramqp-9.0.2/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-07-27 15:18:00.995518 ramqp-9.0.2/ramqp/__init__.py
+-rw-r--r--   0        0        0    16464 2023-07-27 15:18:00.995518 ramqp-9.0.2/ramqp/abstract.py
+-rw-r--r--   0        0        0      668 2023-07-27 15:18:00.995518 ramqp-9.0.2/ramqp/amqp.py
+-rw-r--r--   0        0        0     2729 2023-07-27 15:18:00.996518 ramqp-9.0.2/ramqp/config.py
+-rw-r--r--   0        0        0    10056 2023-07-27 15:18:00.996518 ramqp-9.0.2/ramqp/depends.py
+-rw-r--r--   0        0        0     7010 2023-07-27 15:18:00.996518 ramqp-9.0.2/ramqp/metrics.py
+-rw-r--r--   0        0        0     8652 2023-07-27 15:18:00.996518 ramqp-9.0.2/ramqp/mo.py
+-rw-r--r--   0        0        0        0 2023-07-27 15:18:01.046522 ramqp-9.0.2/ramqp/py.typed
+-rw-r--r--   0        0        0     1367 2023-07-27 15:18:00.997518 ramqp-9.0.2/ramqp/utils.py
+-rw-r--r--   0        0        0     8357 1970-01-01 00:00:00.000000 ramqp-9.0.2/PKG-INFO
```

### Comparing `ramqp-9.0.1/LICENSES/MPL-2.0.txt` & `ramqp-9.0.2/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `ramqp-9.0.1/README.md` & `ramqp-9.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ramqp-9.0.1/pyproject.toml` & `ramqp-9.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ramqp"
-version = "9.0.1"
+version = "9.0.2"
 description = "Rammearkitektur AMQP library (aio_pika wrapper)"
 authors = ["Magenta ApS <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/ramqp"
 keywords = ["os2mo", "amqp"]
```

### Comparing `ramqp-9.0.1/ramqp/abstract.py` & `ramqp-9.0.2/ramqp/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from aio_pika import IncomingMessage
 from aio_pika import Message
 from aio_pika.abc import AbstractExchange
 from aio_pika.abc import AbstractQueue
 from aio_pika.abc import AbstractRobustChannel
 from aio_pika.abc import AbstractRobustConnection
 from aiormq import ChannelPreconditionFailed
+from fastapi.encoders import jsonable_encoder
 from more_itertools import all_unique
 from more_itertools import one
 
 from .config import AMQPConnectionSettings
 from .depends import dependency_injected
 from .metrics import _handle_publish_metrics
 from .metrics import _handle_receive_metrics
@@ -117,15 +118,15 @@
     """Abstract base-class for Publish Mixins.
 
     Shared code used by both PublishMixin and MOPublishMixin.
     """
 
     _exchange: AbstractExchange | None
 
-    async def _publish_message(self, routing_key: Any, payload: dict) -> None:
+    async def _publish_message(self, routing_key: Any, payload: Any) -> None:
         """Publish a message to the given routing key.
 
         Args:
             routing_key: The routing key to send the message to.
             payload: The message payload.
 
         Raises:
@@ -133,15 +134,17 @@
         """
         if self._exchange is None:
             raise ValueError("Must call start() before publish message!")
 
         # Allow using any custom object as routing key as long as it implements __str__
         routing_key = str(routing_key)
         with _handle_publish_metrics(routing_key):
-            message = Message(body=json.dumps(payload).encode("utf-8"))
+            message = Message(
+                body=json.dumps(jsonable_encoder(payload)).encode("utf-8")
+            )
             await self._exchange.publish(routing_key=routing_key, message=message)
 
 
 # pylint: disable=invalid-name
 TRouter = TypeVar("TRouter", bound=AbstractRouter)
 # Workaround until Self Types in Python 3.11 (PEP673)
 # pylint: disable=invalid-name
```

### Comparing `ramqp-9.0.1/ramqp/amqp.py` & `ramqp-9.0.2/ramqp/amqp.py`

 * *Files identical despite different names*

### Comparing `ramqp-9.0.1/ramqp/config.py` & `ramqp-9.0.2/ramqp/config.py`

 * *Files identical despite different names*

### Comparing `ramqp-9.0.1/ramqp/depends.py` & `ramqp-9.0.2/ramqp/depends.py`

 * *Files identical despite different names*

### Comparing `ramqp-9.0.1/ramqp/metrics.py` & `ramqp-9.0.2/ramqp/metrics.py`

 * *Files identical despite different names*

### Comparing `ramqp-9.0.1/ramqp/mo.py` & `ramqp-9.0.2/ramqp/mo.py`

 * *Files identical despite different names*

### Comparing `ramqp-9.0.1/ramqp/utils.py` & `ramqp-9.0.2/ramqp/utils.py`

 * *Files identical despite different names*

### Comparing `ramqp-9.0.1/PKG-INFO` & `ramqp-9.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramqp
-Version: 9.0.1
+Version: 9.0.2
 Summary: Rammearkitektur AMQP library (aio_pika wrapper)
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo,amqp
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.10,<4.0
```

