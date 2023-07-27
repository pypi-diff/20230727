# Comparing `tmp/pyhyypapihawkmod-1.1.6b20.tar.gz` & `tmp/pyhyypapihawkmod-1.1.7b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.1.6b20.tar", last modified: Wed Jul 26 19:21:49 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.1.7b1.tar", last modified: Thu Jul 27 14:24:31 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.1.6b20.tar` & `pyhyypapihawkmod-1.1.7b1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 19:21:49.462267 pyhyypapihawkmod-1.1.6b20/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b20/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b20/MANIFEST.in
--rw-rw-rw-   0        0        0      520 2023-07-26 19:21:49.461760 pyhyypapihawkmod-1.1.6b20/PKG-INFO
--rw-rw-rw-   0        0        0     1940 2023-07-26 19:12:58.000000 pyhyypapihawkmod-1.1.6b20/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 19:21:49.449089 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0     8641 2023-07-26 19:21:25.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    27868 2023-07-26 19:12:58.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4005 2023-07-26 19:12:58.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-07-26 19:21:49.460237 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      520 2023-07-26 19:21:49.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-07-26 19:21:49.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 19:21:49.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-26 19:21:49.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-26 19:21:49.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 19:21:49.462267 pyhyypapihawkmod-1.1.6b20/setup.cfg
--rw-rw-rw-   0        0        0      924 2023-07-26 19:21:30.000000 pyhyypapihawkmod-1.1.6b20/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:24:31.162703 pyhyypapihawkmod-1.1.7b1/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.7b1/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.7b1/MANIFEST.in
+-rw-rw-rw-   0        0        0      519 2023-07-27 14:24:31.161700 pyhyypapihawkmod-1.1.7b1/PKG-INFO
+-rw-rw-rw-   0        0        0     2169 2023-07-27 13:24:43.000000 pyhyypapihawkmod-1.1.7b1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 14:24:31.148793 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0    11035 2023-07-27 13:25:28.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    29480 2023-07-27 13:26:27.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4026 2023-07-27 13:23:03.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:24:31.159411 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      519 2023-07-27 14:24:31.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-07-27 14:24:31.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 14:24:31.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-27 14:24:31.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-27 14:24:31.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 14:24:31.163199 pyhyypapihawkmod-1.1.7b1/setup.cfg
+-rw-rw-rw-   0        0        0      923 2023-07-27 14:22:54.000000 pyhyypapihawkmod-1.1.7b1/setup.py
```

### Comparing `pyhyypapihawkmod-1.1.6b20/LICENSE.md` & `pyhyypapihawkmod-1.1.7b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b20/PKG-INFO` & `pyhyypapihawkmod-1.1.7b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.6b20
+Version: 1.1.7b1
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.6b20/README.md` & `pyhyypapihawkmod-1.1.7b1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -38,14 +38,22 @@
 ```
 print(json.dumps(client.get_sync_info(),indent=2))
 
 ```
 
 Changelog 
 
+1.1.7b1
+
+- Zones now show openviolated and tampered information from IDS server
+- Added delays between server requests to prevent blocking
+
+1.1.6-b3
+- Zones now show openviolated and tampered information from IDS server
+
 1.1.6-b1
 - Test version
 - Will now show zones as bypassed when a stay arm bypassing zones is activated.
 
 1.1.5
 - Added functions to supply notifications for debugging when specifically called.
```

### Comparing `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/alarm_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,60 @@
 """Alarm info for hass integration."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 from datetime import datetime
-from .constants import EventNumber
+import time
+from .constants import EventNumber, STD_PARAMS
+import logging
+
+_LOGGER = logging.getLogger(__name__)
+
 
 if TYPE_CHECKING:
     from .client import HyypClient
 
-
+SLEEP_DELAY = 0.5
 
 class HyypAlarmInfos:
     """Initialize Hyyp alarm objects."""
 
     def __init__(self, client: HyypClient) -> None:
         """init."""
         self._client = client
         self._sync_info: dict = {}
         self._state_info: dict = {}
         self._notifications: dict = {}
+        self._zone_state_info = []
         self._last_notification_check_timestamp = 0
 
     def _fetch_data(self) -> None:
         """Fetch data via client api."""
+        time.sleep(SLEEP_DELAY)
         self._sync_info = self._client.get_sync_info()
+        time.sleep(SLEEP_DELAY)
         self._state_info = self._client.get_state_info()
+        self._zone_state_info.clear()
+        for site in self._sync_info["sites"]:
+            siteid = site["id"]
+            time.sleep(SLEEP_DELAY)
+            entry = {siteid : self._client.get_zone_state_info(site_id=siteid)}
+            self._zone_state_info.append(entry)
+
+            
+        
+    def get_zone_state_info_for_site(self, site):
+        current_siteinfo = {}
+        for siteinfo in self._zone_state_info:
+            if site not in siteinfo:
+                continue
+            current_siteinfo = siteinfo[site]
+        return current_siteinfo
+            
+
         
     def _fetch_notifications(self, site_id: int) -> dict[Any,Any]:
         """Fetch and cache site notifications."""
         self._notifications = self._client.site_notifications(site_id=site_id)
 
 
     def _last_notice(self) -> dict[Any, Any]:
@@ -115,17 +141,20 @@
             trigger["id"]: trigger for trigger in self._sync_info["triggers"]
         }
         
         for site in site_ids:
             
             self._fetch_notifications(site_id=site)
             triggered_zones = self._triggered_zones()
+            zone_states = self.get_zone_state_info_for_site(site=site)
+
 
             # Add last site notification.
             _last_notice = self._last_notice()
+            site_ids[site]["update"] = str(datetime.fromtimestamp(time.time()))
             site_ids[site]["lastNoticeTime"] = _last_notice["lastNoticeTime"]
             site_ids[site]["lastNoticeName"] = _last_notice["lastNoticeName"]
 
             # Add triggers (PGM / Automations in APP)
             site_ids[site]["triggers"] = {}
             for trigger_id in trigger_ids:
                 if trigger_id not in site_ids[site]["triggerIds"]:
@@ -156,14 +185,31 @@
 
                 # Add zone bypass info to zone.
                 for zone in site_ids[site]["partitions"][partition]["zones"]:
                     site_ids[site]["partitions"][partition]["zones"][zone][
                         "bypassed"
                     ] = bool(zone in self._state_info["bypassedZoneIds"])
 
+
+
+                # New zone information from IDS servers
+                for zone in site_ids[site]["partitions"][partition]["zones"]:
+                    for zone_state in zone_states["zones"]:
+                        if site_ids[site]["partitions"][partition]["zones"][zone][
+                            "number"] != zone_state["number"]:
+                            continue
+                        site_ids[site]["partitions"][partition]["zones"][zone][
+                            "bypassed"] = bool(zone_state["bypassed"])
+                        site_ids[site]["partitions"][partition]["zones"][zone][
+                            "openviolated"] = bool(zone_state["openViolated"])
+                        site_ids[site]["partitions"][partition]["zones"][zone][
+                            "tampered"] = bool(zone_state["tampered"])
+                        site_ids[site]["partitions"][partition]["zones"][zone][
+                            "stay_bypassed"] = False
+
                 # Add zone trigger info to zone (Zone triggered alarm).
                 for zone in site_ids[site]["partitions"][partition]["zones"]:
                     site_ids[site]["partitions"][partition]["zones"][zone][
                         "triggered"
                     ] = bool(zone in triggered_zones)
 
 
@@ -193,19 +239,20 @@
                     site_ids[site]["partitions"][partition]["stayArmedProfileName"] = (
                         site_ids[site]["partitions"][partition]["stayProfiles"][
                             stay_profile]["name"]
                     )
                     
                     # Show zone as bypassed if stay partition has it bypassed                 
                     for zone in site_ids[site]["partitions"][partition]["zones"]:
+                        bypassed_due_to_stay = zone in site_ids[site]["partitions"][partition]["stayProfiles"][stay_profile]['zoneIds']
+                        site_ids[site]["partitions"][partition]["zones"][zone]["stay_bypassed"] = bypassed_due_to_stay
                         site_ids[site]["partitions"][partition]["zones"][zone][
                         "bypassed"
-                        ] = bool(site_ids[site]["partitions"][partition]["zones"][zone]["bypassed"] or 
-                                 zone in site_ids[site]["partitions"][partition]["stayProfiles"][stay_profile]['zoneIds']
-                                 )
+                        ] = bool(site_ids[site]["partitions"][partition]["zones"][zone]["bypassed"] or bypassed_due_to_stay)
+                        
 
         return site_ids
 
     def status(self) -> dict[Any, Any]:
         """Return the status of Hyyp connected alarms."""
 
         self._fetch_data()
@@ -215,16 +262,29 @@
 
 
 
     def debug_notifications(self) -> dict[Any, Any]:
         """Pull notifications for debug purposes."""
         # The API returns data from site level.
 
+        """
         self._fetch_data()
         site_ids = {site["id"]: site for site in self._sync_info["sites"]}
         
         for site in site_ids:
             self._fetch_notifications(site_id=site)
             site_ids[site] = self._notifications
 
 
         return site_ids
+        """
+
+
+        self._fetch_data()
+        fb = self.get_zone_state_info_for_site(108781)
+        message = {"rand" : "1147",
+                    "raw" : self._zone_state_info,
+                   "forsite" : fb
+                    }
+        
+        
+        return fb
```

### Comparing `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,34 +26,37 @@
 API_ENDPOINT_ARM_SITE = "/device/armSite"
 API_ENDPOINT_TRIGGER_ALARM = "/device/triggerAlarm"
 API_ENDPOINT_SET_ZONE_BYPASS = "/device/bypass"
 API_ENDPOINT_GET_CAMERA_BY_PARTITION = "/device/getCameraByPartition"
 API_ENDPOINT_UPDATE_SUB_USER = "/user/updateSubUser"
 API_ENDPOINT_SET_NOTIFICATION_SUBSCRIPTIONS = "/user/setNotificationSubscriptionsNew"
 API_ENDPOINT_TRIGGER_AUTOMATION = "/device/trigger"
+API_ENDPOINT_GET_ZONE_STATE_INFO = "/device/getZoneStateInfo"
 
 
 class HyypClient:
     """Initialize api client object."""
 
     def __init__(
         self,
         email: str | None = None,
         password: str | None = None,
         pkg: str = HyypPkg.ADT_SECURE_HOME.value,
         timeout: int = DEFAULT_TIMEOUT,
         token: str | None = None,
+        userid: int | None = None,
     ) -> None:
         """Initialize the client object."""
         self._email = email
         self._password = password
         self._session = requests.session()
         self._session.headers.update(REQUEST_HEADER)
         STD_PARAMS["pkg"] = pkg
         STD_PARAMS["token"] = token
+        STD_PARAMS["userId"] = userid
         self._timeout = timeout
 
     def login(self) -> Any:
         """Login to ADT Secure Home API."""
 
         _params = STD_PARAMS.copy()
         _params["email"] = self._email
@@ -86,14 +89,15 @@
                 + str(req.text)
             ) from err
 
         if _json_result["status"] != "SUCCESS" and _json_result["error"] is not None:
             raise HyypApiError(f"Login error: {_json_result['error']}")
 
         STD_PARAMS["token"] = _json_result["token"]
+        STD_PARAMS["userId"] = _json_result["user"]["id"]
 
         return _json_result
 
     def check_app_version(self) -> Any:
         """Check App version via API."""
 
         _params = STD_PARAMS.copy()
@@ -276,20 +280,62 @@
                 + str(req.text)
             ) from err
 
         if _json_result["status"] != "SUCCESS" and _json_result["error"] is not None:
             raise HyypApiError(
                 f"Error getting partition cameras from api: {_json_result['error']}"
             )
+        if json_key is None:
+            return _json_result
+
+        return _json_result[json_key]
+
+
+
+    def get_zone_state_info(self, site_id: int, json_key: str | None = None) -> Any:
+        """Get state info from API. Returns armed, bypassed partition ids."""
+
+        _params: dict[str, Any] = STD_PARAMS.copy()
+        _params["siteId"] = site_id
+        
+        try:
+            req = self._session.get(
+                "https://" + BASE_URL + API_ENDPOINT_GET_ZONE_STATE_INFO,
+                allow_redirects=False,
+                params=_params,
+                timeout=self._timeout,
+            )
+            req.raise_for_status()
+        except requests.ConnectionError as err:
+            raise InvalidURL("A Invalid URL or Proxy error occured") from err
+
+        except requests.HTTPError as err:
+            raise HTTPError from err    
+        try:
+            _json_result: dict[Any, Any] = req.json()
+
+        except ValueError as err:
+            raise HyypApiError(
+                "Impossible to decode response: "
+                + str(err)
+                + "\nResponse was: "
+                + str(req.text)
+            ) from err
+
+        if _json_result["status"] != "SUCCESS" and _json_result["error"] is not None:
+            raise HyypApiError(
+                f"Error getting zone state info from api: {_json_result['error']}"
+            )
 
         if json_key is None:
             return _json_result
 
         return _json_result[json_key]
 
+
     def get_sync_info(self, json_key: str | None = None) -> Any:
         """Get user, site, partition and users info from API."""
 
         _params = STD_PARAMS
 
         try:
             req = self._session.get(
@@ -820,15 +866,14 @@
         try:
             req = self._session.get(
                 "https://" + BASE_URL + API_ENDPOINT_SET_ZONE_BYPASS,
                 allow_redirects=False,
                 params=_params,
                 timeout=self._timeout,
             )
-
             req.raise_for_status()
 
         except requests.ConnectionError as err:
             raise InvalidURL("A Invalid URL or Proxy error occured") from err
 
         except requests.HTTPError as err:
             raise HTTPError from err
@@ -855,8 +900,8 @@
 
     def close_session(self) -> None:
         """Clear current session."""
         if self._session:
             self._session.close()
 
         self._session = requests.session()
-        self._session.headers.update(REQUEST_HEADER)  # Reset session.
+        self._session.headers.update(REQUEST_HEADER)  # Reset session.
```

### Comparing `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     "appVersionCode": "401",
     "_appVersionCode": "401",
     "deviceOS": "12.0",
     "deviceName": "Python API",
     "pkg": "za.co.adt.securehome.android",
     "_appVersionName": "3.5.19",
     "token": None,
+    "userId": None,
 }  # Standard request parameters.
 
 # Rpc to name mapping. Used in push notifications.
 RpcCodes = {
     "202": "IMEI unknown to SMART platform. Registration failed.",
     "203": "Command failed",
     "204": "VALUE is invalid",
```

### Comparing `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.6b20
+Version: 1.1.7b1
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b20/setup.py` & `pyhyypapihawkmod-1.1.7b1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.1.6b20",
+    version="1.1.7b1",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

