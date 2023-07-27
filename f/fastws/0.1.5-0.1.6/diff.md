# Comparing `tmp/fastws-0.1.5.tar.gz` & `tmp/fastws-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastws-0.1.5.tar", max compression
+gzip compressed data, was "fastws-0.1.6.tar", max compression
```

## Comparing `fastws-0.1.5.tar` & `fastws-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1077 2023-07-06 20:53:23.287732 fastws-0.1.5/LICENSE
--rw-r--r--   0        0        0    10320 2023-07-06 22:45:54.596534 fastws-0.1.5/README.md
--rw-r--r--   0        0        0      437 2023-07-07 21:07:37.952253 fastws-0.1.5/fastws/__init__.py
--rw-r--r--   0        0        0     6890 2023-07-07 20:54:44.192393 fastws-0.1.5/fastws/application.py
--rw-r--r--   0        0        0     1643 2023-07-07 20:52:02.052422 fastws-0.1.5/fastws/asyncapi.py
--rw-r--r--   0        0        0     4505 2023-07-07 21:04:00.652291 fastws-0.1.5/fastws/broker.py
--rw-r--r--   0        0        0     6404 2023-07-07 20:54:39.992394 fastws-0.1.5/fastws/docs.py
--rw-r--r--   0        0        0     7065 2023-07-07 21:01:59.772314 fastws-0.1.5/fastws/routing.py
--rw-r--r--   0        0        0     1225 2023-07-07 21:07:37.822253 fastws-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    11432 1970-01-01 00:00:00.000000 fastws-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-06 20:53:23.287732 fastws-0.1.6/LICENSE
+-rw-r--r--   0        0        0    10497 2023-07-27 10:53:34.903557 fastws-0.1.6/README.md
+-rw-r--r--   0        0        0      437 2023-07-27 11:14:57.453092 fastws-0.1.6/fastws/__init__.py
+-rw-r--r--   0        0        0     6890 2023-07-27 10:32:07.574023 fastws-0.1.6/fastws/application.py
+-rw-r--r--   0        0        0     1643 2023-07-07 20:52:02.052422 fastws-0.1.6/fastws/asyncapi.py
+-rw-r--r--   0        0        0     4505 2023-07-07 21:04:00.652291 fastws-0.1.6/fastws/broker.py
+-rw-r--r--   0        0        0     6404 2023-07-07 20:54:39.992394 fastws-0.1.6/fastws/docs.py
+-rw-r--r--   0        0        0     7148 2023-07-27 11:13:29.813122 fastws-0.1.6/fastws/routing.py
+-rw-r--r--   0        0        0     1261 2023-07-27 11:14:57.363093 fastws-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    11609 1970-01-01 00:00:00.000000 fastws-0.1.6/PKG-INFO
```

### Comparing `fastws-0.1.5/LICENSE` & `fastws-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fastws-0.1.5/README.md` & `fastws-0.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -57,17 +57,17 @@
 
 from fastapi import Depends, FastAPI
 from fastws import Client, FastWS
 
 service = FastWS()
 
 
-@service.send("ping")
-async def send_event_a() -> str:
-    return "pong"
+@service.send("ping", reply="ping")
+async def send_event_a():
+    return
 
 
 @asynccontextmanager
 async def lifespan(app: FastAPI):
     service.setup(app)
     yield
 
@@ -104,30 +104,30 @@
 #### Define event
 
 Next up we connect an operation (a WebSocket message) to the service, using the decorator `@service.send(...)`. We need to define the operation using a string similar to how we define an HTTP-endpoint using a path.
 
 The operation-identificator is in this case `"ping"`, meaning we will use this string to identify what type of message we are receiving.
 
 ```Python
-@service.send("ping")
-async def send_event_a() -> str:
-    return "pong"
+@service.send("ping", reply="ping")
+async def send_event_a():
+    return
 ```
 
 If we want to define an `payload` for the operation we can extend the example:
 
 ```Python
 from pydantic import BaseModel
 
 class PingPayload(BaseModel):
     foo: str
 
-@service.send("ping")
-async def send_event_a(payload: PingPayload) -> str:
-    return "pong"
+@service.send("ping", reply="ping")
+async def send_event_a(payload: PingPayload):
+    return
 ```
 
 An incoming message should now have the following format. (We will later view this in the generated AsyncAPI-documentation).
 
 ```json
 {
     "type": "ping",
@@ -178,15 +178,15 @@
 
 
 class SubscribeResponse(BaseModel):
     detail: str
     topics: set[str]
 
 
-@router.send("subscribe")
+@router.send("subscribe", reply="subscribe.response")
 async def subscribe_to_topic(
     payload: SubscribePayload,
     client: Client,
 ) -> SubscribeResponse:
     client.subscribe(payload.topic)
     return SubscribeResponse(
         detail=f"Subscribed to {payload.topic}",
@@ -239,15 +239,15 @@
     foo: str
 
 
 class Thing(BaseModel):
     bar: str
 
 
-@router.send("foo")
+@router.send("foo", reply="bar")
 async def some_function(
     payload: Something,
     client: Client,
     app: FastWS,
 ) -> Thing:
     print(f"{app.connections=}")
     print(f"{client.uid=}")
@@ -370,15 +370,15 @@
     _=Depends(custom_dep),
 ):
     await service.serve(client)
 ```
 
 ## Heartbeats and connection lifespan
 
-To handle a WebSocket's lifespan FastWS tries to help you by using `asyncio.timeout()`-context managers in its `serve(client)`-function.
+To handle a WebSocket's lifespan at an application level, FastWS tries to help you by using `asyncio.timeout()`-context managers in its `serve(client)`-function.
 
 You can set the both:
 - `heartbeat_interval`: Meaning a client needs to send a message within this time.
 - `max_connection_lifespan`: Meaning all connections will disconnect when exceeding this time.
 
 These must set during initialization:
 
@@ -389,11 +389,11 @@
     heartbeat_interval=10,
     max_connection_lifespan=300,
 )
 ```
 
 Both `heartbeat_interval` and `max_connection_lifespan` can be set to None to disable any restrictions. Note this is the default.
 
-Please note that you can often also set restrictions in your ASGI-server. Applicable settings for [uvicorn](https://www.uvicorn.org/#command-line-options):
+Please note that you can also set restrictions in your ASGI-server. These restrictions apply at a protocol/server-level and are different from the restrictions set by your application. Applicable settings for [uvicorn](https://www.uvicorn.org/#command-line-options):
 - `--ws-ping-interval` INTEGER
 - `--ws-ping-timeout` INTEGER
 - `--ws-max-size` INTEGER
```

### Comparing `fastws-0.1.5/fastws/application.py` & `fastws-0.1.6/fastws/application.py`

 * *Files identical despite different names*

### Comparing `fastws-0.1.5/fastws/asyncapi.py` & `fastws-0.1.6/fastws/asyncapi.py`

 * *Files identical despite different names*

### Comparing `fastws-0.1.5/fastws/broker.py` & `fastws-0.1.6/fastws/broker.py`

 * *Files identical despite different names*

### Comparing `fastws-0.1.5/fastws/docs.py` & `fastws-0.1.6/fastws/docs.py`

 * *Files identical despite different names*

### Comparing `fastws-0.1.5/fastws/routing.py` & `fastws-0.1.6/fastws/routing.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,15 @@
                 operation=f"{prefix}{router.prefix}{route.operation}",
                 handler=route.handler,
                 method=route.method,
                 name=route.name,
                 tags=route.tags,
                 summary=route.summary,
                 description=route.description,
+                reply_operation=f"{prefix}{router.prefix}{route.reply_operation}",
             )
 
     def send(
         self,
         operation: str,
         name: str | None = None,
         tags: list[str | Enum] | None = None,
```

### Comparing `fastws-0.1.5/pyproject.toml` & `fastws-0.1.6/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastws"
-version = "0.1.5"
+version = "0.1.6"
 description = "FastWS framework. A WebSocket wrapper around FastAPI with auto-documentation using AsyncAPI."
 authors = ["Endre Krohn <endre@skript.no>"]
 readme = "README.md"
 packages = [{ include = "fastws" }]
 repository = "https://github.com/endrekrohn/fastws"
 documentation = "https://github.com/endrekrohn/fastws"
 keywords = ["fastapi", "pydantic", "starlette", "websockets", "asyncapi"]
@@ -29,11 +29,13 @@
 
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.24.0"
 black = "^23.3.0"
 ruff = "^0.0.277"
 uvicorn = { extras = ["standard"], version = "^0.22.0" }
+pytest = "^7.4.0"
+httpx = "^0.24.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fastws-0.1.5/PKG-INFO` & `fastws-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastws
-Version: 0.1.5
+Version: 0.1.6
 Summary: FastWS framework. A WebSocket wrapper around FastAPI with auto-documentation using AsyncAPI.
 Home-page: https://github.com/endrekrohn/fastws
 Keywords: fastapi,pydantic,starlette,websockets,asyncapi
 Author: Endre Krohn
 Author-email: endre@skript.no
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -84,17 +84,17 @@
 
 from fastapi import Depends, FastAPI
 from fastws import Client, FastWS
 
 service = FastWS()
 
 
-@service.send("ping")
-async def send_event_a() -> str:
-    return "pong"
+@service.send("ping", reply="ping")
+async def send_event_a():
+    return
 
 
 @asynccontextmanager
 async def lifespan(app: FastAPI):
     service.setup(app)
     yield
 
@@ -131,30 +131,30 @@
 #### Define event
 
 Next up we connect an operation (a WebSocket message) to the service, using the decorator `@service.send(...)`. We need to define the operation using a string similar to how we define an HTTP-endpoint using a path.
 
 The operation-identificator is in this case `"ping"`, meaning we will use this string to identify what type of message we are receiving.
 
 ```Python
-@service.send("ping")
-async def send_event_a() -> str:
-    return "pong"
+@service.send("ping", reply="ping")
+async def send_event_a():
+    return
 ```
 
 If we want to define an `payload` for the operation we can extend the example:
 
 ```Python
 from pydantic import BaseModel
 
 class PingPayload(BaseModel):
     foo: str
 
-@service.send("ping")
-async def send_event_a(payload: PingPayload) -> str:
-    return "pong"
+@service.send("ping", reply="ping")
+async def send_event_a(payload: PingPayload):
+    return
 ```
 
 An incoming message should now have the following format. (We will later view this in the generated AsyncAPI-documentation).
 
 ```json
 {
     "type": "ping",
@@ -205,15 +205,15 @@
 
 
 class SubscribeResponse(BaseModel):
     detail: str
     topics: set[str]
 
 
-@router.send("subscribe")
+@router.send("subscribe", reply="subscribe.response")
 async def subscribe_to_topic(
     payload: SubscribePayload,
     client: Client,
 ) -> SubscribeResponse:
     client.subscribe(payload.topic)
     return SubscribeResponse(
         detail=f"Subscribed to {payload.topic}",
@@ -266,15 +266,15 @@
     foo: str
 
 
 class Thing(BaseModel):
     bar: str
 
 
-@router.send("foo")
+@router.send("foo", reply="bar")
 async def some_function(
     payload: Something,
     client: Client,
     app: FastWS,
 ) -> Thing:
     print(f"{app.connections=}")
     print(f"{client.uid=}")
@@ -397,15 +397,15 @@
     _=Depends(custom_dep),
 ):
     await service.serve(client)
 ```
 
 ## Heartbeats and connection lifespan
 
-To handle a WebSocket's lifespan FastWS tries to help you by using `asyncio.timeout()`-context managers in its `serve(client)`-function.
+To handle a WebSocket's lifespan at an application level, FastWS tries to help you by using `asyncio.timeout()`-context managers in its `serve(client)`-function.
 
 You can set the both:
 - `heartbeat_interval`: Meaning a client needs to send a message within this time.
 - `max_connection_lifespan`: Meaning all connections will disconnect when exceeding this time.
 
 These must set during initialization:
 
@@ -416,11 +416,11 @@
     heartbeat_interval=10,
     max_connection_lifespan=300,
 )
 ```
 
 Both `heartbeat_interval` and `max_connection_lifespan` can be set to None to disable any restrictions. Note this is the default.
 
-Please note that you can often also set restrictions in your ASGI-server. Applicable settings for [uvicorn](https://www.uvicorn.org/#command-line-options):
+Please note that you can also set restrictions in your ASGI-server. These restrictions apply at a protocol/server-level and are different from the restrictions set by your application. Applicable settings for [uvicorn](https://www.uvicorn.org/#command-line-options):
 - `--ws-ping-interval` INTEGER
 - `--ws-ping-timeout` INTEGER
 - `--ws-max-size` INTEGER
```

