# Comparing `tmp/brewblox_service-2.1.1.tar.gz` & `tmp/brewblox_service-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brewblox_service-2.1.1.tar", max compression
+gzip compressed data, was "brewblox_service-2.2.0.tar", max compression
```

## Comparing `brewblox_service-2.1.1.tar` & `brewblox_service-2.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35140 2023-06-16 14:05:24.031319 brewblox_service-2.1.1/LICENSE.md
--rw-r--r--   0        0        0     3464 2023-06-16 14:05:24.031319 brewblox_service-2.1.1/README.md
--rw-r--r--   0        0        0     1147 2023-06-16 14:05:24.031319 brewblox_service-2.1.1/brewblox_service/__init__.py
--rw-r--r--   0        0        0     1503 2023-06-16 14:05:24.031319 brewblox_service-2.1.1/brewblox_service/cors.py
--rw-r--r--   0        0        0     9598 2023-06-16 14:05:24.031319 brewblox_service-2.1.1/brewblox_service/features.py
--rw-r--r--   0        0        0     1153 2023-06-16 14:05:24.031319 brewblox_service-2.1.1/brewblox_service/http.py
--rw-r--r--   0        0        0    13912 2023-06-16 14:05:24.031319 brewblox_service-2.1.1/brewblox_service/mqtt.py
--rw-r--r--   0        0        0     5294 2023-06-16 14:05:24.031319 brewblox_service-2.1.1/brewblox_service/repeater.py
--rw-r--r--   0        0        0     5649 2023-06-16 14:05:24.031319 brewblox_service-2.1.1/brewblox_service/scheduler.py
--rw-r--r--   0        0        0     7470 2023-06-16 14:05:24.035319 brewblox_service-2.1.1/brewblox_service/service.py
--rw-r--r--   0        0        0     1796 2023-06-16 14:05:24.035319 brewblox_service-2.1.1/brewblox_service/testing.py
--rw-r--r--   0        0        0      663 2023-06-16 14:05:24.035319 brewblox_service-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     4094 1970-01-01 00:00:00.000000 brewblox_service-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35140 2023-07-27 15:34:48.033140 brewblox_service-2.2.0/LICENSE.md
+-rw-r--r--   0        0        0     3464 2023-07-27 15:34:48.033140 brewblox_service-2.2.0/README.md
+-rw-r--r--   0        0        0     1147 2023-07-27 15:34:48.033140 brewblox_service-2.2.0/brewblox_service/__init__.py
+-rw-r--r--   0        0        0     1503 2023-07-27 15:34:48.033140 brewblox_service-2.2.0/brewblox_service/cors.py
+-rw-r--r--   0        0        0     9598 2023-07-27 15:34:48.033140 brewblox_service-2.2.0/brewblox_service/features.py
+-rw-r--r--   0        0        0     1153 2023-07-27 15:34:48.033140 brewblox_service-2.2.0/brewblox_service/http.py
+-rw-r--r--   0        0        0    14766 2023-07-27 15:34:48.033140 brewblox_service-2.2.0/brewblox_service/mqtt.py
+-rw-r--r--   0        0        0     5294 2023-07-27 15:34:48.033140 brewblox_service-2.2.0/brewblox_service/repeater.py
+-rw-r--r--   0        0        0     5649 2023-07-27 15:34:48.033140 brewblox_service-2.2.0/brewblox_service/scheduler.py
+-rw-r--r--   0        0        0     7470 2023-07-27 15:34:48.033140 brewblox_service-2.2.0/brewblox_service/service.py
+-rw-r--r--   0        0        0     2805 2023-07-27 15:34:48.033140 brewblox_service-2.2.0/brewblox_service/testing.py
+-rw-r--r--   0        0        0      664 2023-07-27 15:34:48.033140 brewblox_service-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4101 1970-01-01 00:00:00.000000 brewblox_service-2.2.0/PKG-INFO
```

### Comparing `brewblox_service-2.1.1/LICENSE.md` & `brewblox_service-2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.1.1/README.md` & `brewblox_service-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.1.1/brewblox_service/__init__.py` & `brewblox_service-2.2.0/brewblox_service/__init__.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.1.1/brewblox_service/cors.py` & `brewblox_service-2.2.0/brewblox_service/cors.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.1.1/brewblox_service/features.py` & `brewblox_service-2.2.0/brewblox_service/features.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.1.1/brewblox_service/http.py` & `brewblox_service-2.2.0/brewblox_service/http.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.1.1/brewblox_service/mqtt.py` & `brewblox_service-2.2.0/brewblox_service/mqtt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,59 @@
 """
 Offers publishing and subscribing to MQTT events.
 
 Example use:
 
+    import json
     from brewblox_service import mqtt, scheduler
 
     scheduler.setup(app)
     mqtt.setup(app)
 
     async def on_message(topic, body):
-        print(f'Message published to {topic}')
+        print(f'Message topic: {topic}')
         print(f'Message content: {body}')
 
     mqtt.listen(app, 'brewcast/state/a', on_message)
     mqtt.listen(app, 'brewcast/state/b', on_message)
 
     mqtt.subscribe(app, 'brewcast/state/#')
 
-    await mqtt.publish('app', 'brewcast/state', {'example': True})
-    await mqtt.publish('app', 'brewcast/state/a', {'example': True})
+    await mqtt.publish('app', 'brewcast/state', json.dumps({'example': True}))
+    await mqtt.publish('app', 'brewcast/state/a', json.dumps({'example': True}))
 """
 
 import asyncio
 from contextlib import suppress
 from dataclasses import dataclass, field
 from ssl import CERT_NONE
-from typing import Awaitable, Callable, Optional, Union
+from typing import Awaitable, Callable, Literal, Optional
 
-import aiomqtt
 from aiohttp import web
+from aiomqtt import Client, Message, MqttError, TLSParameters, Will
+from aiomqtt.types import PayloadType
 
-from brewblox_service import brewblox_logger, features, strex
+from brewblox_service import brewblox_logger, features, repeater, strex
 
 LOGGER = brewblox_logger(__name__)
-routes = web.RouteTableDef()
+MQTT_LOGGER = brewblox_logger('aiomqtt')
 
-EventData_ = Union[str, bytes, None]
 ListenerCallback_ = Callable[[str, str], Awaitable[None]]
 
+RECONNECT_INTERVAL_S = 2
+INTERACTION_TIMEOUT_S = 5
 DEFAULT_PORTS = {
     'mqtt': 1883,
     'mqtts': 8883,
     'ws': 80,
     'wss': 443,
 }
 
 
-def decoded(msg: Union[str, bytes, bytearray]):
+def decoded(msg: PayloadType):
     if isinstance(msg, (bytes, bytearray)):
         return msg.decode()
     return msg
 
 
 @dataclass
 class MQTTConfig:
@@ -68,22 +71,22 @@
         if self.protocol.startswith('ws'):
             self.transport = 'websockets'
             self.path = self.path or ''
         else:
             self.transport = 'tcp'
             self.path = ''
 
-        if not self.port or self.port == 5672:
+        if not self.port:
             self.port = DEFAULT_PORTS[self.protocol]
 
     def __str__(self):
         return f'{self.protocol}://{self.host}:{self.port}{self.path}'
 
 
-class EventHandler(features.ServiceFeature):
+class EventHandler(repeater.RepeaterFeature):
     """
     Connection handler class for MQTT events.
     Handles both TCP and Websocket connections.
 
     Automatically reconnects and resubscribes when connection is lost.
 
     Subscribe and listen are handled separately.
@@ -124,142 +127,149 @@
             The default path for the broker is '/eventbus'
 
             Examples: (formatted as <protocol>://<host>:<port><path>)
                 ws://eventbus:15675/eventbus
                 wss://BREWBLOX_HOST:443/eventbus
     """
 
-    def __init__(self, app: web.Application, **kwargs):
-        super().__init__(app)
+    def __init__(self,
+                 app: web.Application,
+                 protocol: Literal['ws', 'wss', 'mqtt', 'mqtts'] = None,
+                 host: str = None,
+                 port: int = None,
+                 path: str = None,
+                 **kwargs):
+        super().__init__(app, **kwargs)
 
         config = app['config']
-        protocol = kwargs.get('protocol', config['mqtt_protocol'])
-        host = kwargs.get('host', config['mqtt_host'])
-        port = kwargs.get('port', config['mqtt_port'])
-        path = kwargs.get('path', config['mqtt_path'])
+        protocol = protocol or config['mqtt_protocol']
+        host = host or config['mqtt_host']
+        port = port or config['mqtt_port']
+        path = path or config['mqtt_path']
         self.config = MQTTConfig(protocol, host, port, path)
-        self.client: aiomqtt.Client = None
+        self.client: Client = None
 
-        self._connect_ev: asyncio.Event = None
-        self._subs: list[str] = []
+        self._ready_ev: asyncio.Event = None
+        self._connect_delay: int = 0
+        self._subscribed_topics: list[str] = []
         self._listeners: list[tuple[str, ListenerCallback_]] = []
 
     def __str__(self):
         return f'<{type(self).__name__} for {self.config}>'
 
     @property
-    def connected(self) -> bool:
-        return self.client is not None \
-            and self._connect_ev is not None \
-            and self._connect_ev.is_set()
+    def ready(self) -> Optional[asyncio.Event]:
+        return self._ready_ev
 
-    def set_client_will(self, topic: str, message: EventData_, **kwargs):
+    def set_client_will(self, topic: str, message: PayloadType, **kwargs):
         if self.client:
             raise RuntimeError('Client will must be set before startup')
         self.config.client_will = dict(topic=topic,
-                                       payload=decoded(message),
+                                       payload=message,
                                        **kwargs)
 
     @staticmethod
-    def create_client(config: MQTTConfig) -> aiomqtt.Client:
-        client = aiomqtt.Client(transport=config.transport,
-                                protocol=aiomqtt.MQTTv311)
-        client.ws_set_options(path=config.path)
-
-        if config.protocol in ['mqtts', 'wss']:
-            client.tls_set(cert_reqs=CERT_NONE)
-            client.tls_insecure_set(True)
+    def create_client(config: MQTTConfig) -> Client:
+        secure_protocol = config.protocol in ['mqtts', 'wss']
+        tls_params = None
+        will = None
+
+        if secure_protocol:
+            tls_params = TLSParameters(cert_reqs=CERT_NONE)
 
         if config.client_will:
-            client.will_set(**config.client_will)
+            will = Will(**config.client_will)
+
+        client = Client(hostname=config.host,
+                        port=config.port,
+                        transport=config.transport,
+                        websocket_path=config.path,
+                        tls_params=tls_params,
+                        will=will,
+                        logger=MQTT_LOGGER)
+
+        if secure_protocol:
+            client._client.tls_insecure_set(True)
 
         return client
 
+    async def _handle_callback(self, cb: ListenerCallback_, message: Message):
+        try:
+            await cb(str(message.topic), decoded(message.payload))
+        except Exception as ex:
+            LOGGER.error(f'Exception handling MQTT callback for {message.topic}: {strex(ex)}')
+
     async def startup(self, app: web.Application):
-        self._connect_ev = asyncio.Event()
+        self._ready_ev = asyncio.Event()
         self.client = self.create_client(self.config)
-        self.client.on_connect = self._on_connect
-        self.client.on_disconnect = self._on_disconnect
-        self.client.on_message = self._on_message
-
-        LOGGER.debug(f'Starting {self}')
-        self.client.connect_async(self.config.host, self.config.port)
-        self.client.loop_start()
 
-    async def shutdown(self, app: web.Application):
-        if self.client:
-            self.client.disconnect()
-            await self.client.loop_stop()
-            self.client = None
-
-    def _on_connect(self, *args):
-        LOGGER.debug(f'Applying subscribe for {self._subs}')
-        for topic in self._subs:
-            self.client.subscribe(topic)
-
-        LOGGER.info(f'{self} connected')
-        self._connect_ev.set()
-
-    def _on_disconnect(self, *args):
-        LOGGER.info(f'{self} disconnected')
-        self._connect_ev.clear()
+    async def run(self):
+        await asyncio.sleep(self._connect_delay)
+        self._connect_delay = RECONNECT_INTERVAL_S
 
-    async def _handle_callback(self, cb: ListenerCallback_, topic: str, payload: str):
         try:
-            await cb(topic, payload)
-        except Exception as ex:
-            LOGGER.error(f'Exception handling MQTT callback for {topic}: {strex(ex)}')
+            async with self.client:
+                async with self.client.messages() as messages:
+                    if self._subscribed_topics:
+                        await self.client.subscribe([(t, 0) for t in self._subscribed_topics],
+                                                    timeout=INTERACTION_TIMEOUT_S)
+
+                    LOGGER.debug(f'{self} is ready')
+                    self._ready_ev.set()
+
+                    async for message in messages:  # pragma: no cover
+                        matching = [cb
+                                    for (topic, cb) in self._listeners
+                                    if message.topic.matches(topic)]
 
-    def _on_message(self, client, userdata, message, *args):
-        try:
-            topic = decoded(message.topic)
-            payload = decoded(message.payload)
-        except UnicodeDecodeError:  # pragma: no cover
-            LOGGER.error('Skipping malformed MQTT event')
-            return
-
-        matching = [cb
-                    for (sub, cb) in self._listeners
-                    if aiomqtt.topic_matches_sub(sub, topic)]
+                        for cb in matching:
+                            asyncio.create_task(self._handle_callback(cb, message))
 
-        for cb in matching:
-            asyncio.create_task(self._handle_callback(cb, topic, payload))
+                        if not matching:
+                            LOGGER.debug(f'{self} recv {message}')
 
-        if not matching:
-            LOGGER.debug(f'{self} recv topic={topic}, msg={str(payload)[:30]}...')
+        finally:
+            self._ready_ev.clear()
 
     async def publish(self,
                       topic: str,
-                      message: EventData_,
+                      message: PayloadType,
                       retain=False,
                       qos=0,
                       err=True,
                       **kwargs):
-        info = self.client.publish(topic, decoded(message), retain=retain, qos=qos, **kwargs)
-        error = aiomqtt.error_string(info.rc)
-        LOGGER.debug(f'publish({topic}) -> {error}')
-        if info.rc != 0 and err:
-            raise ConnectionError(f'Publish error="{error}", topic="{topic}"')
+        try:
+            await self.client.publish(topic,
+                                      message,
+                                      retain=retain,
+                                      qos=qos,
+                                      timeout=INTERACTION_TIMEOUT_S,
+                                      **kwargs)
+            LOGGER.debug(f'publish({topic}) -> OK')
+        except MqttError as ex:
+            LOGGER.debug(f'publish({topic}) -> {strex(ex)}')
+            if err:
+                raise ConnectionError(f'Publish error="{strex(ex)}", topic="{topic}"') from ex
 
     async def subscribe(self, topic: str):
         LOGGER.debug(f'subscribe({topic})')
-        self._subs.append(topic)
-        if self.connected:
-            self.client.subscribe(topic)
+        self._subscribed_topics.append(topic)
+        with suppress(MqttError):
+            await self.client.subscribe(topic, timeout=INTERACTION_TIMEOUT_S)
 
     async def listen(self, topic: str, callback: ListenerCallback_):
         LOGGER.debug(f'listen({topic})')
         self._listeners.append((topic, callback))
 
     async def unsubscribe(self, topic: str):
         LOGGER.debug(f'unsubscribe({topic})')
-        if self.connected:
-            self.client.unsubscribe(topic)
+        with suppress(MqttError):
+            await self.client.unsubscribe(topic, timeout=INTERACTION_TIMEOUT_S)
         with suppress(ValueError):
-            self._subs.remove(topic)
+            self._subscribed_topics.remove(topic)
 
     async def unlisten(self, topic: str, callback: ListenerCallback_):
         LOGGER.debug(f'unlisten({topic})')
         with suppress(ValueError):
             self._listeners.remove((topic, callback))
 
 
@@ -268,32 +278,45 @@
     Initializes the EventHandler in the app context.
 
     Args:
         app (web.Application):
             The Aiohttp Application object.
     """
     features.add(app, EventHandler(app, **kwargs))
-    app.router.add_routes(routes)
 
 
-def handler(app: web.Application) -> EventHandler:
+def fget(app: web.Application) -> EventHandler:
+    """
+    Get registered EventHandler.
+    Requires setup(app) to have been called first.
+
+    Args:
+        app (web.Application):
+            The Aiohttp Application object.
     """
+    return features.get(app, EventHandler)
+
+
+def handler(app: web.Application) -> EventHandler:  # pragma: no cover
+    """
+    Deprecated: use fget() instead
+
     Get registered EventHandler.
     Requires setup(app) to have been called first.
 
     Args:
         app (web.Application):
             The Aiohttp Application object.
     """
     return features.get(app, EventHandler)
 
 
 def set_client_will(app: web.Application,
                     topic: str,
-                    message: EventData_ = None,
+                    message: PayloadType = None,
                     **kwargs):
     """
     Set MQTT Last Will and Testament for client.
     Requires setup(app) to have been called first.
     Must be called before startup.
 
     Args:
@@ -307,15 +330,15 @@
             The payload that will be published by the broker on our behalf after disconnecting.
     """
     handler(app).set_client_will(topic, message, **kwargs)
 
 
 async def publish(app: web.Application,
                   topic: str,
-                  message: EventData_,
+                  message: PayloadType,
                   retain=False,
                   qos=0,
                   err=True,
                   **kwargs):
     """
     Publish a new event message.
```

### Comparing `brewblox_service-2.1.1/brewblox_service/repeater.py` & `brewblox_service-2.2.0/brewblox_service/repeater.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.1.1/brewblox_service/scheduler.py` & `brewblox_service-2.2.0/brewblox_service/scheduler.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.1.1/brewblox_service/service.py` & `brewblox_service-2.2.0/brewblox_service/service.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.1.1/brewblox_service/testing.py` & `brewblox_service-2.2.0/brewblox_service/testing.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 Testing utility functions
 """
 
 import re
+from contextlib import contextmanager
+from subprocess import DEVNULL, run
 
 from aiohttp.client_exceptions import ContentTypeError
 
 
 async def response(request, status=200):
     retv = await request
     payload = await retv.text()
@@ -53,7 +55,39 @@
     s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
     s.bind(('0.0.0.0', 0))
     portnum = s.getsockname()[1]
     s.close()
 
     return portnum
+
+
+@contextmanager
+def mqtt_broker(name='mqtt-test-broker', image='ghcr.io/brewblox/mosquitto:develop'):
+    """
+    Spawns and closes an MQTT broker image.
+    To prevent conflict, it listens on random free ports.
+    The context manager yields a dict containing the randomly selected port numbers.
+    """
+    mqtt_port = find_free_port()
+    ws_port = find_free_port()
+    run(['docker', 'stop', name], stdout=DEVNULL)
+    run(
+        [
+            'docker',
+            'run',
+            '--rm',
+            '--detach',
+            f'--name={name}',
+            f'--publish={mqtt_port}:1883',
+            f'--publish={ws_port}:15675',
+            image,
+        ],
+        check=True)
+    try:
+        yield {'mqtt': mqtt_port, 'ws': ws_port}
+    except Exception:
+        run(['docker', 'ps'])
+        raise
+    finally:
+        run(['docker', 'logs', '--timestamps', name])
+        run(['docker', 'stop', name], stdout=DEVNULL)
```

### Comparing `brewblox_service-2.1.1/pyproject.toml` & `brewblox_service-2.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "brewblox-service"
-version = "2.1.1"
+version = "2.2.0"
 description = "Scaffolding for Brewblox backend services"
 authors = ["BrewPi <development@brewpi.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.pyright]
 include = ["brewblox_service"]
 exclude = ["**/node_modules", "**/__pycache__"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 aiohttp = ">=3.7"
-aiomqtt = "0.1.3"
+aiomqtt = "^1.0.0"
 aiohttp-pydantic = ">=1.12"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "*"
 pytest-cov = "*"
 pytest-mock = "*"
 pytest-aiohttp = "*"
```

### Comparing `brewblox_service-2.1.1/PKG-INFO` & `brewblox_service-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: brewblox-service
-Version: 2.1.1
+Version: 2.2.0
 Summary: Scaffolding for Brewblox backend services
 License: GPL-3.0
 Author: BrewPi
 Author-email: development@brewpi.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.7)
 Requires-Dist: aiohttp-pydantic (>=1.12)
-Requires-Dist: aiomqtt (==0.1.3)
+Requires-Dist: aiomqtt (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Scaffolding for Brewblox service applications
 
 In order to reduce code duplication between services, generic functionality is implemented here.
 
 For an example on how to implement your own service based on `brewblox-service`, see <https://github.com/brewblox/brewblox-boilerplate>.
```

