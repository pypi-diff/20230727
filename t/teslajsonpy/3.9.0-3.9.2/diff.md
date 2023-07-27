# Comparing `tmp/teslajsonpy-3.9.0.tar.gz` & `tmp/teslajsonpy-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teslajsonpy-3.9.0.tar", max compression
+gzip compressed data, was "teslajsonpy-3.9.2.tar", max compression
```

## Comparing `teslajsonpy-3.9.0.tar` & `teslajsonpy-3.9.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    24411 2023-06-12 02:53:08.822636 teslajsonpy-3.9.0/CHANGELOG.md
--rw-r--r--   0        0        0    11358 2023-06-12 02:52:26.086402 teslajsonpy-3.9.0/LICENSE
--rw-r--r--   0        0        0     2391 2023-06-12 02:52:26.086402 teslajsonpy-3.9.0/README.md
--rw-r--r--   0        0        0     1558 2023-06-12 02:53:08.838636 teslajsonpy-3.9.0/pyproject.toml
--rw-r--r--   0        0        0      916 2023-06-12 02:52:26.182402 teslajsonpy-3.9.0/teslajsonpy/__init__.py
--rw-r--r--   0        0        0      222 2023-06-12 02:53:08.838636 teslajsonpy-3.9.0/teslajsonpy/__version__.py
--rw-r--r--   0        0        0    48303 2023-06-12 02:52:26.182402 teslajsonpy-3.9.0/teslajsonpy/car.py
--rw-r--r--   0        0        0    25716 2023-06-12 02:52:26.182402 teslajsonpy-3.9.0/teslajsonpy/connection.py
--rw-r--r--   0        0        0     1377 2023-06-12 02:52:26.182402 teslajsonpy-3.9.0/teslajsonpy/const.py
--rw-r--r--   0        0        0    53186 2023-06-12 02:52:26.182402 teslajsonpy-3.9.0/teslajsonpy/controller.py
--rw-r--r--   0        0        0    53342 2023-06-12 02:52:26.182402 teslajsonpy-3.9.0/teslajsonpy/endpoints.json
--rw-r--r--   0        0        0     9422 2023-06-12 02:52:26.182402 teslajsonpy-3.9.0/teslajsonpy/energy.py
--rw-r--r--   0        0        0     3382 2023-06-12 02:52:26.182402 teslajsonpy-3.9.0/teslajsonpy/exceptions.py
--rw-r--r--   0        0        0     7696 2023-06-12 02:52:26.182402 teslajsonpy-3.9.0/teslajsonpy/teslaproxy.py
--rw-r--r--   0        0        0     3775 1970-01-01 00:00:00.000000 teslajsonpy-3.9.0/PKG-INFO
+-rw-r--r--   0        0        0   129986 2023-07-27 06:08:37.351061 teslajsonpy-3.9.2/CHANGELOG.md
+-rw-r--r--   0        0        0    11358 2023-07-27 06:08:37.351061 teslajsonpy-3.9.2/LICENSE
+-rw-r--r--   0        0        0     2391 2023-07-27 06:08:37.351061 teslajsonpy-3.9.2/README.md
+-rw-r--r--   0        0        0     1558 2023-07-27 06:09:08.018153 teslajsonpy-3.9.2/pyproject.toml
+-rw-r--r--   0        0        0      916 2023-07-27 06:08:37.435071 teslajsonpy-3.9.2/teslajsonpy/__init__.py
+-rw-r--r--   0        0        0      222 2023-07-27 06:09:08.018153 teslajsonpy-3.9.2/teslajsonpy/__version__.py
+-rw-r--r--   0        0        0    48321 2023-07-27 06:08:37.435071 teslajsonpy-3.9.2/teslajsonpy/car.py
+-rw-r--r--   0        0        0    25892 2023-07-27 06:08:37.435071 teslajsonpy-3.9.2/teslajsonpy/connection.py
+-rw-r--r--   0        0        0     1377 2023-07-27 06:08:37.435071 teslajsonpy-3.9.2/teslajsonpy/const.py
+-rw-r--r--   0        0        0    54173 2023-07-27 06:08:37.435071 teslajsonpy-3.9.2/teslajsonpy/controller.py
+-rw-r--r--   0        0        0    53342 2023-07-27 06:08:37.435071 teslajsonpy-3.9.2/teslajsonpy/endpoints.json
+-rw-r--r--   0        0        0     9454 2023-07-27 06:08:37.435071 teslajsonpy-3.9.2/teslajsonpy/energy.py
+-rw-r--r--   0        0        0     3867 2023-07-27 06:08:37.435071 teslajsonpy-3.9.2/teslajsonpy/exceptions.py
+-rw-r--r--   0        0        0     7696 2023-07-27 06:08:37.435071 teslajsonpy-3.9.2/teslajsonpy/teslaproxy.py
+-rw-r--r--   0        0        0     3775 1970-01-01 00:00:00.000000 teslajsonpy-3.9.2/PKG-INFO
```

### Comparing `teslajsonpy-3.9.0/LICENSE` & `teslajsonpy-3.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.9.0/README.md` & `teslajsonpy-3.9.2/README.md`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.9.0/pyproject.toml` & `teslajsonpy-3.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "teslajsonpy"
-version = "3.9.0"
+version = "3.9.2"
 description = "A library to work with Tesla API."
 authors = ["Sergey Isachenko <sergey.isachenkol@bool.by>"]
 license = "Apache-2.0"
 repository = "https://github.com/zabuldon/teslajsonpy"
 readme = "README.md"
 homepage = "https://github.com/zabuldon/teslajsonpy"
 documentation = "https://teslajsonpy.readthedocs.io"
```

### Comparing `teslajsonpy-3.9.0/teslajsonpy/__init__.py` & `teslajsonpy-3.9.2/teslajsonpy/__init__.py`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.9.0/teslajsonpy/car.py` & `teslajsonpy-3.9.2/teslajsonpy/car.py`

 * *Files 1% similar despite different names*

```diff
@@ -983,16 +983,15 @@
 
         Args
             enable: True to enable auto steering wheel heat, False to disable.
 
         """
 
         data = await self._send_command(
-            "REMOTE_AUTO_STEERING_WHEEL_HEAT_CLIMATE_REQUEST",
-            on=enable
+            "REMOTE_AUTO_STEERING_WHEEL_HEAT_CLIMATE_REQUEST", on=enable
         )
         if data and data["response"]["result"] is True:
             params = {"auto_steering_wheel_heat": enable}
             self._vehicle_data["climate_state"].update(params)
 
     async def set_heated_steering_wheel(self, value: bool) -> None:
         """Send command to set heated steering wheel."""
@@ -1013,15 +1012,17 @@
         if data and data["response"]["result"] is True:
             params = {"steering_wheel_heat_level": level}
             self._vehicle_data["climate_state"].update(params)
 
     def get_heated_steering_wheel_level(self) -> int:
         """Return the status of the heated steering wheel."""
         if self.data_available:
-            return self._vehicle_data.get("climate_state", {}).get("steering_wheel_heat_level")
+            return self._vehicle_data.get("climate_state", {}).get(
+                "steering_wheel_heat_level"
+            )
         return None
 
     async def set_hvac_mode(self, value: str) -> None:
         """Send command to set HVAC mode.
 
         Args
             value: on, off
```

### Comparing `teslajsonpy-3.9.0/teslajsonpy/connection.py` & `teslajsonpy-3.9.2/teslajsonpy/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,43 +184,46 @@
     ) -> None:
         """Open url."""
         headers = headers or {}
         cookies = cookies or {}
         if not baseurl:
             baseurl = self.baseurl
         url: URL = URL(baseurl).join(URL(url))
-
-        _LOGGER.debug("%s: %s %s", method, url, data)
+        debug = _LOGGER.isEnabledFor(logging.DEBUG)
+        if debug:
+            _LOGGER.debug("%s: %s %s", method, url, data)
 
         try:
             if data:
-                resp = await getattr(self.websession, method)(
+                resp: httpx.Response = await getattr(self.websession, method)(
                     str(url), json=data, headers=headers, cookies=cookies
                 )
             else:
-                resp = await getattr(self.websession, method)(
+                resp: httpx.Response = await getattr(self.websession, method)(
                     str(url), headers=headers, cookies=cookies
                 )
-            _LOGGER.debug("%s: %s", resp.status_code, resp.text)
+            if debug:
+                _LOGGER.debug("%s: %s", resp.status_code, resp.text)
             if resp.status_code > 299:
                 if resp.status_code == 401:
                     if data and data.get("error") == "invalid_token":
                         raise TeslaException(resp.status_code, "invalid_token")
                 elif resp.status_code == 408:
                     raise TeslaException(resp.status_code, "vehicle_unavailable")
                 raise TeslaException(resp.status_code)
-            data = orjson.loads(resp.text)  # pylint: disable=no-member
+            data = orjson.loads(resp.content)  # pylint: disable=no-member
             if data.get("error"):
                 # known errors:
                 #     'vehicle unavailable: {:error=>"vehicle unavailable:"}',
                 #     "upstream_timeout", "vehicle is curently in service"
-                _LOGGER.debug(
-                    "Raising exception for : %s",
-                    f'{data.get("error")}:{data.get("error_description")}',
-                )
+                if debug:
+                    _LOGGER.debug(
+                        "Raising exception for : %s",
+                        f'{data.get("error")}:{data.get("error_description")}',
+                    )
                 raise TeslaException(
                     f'{data.get("error")}:{data.get("error_description")}'
                 )
         except httpx.HTTPStatusError as exception_:
             raise TeslaException(exception_.request.status_code) from exception_
         return data
```

### Comparing `teslajsonpy-3.9.0/teslajsonpy/const.py` & `teslajsonpy-3.9.2/teslajsonpy/const.py`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.9.0/teslajsonpy/controller.py` & `teslajsonpy-3.9.2/teslajsonpy/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,20 @@
     RESOURCE_TYPE_SOLAR,
     SLEEP_INTERVAL,
     UPDATE_INTERVAL,
     WAKE_CHECK_INTERVAL,
     WAKE_TIMEOUT,
 )
 from teslajsonpy.energy import EnergySite, PowerwallSite, SolarPowerwallSite, SolarSite
-from teslajsonpy.exceptions import TeslaException, custom_retry, custom_wait
+from teslajsonpy.exceptions import (
+    TeslaException,
+    custom_retry,
+    custom_retry_except_unavailable,
+    custom_wait,
+)
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def valid_result(result):
     """Check if TeslaAPI result successful.
 
@@ -739,15 +744,19 @@
                 last_update = self._last_attempted_update_time
                 _LOGGER.debug(
                     "Get vehicles. Force: %s Time: %s Interval %s",
                     force,
                     cur_time - last_update,
                     ONLINE_INTERVAL,
                 )
-                if force or cur_time - last_update >= ONLINE_INTERVAL and update_vehicles:
+                if (
+                    force
+                    or cur_time - last_update >= ONLINE_INTERVAL
+                    and update_vehicles
+                ):
                     cars = await self.get_vehicles()
                     for car in cars:
                         self.set_id_vin(car_id=car["id"], vin=car["vin"])
                         self.set_vehicle_id_vin(
                             vehicle_id=car["vehicle_id"], vin=car["vin"]
                         )
                         self.set_car_online(
@@ -1329,18 +1338,42 @@
                 await self.wake_up(car_id=car_id)
                 response = await self.__post_with_retries(
                     "", method=method, data=kwargs, url=uri
                 )
             return response
 
         # Perform request using given keyword arguments as parameters
-        return await self.__post_with_retries("", method=method, data=kwargs, url=uri)
+        # wake_if_asleep is False so we do not retry if the car is asleep
+        # or if the car is unavailable
+        return await self.__post_with_retries_except_unavailable(
+            "", method=method, data=kwargs, url=uri
+        )
 
     @retry(
         wait=custom_wait,
         retry=custom_retry,
         stop=stop_after_delay(MAX_API_RETRY_TIME),
         reraise=True,
     )
     async def __post_with_retries(self, command, method="post", data=None, url=""):
-        """Call connection.post with retries for common exceptions."""
+        """Call connection.post with retries for common exceptions.
+
+        Retries if the car is unavailable.
+        """
+        return await self.__connection.post(command, method=method, data=data, url=url)
+
+    @retry(
+        wait=custom_wait,
+        retry=custom_retry_except_unavailable,
+        stop=stop_after_delay(MAX_API_RETRY_TIME),
+        reraise=True,
+    )
+    async def __post_with_retries_except_unavailable(
+        self, command, method="post", data=None, url=""
+    ):
+        """Call connection.post with retries for common exceptions.
+
+        Does not retry if the car is unavailable. This should be
+        used when wake_if_asleep is False since its unlikely the
+        car will suddenly become available if its offline/sleep.
+        """
         return await self.__connection.post(command, method=method, data=data, url=url)
```

### Comparing `teslajsonpy-3.9.0/teslajsonpy/endpoints.json` & `teslajsonpy-3.9.2/teslajsonpy/endpoints.json`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.9.0/teslajsonpy/energy.py` & `teslajsonpy-3.9.2/teslajsonpy/energy.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,25 +26,25 @@
     def energysite_id(self) -> int:
         """Return energy site id (aka site_id)."""
         return self._energysite.get("energy_site_id")
 
     @property
     def has_load_meter(self) -> bool:
         """Return True if energy site has a load meter."""
-        return self._energysite.get("components").get("load_meter")
+        return self._energysite.get("components", {}).get("load_meter")
 
     @property
     def has_battery(self) -> bool:
         """Return True if energy site has battery."""
-        return self._energysite.get("components").get("battery")
+        return self._energysite.get("components", {}).get("battery")
 
     @property
     def has_solar(self) -> bool:
         """Return True if energy site has solar."""
-        return self._energysite.get("components").get("solar")
+        return self._energysite.get("components", {}).get("solar")
 
     @property
     def id(self) -> str:
         # pylint: disable=invalid-name
         """Return battery_id."""
         return self._energysite.get("id")
 
@@ -104,15 +104,15 @@
     def solar_power(self) -> float:
         """Return solar power in Watts."""
         return self._site_data.get("solar_power")
 
     @property
     def solar_type(self) -> str:
         """Return type of solar (e.g. pv_panels or roof)."""
-        return self._energysite.get("components").get("solar_type")
+        return self._energysite.get("components", {}).get("solar_type")
 
 
 class PowerwallSite(EnergySite):
     """Represents a Tesla Energy Powerwall site.
 
     This class shouldn't be instantiated directly; it will be instantiated
     by :meth:`teslajsonpy.controller.generate_energysite_objects`.
@@ -130,15 +130,15 @@
         super().__init__(api, energysite, site_config)
         self._battery_data: dict = battery_data
         self._battery_summary: dict = battery_summary
 
     @property
     def backup_reserve_percent(self) -> int:
         """Return backup reserve percentage."""
-        return self._battery_data.get("backup").get("backup_reserve_percent")
+        return self._battery_data.get("backup", {}).get("backup_reserve_percent")
 
     @property
     def battery_power(self) -> float:
         """Return battery power in Watts."""
         if self._battery_data.get("power_reading"):
             return self._battery_data["power_reading"][0]["battery_power"]
         return None
@@ -234,30 +234,30 @@
     This class shouldn't be instantiated directly; it will be instantiated
     by :meth:`teslajsonpy.controller.generate_energysite_objects`.
     """
 
     @property
     def export_rule(self) -> str:
         """Return energy export rule setting."""
-        return self._battery_data.get("components").get(
+        return self._battery_data.get("components", {}).get(
             "customer_preferred_export_rule"
         )
 
     @property
     def grid_charging(self) -> bool:
         """Return grid charging."""
         # Key is missing from battery_data when False
-        return not self._battery_data.get("components").get(
+        return not self._battery_data.get("components", {}).get(
             "disallow_charge_from_grid_with_solar_installed", False
         )
 
     @property
     def solar_type(self) -> str:
         """Return type of solar (e.g. pv_panels or roof)."""
-        return self._battery_data.get("components").get("solar_type")
+        return self._battery_data.get("components", {}).get("solar_type")
 
     async def set_grid_charging(self, value: bool) -> None:
         """Set grid charging setting of Powerwall."""
         value = not value
         await self._send_command(
             "ENERGY_SITE_IMPORT_EXPORT_CONFIG",
             path_vars={"site_id": self.energysite_id},
```

### Comparing `teslajsonpy-3.9.0/teslajsonpy/exceptions.py` & `teslajsonpy-3.9.2/teslajsonpy/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -78,14 +78,33 @@
 
 class HomelinkError(TeslaException):
     """Class of exceptions for Homelink Error."""
 
     pass
 
 
+def custom_retry_except_unavailable(retry_state: RetryCallState) -> bool:
+    """Determine whether Tenacity should retry.
+
+    Args
+        retry_state (RetryCallState): Provided by Tenacity
+
+    Returns
+        bool: whether or not to retry
+
+    """
+    if not custom_retry(retry_state):
+        return False
+    ex = retry_state.outcome.exception()
+    if isinstance(ex, TeslaException):
+        if ex.code == 408:  # "VEHICLE_UNAVAILABLE"
+            return False
+    return True
+
+
 def custom_retry(retry_state: RetryCallState) -> bool:
     """Determine whether Tenacity should retry.
 
     Args
         retry_state (RetryCallState): Provided by Tenacity
 
     Returns
```

### Comparing `teslajsonpy-3.9.0/teslajsonpy/teslaproxy.py` & `teslajsonpy-3.9.2/teslajsonpy/teslaproxy.py`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.9.0/PKG-INFO` & `teslajsonpy-3.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teslajsonpy
-Version: 3.9.0
+Version: 3.9.2
 Summary: A library to work with Tesla API.
 Home-page: https://github.com/zabuldon/teslajsonpy
 License: Apache-2.0
 Author: Sergey Isachenko
 Author-email: sergey.isachenkol@bool.by
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```

