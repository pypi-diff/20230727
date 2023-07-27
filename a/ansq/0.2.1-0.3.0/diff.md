# Comparing `tmp/ansq-0.2.1.tar.gz` & `tmp/ansq-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansq-0.2.1.tar", last modified: Tue May 30 13:26:05 2023, max compression
+gzip compressed data, was "ansq-0.3.0.tar", last modified: Thu Jul 27 18:05:48 2023, max compression
```

## Comparing `ansq-0.2.1.tar` & `ansq-0.3.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 os         (501) staff       (20)        0 2023-05-30 13:26:05.032036 ansq-0.2.1/
--rw-r--r--   0 os         (501) staff       (20)     1133 2022-05-31 08:29:33.000000 ansq-0.2.1/LICENSE
--rw-r--r--   0 os         (501) staff       (20)     2960 2023-05-30 13:26:05.032122 ansq-0.2.1/PKG-INFO
--rw-r--r--   0 os         (501) staff       (20)     2198 2023-01-24 15:58:25.000000 ansq-0.2.1/README.md
-drwxr-xr-x   0 os         (501) staff       (20)        0 2023-05-30 13:26:05.026155 ansq-0.2.1/ansq/
--rw-r--r--   0 os         (501) staff       (20)      313 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/__init__.py
-drwxr-xr-x   0 os         (501) staff       (20)        0 2023-05-30 13:26:05.027793 ansq-0.2.1/ansq/http/
--rw-r--r--   0 os         (501) staff       (20)      111 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/http/__init__.py
--rw-r--r--   0 os         (501) staff       (20)     2241 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/http/base.py
--rw-r--r--   0 os         (501) staff       (20)     1210 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/http/http_exceptions.py
--rw-r--r--   0 os         (501) staff       (20)     2916 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/http/lookupd.py
--rw-r--r--   0 os         (501) staff       (20)     4386 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/http/writer.py
--rw-r--r--   0 os         (501) staff       (20)        0 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/py.typed
-drwxr-xr-x   0 os         (501) staff       (20)        0 2023-05-30 13:26:05.029019 ansq-0.2.1/ansq/tcp/
--rw-r--r--   0 os         (501) staff       (20)        0 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/tcp/__init__.py
--rw-r--r--   0 os         (501) staff       (20)    21127 2023-01-24 15:58:25.000000 ansq-0.2.1/ansq/tcp/connection.py
--rw-r--r--   0 os         (501) staff       (20)      245 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/tcp/consts.py
--rw-r--r--   0 os         (501) staff       (20)     2271 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/tcp/exceptions.py
--rw-r--r--   0 os         (501) staff       (20)     5483 2023-01-24 15:58:25.000000 ansq-0.2.1/ansq/tcp/protocol.py
--rw-r--r--   0 os         (501) staff       (20)    11956 2023-01-24 15:58:25.000000 ansq-0.2.1/ansq/tcp/reader.py
-drwxr-xr-x   0 os         (501) staff       (20)        0 2023-05-30 13:26:05.030419 ansq-0.2.1/ansq/tcp/types/
--rw-r--r--   0 os         (501) staff       (20)      584 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/tcp/types/__init__.py
--rw-r--r--   0 os         (501) staff       (20)     2388 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/tcp/types/client.py
--rw-r--r--   0 os         (501) staff       (20)      332 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/tcp/types/commands.py
--rw-r--r--   0 os         (501) staff       (20)     9900 2023-01-24 15:58:25.000000 ansq-0.2.1/ansq/tcp/types/connection.py
--rw-r--r--   0 os         (501) staff       (20)      862 2023-05-30 13:05:57.000000 ansq-0.2.1/ansq/tcp/types/connection_status.py
--rw-r--r--   0 os         (501) staff       (20)      362 2023-05-30 13:05:57.000000 ansq-0.2.1/ansq/tcp/types/frame_type.py
--rw-r--r--   0 os         (501) staff       (20)     4241 2023-01-24 15:58:25.000000 ansq-0.2.1/ansq/tcp/types/message.py
--rw-r--r--   0 os         (501) staff       (20)     2486 2023-01-24 15:58:25.000000 ansq-0.2.1/ansq/tcp/types/response_schemas.py
--rw-r--r--   0 os         (501) staff       (20)     2181 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/tcp/writer.py
--rw-r--r--   0 os         (501) staff       (20)      281 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/typedefs.py
--rw-r--r--   0 os         (501) staff       (20)     5386 2023-01-24 15:58:25.000000 ansq-0.2.1/ansq/utils.py
-drwxr-xr-x   0 os         (501) staff       (20)        0 2023-05-30 13:26:05.027013 ansq-0.2.1/ansq.egg-info/
--rw-r--r--   0 os         (501) staff       (20)     2960 2023-05-30 13:26:05.000000 ansq-0.2.1/ansq.egg-info/PKG-INFO
--rw-r--r--   0 os         (501) staff       (20)      999 2023-05-30 13:26:05.000000 ansq-0.2.1/ansq.egg-info/SOURCES.txt
--rw-r--r--   0 os         (501) staff       (20)        1 2023-05-30 13:26:05.000000 ansq-0.2.1/ansq.egg-info/dependency_links.txt
--rw-r--r--   0 os         (501) staff       (20)      129 2023-05-30 13:26:05.000000 ansq-0.2.1/ansq.egg-info/requires.txt
--rw-r--r--   0 os         (501) staff       (20)        5 2023-05-30 13:26:05.000000 ansq-0.2.1/ansq.egg-info/top_level.txt
--rw-r--r--   0 os         (501) staff       (20)     1508 2023-05-30 13:26:05.032544 ansq-0.2.1/setup.cfg
--rw-r--r--   0 os         (501) staff       (20)       38 2022-05-31 08:29:33.000000 ansq-0.2.1/setup.py
-drwxr-xr-x   0 os         (501) staff       (20)        0 2023-05-30 13:26:05.031912 ansq-0.2.1/tests/
--rw-r--r--   0 os         (501) staff       (20)     3118 2023-01-24 15:58:25.000000 ansq-0.2.1/tests/test_connection.py
--rw-r--r--   0 os         (501) staff       (20)     3447 2022-05-31 08:29:33.000000 ansq-0.2.1/tests/test_convert_to_bytes.py
--rw-r--r--   0 os         (501) staff       (20)     2362 2023-01-24 15:58:25.000000 ansq-0.2.1/tests/test_http_writer.py
--rw-r--r--   0 os         (501) staff       (20)     7287 2023-01-24 15:58:25.000000 ansq-0.2.1/tests/test_read_messages.py
--rw-r--r--   0 os         (501) staff       (20)     2712 2023-01-24 15:58:25.000000 ansq-0.2.1/tests/test_reader.py
--rw-r--r--   0 os         (501) staff       (20)     3118 2023-01-24 15:58:25.000000 ansq-0.2.1/tests/test_reader_lookupd.py
--rw-r--r--   0 os         (501) staff       (20)     2728 2023-01-24 15:58:25.000000 ansq-0.2.1/tests/test_send_commands.py
--rw-r--r--   0 os         (501) staff       (20)      930 2023-01-24 15:58:25.000000 ansq-0.2.1/tests/test_utils.py
--rw-r--r--   0 os         (501) staff       (20)      893 2022-05-31 08:29:33.000000 ansq-0.2.1/tests/test_validation_topic_channel_name.py
--rw-r--r--   0 os         (501) staff       (20)     2110 2023-01-24 15:58:25.000000 ansq-0.2.1/tests/test_writer.py
+drwxr-xr-x   0 os         (501) staff       (20)        0 2023-07-27 18:05:48.406398 ansq-0.3.0/
+-rw-r--r--   0 os         (501) staff       (20)     1133 2023-07-27 17:54:42.000000 ansq-0.3.0/LICENSE
+-rw-r--r--   0 os         (501) staff       (20)     2960 2023-07-27 18:05:48.406483 ansq-0.3.0/PKG-INFO
+-rw-r--r--   0 os         (501) staff       (20)     2198 2023-07-27 17:54:42.000000 ansq-0.3.0/README.md
+drwxr-xr-x   0 os         (501) staff       (20)        0 2023-07-27 18:05:48.397430 ansq-0.3.0/ansq/
+-rw-r--r--   0 os         (501) staff       (20)      313 2023-07-27 17:54:42.000000 ansq-0.3.0/ansq/__init__.py
+drwxr-xr-x   0 os         (501) staff       (20)        0 2023-07-27 18:05:48.401498 ansq-0.3.0/ansq/http/
+-rw-r--r--   0 os         (501) staff       (20)      111 2023-07-27 17:54:42.000000 ansq-0.3.0/ansq/http/__init__.py
+-rw-r--r--   0 os         (501) staff       (20)     2241 2023-07-27 17:54:42.000000 ansq-0.3.0/ansq/http/base.py
+-rw-r--r--   0 os         (501) staff       (20)     1210 2023-07-27 17:54:42.000000 ansq-0.3.0/ansq/http/http_exceptions.py
+-rw-r--r--   0 os         (501) staff       (20)     2916 2023-07-27 17:54:42.000000 ansq-0.3.0/ansq/http/lookupd.py
+-rw-r--r--   0 os         (501) staff       (20)     4386 2023-07-27 17:54:42.000000 ansq-0.3.0/ansq/http/writer.py
+-rw-r--r--   0 os         (501) staff       (20)        0 2023-07-27 17:54:42.000000 ansq-0.3.0/ansq/py.typed
+drwxr-xr-x   0 os         (501) staff       (20)        0 2023-07-27 18:05:48.402820 ansq-0.3.0/ansq/tcp/
+-rw-r--r--   0 os         (501) staff       (20)        0 2023-07-27 17:54:42.000000 ansq-0.3.0/ansq/tcp/__init__.py
+-rw-r--r--   0 os         (501) staff       (20)    21200 2023-07-27 17:54:42.000000 ansq-0.3.0/ansq/tcp/connection.py
+-rw-r--r--   0 os         (501) staff       (20)      245 2023-07-27 17:54:42.000000 ansq-0.3.0/ansq/tcp/consts.py
+-rw-r--r--   0 os         (501) staff       (20)     2271 2023-07-27 17:54:42.000000 ansq-0.3.0/ansq/tcp/exceptions.py
+-rw-r--r--   0 os         (501) staff       (20)     5483 2023-07-27 17:54:42.000000 ansq-0.3.0/ansq/tcp/protocol.py
+-rw-r--r--   0 os         (501) staff       (20)    11971 2023-07-27 17:54:42.000000 ansq-0.3.0/ansq/tcp/reader.py
+drwxr-xr-x   0 os         (501) staff       (20)        0 2023-07-27 18:05:48.404704 ansq-0.3.0/ansq/tcp/types/
+-rw-r--r--   0 os         (501) staff       (20)      584 2023-07-27 17:54:42.000000 ansq-0.3.0/ansq/tcp/types/__init__.py
+-rw-r--r--   0 os         (501) staff       (20)     2433 2023-07-27 17:54:42.000000 ansq-0.3.0/ansq/tcp/types/client.py
+-rw-r--r--   0 os         (501) staff       (20)      332 2023-07-27 17:54:42.000000 ansq-0.3.0/ansq/tcp/types/commands.py
+-rw-r--r--   0 os         (501) staff       (20)     9795 2023-07-27 17:54:42.000000 ansq-0.3.0/ansq/tcp/types/connection.py
+-rw-r--r--   0 os         (501) staff       (20)      862 2023-07-27 17:54:42.000000 ansq-0.3.0/ansq/tcp/types/connection_status.py
+-rw-r--r--   0 os         (501) staff       (20)      362 2023-07-27 17:54:42.000000 ansq-0.3.0/ansq/tcp/types/frame_type.py
+-rw-r--r--   0 os         (501) staff       (20)     4241 2023-07-27 17:54:42.000000 ansq-0.3.0/ansq/tcp/types/message.py
+-rw-r--r--   0 os         (501) staff       (20)     2486 2023-07-27 17:54:42.000000 ansq-0.3.0/ansq/tcp/types/response_schemas.py
+-rw-r--r--   0 os         (501) staff       (20)     2181 2023-07-27 17:54:42.000000 ansq-0.3.0/ansq/tcp/writer.py
+-rw-r--r--   0 os         (501) staff       (20)      281 2023-07-27 17:54:42.000000 ansq-0.3.0/ansq/typedefs.py
+-rw-r--r--   0 os         (501) staff       (20)     5224 2023-07-27 17:54:42.000000 ansq-0.3.0/ansq/utils.py
+drwxr-xr-x   0 os         (501) staff       (20)        0 2023-07-27 18:05:48.398187 ansq-0.3.0/ansq.egg-info/
+-rw-r--r--   0 os         (501) staff       (20)     2960 2023-07-27 18:05:48.000000 ansq-0.3.0/ansq.egg-info/PKG-INFO
+-rw-r--r--   0 os         (501) staff       (20)      999 2023-07-27 18:05:48.000000 ansq-0.3.0/ansq.egg-info/SOURCES.txt
+-rw-r--r--   0 os         (501) staff       (20)        1 2023-07-27 18:05:48.000000 ansq-0.3.0/ansq.egg-info/dependency_links.txt
+-rw-r--r--   0 os         (501) staff       (20)       83 2023-07-27 18:05:48.000000 ansq-0.3.0/ansq.egg-info/requires.txt
+-rw-r--r--   0 os         (501) staff       (20)        5 2023-07-27 18:05:48.000000 ansq-0.3.0/ansq.egg-info/top_level.txt
+-rw-r--r--   0 os         (501) staff       (20)     1468 2023-07-27 18:05:48.406887 ansq-0.3.0/setup.cfg
+-rw-r--r--   0 os         (501) staff       (20)       38 2023-07-27 17:54:42.000000 ansq-0.3.0/setup.py
+drwxr-xr-x   0 os         (501) staff       (20)        0 2023-07-27 18:05:48.406276 ansq-0.3.0/tests/
+-rw-r--r--   0 os         (501) staff       (20)     3118 2023-07-27 17:54:42.000000 ansq-0.3.0/tests/test_connection.py
+-rw-r--r--   0 os         (501) staff       (20)     3215 2023-07-27 17:54:42.000000 ansq-0.3.0/tests/test_convert_to_bytes.py
+-rw-r--r--   0 os         (501) staff       (20)     2362 2023-07-27 17:54:42.000000 ansq-0.3.0/tests/test_http_writer.py
+-rw-r--r--   0 os         (501) staff       (20)     7287 2023-07-27 17:54:42.000000 ansq-0.3.0/tests/test_read_messages.py
+-rw-r--r--   0 os         (501) staff       (20)     2712 2023-07-27 17:54:42.000000 ansq-0.3.0/tests/test_reader.py
+-rw-r--r--   0 os         (501) staff       (20)     3118 2023-07-27 17:54:42.000000 ansq-0.3.0/tests/test_reader_lookupd.py
+-rw-r--r--   0 os         (501) staff       (20)     2728 2023-07-27 17:54:42.000000 ansq-0.3.0/tests/test_send_commands.py
+-rw-r--r--   0 os         (501) staff       (20)      930 2023-07-27 17:54:42.000000 ansq-0.3.0/tests/test_utils.py
+-rw-r--r--   0 os         (501) staff       (20)      893 2023-07-27 17:54:42.000000 ansq-0.3.0/tests/test_validation_topic_channel_name.py
+-rw-r--r--   0 os         (501) staff       (20)     2110 2023-07-27 17:54:42.000000 ansq-0.3.0/tests/test_writer.py
```

### Comparing `ansq-0.2.1/LICENSE` & `ansq-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansq-0.2.1/PKG-INFO` & `ansq-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ansq
-Version: 0.2.1
+Version: 0.3.0
 Summary: Written with native Asyncio NSQ package
 Home-page: https://github.com/list-family/ansq
 Author: LiST
 Author-email: info@list.family
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: coverage
 Provides-Extra: testing
 License-File: LICENSE
 
 # ansq - Async NSQ
 [![PyPI version](https://badge.fury.io/py/ansq.svg)](https://badge.fury.io/py/ansq)
```

### Comparing `ansq-0.2.1/README.md` & `ansq-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ansq-0.2.1/ansq/http/base.py` & `ansq-0.3.0/ansq/http/base.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.1/ansq/http/http_exceptions.py` & `ansq-0.3.0/ansq/http/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.1/ansq/http/lookupd.py` & `ansq-0.3.0/ansq/http/lookupd.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.1/ansq/http/writer.py` & `ansq-0.3.0/ansq/http/writer.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.1/ansq/tcp/connection.py` & `ansq-0.3.0/ansq/tcp/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,36 +358,41 @@
     def _upgrade_to_deflate(self) -> asyncio.Future:
         raise NotImplementedError("Upgrade to deflate not implemented yet")
 
     async def _read_data_task(self) -> None:
         """Response reader task."""
         assert self._reader is not None
 
+        error: Optional[Exception] = None
+
         while not self._reader.at_eof():
             try:
                 data = await self._reader.read(consts.MAX_CHUNK_SIZE)
+
+                self._parser.feed(data)
+
+                if not self._is_upgrading:
+                    await self._read_buffer()
+
             except asyncio.CancelledError:
                 # useful during update to TLS, task canceled but connection
                 # should not be closed
                 return
-            except Exception as exc:
-                await self._do_close(exc)
-                return
-
-            self._parser.feed(data)
+            except Exception as e:
+                error = e
 
-            if not self._is_upgrading:
-                await self._read_buffer()
+        self.logger.info(
+            "Lost connection to NSQ %s due an error: %s", self.endpoint, error
+        )
 
-        self.logger.info("Lost connection to NSQ %s", self.endpoint)
         if self._auto_reconnect:
             await asyncio.sleep(1)
             self._reconnect_task = self._loop.create_task(self._do_auto_reconnect())
         else:
-            await self._do_close()
+            await self._do_close(error=error)
 
     async def _parse_data(self) -> bool:
         try:
             response = self._parser.get()
         except ProtocolError as exc:
             # ProtocolError is fatal
             await self._do_close(exc)
```

### Comparing `ansq-0.2.1/ansq/tcp/exceptions.py` & `ansq-0.3.0/ansq/tcp/exceptions.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.1/ansq/tcp/protocol.py` & `ansq-0.3.0/ansq/tcp/protocol.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.1/ansq/tcp/reader.py` & `ansq-0.3.0/ansq/tcp/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from ansq.http import NsqLookupd
 from ansq.tcp.types import Client, ConnectionOptions
 from ansq.utils import get_logger
 
 if TYPE_CHECKING:
     from ansq.tcp.connection import NSQConnection
-    from ansq.tcp.types import NSQMessage
+    from ansq.tcp.types import NSQMessage, TCPConnection
 
 
 class Reader(Client):
     """A consumer that provides an interface for reading messages from nsqd."""
 
     def __init__(
         self,
@@ -298,15 +298,15 @@
 
             host = producer["broadcast_address"]
             port = int(producer["tcp_port"])
             addresses.append(Address(host, port))
 
         return addresses
 
-    def _on_close_connection(self, connection: "NSQConnection") -> None:
+    def _on_close_connection(self, connection: "TCPConnection") -> None:
         """A callback to be called after a connection being closed."""
         # Remove the connection from the reader so that lookupd could add it later
         self._reader.remove_connection(connection)
 
         # Call an original on_close callback if specified
         if self._orig_on_close_callback is not None:
             self._orig_on_close_callback(connection)
```

### Comparing `ansq-0.2.1/ansq/tcp/types/__init__.py` & `ansq-0.3.0/ansq/tcp/types/__init__.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.1/ansq/tcp/types/client.py` & `ansq-0.3.0/ansq/tcp/types/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import attr
 
 from .connection import ConnectionOptions
 
 if TYPE_CHECKING:
     from ansq.tcp.connection import NSQConnection
+    from ansq.tcp.types import TCPConnection
 
 
 class Client:
     """Base class for reader and writer."""
 
     def __init__(
         self,
@@ -58,15 +59,15 @@
         self.add_connection(connection)
         return connection
 
     def add_connection(self, connection: "NSQConnection") -> None:
         """Add connection to connections pool."""
         self._connections[connection.id] = connection
 
-    def remove_connection(self, connection: "NSQConnection") -> None:
+    def remove_connection(self, connection: "TCPConnection") -> None:
         """Remove connection from connections pool."""
         if connection.id in self._connections:
             del self._connections[connection.id]
 
     @property
     def connections(self) -> Tuple["NSQConnection", ...]:
         """Return a tuple of all instantiated connections."""
```

### Comparing `ansq-0.2.1/ansq/tcp/types/connection.py` & `ansq-0.3.0/ansq/tcp/types/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import abc
 import asyncio
 import functools
 import logging
 import socket
-import sys
 import warnings
 from asyncio.events import AbstractEventLoop
 from asyncio.streams import StreamReader, StreamWriter
 from collections import deque
 from datetime import datetime
 from typing import (
     TYPE_CHECKING,
@@ -28,18 +27,16 @@
 
 if TYPE_CHECKING:
     from ansq.tcp.types import ConnectionStatus, NSQMessage, NSQMessageSchema
 
 
 @functools.lru_cache(maxsize=None)
 def _get_version() -> str:
-    if sys.version_info >= (3, 8):
-        from importlib import metadata
-    else:
-        import importlib_metadata as metadata
+    from importlib import metadata
+
     return metadata.version("ansq")
 
 
 def _get_hostname() -> str:
     return socket.gethostname()
```

### Comparing `ansq-0.2.1/ansq/tcp/types/connection_status.py` & `ansq-0.3.0/ansq/tcp/types/connection_status.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.1/ansq/tcp/types/message.py` & `ansq-0.3.0/ansq/tcp/types/message.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.1/ansq/tcp/types/response_schemas.py` & `ansq-0.3.0/ansq/tcp/types/response_schemas.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.1/ansq/tcp/writer.py` & `ansq-0.3.0/ansq/tcp/writer.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.1/ansq/utils.py` & `ansq-0.3.0/ansq/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import json
 import logging
 import re
+from dataclasses import asdict, is_dataclass
 from datetime import datetime
 from decimal import Decimal
 from enum import Enum
 from functools import singledispatch
-from sys import version_info
 from typing import Any, Optional, Tuple, Union
 from urllib.parse import urlsplit
 
-PY37 = version_info >= (3, 7)
-
 
 class JSONEncoder(json.JSONEncoder):
     def default(self, obj: Any) -> str:
         try:
             return convert_to_str(obj)
         except TypeError:
             return json.JSONEncoder.default(self, obj)
@@ -42,19 +40,18 @@
     """Dispatch for convertible types.
 
     Allowed types: ``bytes``, ``bytearray``, ``str``, ``int``, ``float``,
         ``dict``, ``Decimal``, ``dataclass``.
 
     :raises TypeError:
     """
-    if PY37:
-        from dataclasses import asdict, is_dataclass
 
-        if is_dataclass(value) and not isinstance(value, type):
-            return convert_to_bytes(asdict(value))
+    if is_dataclass(value) and not isinstance(value, type):
+        return convert_to_bytes(asdict(value))
+
     raise TypeError(
         "Argument {} expected to be type of "
         "bytes, bytearray, str, int, float, dict, Decimal, datetime "
         "or dataclass".format(value),
     )
 
 
@@ -102,19 +99,17 @@
     """Dispatch for convertible types.
 
     Allowed types: ``bytes``, ``bytearray``, ``str``, ``int``, ``float``,
         ``dict``, ``Decimal``, ``dataclass``.
 
     :raises TypeError:
     """
-    if PY37:
-        from dataclasses import asdict, is_dataclass
+    if is_dataclass(value) and not isinstance(value, type):
+        return convert_to_str(asdict(value))
 
-        if is_dataclass(value) and not isinstance(value, type):
-            return convert_to_str(asdict(value))
     raise TypeError(
         "Argument {} expected to be type of "
         "bytes, bytearray, str, int, float, dict, Decimal, datetime "
         "or dataclass".format(value),
     )
```

### Comparing `ansq-0.2.1/ansq.egg-info/PKG-INFO` & `ansq-0.3.0/ansq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ansq
-Version: 0.2.1
+Version: 0.3.0
 Summary: Written with native Asyncio NSQ package
 Home-page: https://github.com/list-family/ansq
 Author: LiST
 Author-email: info@list.family
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: coverage
 Provides-Extra: testing
 License-File: LICENSE
 
 # ansq - Async NSQ
 [![PyPI version](https://badge.fury.io/py/ansq.svg)](https://badge.fury.io/py/ansq)
```

### Comparing `ansq-0.2.1/ansq.egg-info/SOURCES.txt` & `ansq-0.3.0/ansq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansq-0.2.1/setup.cfg` & `ansq-0.3.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = ansq
-version = 0.2.1
+version = 0.3.0
 description = Written with native Asyncio NSQ package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/list-family/ansq
 author = LiST
 author_email = info@list.family
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Development Status :: 3 - Alpha
 	Environment :: Web Environment
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python
 	Programming Language :: Python :: 3
@@ -21,16 +21,15 @@
 	Topic :: Software Development :: Libraries
 
 [options]
 packages = find:
 install_requires = 
 	aiohttp>=1.0.0
 	attrs>=20.1
-	importlib-metadata;python_version<"3.8"
-python_requires = >=3.7
+python_requires = >=3.8
 include_package_data = True
 
 [options.packages.find]
 exclude = tests
 
 [options.extras_require]
 coverage =
```

### Comparing `ansq-0.2.1/tests/test_connection.py` & `ansq-0.3.0/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.1/tests/test_convert_to_bytes.py` & `ansq-0.3.0/tests/test_convert_to_bytes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
+from dataclasses import dataclass
 from datetime import datetime
 from decimal import Decimal
 from enum import Enum
-from sys import version_info
 from typing import Optional
 
 import pytest
 
 from ansq.utils import convert_to_bytes
 
-PY37 = version_info >= (3, 7)
-
 
 class Color(Enum):
     RED = 1
     GREEN = "GREEN"
     BLUE = {"real_blue_color": True}
 
 
@@ -59,58 +57,57 @@
         (Color.BLUE, b"BLUE"),
     ),
 )
 def test_convert_to_bytes(value, expected):
     assert convert_to_bytes(value) == expected
 
 
-if PY37:
-    from dataclasses import dataclass
+@dataclass
+class Point:
+    x: int
+    y: int
+    color: Color = Color.BLUE
+    name: Optional[str] = None
 
-    @dataclass
-    class Point:
-        x: int
-        y: int
-        color: Color = Color.BLUE
-        name: Optional[str] = None
-
-    @dataclass
-    class DataclassWithDictPayload:
-        name: str
-        payload: dict
-
-    @pytest.mark.parametrize(
-        "value, expected",
-        (
-            (Point(10, 20), b'{"x":10,"y":20,"color":"BLUE","name":null}'),
-            (
-                Point(10, 20, Color.RED, "A point"),
-                b'{"x":10,"y":20,"color":"RED","name":"A point"}',
-            ),
-            (
-                DataclassWithDictPayload(
-                    "Some str here",
-                    {
-                        "int": 123,
-                        "float": 123.123,
-                        "str": "str",
-                        "list": [1, 2, 3],
-                        "dict": {"a": 1, "b": 2},
-                        "color": Color.GREEN,
-                        "dataclass": Point(10, 20),
-                    },
-                ),
-                b'{"name":"Some str here","payload":{"int":123,'
-                b'"float":123.123,"str":"str","list":[1,2,3],'
-                b'"dict":{"a":1,"b":2},"color":"GREEN","dataclass":'
-                b'{"x":10,"y":20,"color":"BLUE","name":null}}}',
+
+@dataclass
+class DataclassWithDictPayload:
+    name: str
+    payload: dict
+
+
+@pytest.mark.parametrize(
+    "value, expected",
+    (
+        (Point(10, 20), b'{"x":10,"y":20,"color":"BLUE","name":null}'),
+        (
+            Point(10, 20, Color.RED, "A point"),
+            b'{"x":10,"y":20,"color":"RED","name":"A point"}',
+        ),
+        (
+            DataclassWithDictPayload(
+                "Some str here",
+                {
+                    "int": 123,
+                    "float": 123.123,
+                    "str": "str",
+                    "list": [1, 2, 3],
+                    "dict": {"a": 1, "b": 2},
+                    "color": Color.GREEN,
+                    "dataclass": Point(10, 20),
+                },
             ),
+            b'{"name":"Some str here","payload":{"int":123,'
+            b'"float":123.123,"str":"str","list":[1,2,3],'
+            b'"dict":{"a":1,"b":2},"color":"GREEN","dataclass":'
+            b'{"x":10,"y":20,"color":"BLUE","name":null}}}',
         ),
-    )
-    def test_convert_dataclass_to_bytes(value, expected):
-        assert convert_to_bytes(value) == expected
+    ),
+)
+def test_convert_dataclass_to_bytes(value, expected):
+    assert convert_to_bytes(value) == expected
 
 
 @pytest.mark.parametrize("value", (None, [1, 2, 3], (1, 2), ["str_in_list"]))
 def test_convert_to_bytes_with_exception(value):
     with pytest.raises(TypeError):
         convert_to_bytes(value)
```

### Comparing `ansq-0.2.1/tests/test_http_writer.py` & `ansq-0.3.0/tests/test_http_writer.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.1/tests/test_read_messages.py` & `ansq-0.3.0/tests/test_read_messages.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.1/tests/test_reader.py` & `ansq-0.3.0/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.1/tests/test_reader_lookupd.py` & `ansq-0.3.0/tests/test_reader_lookupd.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.1/tests/test_send_commands.py` & `ansq-0.3.0/tests/test_send_commands.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.1/tests/test_utils.py` & `ansq-0.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.1/tests/test_validation_topic_channel_name.py` & `ansq-0.3.0/tests/test_validation_topic_channel_name.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.1/tests/test_writer.py` & `ansq-0.3.0/tests/test_writer.py`

 * *Files identical despite different names*

