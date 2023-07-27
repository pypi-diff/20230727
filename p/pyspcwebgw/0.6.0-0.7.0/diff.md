# Comparing `tmp/pyspcwebgw-0.6.0.tar.gz` & `tmp/pyspcwebgw-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspcwebgw-0.6.0.tar", last modified: Mon Jun 13 20:13:14 2022, max compression
+gzip compressed data, was "pyspcwebgw-0.7.0.tar", max compression
```

## Comparing `pyspcwebgw-0.6.0.tar` & `pyspcwebgw-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 20:13:14.528295 pyspcwebgw-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-06-13 20:13:07.000000 pyspcwebgw-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-06-13 20:13:07.000000 pyspcwebgw-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-06-13 20:13:14.528295 pyspcwebgw-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      633 2022-06-13 20:13:07.000000 pyspcwebgw-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 20:13:14.528295 pyspcwebgw-0.6.0/pyspcwebgw/
--rw-r--r--   0 runner    (1001) docker     (121)     4763 2022-06-13 20:13:07.000000 pyspcwebgw-0.6.0/pyspcwebgw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1446 2022-06-13 20:13:07.000000 pyspcwebgw-0.6.0/pyspcwebgw/area.py
--rw-r--r--   0 runner    (1001) docker     (121)     1117 2022-06-13 20:13:07.000000 pyspcwebgw-0.6.0/pyspcwebgw/const.py
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-06-13 20:13:07.000000 pyspcwebgw-0.6.0/pyspcwebgw/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2538 2022-06-13 20:13:07.000000 pyspcwebgw-0.6.0/pyspcwebgw/websocket.py
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-06-13 20:13:07.000000 pyspcwebgw-0.6.0/pyspcwebgw/zone.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 20:13:14.528295 pyspcwebgw-0.6.0/pyspcwebgw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-06-13 20:13:14.000000 pyspcwebgw-0.6.0/pyspcwebgw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-06-13 20:13:14.000000 pyspcwebgw-0.6.0/pyspcwebgw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-13 20:13:14.000000 pyspcwebgw-0.6.0/pyspcwebgw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-13 20:13:14.000000 pyspcwebgw-0.6.0/pyspcwebgw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-06-13 20:13:14.000000 pyspcwebgw-0.6.0/pyspcwebgw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-06-13 20:13:14.528295 pyspcwebgw-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-06-13 20:13:07.000000 pyspcwebgw-0.6.0/setup.py
+-rw-r--r--   0        0        0     1068 2023-07-27 16:13:56.100322 pyspcwebgw-0.7.0/LICENSE
+-rw-r--r--   0        0        0      633 2023-07-27 16:13:56.100322 pyspcwebgw-0.7.0/README.md
+-rw-r--r--   0        0        0     1007 2023-07-27 16:13:56.100322 pyspcwebgw-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5545 2023-07-27 16:13:56.100322 pyspcwebgw-0.7.0/pyspcwebgw/__init__.py
+-rw-r--r--   0        0        0     2081 2023-07-27 16:13:56.100322 pyspcwebgw-0.7.0/pyspcwebgw/area.py
+-rw-r--r--   0        0        0     1117 2023-07-27 16:13:56.100322 pyspcwebgw-0.7.0/pyspcwebgw/const.py
+-rw-r--r--   0        0        0     1222 2023-07-27 16:13:56.100322 pyspcwebgw-0.7.0/pyspcwebgw/utils.py
+-rw-r--r--   0        0        0     2510 2023-07-27 16:13:56.100322 pyspcwebgw-0.7.0/pyspcwebgw/websocket.py
+-rw-r--r--   0        0        0     1571 2023-07-27 16:13:56.100322 pyspcwebgw-0.7.0/pyspcwebgw/zone.py
+-rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 pyspcwebgw-0.7.0/PKG-INFO
```

### Comparing `pyspcwebgw-0.6.0/LICENSE` & `pyspcwebgw-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspcwebgw-0.6.0/PKG-INFO` & `pyspcwebgw-0.7.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: pyspcwebgw
-Version: 0.6.0
+Version: 0.7.0
 Summary: A Python library for communicating with SPC Web Gateway.
-Home-page: https://github.com/mbrrg/pyspcwebgw
-Author: Martin Berg
-Author-email: mbrrg@users.noreply.github.com
 License: MIT
-Download-URL: https://github.com/mbrrg/pyspcwebgw/archive/0.6.0.zip
 Keywords: spc,vanderbilt,web gateway
-Platform: UNKNOWN
+Author: Martin Berg
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Home Automation
-Requires-Python: >=3.7
+Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 Python library for communicating with [Vanderbilt SPC alarm systems](https://vanderbiltindustries.com/spc) via the REST/websocket API provided by the SPC Web Gateway software made by [Lundix IT](http://www.lundix.se/smarta-losningar/). Using this library you can:
 
 - Retrieve information for all alarm areas and zones.
 - Change the alarm mode, i.e. arming and disarming of the alarm system.
 - Get real-time updates when attributes of areas and zones change, e.g. if motion detector connected to the systems triggers or when the alarm goes off.
 
 ## Usage
 
 ### Library
 
 To use the library in your own application see the example file.
 
-
```

### Comparing `pyspcwebgw-0.6.0/README.md` & `pyspcwebgw-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pyspcwebgw-0.6.0/pyspcwebgw/__init__.py` & `pyspcwebgw-0.7.0/pyspcwebgw/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Python wrapper for the Lundix SPC Web Gateway REST API."""
+import asyncio
 import logging
 from urllib.parse import urljoin
-from asyncio import ensure_future
 
 from .area import Area
-from .zone import Zone
 from .const import AreaMode
 from .utils import async_request
 from .websocket import AIOWSClient
+from .zone import Zone
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class SpcWebGateway:
     """Alarm system representation."""
 
@@ -20,14 +20,15 @@
         self._loop = loop
         self._session = session
         self._api_url = api_url
         self._ws_url = ws_url
         self._info = None
         self._areas = {}
         self._zones = {}
+        self._ethernet = {}
         self._websocket = None
         self._async_callback = async_callback
 
     @property
     def info(self):
         """Retrieve basic panel info."""
         return self._info
@@ -38,107 +39,134 @@
         return self._areas
 
     @property
     def zones(self):
         """Retrieve all available zones."""
         return self._zones
 
+    @property
+    def ethernet(self):
+        """Retrieve all ethernet information."""
+        return self._ethernet
+
     def start(self):
         """Connect websocket to SPC Web Gateway."""
-        self._websocket = AIOWSClient(loop=self._loop,
-                                      session=self._session,
-                                      url=self._ws_url,
-                                      async_callback=self._async_ws_handler)
+        self._websocket = AIOWSClient(
+            loop=self._loop,
+            session=self._session,
+            url=self._ws_url,
+            async_callback=self._async_ws_handler,
+        )
         self._websocket.start()
 
     def stop(self):
         """Disconnect websocket to SPC Web Gateway."""
         self._websocket.stop()
         self._websocket = None
 
     async def async_load_parameters(self):
         """Fetch area and zone info from SPC to initialize."""
-        self._info = await self._async_get_data('panel')
-        zones = await self._async_get_data('zone')
-        areas = await self._async_get_data('area')
+        self._info = await self._async_get_data("panel")
+        self._ethernet = await self._async_get_data("ethernet")
+
+        zones = await self._async_get_data("zone")
+        areas = await self._async_get_data("area")
 
         if not zones or not areas:
             return False
 
         for spc_area in areas:
             area = Area(self, spc_area)
-            area_zones = [Zone(area, z) for z in zones
-                          if z['area'] == spc_area['id']]
+            area_zones = [Zone(area, z) for z in zones if z["area"] == spc_area["id"]]
             area.zones = area_zones
             self._areas[area.id] = area
             self._zones.update({z.id: z for z in area_zones})
 
         return True
 
     async def change_mode(self, area, new_mode):
         """Set/unset/part set an area."""
         if not isinstance(new_mode, AreaMode):
             raise TypeError("new_mode must be an AreaMode")
 
         AREA_MODE_COMMAND_MAP = {
-            AreaMode.UNSET: 'unset',
-            AreaMode.PART_SET_A: 'set_a',
-            AreaMode.PART_SET_B: 'set_b',
-            AreaMode.FULL_SET: 'set'
+            AreaMode.UNSET: "unset",
+            AreaMode.PART_SET_A: "set_a",
+            AreaMode.PART_SET_B: "set_b",
+            AreaMode.FULL_SET: "set",
         }
         if isinstance(area, Area):
             area_id = area.id
         else:
             area_id = area
 
-        url = urljoin(self._api_url, "spc/area/{area_id}/{command}".format(
-            area_id=area_id, command=AREA_MODE_COMMAND_MAP[new_mode]))
+        url = urljoin(
+            self._api_url,
+            "spc/area/{area_id}/{command}".format(
+                area_id=area_id, command=AREA_MODE_COMMAND_MAP[new_mode]
+            ),
+        )
 
         return await async_request(self._session.put, url)
 
     async def _async_ws_handler(self, data):
         """Process incoming websocket message."""
-        sia_message = data['data']['sia']
-        spc_id = sia_message['sia_address']
-        sia_code = sia_message['sia_code']
+        sia_message = data["data"]["sia"]
+        spc_id = sia_message["sia_address"]
+        sia_code = sia_message["sia_code"]
+        # sia_description contains different info in different cases,
+        # needed to get last_changed_by user for PART_SET (sia_code NL)
+        sia_description = sia_message["description"]
 
         _LOGGER.debug("SIA code is %s for ID %s", sia_code, spc_id)
 
         if sia_code in Area.SUPPORTED_SIA_CODES:
-            entity = self._areas.get(spc_id, None)
-            resource = 'area'
+            entities = [self._areas.get(spc_id, None)]
+            resource = "area"
         elif sia_code in Zone.SUPPORTED_SIA_CODES:
-            entity = self._zones.get(spc_id, None)
-            resource = 'zone'
+            entities = [self._zones.get(spc_id, None)]
+            resource = "zone"
+        elif sia_code in ("CL", "OP"):
+            # workaround for area mode change update in certain firmwares
+            # sia_code is in fact the user performing the change so
+            # refresh all areas
+            entities = self._areas.values()
+            resource = "area"
         else:
             _LOGGER.debug("Not interested in SIA code %s", sia_code)
             return
-        if not entity:
+
+        if not entities:
             _LOGGER.error("Received message for unregistered ID %s", spc_id)
             return
 
-        data = await self._async_get_data(resource, entity.id)
-        entity.update(data, sia_code)
+        tasks = []
+
+        for entity in entities:
+            data = await self._async_get_data(resource, entity.id)
+            entity.update(data, sia_code, sia_description)
+
+            if self._async_callback:
+                tasks.append(asyncio.create_task(self._async_callback(entity)))
 
-        if self._async_callback:
-            ensure_future(self._async_callback(entity))
+        return tasks
 
     async def _async_get_data(self, resource, id=None):
         """Get the data from the resource."""
         if id:
             url = urljoin(self._api_url, "spc/{}/{}".format(resource, id))
         else:
             url = urljoin(self._api_url, "spc/{}".format(resource))
         data = await async_request(self._session.get, url)
         if not data:
             return False
-        if id and isinstance(data['data'][resource], list):
+        if id and isinstance(data["data"][resource], list):
             # for some reason the gateway returns an array with a single
             # element for areas but not for zones...
-            return data['data'][resource][0]
+            return data["data"][resource][0]
         elif id:
-            return data['data'][resource]
+            return data["data"][resource]
 
-        if isinstance(data['data'][resource], list):  
-            return [item for item in data['data'][resource]]
+        if isinstance(data["data"][resource], list):
+            return [item for item in data["data"][resource]]
 
-        return data['data'][resource]
+        return data["data"][resource]
```

### Comparing `pyspcwebgw-0.6.0/pyspcwebgw/utils.py` & `pyspcwebgw-0.7.0/pyspcwebgw/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,26 +18,26 @@
 async def async_request(session, url, **kwargs):
     """Do a web request and manage response."""
     try:
         with async_timeout.timeout(10):
             _LOGGER.debug("Sending %s to %s", kwargs, url)
             response = await session(url, **kwargs)
         if response.status != 200:
-            _LOGGER.error("HTTP status %d, response %s.",
-                          response.status, (await response.text()))
+            _LOGGER.error(
+                "HTTP status %d, response %s.", response.status, (await response.text())
+            )
             return False
         result = await response.json()
     except asyncio.TimeoutError:
         _LOGGER.error("Timeout getting SPC data from %s.", url)
         return False
     except aiohttp.ClientError:
         _LOGGER.error("Error getting SPC data from %s.", url)
         return False
     else:
         _LOGGER.debug("HTTP request response: %s", result)
 
-    if result['status'] != 'success':
-        _LOGGER.error(
-            "SPC Web Gateway call unsuccessful for resource: %s", url)
+    if result["status"] != "success":
+        _LOGGER.error("SPC Web Gateway call unsuccessful for resource: %s", url)
         return False
 
     return result
```

### Comparing `pyspcwebgw-0.6.0/pyspcwebgw/websocket.py` & `pyspcwebgw-0.7.0/pyspcwebgw/websocket.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-import logging
 import json
+import logging
 from asyncio import ensure_future
 
 import aiohttp
 
 _LOGGER = logging.getLogger(__name__)
 
-STATE_STARTING = 'starting'
-STATE_RUNNING = 'running'
-STATE_STOPPED = 'stopped'
+STATE_STARTING = "starting"
+STATE_RUNNING = "running"
+STATE_STOPPED = "stopped"
 
 RETRY_TIMER = 15
 
 
 class AIOWSClient:
     """Websocket transport, session handling, message generation."""
+
     """https://github.com/Kane610/deconz/blob/master/pydeconz/websocket.py"""
 
     def __init__(self, loop, session, url, async_callback):
         """Create resources for websocket communication."""
         self._loop = loop
         self._session = session
         self._url = url
@@ -36,40 +37,39 @@
         """"""
         return self._state
 
     @state.setter
     def state(self, value):
         """"""
         self._state = value
-        _LOGGER.debug('Websocket %s', value)
+        _LOGGER.debug("Websocket %s", value)
 
     def start(self):
         if self.state != STATE_RUNNING:
             self.state = STATE_STARTING
         self._task = self._loop.create_task(self.running())
 
     async def running(self):
         """Start websocket connection."""
         try:
             async with self._session.ws_connect(self._url) as ws:
                 self.state = STATE_RUNNING
                 async for msg in ws:
                     if msg.type == aiohttp.WSMsgType.TEXT:
-                        ensure_future(self._async_callback(
-                            json.loads(msg.data)))
-                        _LOGGER.debug('Websocket data: %s', msg.data)
+                        ensure_future(self._async_callback(json.loads(msg.data)))
+                        _LOGGER.debug("Websocket data: %s", msg.data)
                     elif msg.type == aiohttp.WSMsgType.CLOSED:
                         break
                     elif msg.type == aiohttp.WSMsgType.ERROR:
                         break
         except aiohttp.ClientConnectorError:
             if self.state != STATE_STOPPED:
                 self.retry()
         except Exception as err:
-            _LOGGER.error('Unexpected error %s', err)
+            _LOGGER.error("Unexpected error %s", err)
             if self.state != STATE_STOPPED:
                 self.retry()
         else:
             if self.state != STATE_STOPPED:
                 self.retry()
 
     def stop(self):
@@ -78,8 +78,8 @@
         if self._task:
             self._task.cancel()
 
     def retry(self):
         """Retry to connect to SPC."""
         self.state = STATE_STARTING
         self._loop.call_later(RETRY_TIMER, self.start)
-        _LOGGER.debug('Reconnecting to SPC in %i.', RETRY_TIMER)
+        _LOGGER.debug("Reconnecting to SPC in %i.", RETRY_TIMER)
```

### Comparing `pyspcwebgw-0.6.0/pyspcwebgw/zone.py` & `pyspcwebgw-0.7.0/pyspcwebgw/zone.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import logging
 
-from pyspcwebgw.const import ZoneInput, ZoneType, ZoneStatus
-from pyspcwebgw.utils import _load_enum
+from .const import ZoneInput, ZoneStatus, ZoneType
+from .utils import _load_enum
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class Zone:
     """Represents an SPC alarm system zone."""
-    SUPPORTED_SIA_CODES = ('ZO', 'ZC', 'ZX', 'ZD', 'ZM', 'BA',
-                           'BB', 'BU', 'BR', 'BC')
+
+    SUPPORTED_SIA_CODES = ("ZO", "ZC", "ZX", "ZD", "ZM", "BA", "BB", "BU", "BR", "BC")
 
     def __init__(self, area, spc_zone):
-        self._id = spc_zone['id']
-        self._name = spc_zone['zone_name']
+        self._id = spc_zone["id"]
+        self._name = spc_zone["zone_name"]
         self._area = area
 
         self.update(spc_zone)
 
     def __str__(self):
-        return '{id}: {name} ({type}). Input: {inp}, status: {status}'.format(
-            id=self.id, name=self.name, type=self.type,
-            inp=self.input, status=self.status)
+        return "{id}: {name} ({type}). Input: {inp}, status: {status}".format(
+            id=self.id,
+            name=self.name,
+            type=self.type,
+            inp=self.input,
+            status=self.status,
+        )
 
     @property
     def id(self):
         return self._id
 
     @property
     def name(self):
@@ -43,13 +47,20 @@
     def status(self):
         return self._status
 
     @property
     def area(self):
         return self._area
 
-    def update(self, spc_zone, sia_code=None):
+    def update(self, spc_zone, sia_code=None, sia_description=None):
         _LOGGER.debug("Update zone %s", self.id)
 
-        self._input = _load_enum(ZoneInput, spc_zone['input'])
-        self._type = _load_enum(ZoneType, spc_zone['type'])
-        self._status = _load_enum(ZoneStatus, spc_zone['status'])
+        self._type = _load_enum(ZoneType, spc_zone["type"])
+        self._status = _load_enum(ZoneStatus, spc_zone["status"])
+
+        input = _load_enum(ZoneInput, spc_zone["input"])
+
+        if sia_code == "ZO" and input == ZoneInput.CLOSED:
+            # work around race condition for wireless sensors
+            input = ZoneInput.OPEN
+
+        self._input = input
```

