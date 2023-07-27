# Comparing `tmp/reolink_aio-0.7.3.tar.gz` & `tmp/reolink_aio-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reolink_aio-0.7.3.tar", last modified: Mon Jul 10 20:15:42 2023, max compression
+gzip compressed data, was "reolink_aio-0.7.4.tar", last modified: Thu Jul 27 20:03:29 2023, max compression
```

## Comparing `reolink_aio-0.7.3.tar` & `reolink_aio-0.7.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 20:15:42.851384 reolink_aio-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-07-10 20:15:26.000000 reolink_aio-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4720 2023-07-10 20:15:42.851384 reolink_aio-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3912 2023-07-10 20:15:26.000000 reolink_aio-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 20:15:42.851384 reolink_aio-0.7.3/reolink_aio/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-10 20:15:26.000000 reolink_aio-0.7.3/reolink_aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   192713 2023-07-10 20:15:26.000000 reolink_aio-0.7.3/reolink_aio/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-07-10 20:15:26.000000 reolink_aio-0.7.3/reolink_aio/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-07-10 20:15:26.000000 reolink_aio-0.7.3/reolink_aio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     9403 2023-07-10 20:15:26.000000 reolink_aio-0.7.3/reolink_aio/software_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     7935 2023-07-10 20:15:26.000000 reolink_aio-0.7.3/reolink_aio/templates.py
--rw-r--r--   0 runner    (1001) docker     (122)    15330 2023-07-10 20:15:26.000000 reolink_aio-0.7.3/reolink_aio/typings.py
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-10 20:15:26.000000 reolink_aio-0.7.3/reolink_aio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 20:15:42.851384 reolink_aio-0.7.3/reolink_aio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4720 2023-07-10 20:15:42.000000 reolink_aio-0.7.3/reolink_aio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      439 2023-07-10 20:15:42.000000 reolink_aio-0.7.3/reolink_aio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-10 20:15:42.000000 reolink_aio-0.7.3/reolink_aio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-10 20:15:42.000000 reolink_aio-0.7.3/reolink_aio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-10 20:15:42.000000 reolink_aio-0.7.3/reolink_aio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-10 20:15:42.000000 reolink_aio-0.7.3/reolink_aio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-10 20:15:42.851384 reolink_aio-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1381 2023-07-10 20:15:26.000000 reolink_aio-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 20:15:42.851384 reolink_aio-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    15443 2023-07-10 20:15:26.000000 reolink_aio-0.7.3/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 20:03:29.029451 reolink_aio-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-07-27 20:03:18.000000 reolink_aio-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4720 2023-07-27 20:03:29.029451 reolink_aio-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3912 2023-07-27 20:03:18.000000 reolink_aio-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 20:03:29.025451 reolink_aio-0.7.4/reolink_aio/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-27 20:03:18.000000 reolink_aio-0.7.4/reolink_aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   194003 2023-07-27 20:03:18.000000 reolink_aio-0.7.4/reolink_aio/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-07-27 20:03:18.000000 reolink_aio-0.7.4/reolink_aio/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-07-27 20:03:18.000000 reolink_aio-0.7.4/reolink_aio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9403 2023-07-27 20:03:18.000000 reolink_aio-0.7.4/reolink_aio/software_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7935 2023-07-27 20:03:18.000000 reolink_aio-0.7.4/reolink_aio/templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15330 2023-07-27 20:03:18.000000 reolink_aio-0.7.4/reolink_aio/typings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-27 20:03:18.000000 reolink_aio-0.7.4/reolink_aio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 20:03:29.029451 reolink_aio-0.7.4/reolink_aio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4720 2023-07-27 20:03:29.000000 reolink_aio-0.7.4/reolink_aio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      439 2023-07-27 20:03:29.000000 reolink_aio-0.7.4/reolink_aio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 20:03:29.000000 reolink_aio-0.7.4/reolink_aio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 20:03:28.000000 reolink_aio-0.7.4/reolink_aio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-07-27 20:03:29.000000 reolink_aio-0.7.4/reolink_aio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-27 20:03:29.000000 reolink_aio-0.7.4/reolink_aio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-27 20:03:29.029451 reolink_aio-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-07-27 20:03:18.000000 reolink_aio-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 20:03:29.029451 reolink_aio-0.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    15443 2023-07-27 20:03:18.000000 reolink_aio-0.7.4/tests/test.py
```

### Comparing `reolink_aio-0.7.3/LICENSE` & `reolink_aio-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.3/PKG-INFO` & `reolink_aio-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reolink_aio
-Version: 0.7.3
+Version: 0.7.4
 Summary: Reolink NVR/cameras API package
 Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG
 Author-email: starkiller.og@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reolink_aio Version: 0.7.3 Summary: Reolink NVR/
+Metadata-Version: 2.1 Name: reolink_aio Version: 0.7.4 Summary: Reolink NVR/
 cameras API package Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG Author-email: starkiller.og@gmail.com License: MIT
 Platform: any Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier: Topic
 :: Software Development :: Libraries Classifier: Topic :: Home Automation
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `reolink_aio-0.7.3/README.md` & `reolink_aio-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.3/reolink_aio/api.py` & `reolink_aio-0.7.4/reolink_aio/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """ Reolink NVR/camera network API """
 from __future__ import annotations
 
 import asyncio
 import base64
 import hashlib
-import json
 import logging
 import ssl
 import traceback
 import uuid
 from datetime import datetime, timedelta, tzinfo
 from os.path import basename
 from typing import Any, Literal, Optional, overload
 from urllib import parse
 from xml.etree import ElementTree as XML
 from statistics import mean
 
+from orjson import JSONDecodeError, loads as json_loads  # pylint: disable=no-name-in-module
 import aiohttp
 
 from . import templates, typings
 from .enums import DayNightEnum, StatusLedEnum, SpotlightModeEnum, PtzEnum, GuardEnum, TrackMethodEnum, SubType
 from .exceptions import (
     ApiError,
     CredentialsInvalidError,
@@ -858,17 +858,19 @@
             self.clear_token()
             if not login_mutex_owned:
                 await self._aiohttp_session.close()
         finally:
             if not login_mutex_owned:
                 self._login_mutex.release()
 
-    async def expire_session(self):
+    async def expire_session(self, unsubscribe: bool = True):
         if self._lease_time is not None:
             self._lease_time = datetime.now() - timedelta(seconds=5)
+        if unsubscribe:
+            await self.unsubscribe()
         await self._aiohttp_session.close()
 
     def clear_token(self):
         self._token = None
         self._lease_time = None
 
     def construct_capabilities(self, warnings=True) -> None:
@@ -906,27 +908,27 @@
         # Channel capabilities
         for channel in self._channels:
             self._capabilities[channel] = []
 
             if self.is_nvr and self.api_version("supportAutoTrackStream", channel) > 0:
                 self._capabilities[channel].append("autotrack_stream")
 
-            if channel in self._ftp_settings:
+            if channel in self._ftp_settings and (self.api_version("GetFtp") < 1 or "scheduleEnable" in self._ftp_settings[channel]["Ftp"]):
                 self._capabilities[channel].append("ftp")
 
-            if channel in self._push_settings:
+            if channel in self._push_settings and (self.api_version("GetPush") < 1 or "scheduleEnable" in self._push_settings[channel]["Push"]):
                 self._capabilities[channel].append("push")
 
-            if channel in self._recording_settings:
+            if channel in self._recording_settings and (self.api_version("GetRec") < 1 or "scheduleEnable" in self._recording_settings[channel]["Rec"]):
                 self._capabilities[channel].append("recording")
 
-            if channel in self._email_settings:
+            if channel in self._email_settings and (self.api_version("GetEmail") < 1 or "scheduleEnable" in self._email_settings[channel]["Email"]):
                 self._capabilities[channel].append("email")
 
-            if self.api_version("supportBuzzer") > 0:
+            if self.api_version("supportBuzzer") > 0 and "scheduleEnable" in self._buzzer_settings[channel]["Buzzer"]:
                 self._capabilities[channel].append("buzzer")
 
             if self.api_version("ledControl", channel) > 0 and channel in self._ir_settings:
                 self._capabilities[channel].append("ir_lights")
 
             if self.api_version("powerLed", channel) > 0:
                 # powerLed == statusLed = doorbell_led
@@ -1031,15 +1033,15 @@
             if self.api_version("ispSharpen", channel) > 0:
                 self._capabilities[channel].append("isp_sharpen")
             if self.api_version("ispContrast", channel) > 0:
                 self._capabilities[channel].append("isp_contrast")
             if self.api_version("ispBright", channel) > 0:
                 self._capabilities[channel].append("isp_bright")
 
-            if self.api_version("ispDayNight", channel) > 0 and self.daynight_state(channel) is not None:
+            if self.api_version("ispDayNight", channel, no_key_return=1) > 0 and self.daynight_state(channel) is not None:
                 self._capabilities[channel].append("dayNight")
 
             if self.backlight_state(channel) is not None:
                 self._capabilities[channel].append("backLight")
 
     def supported(self, channel: int | None, capability: str) -> bool:
         """Return if a capability is supported by a camera channel."""
@@ -1047,26 +1049,26 @@
             return capability in self._capabilities["Host"]
 
         if channel not in self._capabilities:
             return False
 
         return capability in self._capabilities[channel]
 
-    def api_version(self, capability: str, channel: int | None = None) -> int:
+    def api_version(self, capability: str, channel: int | None = None, no_key_return: int = 0) -> int:
         """Return the api version of a capability, 0=not supported, >0 is supported"""
         if capability in self._api_version:
             return self._api_version[capability]
 
         if channel is None:
             return self._abilities.get(capability, {}).get("ver", 0)
 
         if channel >= len(self._abilities["abilityChn"]):
             return 0
 
-        return self._abilities["abilityChn"][channel].get(capability, {}).get("ver", 0)
+        return self._abilities["abilityChn"][channel].get(capability, {}).get("ver", no_key_return)
 
     async def get_state(self, cmd: str) -> None:
         body = []
         channels = []
         for channel in self._stream_channels:
             ch_body = []
             if cmd == "GetEnc":
@@ -1773,15 +1775,15 @@
         if response is None or response == b"":
             _LOGGER.error(
                 "Host: %s:%s: error obtaining still image response for channel %s.",
                 self._host,
                 self._port,
                 channel,
             )
-            await self.expire_session()
+            await self.expire_session(unsubscribe=False)
             return None
 
         return response
 
     def get_flv_stream_source(self, channel: int, stream: Optional[str] = None) -> Optional[str]:
         if channel not in self._stream_channels:
             return None
@@ -3678,26 +3680,26 @@
 
             if response.status >= 400 or (is_login_logout and response.status != 200):
                 response.release()
                 raise ApiError(f"API returned HTTP status ERROR code {response.status}/{response.reason}")
 
             if expected_response_type == "json" and isinstance(data, str):
                 try:
-                    json_data = json.loads(data)
-                except (TypeError, json.JSONDecodeError) as err:
+                    json_data = json_loads(data)
+                except (TypeError, JSONDecodeError) as err:
                     if retry <= 0:
                         raise InvalidContentTypeError(
                             f"Error translating JSON response: {str(err)}, from commands {[cmd.get('cmd') for cmd in body]}, "
                             f"content type '{response.content_type}', data:\n{data}\n"
                         ) from err
                     _LOGGER.debug("Error translating JSON response: %s, trying again, data:\n%s\n", str(err), data)
-                    await self.expire_session()
+                    await self.expire_session(unsubscribe=False)
                     return await self.send(body, param, expected_response_type, retry)
                 if json_data is None:
-                    await self.expire_session()
+                    await self.expire_session(unsubscribe=False)
                     raise NoDataError(f"Host {self._host}:{self._port}: returned no data: {data}")
                 return json_data
 
             if expected_response_type == "image/jpeg" and isinstance(data, bytes):
                 return data
 
             if expected_response_type == "text/html" and isinstance(data, str):
@@ -3706,35 +3708,45 @@
             if expected_response_type == "application/octet-stream":
                 # response needs to be read or released from the calling function
                 return response
 
             response.release()
             raise InvalidContentTypeError(f"Expected {expected_response_type}, unexpected data received: {data!r}")
         except aiohttp.ClientConnectorError as err:
-            await self.expire_session()
-            _LOGGER.error("Host %s:%s: connection error: %s", self._host, self._port, str(err))
-            raise ReolinkConnectionError(f"Host {self._host}:{self._port}: connection error: {str(err)}") from err
+            if retry <= 0:
+                await self.expire_session()
+                _LOGGER.error("Host %s:%s: connection error: %s", self._host, self._port, str(err))
+                raise ReolinkConnectionError(f"Host {self._host}:{self._port}: connection error: {str(err)}") from err
+            _LOGGER.debug("Host %s:%s: connection error, trying again: %s", self._host, self._port, str(err))
+            return await self.send(body, param, expected_response_type, retry)
         except asyncio.TimeoutError as err:
-            await self.expire_session()
-            _LOGGER.error(
-                "Host %s:%s: connection timeout exception. Please check the connection to this host.",
+            if retry <= 0:
+                await self.expire_session()
+                _LOGGER.error(
+                    "Host %s:%s: connection timeout exception. Please check the connection to this host.",
+                    self._host,
+                    self._port,
+                )
+                raise ReolinkTimeoutError(f"Host {self._host}:{self._port}: Timeout error: {str(err)}") from err
+            _LOGGER.debug(
+                "Host %s:%s: connection timeout exception, trying again.",
                 self._host,
                 self._port,
             )
-            raise ReolinkTimeoutError(f"Host {self._host}:{self._port}: Timeout error: {str(err)}") from err
+            return await self.send(body, param, expected_response_type, retry)
         except ApiError as err:
-            await self.expire_session()
+            await self.expire_session(unsubscribe=False)
             _LOGGER.error("Host %s:%s: API error: %s.", self._host, self._port, str(err))
             raise err
         except CredentialsInvalidError as err:
             await self.expire_session()
             _LOGGER.error("Host %s:%s: login attempt failed.", self._host, self._port)
             raise err
         except InvalidContentTypeError as err:
-            await self.expire_session()
+            await self.expire_session(unsubscribe=False)
             _LOGGER.debug("Host %s:%s: content type error: %s.", self._host, self._port, str(err))
             raise err
         except Exception as err:
             await self.expire_session()
             _LOGGER.error('Host %s:%s: unknown exception "%s" occurred, traceback:\n%s\n', self._host, self._port, str(err), traceback.format_exc())
             raise err
 
@@ -3767,16 +3779,16 @@
             data = await response.text()
         except aiohttp.ClientConnectorError as err:
             raise ReolinkConnectionError(f"Connetion error reading response from {URL}: {str(err)}") from err
         except asyncio.TimeoutError as err:
             raise ReolinkTimeoutError(f"Timeout reading response from {URL}: {str(err)}") from err
 
         try:
-            json_data = json.loads(data)
-        except (TypeError, json.JSONDecodeError) as err:
+            json_data = json_loads(data)
+        except (TypeError, JSONDecodeError) as err:
             raise InvalidContentTypeError(f"Error translating JSON response: {str(err)}, from {URL}, " f"content type '{response.content_type}', data:\n{data}\n") from err
 
         if json_data is None:
             raise NoDataError(f"Request to {URL} returned no data: {data}")
 
         resp_code = json_data.get("result", {}).get("code")
         if resp_code != 0:
```

### Comparing `reolink_aio-0.7.3/reolink_aio/enums.py` & `reolink_aio-0.7.4/reolink_aio/enums.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.3/reolink_aio/exceptions.py` & `reolink_aio-0.7.4/reolink_aio/exceptions.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.3/reolink_aio/software_version.py` & `reolink_aio-0.7.4/reolink_aio/software_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     "RLC-520A": {
         "IPC_523128M5MP": "v3.1.0.951_22041566",
     },
     "RLC-522": {
         "IPC_51516M5M": "v3.0.0.136_20121111",
     },
     "RLC-810A": {
-        "IPC_523128M8MP": "v3.1.0.956_22041503",
+        "IPC_523128M8MP": "v3.0.0.494_21073003",
     },
     "RLC-811A": {
         "IPC_523128M8MP": "v3.1.0.989_22051908",
     },
     "RLC-812A": {
         "IPC_523B188MP": "v3.1.0.920_22040613",
     },
```

### Comparing `reolink_aio-0.7.3/reolink_aio/templates.py` & `reolink_aio-0.7.4/reolink_aio/templates.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.3/reolink_aio/typings.py` & `reolink_aio-0.7.4/reolink_aio/typings.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.3/reolink_aio/utils.py` & `reolink_aio-0.7.4/reolink_aio/utils.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.3/reolink_aio.egg-info/PKG-INFO` & `reolink_aio-0.7.4/reolink_aio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reolink-aio
-Version: 0.7.3
+Version: 0.7.4
 Summary: Reolink NVR/cameras API package
 Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG
 Author-email: starkiller.og@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reolink-aio Version: 0.7.3 Summary: Reolink NVR/
+Metadata-Version: 2.1 Name: reolink-aio Version: 0.7.4 Summary: Reolink NVR/
 cameras API package Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG Author-email: starkiller.og@gmail.com License: MIT
 Platform: any Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier: Topic
 :: Software Development :: Libraries Classifier: Topic :: Home Automation
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `reolink_aio-0.7.3/setup.py` & `reolink_aio-0.7.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(name='reolink_aio',
-      version='0.7.3',
+      version='0.7.4',
       description='Reolink NVR/cameras API package',
       long_description=README,
       long_description_content_type="text/markdown",
       url='https://github.com/starkillerOG/reolink_aio',
       author='starkillerOG',
       author_email='starkiller.og@gmail.com',
       license='MIT',
       packages=find_packages(),
       python_requires='>=3.9',
       install_requires=[
         'ffmpeg',
         'requests',
-        'aiohttp'
+        'aiohttp',
+        'orjson'
         ],
       tests_require=[],
       platforms=['any'],
       zip_safe=False,
       classifiers=[
           "Development Status :: 5 - Production/Stable",
           "Intended Audience :: Developers",
```

### Comparing `reolink_aio-0.7.3/tests/test.py` & `reolink_aio-0.7.4/tests/test.py`

 * *Files identical despite different names*

